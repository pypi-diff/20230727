# Comparing `tmp/python2verilog-0.0.3.tar.gz` & `tmp/python2verilog-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python2verilog-0.0.3.tar", last modified: Fri Jul 21 15:27:40 2023, max compression
+gzip compressed data, was "python2verilog-0.0.4.tar", last modified: Wed Jul 26 23:04:16 2023, max compression
```

## Comparing `python2verilog-0.0.3.tar` & `python2verilog-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.532267 python2verilog-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-21 15:27:40.532267 python2verilog-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-21 15:27:26.000000 python2verilog-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-21 15:27:26.000000 python2verilog-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.524267 python2verilog-0.0.3/python2verilog/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.528267 python2verilog-0.0.3/python2verilog/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22129 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/backend/verilog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.528267 python2verilog-0.0.3/python2verilog/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19875 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/frontend/generator_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.528267 python2verilog-0.0.3/python2verilog/ir/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/ir/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/ir/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/ir/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.528267 python2verilog-0.0.3/python2verilog/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.532267 python2verilog-0.0.3/python2verilog/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/utils/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-21 15:27:26.000000 python2verilog-0.0.3/python2verilog/utils/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:40.528267 python2verilog-0.0.3/python2verilog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-21 15:27:40.000000 python2verilog-0.0.3/python2verilog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-21 15:27:40.000000 python2verilog-0.0.3/python2verilog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:27:40.000000 python2verilog-0.0.3/python2verilog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 15:27:40.000000 python2verilog-0.0.3/python2verilog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:27:40.532267 python2verilog-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.900687 python2verilog-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-26 23:04:16.900687 python2verilog-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-26 23:04:05.000000 python2verilog-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-26 23:04:05.000000 python2verilog-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.892687 python2verilog-0.0.4/python2verilog/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.892687 python2verilog-0.0.4/python2verilog/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26654 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/backend/verilog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.896687 python2verilog-0.0.4/python2verilog/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/frontend/generator2graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/frontend/generator_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.896687 python2verilog-0.0.4/python2verilog/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/ir/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/ir/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/ir/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/ir/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.896687 python2verilog-0.0.4/python2verilog/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.900687 python2verilog-0.0.4/python2verilog/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/utils/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/utils/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.892687 python2verilog-0.0.4/python2verilog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-26 23:04:16.000000 python2verilog-0.0.4/python2verilog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-26 23:04:16.000000 python2verilog-0.0.4/python2verilog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:04:16.000000 python2verilog-0.0.4/python2verilog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 23:04:16.000000 python2verilog-0.0.4/python2verilog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:04:16.900687 python2verilog-0.0.4/setup.cfg
```

### Comparing `python2verilog-0.0.3/PKG-INFO` & `python2verilog-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.0.3
+Version: 0.0.4
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `python2verilog-0.0.3/README.md` & `python2verilog-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python2verilog-0.0.3/pyproject.toml` & `python2verilog-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python2verilog"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "Kerry Wang", email = "kerrywang369@gmail.com" }]
 description = "Converts a subset of python generator functions into synthesizable sequential SystemVerilog"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `python2verilog-0.0.3/python2verilog/backend/verilog.py` & `python2verilog-0.0.4/python2verilog/backend/verilog.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Verilog Abstract Syntax Tree Components"""
 
 from __future__ import annotations
 import warnings
 import ast
 from typing import Optional
+import copy
 
-from ..utils.string import Lines, Indent
-from ..utils.assertions import assert_list_elements
+from ..utils.string import Lines, Indent, ImplementsToLines
+from ..utils.assertions import assert_list_type, assert_type, assert_dict_type
 from .. import ir
 
 
 class Expression:
     """
     Verilog expression, e.g.
     a + b
@@ -46,15 +47,15 @@
 
     def __init__(self, condition: Expression):
         assert isinstance(condition, Expression)
         self.condition = condition
         super().__init__(f"@(negedge {condition.to_string()})")
 
 
-class Statement:
+class Statement(ImplementsToLines):
     """
     Represents a statement in verilog (i.e. a line or a block)
     If used directly, it is treated as a string literal
     """
 
     def __init__(self, literal: str = "", comment: str = ""):
         self.literal = literal
@@ -66,20 +67,14 @@
         """
         if self.literal:
             return Lines(
                 self.literal + self.get_inline_comment()[1:]
             )  # Removes leading space
         return Lines(self.get_inline_comment()[1:])
 
-    def to_string(self):
-        """
-        To Verilog
-        """
-        return self.to_lines().to_string()
-
     def get_inline_comment(self):
         """
         // <comment>
         """
         if self.comment != "":
             return f" // {self.comment}"
         return ""
@@ -93,20 +88,14 @@
         """
         actual_lines = self.comment.split("\n")
         lines = Lines()
         for line in actual_lines:
             lines += f"// {line}"
         return lines
 
-    def append_end_statements(self, _: list[Statement]):
-        """
-        Append end statements
-        """
-        raise NotImplementedError("Statements cannot be appended to")
-
 
 class AtPosedgeStatement(Statement):
     """
     @(posedge <condition>);
     """
 
     def __init__(self, condition: Expression, *args, **kwargs):
@@ -126,114 +115,229 @@
 
 class Verilog:
     """
     Code Generation for Verilog
     """
 
     @staticmethod
-    def __create_module_from_python(root: Statement, context: ir.Context):
+    def __new_module(root: Statement, context: ir.Context):
         """
         Creates a module wrapper from the context
-        e.g. the I/O (from Python), clock, valid and done signals
+
+        Requires context for I/O and declarations
         """
         assert isinstance(root, Statement)
         assert isinstance(context, ir.Context)
         inputs = []
         for var in context.input_vars:
             inputs.append(var)
         outputs = []
         for i in range(len((context.output_vars))):
             outputs.append(f"_out{str(i)}")
         # TODO: make these extras optional
         always = PosedgeSyncAlways(
             Expression("_clock"),
             valid="_valid",
-            body=[Verilog.__get_init(root, context.global_vars)],
+            body=[Verilog.__get_start_ifelse(root, context.global_vars)],
         )
-        return Module(context.name, inputs, outputs, body=[always])
+        body: list[Statement] = [
+            Declaration(v, is_reg=True, is_signed=True) for v in context.global_vars
+        ]
+        body.append(always)
+        return Module(name=context.name, inputs=inputs, outputs=outputs, body=body)
 
-    def __init__(
-        self,
-        root: Optional[ir.Statement] = None,
-        context: Optional[ir.Context] = None,
-    ):
-        # TODO: throw errors if user tries to generate verilog beforeconfig
-        self.module: Optional[Module] = None
-        self.context: Optional[ir.Context] = None
-        if root is not None and context is not None:
-            self.from_ir(root, context)
+    def __init__(self):
+        self._context = None
+        self._module = None
+
+    @classmethod
+    def from_list_ir(cls, root: ir.Statement, context: ir.Context):
+        """
+        Builds tree from list IR
+        """
+        assert isinstance(root, ir.Statement), f"got {type(root)} instead"
+        assert isinstance(context, ir.Context)
+        inst = Verilog()
+        inst._context = context
+        inst._module = Verilog.__new_module(Verilog.list_build_stmt(root), context)
+        return inst
+
+    @classmethod
+    def from_graph_ir(cls, root: ir.Node, context: ir.Context):
+        """ "
+        Builds tree from Graph IR
+        """
+        assert_type(root, ir.Node)
+        assert_type(context, ir.Context)
+        inst = Verilog()
+        inst._context = context
+        root_case = inst.graph_build(root, set())
+        inst._context.global_vars["_state"] = str(len(root_case.case_items))
+        inst._module = Verilog.__new_module(root_case, context)
+        return inst
 
     @staticmethod
