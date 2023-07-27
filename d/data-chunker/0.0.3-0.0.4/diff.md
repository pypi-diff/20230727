# Comparing `tmp/data_chunker-0.0.3.tar.gz` & `tmp/data_chunker-0.0.4.tar.gz`

## Comparing `data_chunker-0.0.3.tar` & `data_chunker-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 data_chunker-0.0.3/src/data_chunker/__init__.py
--rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 data_chunker-0.0.3/src/data_chunker/java_code.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 data_chunker-0.0.3/src/data_chunker/parser.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 data_chunker-0.0.3/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 data_chunker-0.0.3/LICENSE
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 data_chunker-0.0.3/README.adoc
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 data_chunker-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 data_chunker-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 data_chunker-0.0.4/src/data_chunker/__init__.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 data_chunker-0.0.4/src/data_chunker/java_code.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 data_chunker-0.0.4/src/data_chunker/parser.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 data_chunker-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 data_chunker-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 data_chunker-0.0.4/README.adoc
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 data_chunker-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 data_chunker-0.0.4/PKG-INFO
```

### Comparing `data_chunker-0.0.3/src/data_chunker/java_code.py` & `data_chunker-0.0.4/src/data_chunker/java_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,15 +114,21 @@
     return chunk_node_type(tree, node_type, "field", codelines)
 
 def chunk_methods(tree: javalang.tree.CompilationUnit,
                   codelines: list) -> list:
     node_type = javalang.tree.MethodDeclaration
     return chunk_node_type(tree, node_type, "method", codelines)
 
-
+def chunk_all(tree: javalang.tree.CompilationUnit,
+                  codelines: list) -> list:
+    chunks = chunk_constants(tree)
+    chunks = chunks + chunk_constructors(tree, codelines)
+    chunks = chunks + chunk_fields(tree, codelines)
+    chunks = chunks + chunk_methods(tree, codelines)
+    return chunks
 
 def chunk_node_type(tree: javalang.tree.CompilationUnit,
                     node_type: javalang.tree.Declaration,
                     mem_str: str,
                     codelines: list) -> list:
     # Initialize return variables
     chunks = []
```

### Comparing `data_chunker-0.0.3/src/data_chunker/parser.py` & `data_chunker-0.0.4/src/data_chunker/parser.py`

 * *Files identical despite different names*

### Comparing `data_chunker-0.0.3/LICENSE` & `data_chunker-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `data_chunker-0.0.3/README.adoc` & `data_chunker-0.0.4/README.adoc`

 * *Files identical despite different names*

### Comparing `data_chunker-0.0.3/pyproject.toml` & `data_chunker-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "setup/",
     "training/",
     "main.py",
 ]
 
 [project]
 name = "data-chunker"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Chris Mills", email="cmills@breakfreesolutions.com"},
     { name="Colin Pitawanakwat", email="cpitawanakwat@breakfreesolutions.com"}
 ]
 description = "Chunks code into a list made up of indexable dictionaries."
 # Note that AsciiDoc file is passed as 'plain' since the build engine
 # cannot use the '*.adoc' extension.
```

### Comparing `data_chunker-0.0.3/PKG-INFO` & `data_chunker-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-chunker
-Version: 0.0.3
+Version: 0.0.4
 Summary: Chunks code into a list made up of indexable dictionaries.
 Project-URL: Homepage, https://github.com/break-free/data-chunker
 Project-URL: Issues, https://github.com/break-free/data-chunker/issues
 Author-email: Chris Mills <cmills@breakfreesolutions.com>, Colin Pitawanakwat <cpitawanakwat@breakfreesolutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

