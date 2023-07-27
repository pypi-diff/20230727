# Comparing `tmp/aiida-worktree-0.0.1.tar.gz` & `tmp/aiida-worktree-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-worktree-0.0.1.tar", last modified: Wed Jul 19 16:43:18 2023, max compression
+gzip compressed data, was "aiida-worktree-0.0.2.tar", last modified: Thu Jul 27 12:53:42 2023, max compression
```

## Comparing `aiida-worktree-0.0.1.tar` & `aiida-worktree-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,39 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-19 16:43:18.952461 aiida-worktree-0.0.1/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1066 2023-07-19 14:36:50.000000 aiida-worktree-0.0.1/LICENSE
--rw-rw-r--   0 xing      (1000) xing      (1000)     2905 2023-07-19 16:43:18.952461 aiida-worktree-0.0.1/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     2559 2023-07-19 15:48:42.000000 aiida-worktree-0.0.1/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-19 16:43:18.952461 aiida-worktree-0.0.1/aiida_worktree/
--rw-rw-r--   0 xing      (1000) xing      (1000)       74 2023-07-19 16:02:27.000000 aiida-worktree-0.0.1/aiida_worktree/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4599 2023-07-19 14:41:53.000000 aiida-worktree-0.0.1/aiida_worktree/decorator.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-19 16:43:18.952461 aiida-worktree-0.0.1/aiida_worktree/engine/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-07-19 14:37:08.000000 aiida-worktree-0.0.1/aiida_worktree/engine/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    27373 2023-07-19 15:09:15.000000 aiida-worktree-0.0.1/aiida_worktree/engine/worktree.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-19 16:43:18.952461 aiida-worktree-0.0.1/aiida_worktree/nodes/
--rw-rw-r--   0 xing      (1000) xing      (1000)      687 2023-07-19 14:58:04.000000 aiida-worktree-0.0.1/aiida_worktree/nodes/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4836 2023-07-19 16:09:34.000000 aiida-worktree-0.0.1/aiida_worktree/nodes/qe.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7206 2023-07-19 16:09:23.000000 aiida-worktree-0.0.1/aiida_worktree/nodes/test.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-19 16:43:18.952461 aiida-worktree-0.0.1/aiida_worktree/properties/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-07-19 14:37:08.000000 aiida-worktree-0.0.1/aiida_worktree/properties/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3906 2023-07-19 14:37:08.000000 aiida-worktree-0.0.1/aiida_worktree/properties/built_in.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2739 2023-07-19 14:37:08.000000 aiida-worktree-0.0.1/aiida_worktree/utils.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2477 2023-07-19 14:40:29.000000 aiida-worktree-0.0.1/aiida_worktree/worktree.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-19 16:43:18.952461 aiida-worktree-0.0.1/aiida_worktree.egg-info/
--rw-rw-r--   0 xing      (1000) xing      (1000)     2905 2023-07-19 16:43:18.000000 aiida-worktree-0.0.1/aiida_worktree.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      595 2023-07-19 16:43:18.000000 aiida-worktree-0.0.1/aiida_worktree.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2023-07-19 16:43:18.000000 aiida-worktree-0.0.1/aiida_worktree.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      131 2023-07-19 16:43:18.000000 aiida-worktree-0.0.1/aiida_worktree.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       90 2023-07-19 16:43:18.000000 aiida-worktree-0.0.1/aiida_worktree.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       15 2023-07-19 16:43:18.000000 aiida-worktree-0.0.1/aiida_worktree.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2023-07-19 16:43:18.952461 aiida-worktree-0.0.1/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     1320 2023-07-19 14:41:32.000000 aiida-worktree-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.841282 aiida-worktree-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-27 12:53:42.841282 aiida-worktree-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.833282 aiida-worktree-0.0.2/aiida_worktree/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.837282 aiida-worktree-0.0.2/aiida_worktree/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29694 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/engine/worktree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.837282 aiida-worktree-0.0.2/aiida_worktree/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/nodes/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/nodes/qe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/nodes/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.837282 aiida-worktree-0.0.2/aiida_worktree/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/properties/built_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/aiida_worktree/worktree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.837282 aiida-worktree-0.0.2/aiida_worktree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 12:53:42.000000 aiida-worktree-0.0.2/aiida_worktree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:53:42.841282 aiida-worktree-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:42.841282 aiida-worktree-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_calcfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_calcjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_failed_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_qe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_workchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-27 12:53:31.000000 aiida-worktree-0.0.2/tests/test_yaml.py
```

### Comparing `aiida-worktree-0.0.1/LICENSE` & `aiida-worktree-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.1/aiida_worktree/decorator.py` & `aiida-worktree-0.0.2/aiida_worktree/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,151 +1,127 @@
-from typing import Any
-from scinode.utils.node import get_executor
-from aiida.engine.processes.functions import calcfunction, workfunction
-from aiida.engine.processes.calcjobs import CalcJob
-from aiida.engine.processes.workchains import WorkChain
-from aiida.orm.nodes.process.calculation.calcfunction import CalcFunctionNode
-from aiida.orm.nodes.process.workflow.workfunction import WorkFunctionNode
-from aiida.engine.processes.ports import PortNamespace
-
-
-def add_input_recursive(inputs, port, prefix=None):
-    """Add input recursively."""
-    if prefix is None:
-        port_name = port.name
-    else:
-        port_name = f"{prefix}.{port.name}"
-    if isinstance(port, PortNamespace):
-        inputs.append(["General", port_name, ["General", {"default": {}}]])
-        for key, value in port.items():
-            add_input_recursive(inputs, value, prefix=port_name)
-    else:
-        inputs.append(["General", port_name])
-    return inputs
-
+def get_executor(data):
+    """Import executor from path and return the executor and type."""
+    import importlib
+    from aiida.plugins import CalculationFactory, WorkflowFactory, DataFactory
+
+    is_pickle = data.get("is_pickle", False)
+    type = data.get("type", "function")
+    if is_pickle:
+        import cloudpickle as pickle
 