-    def build_tree_stmt(node: ir.Statement) -> Statement:
+    def list_build_stmt(node: ir.Statement) -> Statement:
         """
         Builds the Verilog AST
         """
         assert isinstance(node, (ir.Statement, ir.CaseItem))
         if not node:
             return Statement("")
         if isinstance(node, ir.Case):
-            return Verilog.build_tree_case(node)
+            return Verilog.list_build_case(node)
         if isinstance(node, ir.IfElse):
             then_body = []
             for stmt in node.then_body:
-                then_body.append(Verilog.build_tree_stmt(stmt))
+                then_body.append(Verilog.list_build_stmt(stmt))
             else_body = []
             for stmt in node.else_body:
-                else_body.append(Verilog.build_tree_stmt(stmt))
-            return IfElse(Verilog.build_tree_expr(node.condition), then_body, else_body)
+                else_body.append(Verilog.list_build_stmt(stmt))
+            return IfElse(Verilog.list_build_expr(node.condition), then_body, else_body)
         if isinstance(node, ir.Statement):
             return Statement(node.to_string().replace("\n", " "))
         raise NotImplementedError(f"Unexpected type {type(node)}")
 
     @staticmethod
-    def build_tree_expr(node: ir.Expression) -> Expression:
+    def list_build_expr(node: ir.Expression) -> Expression:
         """
         Handles expressions
         """
         assert isinstance(node, ir.Expression)
         return Expression(node.to_string())
 
     @staticmethod
-    def build_tree_case(node: ir.Case) -> Case:
+    def list_build_case(node: ir.Case) -> Case:
         """
         Handles case statements
         """
         assert isinstance(node, ir.Case)
         case_items = []
         for item in node.case_items:
-            case_items.append(Verilog.build_tree_caseitem(item))
-        return Case(Verilog.build_tree_expr(node.condition), case_items)
+            case_items.append(Verilog.list_build_case_item(item))
+        return Case(Verilog.list_build_expr(node.condition), case_items)
 
     @staticmethod
-    def build_tree_caseitem(node: ir.CaseItem) -> CaseItem:
+    def list_build_case_item(node: ir.CaseItem) -> CaseItem:
         """
         Handles case item
         """
         case_items = []
         for item in node.statements:
-            case_items.append(Verilog.build_tree_stmt(item))
-        return CaseItem(Verilog.build_tree_expr(node.condition), case_items)
+            case_items.append(Verilog.list_build_stmt(item))
+        return CaseItem(Verilog.list_build_expr(node.condition), case_items)
 
-    def from_ir(self, root: ir.Statement, context: ir.Context):
+    def graph_build(self, root: ir.Node, visited: set[str]):
         """
-        Builds tree from IR
+        Builds from graph
         """
-        assert isinstance(root, ir.Statement)
-        assert isinstance(context, ir.Context)
-        root.append_end_statements(
-            [ir.NonBlockingSubsitution(ir.Var("_done"), ir.Int(1))]
-        )
-        self.context = context
-        self.module = Verilog.__create_module_from_python(
-            Verilog.build_tree_stmt(root), context
-        )
-        return self
+        assert_type(root, ir.Node)
+        root_case = Case(expression=Expression("_state"), case_items=[])
+        self.graph_build_node(node=root, root_case=root_case, visited=visited)
+        return root_case
+
+    def graph_build_node(self, node: ir.Node, root_case: Case, visited: set[str]):
+        """
+        Builds from node
+        """
+        assert_type(node, ir.Node)
+        assert isinstance(self._context, ir.Context)
+        if node.unique_id in visited:
+            return node.unique_id
+
+        if isinstance(node, ir.AssignNode):
+            if node.unique_id not in visited:
+                visited.add(node.unique_id)
+                next_state = self.graph_build_node(node._edge, root_case, visited)
+                root_case.case_items.append(
+                    CaseItem(
+                        condition=Expression(node.unique_id),
+                        statements=[
+                            Statement(f"{node.to_string()};"),
+                            NonBlockingSubsitution(
+                                lvalue=root_case.condition.to_string(),
+                                rvalue=next_state,
+                            ),
+                        ],
+                    )
+                )
+                self._context.global_vars[node.unique_id] = len(root_case.case_items)
+            return node.unique_id
+        if isinstance(node, ir.IfElseNode):
+            if node.unique_id not in visited:
+                visited.add(node.unique_id)
+                then_state = self.graph_build_node(node._then_edge, root_case, visited)
+                else_state = self.graph_build_node(node._else_edge, root_case, visited)
+                root_case.case_items.append(
+                    CaseItem(
+                        condition=Expression(node.unique_id),
+                        statements=[
+                            IfElse(
+                                condition=Expression(node._condition.to_string()),
+                                then_body=[
+                                    NonBlockingSubsitution(
+                                        root_case.condition.to_string(), then_state
+                                    )
+                                ],
+                                else_body=[
+                                    NonBlockingSubsitution(
+                                        root_case.condition.to_string(), else_state
+                                    )
+                                ],
+                            )
+                        ],
+                    )
+                )
+                self._context.global_vars[node.unique_id] = len(root_case.case_items)
+            return node.unique_id
+        if isinstance(node, ir.YieldNode):
+            if node.unique_id not in visited:
+                visited.add(node.unique_id)
+                next_state = self.graph_build_node(node._edge, root_case, visited)
+                stmts = [
+                    NonBlockingSubsitution(f"_out{i}", v.to_string())
+                    for i, v in enumerate(node._stmts)
+                ] + [NonBlockingSubsitution("_valid", "1")]
+                root_case.case_items.append(
+                    CaseItem(
+                        condition=Expression(node.unique_id),
+                        statements=[
+                            *stmts,
+                            NonBlockingSubsitution(
+                                lvalue=root_case.condition.to_string(),
+                                rvalue=next_state,
+                            ),
+                        ],
+                    )
+                )
+                self._context.global_vars[node.unique_id] = len(root_case.case_items)
+            return node.unique_id
+        if isinstance(node, ir.Edge):
+            if node.unique_id not in visited:
+                visited.add(node.unique_id)
+                return self.graph_build_node(node._node, root_case, visited)
+            return "bruvlmao"
+        if isinstance(node, ir.Node):
+            if node.unique_id not in visited:
+                visited.add(node.unique_id)
+                root_case.case_items.append(
+                    CaseItem(
+                        condition=Expression(node.unique_id),
+                        statements=[
+                            NonBlockingSubsitution("_done", "1"),
+                        ],
+                    )
+                )
+                self._context.global_vars[node.unique_id] = len(root_case.case_items)
+            return node.unique_id
+        assert_type(node, ir.AssignNode)
+        return ""
 
     @staticmethod
