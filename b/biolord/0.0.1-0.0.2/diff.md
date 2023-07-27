# Comparing `tmp/biolord-0.0.1.tar.gz` & `tmp/biolord-0.0.2.tar.gz`

## Comparing `biolord-0.0.1.tar` & `biolord-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 biolord-0.0.1/.bumpversion.cfg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 biolord-0.0.1/.codecov.yaml
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 biolord-0.0.1/.cruft.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 biolord-0.0.1/.editorconfig
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 biolord-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 biolord-0.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 biolord-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biolord-0.0.1/MANIFEST.in
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 biolord-0.0.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 biolord-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 biolord-0.0.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 biolord-0.0.1/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 biolord-0.0.1/.github/workflows/sync.yaml
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 biolord-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/Makefile
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/changelog.md
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/conf.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/index.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/make.bat
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/_static/.gitkeep
--rw-r--r--   0        0        0    64017 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/_static/img/dark_mode_logo.png
--rw-r--r--   0        0        0    46111 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/_static/img/light_mode_logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0   585343 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/tutorials/biolord_classify.ipynb
--rw-r--r--   0        0        0   719833 2020-02-02 00:00:00.000000 biolord-0.0.1/docs/tutorials/biolord_pipeline.ipynb
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 biolord-0.0.1/src/biolord/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 biolord-0.0.1/src/biolord/_constants.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 biolord-0.0.1/src/biolord/_data.py
--rw-r--r--   0        0        0    33551 2020-02-02 00:00:00.000000 biolord-0.0.1/src/biolord/_model.py
--rw-r--r--   0        0        0    34347 2020-02-02 00:00:00.000000 biolord-0.0.1/src/biolord/_module.py
--rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 biolord-0.0.1/src/biolord/_train.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 biolord-0.0.1/src/biolord/_utils.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 biolord-0.0.1/tests/test_basic.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 biolord-0.0.1/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 biolord-0.0.1/LICENSE
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 biolord-0.0.1/README.md
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 biolord-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 biolord-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 biolord-0.0.2/.bumpversion.cfg
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 biolord-0.0.2/.codecov.yaml
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 biolord-0.0.2/.cruft.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 biolord-0.0.2/.editorconfig
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 biolord-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 biolord-0.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 biolord-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biolord-0.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 biolord-0.0.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 biolord-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 biolord-0.0.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 biolord-0.0.2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 biolord-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/Makefile
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/changelog.md
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/conf.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/conf.py.rej
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/index.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/make.bat
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/_static/.gitkeep
+-rw-r--r--   0        0        0    64017 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/_static/img/dark_mode_logo.png
+-rw-r--r--   0        0        0    46111 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/_static/img/light_mode_logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/_templates/autosummary/class.rst.rej
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0   585439 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/tutorials/biolord_classify.ipynb
+-rw-r--r--   0        0        0   654827 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/tutorials/biolord_omics.ipynb
+-rw-r--r--   0        0        0   718676 2020-02-02 00:00:00.000000 biolord-0.0.2/docs/tutorials/biolord_pipeline.ipynb
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 biolord-0.0.2/src/biolord/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 biolord-0.0.2/src/biolord/_constants.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 biolord-0.0.2/src/biolord/_data.py
+-rw-r--r--   0        0        0    33603 2020-02-02 00:00:00.000000 biolord-0.0.2/src/biolord/_model.py
+-rw-r--r--   0        0        0    35333 2020-02-02 00:00:00.000000 biolord-0.0.2/src/biolord/_module.py
+-rw-r--r--   0        0        0    14523 2020-02-02 00:00:00.000000 biolord-0.0.2/src/biolord/_train.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 biolord-0.0.2/src/biolord/_utils.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 biolord-0.0.2/tests/test_basic.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 biolord-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 biolord-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 biolord-0.0.2/README.md
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 biolord-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 biolord-0.0.2/PKG-INFO
```

### Comparing `biolord-0.0.1/.cruft.json` & `biolord-0.0.2/.cruft.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'checkout'": "'v0.2.11'", "'commit'": "'03ef73af73ea4a927decc396232d9c2c5e958ee1'"}*

```diff
@@ -1,10 +1,10 @@
 {
-    "checkout": null,
-    "commit": "81157a80b6b71773ee499cc8b8053a3c1f5efb89",
+    "checkout": "v0.2.11",
+    "commit": "03ef73af73ea4a927decc396232d9c2c5e958ee1",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 ".github/workflows/**.yaml",
                 "docs/_templates/autosummary/**.rst"
             ],
             "_template": "https://github.com/scverse/cookiecutter-scverse",
```

### Comparing `biolord-0.0.1/.pre-commit-config.yaml` & `biolord-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `biolord-0.0.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `biolord-0.0.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `biolord-0.0.1/.github/workflows/build.yaml` & `biolord-0.0.2/.github/workflows/build.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 
 on:
     push:
         branches: [main]
     pull_request:
         branches: [main]
 
+concurrency:
+    group: ${{ github.workflow }}-${{ github.ref }}
+    cancel-in-progress: true
+
 jobs:
     package:
         runs-on: ubuntu-latest
         steps:
-            - uses: actions/checkout@v2
+            - uses: actions/checkout@v3
             - name: Set up Python 3.10
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v4
               with:
                   python-version: "3.10"
+                  cache: "pip"
+                  cache-dependency-path: "**/pyproject.toml"
             - name: Install build dependencies
               run: python -m pip install --upgrade pip wheel twine build
             - name: Build package
               run: python -m build
             - name: Check package
               run: twine check --strict dist/*.whl
```

### Comparing `biolord-0.0.1/.github/workflows/test.yaml` & `biolord-0.0.2/.github/workflows/test.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -2,49 +2,44 @@
 
 on:
     push:
         branches: [main]
     pull_request:
         branches: [main]
 
+concurrency:
+    group: ${{ github.workflow }}-${{ github.ref }}
+    cancel-in-progress: true
+
 jobs:
     test:
         runs-on: ${{ matrix.os }}
         defaults:
             run:
                 shell: bash -e {0} # -e to fail on error
 
         strategy:
             fail-fast: false
             matrix:
-                python: ["3.8", "3.10"]
+                python: ["3.8"]
                 os: [ubuntu-latest]
 
         env:
             OS: ${{ matrix.os }}
             PYTHON: ${{ matrix.python }}
 
         steps:
-            - uses: actions/checkout@v2
+            - uses: actions/checkout@v3
             - name: Set up Python ${{ matrix.python }}
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v4
               with:
                   python-version: ${{ matrix.python }}
+                  cache: "pip"
+                  cache-dependency-path: "**/pyproject.toml"
 
-            - name: Get pip cache dir
-              id: pip-cache-dir
-              run: |
-                  echo "::set-output name=dir::$(pip cache dir)"
-            - name: Restore pip cache
-              uses: actions/cache@v2
-              with:
-                  path: ${{ steps.pip-cache-dir.outputs.dir }}
-                  key: pip-${{ runner.os }}-${{ env.pythonLocation }}-${{ hashFiles('**/pyproject.toml') }}
-                  restore-keys: |
-                      pip-${{ runner.os }}-${{ env.pythonLocation }}-
             - name: Install test dependencies
               run: |
                   python -m pip install --upgrade pip wheel
                   pip install codecov
             - name: Install dependencies
               run: |
                   pip install ".[dev,test]"
