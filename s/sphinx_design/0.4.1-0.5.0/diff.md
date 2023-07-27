# Comparing `tmp/sphinx_design-0.4.1.tar.gz` & `tmp/sphinx_design-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_design-0.4.1.tar", last modified: Thu Apr 13 09:30:53 2023, max compression
+gzip compressed data, was "sphinx_design-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_design-0.4.1.tar` & `sphinx_design-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     2889 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2081 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/.gitignore
--rw-r--r--   0        0        0     1224 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      177 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/.readthedocs.yml
--rw-r--r--   0        0        0     7841 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     1099 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/LICENSE
--rw-r--r--   0        0        0     3114 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/README.md
--rw-r--r--   0        0        0      162 2023-04-13 09:30:50.514979 sphinx_design-0.4.1/codecov.yml
--rwxr-xr-x   0        0        0      214 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/git_rebase_theme_branches.sh
--rw-r--r--   0        0        0    11363 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/package-lock.json
--rw-r--r--   0        0        0      302 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/package.json
--rw-r--r--   0        0        0     2145 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      433 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/__init__.py
--rw-r--r--   0        0        0      722 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/_compat.py
--rw-r--r--   0        0        0     6410 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/article_info.py
--rw-r--r--   0        0        0     8252 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/badges_buttons.py
--rw-r--r--   0        0        0    10377 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/cards.py
--rw-r--r--   0        0        0        0 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/compiled/__init__.py
--rw-r--r--   0        0        0      577 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/compiled/material-icons_LICENSE
--rw-r--r--   0        0        0      106 2023-04-13 09:30:50.518979 sphinx_design-0.4.1/sphinx_design/compiled/material-icons_VERSION.txt
--rw-r--r--   0        0        0  1613646 2023-04-13 09:30:50.538980 sphinx_design-0.4.1/sphinx_design/compiled/material_outlined.json
--rw-r--r--   0        0        0  1504323 2023-04-13 09:30:50.538980 sphinx_design-0.4.1/sphinx_design/compiled/material_regular.json
--rw-r--r--   0        0        0  2003117 2023-04-13 09:30:50.546980 sphinx_design-0.4.1/sphinx_design/compiled/material_round.json
--rw-r--r--   0        0        0  1370513 2023-04-13 09:30:50.546980 sphinx_design-0.4.1/sphinx_design/compiled/material_sharp.json
--rw-r--r--   0        0        0  1995382 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/compiled/material_twotone.json
--rw-r--r--   0        0        0     1068 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/compiled/octicon_LICENSE
--rw-r--r--   0        0        0   277166 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/compiled/octicons.json
--rw-r--r--   0        0        0      770 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/compiled/sd_tabs.js
--rw-r--r--   0        0        0    48417 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/compiled/style.min.css
--rw-r--r--   0        0        0     7822 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/dropdown.py
--rw-r--r--   0        0        0     5614 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/extension.py
--rw-r--r--   0        0        0     9839 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/grids.py
--rw-r--r--   0        0        0    10620 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/icons.py
--rw-r--r--   0        0        0       26 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/py.typed
--rw-r--r--   0        0        0     3117 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/shared.py
--rw-r--r--   0        0        0     9681 2023-04-13 09:30:50.550980 sphinx_design-0.4.1/sphinx_design/tabs.py
--rw-r--r--   0        0        0     2103 2023-04-13 09:30:50.554980 sphinx_design-0.4.1/tox.ini
--rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 sphinx_design-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      600 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3132 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2081 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1224 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      177 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0     8257 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1099 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3114 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/README.md
+-rw-r--r--   0        0        0      162 2023-07-27 12:45:22.648600 sphinx_design-0.5.0/codecov.yml
+-rwxr-xr-x   0        0        0      214 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/git_rebase_theme_branches.sh
+-rw-r--r--   0        0        0    11363 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/package-lock.json
+-rw-r--r--   0        0        0      302 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/package.json
+-rw-r--r--   0        0        0     2078 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      433 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/__init__.py
+-rw-r--r--   0        0        0      722 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/_compat.py
+-rw-r--r--   0        0        0     6410 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/article_info.py
+-rw-r--r--   0        0        0     8252 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/badges_buttons.py
+-rw-r--r--   0        0        0    10377 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/cards.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/compiled/__init__.py
+-rw-r--r--   0        0        0      577 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/compiled/material-icons_LICENSE
+-rw-r--r--   0        0        0      106 2023-07-27 12:45:22.652600 sphinx_design-0.5.0/sphinx_design/compiled/material-icons_VERSION.txt
+-rw-r--r--   0        0        0  1613646 2023-07-27 12:45:22.668600 sphinx_design-0.5.0/sphinx_design/compiled/material_outlined.json
+-rw-r--r--   0        0        0  1504323 2023-07-27 12:45:22.672600 sphinx_design-0.5.0/sphinx_design/compiled/material_regular.json
+-rw-r--r--   0        0        0  2003117 2023-07-27 12:45:22.680601 sphinx_design-0.5.0/sphinx_design/compiled/material_round.json
+-rw-r--r--   0        0        0  1370513 2023-07-27 12:45:22.680601 sphinx_design-0.5.0/sphinx_design/compiled/material_sharp.json
+-rw-r--r--   0        0        0  1995382 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/compiled/material_twotone.json
+-rw-r--r--   0        0        0     1068 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/compiled/octicon_LICENSE
+-rw-r--r--   0        0        0   277166 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/compiled/octicons.json
+-rw-r--r--   0        0        0      770 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/compiled/sd_tabs.js
+-rw-r--r--   0        0        0    48417 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/compiled/style.min.css
+-rw-r--r--   0        0        0     7822 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/dropdown.py
+-rw-r--r--   0        0        0     5614 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/extension.py
+-rw-r--r--   0        0        0     9839 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/grids.py
+-rw-r--r--   0        0        0    10620 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/icons.py
+-rw-r--r--   0        0        0       26 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/py.typed
+-rw-r--r--   0        0        0     3117 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/shared.py
+-rw-r--r--   0        0        0     9681 2023-07-27 12:45:22.684601 sphinx_design-0.5.0/sphinx_design/tabs.py
+-rw-r--r--   0        0        0     2046 2023-07-27 12:45:22.688601 sphinx_design-0.5.0/tox.ini
+-rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 sphinx_design-0.5.0/PKG-INFO
```

### Comparing `sphinx_design-0.4.1/.github/workflows/ci.yml` & `sphinx_design-0.5.0/.github/workflows/ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -10,108 +10,115 @@
 jobs:
 
   pre-commit:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