-    def __get_init(root: Statement, global_vars: dict[str, str]):
+    def __get_start_ifelse(root: Statement, global_vars: dict[str, str]):
         """
         if (_start) begin
             <var> = <value>;
             ...
         end else begin
         ...
         end
@@ -245,76 +349,87 @@
         block = IfElse(
             Expression("_start"),
             then_body,
             [root],
         )
         return block
 
-    def get_module(self):
+    @property
+    def module(self):
         """
         Get Verilog module
         """
-        decls = [
-            Declaration(v, is_reg=True, is_signed=True)
-            for v in self.context.global_vars
-        ]
-        self.module.body = decls + self.module.body
+        assert isinstance(self._module, Module)
+        return copy.deepcopy(self._module)
+
+    def get_module_lines(self):
+        """
+        Get Verilog module as Lines
+        """
         return self.module.to_lines()
 
-    def get_testbench(self, test_cases: list[tuple[str]]):
+    def get_module_str(self):
+        """
+        Get Verilog module as string
+        """
+        return str(self.get_module_lines())
+
+    def new_testbench(self, test_cases: list[tuple[str]]):
         """
-        Creates testbench with multiple test cases using the _done signal
+        Creates testbench with multiple test cases
+
+        Each element of test_cases represents a single test case
         """
 
         def make_display_stmt():
             """
             Creates a display statement for valid + outputs
 
             $display("%0d, ...", _valid, ...);
             """
             string = '$display("%0d, '
-            string += "%0d, " * (len(self.context.output_vars) - 1)
+            string += "%0d, " * (len(self._context.output_vars) - 1)
             string += '%0d", _valid'
-            for var in self.context.output_vars:
+            for var in self._context.output_vars:
                 string += f", {var}"
             string += ");"
             return Statement(literal=string)
 
-        assert self.context is not None
+        assert isinstance(self._context, ir.Context)
         decl: list[Declaration] = []
         decl.append(Declaration("_clock", size=1, is_reg=True))
         decl.append(Declaration("_start", size=1, is_reg=True))
         decl += [
             Declaration(var, is_signed=True, is_reg=True)
-            for var in self.context.input_vars
+            for var in self._context.input_vars
         ]
-        decl += [Declaration(var, is_signed=True) for var in self.context.output_vars]
+        decl += [Declaration(var, is_signed=True) for var in self._context.output_vars]
 
         decl.append(Declaration("_done", size=1))
         decl.append(Declaration("_valid", size=1))
 
         ports = {
             decl.name: decl.name for decl in decl
         }  # Caution: expects decl to only contain declarations
 
         setups: list[Statement] = list(decl)
-        setups.append(Instantiation(self.context.name, "DUT", ports))
+        setups.append(Instantiation(self._context.name, "DUT", ports))
 
         setups.append(Statement(literal="always #5 _clock = !_clock;"))
 
         initial_body: list[Statement | While] = []  # TODO: replace with Sequence
         initial_body.append(BlockingSubsitution("_clock", "0"))
         initial_body.append(BlockingSubsitution("_start", "0"))
         initial_body.append(AtNegedgeStatement(Expression("_clock")))
         initial_body.append(Statement())
 
         for i, test_case in enumerate(test_cases):
             # setup for new test case
             initial_body.append(Statement(comment=f"Test case {i}: {str(test_case)}"))
-            for i, var in enumerate(self.context.input_vars):
+            for i, var in enumerate(self._context.input_vars):
                 initial_body.append(BlockingSubsitution(var, str(test_case[i])))
             initial_body.append(BlockingSubsitution("_start", "1"))
 
             initial_body.append(AtNegedgeStatement(Expression("_clock")))
 
             # wait for done signal
             while_body: list[Statement] = []
@@ -326,25 +441,37 @@
             initial_body.append(make_display_stmt())
             initial_body.append(Statement())
 
         initial_body.append(Statement(literal="$finish;"))
 
         initial_loop = Initial(body=initial_body)
 
-        if self.context:
+        if self._context:
             module = Module(
-                f"{self.context.name}_tb",
+                f"{self._context.name}_tb",
                 [],
                 [],
                 body=setups + [initial_loop],
                 add_default_ports=False,
             )
             return module
         raise RuntimeError("Needs the context")
 
+    def new_testbench_lines(self, test_cases: list[tuple[str]]):
+        """
+        New Testbench as lines
+        """
+        return self.new_testbench(test_cases).to_lines()
+
+    def new_testbench_str(self, test_cases: list[tuple[str]]):
+        """
+        New testbench as str
+        """
+        return str(self.new_testbench_lines(test_cases))
+
 
 class Instantiation(Statement):
     """
     Instantiationo f Verilog module.
     <module-name> <given-name> (...);
     """
 
@@ -378,15 +505,15 @@
         for key, val in self.port_connections.items():
             lines += Indent(1) + f".{key}({val}),"
         lines[-1] = lines[-1][:-1]  # Remove last comma
         lines += Indent(1) + ");"
         return lines
 
 
-class Module:
+class Module(ImplementsToLines):
     """
     module name(...); endmodule
     """
 
     def __init__(
         self,
         name: str,
@@ -448,15 +575,15 @@
     initial begin
         ...
     end
     """
 
     def __init__(self, *args, body: Optional[list[Statement]] = None, **kwargs):
         if body:
-            assert_list_elements(body, Statement)
+            assert_list_type(body, Statement)
         self.body = body
         super().__init__(*args, **kwargs)
 
     def to_lines(self):
         lines = Lines("initial begin")
         for stmt in self.body:
             lines.concat(stmt.to_lines(), 1)
@@ -635,26 +762,14 @@
 
     def to_string(self):
         """
         To Verilog
         """
         return self.to_lines().to_string()
 