```

### Comparing `biolord-0.0.1/docs/Makefile` & `biolord-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `biolord-0.0.1/docs/conf.py` & `biolord-0.0.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # -- Project information -----------------------------------------------------
 needs_sphinx = "5.0"
 templates_path = ["_templates"]
 
 info = metadata("biolord")
 project_name = info["Name"]
 author = info["Author"]
-copyright = f"{datetime.now():%Y}, {author}."
+copyright = f"{datetime.now():%Y}, {author}"
 version = info["Version"]
 release = info["Version"]
 
 source_suffix = {
     ".rst": "restructuredtext",
     ".ipynb": "myst-nb",
     ".myst": "myst-nb",
```

### Comparing `biolord-0.0.1/docs/make.bat` & `biolord-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `biolord-0.0.1/docs/_static/img/dark_mode_logo.png` & `biolord-0.0.2/docs/_static/img/dark_mode_logo.png`

 * *Files identical despite different names*

### Comparing `biolord-0.0.1/docs/_static/img/light_mode_logo.png` & `biolord-0.0.2/docs/_static/img/light_mode_logo.png`

 * *Files identical despite different names*

### Comparing `biolord-0.0.1/docs/_templates/autosummary/class.rst` & `biolord-0.0.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `biolord-0.0.1/docs/extensions/typed_returns.py` & `biolord-0.0.2/docs/extensions/typed_returns.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # code from https://github.com/theislab/scanpy/blob/master/docs/extensions/typed_returns.py
 # with some minor adjustment
+from __future__ import annotations
+
 import re
+from collections.abc import Generator, Iterable
 
 from sphinx.application import Sphinx
 from sphinx.ext.napoleon import NumpyDocstring
 
 
-def _process_return(lines):
+def _process_return(lines: Iterable[str]) -> Generator[str, None, None]:
     for line in lines:
-        m = re.fullmatch(r"(?P<param>\w+)\s+:\s+(?P<type>[\w.]+)", line)
-        if m:
-            # Once this is in scanpydoc, we can use the fancy hover stuff
+        if m := re.fullmatch(r"(?P<param>\w+)\s+:\s+(?P<type>[\w.]+)", line):
             yield f'-{m["param"]} (:class:`~{m["type"]}`)'
         else:
             yield line
 
 
-def _parse_returns_section(self, section):
-    lines_raw = list(_process_return(self._dedent(self._consume_to_next_section())))
-    lines = self._format_block(":returns: ", lines_raw)
+def _parse_returns_section(self: NumpyDocstring, section: str) -> list[str]:
+    lines_raw = self._dedent(self._consume_to_next_section())
+    if lines_raw[0] == ":":
+        del lines_raw[0]
+    lines = self._format_block(":returns: ", list(_process_return(lines_raw)))
     if lines and lines[-1]:
         lines.append("")
     return lines
 
 
 def setup(app: Sphinx):
     """Set app."""