-def register_node(ndata):
-    """Register a node from a AiiDA component."""
-    from scinode.utils.decorator import register_node as register_scinode_node
-
-    path, executor_name, = ndata.pop(
-        "path"
-    ).rsplit(".", 1)
-    ndata["executor"] = {"path": path, "name": executor_name}
-    executor, type = get_executor(ndata["executor"])
-    # print(executor)
-    if issubclass(executor, CalcJob):
-        ndata["node_type"] = "calcjob"
-    elif issubclass(executor, WorkChain):
-        ndata["node_type"] = "workchain"
+        executor = pickle.loads(data["executor"])
     else:
-        ndata["node_type"] = "normal"
-    inputs = []
-    outputs = []
-    spec = executor.spec()
-    for key, port in spec.inputs.ports.items():
-        add_input_recursive(inputs, port)
-    kwargs = [input[1] for input in inputs]
-    for key, port in spec.outputs.ports.items():
-        outputs.append(["General", port.name])
-    # print("kwargs: ", kwargs)
-    ndata["kwargs"] = kwargs
-    ndata["inputs"] = inputs
-    ndata["outputs"] = outputs
-    identifier = ndata.pop("identifier", ndata["executor"]["name"])
-    node = register_scinode_node(identifier, **ndata)
-    return node
-
-
-# decorator with arguments indentifier, args, kwargs, properties, inputs, outputs, executor
-def decorator_node(
-    identifier=None,
-    node_type="Normal",
-    properties=None,
-    inputs=None,
-    outputs=None,
-    catalog="Others",
-    type="function",
-):
-    """Generate a decorator that register a function as a SciNode node.
-
-    Attributes:
-        indentifier (str): node identifier
-        catalog (str): node catalog
-        args (list): node args
-        kwargs (dict): node kwargs
-        properties (list): node properties
-        inputs (list): node inputs
-        outputs (list): node outputs
-    """
-    properties = properties or []
-    inputs = inputs or []
-    outputs = outputs or []
+        if type == "WorkflowFactory":
+            executor = WorkflowFactory(data["name"])
+        elif type == "CalculationFactory":
+            executor = CalculationFactory(data["name"])
+        elif type == "DataFactory":
+            executor = DataFactory(data["name"])
+        else:
+            module = importlib.import_module("{}".format(data.get("path", "")))
+            executor = getattr(module, data["name"])
 
-    def decorator(func):
-        import cloudpickle as pickle
-        from scinode.utils.decorator import generate_input_sockets, register_node
+    return executor, type
 
-        nonlocal identifier
 
