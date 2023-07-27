# Comparing `tmp/jax_enums-0.1.1.tar.gz` & `tmp/jax_enums-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_enums-0.1.1.tar", last modified: Tue Jul 18 15:22:14 2023, max compression
+gzip compressed data, was "jax_enums-0.1.2.tar", last modified: Thu Jul 27 07:59:26 2023, max compression
```

## Comparing `jax_enums-0.1.1.tar` & `jax_enums-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:22:14.289002 jax_enums-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:22:14.285002 jax_enums-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:22:14.289002 jax_enums-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-18 15:21:57.000000 jax_enums-0.1.1/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-18 15:21:57.000000 jax_enums-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 15:21:57.000000 jax_enums-0.1.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-18 15:21:57.000000 jax_enums-0.1.1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 15:21:57.000000 jax_enums-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-18 15:21:57.000000 jax_enums-0.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-07-18 15:22:14.289002 jax_enums-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-18 15:21:57.000000 jax_enums-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:22:14.289002 jax_enums-0.1.1/jax_enums/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 15:21:57.000000 jax_enums-0.1.1/jax_enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-18 15:21:57.000000 jax_enums-0.1.1/jax_enums/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-18 15:21:57.000000 jax_enums-0.1.1/jax_enums/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:22:14.289002 jax_enums-0.1.1/jax_enums.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-07-18 15:22:14.000000 jax_enums-0.1.1/jax_enums.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-18 15:22:14.000000 jax_enums-0.1.1/jax_enums.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:22:14.000000 jax_enums-0.1.1/jax_enums.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 15:22:14.000000 jax_enums-0.1.1/jax_enums.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:22:14.000000 jax_enums-0.1.1/jax_enums.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 15:21:58.000000 jax_enums-0.1.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-18 15:21:57.000000 jax_enums-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 15:21:57.000000 jax_enums-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:22:14.289002 jax_enums-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:59:26.222891 jax_enums-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:59:26.218891 jax_enums-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:59:26.222891 jax_enums-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-27 07:59:13.000000 jax_enums-0.1.2/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-27 07:59:13.000000 jax_enums-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-27 07:59:13.000000 jax_enums-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 07:59:13.000000 jax_enums-0.1.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-27 07:59:13.000000 jax_enums-0.1.2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 07:59:13.000000 jax_enums-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-27 07:59:13.000000 jax_enums-0.1.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-07-27 07:59:26.222891 jax_enums-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-27 07:59:13.000000 jax_enums-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:59:26.222891 jax_enums-0.1.2/jax_enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 07:59:13.000000 jax_enums-0.1.2/jax_enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-27 07:59:13.000000 jax_enums-0.1.2/jax_enums/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-27 07:59:13.000000 jax_enums-0.1.2/jax_enums/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:59:26.222891 jax_enums-0.1.2/jax_enums.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-07-27 07:59:26.000000 jax_enums-0.1.2/jax_enums.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-27 07:59:26.000000 jax_enums-0.1.2/jax_enums.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:59:26.000000 jax_enums-0.1.2/jax_enums.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 07:59:26.000000 jax_enums-0.1.2/jax_enums.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 07:59:26.000000 jax_enums-0.1.2/jax_enums.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-27 07:59:13.000000 jax_enums-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 07:59:13.000000 jax_enums-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 07:59:26.222891 jax_enums-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:59:26.222891 jax_enums-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-27 07:59:13.000000 jax_enums-0.1.2/tests/test_enum.py
```

### Comparing `jax_enums-0.1.1/.github/workflows/CD.yml` & `jax_enums-0.1.2/.github/workflows/CD.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 name: CD
 
-on: workflow_dispatch
+on:
+  workflow_dispatch:
+  push:
+    branches:
+      - "main"
 
 jobs:
   release:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
@@ -15,32 +19,28 @@
           VERSION_FILE="$/jax_enums/_version.py"
           JAX_ENUMS_VERSION="$(cat jax_enums/_version.py | grep '__version__ = ' |  cut -d'=' -f2 | sed 's,\",,g' | sed "s,\',,g" | sed 's, ,,g')"
           echo "Current version is:"
           echo "$JAX_ENUMS_VERSION"
 
           echo "JAX_ENUMS_VERSION=$JAX_ENUMS_VERSION" >> $GITHUB_ENV
 
-      - name: Create and push tag
-        run: |
-          echo "Creating tag ${{ env.JAX_ENUMS_VERSION }}"
-          git tag ${{ env.JAX_ENUMS_VERSION }}
-          git push --tags
-
-      - name: Create changelog
+      - name: Create changelog and push tag
         id: changelog
         uses: TriPSs/conventional-changelog-action@v3
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
-          output-file: "false"
+          output-file: false
+          fallback-version: ${{ env.JAX_ENUMS_VERSION }}
+          skip-commit: true
 
       - name: Create Release
         uses: ncipollo/release-action@v1
         with:
           tag: ${{ env.JAX_ENUMS_VERSION }}