```

### Comparing `biolord-0.0.1/docs/tutorials/biolord_classify.ipynb` & `biolord-0.0.2/docs/tutorials/biolord_classify.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997174784674785%*

 * *Differences: {"'cells'": '{11: {\'source\': {insert: [(1, \'    "decoder_width": 512,\\n\'), (2, \'    '*

 * *            '"decoder_depth": 4,\\n\'), (11, \'    "gene_likelihood": "normal",\\n\'), (12, \'    '*

 * *            '"loss_regression": "normal",\\n\')], delete: [12, 11, 2, 1]}}, 15: {\'source\': '*

 * *            '{insert: [(2, \'    "latent_lr": 1e-4,\\n\'), (3, \'    "latent_wd": 1e-4,\\n\'), (4, '*

 * *            '\'    "decoder_lr": 1e-4,\\n\'), (5, \'    "decoder_wd": 1e-4,\\n\')], delete: [3, '*

 * *            "2]}}, 16: {'s […]*

```diff
@@ -185,26 +185,26 @@
             "execution_count": 7,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "module_params = {\n",
-                "    \"autoencoder_width\": 512,\n",
-                "    \"autoencoder_depth\": 4,\n",
+                "    \"decoder_width\": 512,\n",
+                "    \"decoder_depth\": 4,\n",
                 "    \"attribute_nn_width\": 512,\n",
                 "    \"attribute_nn_depth\": 4,\n",
                 "    \"use_batch_norm\": False,\n",
                 "    \"use_layer_norm\": False,\n",
                 "    \"unknown_attribute_noise_param\": 1e-1,\n",
                 "    \"seed\": 42,\n",
                 "    \"n_latent_attribute_ordered\": 16,\n",
                 "    \"n_latent_attribute_categorical\": 4,\n",
-                "    \"loss_ae\": \"gauss\",\n",
-                "    \"loss_ordered_attribute\": \"gauss\",\n",
+                "    \"gene_likelihood\": \"normal\",\n",
+                "    \"loss_regression\": \"normal\",\n",
                 "    \"reconstruction_penalty\": 1e1,\n",
                 "    \"unknown_attribute_penalty\": 1e2,\n",
                 "    \"attribute_dropout_rate\": 0.05,\n",
                 "    \"eval_r2_ordered\": False,\n",
                 "    \"classifier_penalty\": 1e1,\n",
                 "    \"classification_penalty\": 0,\n",
                 "    \"classify_all\": False,\n",
@@ -260,16 +260,18 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "trainer_params = {\n",
                 "    \"n_epochs_warmup\": 0,\n",
-                "    \"autoencoder_lr\": 1e-4,\n",
-                "    \"autoencoder_wd\": 1e-4,\n",
+                "    \"latent_lr\": 1e-4,\n",
+                "    \"latent_wd\": 1e-4,\n",
+                "    \"decoder_lr\": 1e-4,\n",
+                "    \"decoder_wd\": 1e-4,\n",
                 "    \"attribute_nn_lr\": 1e-2,\n",
                 "    \"attribute_nn_wd\": 4e-8,\n",
                 "    \"step_size_lr\": 90,\n",
                 "    \"cosine_scheduler\": True,\n",
                 "    \"scheduler_final_lr\": 1e-5,\n",
                 "}"
             ]
@@ -307,14 +309,15 @@
                 "    max_epochs=200,\n",
                 "    batch_size=256,\n",
                 "    plan_kwargs=trainer_params,\n",
                 "    early_stopping=True,\n",
                 "    early_stopping_patience=20,\n",
                 "    check_val_every_n_epoch=10,\n",
                 "    num_workers=1,\n",
+                "    enable_checkpointing=False,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
```

### Comparing `biolord-0.0.1/docs/tutorials/biolord_pipeline.ipynb` & `biolord-0.0.2/docs/tutorials/biolord_pipeline.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986539964121613%*

 * *Differences: {"'cells'": '{4: {\'outputs\': [], \'source\': [\'adata = sc.read("adata_infected.h5ad", '*

 * *            'backup_url="https://figshare.com/ndownloader/files/39375713")\']}, 10: {\'source\': '*

 * *            '{insert: [(1, \'    "decoder_width": 1024,\\n\'), (2, \'    "decoder_depth": '*

 * *            '4,\\n\'), (6, \'    "gene_likelihood": "normal",\\n\')], delete: [7, 6, 2, 1]}}, 13: '*

 * *            '{\'source\': {insert: [(2, \'    "latent_lr": 1e-4,\\n\'), (3, \'    "latent_wd": '*

 * *            '1e-4,\\n\'), (4, \'  […]*

```diff
@@ -59,36 +59,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "tags": []
             },
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "AnnData object with n_obs \u00d7 n_vars = 19053 \u00d7 8203\n",
-                            "    obs: 'barcode', 'mouse', 'marker', 'time', 'infected', 'experiment', 'coarse_time', 'MB', 'eta', 'n_genes_by_counts', 'total_counts', 'total_counts_mt', 'pct_counts_mt', 'mt_qc', 'SUMPBA', 'n_counts', 'n_genes', 'mus_rRNA', 'pba_rRNA', 'pba_rRNA_fraction', 'nCount_PBA', 'nFeature_PBA', 'nCount_MUS', 'nFeature_MUS', 'RNA_snn_res.0.2', 'seurat_clusters', 'MBinfected', 'cluster_names', 'ident', 'eta_normalized', 'nCounts_tot', 'normalized_PBA', 'coarse_time_orig', 'zone', 'status', 'status_control', 'time_int', 'split_random'\n",
-                            "    var: 'org', 'highly_variable', 'highly_variable_rank', 'means', 'variances', 'variances_norm'\n",
-                            "    uns: 'coarse_time_colors', 'hvg', 'log1p', 'neighbors', 'pca', 'status_colors', 'status_control_colors', 'umap', 'zone_colors'\n",
-                            "    obsm: 'X_pca', 'X_umap'\n",
-                            "    varm: 'PCs'\n",
-                            "    layers: 'counts', 'logcounts', 'scaledata'\n",
-                            "    obsp: 'connectivities', 'distances'"
-                        ]
-                    },
-                    "execution_count": 3,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "adata = sc.read(\"adata_infected.h5ad\", backup_url=\"https://figshare.com/ndownloader/files/39375713\")\n",
-                "adata"
+                "adata = sc.read(\"adata_infected.h5ad\", backup_url=\"https://figshare.com/ndownloader/files/39375713\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "tags": []
@@ -169,21 +150,20 @@
             "execution_count": 6,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "module_params = {\n",
-                "    \"autoencoder_width\": 1024,\n",
-                "    \"autoencoder_depth\": 4,\n",
+                "    \"decoder_width\": 1024,\n",
+                "    \"decoder_depth\": 4,\n",
                 "    \"attribute_nn_width\": 512,\n",
                 "    \"attribute_nn_depth\": 2,\n",
                 "    \"n_latent_attribute_categorical\": 4,\n",
-                "    \"loss_ae\": \"gauss\",\n",
-                "    \"loss_ordered_attribute\": \"gauss\",\n",
+                "    \"gene_likelihood\": \"normal\",\n",
                 "    \"reconstruction_penalty\": 1e2,\n",
                 "    \"unknown_attribute_penalty\": 1e1,\n",
                 "    \"unknown_attribute_noise_param\": 1e-1,\n",
                 "    \"attribute_dropout_rate\": 0.1,\n",
                 "    \"use_batch_norm\": False,\n",
                 "    \"use_layer_norm\": False,\n",
                 "    \"seed\": 42,\n",
@@ -231,16 +211,18 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "trainer_params = {\n",
                 "    \"n_epochs_warmup\": 0,\n",
-                "    \"autoencoder_lr\": 1e-4,\n",
-                "    \"autoencoder_wd\": 1e-4,\n",
+                "    \"latent_lr\": 1e-4,\n",
+                "    \"latent_wd\": 1e-4,\n",
+                "    \"decoder_lr\": 1e-4,\n",
+                "    \"decoder_wd\": 1e-4,\n",
                 "    \"attribute_nn_lr\": 1e-2,\n",
                 "    \"attribute_nn_wd\": 4e-8,\n",
                 "    \"step_size_lr\": 45,\n",
                 "    \"cosine_scheduler\": True,\n",
                 "    \"scheduler_final_lr\": 1e-5,\n",
                 "}"
             ]
@@ -264,28 +246,29 @@
                         "SLURM auto-requeueing enabled. Setting signal handlers.\n"
                     ]
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Epoch 70/500:  14%|\u2588\u258d        | 70/500 [02:44<16:51,  2.35s/it, v_num=1, val_generative_mean_accuracy=0.964, val_generative_var_accuracy=0.776, val_biolord_metric=0.87, val_reconstruction_loss=18.8, val_unknown_attribute_penalty_loss=22, generative_mean_accuracy=0, generative_var_accuracy=0, biolord_metric=0, reconstruction_loss=18, unknown_attribute_penalty_loss=30.2]     \n",
+                        "Epoch 70/500:  14%|\u2588\u258d        | 70/500 [02:38<16:15,  2.27s/it, v_num=1, val_generative_mean_accuracy=0.964, val_generative_var_accuracy=0.776, val_biolord_metric=0.87, val_reconstruction_loss=18.8, val_unknown_attribute_penalty_loss=22, generative_mean_accuracy=0, generative_var_accuracy=0, biolord_metric=0, reconstruction_loss=18, unknown_attribute_penalty_loss=30.2]     \n",
                         "Monitored metric val_biolord_metric did not improve in the last 20 records. Best score: 0.874. Signaling Trainer to stop.\n"
                     ]
                 }
             ],
             "source": [
                 "model.train(\n",
                 "    max_epochs=500,\n",
                 "    batch_size=512,\n",
                 "    plan_kwargs=trainer_params,\n",
                 "    early_stopping=True,\n",
                 "    early_stopping_patience=20,\n",
                 "    check_val_every_n_epoch=10,\n",
                 "    num_workers=1,\n",
+                "    enable_checkpointing=False,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
@@ -392,43 +375,43 @@
                         "\u001b[34mINFO    \u001b[0m AnnData object appears to be a copy. Attempting to transfer setup.                                        \n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "1it [00:00,  4.80it/s]"
+                        "1it [00:00,  5.03it/s]"
                     ]
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u001b[34mINFO    \u001b[0m AnnData object appears to be a copy. Attempting to transfer setup.                                        \n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "2it [00:00,  4.11it/s]"
+                        "2it [00:00,  4.25it/s]"
                     ]
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u001b[34mINFO    \u001b[0m AnnData object appears to be a copy. Attempting to transfer setup.                                        \n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "3it [00:01,  2.51it/s]\n"
+                        "3it [00:01,  2.43it/s]\n"
                     ]
                 }
             ],
             "source": [
                 "adata_preds = model.compute_prediction_adata(\n",
                 "    adata, adata_source, target_attributes=[\"status_control\"], add_attributes=[\"zone\", \"eta_normalized\"]\n",
                 ")"
```

### Comparing `biolord-0.0.1/src/biolord/__init__.py` & `biolord-0.0.2/src/biolord/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from . import _utils as ul
 from ._model import Biolord
 from ._module import BiolordClassifyModule, BiolordModule
 
 __all__ = ["Biolord", "BiolordModule", "BiolordClassifyModule"]
 
 
 def _get_version() -> str:
```

### Comparing `biolord-0.0.1/src/biolord/_data.py` & `biolord-0.0.2/src/biolord/_data.py`

 * *Files identical despite different names*

### Comparing `biolord-0.0.1/src/biolord/_model.py` & `biolord-0.0.2/src/biolord/_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from ._train import biolordClassifyTrainingPlan, biolordTrainingPlan
 from ._utils import repeat_n
 
 logger = logging.getLogger(__name__)
 logger.propagate = False
 logging_dir = "./biolord_log/"
 
-
 __all__ = ["Biolord"]
 
 
 class Biolord(BaseModelClass):
     """The biolord model class.
 
     Parameters
@@ -46,15 +45,15 @@
         Annotated data object.
     model_name
         Name of the model.
     module_params
         Hyperparameters for the model's module initialization, e.g, :class:`~biolord.BiolordModule` or
         :class:`~biolord.BiolordClassifyModule`.
     n_latent
-        Number of latent dimensions used for the autoencoder.
+        Number of latent dimensions used for the latent embedding.
     train_classifiers
         Whether to activate a :class:`~biolord.BiolordClassifyModule`.
     split_key
         Key in :attr:`anndata.AnnData.obs` used to split the data between train, test and validation.
     train_split
         Value in :attr:`anndata.AnnData.obs` ``['{split_key}']`` marking the train set.
     valid_split
@@ -467,15 +466,15 @@
 
         return pred_adata_mean, pred_adata_var
 
     @torch.no_grad()
     def get_ordered_attribute_embedding(
         self,
         attribute_key: str,
-        vals: Optional[Union[float, str, np.ndarray]],
+        vals: Optional[Union[float, str, np.ndarray]] = None,
     ) -> np.ndarray:
         """Compute embedding of an ordered attribute.
 
         Parameters
         ----------
         attribute_key
             The key of the desired attribute.
@@ -709,15 +708,15 @@
             self,
             training_plan=self.training_plan,
             data_splitter=self.data_splitter,
             max_epochs=max_epochs,
             use_gpu=use_gpu,
             early_stopping_monitor=monitor,
             early_stopping_mode="max",
-            enable_checkpointing=True,
+            enable_checkpointing=enable_checkpointing,
             **trainer_kwargs,
         )
 
         return runner()
 
     @torch.no_grad()
     def evaluate_retrieval(
@@ -887,15 +886,15 @@
 
         start = 0
         obs_names_tmp = adata_preds.obs_names.values
         for key_, vals_ in predictions_dict.items():
             for ci, _ in enumerate(target_attributes):
                 adata_preds.obs.iloc[start : start + vals_.shape[0], ci] = key_[ci]
             obs_names_tmp[start : start + vals_.shape[0]] = [
-                obs_name + "_" + key_[0] for obs_name in adata_source.obs_names
+                obs_name + "_" + "_".join([str(k) for k in key_]) for obs_name in adata_source.obs_names
             ]
             start += vals_.shape[0]
 
         adata_preds.obs_names = obs_names_tmp
         for attribute_ in target_attributes:
             adata_preds.obs[attribute_] = adata_preds.obs[attribute_].astype("category")
```

### Comparing `biolord-0.0.1/src/biolord/_module.py` & `biolord-0.0.2/src/biolord/_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, List, Literal, Optional, Tuple
 
 import numpy as np
 import torch
 from scvi import REGISTRY_KEYS, settings
-from scvi.distributions import NegativeBinomial
+from scvi.distributions import NegativeBinomial, Poisson
 from scvi.module import Classifier
 from scvi.module.base import BaseModuleClass, auto_move_data
 from scvi.nn import Decoder, DecoderSCVI, FCLayers
 from sklearn.metrics import mean_squared_error, r2_score
 from torch import nn
 from torch.distributions import Categorical, Normal
 
@@ -20,31 +20,33 @@
     """Regularized embedding module."""
 
     def __init__(
         self,
         n_input: int,
         n_output: int,
         sigma: float,
+        embed: bool = True,
     ):
         super().__init__()
         self.embedding = nn.Embedding(
             num_embeddings=n_input,
             embedding_dim=n_output,
         )
-        self.sigma = sigma
+        self.sigma = sigma if embed else 0
+        self.embed = embed
 
     def forward(self, x):
         """Forward pass."""
         x_ = self.embedding(x)
         if self.training and self.sigma != 0:
             noise = torch.zeros_like(x_)
             noise.normal_(mean=0, std=self.sigma)
 
             x_ = x_ + noise
-
+        x_ = x_ * self.embed
         return x_
 
 
 class BiolordModule(BaseModuleClass):
     """The :mod:`biolord` module.
 
     Parameters
@@ -62,36 +64,40 @@
         as the categorical integer assignment.
     n_latent
         Latent dimension.
     n_latent_attribute_ordered
         Latent dimension of ordered attributes.
     n_latent_attribute_categorical
         Latent dimension of categorical attributes.
-    loss_ae
-        Autoencoder loss.
+    gene_likelihood
+        The gene_likelihood model.
     reconstruction_penalty
         MSE error to reconstruction loss.
-    loss_ordered_attribute
-        Autoencoder loss.
     use_batch_norm
         Use batch norm in layers.
     use_layer_norm
         Use layer norm in layers.
     unknown_attribute_noise_param
         Noise strength added to encoding of unknown attributes.
+    unknown_attributes
+        Whether to include learning for unknown attributes
     attribute_dropout_rate
         Dropout rate.
-    autoencoder_width
-        Autoencoder layers' width.
-    autoencoder_depth
-        Autoencoder number of layers.
     attribute_nn_width
         Ordered attributes autoencoder layers' width.
     attribute_nn_depth
         Ordered attributes autoencoder number of layers.
+    attribute_nn_activation
+        Use activation in ordered attributes.
+    decoder_width
+        Decoder layers' width.
+    decoder_depth
+        Decoder number of layers.
+    decoder_activation
+        Use activation in decoder.
     eval_r2_ordered
         Evaluate the R2 w.r.t. the ordered attribute. Set to `True` only if ordered attributes are binned.
     decoder_dropout_rate
         Decoder dropout rate.
     seed
         Random seed.
     """
@@ -102,53 +108,54 @@
         n_samples: int,
         x_loc: str,
         ordered_attributes_map: Optional[Dict[str, int]] = None,
         categorical_attributes_map: Optional[Dict[str, Dict]] = None,
         n_latent: int = 32,
         n_latent_attribute_categorical: int = 4,
         n_latent_attribute_ordered: int = 16,
-        loss_ae: Literal["gauss", "nb"] = "gauss",
+        gene_likelihood: Literal["normal", "nb", "poisson"] = "normal",
         reconstruction_penalty: float = 1e2,
         unknown_attribute_penalty: float = 1e1,
-        loss_ordered_attribute: Literal["gauss", "mse"] = "gauss",
         use_batch_norm: bool = True,
         use_layer_norm: bool = False,
         unknown_attribute_noise_param: float = 1e-1,
+        unknown_attributes: bool = True,
         attribute_dropout_rate: Dict[str, float] = None,
-        autoencoder_width: int = 512,
-        autoencoder_depth: int = 4,
+        decoder_width: int = 512,
+        decoder_depth: int = 4,
+        decoder_activation: bool = True,
         attribute_nn_width: Dict[str, int] = None,
         attribute_nn_depth: Dict[str, int] = None,
+        attribute_nn_activation: bool = True,
         eval_r2_ordered: bool = False,
         decoder_dropout_rate: float = 0.1,
         seed: int = 0,
     ):
         super().__init__()
-        loss_ae, loss_ordered_attribute = loss_ae.lower(), loss_ordered_attribute.lower()
-        assert loss_ae in ["gauss", "nb"], loss_ae
-        assert loss_ordered_attribute in ["gauss", "mse"], loss_ordered_attribute
+        gene_likelihood = gene_likelihood.lower()
+        assert gene_likelihood in ["normal", "nb", "poisson"], gene_likelihood
 
+        default_width = 256
+        default_depth = 2
         torch.manual_seed(seed)
         np.random.seed(seed)
         settings.seed = seed
 
         self.ae_loss_fn = nn.GaussianNLLLoss()
         self.ae_loss_mse_fn = nn.MSELoss()
         self.reconstruction_penalty = reconstruction_penalty
         self.unknown_attribute_penalty = unknown_attribute_penalty
-        self.regression_loss_fn = nn.MSELoss() if loss_ordered_attribute == "mse" else nn.GaussianNLLLoss()
         self.mm_regression_loss_fn = nn.BCEWithLogitsLoss()
 
         self.n_genes = n_genes
         self.n_latent = n_latent
         self.x_loc = x_loc
         self.n_latent_attribute_categorical = n_latent_attribute_categorical
         self.n_latent_attribute_ordered = n_latent_attribute_ordered
-        self.loss_ae = loss_ae
-        self.loss_ordered_class = loss_ordered_attribute
+        self.gene_likelihood = gene_likelihood
         self.use_batch_norm = use_batch_norm
         self.use_layer_norm = use_layer_norm
         self.eval_r2_ordered = eval_r2_ordered
 
         self.n_decoder_input = n_latent + (
             n_latent_attribute_categorical * len(categorical_attributes_map)
             + n_latent_attribute_ordered * len(ordered_attributes_map)
@@ -157,22 +164,22 @@
             categorical_attributes_map if isinstance(categorical_attributes_map, Dict) else {}
         )
         self.ordered_attributes_map = ordered_attributes_map if isinstance(ordered_attributes_map, Dict) else {}
 
         if isinstance(attribute_nn_width, Dict):
             self.attribute_nn_width = attribute_nn_width
         elif attribute_nn_width is None:
-            self.attribute_nn_width = {attribute_: autoencoder_width for attribute_ in self.ordered_attributes_map}
+            self.attribute_nn_width = {attribute_: default_width for attribute_ in self.ordered_attributes_map}
         else:
             self.attribute_nn_width = {attribute_: attribute_nn_width for attribute_ in self.ordered_attributes_map}
 
         if isinstance(attribute_nn_depth, Dict):
             self.attribute_nn_depth = attribute_nn_depth
         elif attribute_nn_depth is None:
-            self.attribute_nn_depth = {attribute_: autoencoder_depth for attribute_ in self.ordered_attributes_map}
+            self.attribute_nn_depth = {attribute_: default_depth for attribute_ in self.ordered_attributes_map}
         else:
             self.attribute_nn_depth = {attribute_: attribute_nn_depth for attribute_ in self.ordered_attributes_map}
 
         if isinstance(attribute_dropout_rate, Dict):
             self.attribute_dropout_rate = attribute_dropout_rate
         elif attribute_dropout_rate is None:
             self.attribute_dropout_rate = {
@@ -180,61 +187,72 @@
             }
         else:
             self.attribute_dropout_rate = {
                 attribute_: attribute_dropout_rate for attribute_ in self.ordered_attributes_map
             }
 
         self.latent_codes = RegularizedEmbedding(
-            n_input=n_samples, n_output=n_latent, sigma=unknown_attribute_noise_param
+            n_input=n_samples, n_output=n_latent, sigma=unknown_attribute_noise_param, embed=unknown_attributes
         )
 
         # Create Embeddings
         # 1. ordered classes
-        self.ordered_networks = nn.ModuleDict(
-            {
-                attribute_: FCLayers(
+        reps_ordered = []
+        self.ordered_networks = nn.ModuleDict()
+        for attribute_, len_ in self.ordered_attributes_map.items():
+            if "_rep" in attribute_:
+                reps_ordered.append(attribute_)
+            else:
+                self.ordered_networks[attribute_] = FCLayers(
                     n_in=len_,
                     n_out=self.n_latent_attribute_ordered,
                     n_layers=self.attribute_nn_depth[attribute_],
                     n_hidden=self.attribute_nn_width[attribute_],
                     dropout_rate=self.attribute_dropout_rate[attribute_],
                     bias=False,
+                    use_activation=attribute_nn_activation,
                 )
-                for attribute_, len_ in self.ordered_attributes_map.items()
-            }
-        )
+        for attribute_ in reps_ordered:
+            self.ordered_networks[attribute_] = self.ordered_networks[attribute_.split("_rep")[0]]
 
         # 2. categorical classes
         self.categorical_embeddings = nn.ModuleDict()
+        reps_categorical = []
         for attribute_, unique_categories in self.categorical_attributes_map.items():
-            self.categorical_embeddings[attribute_] = torch.nn.Embedding(
-                len(unique_categories),
-                n_latent_attribute_categorical,
-            )
+            if "_rep" in attribute_:
+                reps_categorical.append(attribute_)
+            else:
+                self.categorical_embeddings[attribute_] = torch.nn.Embedding(
+                    len(unique_categories),
+                    n_latent_attribute_categorical,
+                )
+        for attribute_ in reps_categorical:
+            self.categorical_embeddings[attribute_] = self.categorical_embeddings[attribute_.split("_rep")[0]]
 
         # Decoder components
-        if self.loss_ae == "nb":
+        if self.gene_likelihood in ["nb", "poisson"]:
             self.decoder = DecoderSCVI(
                 n_input=self.n_decoder_input,
                 n_output=n_genes,
-                n_hidden=autoencoder_width,
-                n_layers=autoencoder_depth,
+                n_hidden=decoder_width,
+                n_layers=decoder_depth,
                 use_batch_norm=use_batch_norm,
                 use_layer_norm=use_layer_norm,
                 scale_activation="softmax",
             )
             self.px_r = torch.nn.Parameter(torch.randn(n_genes))
         else:
             self.decoder = Decoder(
                 n_input=self.n_decoder_input,
                 n_output=n_genes,
-                n_hidden=autoencoder_width,
-                n_layers=autoencoder_depth,
+                n_hidden=decoder_width,
+                n_layers=decoder_depth,
                 use_batch_norm=use_batch_norm,
                 use_layer_norm=use_layer_norm,
+                use_activation=decoder_activation,
             )
 
     def _get_inference_input(self, tensors: Dict[Any, Any], **kwargs):
         x = tensors[self.x_loc]  # batch_size, n_genes
         sample_indices = tensors[REGISTRY_KEYS.INDICES_KEY].long().ravel()
 
         categorical_attribute_dict = {}
@@ -299,22 +317,20 @@
                 latent_i = torch.zeros_like(latent_i)
             inference_output[attribute_] = latent_i
 
         return inference_output
 
     def _get_latent_unknown_attributes(
         self,
-        genes,
         sample_indices,
     ):
         """Get the module's latent unknown attributes representation."""
         latent_unknown_attributes = self.latent_codes(sample_indices)
-        unknown_attributes_distribution = 0
 
-        return latent_unknown_attributes, unknown_attributes_distribution
+        return latent_unknown_attributes
 
     @auto_move_data
     def inference(
         self,
         genes: torch.Tensor,
         sample_indices: torch.Tensor,
         categorical_attribute_dict: Dict[Any, Any],
@@ -339,22 +355,17 @@
         Returns
         -------
         Dictionary with the module's expected input tensors (`genes`, `sample_indices`, `categorical_attribute_dict`, and `ordered_attribute_dict`).
         """
         nullify_attribute = [] if nullify_attribute is None else nullify_attribute
         inference_output = {}
         x_ = genes
-        library = None
-        if self.loss_ae == "nb":
-            library = torch.log(genes.sum(1)).unsqueeze(1)
-            x_ = torch.log(1 + x_)
+        library = torch.log(genes.sum(1)).unsqueeze(1)
 
-        latent_unknown_attributes, unknown_attributes_distribution = self._get_latent_unknown_attributes(
-            genes=x_, sample_indices=sample_indices
-        )
+        latent_unknown_attributes = self._get_latent_unknown_attributes(sample_indices=sample_indices)
 
         latent_classes = self._inference_attribute_embeddings(
             genes=x_,
             categorical_attribute_dict=categorical_attribute_dict,
             ordered_attribute_dict=ordered_attribute_dict,
             nullify_attribute=nullify_attribute,
         )
@@ -364,15 +375,14 @@
             latent_vecs.append(latent_.squeeze())
             inference_output[key_] = latent_.squeeze()
 
         latent = torch.cat(latent_vecs, dim=-1)
 
         inference_output["latent"] = latent
         inference_output["latent_unknown_attributes"] = latent_unknown_attributes
-        inference_output["unknown_attributes_distribution"] = unknown_attributes_distribution
         inference_output["library"] = library
 
         return inference_output
 
     def _get_generative_input(self, tensors, inference_outputs, **kwargs):
         input_dict = {
             "latent": inference_outputs["latent"],
@@ -395,29 +405,34 @@
         library
             Library sizes for each cell.
 
         Returns
         -------
         Dictionary with the generative predictions of the expression distribution.
         """
-        if self.loss_ae == "nb":
+        if self.gene_likelihood in ["nb", "poisson"]:
             px_scale, _, px_rate, _ = self.decoder(
                 dispersion="gene",
                 z=latent,
                 library=library,
             )
             px_r = torch.exp(self.px_r)
-            px = NegativeBinomial(mu=px_rate, theta=px_r, scale=px_scale)
+            px = (
+                NegativeBinomial(mu=px_rate, theta=px_r, scale=px_scale)
+                if self.gene_likelihood == "nb"
+                else Poisson(px_rate)
+            )  # , scale=px_scale)
 
             return {
                 "means": px.mean,
                 "variances": px.variance,
                 "distribution": px,
                 "samples": px.sample().squeeze(0),
             }
+
         else:
             p_m, p_v = self.decoder(x=latent)
             px = Normal(loc=p_m, scale=p_v.sqrt())
             return {
                 "means": px.loc,
                 "variances": px.variance,
                 "distribution": px,
@@ -443,24 +458,24 @@
             Generative step outputs.
 
         Returns
         -------
         The loss elements.
         """
         x_ = tensors[self.x_loc]
+        means = generative_outputs["means"]
+        variances = generative_outputs["variances"]
 
-        if self.loss_ae == "nb":
-            reconstruction_loss = -generative_outputs["distribution"].log_prob(x_).mean(-1)
+        if self.gene_likelihood in ["nb", "poisson"]:
+            reconstruction_loss = -generative_outputs["distribution"].log_prob(x_).sum(-1)
             reconstruction_loss = reconstruction_loss.mean()
         else:
-            means = generative_outputs["means"]
-            variances = generative_outputs["variances"]
-            reconstruction_loss = self.ae_loss_fn(
-                input=means, target=x_, var=variances
-            ) + self.reconstruction_penalty * self.ae_loss_mse_fn(input=means, target=x_)
+            reconstruction_loss = self.ae_loss_fn(input=means, target=x_, var=variances)
+
+        reconstruction_loss += self.reconstruction_penalty * self.ae_loss_mse_fn(input=means, target=x_)
 
         unknown_attribute_penalty_loss_val = self.unknown_attribute_penalty_loss(
             inference_outputs["latent_unknown_attributes"]
         )
 
         return {
             LOSS_KEYS.RECONSTRUCTION: reconstruction_loss,
@@ -537,15 +552,17 @@
                 variances_index = pred_x_var[index_mask]
 
                 true_mean_index = np.nanmean(x_index, axis=0)
                 pred_mean_index = np.nanmean(means_index, axis=0)
 
                 true_var_index = np.nanvar(x_index, axis=0)
                 pred_var_index = (
-                    np.nanvar(means_index, axis=0) if self.loss_ae == "nb" else np.nanmean(variances_index, axis=0)
+                    np.nanvar(means_index, axis=0)
+                    if self.gene_likelihood in ["nb", "poisson"]
+                    else np.nanmean(variances_index, axis=0)
                 )
 
                 r2_mean += r2_score(true_mean_index, pred_mean_index)
                 r2_var += r2_score(true_var_index, pred_var_index)
                 k += 1
             else:
                 continue
@@ -602,14 +619,16 @@
         Classification penalty strength.
     classifier_nn_width
         Classifier's layer width.
     classifier_nn_depth
         Classifier's number of layers.
     classifier_dropout_rate
         Classifier's dropout rate.
+    loss_regression
+        Loss function for regressors
     kwargs
         Keyword arguments for :class:`~biolord.BiolordModule`.
     """
 
     def __init__(
         self,
         categorical_attributes_missing: Optional[Dict[str, str]] = None,
@@ -617,24 +636,29 @@
         logits: bool = False,
         bias: bool = True,
         classification_penalty: float = 1e-1,
         classifier_penalty: float = 1e-4,
         classifier_nn_width: int = 128,
         classifier_nn_depth: int = 2,
         classifier_dropout_rate: float = 1e-1,
+        loss_regression: Literal["normal", "mse"] = "normal",
         **kwargs: Any,
     ):
         super().__init__(**kwargs)
 
+        loss_regression = loss_regression.lower()
+        assert loss_regression in ["normal", "mse"], loss_regression
+
         self.ae_loss_fn = nn.GaussianNLLLoss()
         self.ae_loss_mse_fn = nn.MSELoss()
         self.classification_penalty = classification_penalty
         self.classifier_penalty = classifier_penalty
         self.classification_loss_fn = nn.CrossEntropyLoss()
-        self.regression_loss_fn = nn.MSELoss() if self.loss_ordered_class == "mse" else nn.GaussianNLLLoss()
+        self.regression_loss_fn = nn.MSELoss() if loss_regression == "mse" else nn.GaussianNLLLoss()
+        self.loss_regression = "mse"
         self.mm_regression_loss_fn = nn.BCEWithLogitsLoss()
         self.classify_all = classify_all
 
         if isinstance(categorical_attributes_missing, Dict):
             self.categorical_attributes_missing = categorical_attributes_missing
         elif categorical_attributes_missing is None:
             self.categorical_attributes_missing = {attribute_: None for attribute_ in self.categorical_attributes_map}
@@ -658,15 +682,15 @@
                     len(unique_categories),
                     self.n_latent_attribute_categorical,
                 )
 
         # Create classifiers
         self.ordered_regressors = nn.ModuleDict()
         if self.classify_all:
-            if self.loss_ordered_class == "mse":
+            if self.loss_regression == "mse":
                 self.ordered_regressors = nn.ModuleDict(
                     {
                         attribute_: nn.Linear(
                             in_features=self.n_genes,
                             out_features=len_,
                             bias=bias,
                         )
@@ -675,16 +699,16 @@
                 )
             else:
                 self.ordered_regressors = nn.ModuleDict(
                     {
                         attribute_: Decoder(
                             n_input=self.n_genes,
                             n_output=len_,
-                            n_hidden=self.autoencoder_width,
-                            n_layers=self.autoencoder_depth,
+                            n_hidden=classifier_nn_width,
+                            n_layers=classifier_nn_depth,
                             use_batch_norm=self.use_batch_norm,
                             use_layer_norm=self.use_layer_norm,
                         )
                         for attribute_, len_ in self.ordered_attributes_map.items()
                     }
                 )
 
@@ -795,15 +819,15 @@
                     classification[attribute_],
                     attribute_vals,
                 )
 
         for attribute_, len_ in self.ordered_attributes_map.items():
             if attribute_ in classification:
                 if len_ > 1:
-                    if self.loss_ordered_class == "mse":
+                    if self.loss_regression == "mse":
                         classification_loss += self.regression_loss_fn(
                             classification[attribute_], tensors[attribute_].float()
                         ) + self.classification_penalty * self.mm_regression_loss_fn(
                             classification[attribute_], tensors[attribute_].gt(0).float()
                         )
                     else:
                         classification_loss += self.regression_loss_fn(
@@ -879,15 +903,15 @@
                     accuracy_val += accuracy_dict[attribute_]
             else:
                 accuracy_dict[attribute_] = np.mean(attribute_vals_pred == attribute_vals)
                 accuracy_val += accuracy_dict[attribute_]
 
         for attribute_ in self.ordered_regressors:
             attribute_vals_pred = (
-                classification[attribute_] if self.loss_ordered_class == "mse" else classification[attribute_][0]
+                classification[attribute_] if self.regression_loss == "mse" else classification[attribute_][0]
             )
             attribute_vals = tensors[attribute_].cpu().numpy()
             attribute_vals_pred = (
                 torch.nan_to_num(attribute_vals_pred, nan=0, neginf=0, posinf=100).detach().cpu().numpy()
             )
 
             r2_dict[attribute_] = r2_score(attribute_vals, attribute_vals_pred) if attribute_vals.shape[0] > 2 else 0
```

### Comparing `biolord-0.0.1/src/biolord/_train.py` & `biolord-0.0.2/src/biolord/_train.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,56 +16,61 @@
     def __init__(
         self,
         module: BiolordModule,
         n_steps_kl_warmup: Union[int, None] = None,
         n_epochs_kl_warmup: Union[int, None] = None,
         n_epochs_warmup: Union[int, None] = None,
         checkpoint_freq: int = 20,
-        autoencoder_lr=1e-4,
-        autoencoder_wd=1e-4,
+        latent_lr=1e-4,
+        latent_wd=1e-4,
+        decoder_lr=1e-4,
+        decoder_wd=1e-4,
         step_size_lr: int = 45,
         batch_size: int = 256,
         cosine_scheduler: bool = False,
         scheduler_max_epochs: int = 1000,
         scheduler_final_lr: float = 1e-5,
         attribute_nn_lr: Dict[str, float] = None,
         attribute_nn_wd: Dict[str, float] = None,
     ):
         super().__init__(
             module=module,
-            lr=autoencoder_lr,
-            weight_decay=autoencoder_wd,
+            lr=latent_lr,
+            weight_decay=latent_wd,
             n_steps_kl_warmup=n_steps_kl_warmup,
             n_epochs_kl_warmup=n_epochs_kl_warmup,
             reduce_lr_on_plateau=False,
             lr_factor=None,
             lr_patience=None,
             lr_threshold=None,
             lr_scheduler_metric=None,
             lr_min=None,
         )
 
         if isinstance(attribute_nn_lr, Dict):
             self.attribute_nn_lr = attribute_nn_lr
         elif attribute_nn_lr is None:
-            self.attribute_nn_lr = {attribute_: self.autoencoder_lr for attribute_ in self.module.ordered_networks}
+            self.attribute_nn_lr = {attribute_: self.latent_lr for attribute_ in self.module.ordered_networks}
         else:
             self.attribute_nn_lr = {attribute_: attribute_nn_lr for attribute_ in self.module.ordered_networks}
 
         if isinstance(attribute_nn_wd, Dict):
             self.attribute_nn_wd = attribute_nn_wd
         elif attribute_nn_wd is None:
-            self.attribute_nn_wd = {attribute_: self.autoencoder_wd for attribute_ in self.module.ordered_networks}
+            self.attribute_nn_wd = {attribute_: self.latent_wd for attribute_ in self.module.ordered_networks}
         else:
             self.attribute_nn_wd = {attribute_: attribute_nn_wd for attribute_ in self.module.ordered_networks}
 
         self.n_epochs_warmup = n_epochs_warmup if n_epochs_warmup is not None else 0
 
-        self.autoencoder_wd = autoencoder_wd
-        self.autoencoder_lr = autoencoder_lr
+        self.decoder_wd = decoder_wd
+        self.decoder_lr = decoder_lr
+
+        self.latent_wd = latent_wd
+        self.latent_lr = latent_lr
 
         self.checkpoint_freq = checkpoint_freq
 
         self.scheduler = CosineAnnealingLR if cosine_scheduler else StepLR
         self.scheduler_params = (
             {"T_max": scheduler_max_epochs, "eta_min": scheduler_final_lr}
             if cosine_scheduler
@@ -73,14 +78,16 @@
         )
 
         self.step_size_lr = step_size_lr
         self.batch_size = batch_size
 
         self.automatic_optimization = False
         self.iter_count = 0
+        self.training_step_outputs = []
+        self.validation_step_outputs = []
         self._epoch_keys = []
 
         self.epoch_keys = [
             "generative_mean_accuracy",  # accuracy in prediction of mean gene exp.
             "generative_var_accuracy",  # accuracy in prediction of variance of gene exp.
             "biolord_metric",  # combination of metrics above
             LOSS_KEYS.RECONSTRUCTION,
@@ -103,16 +110,16 @@
                     {
                         "params": list(
                             filter(
                                 lambda p: p.requires_grad,
                                 self.module.latent_codes.parameters(),
                             )
                         ),
-                        "lr": self.autoencoder_lr,
-                        "weight_decay": self.autoencoder_wd,
+                        "lr": self.latent_lr,
+                        "weight_decay": self.latent_wd,
                         # betas=(0.5, 0.999),
                     }
                 ]
             )
         )
         # latent decoder
         optimizers.append(
@@ -121,16 +128,16 @@
                     {
                         "params": list(
                             filter(
                                 lambda p: p.requires_grad,
                                 self.module.decoder.parameters(),
                             )
                         ),
-                        "lr": self.autoencoder_lr,
-                        "weight_decay": self.autoencoder_wd,
+                        "lr": self.decoder_lr,
+                        "weight_decay": self.decoder_wd,
                     }
                 ]
             )
         )
         # categorical classes
         optimizers.append(
             torch.optim.Adam(
@@ -138,16 +145,16 @@
                     {
                         "params": list(
                             filter(
                                 lambda p: p.requires_grad,
                                 self.module.categorical_embeddings.parameters(),
                             )
                         ),
-                        "lr": self.autoencoder_lr,
-                        "weight_decay": self.autoencoder_wd,
+                        "lr": self.latent_lr,
+                        "weight_decay": self.latent_wd,
                     }
                 ]
             )
         )
         # ordered classes
         for attribute_, nn_ in self.module.ordered_networks.items():
             params_class = list(filter(lambda p: p.requires_grad, nn_.parameters()))