-        if identifier is None:
-            identifier = func.__name__
-        # use cloudpickle to serialize function
-        executor = {
-            "executor": pickle.dumps(func),
-            "type": type,
-            "is_pickle": True,
-        }
-        #
-        # Get the args and kwargs of the function
-        args, kwargs, _inputs = generate_input_sockets(func, inputs, properties)
-        # I don't know why isinstance(func.node_class, CalcFunctionNode) is False
-        # print("func: ", func)
-        # print("node_class: ", func.node_class)
-        if func.node_class is CalcFunctionNode:
-            node_type = "calcfunction"
-        elif func.node_class is WorkFunctionNode:
-            node_type = "workfunction"
-        else:
-            node_type = "Normal"
-        node = register_node(
-            identifier,
-            node_type,
-            args,
-            kwargs,
-            properties,
-            _inputs,
-            outputs,
-            executor,
-            catalog=catalog,
-        )
-        func.identifier = identifier
-        func.node = node
-        return func
-
-    return decorator
-
-
-class NodeDecoratorCollection:
-    """Collection of node decorators."""
+def create_data_node(executor, args, kwargs):
+    from aiida import orm
 
-    node = staticmethod(decorator_node)
+    # print("Create data node: ", executor, args, kwargs)
+    extras = kwargs.pop("extras", {})
+    repository_metadata = kwargs.pop("repository_metadata", {})
+    if issubclass(executor, (orm.BaseType, orm.Dict)):
+        data_node = executor(*args)
+    else:
+        data_node = executor(*args)
+        data_node.base.attributes.set_many(kwargs)
+    data_node.base.extras.set_many(extras)
+    data_node.base.repository.repository_metadata = repository_metadata
+    data_node.store()
+    return data_node
 
-    __call__: Any = node  # Alias '@node' to '@node.node'.
 
+def update_nested_dict(d, key, value):
+    """
+    d = {"base": {"pw": {"parameters": 1}}
+    key = "base.pw.parameters"
+    value = 2
+    """
+    keys = key.split(".")
+    current = d
+    for k in keys[:-1]:
+        current = current.setdefault(k, {})
+    current[keys[-1]] = value
+
+
+def update_nested_dict_with_special_keys(d):
+    # first remove None and empty value
+    d = {k: v for k, v in d.items() if v is not None and v != {}}
+    #
+    special_keys = [k for k in d.keys() if "." in k]
+    for key in special_keys:
+        value = d.pop(key)
+        update_nested_dict(d, key, value)
+    return d
+
+
+def merge_properties(ntdata):
+    """Merge properties."""
+    for name, node in ntdata["nodes"].items():
+        for key, prop in node["properties"].items():
+            if "." in key and prop["value"] not in [None, {}]:
+                root, key = key.split(".", 1)
+                update_nested_dict(
+                    node["properties"][root]["value"], key, prop["value"]
+                )
+                prop["value"] = None
+
+
+def generate_node_graph(pk):
+    from aiida.tools.visualization import Graph
+    from aiida import orm
+
+    graph = Graph()
+    calc_node = orm.load_node(pk)
+    graph.recurse_ancestors(calc_node, annotate_links="both")
+    graph.recurse_descendants(calc_node, annotate_links="both")
+    return graph.graphviz
+
+
+def build_node_link(ntdata):
+    """Create links for nodes.
+    Create the links for node inputs using:
+    1) nodetree links
+    2) if it is a node group tree, expose the group inputs and outputs
+    sockets.
+    """
+    # reset node input links
+    for name, node in ntdata["nodes"].items():
+        for input in node["inputs"]:
+            input["links"] = []
+        for output in node["outputs"]:
+            output["links"] = []
+    for link in ntdata["links"]:
+        to_socket = [
+            socket
+            for socket in ntdata["nodes"][link["to_node"]]["inputs"]
+            if socket["name"] == link["to_socket"]
+        ][0]
+        from_socket = [
+            socket
+            for socket in ntdata["nodes"][link["from_node"]]["outputs"]
+            if socket["name"] == link["from_socket"]
+        ][0]
+        to_socket["links"].append(link)
+        from_socket["links"].append(link)
 
-node = NodeDecoratorCollection()
 
 if __name__ == "__main__":