-    def append_end_statements(self, statements: list[Statement]):
-        """
-        Append statements to case item
-        """
-        # self.statements = self.statements + assert_list_elements(statements, Statement)
-        # warnings.warn(statements[0].to_string() + " " + str(type(self.statements[-1])))
-        self.statements[-1].append_end_statements(
-            assert_list_elements(statements, Statement)
-        )
-        # warnings.warn(statements[0].to_string())
-        return self
-
 
 class Case(Statement):
     """
     Verilog case statement with various cases
     case (<expression>)
         <items[0]>
         ...
@@ -682,23 +797,14 @@
         lines = Lines()
         lines += f"case ({self.condition.to_string()})"
         for item in self.case_items:
             lines.concat(item.to_lines(), indent=1)
         lines += "endcase"
         return lines
 
-    def append_end_statements(self, statements: list[Statement]):
-        """
-        Adds statements to the last case item
-        """
-        self.case_items[-1].append_end_statements(
-            assert_list_elements(statements, Statement)
-        )
-        return self
-
 
 class IfElse(Statement):
     """
     Verilog if else
     """
 
     def __init__(
@@ -708,16 +814,16 @@
         else_body: list[Statement],
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         assert isinstance(condition, Expression)
         self.condition = condition
-        self.then_body = assert_list_elements(then_body, Statement)
-        self.else_body = assert_list_elements(else_body, Statement)
+        self.then_body = assert_list_type(then_body, Statement)
+        self.else_body = assert_list_type(else_body, Statement)
 
     def to_lines(self):
         lines = Lines()
         lines += f"if ({self.condition.to_string()}) begin"
         for stmt in self.then_body:
             lines.concat(stmt.to_lines(), indent=1)
         lines += "end else begin"
@@ -726,15 +832,15 @@
         lines += "end"
         return lines
 
     def append_end_statements(self, statements: list[Statement]):
         """
         Appends statements to both branches
         """
-        statements = assert_list_elements(statements, Statement)
+        statements = assert_list_type(statements, Statement)
         # warnings.warn("appending " + statements[0].to_string())
         # if len(statements) > 1:
         #     warnings.warn(statements[1].to_string())
         self.then_body[-1].append_end_statements(statements)
         self.else_body[-1].append_end_statements(statements)
         return self
 
@@ -753,15 +859,15 @@
         condition: Expression,
         body: Optional[list[Statement]] = None,
         **kwargs,
     ):
         assert isinstance(condition, Expression)
         self.condition = condition
         if body:
-            assert_list_elements(body, Statement)
+            assert_list_type(body, Statement)
         self.body = body
         super().__init__(*args, **kwargs)
 
     def to_lines(self):
         lines = Lines(f"while ({self.condition.to_string()}) begin")
         for stmt in self.body:
             lines.concat(stmt.to_lines(), 1)
```

### Comparing `python2verilog-0.0.3/python2verilog/convert.py` & `python2verilog-0.0.4/python2verilog/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,41 @@
 To run the basic conversion as a CLI script
 """
 
 import argparse
 import os
 import ast
 import warnings
-from .frontend import GeneratorParser
+from typing import Optional
+from .frontend import Generator2List, Generator2Graph
 from .backend.verilog import Verilog
 from .optimizer import optimizer
 
 
-def convert(func: ast.FunctionDef, optimization_level: int):
+def convert_list(func: ast.FunctionDef, optimization_level: int):
     """
     Wrapper for common Python to Verilog conversion
     """
-    ir_root, context = GeneratorParser(func).get_results()
+    ir_root, context = Generator2List(func).get_results()
     if optimization_level > 0:
-        ir_root = optimizer.replace_single_case(ir_root)
         ir_root = optimizer.optimize_if(ir_root)
         ir_root = optimizer.combine_cases(ir_root)
-    return Verilog(ir_root, context)
+        ir_root = optimizer.remove_unreferenced_states(ir_root)
+    return Verilog.from_list_ir(ir_root, context)
+
+
+def convert_graph(func: ast.FunctionDef, optimization_level: int):
+    """
+    Wrapper for Python to Verilog conversion
+    """
+
+    ir, context = Generator2Graph(func).results
+    if optimization_level > 0:
+        pass
+    return Verilog.from_graph_ir(ir, context)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description=__doc__, formatter_class=argparse.RawTextHelpFormatter
     )
 
@@ -88,27 +100,27 @@
         python = python_file.read()
         _locals: dict[str, str] = {}
         exec(python, None, _locals)  # grab's exec's populated scoped variables
 
         tree = ast.parse(python)
         function = tree.body[0]
         assert isinstance(function, ast.FunctionDef)
-        verilog = convert(function, args.optimization_level)
+        verilog = convert_list(function, args.optimization_level)
 
         with open(
             os.path.abspath(args.output), mode="w+", encoding="utf8"
         ) as module_file:
-            module_file.write(verilog.get_module().to_string())
+            module_file.write(verilog.get_module_lines().to_string())
 
         if args.test_cases != "":
             with open(
                 os.path.abspath(args.testbench), mode="w+", encoding="utf8"
             ) as tb_file:
                 tb_file.write(
-                    verilog.get_testbench(ast.literal_eval(args.test_cases))
+                    verilog.new_testbench(ast.literal_eval(args.test_cases))
                     .to_lines()
                     .to_string()
                 )
         elif args.test_cases == "" and args.testbench != get_default_tb_filename(
             input_file_stem
         ):
             raise argparse.ArgumentError(
```

### Comparing `python2verilog-0.0.3/python2verilog/frontend/generator_parser.py` & `python2verilog-0.0.4/python2verilog/frontend/generator_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,138 +4,70 @@
 import copy
 import warnings
 import ast as pyast
 from typing import Optional
 
 from .. import ir
 from ..utils.string import Lines, Indent
+from ..utils.assertions import assert_type, assert_list_type
 
 
-class GeneratorParser:
+class Generator2List:
     """
     Parses python generator functions to Verilog AST
     """
 
     def __init__(self, python_func: pyast.FunctionDef):
         """
         Initializes the parser, does quick setup work
         """
-        assert isinstance(python_func, pyast.FunctionDef)
-        self._name = python_func.name
-        self._unique_name_counter = 0
-        self._global_vars: dict[str, str] = {}
+        self._name = assert_type(python_func.name, str)
+        self._context = ir.Context(name=assert_type(python_func.name, str))
         self._python_func = python_func
 
         assert python_func.returns is not None, "Write a return type-hint for function"
-        self._output_vars = self.__generate_output_vars(python_func.returns, "")
-        self._input_vars = [var.arg for var in self._python_func.args.args]
-        self._root = self.__parse_statements(list(python_func.body), "")
+        self._context.output_vars = self.__generate_output_vars(python_func.returns, "")
+        self._context.input_vars = [var.arg for var in self._python_func.args.args]
 
-    def __str__(self):
-        return self.generate_verilog().to_string()
-
-    def get_root(self):
-        """
-        Gets the root of the IR tree
-        """
-        return copy.deepcopy(self._root)
+        self.state_var = ir.State("_state")
+        self.states = ir.Case(
+            self.state_var,
+            [],
+        )
 
-    def generate_verilog(self, indent: int = 0):
-        """
-        Generates the verilog (does the most work, calls other functions)
-        """
-        stmt_lines = (
-            self.__parse_statements(
-                list(self._python_func.body),
-                prefix="",
-                end_stmts=[ir.NonBlockingSubsitution(ir.Var("_done"), ir.Int(1))],
-            ).to_lines(),
-            Lines(),
+        done_state = self.__add_state_var(ir.State("_statedone"))
+        self._root = self.__parse_statements(
+            list(python_func.body), "_state", done_state
         )
-        module_lines = self.__stringify_module()
-        decl_lines = self.__stringify_declarations(self._global_vars)
-        always_blk_lines = self.__stringify_always_block()
-        decl_and_always_blk_lines = (
-            decl_lines[0].concat(always_blk_lines[0]),
-            decl_lines[1].concat(always_blk_lines[1]),
-        )  # TODO: there should be a function for this
-        init_lines = self.__stringify_initialization(self._global_vars)
 
-        return Lines.nestify(
-            [
-                module_lines,
-                decl_and_always_blk_lines,
-                init_lines,
-                stmt_lines,
-            ],
-            indent,
+        self.states.case_items.append(
+            ir.CaseItem(
+                done_state,
+                [ir.NonBlockingSubsitution(ir.Var("_done"), ir.Int(1))],
+            )
         )
 
-    def parse_statements(
-        self,
-        stmts: list[pyast.AST],
-        prefix: str,
-        end_stmts: Optional[list[ir.Statement]] = None,
-        reset_to_zero: bool = False,
-    ):
-        """
-        Parses a list of python statements
-        """
-        return self.__parse_statements(stmts, prefix, end_stmts, reset_to_zero)
+    def __str__(self):
+        return self.generate_verilog().to_string()
 
-    def __parse_statements(
-        self,
-        stmts: list[pyast.AST],
-        prefix: str,
-        end_stmts: Optional[list[ir.Statement]] = None,
-        reset_to_zero: bool = False,
-    ):
-        """
-        Warning: mutates global_vars
+    wow_counter = 0
 
-        {
-            <statement0>
-            <statement1>
-            ...
-        }
-        """
-        if not end_stmts:
-            end_stmts = []
-        assert end_stmts is not None
-        state_var = self.__add_global_var(
-            str(0), f"{prefix}_STATE{self.__create_unique_name()}"
-        )
-        cases = []
-
-        index = 0
-        for stmt in stmts:
-            body = self.__parse_statement(stmt, prefix=state_var)
-            case_item = ir.CaseItem(ir.Expression(str(index)), body)
-            if (
-                not isinstance(stmt, pyast.For)
-                and not isinstance(stmt, pyast.While)
-                and not isinstance(stmt, pyast.If)
-            ):
-                case_item.append_end_statements(
-                    [
-                        ir.StateSubsitution(
-                            ir.Var(state_var), ir.Add(ir.Var(state_var), ir.Int(1))
-                        )
-                    ]
-                )
-            cases.append(case_item)  # TODO: cases can have multiple statements
-            index += 1
-        if reset_to_zero:
-            end_stmts.append(ir.NonBlockingSubsitution(ir.Var(state_var), ir.Int(0)))
-
-        the_case = ir.Case(ir.Expression(state_var), cases)
-        assert end_stmts is not None
-        the_case.append_end_statements(end_stmts)
+    def __add_state_var(self, state: ir.State):
+        if state.string == "_state4while4":
+            self.wow_counter += 1
+            # if self.wow_counter == 1:
+            #     raise Exception()
+        self._context.state_vars.append(state)
+        return state
 
-        return ir.Case(ir.Expression(state_var), cases)
+    def get_root(self):
+        """
+        Gets the root of the IR tree
+        """
+        return copy.deepcopy(self.states)
 
     @staticmethod
     def __generate_output_vars(node: pyast.AST, prefix: str):
         """
         Generates the yielded variables of the function
         """
         assert isinstance(node, pyast.Subscript)
@@ -143,45 +75,63 @@
             return [f"{prefix}_out{str(i)}" for i in range(len(node.slice.elts))]
         if isinstance(node.slice, pyast.Name):
             return [f"{prefix}_out0"]
         raise NotImplementedError(
             f"Unexpected function return type hint {type(node.slice)}, {pyast.dump(node.slice)}"
         )
 
-    def __create_unique_name(self):
-        """
-        Generates an id that is unique among all unique global variables
-        """
-        self._unique_name_counter += 1
-        return f"{self._unique_name_counter}"
-
     def __add_global_var(self, initial_value: str, name: str):
         """
         Adds global variables
         """
-        self._global_vars[name] = initial_value
+        self._context.global_vars[name] = initial_value
         return name
 
     def get_context(self):
         """
         Gets the context of the Python function
         """
-        return ir.Context(
-            name=self._name,
-            global_vars=copy.deepcopy(self._global_vars),
-            input_vars=copy.deepcopy(self._input_vars),
-            output_vars=copy.deepcopy(self._output_vars),
-        )
+        self.__add_global_var(str(1), self.state_var.to_string())  # State 0 is done
+        for i, var in enumerate(self._context.state_vars):
+            self.__add_global_var(str(i), var.to_string())
+        return self._context
 
     def get_results(self):
         """
         Gets root of IR and Context
         """
         return (self.get_root(), self.get_context())
 
+    def generate_verilog(self, indent: int = 0):
+        """
+        Generates the verilog (does the most work, calls other functions)
+        """
+        stmt_lines = (
+            self.states.to_lines(),
+            Lines(),
+        )
+        module_lines = self.__stringify_module()
+        decl_lines = self.__stringify_declarations(self._context.global_vars)
+        always_blk_lines = self.__stringify_always_block()
+        decl_and_always_blk_lines = (
+            decl_lines[0].concat(always_blk_lines[0]),
+            decl_lines[1].concat(always_blk_lines[1]),
+        )  # TODO: there should be a function for this
+        init_lines = self.__stringify_initialization(self._context.global_vars)
+
+        return Lines.nestify(
+            [
+                module_lines,
+                decl_and_always_blk_lines,
+                init_lines,
+                stmt_lines,
+            ],
+            indent,
+        )
+
     @staticmethod
     def __stringify_always_block():
         """
         always @(posedge _clock) begin
         end
         """
         return (
@@ -230,49 +180,53 @@
             "function",
         }  # Verilog Reserved Keywords
         start_lines += f"module {self._name}("
         start_lines += Indent(1) + "input wire _clock,"
         start_lines += Indent(1) + "input wire _start,"
         for var in self._python_func.args.args:
             start_lines += Indent(1) + f"input wire signed [31:0] {var.arg},"
-        for var in self._output_vars:
+        for var in self._context.output_vars:
             start_lines += Indent(1) + f"output reg signed [31:0] {var},"
         start_lines += Indent(1) + "output reg _done,"
         start_lines += Indent(1) + "output reg _valid"
         start_lines += ");"
         end_lines += "endmodule"
         return (start_lines, end_lines)
 
-    def __parse_for(self, node: pyast.For, prefix: str):
-        """
-        Creates a conditional while loop from for loop
-        """
-        raise NotImplementedError("for not implemented")
-
     def __parse_targets(self, nodes: list[pyast.AST]):
         """
         Warning: only single target on left-hand-side supported
 
         <target0, target1, ...> =
         """
         assert len(nodes) == 1
         node = nodes[0]
         if isinstance(node, pyast.Subscript):
             assert isinstance(node.value, pyast.Name)
             if node.value.id not in set(
-                [*self._global_vars, *self._output_vars, *self._input_vars]
+                [
+                    *self._context.global_vars,
+                    *self._context.output_vars,
+                    *self._context.input_vars,
+                ]
             ):
                 warnings.warn(
                     str(
-                        set([*self._global_vars, *self._output_vars, *self._input_vars])
+                        set(
+                            [
+                                *self._context.global_vars,
+                                *self._context.output_vars,
+                                *self._context.input_vars,
+                            ]
+                        )
                     )
                 )
                 self.__add_global_var(str(0), node.value.id)
         elif isinstance(node, pyast.Name):
-            if node.id not in self._global_vars:
+            if node.id not in self._context.global_vars:
                 self.__add_global_var(str(0), node.id)
         else:
             raise TypeError(f"Unsupported lvalue type {type(node)} {pyast.dump(node)}")
         return self.__parse_expression(node)
 
     def __parse_assign(self, node: pyast.Assign):
         """
@@ -280,102 +234,108 @@
         """
         assign = ir.NonBlockingSubsitution(
             self.__parse_targets(list(node.targets)),
             self.__parse_expression(node.value),
         )
         return [assign]
 
-    def __parse_statement(self, stmt: pyast.AST, prefix: str):
+    def __parse_statements(
+        self, stmts: list[pyast.AST], prefix: str, next_state: ir.State
+    ):
+        """
+        Returns state of the first stmt in block
+
+        Give it a prefix and name-mangling is handled for you
+
+        {
+            <statement0>
+            <statement1>
+            ...
+        }
         """
-        <statement> (e.g. assign, for loop, etc., those that do not return a value)
+        assert isinstance(stmts, list)
+        assert isinstance(prefix, str)
+        assert isinstance(next_state, ir.State)
+
+        # state[x] has next state of state[x+1]
+        cur_states = [ir.State(f"{prefix}{i}") for i in range(len(stmts))]
+        next_states = cur_states[1:] + [next_state]
+
+        for stmt, cur, nextt in zip(stmts, cur_states, next_states):
+            self.__parse_statement(stmt, cur, nextt)
+
+        return cur_states[0]
+
+    def __parse_statement(
+        self, stmt: pyast.AST, cur_state: ir.State, next_state: ir.State
+    ):
         """
+        <statement> (e.g. assign, for loop, etc., cannot be equated to)
+
+        creates cur_state
+        """
+        body = []
         if isinstance(stmt, pyast.Assign):
-            return self.__parse_assign(stmt)
-        if isinstance(stmt, pyast.For):
-            return self.__parse_for(stmt, prefix=prefix)
-        if isinstance(stmt, pyast.Expr):
-            return self.__parse_statement(stmt.value, prefix=prefix)
-        if isinstance(stmt, pyast.Yield):
-            return self.__parse_yield(stmt)
-        if isinstance(stmt, pyast.While):
-            return self.__parse_while(stmt, prefix=prefix)
-        if isinstance(stmt, pyast.If):
-            return self.__parse_ifelse(stmt, prefix=prefix)
-        if isinstance(stmt, pyast.AugAssign):
+            body = self.__parse_assign(stmt)
+        elif isinstance(stmt, pyast.Yield):
+            body = self.__parse_yield(stmt)
+        elif isinstance(stmt, pyast.While):
+            body = self.__parse_while(stmt, cur_state, next_state)
+        elif isinstance(stmt, pyast.If):
+            body = self.__parse_ifelse(stmt, cur_state, next_state)
+        elif isinstance(stmt, pyast.Expr):
+            # TODO: solve the inconsistency
+            # raise Exception(f"{pyast.dump(stmt)}")
+            self.__parse_statement(stmt.value, cur_state, next_state)
+            return
+        elif isinstance(stmt, pyast.AugAssign):
             assert isinstance(
                 stmt.target, pyast.Name
             ), "Error: only supports single target"
-            return [
+            body = [
                 ir.NonBlockingSubsitution(
                     self.__parse_expression(stmt.target),
                     self.__parse_expression(
                         pyast.BinOp(stmt.target, stmt.op, stmt.value)
                     ),
                 )
             ]
-        raise TypeError(
-            "Error: unexpected statement type", type(stmt), pyast.dump(stmt)
+        else:
+            raise TypeError(
+                "Error: unexpected statement type", type(stmt), pyast.dump(stmt)
+            )
+
+        self.__add_state_var(cur_state)
+        self.states.case_items.append(
+            ir.CaseItem(
+                cur_state,
+                [ir.StateSubsitution(self.state_var, next_state), *body],
+            )
         )
 
-    def __parse_ifelse(self, stmt: pyast.If, prefix: str):
+    def __parse_ifelse(self, stmt: pyast.If, cur_state: ir.State, next_state: ir.State):
         """
         If statement
         """
         assert isinstance(stmt, pyast.If)
-        state_var = self.__add_global_var(
-            str(0), f"{prefix}_IFELSE{self.__create_unique_name()}"
-        )
-        conditional_item = ir.CaseItem(
-            ir.Int(0),
-            [
-                ir.IfElse(
-                    self.__parse_expression(stmt.test),
-                    [ir.NonBlockingSubsitution(ir.Var(state_var), ir.Int(1))],
-                    [ir.NonBlockingSubsitution(ir.Var(state_var), ir.Int(2))],
-                )
-            ],
+
+        then_start_state = self.__parse_statements(
+            list(stmt.body), f"{cur_state.to_string()}then", next_state
         )
-        then_item = ir.CaseItem(
-            ir.Expression("1"),
-            [
-                self.__parse_statements(
-                    list(stmt.body),
-                    f"{state_var}",
-                    end_stmts=[
-                        ir.StateSubsitution(
-                            ir.Var(prefix), ir.Add(ir.Var(prefix), ir.Int(1))
-                        ),
-                        ir.StateSubsitution(ir.Var(state_var), ir.Int(0)),
-                    ],
-                    reset_to_zero=True,
-                )
-            ],
+        else_start_state = self.__parse_statements(
+            list(stmt.orelse), f"{cur_state.to_string()}else", next_state
         )
-        else_item = ir.CaseItem(
-            ir.Expression("2"),
-            [
-                self.__parse_statements(
-                    list(stmt.orelse),
-                    f"{state_var}",
-                    end_stmts=[
-                        ir.StateSubsitution(
-                            ir.Var(prefix), ir.Add(ir.Var(prefix), ir.Int(1))
-                        ),
-                        ir.StateSubsitution(ir.Var(state_var), ir.Int(0)),
-                    ],
-                    reset_to_zero=True,
-                )
-            ],
+
+        ifelse = ir.IfElse(
+            self.__parse_expression(stmt.test),
+            [ir.StateSubsitution(self.state_var, then_start_state)],
+            [ir.StateSubsitution(self.state_var, else_start_state)],
         )
-        return [
-            ir.IfElseWrapper(
-                ir.Expression(f"{state_var}"),
-                [conditional_item, then_item, else_item],
-            )
-        ]
+
+        return [ifelse]
 
     def __parse_yield(self, node: pyast.Yield):
         """
         Warning: may not work for single output
 
         Warning: requires self.yieldVars to be complete
 
@@ -388,22 +348,23 @@
         else:
             raise NotImplementedError(
                 f"Unexpected yield {type(node.value)} {pyast.dump(node)}"
             )
         try:
             return [
                 ir.NonBlockingSubsitution(
-                    ir.Var(self._output_vars[idx]), self.__parse_expression(elem)
+                    ir.Var(self._context.output_vars[idx]),
+                    self.__parse_expression(elem),
                 )
                 for idx, elem in enumerate(output_vars)
             ] + [ir.ValidSubsitution(ir.Var("_valid"), ir.Int(1))]
-        except IndexError as e:
+        except IndexError as err:
             raise IndexError(
                 "yield return length differs from function return length type hint"
-            ) from e
+            ) from err
 
     def __parse_binop_improved(self, expr: pyast.BinOp):
         """
         <left> <op> <right>
         """
         if isinstance(expr.op, pyast.Add):
             return ir.Add(
@@ -444,35 +405,19 @@
             # e.g. Verilog: -5 / 2 == -2, Python: -5 // 2 == -3
             if (
                 isinstance(expr.op, pyast.FloorDiv)
                 and isinstance(expr.right, pyast.Constant)
                 and expr.right.value > 0
                 and expr.right.value % 2 == 0
             ):
-                # return vast.Expression(
-                #     f"({self.parse_expression(expr.left).to_string()}
-                # >> {int(expr.right.value / 2)})"
-                # )
                 a_var = self.__parse_expression(expr.left).to_string()
                 b_var = expr.right.value
-                # return vast.Expression(
-                #     f"({a} > 0) ? ({a} >> {int(b / 2)}) : -(-({a}) >> {int(b / 2)})"
-                # )
                 return ir.Expression(
                     f"({a_var} > 0) ? ({a_var} / {b_var}) : ({a_var} / {b_var} - 1)"
                 )
-
-            # warnings.warn(pyast.dump(expr))
-            # return irast.Expression(
-            #     "("
-            #     + self.__parse_expression(expr.left).to_string()
-            #     + self.__parse_binop(expr)
-            #     + self.__parse_expression(expr.right).to_string()
-            #     + ")"
-            # )
             return self.__parse_binop_improved(expr)
         if isinstance(expr, pyast.UnaryOp):
             if isinstance(expr.op, pyast.USub):
                 return ir.Expression(
                     f"-({self.__parse_expression(expr.operand).to_string()})"
                 )
             raise TypeError(
@@ -520,49 +465,26 @@
                 "Error: unknown operator", type(node.ops[0]), pyast.dump(node.ops[0])
             )
         return ir.Expression(
             f"{self.__parse_expression(node.left).to_string()} {operator}"
             f" {self.__parse_expression(node.comparators[0]).to_string()}"
         )
 
-    def __parse_while(self, stmt: pyast.While, prefix: str):
+    def __parse_while(
+        self, stmt: pyast.While, cur_state: ir.State, next_state: ir.State
+    ):
         """
         Converts while loop to a while-true-if-break loop
         """
         assert isinstance(stmt, pyast.While)
-        assert prefix != ""
-        state_var = self.__add_global_var(
-            str(0), f"{prefix}_WHILE{self.__create_unique_name()}"
-        )
-        conditional_item = ir.CaseItem(
-            ir.Int(0),
-            [
-                ir.IfElse(
-                    ir.Expression(
-                        f"!({self.__parse_expression(stmt.test).to_string()})"
-                    ),
-                    [
-                        ir.StateSubsitution(
-                            ir.Var(prefix), ir.Add(ir.Var(prefix), ir.Int(1))
-                        )
-                    ],
-                    [ir.NonBlockingSubsitution(ir.Var(state_var), ir.Int(1))],
-                )
-            ],
+
+        body_start_state = self.__parse_statements(
+            list(stmt.body), f"{cur_state.to_string()}while", cur_state
         )
-        then_item = ir.CaseItem(
-            ir.Expression("1"),
-            [
-                self.__parse_statements(
-                    list(stmt.body),
-                    f"{state_var}",
-                    end_stmts=[ir.NonBlockingSubsitution(ir.Var(state_var), ir.Int(0))],
-                    reset_to_zero=True,
-                )
-            ],
+
+        ifelse = ir.IfElse(
+            self.__parse_expression(stmt.test),
+            [ir.StateSubsitution(self.state_var, body_start_state)],
+            [ir.StateSubsitution(self.state_var, next_state)],
         )
-        return [
-            ir.WhileWrapper(
-                ir.Expression(f"{state_var}"),
-                [conditional_item, then_item],
-            )
-        ]
+
+        return [ifelse]
```

### Comparing `python2verilog-0.0.3/python2verilog/ir/context.py` & `python2verilog-0.0.4/python2verilog/ir/context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 """Context for Intermediate Representation"""
+from __future__ import annotations
+from typing import Optional
+from ..utils.assertions import assert_list_type, assert_type, assert_dict_type
 
 
 class Context:
     """
     Context needed by the Intermediate Representation
     E.g. variables, I/O, parameters, localparam
     """
 
     def __init__(
         self,
-        name: str,
-        global_vars: dict[str, str],
-        input_vars: list[str],
-        output_vars: list[str],
+        name: str = "",
+        global_vars: Optional[dict[str, str]] = None,
+        input_vars: Optional[list[str]] = None,
+        output_vars: Optional[list[str]] = None,
+        state_vars: Optional[list[str]] = None,
     ):
-        self.name = name
-        self.global_vars = global_vars
-        self.input_vars = input_vars
-        self.output_vars = output_vars
-        # TODO: add strings for name of valid, done, clock, etc.
+        self.name = assert_type(name, str)
+        self.global_vars = assert_dict_type(global_vars, str, str)
+        self.input_vars = assert_list_type(input_vars, str)
+        self.output_vars = assert_list_type(output_vars, str)
+        self.state_vars = assert_list_type(state_vars, str)
 
     def is_declared(self, name: str):
         """
         Checks if a variable has been already declared or not
         """
         return name in set([*self.global_vars, *self.input_vars, *self.output_vars])
+
+    def to_string(self):
+        """
+        To string
+        """
+        return str(self.__dict__)
```

### Comparing `python2verilog-0.0.3/python2verilog/ir/expressions.py` & `python2verilog-0.0.4/python2verilog/ir/expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def to_string(self):
         """
         To String
         """
         return self.string
 
     def __repr__(self):
-        return f"({__name__}: {self.to_string()})"
+        return f"({self.to_string()})"
 
 
 class Int(Expression):
     """
     Integer literal
     """
 
@@ -39,14 +39,20 @@
     """
 
     def __init__(self, name: str):
         assert isinstance(name, str)
         super().__init__(name)
 
 
+class State(Var):
+    """
+    State variable
+    """
+
+
 class BinOp(Expression):
     """
     <left> <op> <right>
     """
 
     def __init__(self, left: Expression, right: Expression, oper: str):
         self.left = left
```

### Comparing `python2verilog-0.0.3/python2verilog/ir/statements.py` & `python2verilog-0.0.4/python2verilog/ir/statements.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,57 +3,45 @@
 from __future__ import annotations
 import warnings
 import inspect
 from typing import Optional
 
 from python2verilog.ir.expressions import Expression
 
-from ..utils.string import Lines
-from ..utils.assertions import assert_list_elements
+from ..utils.string import Lines, ImplementsToLines
+from ..utils.assertions import assert_list_type
 
 
-class Statement:
+class Statement(ImplementsToLines):
     """
     Represents a statements (i.e. a line or a block)
     If used directly, it is treated as a string literal
     """
 
     def __init__(self, literal: Optional[str] = None):
         self.literal = literal
 
     def to_lines(self):
         """
         To Lines
         """
         return Lines(self.literal)
 
-    def to_string(self):
-        """
-        To String
-        """
-        return self.to_lines().to_string()
-
     def __repr__(self):
         return self.to_string()
 
-    def append_end_statements(self, _: list[Statement]):
-        """
-        Abstract
-        """
-        raise NotImplementedError("cannot append to statement")
-
 
 def is_valid_append_end_statements(stmt: Statement, statements: list[Statement]):
     """
     Checks if stmt encapsulates other Statements or not
     If it does, it handles the append, otherwise returns false
     # TODO: there should be a subclass/interface for ones that do encapsulate
     """
     if isinstance(stmt, (Case, IfElse)):
-        stmt.append_end_statements(assert_list_elements(statements, Statement))
+        stmt.append_end_statements(assert_list_type(statements, Statement))
         return True
     return False
 
 
 class Subsitution(Statement):
     """
     Interface for
@@ -146,15 +134,15 @@
             string += " signed"
         string += f" [{self.size-1}:0]"
         string += f" {self.name}"
         string += ";"
         return Lines(string)
 
 
-class CaseItem:
+class CaseItem(ImplementsToLines):
     """
     case item, i.e.
     <condition>: begin
         <statements>
     end
     """
 
@@ -175,28 +163,20 @@
         lines = Lines()
         lines += f"{self.condition.to_string()}: begin"
         for stmt in self.statements:
             lines.concat(stmt.to_lines(), indent=1)
         lines += "end"
         return lines
 
-    def to_string(self):
-        """
-        To String
-        """
-        return self.to_lines().to_string()
-
     def append_end_statements(self, statements: list[Statement]):
         """
         Append statements to case item
         """
         if not is_valid_append_end_statements(self.statements[-1], statements):
-            self.statements = self.statements + assert_list_elements(
-                statements, Statement
-            )
+            self.statements = self.statements + assert_list_type(statements, Statement)
         return self
 
 
 class Case(Statement):
     """
     case (<expression>)
         <items[0]>
@@ -230,15 +210,15 @@
         return lines
 
     def append_end_statements(self, statements: list[Statement]):
         """
         Adds statements to the last case item
         """
         self.case_items[-1].append_end_statements(
-            assert_list_elements(statements, Statement)
+            assert_list_type(statements, Statement)
         )
         return self
 
 
 class IfElse(Statement):
     """
     If Else
@@ -251,16 +231,16 @@
         else_body: list[Statement],
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         assert isinstance(condition, Expression)
         self.condition = condition
-        self.then_body = assert_list_elements(then_body, Statement)
-        self.else_body = assert_list_elements(else_body, Statement)
+        self.then_body = assert_list_type(then_body, Statement)
+        self.else_body = assert_list_type(else_body, Statement)
 
     def to_lines(self):
         lines = Lines()
         lines += f"if ({self.condition.to_string()}) begin"
         for stmt in self.then_body:
             lines.concat(stmt.to_lines(), indent=1)
         lines += "end else begin"
@@ -269,15 +249,15 @@
         lines += "end"
         return lines
 
     def append_end_statements(self, statements: list[Statement]):
         """
         Appends statements to both branches
         """
-        statements = assert_list_elements(statements, Statement)
+        statements = assert_list_type(statements, Statement)
         # warnings.warn("appending " + statements[0].to_string())
         # if len(statements) > 1:
         #     warnings.warn(statements[1].to_string())
         if not is_valid_append_end_statements(self.then_body[-1], statements):
             self.then_body = self.then_body + statements
         if not is_valid_append_end_statements(self.else_body[-1], statements):
             self.else_body = self.else_body + statements
@@ -297,15 +277,15 @@
     """
 
     def append_end_statements(self, statements: list[Statement]):
         """
         While statements have a special case structure,
         where their first case always contains an if statement
         """
-        statements = assert_list_elements(statements, Statement)
+        statements = assert_list_type(statements, Statement)
         assert isinstance(self.case_items[0], CaseItem)
         assert isinstance(self.case_items[0].statements[0], IfElse)
         self.case_items[0].statements[0].then_body = (
             self.case_items[0].statements[0].then_body + statements
         )
         return self
```

### Comparing `python2verilog-0.0.3/python2verilog/utils/string.py` & `python2verilog-0.0.4/python2verilog/utils/string.py`

 * *Files 10% similar despite different names*

```diff
@@ -132,7 +132,28 @@
 
     def __radd__(self, other: str):
         assert isinstance(other, str)
         return other + self.indentify(self.indent)
 
     def __str__(self):
         return self.indentify(self.indent)
+
+
+class ImplementsToLines:
+    """
+    A base class defining an interface for classes that need to provide a 'to_lines' method
+    """
+
+    def to_lines(self):
+        """
+        To Lines
+        """
+        raise NotImplementedError("Derived class must implement to_lines")
+
+    def to_string(self):
+        """
+        To string
+        """
+        return str(self.to_lines())
+
+    def __str__(self):
+        return self.to_string()
```

### Comparing `python2verilog-0.0.3/python2verilog/utils/visualization.py` & `python2verilog-0.0.4/python2verilog/utils/visualization.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,21 @@
     Any iterable of tuples where the tuples are of length > 0 will work.
     Visualizes the first 3 elements of each tuple as (x, y, colour)
     """
 
     # Generate the data using the generator function
     data_triple_list = []
 
-    for yields in generator_inst:
+    for idx, yields in enumerate(generator_inst):
         if len(yields) >= 3:
             data_triple_list.append(yields[:3])
         elif len(yields) >= 2:
             data_triple_list.append((*yields[:2], 1))
         else:
-            data_triple_list.append((yields[0], 1, 2))
+            data_triple_list.append((yields[0], idx, 1))
 
     data_triple = np.array(data_triple_list)
 
     height = max(data_triple[:, 0])
     width = max(data_triple[:, 1])
     grid = np.zeros((int(height) + 1, int(width) + 1))
     for x_coord, y_coord, colour in data_triple:
```

### Comparing `python2verilog-0.0.3/python2verilog.egg-info/PKG-INFO` & `python2verilog-0.0.4/python2verilog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.0.3
+Version: 0.0.4
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `python2verilog-0.0.3/python2verilog.egg-info/SOURCES.txt` & `python2verilog-0.0.4/python2verilog.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 python2verilog.egg-info/PKG-INFO
 python2verilog.egg-info/SOURCES.txt
 python2verilog.egg-info/dependency_links.txt
 python2verilog.egg-info/top_level.txt
 python2verilog/backend/__init__.py
 python2verilog/backend/verilog.py
 python2verilog/frontend/__init__.py
+python2verilog/frontend/generator2graph.py
 python2verilog/frontend/generator_parser.py
 python2verilog/ir/__init__.py
 python2verilog/ir/context.py
 python2verilog/ir/expressions.py
+python2verilog/ir/graph.py
 python2verilog/ir/statements.py
 python2verilog/optimizer/__init__.py
 python2verilog/optimizer/optimizer.py
 python2verilog/utils/__init__.py
 python2verilog/utils/assertions.py
 python2verilog/utils/string.py
 python2verilog/utils/visualization.py
```