@@ -207,54 +214,62 @@
 
         self.iter_count += 1
 
         for key in self.epoch_keys:
             if key not in results:
                 results.update({key: 0.0})
 
+        self.training_step_outputs.append(results)
         return results
 
-    def training_epoch_end(self, outputs):
+    def on_train_epoch_end(self):
         """Training epoch end."""
+        outputs = self.training_step_outputs
         self.epoch_history["epoch"].append(self.current_epoch)
         self.epoch_history["mode"].append("train")
 
         for key in self.epoch_keys:
             self.epoch_history[key].append(np.mean([output[key] for output in outputs]))
             self.log(key, self.epoch_history[key][-1], prog_bar=True)
 
         if self.current_epoch > 1 and self.current_epoch % self.step_size_lr == 0:
             schedulers = self.lr_schedulers()
             for scheduler in schedulers:
                 scheduler.step()
 
+        self.training_step_outputs.clear()
+
     def validation_step(self, batch, batch_idx):
         """Validation step."""
         inf_outputs, gen_outputs, losses = self(batch)
 
         r2_mean, r2_var = self.module.r2_metric(batch, gen_outputs)
 
         results = {}
         for key in losses:
             results.update({key: losses[key].item()})
 
         results.update({"generative_mean_accuracy": r2_mean})
         results.update({"generative_var_accuracy": r2_var})
         results.update({"biolord_metric": biolord_metric(r2_mean, r2_var)})
 