-    from aiida.engine import calcfunction
-    from aiida_worktree.decorator import node
-
-    @node(
-        identifier="MyAdd",
-        outputs=[["General", "result"]],
-        type="calcfunction",
-    )
-    @calcfunction
-    def myadd(x, y):
-        return x + y
-
-    print(myadd.node)
+    d = {
+        "base": {
+            "pw": {"code": 1, "parameters": 1, "pseudos": 1, "metadata": 1},
+            "kpoints": 1,
+        },
+        "base.pw.parameters": 2,
+    }
+    d = update_nested_dict_with_special_keys(d)
+    print(d)
```

### Comparing `aiida-worktree-0.0.1/aiida_worktree/engine/worktree.py` & `aiida-worktree-0.0.2/aiida_worktree/engine/worktree.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 import functools
 import logging
 import typing as t
 
 from plumpy.persistence import auto_persist
 from plumpy.process_states import Continue, Wait
 from plumpy.workchains import _PropagateReturn
-from plumpy.workchains import WorkChainSpec as PlumpyWorkChainSpec
 
 from aiida.common import exceptions
 from aiida.common.extendeddicts import AttributeDict
 from aiida.common.lang import override
 from aiida import orm
-from aiida.orm import Node, ProcessNode, WorkflowNode
+from aiida.orm import Node, ProcessNode, WorkChainNode
 from aiida.orm.utils import load_node
 
 
 from aiida.engine.processes.exit_code import ExitCode
 from aiida.engine.processes.process import Process, ProcessState
-from aiida.engine.processes.process_spec import ProcessSpec
 
 from aiida.engine.processes.workchains.awaitable import (
     Awaitable,
     AwaitableAction,
     AwaitableTarget,
     construct_awaitable,
 )
@@ -38,70 +36,54 @@
 
 if t.TYPE_CHECKING:
     from aiida.engine.runners import Runner  # pylint: disable=unused-import
 
 __all__ = "WorkTree"
 
 
-def get_input_links(node_name, links):
-    inputs = []
-    for link in links:
-        if link["to_node"] == node_name:
-            inputs.append(link)
-    return inputs
-
-
-class WorkTreeSpec(ProcessSpec, PlumpyWorkChainSpec):
-    pass
-
-
 @auto_persist("_awaitables")
 class WorkTree(Process, metaclass=Protect):
     """The `WorkTree` class is used to construct workflows in AiiDA."""
 
-    _node_class = WorkflowNode
-    _spec_class = WorkTreeSpec
+    # used to create a process node that represents what happened in this process.
+    _node_class = WorkChainNode
+    _spec_class = WorkChainSpec
     _CONTEXT = "CONTEXT"
 
     def __init__(
         self,
         inputs: dict | None = None,
         logger: logging.Logger | None = None,
         runner: "Runner" | None = None,
         enable_persistence: bool = True,
     ) -> None:
-        """Construct a WorkChain instance.
-
-        Construct the instance only if it is a sub class of `WorkChain`, otherwise raise `InvalidOperation`.
+        """Construct a WorkTree instance.
 
-        :param inputs: work chain inputs
+        :param inputs: work tree inputs
         :param logger: aiida logger