-    - uses: pre-commit/action@v2.0.0
+    - uses: pre-commit/action@v3.0.0
 
   tests:
 
     strategy:
+      fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        sphinx-version: ["~=7.0"]
         include:
+        - os: ubuntu-latest
+          python-version: 3.8
+          sphinx-version: "~=5.0"
+        - os: ubuntu-latest
+          python-version: 3.8
+          sphinx-version: "~=6.0"
         - os: windows-latest
           python-version: 3.8
+          sphinx-version: "~=7.0"
 
     runs-on: ${{ matrix.os }}
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
+        cache: pip
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -e .[testing]
+        pip install --upgrade "sphinx${{ matrix.sphinx-version }}" -e .[testing]
     - name: Run pytest
       run: |
         pytest --cov=sphinx_design --cov-report=xml --cov-report=term-missing
     - name: Upload to Codecov
       if: matrix.python-version == '3.8' && matrix.os == 'ubuntu-latest'
-      uses: codecov/codecov-action@v1
+      uses: codecov/codecov-action@v3
       with:
         name: pytests
         flags: pytests
         file: ./coverage.xml
         fail_ci_if_error: true
 
-  tests-sphinx4:
-
-    strategy:
-      matrix:
-        os: [ubuntu-latest]
-        python-version: ["3.7", "3.10"]
-
-    runs-on: ${{ matrix.os }}
-
-    steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install -e .[testing] sphinx~=4.5
-    - name: Run pytest
-      run: pytest
-
   docs-build-format:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
         format: [html, latex, man]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.9
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: "3.9"
+        cache: pip
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[rtd]
     - name: Build documentation
       run: sphinx-build -nW --keep-going -b ${{ matrix.format }} docs/ docs/_build/${{ matrix.format }}
 
+  # https://github.com/marketplace/actions/alls-green#why
+  check:  # This job does nothing and is only used for the branch protection
+
+    if: always()
+
+    needs:
+    - pre-commit
+    - tests
+    - docs-build-format
+
+    runs-on: ubuntu-latest
+
+    steps:
+    - name: Decide whether the needed jobs succeeded or failed
+      uses: re-actors/alls-green@release/v1
+      with:
+        jobs: ${{ toJSON(needs) }}
+
   publish:
 
     name: Publish to PyPi
     needs: [pre-commit, tests]
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
     - name: install flit
       run: |
         pip install flit~=3.4
     - name: Build and publish
       run: |