+        self.validation_step_outputs.append(results)
         return results
 
-    def validation_epoch_end(self, outputs):
+    def on_validation_epoch_end(self):
         """Validation step end."""
+        outputs = self.validation_step_outputs
         self.epoch_history["epoch"].append(self.current_epoch)
         self.epoch_history["mode"].append("valid")
         for key in self.epoch_keys:
             self.epoch_history[key].append(np.mean([output[key] for output in outputs]))
             self.log(f"val_{key}", self.epoch_history[key][-1], prog_bar=True)
 
+        self.validation_step_outputs.clear()
+
     def test_step(self, batch, batch_idx):
         """Test step."""
         return self.validation_step(batch, batch_idx)
 
     def test_epoch_end(self, outputs):
         """Test step end."""
         self.epoch_history["epoch"].append(self.current_epoch)
@@ -307,16 +322,16 @@
                         {
                             "params": list(
                                 filter(
                                     lambda p: p.requires_grad,
                                     classifier_.parameters(),
                                 )
                             ),
-                            "lr": self.autoencoder_lr,
-                            "weight_decay": self.autoencoder_wd,
+                            "lr": self.latent_lr,
+                            "weight_decay": self.latent_wd,
                             # betas=(0.5, 0.999),
                         }
                     ]
                 )
             )
 
         for _, regressor_ in self.module.ordered_regressors.items():