-        :param runner: work chain runner
-        :param enable_persistence: whether to persist this work chain
+        :param runner: work tree runner
+        :param enable_persistence: whether to persist this work tree
 
         """
 
         super().__init__(inputs, logger, runner, enable_persistence=enable_persistence)
 
         self._awaitables: list[Awaitable] = []
         self._context = AttributeDict()
 
     @classmethod
-    def spec(cls) -> WorkChainSpec:
-        return super().spec()  # type: ignore[return-value]
-
-    @classmethod
     def define(cls, spec):
         super().define(spec)
         spec.input("input_file", valid_type=orm.SinglefileData, required=False)
         spec.input_namespace("nt", dynamic=True, required=False)
         spec.input_namespace("input_nodes", dynamic=True, required=False)
         spec.exit_code(2, "ERROR_SUBPROCESS", message="A subprocess has failed.")
 
-        spec.output_namespace("results", dynamic=True)
+        spec.output_namespace("new_data", dynamic=True)
+        spec.output_namespace("group_outputs", dynamic=True)
         #
         spec.exit_code(
             201, "UNKNOWN_MESSAGE_TYPE", message="The message type is unknown."
         )
         spec.exit_code(202, "UNKNOWN_NODE_TYPE", message="The node type is unknown.")
         #
         spec.exit_code(
@@ -110,18 +92,19 @@
             message="The outputs of the process do not match the results.",
         )
         spec.exit_code(
             302,
             "NODE_FAILED",
             message="Some of the nodes failed.",
         )
-
-    @property
-    def node(self) -> WorkflowNode:
-        return super().node  # type: ignore
+        spec.exit_code(
+            303,
+            "NODE_NON_ZERO_EXIT_STATUS",
+            message="Some of the nodes exited with non-zero status.",
+        )
 
     @property
     def ctx(self) -> AttributeDict:
         """Get the context."""
         return self._context
 
     @override
@@ -145,18 +128,14 @@
         self._context = saved_state[self._CONTEXT]
 
         self.set_logger(self.node.logger)
 
         if self._awaitables:
             self._action_awaitables()
 
-    @Protect.final
-    def on_run(self):
-        super().on_run()
-
     def _resolve_nested_context(self, key: str) -> tuple[AttributeDict, str]:
         """
         Returns a reference to a sub-dictionary of the context and the last key,
         after resolving a potentially segmented key where required sub-dictionaries are created as needed.
 
         :param key: A key into the context, where words before a dot are interpreted as a key for a sub-dictionary
         """
@@ -250,15 +229,15 @@
             self._update_process_status()
 
     @Protect.final
     def to_context(self, **kwargs: Awaitable | ProcessNode) -> None:
         """Add a dictionary of awaitables to the context.
 
         This is a convenience method that provides syntactic sugar, for a user to add multiple intersteps that will
-        assign a certain value to the corresponding key in the context of the work chain.
+        assign a certain value to the corresponding key in the context of the work tree.
         """
         for key, value in kwargs.items():
             awaitable = construct_awaitable(value)
             awaitable.key = key
             self._insert_awaitable(awaitable)
 
     def _update_process_status(self) -> None:
@@ -272,15 +251,15 @@
     @override
     def run(self) -> t.Any:
         self.report("Run: ")
         self.setup()
         return self._do_step()
 
     def _do_step(self) -> t.Any:
-        """Execute the next step in the outline and return the result.
+        """Execute the next step in the worktree and return the result.
 
         If any awaitables were created, the process will enter in the Wait state,
         otherwise it will go to Continue.
         """
 
         self._awaitables = []
         result: t.Any = None
@@ -385,48 +364,46 @@
         self._resolve_awaitable(awaitable, value)
 
         if self.state == ProcessState.WAITING and not self._awaitables:
             self.resume()
 
     def setup(self):
         from scinode.utils.nt_analysis import ConnectivityAnalysis
+        from aiida_worktree.utils import build_node_link
 
-        self.ctx.results = dict()
+        self.ctx.new_data = dict()
         self.ctx.input_nodes = dict()
         if "input_file" in self.inputs:
             ext = splitext(self.inputs["input_file"].filename)[1]
             with self.inputs["input_file"].open(mode="r") as f:
                 if ext == ".yaml":
                     ntdata = yaml.safe_load(f)
                 else:
                     raise Exception("Please use a yaml file.")
         elif "nt" in self.inputs:
             ntdata = self.inputs["nt"]
         else:
             raise Exception("Please set input!")
 
         # ntdata = jsonref.JsonRef.replace_refs(tntdata, loader = JsonYamlLoader())
-        self.ctx.worktree = ntdata
-        nodes = {}
-        for name, node in ntdata["nodes"].items():
-            inputs = get_input_links(name, ntdata["links"])
-            node["inputs"] = inputs
-            nodes[name] = node
-        self.ctx.nodes = nodes
+        build_node_link(ntdata)
+        self.ctx.nodes = ntdata["nodes"]
         self.ctx.links = ntdata["links"]
         self.ctx.ctrl_links = ntdata["ctrl_links"]
+        self.ctx.worktree = ntdata
+        print("init")
         # init
         for name, node in self.ctx.nodes.items():
             node["state"] = "CREATED"
             node["process"] = None
         #
         nc = ConnectivityAnalysis(ntdata)
         self.ctx.connectivity = nc.build_connectivity()
         self.ctx.msgs = []
-        # self.node.set_process_label(f"WorkTree: {self.ctx.worktree['name']}")
+        self.node.set_process_label(f"WorkTree: {self.ctx.worktree['name']}")
 
     def launch_worktree(self):
         self.report("Lanch worktree.")
         node_to_run = []
         for name, node in self.ctx.nodes.items():
             # update node state
             if node["state"] in ["RUNNING", "FINISHED", "FAILED", "SKIPPED"]:
@@ -447,30 +424,38 @@
             if (
                 node["metadata"]["node_type"]
                 in [
                     "calcfunction",
                     "workfunction",
                     "calcjob",
                     "workchain",
+                    "worktree",
                 ]
                 and node["state"] == "RUNNING"
             ):
                 if node.get("process"):
                     state = node["process"].process_state.value.upper()
                     print(node["name"], state)
                     if state == "FINISHED":
                         node["state"] = state
-                        node["results"] = node["process"].outputs
-                        self.ctx.results[name] = node["results"]
+                        if node["metadata"]["node_type"] == "worktree":
+                            # expose the outputs of nodetree
+                            node["results"] = getattr(
+                                node["process"].outputs, "group_outputs", None
+                            )
+                            # self.ctx.new_data[name] = outputs
+                        else:
+                            node["results"] = node["process"].outputs
+                            # self.ctx.new_data[name] = node["results"]
                         self.ctx.nodes[name]["state"] = "FINISHED"
                         print(f"Node: {name} finished.")
                     elif state == "EXCEPTED":
                         node["state"] = state
                         node["results"] = node["process"].outputs
-                        self.ctx.results[name] = node["results"]
+                        # self.ctx.new_data[name] = node["results"]
                         self.ctx.nodes[name]["state"] = "FAILED"
                         # set child state to FAILED
                         self.set_node_state(
                             self.ctx.connectivity["child_node"][name], "FAILED"
                         )
                         print(f"Node: {name} failed.")
             if node["state"] in ["RUNNING", "CREATED", "READY"]:
@@ -478,35 +463,30 @@
         return flag
 
     def run_nodes(self, names):
         """Run node
         Here we use ToContext to pass the results of the run to the next step.
         This will force the engine to wait for all the submitted processes to
         finish before continuing to the next step.
-
-        Raises:
-            Exception: _description_
-
-        Returns:
-            _type_: _description_
         """
         from aiida_worktree.utils import (
             get_executor,
             create_data_node,
             update_nested_dict_with_special_keys,
         )
 
         for name in names:
-            # print("-" * 60)
+            print("-" * 60)
             node = self.ctx.nodes[name]
-            print(f"Run node: {name}, type: {node['metadata']['node_type']}")
+            print(f"\nRun node: {name}, type: {node['metadata']['node_type']}")
             self.report(f"Run node: {name}, type: {node['metadata']['node_type']}")
             # print("Run node: ", name)
             # print("executor: ", node["executor"])
             executor, _ = get_executor(node["executor"])
+            print("executor: ", executor)
             args, kwargs = self.get_inputs(node)
             # update the port namespace
             kwargs = update_nested_dict_with_special_keys(kwargs)
             print("args: ", args)
             print("kwargs: ", kwargs)
             # kwargs["meta.label"] = name
             # output must be a Data type or a mapping of {string: Data}
@@ -524,15 +504,15 @@
                 # ValueError: attempted to add an input link after the process node was already stored.
                 # self.node.base.links.add_incoming(results, "INPUT_WORK", name)
             elif node["metadata"]["node_type"] == "data":
                 print("node  type: data.")
                 results = create_data_node(executor, args, kwargs)
                 node["results"] = {node["outputs"][0]["name"]: results}
                 node["process"] = results
-                self.ctx.results[name] = results
+                self.ctx.new_data[name] = results
                 self.ctx.nodes[name]["state"] = "FINISHED"
             elif node["metadata"]["node_type"] in ["calcfunction", "workfunction"]:
                 print("node  type: calcfunction/workfunction.")
                 kwargs.setdefault("metadata", {})
                 kwargs["metadata"].update({"call_link_label": name})
                 try:
                     results, process = run_get_node(executor, *args, **kwargs)
@@ -541,28 +521,48 @@
                         results = {node["outputs"][0]["name"]: results}
                     node["results"] = results
                     # print("results: ", results)
                     node["process"] = process
                     self.ctx.nodes[name]["state"] = "FINISHED"
                 except Exception as e:
                     print(e)
