# Comparing `tmp/data-dag-0.2.2.tar.gz` & `tmp/data_dag-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-dag-0.2.2.tar", last modified: Thu Apr  6 17:32:45 2023, max compression
+gzip compressed data, was "data_dag-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `data-dag-0.2.2.tar` & `data_dag-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0      177 2023-04-06 17:31:12.370152 data-dag-0.2.2/.bumpversion.cfg
--rw-r--r--   0        0        0     1351 2022-07-12 18:41:30.346472 data-dag-0.2.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      359 2022-07-12 16:43:24.229520 data-dag-0.2.2/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      702 2022-07-12 16:43:24.229520 data-dag-0.2.2/.github/workflows/pypi.yml
--rw-r--r--   0        0        0     1008 2022-07-12 16:43:24.229520 data-dag-0.2.2/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2162 2022-07-05 17:25:03.902436 data-dag-0.2.2/.gitignore
--rw-r--r--   0        0        0      720 2023-04-06 17:29:46.795060 data-dag-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1015 2023-04-06 17:29:46.795584 data-dag-0.2.2/.ruff.toml
--rw-r--r--   0        0        0     4012 2023-04-06 17:32:20.400308 data-dag-0.2.2/README.md
--rw-r--r--   0        0        0       71 2023-04-06 17:31:12.369113 data-dag-0.2.2/data_dag/__init__.py
--rw-r--r--   0        0        0     4140 2023-04-06 17:29:46.796641 data-dag-0.2.2/data_dag/dag_factory.py
--rw-r--r--   0        0        0      371 2023-04-06 17:29:46.797160 data-dag-0.2.2/data_dag/operator_factory/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-06 17:29:46.798193 data-dag-0.2.2/data_dag/operator_factory/base.py
--rw-r--r--   0        0        0     6060 2023-04-06 17:29:46.798708 data-dag-0.2.2/data_dag/operator_factory/dynamic.py
--rw-r--r--   0        0        0     3760 2023-04-06 17:29:46.799230 data-dag-0.2.2/data_dag/operator_factory/simple.py
--rw-r--r--   0        0        0      654 2022-07-12 16:43:24.230519 data-dag-0.2.2/docs/Makefile
--rw-r--r--   0        0        0    35824 2022-07-12 16:43:24.231196 data-dag-0.2.2/docs/_images/img.png
--rw-r--r--   0        0        0      517 2023-04-06 17:29:41.241718 data-dag-0.2.2/docs/changelog.md
--rw-r--r--   0        0        0     2345 2023-04-06 17:31:12.369625 data-dag-0.2.2/docs/conf.py
--rw-r--r--   0        0        0    15045 2023-04-06 17:29:41.243816 data-dag-0.2.2/docs/getting_started.md
--rw-r--r--   0        0        0      503 2022-07-13 17:23:05.120784 data-dag-0.2.2/docs/index.md
--rw-r--r--   0        0        0       71 2022-07-12 16:43:24.233210 data-dag-0.2.2/docs/installation.md
--rwxr-xr-x   0        0        0      800 2022-07-12 16:43:24.234202 data-dag-0.2.2/docs/make.bat
--rw-r--r--   0        0        0     9157 2023-04-06 17:29:41.244380 data-dag-0.2.2/docs/overview.md
--rw-r--r--   0        0        0      189 2022-09-21 18:57:00.581648 data-dag-0.2.2/docs/reference/dag_factory.rst
--rw-r--r--   0        0        0      102 2022-07-13 17:25:22.892593 data-dag-0.2.2/docs/reference/modules.rst
--rw-r--r--   0        0        0      374 2023-04-06 17:29:41.245435 data-dag-0.2.2/docs/reference/operator_factory.rst
--rw-r--r--   0        0        0       72 2023-04-06 17:29:41.245962 data-dag-0.2.2/docs/requirements.txt
--rw-r--r--   0        0        0      187 2023-04-06 17:29:41.246483 data-dag-0.2.2/docs/usage/dag_factory.md
--rw-r--r--   0        0        0      127 2022-07-13 19:27:31.672485 data-dag-0.2.2/docs/usage/index.md
--rw-r--r--   0        0        0     2850 2023-04-06 17:29:41.247535 data-dag-0.2.2/docs/usage/operator_factory.md
--rw-r--r--   0        0        0      308 2023-04-06 17:29:46.800790 data-dag-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      204 2022-07-12 16:43:24.236204 data-dag-0.2.2/requirements.txt
--rw-r--r--   0        0        0      769 2023-04-06 17:31:12.368072 data-dag-0.2.2/setup.cfg
--rw-r--r--   0        0        0     1384 2022-07-06 20:04:36.688948 data-dag-0.2.2/tests/test_dag_factory.py
--rw-r--r--   0        0        0     4509 2022-07-13 19:52:45.671498 data-dag-0.2.2/tests/test_dynamic_operator_factory.py
--rw-r--r--   0        0        0     3811 2023-04-06 17:29:46.801830 data-dag-0.2.2/tests/test_operator_factory.py
--rw-r--r--   0        0        0     4121 1970-01-01 00:00:00.000000 data-dag-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      137 2023-07-26 22:06:21.894603 data_dag-0.3.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1309 2023-07-26 21:47:30.865196 data_dag-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      339 2023-07-26 21:47:30.865196 data_dag-0.3.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-07-26 21:47:30.865196 data_dag-0.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      977 2023-07-26 21:47:30.865196 data_dag-0.3.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2162 2023-07-26 21:47:30.865196 data_dag-0.3.0/.gitignore
+-rw-r--r--   0        0        0      696 2023-07-26 22:07:05.174882 data_dag-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      966 2023-07-26 21:47:30.865196 data_dag-0.3.0/.ruff.toml
+-rw-r--r--   0        0        0     3880 2023-07-26 21:47:30.865196 data_dag-0.3.0/README.md
+-rw-r--r--   0        0        0       68 2023-07-26 22:06:21.894603 data_dag-0.3.0/data_dag/__init__.py
+-rw-r--r--   0        0        0     4099 2023-07-26 21:55:25.037256 data_dag-0.3.0/data_dag/dag_factory.py
+-rw-r--r--   0        0        0      352 2023-07-26 21:47:30.865196 data_dag-0.3.0/data_dag/operator_factory/__init__.py
+-rw-r--r--   0        0        0     2507 2023-07-26 22:05:36.846225 data_dag-0.3.0/data_dag/operator_factory/base.py
+-rw-r--r--   0        0        0     5935 2023-07-26 21:47:30.865196 data_dag-0.3.0/data_dag/operator_factory/dynamic.py
+-rw-r--r--   0        0        0     3660 2023-07-26 21:47:30.865196 data_dag-0.3.0/data_dag/operator_factory/simple.py
+-rw-r--r--   0        0        0      634 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0    35824 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/_images/img.png
+-rw-r--r--   0        0        0      499 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/changelog.md
+-rw-r--r--   0        0        0     2277 2023-07-26 22:06:21.894603 data_dag-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0    14672 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/getting_started.md
+-rw-r--r--   0        0        0      470 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/index.md
+-rw-r--r--   0        0        0       65 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/installation.md
+-rw-r--r--   0        0        0      765 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0     8985 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/overview.md
+-rw-r--r--   0        0        0      183 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/reference/dag_factory.rst
+-rw-r--r--   0        0        0       94 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/reference/modules.rst
+-rw-r--r--   0        0        0      359 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/reference/operator_factory.rst
+-rw-r--r--   0        0        0       67 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0      179 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/usage/dag_factory.md
+-rw-r--r--   0        0        0      114 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/usage/index.md
+-rw-r--r--   0        0        0     2796 2023-07-26 21:47:30.865196 data_dag-0.3.0/docs/usage/operator_factory.md
+-rw-r--r--   0        0        0      902 2023-07-26 22:06:54.262819 data_dag-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-07-26 21:47:30.865196 data_dag-0.3.0/requirements.txt
+-rw-r--r--   0        0        0     1384 2023-07-26 21:47:30.865196 data_dag-0.3.0/tests/test_dag_factory.py
+-rw-r--r--   0        0        0     4509 2023-07-26 21:47:30.865196 data_dag-0.3.0/tests/test_dynamic_operator_factory.py
+-rw-r--r--   0        0        0     3667 2023-07-26 21:47:30.865196 data_dag-0.3.0/tests/test_operator_factory.py
+-rw-r--r--   0        0        0     4459 1970-01-01 00:00:00.000000 data_dag-0.3.0/PKG-INFO
```

### Comparing `data-dag-0.2.2/.github/workflows/docs.yml` & `data_dag-0.3.0/.github/workflows/docs.yml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Copied almost verbatim from https://github.com/marketplace/actions/sphinx-build
-name: sphinx
-on:
-  - push
-
-jobs:
-  docs_build:
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - uses: ammaraskar/sphinx-action@master
-        with:
-          docs-folder: "docs/"
-
-      - uses: actions/upload-artifact@v1
-        with:
-          name: DocumentationHTML
-          path: docs/_build/html/
-
-# Use RTFD instead
-#  publish_gh_pages:
-#    runs-on: ubuntu-latest
-#    needs: docs_build
-#    if: github.ref == 'refs/heads/master'
-#    steps:
-#      - name: Commit documentation changes
-#        run: |
-#          git clone https://github.com/your_git/repository.git --branch gh-pages --single-branch gh-pages
-#          cp -r docs/_build/html/* gh-pages/
-#          cd gh-pages
-#          git config --local user.email "action@github.com"
-#          git config --local user.name "GitHub Action"
-#          git add .
-#          git commit -m "Update documentation" -a || true
-#          # The above command will fail if no changes were present, so we ignore
-#          # the return code.
-#      - name: Push changes
-#        uses: ad-m/github-push-action@master
-#        with:
-#          branch: gh-pages
-#          directory: gh-pages
-#          github_token: ${{ secrets.GITHUB_TOKEN }}
+# Copied almost verbatim from https://github.com/marketplace/actions/sphinx-build
+name: sphinx
+on:
+  - push
+
+jobs:
+  docs_build:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: ammaraskar/sphinx-action@master
+        with:
+          docs-folder: "docs/"
+
+      - uses: actions/upload-artifact@v1
+        with:
+          name: DocumentationHTML
+          path: docs/_build/html/
+
+# Use RTFD instead
+#  publish_gh_pages:
+#    runs-on: ubuntu-latest
+#    needs: docs_build
+#    if: github.ref == 'refs/heads/master'
+#    steps:
+#      - name: Commit documentation changes
+#        run: |
+#          git clone https://github.com/your_git/repository.git --branch gh-pages --single-branch gh-pages
+#          cp -r docs/_build/html/* gh-pages/
+#          cd gh-pages
+#          git config --local user.email "action@github.com"
+#          git config --local user.name "GitHub Action"
+#          git add .
+#          git commit -m "Update documentation" -a || true
+#          # The above command will fail if no changes were present, so we ignore
+#          # the return code.
+#      - name: Push changes
+#        uses: ad-m/github-push-action@master
+#        with:
+#          branch: gh-pages
+#          directory: gh-pages
+#          github_token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `data-dag-0.2.2/.github/workflows/pypi.yml` & `data_dag-0.3.0/.github/workflows/pypi.yml`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-name: Upload Python Package
-
-on:
-  release:
-    types: [published]
-
-jobs:
-  deploy:
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: '3.x'
-          cache: 'pip'
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          pip install build
-      - name: Build package
-        run: python -m build
-      - name: Publish package
-        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
-        with:
-          user: __token__
-          password: ${{ secrets.PYPI_API_TOKEN }}
+name: Upload Python Package
+
+on:
+  release:
+    types: [published]
+
+jobs:
+  deploy:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.x'
+          cache: 'pip'
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install build
+      - name: Build package
+        run: python -m build
+      - name: Publish package
+        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+        with:
+          user: __token__
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `data-dag-0.2.2/.gitignore` & `data_dag-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `data-dag-0.2.2/README.md` & `data_dag-0.3.0/README.md`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-[![Documentation Status](https://readthedocs.org/projects/data-dag/badge/?version=latest)](https://data-dag.readthedocs.io/en/latest/?badge=latest) ![PyPI](https://img.shields.io/pypi/v/data-dag)
-
-# Overview
-
-`data-dag` is a library for writing data-defined Airflow DAGs and operators.
-
-# Installation
-
-```pip install data-dag```
-
-# Example
-
-Re-usable operator and DAG template can be stored in a central location, such as a custom Airflow plugin (or a package within `dags/` works fine too):
-
-```python
-# plugins/my_factories/download.py
-
-from data_dag.operator_factory import OperatorFactory
-from data_dag.dag_factory import DagFactory
-
-from urllib.request import urlretrieve
-from typing import List
-from airflow.operators.dummy import DummyOperator
-from airflow.providers.http.sensors.http import HttpSensor
-from airflow.operators.python import PythonOperator
-from airflow.utils.task_group import TaskGroup
-
-
-class DownloadOperator(OperatorFactory):
-    """An operator factory for safely downloading files to a known location"""
-
-    name: str
-    url: str
-    path: str
-
-    def make_operator(self):
-        with TaskGroup(group_id=f'download_{self.name}') as group:
-            check = HttpSensor(
-                task_id='check_exists',
-                endpoint=self.url
-            )
-            download = PythonOperator(
-                task_id=f'download',
-                python_callable=lambda: urlretrieve(self.url, self.path)
-            )
-            check >> download
-
-        return group
-
-
-class DownloaderDag(DagFactory):
-    """A DAG factory for producing simple DAGs that just download a bunch of files"""
-
-    downloads: List[DownloadOperator]
-
-    def _make_dag(self):
-        start = DummyOperator(task_id='start')
-        end = DummyOperator(task_id='end')
-
-        for download in self.downloads:
-            start >> download.make_operator() >> end
-```
-
-Then a definition for a particular DAG can live in a data file:
-
-```yaml
-# dags/yaml/sample_dag.yaml
-
-dag_id: sample_dag
-description: An example of how to write a data-driven DAG
-schedule_interval: '@daily'
-start_date: '2020-01-01T00:00:00'
-downloads:
-- name: data
-  url: https://www.example.com/data.zip
-  path: data.zip
-- name: manifest
-  url: https://www.example.com/manifest.json
-  path: manifest.json
-```
-
-That data file can then be loaded into a DAG. Per Airflow's requirements, this must be done in a file located in `dags/` and the result must be saved into a uniquely named global variable. The simplest possible example is this:
-
-```python
-# dags/sample_dag.py
-
-from yaml import safe_load
-from my_factories.download import DownloaderDag
-
-with open('yaml/sample_dag.yaml', 'r') as f:
-    dag_data = safe_load(f)
-
-dag = DownloaderDag.parse_obj(dag_data).make_dag()
-```
-
-![img.png](docs/_images/img.png)
-
-## Multiple DAGs
-
-Obviously, using a template isn't much use if you only fill it in once. Here's a simple example of a loader that will load any number of YML files from a folder and publish each one as a DAG in Airflow:
-
-```python
-# dags/load_yml_files.py
-
-from pathlib import Path
-from airflow import DAG
-import yaml
-from my_factories import BaseDag
-
-dag_dir = Path(__file__).parent
-
-# For each YAML file in a particular directory...
-for yaml_file_path in dag_dir.glob('typical_dags/**.yml'):
-    with open(yaml_file_path) as f:
-        dag_metadata = yaml.safe_load(f)
-
-    # ... generate a DAG from that metadata
-    dag_metadata_obj = BaseDag.parse_obj(dag_metadata)
-    dag = dag_metadata_obj.make_dag()
-
-    # See https://www.astronomer.io/guides/dynamically-generating-dags/
-    dag_name = yaml_file_path.with_suffix('').name
-    globals()[dag_name] = dag
-```
-
-# Documentation
-
-[Complete docs can be found here](https://data-dag.rtfd.org/)
-
-[//]: # (TODO)
-[//]: # (- Add DAG loader factory to enable a 2-liner DAG python file
-[//]: # (- Add dependency group mixin or something )
+[![Documentation Status](https://readthedocs.org/projects/data-dag/badge/?version=latest)](https://data-dag.readthedocs.io/en/latest/?badge=latest) ![PyPI](https://img.shields.io/pypi/v/data-dag)
+
+# Overview
+
+`data-dag` is a library for writing data-defined Airflow DAGs and operators.
+
+# Installation
+
+```pip install data-dag```
+
+# Example
+
+Re-usable operator and DAG template can be stored in a central location, such as a custom Airflow plugin (or a package within `dags/` works fine too):
+
+```python
+# plugins/my_factories/download.py
+
+from data_dag.operator_factory import OperatorFactory
+from data_dag.dag_factory import DagFactory
+
+from urllib.request import urlretrieve
+from typing import List
+from airflow.operators.dummy import DummyOperator
+from airflow.providers.http.sensors.http import HttpSensor
+from airflow.operators.python import PythonOperator
+from airflow.utils.task_group import TaskGroup
+
+
+class DownloadOperator(OperatorFactory):
+    """An operator factory for safely downloading files to a known location"""
+
+    name: str
+    url: str
+    path: str
+
+    def make_operator(self):
+        with TaskGroup(group_id=f'download_{self.name}') as group:
+            check = HttpSensor(
+                task_id='check_exists',
+                endpoint=self.url
+            )
+            download = PythonOperator(
+                task_id=f'download',
+                python_callable=lambda: urlretrieve(self.url, self.path)
+            )
+            check >> download
+
+        return group
+
+
+class DownloaderDag(DagFactory):
+    """A DAG factory for producing simple DAGs that just download a bunch of files"""
+
+    downloads: List[DownloadOperator]
+
+    def _make_dag(self):
+        start = DummyOperator(task_id='start')
+        end = DummyOperator(task_id='end')
+
+        for download in self.downloads:
+            start >> download.make_operator() >> end
+```
+
+Then a definition for a particular DAG can live in a data file:
+
+```yaml
+# dags/yaml/sample_dag.yaml
+
+dag_id: sample_dag
+description: An example of how to write a data-driven DAG
+schedule_interval: '@daily'
+start_date: '2020-01-01T00:00:00'
+downloads:
+- name: data
+  url: https://www.example.com/data.zip
+  path: data.zip
+- name: manifest
+  url: https://www.example.com/manifest.json
+  path: manifest.json
+```
+
+That data file can then be loaded into a DAG. Per Airflow's requirements, this must be done in a file located in `dags/` and the result must be saved into a uniquely named global variable. The simplest possible example is this:
+
+```python
+# dags/sample_dag.py
+
+from yaml import safe_load
+from my_factories.download import DownloaderDag
+
+with open('yaml/sample_dag.yaml', 'r') as f:
+    dag_data = safe_load(f)
+
+dag = DownloaderDag.parse_obj(dag_data).make_dag()
+```
+
+![img.png](docs/_images/img.png)
+
+## Multiple DAGs
+
+Obviously, using a template isn't much use if you only fill it in once. Here's a simple example of a loader that will load any number of YML files from a folder and publish each one as a DAG in Airflow:
+
+```python
+# dags/load_yml_files.py
+
+from pathlib import Path
+from airflow import DAG
+import yaml
+from my_factories import BaseDag
+
+dag_dir = Path(__file__).parent
+
+# For each YAML file in a particular directory...
+for yaml_file_path in dag_dir.glob('typical_dags/**.yml'):
+    with open(yaml_file_path) as f:
+        dag_metadata = yaml.safe_load(f)
+
+    # ... generate a DAG from that metadata
+    dag_metadata_obj = BaseDag.parse_obj(dag_metadata)
+    dag = dag_metadata_obj.make_dag()
+
+    # See https://www.astronomer.io/guides/dynamically-generating-dags/
+    dag_name = yaml_file_path.with_suffix('').name
+    globals()[dag_name] = dag
+```
+
+# Documentation
+
+[Complete docs can be found here](https://data-dag.rtfd.org/)
+
+[//]: # (TODO)
+[//]: # (- Add DAG loader factory to enable a 2-liner DAG python file
+[//]: # (- Add dependency group mixin or something )
```