@@ -326,16 +341,16 @@
                         {
                             "params": list(
                                 filter(
                                     lambda p: p.requires_grad,
                                     regressor_.parameters(),
                                 )
                             ),
-                            "lr": self.autoencoder_lr,
-                            "weight_decay": self.autoencoder_wd,
+                            "lr": self.latent_lr,
+                            "weight_decay": self.latent_wd,
                             # betas=(0.5, 0.999),
                         }
                     ]
                 )
             )
 
         if self.step_size_lr is not None:
```

### Comparing `biolord-0.0.1/tests/test_basic.py` & `biolord-0.0.2/tests/test_basic.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,11 +17,11 @@
         retrieval_attribute_key=None,
     )
 
     model = biolord.Biolord(
         adata=adata,
         n_latent=n_latent,
     )
-    model.train(10, check_val_every_n_epoch=1, train_size=0.5)
+    model.train(10, check_val_every_n_epoch=1, train_size=0.5, enable_checkpointing=False)
 
     # tests __repr__
     print(model)
```

### Comparing `biolord-0.0.1/.gitignore` & `biolord-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `biolord-0.0.1/LICENSE` & `biolord-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biolord-0.0.1/pyproject.toml` & `biolord-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "biolord"
-version = "0.0.1"
+version = "0.0.2"
 description = "A deep generative framework for disentangling known and unknown attributes in single-cell data."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "Zoe Piran"},
 ]
@@ -22,14 +22,15 @@
     "anndata",
     # for debug logging (referenced from the issue template)
     "session-info",
     "rich",
     "scvi-tools",
     "torch",
     "scikit-learn",
+    "scanpy"
 ]
 
 [project.optional-dependencies]
 dev = [
     # CLI for bumping the version number
     "bump2version",
     "pre-commit",
```