+                    self.report(e)
                     self.ctx.nodes[name]["state"] = "FAILED"
                     # set child state to FAILED
                     self.set_node_state(
                         self.ctx.connectivity["child_node"][name], "FAILED"
                     )
                     print(f"Node: {name} failed.")
             elif node["metadata"]["node_type"] in ["calcjob", "workchain"]:
                 # process = run_get_node(executor, *args, **kwargs)
                 print("node  type: calcjob/workchain.")
                 kwargs.setdefault("metadata", {})
                 kwargs["metadata"].update({"call_link_label": name})
                 process = self.submit(executor, *args, **kwargs)
                 node["process"] = process
                 self.ctx.nodes[name]["state"] = "RUNNING"
+                self.to_context(process=process)
+            elif node["metadata"]["node_type"] in ["worktree"]:
+                # process = run_get_node(executor, *args, **kwargs)
+                from aiida_worktree.utils import merge_properties
+
+                print("node  type: worktree.")
+                nt = executor(*args, **kwargs)
+                print("group outputs: ", executor.group_outputs)
+                nt.group_outputs = executor.group_outputs
+                nt.name = name
+                ntdata = nt.to_dict()
+                # merge the kwargs
+                merge_properties(ntdata)
+                all = {"nt": ntdata, "metadata": {"call_link_label": name}}
+                print("submit worktree: ")
+                process = self.submit(self.__class__, **all)
+                node["process"] = process
+                # self.ctx.nodes[name]["group_outputs"] = executor.group_outputs
+                self.ctx.nodes[name]["state"] = "RUNNING"
                 return self.to_context(process=process)
             elif node["metadata"]["node_type"] in ["Normal"]:
                 print("node  type: Normal.")
                 # normal function does not have a process
                 if "ctx" in node["metadata"]["kwargs"]:
                     self.ctx.node_name = name
                     kwargs.update({"ctx": self.ctx})
@@ -580,43 +580,54 @@
                 # print("result from node: ", node["results"])
             else:
                 print("node  type: unknown.")
                 # self.report("Unknow node type {}".format(node["metadata"]["node_type"]))
                 return self.exit_codes.UNKNOWN_NODE_TYPE
 
     def get_inputs(self, node):
+        """Get input based on the links."""
         args = []
         kwargs = {}
         properties = node.get("properties", {})
         # TODO: check if input is linked, otherwise use the property value