### Comparing `data-dag-0.2.2/data_dag/dag_factory.py` & `data_dag-0.3.0/data_dag/dag_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,99 @@
-import abc
-from datetime import datetime, timedelta
-from typing import Dict, Iterable, List, Optional, Union
-
-from airflow.models.dag import DAG
-from pydantic import BaseModel
-
-
-class DagFactory(BaseModel, abc.ABC):
-    """
-    Base factory class for generating DAGs.
-
-    This class serves as a metadata wrapper around :py:class:`airflow.models.dag.DAG`.
-
-    The simplest way to create a DAG factory is to inherit from :py:class:`DagFactory` and implement :py:meth:`_make_dag`, like::
-
-        class MyKindOfDag(DagFactory):
-            def _make_dag(self):
-                start = DummyOperator(...)
-                do_something = PythonOperator(...)
-                end = DummyOperator(...)
-
-                start >> do_something >> end
-
-    The :py:class:`~airflow.models.dag.DAG` object itself will be automatically created and opened prior to :py:meth:`_make_dag` being called.
-    The final DAG can be obtained by calling :py:meth:`make_dag` on an instance of your factory::
-
-        my_particular_dag_metadata = MyKindOfDag()
-        dag = my_particular_dag_metadata.make_dag()
-
-    For documentation on the attributes of :py:class:`DagFactory`, see the `DAG type docs <https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/dag/index.html#airflow.models.dag.DAG>`_.
-
-    DAG keyword arguments can be passed in any of three ways (in ascending priority):
-    1. Overriding :py:meth:`default_dag_kwargs` to return a dictionary of default keyword arguments
-    2. Passing in data during construction (either directly or in an overridden constructor)
-    3. As a ``dag_overrides`` dictionary when calling :py:meth:`make_dag`
-    """
-
-    dag_id: str
-    description: Optional[str] = None
-    schedule_interval: Union[timedelta, str, None] = None
-    start_date: Optional[datetime] = None
-    end_date: Optional[datetime] = None
-    full_filepath: Optional[str] = None
-    template_searchpath: Optional[Union[str, Iterable[str]]] = None
-    user_defined_macros: Optional[Dict] = None
-    user_defined_filters: Optional[Dict] = None
-    default_args: Optional[Dict] = None
-    concurrency: Optional[int] = None
-    max_active_tasks: Optional[int] = None
-    max_active_runs: Optional[int] = None
-    dagrun_timeout: Optional[timedelta] = None
-    default_view: Optional[str] = None
-    orientation: Optional[str] = None
-    catchup: Optional[bool] = None
-    doc_md: Optional[str] = None
-    params: Optional[Dict] = None
-    access_control: Optional[Dict] = None
-    is_paused_upon_creation: Optional[bool] = None
-    jinja_environment_kwargs: Optional[Dict] = None
-    render_template_as_native_obj: bool = False
-    tags: Optional[List[str]] = None
-
-    @property
-    def default_dag_kwargs(self) -> Dict:
-        """Override this property in a subclass to provide default arguments to the
-        :py:class:`airflow.models.dag.DAG` constructor."""
-        return {}
-
-    def make_dag_object(self, **overrides) -> DAG:
-        """Creates the basic :py:class:`airflow.models.dag.DAG` object represented by this metadata.
-
-        This doesn't populate the DAG with nodes, it is only responsible for creating the initial DAG object.
-        """
-        kwargs = self.default_dag_kwargs.copy()
-        kwargs.update(
-            {
-                field: getattr(self, field, None)
-                for field in DagFactory.__fields__
-                if getattr(self, field, None) is not None
-            }
-        )
-        kwargs.update(overrides)
-        return DAG(**kwargs)
-
-    def make_dag(self, *args, dag_overrides: Optional[Dict] = None, **kwargs) -> DAG:
-        """Creates and populates a :py:class:`airflow.models.dag.DAG` represented by this metadata"""
-        dag = self.make_dag_object(**(dag_overrides or {}))
-        with dag:
-            self._make_dag(*args, **kwargs)
-
-        return dag
-
-    def _make_dag(self, *args, **kwargs) -> None:
-        """Override this method in a subclass to populate the :py:class:`airflow.models.dag.DAG` object with nodes and edges"""
-        raise NotImplementedError()
+import abc
+from datetime import datetime, timedelta
+from typing import Dict, Iterable, List, Optional, Union
+
+from airflow.models.dag import DAG
+from pydantic import BaseModel, Extra
+
+
+class DagFactory(BaseModel, abc.ABC):
+    """
+    Base factory class for generating DAGs.
+
+    This class serves as a metadata wrapper around :py:class:`airflow.models.dag.DAG`.
+
+    The simplest way to create a DAG factory is to inherit from :py:class:`DagFactory` and implement :py:meth:`_make_dag`, like::
+
+        class MyKindOfDag(DagFactory):
+            def _make_dag(self):
+                start = DummyOperator(...)
+                do_something = PythonOperator(...)
+                end = DummyOperator(...)
+
+                start >> do_something >> end
+
+    The :py:class:`~airflow.models.dag.DAG` object itself will be automatically created and opened prior to :py:meth:`_make_dag` being called.
+    The final DAG can be obtained by calling :py:meth:`make_dag` on an instance of your factory::
+
+        my_particular_dag_metadata = MyKindOfDag()
+        dag = my_particular_dag_metadata.make_dag()
+
+    For documentation on the attributes of :py:class:`DagFactory`, see the `DAG type docs <https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/dag/index.html#airflow.models.dag.DAG>`_.
+
+    DAG keyword arguments can be passed in any of three ways (in ascending priority):
+    1. Overriding :py:meth:`default_dag_kwargs` to return a dictionary of default keyword arguments
+    2. Passing in data during construction (either directly or in an overridden constructor)
+    3. As a ``dag_overrides`` dictionary when calling :py:meth:`make_dag`
+    """
+
+    dag_id: str
+    description: Optional[str] = None
+    schedule_interval: Union[timedelta, str, None] = None
+    start_date: Optional[datetime] = None
+    end_date: Optional[datetime] = None
+    full_filepath: Optional[str] = None
+    template_searchpath: Optional[Union[str, Iterable[str]]] = None
+    user_defined_macros: Optional[Dict] = None
+    user_defined_filters: Optional[Dict] = None
+    default_args: Optional[Dict] = None
+    concurrency: Optional[int] = None
+    max_active_tasks: Optional[int] = None
+    max_active_runs: Optional[int] = None
+    dagrun_timeout: Optional[timedelta] = None
+    default_view: Optional[str] = None
+    orientation: Optional[str] = None
+    catchup: Optional[bool] = None
+    doc_md: Optional[str] = None
+    params: Optional[Dict] = None
+    access_control: Optional[Dict] = None
+    is_paused_upon_creation: Optional[bool] = None
+    jinja_environment_kwargs: Optional[Dict] = None
+    render_template_as_native_obj: bool = False
+    tags: Optional[List[str]] = None
+
+    class Config:
+        extra = Extra.forbid
+
+    @property
+    def default_dag_kwargs(self) -> Dict:
+        """Override this property in a subclass to provide default arguments to the
+        :py:class:`airflow.models.dag.DAG` constructor."""
+        return {}
+
+    def make_dag_object(self, **overrides) -> DAG:
+        """Creates the basic :py:class:`airflow.models.dag.DAG` object represented by this metadata.
+
+        This doesn't populate the DAG with nodes, it is only responsible for creating the initial DAG object.
+        """
+        kwargs = self.default_dag_kwargs.copy()
+        kwargs.update(
+            {
+                field: getattr(self, field, None)
+                for field in DagFactory.__fields__
+                if getattr(self, field, None) is not None
+            }
+        )
+        kwargs.update(overrides)
+        return DAG(**kwargs)
+
+    def make_dag(self, *args, dag_overrides: Optional[Dict] = None, **kwargs) -> DAG:
+        """Creates and populates a :py:class:`airflow.models.dag.DAG` represented by this metadata"""
+        dag = self.make_dag_object(**(dag_overrides or {}))
+        with dag:
+            self._make_dag(*args, **kwargs)
+
+        return dag
+
+    def _make_dag(self, *args, **kwargs) -> None:
+        """Override this method in a subclass to populate the :py:class:`airflow.models.dag.DAG` object with nodes and edges"""
+        raise NotImplementedError()
```

### Comparing `data-dag-0.2.2/data_dag/operator_factory/base.py` & `data_dag-0.3.0/data_dag/operator_factory/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,72 @@
-import abc
-import contextlib
-from typing import Optional, Sequence, Union
-
-from airflow.models.taskmixin import TaskMixin
-from airflow.utils.task_group import TaskGroup
-from pydantic import BaseModel
-
-
-class BaseOperatorFactory(BaseModel, abc.ABC):
-    def make_operator(
-        self, *args, **kwargs
-    ) -> Union[TaskMixin, Sequence[TaskMixin], None]:
-        """Converts this factory metadata into an operator.
-
-        Returns:
-            Zero or more operator-like things. The code that calls this should know how to handle the possible return types for this particular factory.
-        """
-        raise NotImplementedError()
-
-
-class OperatorFactory(BaseOperatorFactory, abc.ABC):
-    """An interface for writing operator factories."""
-
-    task_id: Optional[str]
-
-    @property
-    def default_task_id(self) -> str:
-        """If overridden, defines a default task ID when none is manually specified"""
-        raise NotImplementedError()
-
-    def get_task_id(self):
-        """Provides the custom task ID if provided, else this factory's default task ID"""
-        return self.task_id or self.default_task_id
-
-    @contextlib.contextmanager
-    def _task_group(self):
-        with TaskGroup(group_id=self.get_task_id()) as group:
-            yield
-
-        return group
-
-    def make_operator(
-        self, *args, **kwargs
-    ) -> Union[TaskMixin, Sequence[TaskMixin], None]:
-        """Converts this factory metadata into an operator.
-
-        If you need to create multiple operators, whether connected or not, implement :py:meth:`_make_operators`
-        instead, and they will be automatically wrapped in a :py:class:`airflow.utils.task_group.TaskGroup`.
-
-        Returns:
-            Zero or more operator-like things. The code that calls this should know how to handle the possible return types for this particular factory.
-        """
-        with self._task_group() as group:
-            self._make_operators(*args, **kwargs)
-
-        return group
-
-    def _make_operators(self, *args, **kwargs) -> None:
-        """Can be implemented instead of :py:meth:`make_operator` to define an operator collection inside a
-        default :py:class:`airflow.utils.task_group.TaskGroup`"""
-        raise NotImplementedError()
-
-
-class OperatorComponent(BaseModel, abc.ABC):
-    """A non-operator component for use in other operator factories. Just a proxy for :py:class:`pydantic.BaseModel`."""
-
-    pass
+import abc
+import contextlib
+from typing import Optional, Sequence, Union
+
+from airflow.models.taskmixin import TaskMixin
+from airflow.utils.task_group import TaskGroup
+from pydantic import BaseModel, Extra
+
+
+class BaseOperatorFactory(BaseModel, abc.ABC):
+    class Config:
+        extra = Extra.forbid
+
+    def make_operator(
+        self, *args, **kwargs
+    ) -> Union[TaskMixin, Sequence[TaskMixin], None]:
+        """Converts this factory metadata into an operator.
+
+        Returns:
+            Zero or more operator-like things. The code that calls this should know how to handle the possible return types for this particular factory.
+        """
+        raise NotImplementedError()
+
+
+class OperatorFactory(BaseOperatorFactory, abc.ABC):
+    """An interface for writing operator factories."""
+
+    task_id: Optional[str]
+
+    @property
+    def default_task_id(self) -> str:
+        """If overridden, defines a default task ID when none is manually specified"""
+        raise NotImplementedError()
+
+    def get_task_id(self):
+        """Provides the custom task ID if provided, else this factory's default task ID"""
+        return self.task_id or self.default_task_id
+
+    @contextlib.contextmanager
+    def _task_group(self):
+        with TaskGroup(group_id=self.get_task_id()) as group:
+            yield
+
+        return group
+
+    def make_operator(
+        self, *args, **kwargs
+    ) -> Union[TaskMixin, Sequence[TaskMixin], None]:
+        """Converts this factory metadata into an operator.
+
+        If you need to create multiple operators, whether connected or not, implement :py:meth:`_make_operators`
+        instead, and they will be automatically wrapped in a :py:class:`airflow.utils.task_group.TaskGroup`.
+
+        Returns:
+            Zero or more operator-like things. The code that calls this should know how to handle the possible return types for this particular factory.
+        """
+        with self._task_group() as group:
+            self._make_operators(*args, **kwargs)
+
+        return group
+
+    def _make_operators(self, *args, **kwargs) -> None:
+        """Can be implemented instead of :py:meth:`make_operator` to define an operator collection inside a
+        default :py:class:`airflow.utils.task_group.TaskGroup`"""
+        raise NotImplementedError()
+
+
+class OperatorComponent(BaseModel, abc.ABC):
+    """A non-operator component for use in other operator factories. Just a proxy for :py:class:`pydantic.BaseModel`."""
+
+    class Config:
+        extra = Extra.forbid
```

### Comparing `data-dag-0.2.2/data_dag/operator_factory/dynamic.py` & `data_dag-0.3.0/data_dag/operator_factory/dynamic.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import abc
-import inspect
-import warnings
-
-from pydantic.main import ModelMetaclass
-
-from .base import OperatorComponent, OperatorFactory
-
-
-class _DynamicModelMetaclass(ModelMetaclass):
-    def __new__(mcs, *args, **kwargs):
-        cls = super().__new__(mcs, *args, **kwargs)
-        cls.__known_subclasses__ = dict()
-        return cls
-
-    def __call__(cls, *args, **kwargs):
-        known_subtype = cls.__type_name__
-        specified_subtype = kwargs.pop(
-            cls.__type_kwarg_name__, cls.__default_type_name__
-        )
-
-        if known_subtype is None and specified_subtype is None:
-            raise TypeError(
-                f"Failed to find type kwarg `{cls.__type_kwarg_name__}` while instantiating {cls}"
-            )
-        elif known_subtype is not None and specified_subtype is not None:
-            raise TypeError(
-                f"Cannot specify explicit `{cls.__type_kwarg_name__}` to specific type {cls}"
-            )
-
-        # At this point, we know that exactly one of known_subtype and specified_subtype is given
-        assert bool(known_subtype) ^ bool(specified_subtype), (
-            known_subtype,
-            specified_subtype,
-        )
-
-        if known_subtype:
-            specified_cls = cls
-        elif specified_subtype:
-            try:
-                specified_cls = cls.__known_subclasses__[specified_subtype]
-            except KeyError as ex:
-                raise TypeError(
-                    f"Subtype `{specified_subtype}` not found for {cls}. Options are {list(cls.__known_subclasses__)}"
-                ) from ex
-        else:  # pragma: no cover
-            assert False, ("How did we get here?", known_subtype, specified_subtype)
-
-        return super(_DynamicModelMetaclass, specified_cls).__call__(*args, **kwargs)
-
-
-# With much help from
-# https://stackoverflow.com/questions/23374715/changing-the-bases-of-an-object-based-on-arguments-to-init
-class _DynamicOperatorBase:
-    __type_name__ = None
-    __default_type_name__ = None
-    __type_kwarg_name__ = "type"
-
-    def __init_subclass__(cls, **kwargs):
-        if not inspect.isabstract(cls) and abc.ABC not in cls.__bases__:
-            subtype_name = cls.__type_name__
-
-            if not subtype_name:
-                warnings.warn(
-                    f"Type {cls} does not specify a subtype name (as __type_name__) and cannot be dynamically instantiated; if this is intentional, make the clas abstract, like `class {cls.__name__}(..., abc.ABC):`"
-                )
-
-            cls.__known_subclasses__[subtype_name] = cls
-
-
-class DynamicOperatorFactory(
-    OperatorFactory, _DynamicOperatorBase, abc.ABC, metaclass=_DynamicModelMetaclass
-):
-    """An OperatorFactory that can automatically instantiate sub-classes based on the input data.
-
-    Consider the following example::
-
-        class InputFile(DynamicOperatorFactory, abc.ABC):
-            pass
-
-        class LocalFile(InputFile):
-            __type_name__ = 'local'
-
-            path: str
-
-        class S3File(InputFile):
-            __type_name__ = 's3'
-
-            bucket: str
-            key: str
-
-        InputFile.parse_obj({'type': 's3', 'bucket': 'my-bucket', 'key': 'my-key'})
-        # S3File(bucket='my-bucket', key='my-key')
-
-    Note how the type of object that gets instantiated is dynamically chosen from the data, rather than specified by the code. This allows a supertype to be used in code, and for the subtype to be chosen at runtime based on data.
-
-    To use a dynamic factory, define your base supertype to inherit directly from :py:class:`DynamicOperatorFactory` and :py:class:`abc.ABC`. The class can be totally empty, as in the example above. This top-level class will be populated with a dictionary that will automatically track subclasses as they get define.
-
-    .. warning::
-
-        It's important to remember that, while subtypes are automatically tracked upon definition, they must still be imported somewhere. Make sure that when the supertype is imported, the subtypes also eventually get imported, or else they will be unavailable at DAG resolution time.
-
-    Subclasses must either define ``__type_name__ = "some_name"`` or else inherit from :py:class:`abc.ABC` to indicate that they are abstract. Classes that are not abstract and not named will generate a warning.
-
-    A default subtype can be specified using ``__default_type_name__`` in the top-level type. Note that this is the ``__type_name__`` of the default subclass, not the class name itself.
-
-    By default, the subclass is chosen by the ``"type"`` key in the input data. This can be changed by setting ``__type_kwarg_name__`` in the top-level type to some other string. This key will be stripped from the input data and all other keys will be passed along to the subtype's constructor without further modification.
-
-    Attempting to construct a top-level object, either directly (with its constructor) or using ``parse_obj``, without specifying a "type" (or whatever you renamed the key to be) will result in a :py:exc:`TypeError`.
-
-    .. note::
-
-        Pydantic already supports Union types, so why would we use a custom DynamicOperatorFactory instead?
-
-        Dynamic factories provide two key advantages:
-
-        - The subtype selected is explicit rather than implicit. The subtypes don't need to be distinguishable in any other way besides their ``__type_name__``, nor is there any kind of ordering of the subtypes.
-        - The list of options is automatically maintained, as long as the modules containing the subtypes are sure to be imported. That is, another component or factory can use the top-level type to annotate one of its fields, and the subtypes will automatically be implied.
-    """
-
-
-class DynamicOperatorComponent(
-    OperatorComponent, _DynamicOperatorBase, abc.ABC, metaclass=_DynamicModelMetaclass
-):
-    """Identical to :py:class:`DynamicOperatorFactory` but based on :py:class:`OperatorComponent` instead."""
+import abc
+import inspect
+import warnings
+
+from pydantic.main import ModelMetaclass
+
+from .base import OperatorComponent, OperatorFactory
+
+
+class _DynamicModelMetaclass(ModelMetaclass):
+    def __new__(mcs, *args, **kwargs):
+        cls = super().__new__(mcs, *args, **kwargs)
+        cls.__known_subclasses__ = dict()
+        return cls
+
+    def __call__(cls, *args, **kwargs):
+        known_subtype = cls.__type_name__
+        specified_subtype = kwargs.pop(
+            cls.__type_kwarg_name__, cls.__default_type_name__
+        )
+
+        if known_subtype is None and specified_subtype is None:
+            raise TypeError(
+                f"Failed to find type kwarg `{cls.__type_kwarg_name__}` while instantiating {cls}"
+            )
+        elif known_subtype is not None and specified_subtype is not None:
+            raise TypeError(
+                f"Cannot specify explicit `{cls.__type_kwarg_name__}` to specific type {cls}"
+            )
+
+        # At this point, we know that exactly one of known_subtype and specified_subtype is given
+        assert bool(known_subtype) ^ bool(specified_subtype), (
+            known_subtype,
+            specified_subtype,
+        )
+
+        if known_subtype:
+            specified_cls = cls
+        elif specified_subtype:
+            try:
+                specified_cls = cls.__known_subclasses__[specified_subtype]
+            except KeyError as ex:
+                raise TypeError(
+                    f"Subtype `{specified_subtype}` not found for {cls}. Options are {list(cls.__known_subclasses__)}"
+                ) from ex
+        else:  # pragma: no cover
+            assert False, ("How did we get here?", known_subtype, specified_subtype)
+
+        return super(_DynamicModelMetaclass, specified_cls).__call__(*args, **kwargs)
+
+
+# With much help from
+# https://stackoverflow.com/questions/23374715/changing-the-bases-of-an-object-based-on-arguments-to-init
+class _DynamicOperatorBase:
+    __type_name__ = None
+    __default_type_name__ = None
+    __type_kwarg_name__ = "type"
+
+    def __init_subclass__(cls, **kwargs):
+        if not inspect.isabstract(cls) and abc.ABC not in cls.__bases__:
+            subtype_name = cls.__type_name__
+
+            if not subtype_name:
+                warnings.warn(
+                    f"Type {cls} does not specify a subtype name (as __type_name__) and cannot be dynamically instantiated; if this is intentional, make the clas abstract, like `class {cls.__name__}(..., abc.ABC):`"
+                )
+
+            cls.__known_subclasses__[subtype_name] = cls
+
+
+class DynamicOperatorFactory(
+    OperatorFactory, _DynamicOperatorBase, abc.ABC, metaclass=_DynamicModelMetaclass
+):
+    """An OperatorFactory that can automatically instantiate sub-classes based on the input data.
+
+    Consider the following example::
+
+        class InputFile(DynamicOperatorFactory, abc.ABC):
+            pass
+
+        class LocalFile(InputFile):
+            __type_name__ = 'local'
+
+            path: str
+
+        class S3File(InputFile):
+            __type_name__ = 's3'
+
+            bucket: str
+            key: str
+
+        InputFile.parse_obj({'type': 's3', 'bucket': 'my-bucket', 'key': 'my-key'})
+        # S3File(bucket='my-bucket', key='my-key')
+
+    Note how the type of object that gets instantiated is dynamically chosen from the data, rather than specified by the code. This allows a supertype to be used in code, and for the subtype to be chosen at runtime based on data.
+
+    To use a dynamic factory, define your base supertype to inherit directly from :py:class:`DynamicOperatorFactory` and :py:class:`abc.ABC`. The class can be totally empty, as in the example above. This top-level class will be populated with a dictionary that will automatically track subclasses as they get define.
+
+    .. warning::
+
+        It's important to remember that, while subtypes are automatically tracked upon definition, they must still be imported somewhere. Make sure that when the supertype is imported, the subtypes also eventually get imported, or else they will be unavailable at DAG resolution time.
+
+    Subclasses must either define ``__type_name__ = "some_name"`` or else inherit from :py:class:`abc.ABC` to indicate that they are abstract. Classes that are not abstract and not named will generate a warning.
+
+    A default subtype can be specified using ``__default_type_name__`` in the top-level type. Note that this is the ``__type_name__`` of the default subclass, not the class name itself.
+
+    By default, the subclass is chosen by the ``"type"`` key in the input data. This can be changed by setting ``__type_kwarg_name__`` in the top-level type to some other string. This key will be stripped from the input data and all other keys will be passed along to the subtype's constructor without further modification.
+
+    Attempting to construct a top-level object, either directly (with its constructor) or using ``parse_obj``, without specifying a "type" (or whatever you renamed the key to be) will result in a :py:exc:`TypeError`.
+
+    .. note::
+
+        Pydantic already supports Union types, so why would we use a custom DynamicOperatorFactory instead?
+
+        Dynamic factories provide two key advantages:
+
+        - The subtype selected is explicit rather than implicit. The subtypes don't need to be distinguishable in any other way besides their ``__type_name__``, nor is there any kind of ordering of the subtypes.
+        - The list of options is automatically maintained, as long as the modules containing the subtypes are sure to be imported. That is, another component or factory can use the top-level type to annotate one of its fields, and the subtypes will automatically be implied.
+    """
+
+
+class DynamicOperatorComponent(
+    OperatorComponent, _DynamicOperatorBase, abc.ABC, metaclass=_DynamicModelMetaclass
+):
+    """Identical to :py:class:`DynamicOperatorFactory` but based on :py:class:`OperatorComponent` instead."""
```

### Comparing `data-dag-0.2.2/data_dag/operator_factory/simple.py` & `data_dag-0.3.0/data_dag/operator_factory/simple.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-import abc
-import inspect
-from typing import Any, Type
-
-from pydantic import BaseModel
-from typing_extensions import get_origin
-
-from .base import OperatorComponent, OperatorFactory
-
-
-def _dict_from_primitive(cls: "Type[_SimpleModelMixin]", obj):
-    assert cls.__simple_field__ is not None
-    if not isinstance(obj, dict):
-        return {cls.__simple_field__.name: obj}
-    else:
-        # Check if we're expecting a dictionary...
-        tp = cls.__simple_field__.outer_type_
-        tp = get_origin(tp) or tp
-        if isinstance(tp, type) and issubclass(tp, dict):
-            raise NotImplementedError(
-                "Not yet sure how to handle sanitizing a dictionary when the class is just a proxy for a dictionary field"
-            )
-        ###
-        return obj
-
-
-class _SimpleModelMixin:
-    """A mixin to support single-field pydantic models being parsed directly from primitives rather than requiring dictionaries"""
-
-    def __init_subclass__(cls, **kwargs):
-        assert issubclass(cls, BaseModel)
-
-        if not inspect.isabstract(cls) and abc.ABC not in cls.__bases__:
-            required_fields = [
-                field for field in cls.__fields__.values() if field.required
-            ]
-            if len(required_fields) != 1:
-                raise TypeError(
-                    f"A non-abstract inheritor of {cls} must have exactly one non-default field (Found {[f.name for f in required_fields]})"
-                )
-
-            field = required_fields[0]
-            cls.__simple_field__ = field
-            cls.__pre_root_validators__ = [_dict_from_primitive]
-
-    @classmethod
-    def _enforce_dict_if_root(cls, obj: Any) -> Any:
-        obj = super()._enforce_dict_if_root(obj)
-        obj = _dict_from_primitive(cls, obj)
-        return obj
-
-
-class SimpleOperatorFactory(_SimpleModelMixin, OperatorFactory, abc.ABC):
-    """Identical to :py:class:`OperatorFactory` except that this represents predominantly a single field of metadata.
-
-    The model that inherits from :py:class:`SimpleOperatorFactory` can only have a single non-required field
-    (meaning no default value and not :py:class:`~typing.Optional`). In return the constructor for this object,
-    in addition to being callable with a dictionary of field values, can also be called with a simple literal to fill
-    in the single required field.
-
-    Consider the following example::
-
-        class FilePath(SimpleOperatorFactory):
-            path: str  # <-- single required field
-            is_file: bool = True  # <-- optional field (because of default)
-            mime_type: Optional[str]  # <-- optional field (because of Optional type)
-
-            def make_operator(self):
-                ...
-
-    Normally, this object could only be instantiated using a dictionary::
-
-        FilePath.parse_obj({'path': 'path/to/file.txt'})
-
-        # Or, in YAML:
-        # outer_object:
-        #   my_file:
-        #     path: 'path/to/file.txt'
-        # Or, in JSON:
-        # {"outer_object": {"my_file": {"path": "path/to/file.txt"}}}
-
-    However, because we inherit from :py:class:`SimpleOperatorFactory`, we can instantiate a ``FilePath`` by specifying just the ``path`` literal::
-
-        FilePath.parse_obj('path/to/file.txt')
-
-        # Or, in YAML:
-        # outer_object:
-        #   my_file: 'path/to/file.txt'
-        # Or, in JSON:
-        # {"outer_object": {"my_file": "path/to/file.txt"}}
-    """
-
-    pass
-
-
-class SimpleOperatorComponent(_SimpleModelMixin, OperatorComponent, abc.ABC):
-    """An extension of :py:class:`OperatorComponent` to have the same single-field functionality as
-    :py:class:`SimpleOperatorFactory`."""
-
-    pass
+import abc
+import inspect
+from typing import Any, Type
+
+from pydantic import BaseModel
+from typing_extensions import get_origin
+
+from .base import OperatorComponent, OperatorFactory
+
+
+def _dict_from_primitive(cls: "Type[_SimpleModelMixin]", obj):
+    assert cls.__simple_field__ is not None
+    if not isinstance(obj, dict):
+        return {cls.__simple_field__.name: obj}
+    else:
+        # Check if we're expecting a dictionary...
+        tp = cls.__simple_field__.outer_type_
+        tp = get_origin(tp) or tp
+        if isinstance(tp, type) and issubclass(tp, dict):
+            raise NotImplementedError(
+                "Not yet sure how to handle sanitizing a dictionary when the class is just a proxy for a dictionary field"
+            )
+        ###
+        return obj
+
+
+class _SimpleModelMixin:
+    """A mixin to support single-field pydantic models being parsed directly from primitives rather than requiring dictionaries"""
+
+    def __init_subclass__(cls, **kwargs):
+        assert issubclass(cls, BaseModel)
+
+        if not inspect.isabstract(cls) and abc.ABC not in cls.__bases__:
+            required_fields = [
+                field for field in cls.__fields__.values() if field.required
+            ]
+            if len(required_fields) != 1:
+                raise TypeError(
+                    f"A non-abstract inheritor of {cls} must have exactly one non-default field (Found {[f.name for f in required_fields]})"
+                )
+
+            field = required_fields[0]
+            cls.__simple_field__ = field
+            cls.__pre_root_validators__ = [_dict_from_primitive]
+
+    @classmethod
+    def _enforce_dict_if_root(cls, obj: Any) -> Any:
+        obj = super()._enforce_dict_if_root(obj)
+        obj = _dict_from_primitive(cls, obj)
+        return obj
+
+
+class SimpleOperatorFactory(_SimpleModelMixin, OperatorFactory, abc.ABC):
+    """Identical to :py:class:`OperatorFactory` except that this represents predominantly a single field of metadata.
+
+    The model that inherits from :py:class:`SimpleOperatorFactory` can only have a single non-required field
+    (meaning no default value and not :py:class:`~typing.Optional`). In return the constructor for this object,
+    in addition to being callable with a dictionary of field values, can also be called with a simple literal to fill
+    in the single required field.
+
+    Consider the following example::
+
+        class FilePath(SimpleOperatorFactory):
+            path: str  # <-- single required field
+            is_file: bool = True  # <-- optional field (because of default)
+            mime_type: Optional[str]  # <-- optional field (because of Optional type)
+
+            def make_operator(self):
+                ...
+
+    Normally, this object could only be instantiated using a dictionary::
+
+        FilePath.parse_obj({'path': 'path/to/file.txt'})
+
+        # Or, in YAML:
+        # outer_object:
+        #   my_file:
+        #     path: 'path/to/file.txt'
+        # Or, in JSON:
+        # {"outer_object": {"my_file": {"path": "path/to/file.txt"}}}
+
+    However, because we inherit from :py:class:`SimpleOperatorFactory`, we can instantiate a ``FilePath`` by specifying just the ``path`` literal::
+
+        FilePath.parse_obj('path/to/file.txt')
+
+        # Or, in YAML:
+        # outer_object:
+        #   my_file: 'path/to/file.txt'
+        # Or, in JSON:
+        # {"outer_object": {"my_file": "path/to/file.txt"}}
+    """
+
+    pass
+
+
+class SimpleOperatorComponent(_SimpleModelMixin, OperatorComponent, abc.ABC):
+    """An extension of :py:class:`OperatorComponent` to have the same single-field functionality as
+    :py:class:`SimpleOperatorFactory`."""
+
+    pass
```

### Comparing `data-dag-0.2.2/docs/Makefile` & `data_dag-0.3.0/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `data-dag-0.2.2/docs/_images/img.png` & `data_dag-0.3.0/docs/_images/img.png`

 * *Files identical despite different names*

