# Comparing `tmp/pysmiles-1.0.2.tar.gz` & `tmp/pysmiles-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmiles-1.0.2.tar", last modified: Fri Dec  2 10:45:45 2022, max compression
+gzip compressed data, was "pysmiles-1.1.1.tar", last modified: Thu Jul 27 10:59:51 2023, max compression
```

## Comparing `pysmiles-1.0.2.tar` & `pysmiles-1.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:45:45.388602 pysmiles-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-02 10:45:28.000000 pysmiles-1.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-02 10:45:28.000000 pysmiles-1.0.2/.coveralls.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:45:45.384602 pysmiles-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:45:45.384602 pysmiles-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2022-12-02 10:45:28.000000 pysmiles-1.0.2/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2022-12-02 10:45:28.000000 pysmiles-1.0.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2022-12-02 10:45:28.000000 pysmiles-1.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-02 10:45:28.000000 pysmiles-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2022-12-02 10:45:45.388602 pysmiles-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2022-12-02 10:45:28.000000 pysmiles-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:45:45.388602 pysmiles-1.0.2/pysmiles/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2022-12-02 10:45:28.000000 pysmiles-1.0.2/pysmiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2022-12-02 10:45:28.000000 pysmiles-1.0.2/pysmiles/read_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    17436 2022-12-02 10:45:28.000000 pysmiles-1.0.2/pysmiles/smiles_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2022-12-02 10:45:28.000000 pysmiles-1.0.2/pysmiles/testhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2022-12-02 10:45:28.000000 pysmiles-1.0.2/pysmiles/write_smiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:45:45.388602 pysmiles-1.0.2/pysmiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2022-12-02 10:45:45.000000 pysmiles-1.0.2/pysmiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2022-12-02 10:45:45.000000 pysmiles-1.0.2/pysmiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 10:45:45.000000 pysmiles-1.0.2/pysmiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 10:45:45.000000 pysmiles-1.0.2/pysmiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-02 10:45:45.000000 pysmiles-1.0.2/pysmiles.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-02 10:45:45.000000 pysmiles-1.0.2/pysmiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-02 10:45:45.000000 pysmiles-1.0.2/pysmiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2022-12-02 10:45:28.000000 pysmiles-1.0.2/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2022-12-02 10:45:28.000000 pysmiles-1.0.2/run_pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2022-12-02 10:45:45.392602 pysmiles-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      655 2022-12-02 10:45:28.000000 pysmiles-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 10:45:45.388602 pysmiles-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 10:45:28.000000 pysmiles-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2022-12-02 10:45:28.000000 pysmiles-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2022-12-02 10:45:28.000000 pysmiles-1.0.2/tests/test_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    22025 2022-12-02 10:45:28.000000 pysmiles-1.0.2/tests/test_read_smiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2022-12-02 10:45:28.000000 pysmiles-1.0.2/tests/test_smiles_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2022-12-02 10:45:28.000000 pysmiles-1.0.2/tests/test_write_smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:59:51.377104 pysmiles-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-27 10:59:38.000000 pysmiles-1.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 10:59:38.000000 pysmiles-1.1.1/.coveralls.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:59:51.369104 pysmiles-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:59:51.373104 pysmiles-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-27 10:59:38.000000 pysmiles-1.1.1/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-27 10:59:38.000000 pysmiles-1.1.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-27 10:59:38.000000 pysmiles-1.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-27 10:59:38.000000 pysmiles-1.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-07-27 10:59:51.377104 pysmiles-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-07-27 10:59:38.000000 pysmiles-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:59:51.373104 pysmiles-1.1.1/pysmiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 10:59:38.000000 pysmiles-1.1.1/pysmiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-07-27 10:59:38.000000 pysmiles-1.1.1/pysmiles/read_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-07-27 10:59:38.000000 pysmiles-1.1.1/pysmiles/smiles_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-27 10:59:38.000000 pysmiles-1.1.1/pysmiles/testhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-27 10:59:38.000000 pysmiles-1.1.1/pysmiles/write_smiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:59:51.377104 pysmiles-1.1.1/pysmiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-07-27 10:59:51.000000 pysmiles-1.1.1/pysmiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-27 10:59:51.000000 pysmiles-1.1.1/pysmiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:59:51.000000 pysmiles-1.1.1/pysmiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:59:51.000000 pysmiles-1.1.1/pysmiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 10:59:51.000000 pysmiles-1.1.1/pysmiles.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 10:59:51.000000 pysmiles-1.1.1/pysmiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 10:59:51.000000 pysmiles-1.1.1/pysmiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-27 10:59:38.000000 pysmiles-1.1.1/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-27 10:59:38.000000 pysmiles-1.1.1/run_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-27 10:59:51.381104 pysmiles-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 10:59:38.000000 pysmiles-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:59:51.377104 pysmiles-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:59:38.000000 pysmiles-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-27 10:59:38.000000 pysmiles-1.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-27 10:59:38.000000 pysmiles-1.1.1/tests/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-07-27 10:59:38.000000 pysmiles-1.1.1/tests/test_read_smiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-07-27 10:59:38.000000 pysmiles-1.1.1/tests/test_smiles_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-07-27 10:59:38.000000 pysmiles-1.1.1/tests/test_write_smiles.py
```

### Comparing `pysmiles-1.0.2/.github/workflows/deploy.yaml` & `pysmiles-1.1.1/.github/workflows/deploy.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
        py_version: ["3.9"]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.py_version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.py_version }}
     - name: Install dependencies
       run: |
         pip install --upgrade setuptools pip
     - name: Install package and requirements
       run: |
