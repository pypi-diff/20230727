# Comparing `tmp/pytreeclass-0.5.0.tar.gz` & `tmp/pytreeclass-0.5.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytreeclass-0.5.0.tar", last modified: Mon Jul 24 19:33:09 2023, max compression
+gzip compressed data, was "pytreeclass-0.5.0.post0.tar", last modified: Thu Jul 27 21:44:30 2023, max compression
```

## Comparing `pytreeclass-0.5.0.tar` & `pytreeclass-0.5.0.post0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:09.491657 pytreeclass-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-07-24 19:33:09.491657 pytreeclass-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:09.487656 pytreeclass-0.5.0/pytreeclass/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:09.487656 pytreeclass-0.5.0/pytreeclass/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/code_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/tree_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    26041 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/tree_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/tree_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    28977 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/pytreeclass/_src/tree_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:09.487656 pytreeclass-0.5.0/pytreeclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-07-24 19:33:09.000000 pytreeclass-0.5.0/pytreeclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-24 19:33:09.000000 pytreeclass-0.5.0/pytreeclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:33:09.000000 pytreeclass-0.5.0/pytreeclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 19:33:09.000000 pytreeclass-0.5.0/pytreeclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 19:33:09.000000 pytreeclass-0.5.0/pytreeclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:33:09.491657 pytreeclass-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:33:09.487656 pytreeclass-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_tree_freeze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_tree_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_tree_pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_tree_viz_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_treeclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-24 19:32:48.000000 pytreeclass-0.5.0/tests/test_under_jit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:44:30.210432 pytreeclass-0.5.0.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-07-27 21:44:30.210432 pytreeclass-0.5.0.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:44:30.206432 pytreeclass-0.5.0.post0/pytreeclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:44:30.210432 pytreeclass-0.5.0.post0/pytreeclass/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/code_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/tree_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26041 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/tree_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/tree_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28977 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20927 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/pytreeclass/_src/tree_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:44:30.206432 pytreeclass-0.5.0.post0/pytreeclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-07-27 21:44:30.000000 pytreeclass-0.5.0.post0/pytreeclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-27 21:44:30.000000 pytreeclass-0.5.0.post0/pytreeclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:44:30.000000 pytreeclass-0.5.0.post0/pytreeclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 21:44:30.000000 pytreeclass-0.5.0.post0/pytreeclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 21:44:30.000000 pytreeclass-0.5.0.post0/pytreeclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:44:30.210432 pytreeclass-0.5.0.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:44:30.210432 pytreeclass-0.5.0.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_tree_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_tree_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_tree_pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_tree_viz_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_treeclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-27 21:44:13.000000 pytreeclass-0.5.0.post0/tests/test_under_jit.py
```

### Comparing `pytreeclass-0.5.0/LICENSE` & `pytreeclass-0.5.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/PKG-INFO` & `pytreeclass-0.5.0.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.5.0
+Version: 0.5.0.post0
 Summary: Visualize, create, and operate on JAX PyTree in the most intuitive way possible.
 Author-email: Mahmoud Asem <mahmoudasem00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pytreeclass-0.5.0/README.md` & `pytreeclass-0.5.0.post0/README.md`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/pyproject.toml` & `pytreeclass-0.5.0.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/pytreeclass/__init__.py` & `pytreeclass-0.5.0.post0/pytreeclass/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,12 +72,12 @@
     "tree_leaves_with_trace",
     "tree_flatten_with_trace",
     "tree_repr_with_trace",
     "Partial",
     "leafwise",
 )
 
-__version__ = "0.5.0"
+__version__ = "0.5.0post0"
 
 AtIndexer.__module__ = "pytreeclass"
 TreeClass.__module__ = "pytreeclass"
 Partial.__module__ = "pytreeclass"
```

### Comparing `pytreeclass-0.5.0/pytreeclass/_src/__init__.py` & `pytreeclass-0.5.0.post0/pytreeclass/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/pytreeclass/_src/code_build.py` & `pytreeclass-0.5.0.post0/pytreeclass/_src/code_build.py`

 * *Files 7% similar despite different names*

```diff
@@ -287,19 +287,39 @@
 def autoinit(klass: type[T]) -> type[T]:
     """A class decorator that generates the ``__init__`` method from type hints.
 
     Similar to ``dataclasses.dataclass``, this decorator generates the ``__init__``
     method for the given class from the type hints or the :func:`field` objects
     set to the class attributes.
 
+    Compared to ``dataclasses.dataclass``, ``autoinit`` with :func:`field` objects
+    can be used to apply functions on the field values during initialization,
+    and/or support multiple argument kinds.
+
     Example:
         >>> import pytreeclass as pytc
         >>> @pytc.autoinit
         ... class Tree:
         ...     x: int
         ...     y: int
         >>> tree = Tree(1, 2)
         >>> tree.x, tree.y
         (1, 2)
+
+    Example:
+        >>> # define fields with different argument kinds
+        >>> import pytreeclass as pytc
+        >>> @pytc.autoinit
+        ... class Tree:
+        ...     kw_only_field: int = pytc.field(default=1, kind="KW_ONLY")
+        ...     pos_only_field: int = pytc.field(default=2, kind="POS_ONLY")
+
+    Example:
+        >>> # define a validator to apply ``abs`` on the field value
+        >>> @pytc.autoinit
+        ... class Tree:
+        ...     a:int = pytc.field(callbacks=[abs])
+        >>> Tree(a=-1).a
+        1
     """
     klass.__init__ = _build_init_method(klass)
     return klass
```