### Comparing `data-dag-0.2.2/docs/conf.py` & `data_dag-0.3.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# This file only contains a selection of the most common options. For a full
-# list see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-# -- Path setup --------------------------------------------------------------
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-#
-# import os
-import sys
-from pathlib import Path
-
-sys.path.insert(0, str(Path(__file__).parent.parent))
-
-
-# -- Project information -----------------------------------------------------
-
-project = "data-dag"
-copyright = "2022, David Maxson (david.maxson@rearc.io)"
-author = "David Maxson (david.maxson@rearc.io)"
-
-# The full version, including alpha/beta/rc tags
-release = "0.2.2"
-
-# -- General configuration ---------------------------------------------------
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
-# ones.
-extensions = [
-    "myst_parser",
-    "sphinx.ext.doctest",
-    "sphinx.ext.todo",
-    "sphinx.ext.coverage",
-    "sphinx.ext.napoleon",
-    "sphinxcontrib.mermaid",
-]
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
-
-# -- Options for HTML output -------------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-html_theme = "sphinx_rtd_theme"
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
-
-autodoc_mock_imports = [
-    "airflow",
-    "requests",
-    "pyyaml",
-    "apache-airflow-providers-docker",
-]
+# Configuration file for the Sphinx documentation builder.
+#
+# This file only contains a selection of the most common options. For a full
+# list see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+# -- Path setup --------------------------------------------------------------
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+#
+# import os
+import sys
+from pathlib import Path
+
+sys.path.insert(0, str(Path(__file__).parent.parent))
+
+
+# -- Project information -----------------------------------------------------
+
+project = "data-dag"
+copyright = "2022, David Maxson (david.maxson@rearc.io)"
+author = "David Maxson (david.maxson@rearc.io)"
+
+# The full version, including alpha/beta/rc tags
+release = "0.3.0"
+
+# -- General configuration ---------------------------------------------------
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
+# ones.
+extensions = [
+    "myst_parser",
+    "sphinx.ext.doctest",
+    "sphinx.ext.todo",
+    "sphinx.ext.coverage",
+    "sphinx.ext.napoleon",
+    "sphinxcontrib.mermaid",
+]
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ["_templates"]
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This pattern also affects html_static_path and html_extra_path.
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+
+# -- Options for HTML output -------------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+html_theme = "sphinx_rtd_theme"
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ["_static"]
+
+autodoc_mock_imports = [
+    "airflow",
+    "requests",
+    "pyyaml",
+    "apache-airflow-providers-docker",
+]
```

### Comparing `data-dag-0.2.2/docs/getting_started.md` & `data_dag-0.3.0/docs/getting_started.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,373 +1,373 @@
-# Getting Started
-
-If you are looking to write abstractions, or want to start converting existing DAGs into data-driven DAGs, start by [writing some abstractions](writing_abstractions).
-
-If you already have some abstractions and are looking to start using them to define concrete DAGs, you can jump straight to [using abstractions](using_abstractions).
-
-(writing_abstractions)=
-
-## Writing Abstractions
-
-There are primarily three tiers of abstractions:
-
-- A [DAG factory](dag_factory)
-- An [operator factory](operator_factory)
-- A [component](component)
-
-All three are interfaces over a `pydantic` model, and thus provide much of the same functionality. Let's explore their differences and where each one is helpful.
-
-Common workflows that all abstractions share are:
-
-- Can use `parse_obj` to instantiate the class from a dictionary of data (e.g., from a YAML or JSON file)
-- Can also be directly constructed in-code, just like any other `pydantic`-based class
-- Can have custom field validation that goes well beyond mere type verification or coercion (e.g. checking that a string matches a regex, or that a number is within a given range, or converting a string to an enum)
-- `*args, **kwargs` can often be passed to the primary methods of the various factories; however, it is recommended to make each class's attributes self-contained such that the factory can be executed without any additional arguments.
-- Any classes you write that should not be able to be instantiated should inherit {py:class}`abc.ABC`
-
-(dag_factory)=
-### DAG Factory
-
-A {py:class}`~data_dag.dag_factory.DagFactory` constructs a complete DAG, and contains related DAG metadata (such as schedule, name, and start date). It can compose together operator factories, or it can be entirely self-container, or a mix.
-
-```python
-from typing import List
-from data_dag.dag_factory import DagFactory
-from data_dag.operator_factory import OperatorFactory
-
-
-class SimpleChainDag(DagFactory):
-    ops: List[OperatorFactory]
-
-    def _make_dag(self, *args, **kwargs) -> None:
-        operator_instances = [op.make_operator() for op in self.ops]
-        for a, b in zip(operator_instances[:-1], operator_instances[1:]):
-            a >> b
-```
-
-The base factory class provides definitions for virtually all attributes of {py:class}`~airflow.models.dag.DAG`, such that your custom factory classes need only define any additional attributes needed for your particular DAG. It also provides a convenience implementation of {py:meth}`~data_dag.dag_factory.DagFactory.make_dag` that is effectively the following:
-
-```python
-def make_dag(self, *args, **kwargs):
-    with DAG(**self.dag_args) as dag:
-        self._make_dag(*args, **kwargs)
-    return dag
-```
-
-That is, your custom factory, in general, needs only define {py:meth}`~data_dag.dag_factory.DagFactory._make_dag` to create and link the operators needed for your DAG. See the [example DAG](example_dag) for reference.
-
-(operator_factory)=
-### Operator Factory
-
-```{py:currentmodule} data_dag.operator_factory
-```
-
-An {py:class}`.OperatorFactory` use used to create one or more operators as a pattern. The result should generally be a single operator-like object, or a list (though your calling code will need to know how to handle this properly).
-
-Let's create, as an example, a universal Docker abstraction. We'll start with a simple wrapper around a DockerOperator:
-
-```python
-from data_dag.operator_factory import OperatorFactory
-
-from airflow.providers.docker.operators.docker import DockerOperator
-
-class DockerContainer(OperatorFactory):
-    name: str
-    image: str
-    command: str
-
-    def make_operator(self):
-        return DockerOperator(
-            task_id=f'docker_run_{self.name}',
-            image=self.image,
-            command=self.command,
-        )
-```
-
-To expand this, let's say we wish to re-use this factory to create a kubernetes operator. In this case, we pass kubernetes-specific configuration into the factory, but in practice this might be best handled using external configuration, such as an Airflow connection. We might get the following:
-
-```python
-...
-from typing import Optional, Dict
-
-class DockerContainer(OperatorFactory):
-    ...
-    kubernetes_config: Optional[Dict]
-
-    def make_docker_operator(self):
-        return DockerOperator(...)
-
-    def make_kubernetes_operator(self):
-        return KubernetesPodOperator(..., **self.kubernetes_config)
-
-    def make_operator(self):
-        return self.make_docker_operator()
-```
-
-We could then expose this additional functionality to datafiles by allowing a runtime switch of which operator, regular Docker or Kubernetes, we wish to use.
-
-```python
-import enum
-
-class DockerRuntime(enum.Enum):
-    LOCAL = 'docker'
-    KUBERNETES = 'kubernetes'
-
-class DockerContainer(OperatorFactory):
-    ...
-    runtime: DockerRuntime
-
-    def make_operator(self):
-        if self.runtime == DockerRuntime.LOCAL:
-            return self.make_docker_operator()
-        elif self.runtime == DockerRuntime.KUBERNETES:
-            return self.make_kubernetes_operator()
-```
-
-This could be instantiated with the following data:
-
-```yaml
-image: python3
-command: python -m "print('hello world!')"
-runtime: docker
-```
-
-Let's say, for some reason, you want the ability to build a docker image before running it. This would be easy to integrate into this factory:
-
-```python
-from airflow.utils.task_group import TaskGroup
-
-class DockerContainer(OperatorFactory):
-    ...
-    build_config: Optional[Dict]
-
-    def make_build_operator(self):
-        return BashOperator(
-            task_id='docker build -t {self.image} ...'
-        )
-
-    def make_operator(self):
-        with TaskGroup(group_id=f'run_{self.name}') as group:
-            if self.runtime == DockerRuntime.LOCAL:
-                run_operator = self.make_docker_operator()
-            elif self.runtime == DockerRuntime.KUBERNETES:
-                run_operator = self.make_kubernetes_operator()
-
-            if self.build_config:
-                build_operator = self.make_build_operator()
-                build_operator >> run_operator
-
-        return group
-```
-
-```{note}
-In most cases, when creating multiple operators, you should wrap them up in a {py:class}`airflow.utils.task_group.TaskGroup` so that the result can be treated like a single operator. This makes single operators and compositions of operators indistinguishable from outside your factory, allowing both to be used identically.
-```
-
-This approach allows for factories to become flexible abstractions for common functionality. Additionally, if necessary, it would be straightforward to break an abstraction apart into a composition of multiple simpler factories.
-
-(components)=
-### Components
-
-Not every abstraction directly maps to a DAG or operator, or even a collection of operators. For example, you might want an abstraction for a file in S3 that can be re-used in a variety of other operator factories. This can still be data-driven using {py:class}`.OperatorComponent`:
-
-```python
-from data_dag.operator_factory import OperatorComponent, OperatorFactory
-
-class S3File(OperatorComponent):
-    bucket: str
-    key: str
-
-class CopyFileToS3(OperatorFactory):
-    local_file: str
-    s3_file: S3File
-
-    def make_operator(self):
-        ...
-```
-
-In some cases, it may be desirable to create a very simple component or factory with a single required field. Consider the following trivial example:
-
-```python
-from data_dag.operator_factory import SimpleOperatorComponent, SimpleOperatorFactory
-
-class Path(SimpleOperatorComponent):
-    path: str
-    is_file: bool = True
-
-class CheckFileExists(SimpleOperatorFactory):
-    file_path: Path
-
-    def make_operator(self):
-        return BashOperator(...)
-```
-
-By extending {py:class}`SimpleOperatorComponent` instead of the ordinary {py:class}`OperatorComponent`, this object can be defined in data using just a string rather than a fully dictionary:
-
-```yaml
-file_path: 'path/to/file.txt'
-
-# is equivalent to
-file_path:
-  path: 'path/to/file.txt'
-```
-
-The same is true of {py:class}`.SimpleOperatorFactory` relative to {py:class}`.OperatorFactory`. In fact, since the above sample code uses both a {py:class}`.SimpleOperatorComponent` and a {py:class}`.SimpleOperatorFactory`, the entire operator can be defined using a string rather than a full dictionary:
-
-```python
-CheckFileExists.parse_obj('path/to/file.txt')
-# CheckFileExists(file_path=Path(path='path/to/file.txt', is_file=True))
-```
-
-This allows, in many cases, creating fine-grained types to help keep data organized without sacrificing readability in the data needed to define those types:
-
-```python
-from pydantic import Field
-
-class Schema(SimpleOperatorComponent):
-    name: str
-
-class Column(SimpleOperatorComponent):
-    name: str
-    type: str = 'VARCHAR'
-
-class Table(OperatorFactory):
-    schema_: Schema = Field(alias='schema')
-    name: str
-    columns: List[Column]
-```
-
-```yaml
-schema: 'my_schema'
-name: 'my_table'
-columns:
-- col1
-- col2
-- name: col3
-  type: INTEGER
-```
-
-(using_abstractions)=
-## Using abstractions
-
-All abstractions in {py:mod}`data_dag` are {py:mod}`pydantic` models, meaning that all usual Pydantic features are available. This section is a quick introduction to how those features allow for making data-driven DAGs.
-
-### Interacting with dictionaries
-
-Several common data languages, such as YAML and JSON, serialize collections of simple objects, such as dictionaries, lists, numbers, and strings. Different markup languages support different types and features, so they may each be appropriate under different circumstances.
-
-When these files are loaded into memory, e.g. using `json` or `pyyaml`, the result is an in-memory object comprised of simple data types. Beyond the most trivial use cases, these objects are typically nested and represent a variety of application-specific details. Working directly with these raw dictionaries and lists is likely to involve a lot of boilerplate code; however, if we can map this data into classes, creating useful object instances, we can tie data directly into the functionality related to it.
-
-To do this mapping from in-memory data (no matter where it was loaded from or how it was constructed), `pydantic` allows us to use `MyType.parse_obj(data)` where `MyType` is the factory or component that is represented by the data.
-
-```{note}
-This approach requires that your full top-level data object maps directly onto a Python type. In general, this either isn't hard or is a good idea to add; however, you can also parse out pieces of the data, or restructure it, to match the data types you've defined, especially if you're working with a legacy or shared data schema that isn't easy to modify. Another option is to add [a custom `__init__`](custom_constructor) to a top-level type that knows how to interpret a slightly different input data schema.
-```
-
-For example, consider that you already have the following model:
-
-```python
-from data_dag.operator_factory import OperatorFactory
-from data_dag.dag_factory import DagFactory
-
-from typing import List
-
-class EmailUser(OperatorFactory):
-    email_address: str
-    message_html: str
-
-    def make_operator(self):
-        ...
-
-class EmailAllUsers(DagFactory):
-    emails: List[EmailUser]
-    email_upon_completion: EmailUser
-
-    def _make_dag(self):
-        ...
-```
-
-You could load an email list from the following YAML:
-```yaml
-dag_id: email_users
-schedule_interval: '@weekly'
-
-emails:
-  - email_address: sample@example.com
-    message_html: "<p>Hello, world!</p>"
-  - email_address: sample2@example.com
-    message_html: "<p>Hi, you're our second email</p>"
-email_upon_completion:
-  email_address: admin@my.site.com
-  message_html: "<p>All messages sent</p>"
-```
-
-This would produce the following in-memory object:
-```python
-data = {
-    'dag_id': 'email_users',
-    'schedule_interval': '@weekly',
-    'email_upon_completion': {
-        'email_address': 'admin@my.site.com',
-        'message_html': '<p>All messages sent</p>'
-    },
-    'emails': [
-        {'email_address': 'sample@example.com', 'message_html': '<p>Hello, world!</p>'},
-        {'email_address': 'sample2@example.com', 'message_html': "<p>Hi, you're our second email</p>"}
-    ]
-}
-```
-
-Which we can then parse as:
-```python
-dag_metadata = EmailAllUsers.parse_obj(data)
-# EmailAllUsers(
-#   dag_id='email_users',
-#   ...
-#   emails=[
-#       EmailUser(
-#           email_address='sample@example.com',
-#           message_html='<p>Hello, world!</p>'),
-#       EmailUser(
-#           email_address='sample2@example.com',
-#           message_html="<p>Hi, you're our second email</p>")
-#   ],
-#   email_upon_completion=EmailUser(
-#       email_address='admin@my.site.com',
-#       message_html='<p>All messages sent</p>'
-#   )
-# )
-```
-
-To finally convert that metadata object into an Airflow DAG, we can run `dag_metadata.make_dag()`. Typically, this would be done in a [loader script](loader_script) that's designed to interact cleanly with Airflow.
-
-You can also generate these objects dynamically in-code:
-
-```python
-email_tasks = [
-    EmailUser(email_address=user.email, message_html=message_template.render(user))
-    for user in User.objects.all()
-]
-admin_email_task = EmailUser(
-    email_address=User.objects.get(admin=True),
-    message_html=success_template.render(),
-)
-dag_metadata = EmailAllUsers(
-    dag_id='email_users',
-    schedule='@weekly',
-    emails=email_tasks,
-    email_upon_completion=admin_email_task,
-)
-```
-
-Note that you can also use `pydantic` to map the resulting in-memory objects back into data, either into a dictionary or directly into JSON:
-
-```python
-dag_metadata.dict()
-dag_metadata.json()
-```
-
-This additionally means that you can generate the DAG metadata in one location (say, nightly in a web application), save it out to a known location, then restore it from that location back into your Airflow server to be rendered as a functional DAG. This can be done without direct communication between your servers and without introducing the possibility of arbitrary code execution in your Airflow DAGs, since all code is self-contained and only validated parameters are allowed to be passed around.
-
-```{warning}
-While this is similar, for example, to using JSON serialization to define celery tasks, you must keep in mind that the final result will be entirely rendered, all at once and repeatedly every several seconds, in Airflow, and is thus subject to Airflow's scaling limitations. These limitations mean that individual DAGs should generally be kept fairly small (no more than a few hundred operators) and that the number of DAGs likewise should be kept limited, depending on the scale of your deployment.
-```
+# Getting Started
+
+If you are looking to write abstractions, or want to start converting existing DAGs into data-driven DAGs, start by [writing some abstractions](writing_abstractions).
+
+If you already have some abstractions and are looking to start using them to define concrete DAGs, you can jump straight to [using abstractions](using_abstractions).
+
+(writing_abstractions)=
+
+## Writing Abstractions
+
+There are primarily three tiers of abstractions:
+
+- A [DAG factory](dag_factory)
+- An [operator factory](operator_factory)
+- A [component](component)
+
+All three are interfaces over a `pydantic` model, and thus provide much of the same functionality. Let's explore their differences and where each one is helpful.
+
+Common workflows that all abstractions share are:
+
+- Can use `parse_obj` to instantiate the class from a dictionary of data (e.g., from a YAML or JSON file)
+- Can also be directly constructed in-code, just like any other `pydantic`-based class
+- Can have custom field validation that goes well beyond mere type verification or coercion (e.g. checking that a string matches a regex, or that a number is within a given range, or converting a string to an enum)
+- `*args, **kwargs` can often be passed to the primary methods of the various factories; however, it is recommended to make each class's attributes self-contained such that the factory can be executed without any additional arguments.
+- Any classes you write that should not be able to be instantiated should inherit {py:class}`abc.ABC`
+
+(dag_factory)=
+### DAG Factory
+
+A {py:class}`~data_dag.dag_factory.DagFactory` constructs a complete DAG, and contains related DAG metadata (such as schedule, name, and start date). It can compose together operator factories, or it can be entirely self-container, or a mix.
+
+```python
+from typing import List
+from data_dag.dag_factory import DagFactory
+from data_dag.operator_factory import OperatorFactory
+
+
+class SimpleChainDag(DagFactory):
+    ops: List[OperatorFactory]
+
+    def _make_dag(self, *args, **kwargs) -> None:
+        operator_instances = [op.make_operator() for op in self.ops]
+        for a, b in zip(operator_instances[:-1], operator_instances[1:]):
+            a >> b
+```
+
+The base factory class provides definitions for virtually all attributes of {py:class}`~airflow.models.dag.DAG`, such that your custom factory classes need only define any additional attributes needed for your particular DAG. It also provides a convenience implementation of {py:meth}`~data_dag.dag_factory.DagFactory.make_dag` that is effectively the following:
+
+```python
+def make_dag(self, *args, **kwargs):
+    with DAG(**self.dag_args) as dag:
+        self._make_dag(*args, **kwargs)
+    return dag
+```
+
+That is, your custom factory, in general, needs only define {py:meth}`~data_dag.dag_factory.DagFactory._make_dag` to create and link the operators needed for your DAG. See the [example DAG](example_dag) for reference.
+
+(operator_factory)=
+### Operator Factory
+
+```{py:currentmodule} data_dag.operator_factory
+```
+
+An {py:class}`.OperatorFactory` use used to create one or more operators as a pattern. The result should generally be a single operator-like object, or a list (though your calling code will need to know how to handle this properly).
+
+Let's create, as an example, a universal Docker abstraction. We'll start with a simple wrapper around a DockerOperator:
+
+```python
+from data_dag.operator_factory import OperatorFactory
+
+from airflow.providers.docker.operators.docker import DockerOperator
+
+class DockerContainer(OperatorFactory):
+    name: str
+    image: str
+    command: str
+
+    def make_operator(self):
+        return DockerOperator(
+            task_id=f'docker_run_{self.name}',
+            image=self.image,
+            command=self.command,
+        )
+```
+
+To expand this, let's say we wish to re-use this factory to create a kubernetes operator. In this case, we pass kubernetes-specific configuration into the factory, but in practice this might be best handled using external configuration, such as an Airflow connection. We might get the following:
+
+```python
+...
+from typing import Optional, Dict
+
+class DockerContainer(OperatorFactory):
+    ...
+    kubernetes_config: Optional[Dict]
+
+    def make_docker_operator(self):
+        return DockerOperator(...)
+
+    def make_kubernetes_operator(self):
+        return KubernetesPodOperator(..., **self.kubernetes_config)
+
+    def make_operator(self):
+        return self.make_docker_operator()
+```
+
+We could then expose this additional functionality to datafiles by allowing a runtime switch of which operator, regular Docker or Kubernetes, we wish to use.
+
+```python
+import enum
+
+class DockerRuntime(enum.Enum):
+    LOCAL = 'docker'
+    KUBERNETES = 'kubernetes'
+
+class DockerContainer(OperatorFactory):
+    ...
+    runtime: DockerRuntime
+
+    def make_operator(self):
+        if self.runtime == DockerRuntime.LOCAL:
+            return self.make_docker_operator()
+        elif self.runtime == DockerRuntime.KUBERNETES:
+            return self.make_kubernetes_operator()
+```
+
+This could be instantiated with the following data:
+
+```yaml
+image: python3
+command: python -m "print('hello world!')"
+runtime: docker
+```
+
+Let's say, for some reason, you want the ability to build a docker image before running it. This would be easy to integrate into this factory:
+
+```python
+from airflow.utils.task_group import TaskGroup
+
+class DockerContainer(OperatorFactory):
+    ...
+    build_config: Optional[Dict]
+
+    def make_build_operator(self):
+        return BashOperator(
+            task_id='docker build -t {self.image} ...'
+        )
+
+    def make_operator(self):
+        with TaskGroup(group_id=f'run_{self.name}') as group:
+            if self.runtime == DockerRuntime.LOCAL:
+                run_operator = self.make_docker_operator()
+            elif self.runtime == DockerRuntime.KUBERNETES:
+                run_operator = self.make_kubernetes_operator()
+
+            if self.build_config:
+                build_operator = self.make_build_operator()
+                build_operator >> run_operator
+
+        return group
+```
+
+```{note}
+In most cases, when creating multiple operators, you should wrap them up in a {py:class}`airflow.utils.task_group.TaskGroup` so that the result can be treated like a single operator. This makes single operators and compositions of operators indistinguishable from outside your factory, allowing both to be used identically.
+```
+
+This approach allows for factories to become flexible abstractions for common functionality. Additionally, if necessary, it would be straightforward to break an abstraction apart into a composition of multiple simpler factories.
+
+(components)=
+### Components
+
+Not every abstraction directly maps to a DAG or operator, or even a collection of operators. For example, you might want an abstraction for a file in S3 that can be re-used in a variety of other operator factories. This can still be data-driven using {py:class}`.OperatorComponent`:
+
+```python
+from data_dag.operator_factory import OperatorComponent, OperatorFactory
+
+class S3File(OperatorComponent):
+    bucket: str
+    key: str
+
+class CopyFileToS3(OperatorFactory):
+    local_file: str
+    s3_file: S3File
+
+    def make_operator(self):
+        ...
+```
+
+In some cases, it may be desirable to create a very simple component or factory with a single required field. Consider the following trivial example:
+
+```python
+from data_dag.operator_factory import SimpleOperatorComponent, SimpleOperatorFactory
+
+class Path(SimpleOperatorComponent):
+    path: str
+    is_file: bool = True
+
+class CheckFileExists(SimpleOperatorFactory):
+    file_path: Path
+
+    def make_operator(self):
+        return BashOperator(...)
+```
+
+By extending {py:class}`SimpleOperatorComponent` instead of the ordinary {py:class}`OperatorComponent`, this object can be defined in data using just a string rather than a fully dictionary:
+
+```yaml
+file_path: 'path/to/file.txt'
+
+# is equivalent to
+file_path:
+  path: 'path/to/file.txt'
+```
+
+The same is true of {py:class}`.SimpleOperatorFactory` relative to {py:class}`.OperatorFactory`. In fact, since the above sample code uses both a {py:class}`.SimpleOperatorComponent` and a {py:class}`.SimpleOperatorFactory`, the entire operator can be defined using a string rather than a full dictionary:
+
+```python
+CheckFileExists.parse_obj('path/to/file.txt')
+# CheckFileExists(file_path=Path(path='path/to/file.txt', is_file=True))
+```
+
+This allows, in many cases, creating fine-grained types to help keep data organized without sacrificing readability in the data needed to define those types:
+
+```python
+from pydantic import Field
+
+class Schema(SimpleOperatorComponent):
+    name: str
+
+class Column(SimpleOperatorComponent):
+    name: str
+    type: str = 'VARCHAR'
+
+class Table(OperatorFactory):
+    schema_: Schema = Field(alias='schema')
+    name: str
+    columns: List[Column]
+```
+
+```yaml
+schema: 'my_schema'
+name: 'my_table'
+columns:
+- col1
+- col2
+- name: col3
+  type: INTEGER
+```
+
+(using_abstractions)=
+## Using abstractions
+
+All abstractions in {py:mod}`data_dag` are {py:mod}`pydantic` models, meaning that all usual Pydantic features are available. This section is a quick introduction to how those features allow for making data-driven DAGs.
+
+### Interacting with dictionaries
+
+Several common data languages, such as YAML and JSON, serialize collections of simple objects, such as dictionaries, lists, numbers, and strings. Different markup languages support different types and features, so they may each be appropriate under different circumstances.
+
+When these files are loaded into memory, e.g. using `json` or `pyyaml`, the result is an in-memory object comprised of simple data types. Beyond the most trivial use cases, these objects are typically nested and represent a variety of application-specific details. Working directly with these raw dictionaries and lists is likely to involve a lot of boilerplate code; however, if we can map this data into classes, creating useful object instances, we can tie data directly into the functionality related to it.
+
+To do this mapping from in-memory data (no matter where it was loaded from or how it was constructed), `pydantic` allows us to use `MyType.parse_obj(data)` where `MyType` is the factory or component that is represented by the data.
+
+```{note}
+This approach requires that your full top-level data object maps directly onto a Python type. In general, this either isn't hard or is a good idea to add; however, you can also parse out pieces of the data, or restructure it, to match the data types you've defined, especially if you're working with a legacy or shared data schema that isn't easy to modify. Another option is to add [a custom `__init__`](custom_constructor) to a top-level type that knows how to interpret a slightly different input data schema.
+```
+
+For example, consider that you already have the following model:
+
+```python
+from data_dag.operator_factory import OperatorFactory
+from data_dag.dag_factory import DagFactory
+
+from typing import List
+
+class EmailUser(OperatorFactory):
+    email_address: str
+    message_html: str
+
+    def make_operator(self):
+        ...
+
+class EmailAllUsers(DagFactory):
+    emails: List[EmailUser]
+    email_upon_completion: EmailUser
+
+    def _make_dag(self):
+        ...
+```
+
+You could load an email list from the following YAML:
+```yaml
+dag_id: email_users
+schedule_interval: '@weekly'
+
+emails:
+  - email_address: sample@example.com
+    message_html: "<p>Hello, world!</p>"
+  - email_address: sample2@example.com
+    message_html: "<p>Hi, you're our second email</p>"
+email_upon_completion:
+  email_address: admin@my.site.com
+  message_html: "<p>All messages sent</p>"
+```
+
+This would produce the following in-memory object:
+```python
+data = {
+    'dag_id': 'email_users',
+    'schedule_interval': '@weekly',
+    'email_upon_completion': {
+        'email_address': 'admin@my.site.com',
+        'message_html': '<p>All messages sent</p>'
+    },
+    'emails': [
+        {'email_address': 'sample@example.com', 'message_html': '<p>Hello, world!</p>'},
+        {'email_address': 'sample2@example.com', 'message_html': "<p>Hi, you're our second email</p>"}
+    ]
+}
+```
+
+Which we can then parse as:
+```python
+dag_metadata = EmailAllUsers.parse_obj(data)
+# EmailAllUsers(
+#   dag_id='email_users',
+#   ...
+#   emails=[
+#       EmailUser(
+#           email_address='sample@example.com',
+#           message_html='<p>Hello, world!</p>'),
+#       EmailUser(
+#           email_address='sample2@example.com',
+#           message_html="<p>Hi, you're our second email</p>")
+#   ],
+#   email_upon_completion=EmailUser(
+#       email_address='admin@my.site.com',
+#       message_html='<p>All messages sent</p>'
+#   )
+# )
+```
+
+To finally convert that metadata object into an Airflow DAG, we can run `dag_metadata.make_dag()`. Typically, this would be done in a [loader script](loader_script) that's designed to interact cleanly with Airflow.
+
+You can also generate these objects dynamically in-code:
+
+```python
+email_tasks = [
+    EmailUser(email_address=user.email, message_html=message_template.render(user))
+    for user in User.objects.all()
+]
+admin_email_task = EmailUser(
+    email_address=User.objects.get(admin=True),
+    message_html=success_template.render(),
+)
+dag_metadata = EmailAllUsers(
+    dag_id='email_users',
+    schedule='@weekly',
+    emails=email_tasks,
+    email_upon_completion=admin_email_task,
+)
+```
+
+Note that you can also use `pydantic` to map the resulting in-memory objects back into data, either into a dictionary or directly into JSON:
+
+```python
+dag_metadata.dict()
+dag_metadata.json()
+```
+
+This additionally means that you can generate the DAG metadata in one location (say, nightly in a web application), save it out to a known location, then restore it from that location back into your Airflow server to be rendered as a functional DAG. This can be done without direct communication between your servers and without introducing the possibility of arbitrary code execution in your Airflow DAGs, since all code is self-contained and only validated parameters are allowed to be passed around.
+
+```{warning}
+While this is similar, for example, to using JSON serialization to define celery tasks, you must keep in mind that the final result will be entirely rendered, all at once and repeatedly every several seconds, in Airflow, and is thus subject to Airflow's scaling limitations. These limitations mean that individual DAGs should generally be kept fairly small (no more than a few hundred operators) and that the number of DAGs likewise should be kept limited, depending on the scale of your deployment.
+```
```

### Comparing `data-dag-0.2.2/docs/make.bat` & `data_dag-0.3.0/docs/make.bat`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set SOURCEDIR=.
-set BUILDDIR=_build
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.https://www.sphinx-doc.org/
-	exit /b 1
-)
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set SOURCEDIR=.
+set BUILDDIR=_build
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.https://www.sphinx-doc.org/
+	exit /b 1
+)
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+
+:end
+popd
```