```

### Comparing `sphinx_design-0.4.1/.gitignore` & `sphinx_design-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/.pre-commit-config.yaml` & `sphinx_design-0.5.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
     - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
     - id: black
 
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
     - id: flake8
       additional_dependencies: [flake8-bugbear~=22.7]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.4.1
     hooks:
     - id: mypy
       additional_dependencies: []
 
   - repo: local
     hooks:
     - id: css
```

### Comparing `sphinx_design-0.4.1/CHANGELOG.md` & `sphinx_design-0.5.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # Change Log
 
-## v0.4.0 - 2023-04-13
+## 0.5.0 - 2023-07-27
+
+## What's Changed
+
+* ⬆️ Drop Python 3.7 support, by [@chrisjsewell](https://github.com/chrisjsewell)) in [#146](https://github.com/executablebooks/sphinx-design/pull/146)
+* ⬆️ UPGRADE: sphinx>=5,<8, by [@chrisjsewell](https://github.com/chrisjsewell)) in [#148](https://github.com/executablebooks/sphinx-design/pull/148)
 
+**Full Changelog**: <https://github.com/executablebooks/sphinx-design/compare/v0.4.1...v0.5.0>
+
+## v0.4.0 - 2023-04-13
 
-([full changelog](https://github.com/executablebooks/sphinx-design/compare/v0.3.0...3d0db63f06a8f59a5ea1067e0f43782464eeff83))
+**Full Changelog**: <https://github.com/executablebooks/sphinx-design/compare/v0.3.0...v0.4.0>
 
 ### Enhancements made
 
 - Make default blue color a11y friendly. [#124](https://github.com/executablebooks/sphinx-design/pull/124) ([@feanil](https://github.com/feanil), [@choldgraf](https://github.com/choldgraf))
 - Make card titles translatable [#113](https://github.com/executablebooks/sphinx-design/pull/113) ([@jpmckinney](https://github.com/jpmckinney), [@chrisjsewell](https://github.com/chrisjsewell))
 
 ### Version upgrades
```

### Comparing `sphinx_design-0.4.1/LICENSE` & `sphinx_design-0.5.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MIT License Copyright (c) 2021 Chris Sewell
+MIT License Copyright (c) 2023 Chris Sewell
 
 Permission is hereby granted, free
 of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use, copy, modify, merge,
 publish, distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to the
```

### Comparing `sphinx_design-0.4.1/README.md` & `sphinx_design-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/package-lock.json` & `sphinx_design-0.5.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/pyproject.toml` & `sphinx_design-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,46 +11,45 @@
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: Markdown",
     "Topic :: Text Processing :: Markup :: reStructuredText",
 ]
 keywords = ["sphinx", "extension", "material design", "web components"]
-requires-python = ">=3.7"
-dependencies = ["sphinx>=4,<7"]
+requires-python = ">=3.8"
+dependencies = ["sphinx>=5,<8"]
 
 [project.urls]
 Homepage = "https://github.com/executablebooks/sphinx-design"
 Documentation = "https://sphinx-design.readthedocs.io"
 
 [project.optional-dependencies]
-code_style = ["pre-commit~=2.12"]
-rtd = ["myst-parser>=0.18.0,<2"]
+code_style = ["pre-commit>=3,<4"]
+rtd = ["myst-parser>=1,<3"]
 testing = [
-    "myst-parser>=0.18.0,<2",
+    "myst-parser>=1,<3",
     "pytest~=7.1",
     "pytest-cov",
     "pytest-regressions",
 ]
-theme_furo = ["furo>=2022.06.04,<2022.07"]
-theme_pydata = ["pydata-sphinx-theme~=0.9.0"]
+theme_furo = ["furo~=2023.7.0"]
+theme_pydata = ["pydata-sphinx-theme~=0.13.0"]
 theme_rtd = ["sphinx-rtd-theme~=1.0"]
-theme_sbt = ["sphinx-book-theme~=0.3.0"]
+theme_sbt = ["sphinx-book-theme~=1.0"]
 
 [tool.flit.sdist]
 exclude = [
     "docs/",
     "style/",
     "tests/",
 ]
```

### Comparing `sphinx_design-0.4.1/sphinx_design/_compat.py` & `sphinx_design-0.5.0/sphinx_design/_compat.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/article_info.py` & `sphinx_design-0.5.0/sphinx_design/article_info.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/badges_buttons.py` & `sphinx_design-0.5.0/sphinx_design/badges_buttons.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/cards.py` & `sphinx_design-0.5.0/sphinx_design/cards.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/compiled/material-icons_LICENSE` & `sphinx_design-0.5.0/sphinx_design/compiled/material-icons_LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/compiled/material_outlined.json` & `sphinx_design-0.5.0/sphinx_design/compiled/material_outlined.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/compiled/material_regular.json` & `sphinx_design-0.5.0/sphinx_design/compiled/material_regular.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/compiled/material_round.json` & `sphinx_design-0.5.0/sphinx_design/compiled/material_round.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/compiled/material_sharp.json` & `sphinx_design-0.5.0/sphinx_design/compiled/material_sharp.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/compiled/material_twotone.json` & `sphinx_design-0.5.0/sphinx_design/compiled/material_twotone.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/compiled/octicon_LICENSE` & `sphinx_design-0.5.0/sphinx_design/compiled/octicon_LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/compiled/octicons.json` & `sphinx_design-0.5.0/sphinx_design/compiled/octicons.json`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/compiled/sd_tabs.js` & `sphinx_design-0.5.0/sphinx_design/compiled/sd_tabs.js`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/compiled/style.min.css` & `sphinx_design-0.5.0/sphinx_design/compiled/style.min.css`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/dropdown.py` & `sphinx_design-0.5.0/sphinx_design/dropdown.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/extension.py` & `sphinx_design-0.5.0/sphinx_design/extension.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/grids.py` & `sphinx_design-0.5.0/sphinx_design/grids.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/icons.py` & `sphinx_design-0.5.0/sphinx_design/icons.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/shared.py` & `sphinx_design-0.5.0/sphinx_design/shared.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/sphinx_design/tabs.py` & `sphinx_design-0.5.0/sphinx_design/tabs.py`

 * *Files identical despite different names*

### Comparing `sphinx_design-0.4.1/tox.ini` & `sphinx_design-0.5.0/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,18 @@
 # run in parallel using `tox -p`
 [tox]
 envlist = py38
 
 [testenv]
 usedevelop = true
 
-[testenv:py{37,38,39,310}]
+[testenv:py{38,39,310,311}]
 description = Run unit tests with this Python version
 extras =
     testing
-deps =
-    black
-    flake8~=3.8
-    flake8-bugbear~=21.3
 commands = pytest {posargs}
 
 [testenv:docs-{update,clean}-{alabaster,rtd,pydata,sbt,furo}]
 description =
     clean: Run documentation build for this theme (removing existing builds)
     update: Run documentation build for this theme (reusing existing builds)
 extras =
```

### Comparing `sphinx_design-0.4.1/PKG-INFO` & `sphinx_design-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: sphinx_design
-Version: 0.4.1
+Version: 0.5.0
 Summary: A sphinx extension for designing beautiful, view size responsive web components.
 Keywords: sphinx,extension,material design,web components
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
-Requires-Dist: sphinx>=4,<7
-Requires-Dist: pre-commit~=2.12 ; extra == "code_style"
-Requires-Dist: myst-parser>=0.18.0,<2 ; extra == "rtd"
-Requires-Dist: myst-parser>=0.18.0,<2 ; extra == "testing"
+Requires-Dist: sphinx>=5,<8
+Requires-Dist: pre-commit>=3,<4 ; extra == "code_style"
+Requires-Dist: myst-parser>=1,<3 ; extra == "rtd"
+Requires-Dist: myst-parser>=1,<3 ; extra == "testing"
 Requires-Dist: pytest~=7.1 ; extra == "testing"
 Requires-Dist: pytest-cov ; extra == "testing"
 Requires-Dist: pytest-regressions ; extra == "testing"
-Requires-Dist: furo>=2022.06.04,<2022.07 ; extra == "theme_furo"
-Requires-Dist: pydata-sphinx-theme~=0.9.0 ; extra == "theme_pydata"
+Requires-Dist: furo~=2023.7.0 ; extra == "theme_furo"
+Requires-Dist: pydata-sphinx-theme~=0.13.0 ; extra == "theme_pydata"
 Requires-Dist: sphinx-rtd-theme~=1.0 ; extra == "theme_rtd"
-Requires-Dist: sphinx-book-theme~=0.3.0 ; extra == "theme_sbt"
+Requires-Dist: sphinx-book-theme~=1.0 ; extra == "theme_sbt"
 Project-URL: Documentation, https://sphinx-design.readthedocs.io
 Project-URL: Homepage, https://github.com/executablebooks/sphinx-design
 Provides-Extra: code_style
 Provides-Extra: rtd
 Provides-Extra: testing
 Provides-Extra: theme_furo
 Provides-Extra: theme_pydata
```