-        for name in node["metadata"].get("args", {}):
-            has_input_link = False
-            for input in node["inputs"]:
-                if name == input["to_socket"]:
-                    args.append(
-                        self.ctx.nodes[input["from_node"]]["results"][
-                            input["from_socket"]
+        inputs = {}
+        for input in node["inputs"]:
+            # print(f"input: {input['name']}")
+            if len(input["links"]) == 0:
+                inputs[input["name"]] = properties[input["name"]]["value"]
+            elif len(input["links"]) == 1:
+                link = input["links"][0]
+                if self.ctx.nodes[link["from_node"]]["results"] is None:
+                    inputs[input["name"]] = None
+                else:
+                    inputs[input["name"]] = self.ctx.nodes[link["from_node"]][
+                        "results"
+                    ][link["from_socket"]]
+            elif len(input["links"]) > 1:
+                value = {}
+                for link in input["links"]:
+                    name = f'{link["from_node"]}_{link["from_socket"]}'
+                    if self.ctx.nodes[link["from_node"]]["results"] is None:
+                        value[name] = None
+                    else:
+                        value[name] = self.ctx.nodes[link["from_node"]]["results"][
+                            link["from_socket"]
                         ]
-                    )
-                    has_input_link = True
-                    break
-            if not has_input_link and name in properties:
+                inputs[input["name"]] = value
+
+        for name in node["metadata"].get("args", []):
+            if name in inputs:
+                args.append(inputs[name])
+            else:
                 args.append(properties[name]["value"])
-        for name in node["metadata"].get("kwargs", {}):
-            if name in properties:
+        for name in node["metadata"].get("kwargs", []):
+            if name in inputs:
+                kwargs[name] = inputs[name]
+            else:
                 kwargs[name] = properties[name]["value"]
-            for input in node["inputs"]:
-                if name == input["to_socket"]:
-                    # print("input: ", input)
-                    if self.ctx.nodes[input["from_node"]]["results"] is None:
-                        kwargs[name] = None
-                    else:
-                        kwargs[name] = self.ctx.nodes[input["from_node"]]["results"][
-                            input["from_socket"]
-                        ]
         return args, kwargs
 
     def check_node_state(self, name):
         """Check node states.
 
         - if all input nodes finished, launch node
         - if node is a scatter node, check if all scattered nodes finished
@@ -646,36 +657,55 @@
             if input_links.get("Entry", {}):
                 states = [self.ctx.ctrl_links[i]["state"] for i in input_links["Entry"]]
                 if True not in states:
                     ready = False
                     return ready, f"{name}, input entry control link is not FINISHED"
             for input in inputs:
                 # print("    input, ", input["from_node"], self.ctx.nodes[input["from_node"]]["state"])
-                if self.ctx.nodes[input["from_node"]]["state"] not in [
-                    "FINISHED",
-                    "SKIPPED",
-                    "FAILED",
-                ]:
-                    print(
-                        f"    {name}: Input node {input['from_node']}, {self.ctx.nodes[input['from_node']]['state']} ."
-                    )
-                    ready = False
-                    return (
-                        ready,
-                        f"{name}, input: {input['from_node']} is {self.ctx.nodes[input['from_node']]['state']}",
-                    )
+                for link in input["links"]:
+                    if self.ctx.nodes[link["from_node"]]["state"] not in [
+                        "FINISHED",
+                        "SKIPPED",
+                        "FAILED",
+                    ]:
+                        print(
+                            f"    {name}: Input node {link['from_node']}, {self.ctx.nodes[link['from_node']]['state']} ."
+                        )
+                        ready = False
+                        return (
+                            ready,
+                            f"{name}, input: {link['from_node']} is {self.ctx.nodes[link['from_node']]['state']}",
+                        )
         return ready, None
 
+    # def expose_node_group_outputs(self, name):
+    #     # print("expose_node_group_outputs")
+    #     outputs = {}
+    #     process = self.ctx.nodes[name]["process"]
+    #     outgoing = process.base.links.get_outgoing()
+    #     for output in self.ctx.nodes[name]["group_outputs"]:
+    #         node = outgoing.get_node_by_label(output[0])
+    #         outputs[output[2]] = getattr(node.outputs, output[1])
+    #     return outputs
+
     def set_node_state(self, names, value):
         """Set node state"""
         for name in names:
             self.ctx.nodes[name]["state"] = value
 
     def finalize(self):
         """"""
-        self.out("results", self.ctx.results)
+        # expose group outputs
+        group_outputs = {}
+        print("group outputs: ", self.ctx.worktree["metadata"]["group_outputs"])
+        for output in self.ctx.worktree["metadata"]["group_outputs"]:
+            print("output: ", output)
+            group_outputs[output[2]] = self.ctx.nodes[output[0]]["results"][output[1]]
+        self.out("group_outputs", group_outputs)
+        self.out("new_data", self.ctx.new_data)
         self.report("Finalize")
-        print("Finalize")
+        print(f"Finalize worktree {self.ctx.worktree['name']}")
         for name, node in self.ctx.nodes.items():
             if node["state"] == "FAILED":
                 print(f"    Node {name} failed.")
                 return self.exit_codes.NODE_FAILED
+        # check if all nodes are finished with nonzero exit code
```

### Comparing `aiida-worktree-0.0.1/aiida_worktree/nodes/qe.py` & `aiida-worktree-0.0.2/aiida_worktree/nodes/qe.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.1/aiida_worktree/nodes/test.py` & `aiida-worktree-0.0.2/aiida_worktree/nodes/test.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.1/aiida_worktree/properties/built_in.py` & `aiida-worktree-0.0.2/aiida_worktree/properties/built_in.py`

 * *Files identical despite different names*

### Comparing `aiida-worktree-0.0.1/setup.py` & `aiida-worktree-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="aiida-worktree",
-    version="0.0.1",
+    version="0.0.2",
     description="Design flexible node-based workflow for AiiDA calculation.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/superstart54/aiida-worktree",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
@@ -35,14 +35,17 @@
         "cloudpickle",
         "aiida-pseudo",
         "aiida-quantumespresso",
         "pytest",
         "pre-commit",
     ],
     entry_points={
+        "aiida.node": [
+            "process.workflow.worktree = aiida_worktree.orm.worktree:WorkTreeNode",
+        ],
         "scinode_node": [
             "aiida = aiida_worktree.nodes:node_list",
         ],
         "scinode_property": [
             "aiida = aiida_worktree.properties.built_in:property_list",
         ],
     },
```