### Comparing `biolord-0.0.1/PKG-INFO` & `biolord-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biolord
-Version: 0.0.1
+Version: 0.0.2
 Summary: A deep generative framework for disentangling known and unknown attributes in single-cell data.
 Project-URL: Documentation, https://biolord.readthedocs.io/
 Project-URL: Source, https://github.com/nitzanlab/biolord
 Project-URL: Home-page, https://github.com/nitzanlab/biolord
 Author: Zoe Piran
 Maintainer-email: Zoe Piran <zoe.piran@mail.huji.ac.il>
 License: BSD 3-Clause License
@@ -36,14 +36,15 @@
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: anndata
 Requires-Dist: rich
+Requires-Dist: scanpy
 Requires-Dist: scikit-learn
 Requires-Dist: scvi-tools
 Requires-Dist: session-info
 Requires-Dist: torch
 Provides-Extra: dev
 Requires-Dist: bump2version; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
@@ -72,14 +73,16 @@
 
 A deep generative framework for disentangling known and unknown attributes in single-cell data.
 
 We assume partial supervision over known attributes (categorical or ordered) along with single-cell measurements.
 Given the partial supervision [biolord][link-api] finds a decomposed latent space, and provides a generative model to
 obtain single-cell measurements for different cell states.
 
+For more details read the [preprint][link-preprint].
+
 ![The biolord pipeline][badge-pipeline]
 
 [badge-pipeline]: https://user-images.githubusercontent.com/43661890/222221567-09111a1a-8837-4bc5-8f71-15b596571c69.png?raw=true
 
 ## Getting started
 
 Please refer to the [documentation][link-docs].
@@ -106,14 +109,24 @@
 ## Contact
 
 Feel free to contact us by [mail][email].
 If you found a bug, please use the [issue tracker][issue-tracker].
 
 ## Citation
 
-> t.b.a
+```
+@article{piran2023biological,
+  title={Biological representation disentanglement of single-cell data},
+  author={Piran, Zoe and Cohen, Niv and Hoshen, Yedid and Nitzan, Mor},
+  journal={bioRxiv},
+  pages={2023--03},
+  year={2023},
+  publisher={Cold Spring Harbor Laboratory}
+}
+```
 
 [issue-tracker]: https://github.com/nitzanlab/biolord/issues
-[changelog]: https://biolord.readthedocs.io/latest/changelog.html
+[changelog]: https://biolord.readthedocs.io/en/latest/changelog.html
 [link-docs]: https://biolord.readthedocs.io
-[link-api]: https://biolord.readthedocs.io/latest/api.html
+[link-api]: https://biolord.readthedocs.io/en/latest/api.html
+[link-preprint]: https://www.biorxiv.org/content/10.1101/2023.03.05.531195v1
 [email]: mailto::zoe.piran@mail.huji.ac.il
```