@@ -38,17 +38,17 @@
         coverage report
 
   deploy:
     needs: [build]
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@master
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
         python-version: 3.9
 
     - name: Install pypa/build
       run: >-
         python -m
         pip install
@@ -61,11 +61,11 @@
         python -m
         build
         --sdist
         --wheel
         --outdir dist/
 
     - name: Publish package to PyPI
-      uses: pypa/gh-action-pypi-publish@master
+      uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `pysmiles-1.0.2/.github/workflows/test.yaml` & `pysmiles-1.1.1/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
        py_version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.py_version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.py_version }}
     - name: Install dependencies
       run: |
         pip install --upgrade setuptools pip
     - name: Install package and requirements
       run: |
@@ -40,17 +40,17 @@
         coverage report
         coveralls
 
   lint:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.9
     - name: Install dependencies
       run: |
         pip install --upgrade setuptools pip
         pip install -r requirements-tests.txt
         pip install --upgrade .
```

### Comparing `pysmiles-1.0.2/.pylintrc` & `pysmiles-1.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/LICENSE.md` & `pysmiles-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/PKG-INFO` & `pysmiles-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmiles
-Version: 1.0.2
+Version: 1.1.1
 Summary: A lightweight SMILES reader and writer
 Home-page: https://github.com/pckroon/pysmiles
 Author: P C Kroon
 Author-email: p.c.kroon@rug.nl
 License: Apache 2.0
 Keywords: SMILES cheminformatics chemistry
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pysmiles-1.0.2/README.md` & `pysmiles-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/pysmiles/__init__.py` & `pysmiles-1.1.1/pysmiles/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/pysmiles/read_smiles.py` & `pysmiles-1.1.1/pysmiles/read_smiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,17 +99,20 @@
 
     Parameters
     ----------
     smiles : iterable
         The SMILES string to parse. Should conform to the OpenSMILES
         specification.
     explicit_hydrogen : bool
-        Whether hydrogens should be explicit nodes in the outout graph, or be
+        Whether hydrogens should be explicit nodes in the output graph, or be
         implicit in 'hcount' attributes.
-    reinterprit_aromatic : bool
+    zero_order_bonds : bool
+        Whether zero-order bonds (".") should be added as edges with an order of
+        0.
+    reinterpret_aromatic : bool
         Whether aromaticity should be determined from the created molecule,
         instead of taken from the SMILES string.
 
     Returns
     -------
     nx.Graph
         A graph describing a molecule. Nodes will have an 'element', 'aromatic'
```

### Comparing `pysmiles-1.0.2/pysmiles/smiles_helper.py` & `pysmiles-1.1.1/pysmiles/smiles_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,16 @@
 
     if stereo is not None:
         raise NotImplementedError
 
     if aromatic:
         name = name.lower()
 
-    if (stereo is None and isotope == '' and charge == 0 and default_h and
-            class_ == '' and name.lower() in 'b c n o p s se as *'.split()):
+    if (stereo is None and isotope == '' and charge == 0 and default_h and class_ == '' and
+            (name.lower() in 'b c n o p s *'.split() or name in 'F Cl Br I'.split())):
         return name
 
     if hcount:
         hcountstr = 'H'
         if hcount > 1:
             hcountstr += str(hcount)
     else:
```

### Comparing `pysmiles-1.0.2/pysmiles/testhelper.py` & `pysmiles-1.1.1/pysmiles/testhelper.py`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/pysmiles/write_smiles.py` & `pysmiles-1.1.1/pysmiles/write_smiles.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 # limitations under the License.
 
 """
 Exposes functionality for writing SMILES strings
 """
 
 from collections import defaultdict
+import logging
 
 import networkx as nx
 
 from .smiles_helper import remove_explicit_hydrogens, format_atom
 
+LOGGER = logging.getLogger(__name__)
 
 def _get_ring_marker(used_markers):
     """
     Returns the lowest number larger than 0 that is not in `used_markers`.
 
     Parameters
     ----------
@@ -70,18 +72,18 @@
                      molecule.nodes[n_jdx].get('element', '*').islower()
     aromatic_bond = aromatic_atoms and order == 1.5
     cross_aromatic = aromatic_atoms and order == 1
     single_bond = order == 1
     return cross_aromatic or not (aromatic_bond or single_bond)
 
 
-def write_smiles(molecule, default_element='*', start=None):
+def write_smiles_component(molecule, default_element='*', start=None):
     """
     Creates a SMILES string describing `molecule` according to the OpenSMILES
-    standard.
+    standard. `molecule` should be a single connected component.
 
     Parameters
     ----------
     molecule : nx.Graph
         The molecule for which a SMILES string should be generated.
     default_element : str
         The element to write if the attribute is missing for a node.
@@ -183,7 +185,47 @@
         elif branch_depth:
             # We're finished with this branch.
             smiles += ')'
             branch_depth -= 1
 
     smiles += ')' * branch_depth
     return smiles
+
+def write_smiles(molecule, default_element='*', start=None):
+    """
+    Creates a SMILES string describing `molecule` according to the OpenSMILES
+    standard. If `molecule` consists of multiple disconnected components their
+    corresponding SMILES string will be joined by zero-order bonds (".").
+
+    Parameters
+    ----------
+    molecule : nx.Graph
+        The molecule for which a SMILES string should be generated.
+    default_element : str
+        The element to write if the attribute is missing for a node.
+    start : Hashable
+        The atom at which the depth first traversal of the molecule should
+        start. A sensible one is chosen: preferably a terminal heteroatom.
+
+    Returns
+    -------
+    str
+        The SMILES string describing `molecule`.
+    """
+    smiles = []
+    components = list(nx.connected_components(molecule))
+    try:
+        components = sorted(components, key=lambda c: sorted(c))
+    except TypeError:
+        pass
+    for nodes in components:
+        if start is not None and start in nodes:
+            start_ = start
+        else:
+            start_ = None
+        smiles.append(write_smiles_component(molecule.subgraph(nodes),
+                      default_element=default_element, start=start_))
+    if len(smiles) > 1:
+        LOGGER.info('Be aware the specified molecule is disconnected and '
+                    'consists of %d connected components.', len(smiles))
+    return '.'.join(smiles)
+
```

### Comparing `pysmiles-1.0.2/pysmiles.egg-info/PKG-INFO` & `pysmiles-1.1.1/pysmiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmiles
-Version: 1.0.2
+Version: 1.1.1
 Summary: A lightweight SMILES reader and writer
 Home-page: https://github.com/pckroon/pysmiles
 Author: P C Kroon
 Author-email: p.c.kroon@rug.nl
 License: Apache 2.0
 Keywords: SMILES cheminformatics chemistry
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pysmiles-1.0.2/pysmiles.egg-info/SOURCES.txt` & `pysmiles-1.1.1/pysmiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/run_pylint.py` & `pysmiles-1.1.1/run_pylint.py`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/setup.cfg` & `pysmiles-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/setup.py` & `pysmiles-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/tests/conftest.py` & `pysmiles-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/tests/test_hypothesis.py` & `pysmiles-1.1.1/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/tests/test_read_smiles.py` & `pysmiles-1.1.1/tests/test_read_smiles.py`

 * *Files identical despite different names*

### Comparing `pysmiles-1.0.2/tests/test_smiles_helpers.py` & `pysmiles-1.1.1/tests/test_smiles_helpers.py`

 * *Files identical despite different names*