-          name: "JAX_ENUM release v${{ env.JAX_ENUMS_VERSION }}"
+          name: "JAX_ENUMS release v${{ env.JAX_ENUMS_VERSION }}"
           body: ${{ steps.changelog.outputs.clean_changelog }}
 
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
 
       - name: Install pypa/build
```

### Comparing `jax_enums-0.1.1/.gitignore` & `jax_enums-0.1.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
+.vscode/
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
```

### Comparing `jax_enums-0.1.1/COPYRIGHT` & `jax_enums-0.1.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `jax_enums-0.1.1/LICENSE` & `jax_enums-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jax_enums-0.1.1/PKG-INFO` & `jax_enums-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax_enums
-Version: 0.1.1
+Version: 0.1.2
 Summary: JAX-compatible Enumerations.
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `jax_enums-0.1.1/README.md` & `jax_enums-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jax_enums-0.1.1/jax_enums/_version.py` & `jax_enums-0.1.2/jax_enums/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `jax_enums-0.1.1/jax_enums/enum.py` & `jax_enums-0.1.2/jax_enums/enum.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,54 +15,85 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from __future__ import annotations
 
-from typing import Type, Any
+from typing import Any
 from enum import Enum, EnumMeta
+from dataclasses import dataclass
 
 import jax
 import jax.numpy as jnp
-from dataclasses import dataclass
 
 
 @jax.tree_util.register_pytree_node_class
 @dataclass
 class EnumItem:
     name: str
     value: jax.Array
-    obj_class: Type
+    obj_class: str
 
     def __str__(self):
-        return f"<{self.obj_class.__name__}.{self.name}: {self.value}> as PyTreeNode"
+        return f"<{self.obj_class}.{self.name}: {self.value}> as PyTreeNode"
 
     def __repr__(self):
         return str(self)
 
     def __hash__(self):
         return hash(tuple(jax.tree_util.tree_leaves(self)))
 
+    def __getitem__(self, idx):
+        return jax.tree_util.tree_map(lambda x: x[idx], self)
+
     def __eq__(self, other):
-        if isinstance(other, EnumItem):
-            with jax.ensure_compile_time_eval():
-                return self.value == other.value
-        return hash(self) == hash(other)
+        if not isinstance(other, EnumItem):
+            raise TypeError(
+                "Cannot compare EnumItem with non-EnumItem {}".format(other)
+            )
+        with jax.ensure_compile_time_eval():
+            return jnp.array_equal(self.value, other.value)
+
+    def __ne__(self, other):
+        return jnp.logical_not(self.__eq__(other))
 
     def tree_flatten(self):
-        return jnp.asarray(self.value)[None], (self.name, self.obj_class)
+        return (self.value,), (self.name, self.obj_class)
 
     @classmethod
     def tree_unflatten(cls, aux, children) -> EnumItem:
         return cls(value=children[0], name=aux[0], obj_class=aux[1])
 
 
 class EnumerableMeta(EnumMeta):
+    def __new__(mcls, attr_name, bases, attrs, **kwargs):
+        # this hack is to pass the equality tests in Enum.__new__
+        # since, if the value of an enum is an Array,
+        #  Array == Array returns an Array, which cannot be cast to bool
+        for attr_name, value in attrs.items():
+            if not attr_name.startswith("_") and not isinstance(value, EnumItem):
+                # value is the value assigned to the item, e.g., 0 for A = 0
+                # A == attrs["__qualname__"]
+                # 0 == value
+                value = EnumItem(
+                    value=jnp.asarray(value), name=attr_name, obj_class=attrs["__qualname__"]
+                )
+                dict.update(attrs, {attr_name: value})
+        return super().__new__(mcls, attr_name, bases, attrs)
+
     def __setattr__(self, name: str, value: Any) -> None:
-        if not name.startswith("_"):
-            value = EnumItem(name, value.value, self)
+        if (
+            not name.startswith("_")
+            and not isinstance(value, EnumItem)
+            and name == value.name
+        ):
+            value = EnumItem(
+                value=jnp.asarray(value.value.value),
+                name=name,
+                obj_class=value.value.obj_class,
+            )
         return super().__setattr__(name, value)
 
 
 class Enumerable(Enum, metaclass=EnumerableMeta):
     ...
```

### Comparing `jax_enums-0.1.1/jax_enums.egg-info/PKG-INFO` & `jax_enums-0.1.2/jax_enums.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-enums
-Version: 0.1.1
+Version: 0.1.2
 Summary: JAX-compatible Enumerations.
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `jax_enums-0.1.1/pyproject.toml` & `jax_enums-0.1.2/pyproject.toml`

 * *Files identical despite different names*