### Comparing `pytreeclass-0.5.0/pytreeclass/_src/tree_base.py` & `pytreeclass-0.5.0.post0/pytreeclass/_src/tree_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,21 +141,21 @@
         >>> tree = Tree()
         >>> tree.at["a"].get()
         Tree(a=1, b=None)
         >>> tree.at[0].get()
         Tree(a=1, b=None)
     """
 
-    def __init_subclass__(klass: type[T]):
+    def __init_subclass__(klass: type[T], **k):
         if "__setattr__" in vars(klass):
             raise TypeError(f"Reserved methods: `__setattr__` defined in `{klass}`.")
         if "__delattr__" in vars(klass):
             raise TypeError(f"Reserved methods: `__delattr__` defined in `{klass}`.")
 
-        super().__init_subclass__()
+        super().__init_subclass__(**k)
 
         def tree_unflatten(keys: tuple[str, ...], leaves: tuple[Any, ...]) -> T:
             # unflatten rule to use with `jax.tree_unflatten`
             vars(tree := getattr(object, "__new__")(klass)).update(zip(keys, leaves))
             return tree
 
         def tree_flatten(tree: T) -> tuple[tuple[Any, ...], tuple[str, ...]]:
```

### Comparing `pytreeclass-0.5.0/pytreeclass/_src/tree_index.py` & `pytreeclass-0.5.0.post0/pytreeclass/_src/tree_index.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/pytreeclass/_src/tree_mask.py` & `pytreeclass-0.5.0.post0/pytreeclass/_src/tree_mask.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/pytreeclass/_src/tree_pprint.py` & `pytreeclass-0.5.0.post0/pytreeclass/_src/tree_pprint.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/pytreeclass/_src/tree_util.py` & `pytreeclass-0.5.0.post0/pytreeclass/_src/tree_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,14 +298,31 @@
 
     Args:
         klass: The class to be decorated.
 
     Returns:
         The decorated class.
 
+    Example:
+        >>> # use ``numpy`` functions on :class:`TreeClass`` classes decorated with ``leafwise``
+        >>> import pytreeclass as pytc
+        >>> import jax.numpy as jnp
+        >>> @pytc.leafwise
+        ... @pytc.autoinit
+        ... class Point(pytc.TreeClass):
+        ...    x: float = 0.5
+        ...    y: float = 1.0
+        ...    description: str = "point coordinates"
+        >>> # use :func:`tree_mask` to mask the non-inexact part of the tree
+        >>> # i.e. mask the string leaf ``description`` to ``Point`` work
+        >>> # with ``jax.numpy`` functions
+        >>> co = pytc.tree_mask(Point())
+        >>> print(pytc.bcmap(jnp.where)(co > 0.5, co, 1000))
+        Point(x=1000.0, y=1.0, description=#point coordinates)
+
     Note:
         If a mathematically equivalent operator is already defined on the class,
         then it is not overridden.
 
     ==================      ============
     Method                  Operator
     ==================      ============
@@ -332,15 +349,14 @@
     ``__pow__``              ``**``
     ``__round__``            ``round``
     ``__sub__``              ``-``
     ``__truediv__``          ``/``
     ``__trunc__``            ``math.trunc``
     ``__xor__``              ``^``
     ==================      ============
-
     """
     for key, method in (
         ("__abs__", uop(abs)),
         ("__add__", bop(op.add)),
         ("__and__", bop(op.and_)),
         ("__ceil__", uop(ceil)),
         ("__divmod__", bop(divmod)),
```

### Comparing `pytreeclass-0.5.0/pytreeclass.egg-info/PKG-INFO` & `pytreeclass-0.5.0.post0/pytreeclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytreeclass
-Version: 0.5.0
+Version: 0.5.0.post0
 Summary: Visualize, create, and operate on JAX PyTree in the most intuitive way possible.
 Author-email: Mahmoud Asem <mahmoudasem00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pytreeclass-0.5.0/pytreeclass.egg-info/SOURCES.txt` & `pytreeclass-0.5.0.post0/pytreeclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/tests/test_indexing.py` & `pytreeclass-0.5.0.post0/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/tests/test_nn.py` & `pytreeclass-0.5.0.post0/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/tests/test_tree_freeze.py` & `pytreeclass-0.5.0.post0/tests/test_tree_freeze.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/tests/test_tree_operator.py` & `pytreeclass-0.5.0.post0/tests/test_tree_operator.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/tests/test_tree_pprint.py` & `pytreeclass-0.5.0.post0/tests/test_tree_pprint.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/tests/test_tree_viz_util.py` & `pytreeclass-0.5.0.post0/tests/test_tree_viz_util.py`

 * *Files identical despite different names*

### Comparing `pytreeclass-0.5.0/tests/test_treeclass.py` & `pytreeclass-0.5.0.post0/tests/test_treeclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,7 +584,18 @@
 
     with pytest.raises(TypeError):
 
         @pytc.autoinit
         class Tree(pytc.TreeClass):
             a: int = pytc.field(kind="VAR_KW")
             b: int = pytc.field(kind="VAR_KW")
+
+
+def test_init_subclass():
+    class Test:
+        def __init_subclass__(cls, hello):
+            cls.hello = hello
+
+    class Test2(pytc.TreeClass, Test, hello=1):
+        ...
+
+    assert Test2.hello == 1
```

### Comparing `pytreeclass-0.5.0/tests/test_under_jit.py` & `pytreeclass-0.5.0.post0/tests/test_under_jit.py`

 * *Files identical despite different names*