### Comparing `data-dag-0.2.2/docs/overview.md` & `data_dag-0.3.0/docs/overview.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-(overview_base)=
-# Overview
-
-`data-dag` provides a variety of tools to simplify the process of writing data-defined Airflow DAGs. This library was created to simplify and formalize the approach introduced [in this article](https://engineering.rearc.io/posts/2022_05_09-airflow_operator_factory_pattern/).
-
-This approach is incredibly useful when writing a large number of DAGs that rely, either in part or entirely, on shareable primitives. A primitive may or may not be a single Airflow operator. For example, you might want the following primitive to only create a table if it doesn't exist:
-
-```{mermaid}
-graph LR
-    a["Check if table exists"] --> b["Create table (all_failed)"] --> c["Done (one_success)"]
-    a --> c
-```
-
-While it is certainly possible to write a more complicated operator that performs this logic, it's often easier, clearer, and more maintainable to work with existing operators. Additionally, writing factories like this is easy to stack to build multiple levels of abstractions, or to re-use components across multiple different abstractions.
-
-This pattern, in addition to simplifying and standardizing how multiple DAGs can be defined, also provides a framework for writing re-usable abstractions and operator compositions (for example, as a shareable plugin). This is because factories defined using `data-dag` can be defined in-code too, not just using data.
-
-`data-dag` is written on top of the excellent [`pydantic` library](https://pydantic-docs.helpmanual.io/), providing automatic type coercion, field validation, and serialization and deserialization against a variety of data formats.
-
-## Example
-
-Re-usable operator and DAG template can be stored in a central location, such as a custom Airflow plugin (or a package within `dags/` works fine too):
-
-(example_dag)=
-```python
-# plugins/my_factories/download.py
-
-from data_dag.operator_factory import OperatorFactory
-from data_dag.dag_factory import DagFactory
-
-from urllib.request import urlretrieve
-from typing import List
-from airflow.operators.dummy import DummyOperator
-from airflow.providers.http.sensors.http import HttpSensor
-from airflow.operators.python import PythonOperator
-from airflow.utils.task_group import TaskGroup
-
-
-class DownloadOperator(OperatorFactory):
-    """An operator factory for safely downloading files to a known location"""
-
-    name: str
-    url: str
-    path: str
-
-    def make_operator(self):
-        with TaskGroup(group_id=f'download_{self.name}') as group:
-            check = HttpSensor(
-                task_id='check_exists',
-                endpoint=self.url
-            )
-            download = PythonOperator(
-                task_id=f'download',
-                python_callable=lambda: urlretrieve(self.url, self.path)
-            )
-            check >> download
-
-        return group
-
-
-class DownloaderDag(DagFactory):
-    """A DAG factory for producing simple DAGs that just download a bunch of files"""
-
-    downloads: List[DownloadOperator]
-
-    def _make_dag(self):
-        start = DummyOperator(task_id='start')
-        end = DummyOperator(task_id='end')
-
-        for download in self.downloads:
-            start >> download.make_operator() >> end
-```
-
-Then a definition for a particular DAG can live in a data file:
-
-```yaml
-# dags/yaml/sample_dag.yaml
-
-dag_id: sample_dag
-description: An example of how to write a data-driven DAG
-schedule_interval: '@daily'
-start_date: '2020-01-01T00:00:00'
-downloads:
-- name: data
-  url: https://www.example.com/data.zip
-  path: data.zip
-- name: manifest
-  url: https://www.example.com/manifest.json
-  path: manifest.json
-```
-
-That data file can then be loaded into a DAG. Per Airflow's requirements, this must be done in a Python file located in `dags/` and the result must be saved into a uniquely named global variable. The simplest possible example is this:
-
-```python
-# dags/sample_dag.py
-
-from yaml import safe_load
-from my_factories.download import DownloaderDag
-
-with open('yaml/sample_dag.yaml', 'r') as f:
-    dag_data = safe_load(f)
-
-dag = DownloaderDag.parse_obj(dag_data).make_dag()
-```
-
-![img.png](_images/img.png)
-
-## Multiple DAGs
-
-Obviously, using a template isn't much use if you only fill it in once. Here's a simple example of a loader that will load any number of YML files from a folder and publish each one as a DAG in Airflow:
-
-(loader_script)=
-```python
-# dags/load_yml_files.py
-
-from pathlib import Path
-from airflow import DAG
-import yaml
-from my_factories import BaseDag
-
-dag_dir = Path(__file__).parent
-
-# For each YAML file in a particular directory...
-for yaml_file_path in dag_dir.glob('typical_dags/**.yml'):
-    with open(yaml_file_path) as f:
-        dag_metadata = yaml.safe_load(f)
-
-    # ... generate a DAG from that metadata
-    dag_metadata_obj = BaseDag.parse_obj(dag_metadata)
-    dag = dag_metadata_obj.make_dag()
-
-    # See https://www.astronomer.io/guides/dynamically-generating-dags/
-    globals()[dag_metadata_obj.dag_id] = dag
-```
-
-## Use Cases
-
-### Custom No-Code DAGs
-
-Defining dataflows without Python code means that anyone can write a dataflow, not just programmers.
-
-Since the abstractions are easy to write, or can be readily shared with plugins, it's straightforward to come up with the abstractions useful to your business case. Focus your DAG authoring on what matters to you, and abstract away everything else.
-
-### Write and upgrade DAGs centrally
-
-The actual DAG code that Airflow sees is generated by shared Python code. That means you can write abstractions once and re-use them multiple times in a standard pattern. Also, if a pattern is later discovered to be lacking, or needs extra features, it can be upgraded in-place and all DAGs that rely on it will automatically be upgraded.
-
-This also provides a standard way for testing DAGs, since now DAGs are composed of components which can more easily be unit tested.
-
-### Re-use patterns, not just operators
-
-Operators are great, and custom operators aren't hard to write, but often more complicated tasks are better defined as patterns of operators rather than complicated single operators. By relying on a factory pattern rather than expecting data to map directly to operators, data-driven DAGs maintain transparency in the DAG's execution without requiring that the DAG authoring itself be complicated.
-
-### Secure DAG authoring
-
-If desired, direct Python access to the DAGs folder can be restricted and only data-driven DAGs may be submitted by authors to a different location. This would allow a small number of admins to control the exact code and configuration of execution on the Airflow server without limiting the ability of various external authors to contribute business-relevant dataflows.
-
-### Generate DAGs without code generation
-
-Some DAGs are best generated by code, e.g. to loop through a long list of URLs or to leverage data in a database. With Airflow, this must either occur within an operator in a static DAG or at DAG creation time. Using data-driven DAGs makes it easy to programmatically generate the DAG by having some code generate and export a data file.
-
-```{note}
-Non DAG-oriented orchetsration engines, such as Prefect, don't necessarily have this same limitation. However, DAGs have a tremendous number of advantages in many ways and remain heavily used industry-wide, so empowering their use is worthwhile despite such limitations.
-```
-
-### Introspect dataflows
-
-There are a variety of reasons it may be helpful to analye the dataflows deployed on a given Airflow server. Perhaps for refactoring, or for determining feature usage, or to figure out which dataflows interact with which files. Whatever the reason, this is normally near-impossible to automate since each DAG is arbitrary Python code that produces complicated, Airflow-specific objects. With data-driven DAGs, though, it's trivial to open the data files and investigate them; this can be done either directly, on the dictionaries, lists, etc. represented by the data files, or by loading them into their appropriate metadata objects and introspecting those. All this can be done without needing Airflow to be running at all, since no operators or DAGs need be generated in this process.
-
-### And you can still write Python DAGs too
-
-Interested, but not able or interested in diving head-first into using data-driven DAGs? There's no need to make any sort of commitment. All factories can be used by themselves, piecemeal, either instantiated from data or from code. It doesn't matter. The design put forward by `data-dag` only enables data-driven DAGs, but it's little more than a standard way of mapping minimal, business-specific metadata into Airflow constructs. Re-use your abstractions within Python DAGs, use standard Airflow operators within a DAG factory, or whatever is simplest for you. Let some DAGs be fully data-defined, and others be custom-written. Whatever works best for your use case: using `data-dag` only simplifies your DAG authoring, it doesn't in any way limit how you do so.
+(overview_base)=
+# Overview
+
+`data-dag` provides a variety of tools to simplify the process of writing data-defined Airflow DAGs. This library was created to simplify and formalize the approach introduced [in this article](https://engineering.rearc.io/posts/2022_05_09-airflow_operator_factory_pattern/).
+
+This approach is incredibly useful when writing a large number of DAGs that rely, either in part or entirely, on shareable primitives. A primitive may or may not be a single Airflow operator. For example, you might want the following primitive to only create a table if it doesn't exist:
+
+```{mermaid}
+graph LR
+    a["Check if table exists"] --> b["Create table (all_failed)"] --> c["Done (one_success)"]
+    a --> c
+```
+
+While it is certainly possible to write a more complicated operator that performs this logic, it's often easier, clearer, and more maintainable to work with existing operators. Additionally, writing factories like this is easy to stack to build multiple levels of abstractions, or to re-use components across multiple different abstractions.
+
+This pattern, in addition to simplifying and standardizing how multiple DAGs can be defined, also provides a framework for writing re-usable abstractions and operator compositions (for example, as a shareable plugin). This is because factories defined using `data-dag` can be defined in-code too, not just using data.
+
+`data-dag` is written on top of the excellent [`pydantic` library](https://pydantic-docs.helpmanual.io/), providing automatic type coercion, field validation, and serialization and deserialization against a variety of data formats.
+
+## Example
+
+Re-usable operator and DAG template can be stored in a central location, such as a custom Airflow plugin (or a package within `dags/` works fine too):
+
+(example_dag)=
+```python
+# plugins/my_factories/download.py
+
+from data_dag.operator_factory import OperatorFactory
+from data_dag.dag_factory import DagFactory
+
+from urllib.request import urlretrieve
+from typing import List
+from airflow.operators.dummy import DummyOperator
+from airflow.providers.http.sensors.http import HttpSensor
+from airflow.operators.python import PythonOperator
+from airflow.utils.task_group import TaskGroup
+
+
+class DownloadOperator(OperatorFactory):
+    """An operator factory for safely downloading files to a known location"""
+
+    name: str
+    url: str
+    path: str
+
+    def make_operator(self):
+        with TaskGroup(group_id=f'download_{self.name}') as group:
+            check = HttpSensor(
+                task_id='check_exists',
+                endpoint=self.url
+            )
+            download = PythonOperator(
+                task_id=f'download',
+                python_callable=lambda: urlretrieve(self.url, self.path)
+            )
+            check >> download
+
+        return group
+
+
+class DownloaderDag(DagFactory):
+    """A DAG factory for producing simple DAGs that just download a bunch of files"""
+
+    downloads: List[DownloadOperator]
+
+    def _make_dag(self):
+        start = DummyOperator(task_id='start')
+        end = DummyOperator(task_id='end')
+
+        for download in self.downloads:
+            start >> download.make_operator() >> end
+```
+
+Then a definition for a particular DAG can live in a data file:
+
+```yaml
+# dags/yaml/sample_dag.yaml
+
+dag_id: sample_dag
+description: An example of how to write a data-driven DAG
+schedule_interval: '@daily'
+start_date: '2020-01-01T00:00:00'
+downloads:
+- name: data
+  url: https://www.example.com/data.zip
+  path: data.zip
+- name: manifest
+  url: https://www.example.com/manifest.json
+  path: manifest.json
+```
+
+That data file can then be loaded into a DAG. Per Airflow's requirements, this must be done in a Python file located in `dags/` and the result must be saved into a uniquely named global variable. The simplest possible example is this:
+
+```python
+# dags/sample_dag.py
+
+from yaml import safe_load
+from my_factories.download import DownloaderDag
+
+with open('yaml/sample_dag.yaml', 'r') as f:
+    dag_data = safe_load(f)
+
+dag = DownloaderDag.parse_obj(dag_data).make_dag()
+```
+
+![img.png](_images/img.png)
+
+## Multiple DAGs
+
+Obviously, using a template isn't much use if you only fill it in once. Here's a simple example of a loader that will load any number of YML files from a folder and publish each one as a DAG in Airflow:
+
+(loader_script)=
+```python
+# dags/load_yml_files.py
+
+from pathlib import Path
+from airflow import DAG
+import yaml
+from my_factories import BaseDag
+
+dag_dir = Path(__file__).parent
+
+# For each YAML file in a particular directory...
+for yaml_file_path in dag_dir.glob('typical_dags/**.yml'):
+    with open(yaml_file_path) as f:
+        dag_metadata = yaml.safe_load(f)
+
+    # ... generate a DAG from that metadata
+    dag_metadata_obj = BaseDag.parse_obj(dag_metadata)
+    dag = dag_metadata_obj.make_dag()
+
+    # See https://www.astronomer.io/guides/dynamically-generating-dags/
+    globals()[dag_metadata_obj.dag_id] = dag
+```
+
+## Use Cases
+
+### Custom No-Code DAGs
+
+Defining dataflows without Python code means that anyone can write a dataflow, not just programmers.
+
+Since the abstractions are easy to write, or can be readily shared with plugins, it's straightforward to come up with the abstractions useful to your business case. Focus your DAG authoring on what matters to you, and abstract away everything else.
+
+### Write and upgrade DAGs centrally
+
+The actual DAG code that Airflow sees is generated by shared Python code. That means you can write abstractions once and re-use them multiple times in a standard pattern. Also, if a pattern is later discovered to be lacking, or needs extra features, it can be upgraded in-place and all DAGs that rely on it will automatically be upgraded.
+
+This also provides a standard way for testing DAGs, since now DAGs are composed of components which can more easily be unit tested.
+
+### Re-use patterns, not just operators
+
+Operators are great, and custom operators aren't hard to write, but often more complicated tasks are better defined as patterns of operators rather than complicated single operators. By relying on a factory pattern rather than expecting data to map directly to operators, data-driven DAGs maintain transparency in the DAG's execution without requiring that the DAG authoring itself be complicated.
+
+### Secure DAG authoring
+
+If desired, direct Python access to the DAGs folder can be restricted and only data-driven DAGs may be submitted by authors to a different location. This would allow a small number of admins to control the exact code and configuration of execution on the Airflow server without limiting the ability of various external authors to contribute business-relevant dataflows.
+
+### Generate DAGs without code generation
+
+Some DAGs are best generated by code, e.g. to loop through a long list of URLs or to leverage data in a database. With Airflow, this must either occur within an operator in a static DAG or at DAG creation time. Using data-driven DAGs makes it easy to programmatically generate the DAG by having some code generate and export a data file.
+
+```{note}
+Non DAG-oriented orchetsration engines, such as Prefect, don't necessarily have this same limitation. However, DAGs have a tremendous number of advantages in many ways and remain heavily used industry-wide, so empowering their use is worthwhile despite such limitations.
+```
+
+### Introspect dataflows
+
+There are a variety of reasons it may be helpful to analye the dataflows deployed on a given Airflow server. Perhaps for refactoring, or for determining feature usage, or to figure out which dataflows interact with which files. Whatever the reason, this is normally near-impossible to automate since each DAG is arbitrary Python code that produces complicated, Airflow-specific objects. With data-driven DAGs, though, it's trivial to open the data files and investigate them; this can be done either directly, on the dictionaries, lists, etc. represented by the data files, or by loading them into their appropriate metadata objects and introspecting those. All this can be done without needing Airflow to be running at all, since no operators or DAGs need be generated in this process.
+
+### And you can still write Python DAGs too
+
+Interested, but not able or interested in diving head-first into using data-driven DAGs? There's no need to make any sort of commitment. All factories can be used by themselves, piecemeal, either instantiated from data or from code. It doesn't matter. The design put forward by `data-dag` only enables data-driven DAGs, but it's little more than a standard way of mapping minimal, business-specific metadata into Airflow constructs. Re-use your abstractions within Python DAGs, use standard Airflow operators within a DAG factory, or whatever is simplest for you. Let some DAGs be fully data-defined, and others be custom-written. Whatever works best for your use case: using `data-dag` only simplifies your DAG authoring, it doesn't in any way limit how you do so.
```

### Comparing `data-dag-0.2.2/docs/usage/operator_factory.md` & `data_dag-0.3.0/docs/usage/operator_factory.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# Operator Factory
-
-```{py:currentmodule} data_dag.operator_factory
-```
-
-See {py:class}`~data_dag.operator_factory.OperatorFactory`
-
-For an example, see [the getting started guide](operator_factory).
-
-(custom_constructor)=
-## Re-Interpreting Data
-
-Ultimately, each object is created by its constructor being called. Since each factory and component is fundamentally a {py:class}`pydantic.BaseModel` object, its fields are defined at the class level, but how those fields get populated is customizable.
-
-Let's say you have an old class like this::
-
-    class Url(OperatorComponent):
-        url: str
-
-and then, at some point, you decide you want to update it to store the pieces of the url, like this::
-
-    class Url(OperatorComponent):
-        scheme: str
-        host: str
-        path: str
-        params: Dict[str, Any] = {}
-
-To avoid breaking existing code or data, you can write a custom constructor to permit old-style data definitions to continue to work::
-
-    class Url(OperatorComponent):
-        ...
-
-        def __init__(self, url):
-            parsed = urllib.parse.urlparse(url)
-            super().__init__(scheme=parsed.scheme, host=parsed.host, ...)
-
-This allows separating the input data definition for a type from its internal representation.
-
-Note that, in many cases, {py:mod}`pydantic` may already have features that allow a variety of tweaks without needing a custom constructor. Single- and multi-field validation and transformation, amongst other features, are well-supported.
-
-(component)=
-## Components
-
-{py:class}`OperatorFactory` defines a standard interface for how the operator should be constructed from the metadata, and provides the `task_id` attribute by default to facilitate that. {py:class}`OperatorComponent`, on the other hand, is currently just a proxy for {py:class}`pydantic.BaseModel` to encourage a consistent pattern for sharing data and validation across a DAG. This may change in the future.
-
-## Task ID's and Groups
-
-{py:class}`OperatorFactory` provides some pre-baked tooling to help define Task IDs.
-
-- {py:class}`OperatorFactory` inherently has an optional `task_id: Optional[str]` attribute which can be set in data. To disallow using this, you can define a validator function that ensures this is empty.
-- The {py:meth}`~OperatorFactory.default_task_id` property can be overridden to provide a default value if no task ID is specified. This is recommended to implement where practical.
-- The {py:meth}`~OperatorFactory.get_task_id` method provides either the custom task ID, if provided, or the default if possible.
-
-If implementing an operator pattern wrapped as a group (using {py:meth}`~OperatorFactory._make_operators`), then the task ID is used as the group ID, and the inner operator task ID's need only be unique within that context.
+# Operator Factory
+
+```{py:currentmodule} data_dag.operator_factory
+```
+
+See {py:class}`~data_dag.operator_factory.OperatorFactory`
+
+For an example, see [the getting started guide](operator_factory).
+
+(custom_constructor)=
+## Re-Interpreting Data
+
+Ultimately, each object is created by its constructor being called. Since each factory and component is fundamentally a {py:class}`pydantic.BaseModel` object, its fields are defined at the class level, but how those fields get populated is customizable.
+
+Let's say you have an old class like this::
+
+    class Url(OperatorComponent):
+        url: str
+
+and then, at some point, you decide you want to update it to store the pieces of the url, like this::
+
+    class Url(OperatorComponent):
+        scheme: str
+        host: str
+        path: str
+        params: Dict[str, Any] = {}
+
+To avoid breaking existing code or data, you can write a custom constructor to permit old-style data definitions to continue to work::
+
+    class Url(OperatorComponent):
+        ...
+
+        def __init__(self, url):
+            parsed = urllib.parse.urlparse(url)
+            super().__init__(scheme=parsed.scheme, host=parsed.host, ...)
+
+This allows separating the input data definition for a type from its internal representation.
+
+Note that, in many cases, {py:mod}`pydantic` may already have features that allow a variety of tweaks without needing a custom constructor. Single- and multi-field validation and transformation, amongst other features, are well-supported.
+
+(component)=
+## Components
+
+{py:class}`OperatorFactory` defines a standard interface for how the operator should be constructed from the metadata, and provides the `task_id` attribute by default to facilitate that. {py:class}`OperatorComponent`, on the other hand, is currently just a proxy for {py:class}`pydantic.BaseModel` to encourage a consistent pattern for sharing data and validation across a DAG. This may change in the future.
+
+## Task ID's and Groups
+
+{py:class}`OperatorFactory` provides some pre-baked tooling to help define Task IDs.
+
+- {py:class}`OperatorFactory` inherently has an optional `task_id: Optional[str]` attribute which can be set in data. To disallow using this, you can define a validator function that ensures this is empty.
+- The {py:meth}`~OperatorFactory.default_task_id` property can be overridden to provide a default value if no task ID is specified. This is recommended to implement where practical.
+- The {py:meth}`~OperatorFactory.get_task_id` method provides either the custom task ID, if provided, or the default if possible.
+
+If implementing an operator pattern wrapped as a group (using {py:meth}`~OperatorFactory._make_operators`), then the task ID is used as the group ID, and the inner operator task ID's need only be unique within that context.
```

### Comparing `data-dag-0.2.2/tests/test_dag_factory.py` & `data_dag-0.3.0/tests/test_dag_factory.py`

 * *Files identical despite different names*

### Comparing `data-dag-0.2.2/tests/test_dynamic_operator_factory.py` & `data_dag-0.3.0/tests/test_dynamic_operator_factory.py`

 * *Files identical despite different names*

### Comparing `data-dag-0.2.2/tests/test_operator_factory.py` & `data_dag-0.3.0/tests/test_operator_factory.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-from datetime import datetime
-from typing import Any, Dict, Optional
-
-import pytest
-from airflow.operators.dummy import DummyOperator
-
-from data_dag.operator_factory import (
-    OperatorFactory,
-    SimpleOperatorComponent,
-    SimpleOperatorFactory,
-)
-from data_dag.operator_factory.base import BaseOperatorFactory
-
-_junk_dag_kwargs = dict(
-    dag_id="junk",
-    schedule_interval="@daily",
-    start_date=datetime.today(),
-)
-
-
-def test_basic():
-    class SampleOp(OperatorFactory):
-        to_add: float
-
-        def make_operator(self, *args, **kwargs):
-            return DummyOperator(task_id=f"Add_{self.to_add}")
-
-    data = {"to_add": 5}
-    op = SampleOp.parse_obj(data)
-    airflow_op = op.make_operator()
-    assert isinstance(airflow_op, DummyOperator)
-    assert airflow_op.task_id == "Add_5.0"
-
-
-def test_not_implemented1():
-    class SampleOp(OperatorFactory):
-        pass
-
-    with pytest.raises(NotImplementedError):
-        SampleOp().default_task_id
-
-
-def test_not_implemented2():
-    class SampleOp(OperatorFactory):
-        @property
-        def default_task_id(self) -> str:
-            return "junk"
-
-    from data_dag.dag_factory import DagFactory
-
-    class SampleDag(DagFactory):
-        def _make_dag(self):
-            SampleOp().make_operator()
-
-    with pytest.raises(NotImplementedError):
-        SampleDag(**_junk_dag_kwargs).make_dag()
-
-
-def test_not_implemented3():
-    class SampleOp(BaseOperatorFactory):
-        pass
-
-    with pytest.raises(NotImplementedError):
-        SampleOp().make_operator()
-
-
-def test_failure_direct_instantiation():
-    pytest.raises(NotImplementedError, OperatorFactory.parse_obj({}).make_operator)
-
-
-def test_simple():
-    """Tests that SimpleOperatorFactory works as intended"""
-
-    class SampleOp(SimpleOperatorFactory):
-        i: int
-        flag: bool = True
-
-        def make_operator(self):
-            raise NotImplementedError()
-
-    op = SampleOp.parse_obj(5)
-    assert isinstance(op, SampleOp)
-    assert op.i == 5
-    assert op.flag is True
-
-    op = SampleOp.parse_obj({"i": 5})
-    assert isinstance(op, SampleOp)
-    assert op.i == 5
-    assert op.flag is True
-
-    op = SampleOp.parse_obj({"i": 5, "flag": False})
-    assert isinstance(op, SampleOp)
-    assert op.i == 5
-    assert op.flag is False
-
-
-def test_simple_failure_multiple_fields():
-    with pytest.raises(TypeError):
-
-        class _SampleOp(SimpleOperatorComponent):
-            a: int
-            b: int
-
-
-def test_simple_failure_dict_field():
-    class SampleOp(SimpleOperatorComponent):
-        d: Dict[str, Any]
-
-    with pytest.raises(NotImplementedError):
-        SampleOp.parse_obj(dict())
-
-
-def test_none_not_the_same_as_undefined():
-    class SampleOp(SimpleOperatorComponent):
-        a: int
-        b: Optional[int]  # Defaults to None, so there's only one undefined field
-
-
-def test_task_id_and_task_group():
-    class SampleOp(OperatorFactory):
-        i: int
-
-        @property
-        def default_task_id(self):
-            return f"add_{self.i}"
-
-        def _make_operators(self, *args, **kwargs) -> None:
-            load_value = DummyOperator(task_id="load")
-            compute_result = DummyOperator(task_id="compute")
-            finish = DummyOperator(task_id="finish")
-
-            load_value >> compute_result >> finish
-
-    from data_dag.dag_factory import DagFactory
-
-    class SampleDag(DagFactory):
-        def _make_dag(self):
-            SampleOp(i=3).make_operator()
-
-    dag = SampleDag(**_junk_dag_kwargs).make_dag()
-    load, compute, finish = dag.tasks
-    assert load.task_id == "add_3.load"
-    assert compute.task_id == "add_3.compute"
-    assert finish.task_id == "add_3.finish"
+from datetime import datetime
+from typing import Any, Dict, Optional
+
+import pytest
+from airflow.operators.dummy import DummyOperator
+
+from data_dag.operator_factory import (
+    OperatorFactory,
+    SimpleOperatorComponent,
+    SimpleOperatorFactory,
+)
+from data_dag.operator_factory.base import BaseOperatorFactory
+
+_junk_dag_kwargs = dict(
+    dag_id="junk",
+    schedule_interval="@daily",
+    start_date=datetime.today(),
+)
+
+
+def test_basic():
+    class SampleOp(OperatorFactory):
+        to_add: float
+
+        def make_operator(self, *args, **kwargs):
+            return DummyOperator(task_id=f"Add_{self.to_add}")
+
+    data = {"to_add": 5}
+    op = SampleOp.parse_obj(data)
+    airflow_op = op.make_operator()
+    assert isinstance(airflow_op, DummyOperator)
+    assert airflow_op.task_id == "Add_5.0"
+
+
+def test_not_implemented1():
+    class SampleOp(OperatorFactory):
+        pass
+
+    with pytest.raises(NotImplementedError):
+        SampleOp().default_task_id
+
+
+def test_not_implemented2():
+    class SampleOp(OperatorFactory):
+        @property
+        def default_task_id(self) -> str:
+            return "junk"
+
+    from data_dag.dag_factory import DagFactory
+
+    class SampleDag(DagFactory):
+        def _make_dag(self):
+            SampleOp().make_operator()
+
+    with pytest.raises(NotImplementedError):
+        SampleDag(**_junk_dag_kwargs).make_dag()
+
+
+def test_not_implemented3():
+    class SampleOp(BaseOperatorFactory):
+        pass
+
+    with pytest.raises(NotImplementedError):
+        SampleOp().make_operator()
+
+
+def test_failure_direct_instantiation():
+    pytest.raises(NotImplementedError, OperatorFactory.parse_obj({}).make_operator)
+
+
+def test_simple():
+    """Tests that SimpleOperatorFactory works as intended"""
+
+    class SampleOp(SimpleOperatorFactory):
+        i: int
+        flag: bool = True
+
+        def make_operator(self):
+            raise NotImplementedError()
+
+    op = SampleOp.parse_obj(5)
+    assert isinstance(op, SampleOp)
+    assert op.i == 5
+    assert op.flag is True
+
+    op = SampleOp.parse_obj({"i": 5})
+    assert isinstance(op, SampleOp)
+    assert op.i == 5
+    assert op.flag is True
+
+    op = SampleOp.parse_obj({"i": 5, "flag": False})
+    assert isinstance(op, SampleOp)
+    assert op.i == 5
+    assert op.flag is False
+
+
+def test_simple_failure_multiple_fields():
+    with pytest.raises(TypeError):
+
+        class _SampleOp(SimpleOperatorComponent):
+            a: int
+            b: int
+
+
+def test_simple_failure_dict_field():
+    class SampleOp(SimpleOperatorComponent):
+        d: Dict[str, Any]
+
+    with pytest.raises(NotImplementedError):
+        SampleOp.parse_obj(dict())
+
+
+def test_none_not_the_same_as_undefined():
+    class SampleOp(SimpleOperatorComponent):
+        a: int
+        b: Optional[int]  # Defaults to None, so there's only one undefined field
+
+
+def test_task_id_and_task_group():
+    class SampleOp(OperatorFactory):
+        i: int
+
+        @property
+        def default_task_id(self):
+            return f"add_{self.i}"
+
+        def _make_operators(self, *args, **kwargs) -> None:
+            load_value = DummyOperator(task_id="load")
+            compute_result = DummyOperator(task_id="compute")
+            finish = DummyOperator(task_id="finish")
+
+            load_value >> compute_result >> finish
+
+    from data_dag.dag_factory import DagFactory
+
+    class SampleDag(DagFactory):
+        def _make_dag(self):
+            SampleOp(i=3).make_operator()
+
+    dag = SampleDag(**_junk_dag_kwargs).make_dag()
+    load, compute, finish = dag.tasks
+    assert load.task_id == "add_3.load"
+    assert compute.task_id == "add_3.compute"
+    assert finish.task_id == "add_3.finish"
```

### Comparing `data-dag-0.2.2/PKG-INFO` & `data_dag-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 Metadata-Version: 2.1
 Name: data-dag
-Version: 0.2.2
+Version: 0.3.0
 Summary: Tooling to help build data-driven DAGs
 Author-email: Rearc Data <data@rearc.io>
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Project-URL: Home, https://github.com/rearc-data/data-dag
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Dist: apache-airflow
+Requires-Dist: typing_extensions>=4
+Requires-Dist: pydantic>=1
+Project-URL: Bug Tracker, https://github.com/rearc-data/data_dag/issues
+Project-URL: Homepage, https://github.com/rearc-data/data_dag
 
 [![Documentation Status](https://readthedocs.org/projects/data-dag/badge/?version=latest)](https://data-dag.readthedocs.io/en/latest/?badge=latest) ![PyPI](https://img.shields.io/pypi/v/data-dag)
 
 # Overview
 
 `data-dag` is a library for writing data-defined Airflow DAGs and operators.
```

