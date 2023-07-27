# Comparing `tmp/openvino2onnx-0.1.1.tar.gz` & `tmp/openvino2onnx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvino2onnx-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openvino2onnx-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openvino2onnx-0.1.1.tar` & `openvino2onnx-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        0 2023-07-02 03:33:52.165349 openvino2onnx-0.1.1/.github/words_bag.txt
--rw-r--r--   0        0        0     1279 2023-07-02 08:01:15.072831 openvino2onnx-0.1.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      756 2023-07-02 06:32:19.993506 openvino2onnx-0.1.1/.github/workflows/unittests.yml
--rw-r--r--   0        0        0      112 2023-07-02 03:39:49.201424 openvino2onnx-0.1.1/.gitignore
--rw-r--r--   0        0        0      829 2023-07-02 07:03:14.773393 openvino2onnx-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1098 2023-07-02 03:38:31.602066 openvino2onnx-0.1.1/LICENSE
--rw-r--r--   0        0        0      286 2023-07-02 05:49:32.964854 openvino2onnx-0.1.1/README.md
--rw-r--r--   0        0        0      196 2023-07-02 08:48:52.945705 openvino2onnx-0.1.1/openvino2onnx/__init__.py
--rw-r--r--   0        0        0      167 2023-07-11 04:57:07.412504 openvino2onnx-0.1.1/openvino2onnx/__main__.py
--rw-r--r--   0        0        0     4971 2023-07-02 06:33:32.684644 openvino2onnx-0.1.1/openvino2onnx/builder.py
--rw-r--r--   0        0        0        0 2023-07-02 08:01:15.075833 openvino2onnx-0.1.1/openvino2onnx/cli/__init__.py
--rw-r--r--   0        0        0     1624 2023-07-11 04:57:07.413407 openvino2onnx-0.1.1/openvino2onnx/cli/main_cli.py
--rw-r--r--   0        0        0     1199 2023-07-02 08:01:15.077831 openvino2onnx-0.1.1/openvino2onnx/cli/omz_download.py
--rw-r--r--   0        0        0     4672 2023-07-02 06:07:42.919880 openvino2onnx-0.1.1/openvino2onnx/ir11.py
--rw-r--r--   0        0        0      207 2023-07-01 03:29:57.962412 openvino2onnx-0.1.1/openvino2onnx/legalize/__init__.py
--rw-r--r--   0        0        0      772 2023-07-02 08:01:15.078832 openvino2onnx-0.1.1/openvino2onnx/legalize/compose.py
--rw-r--r--   0        0        0     3257 2023-07-02 08:48:52.946741 openvino2onnx-0.1.1/openvino2onnx/legalize/fold_const.py
--rw-r--r--   0        0        0      602 2023-07-02 06:24:27.231265 openvino2onnx-0.1.1/openvino2onnx/legalize/mutator.py
--rw-r--r--   0        0        0     9202 2023-07-11 04:57:07.415411 openvino2onnx-0.1.1/openvino2onnx/legalize/single_node.py
--rw-r--r--   0        0        0      523 2023-07-02 06:25:38.153144 openvino2onnx-0.1.1/openvino2onnx/legalize/utils.py
--rw-r--r--   0        0        0      930 2023-07-02 06:09:12.801701 openvino2onnx-0.1.1/openvino2onnx/mapping.py
--rw-r--r--   0        0        0     2634 2023-07-02 06:38:00.401629 openvino2onnx-0.1.1/openvino2onnx/ops/__init__.py
--rw-r--r--   0        0        0      207 2023-06-30 10:50:48.931036 openvino2onnx-0.1.1/openvino2onnx/ops/activation.py
--rw-r--r--   0        0        0      394 2023-07-01 07:14:54.978839 openvino2onnx-0.1.1/openvino2onnx/ops/concat.py
--rw-r--r--   0        0        0     1732 2023-06-30 10:53:59.903857 openvino2onnx-0.1.1/openvino2onnx/ops/conv.py
--rw-r--r--   0        0        0     1228 2023-07-02 06:36:28.024510 openvino2onnx-0.1.1/openvino2onnx/ops/convert.py
--rw-r--r--   0        0        0      304 2023-06-30 14:12:38.077664 openvino2onnx-0.1.1/openvino2onnx/ops/element_wise.py
--rw-r--r--   0        0        0      394 2023-07-01 12:02:25.216027 openvino2onnx-0.1.1/openvino2onnx/ops/gather.py
--rw-r--r--   0        0        0     1475 2023-07-01 12:46:28.795270 openvino2onnx-0.1.1/openvino2onnx/ops/interpolate.py
--rw-r--r--   0        0        0     2900 2023-07-11 04:57:07.416409 openvino2onnx-0.1.1/openvino2onnx/ops/pool.py
--rw-r--r--   0        0        0      232 2023-07-11 04:57:07.417414 openvino2onnx-0.1.1/openvino2onnx/ops/strided_slice.py
--rw-r--r--   0        0        0      542 2023-07-02 03:50:06.140057 openvino2onnx-0.1.1/openvino2onnx/ops/transpose.py
--rw-r--r--   0        0        0     1016 2023-07-02 08:01:15.080832 openvino2onnx-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1750 2023-07-02 08:48:52.949708 openvino2onnx-0.1.1/tests/test.py
--rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 openvino2onnx-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-02 03:33:52.165349 openvino2onnx-0.1.2/.github/words_bag.txt
+-rw-r--r--   0        0        0     1279 2023-07-02 08:01:15.072831 openvino2onnx-0.1.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      756 2023-07-02 06:32:19.993506 openvino2onnx-0.1.2/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0      112 2023-07-02 03:39:49.201424 openvino2onnx-0.1.2/.gitignore
+-rw-r--r--   0        0        0      829 2023-07-02 07:03:14.773393 openvino2onnx-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1098 2023-07-02 03:38:31.602066 openvino2onnx-0.1.2/LICENSE
+-rw-r--r--   0        0        0      286 2023-07-02 05:49:32.964854 openvino2onnx-0.1.2/README.md
+-rw-r--r--   0        0        0      187 2023-07-27 13:17:20.225031 openvino2onnx-0.1.2/openvino2onnx/__init__.py
+-rw-r--r--   0        0        0      167 2023-07-11 04:57:07.412504 openvino2onnx-0.1.2/openvino2onnx/__main__.py
+-rw-r--r--   0        0        0     4971 2023-07-02 06:33:32.684644 openvino2onnx-0.1.2/openvino2onnx/builder.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:01:15.075833 openvino2onnx-0.1.2/openvino2onnx/cli/__init__.py
+-rw-r--r--   0        0        0     1624 2023-07-11 04:57:07.413407 openvino2onnx-0.1.2/openvino2onnx/cli/main_cli.py
+-rw-r--r--   0        0        0     1199 2023-07-02 08:01:15.077831 openvino2onnx-0.1.2/openvino2onnx/cli/omz_download.py
+-rw-r--r--   0        0        0     4672 2023-07-02 06:07:42.919880 openvino2onnx-0.1.2/openvino2onnx/ir11.py
+-rw-r--r--   0        0        0      207 2023-07-01 03:29:57.962412 openvino2onnx-0.1.2/openvino2onnx/legalize/__init__.py
+-rw-r--r--   0        0        0      772 2023-07-02 08:01:15.078832 openvino2onnx-0.1.2/openvino2onnx/legalize/compose.py
+-rw-r--r--   0        0        0     3547 2023-07-27 13:16:28.338640 openvino2onnx-0.1.2/openvino2onnx/legalize/fold_const.py
+-rw-r--r--   0        0        0      602 2023-07-02 06:24:27.231265 openvino2onnx-0.1.2/openvino2onnx/legalize/mutator.py
+-rw-r--r--   0        0        0    10208 2023-07-27 13:16:28.339654 openvino2onnx-0.1.2/openvino2onnx/legalize/single_node.py
+-rw-r--r--   0        0        0     1115 2023-07-27 13:16:28.341639 openvino2onnx-0.1.2/openvino2onnx/legalize/utils.py
+-rw-r--r--   0        0        0      930 2023-07-02 06:09:12.801701 openvino2onnx-0.1.2/openvino2onnx/mapping.py
+-rw-r--r--   0        0        0     2634 2023-07-02 06:38:00.401629 openvino2onnx-0.1.2/openvino2onnx/ops/__init__.py
+-rw-r--r--   0        0        0      207 2023-07-27 12:43:32.062742 openvino2onnx-0.1.2/openvino2onnx/ops/activation.py
+-rw-r--r--   0        0        0      394 2023-07-01 07:14:54.978839 openvino2onnx-0.1.2/openvino2onnx/ops/concat.py
+-rw-r--r--   0        0        0     1732 2023-06-30 10:53:59.903857 openvino2onnx-0.1.2/openvino2onnx/ops/conv.py
+-rw-r--r--   0        0        0     1228 2023-07-02 06:36:28.024510 openvino2onnx-0.1.2/openvino2onnx/ops/convert.py
+-rw-r--r--   0        0        0      304 2023-06-30 14:12:38.077664 openvino2onnx-0.1.2/openvino2onnx/ops/element_wise.py
+-rw-r--r--   0        0        0      394 2023-07-01 12:02:25.216027 openvino2onnx-0.1.2/openvino2onnx/ops/gather.py
+-rw-r--r--   0        0        0     1475 2023-07-01 12:46:28.795270 openvino2onnx-0.1.2/openvino2onnx/ops/interpolate.py
+-rw-r--r--   0        0        0     2900 2023-07-11 04:57:07.416409 openvino2onnx-0.1.2/openvino2onnx/ops/pool.py
+-rw-r--r--   0        0        0      232 2023-07-11 04:57:07.417414 openvino2onnx-0.1.2/openvino2onnx/ops/strided_slice.py
+-rw-r--r--   0        0        0      542 2023-07-02 03:50:06.140057 openvino2onnx-0.1.2/openvino2onnx/ops/transpose.py
+-rw-r--r--   0        0        0     1016 2023-07-02 08:01:15.080832 openvino2onnx-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1750 2023-07-02 08:48:52.949708 openvino2onnx-0.1.2/tests/test.py
+-rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 openvino2onnx-0.1.2/PKG-INFO
```

### Comparing `openvino2onnx-0.1.1/.github/workflows/lint.yml` & `openvino2onnx-0.1.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/.github/workflows/unittests.yml` & `openvino2onnx-0.1.2/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/.pre-commit-config.yaml` & `openvino2onnx-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/LICENSE` & `openvino2onnx-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/builder.py` & `openvino2onnx-0.1.2/openvino2onnx/builder.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/cli/main_cli.py` & `openvino2onnx-0.1.2/openvino2onnx/cli/main_cli.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/cli/omz_download.py` & `openvino2onnx-0.1.2/openvino2onnx/cli/omz_download.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/ir11.py` & `openvino2onnx-0.1.2/openvino2onnx/ir11.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/legalize/compose.py` & `openvino2onnx-0.1.2/openvino2onnx/legalize/compose.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/legalize/mutator.py` & `openvino2onnx-0.1.2/openvino2onnx/legalize/mutator.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/legalize/single_node.py` & `openvino2onnx-0.1.2/openvino2onnx/legalize/single_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,254 +1,294 @@
-"""
-Copyright Wenyi Tang 2023
-
-:Author: Wenyi Tang
-:Email: wenyitang@outlook.com
-
-Split IR op to more than 1 onnx op
-"""
-
-import copy
-from contextlib import suppress
-from itertools import product
-
-import networkx as nx
-import numpy as np
-
-from openvino2onnx.mapping import PREC2DTYPE
-
-from .compose import legalize
-from .fold_const import expand_const_on_node, fold_const_on_node
-from .mutator import SingleNodeMutator
-from .utils import get_node_on_edge
-
-
-@legalize.register
-class ShapeOf(SingleNodeMutator):
-    """Change ShapeOf to Const"""
-
-    def __init__(self):
-        super().__init__(pattern="ShapeOf")
-
-    def trans(self, graph: nx.MultiDiGraph, node):
-        attrs = graph.nodes[node]
-        graph.remove_edges_from(list(graph.in_edges(node)))
-        dims = [i["dim"] for i in attrs["inputs"].values()]
-        assert len(dims) == 1
-        dim = list(map(int, dims[0]))
-        output = attrs["outputs"].pop("1")
-        attrs["type"] = "Const"
-        attrs["data"] = np.array(dim, dtype=PREC2DTYPE[output["precision"]])
-        attrs["inputs"].clear()
-        attrs["outputs"]["0"] = output
-
-
-@legalize.register
-class Reshape(SingleNodeMutator):
-    """Calculate reshape accurate shape"""
-
-    def __init__(self):
-        super().__init__(pattern="Reshape")
-
-    def trans(self, graph: nx.MultiDiGraph, node):
-        attrs = graph.nodes[node]
-        # treat 0 as a wildcard to copy from the input on same axis
-        special_zero = attrs["special_zero"]
-        shape_node = get_node_on_edge(graph, node, "1")
-        shape_is_const = False
-        with suppress(Exception):
-            shape = fold_const_on_node(graph, shape_node)
-            shape_is_const = True
-        if shape_is_const:
-            ref_data = np.empty(list(map(int, attrs["inputs"]["0"]["dim"])))
-            if special_zero:
-                for i, d in enumerate(shape):
-                    if d == 0:
-                        shape[i] = ref_data.shape[i]
-            shape = ref_data.reshape(shape).shape
-            attrs["inputs"].pop("1")
-            expand_const_on_node(graph, node, np.array(shape, "int64"), "1")
-
-
-@legalize.register
-class Unsqueeze(SingleNodeMutator):
-    """legalize axes shape"""
-
-    def __init__(self):
-        super().__init__(pattern="Unsqueeze")
-
-    def trans(self, graph: nx.MultiDiGraph, node):
-        attrs = graph.nodes[node]
-        u = get_node_on_edge(graph, node, "1")
-        axes = fold_const_on_node(graph, u)
-        assert axes.ndim == 1
-        attrs["axes"] = axes.flatten()
-        attrs["inputs"].pop("1")
-        expand_const_on_node(graph, node, np.array(attrs["axes"], "int64"), "1")
-
-
-@legalize.register
-class MatMul(SingleNodeMutator):
-    """Split matmul to transpose + matmul"""
-
-    def __init__(self):
-        super().__init__(pattern="MatMul")
-
-    def trans(self, graph: nx.MultiDiGraph, node):
-        attrs = graph.nodes[node]
-        ports = ("a", "0"), ("b", "1")
-        for (u, v, data), (port, order) in product(graph.in_edges(node, True), ports):
-            if attrs[f"transpose_{port}"] == "true" and data["dst"] == order:
-                graph.remove_edge(u, v)
-                output = copy.deepcopy(attrs["inputs"][order])
-                output["dim"] = output["dim"][::-1]
-                output["name"] = "output1"
-                transpose = f"{node}_transpose_{port}"
-                graph.add_node(
-                    transpose,
-                    name=f"{attrs['name']}_transpose_{port}",
-                    type="Transpose",
-                    version="opset1",
-                    inputs={"0": attrs["inputs"][order]},
-                    outputs={"1": output},
-                    perm="1, 0",
-                )
-                graph.add_edge(u, transpose, src=data["src"], dst=order)
-                graph.add_edge(transpose, node, src="1", dst=data["dst"])
-
-
-@legalize.register
-class Transpose(SingleNodeMutator):
-    """Fold const input:1 as attribute perm."""
-
-    def __init__(self):
-        super().__init__(pattern="Transpose")
-
-    def trans(self, graph: nx.MultiDiGraph, node):
-        attrs = graph.nodes[node]
-        if "perm" in attrs:
-            return
-        # find a solo path to input:1
-        u = get_node_on_edge(graph, node, "1")
-        const = fold_const_on_node(graph, u)
-        assert const.ndim == 1
-        attrs["inputs"].pop("1")
-        attrs.update(perm=",".join(map(str, const.tolist())))
-
-
-@legalize.register
-class Gather(SingleNodeMutator):
-    """Evaluate axis to attr"""
-
-    def __init__(self):
-        super().__init__(pattern="Gather")
-
-    def trans(self, graph: nx.MultiDiGraph, node):
-        attrs = graph.nodes[node]
-        u = get_node_on_edge(graph, node, "2")
-        const = fold_const_on_node(graph, u)
-        assert const.size == 1
-        attrs["axis"] = int(const.flatten()[0])
-        attrs["inputs"].pop("2")
-
-
-@legalize.register
-class StridedSlice(SingleNodeMutator):
-    """Swap axes and steps"""
-
-    def __init__(self):
-        super().__init__(pattern="StridedSlice")
-
-    def trans(self, graph: nx.MultiDiGraph, node):
-        attrs = graph.nodes[node]
-        strides = get_node_on_edge(graph, node, "3")
-        steps = fold_const_on_node(graph, strides)
-        assert steps.ndim == 1
-        attrs["inputs"]["3"].update(empty=True)
-        expand_const_on_node(graph, node, steps, "4")
-        begin_mask = list(map(int, attrs["begin_mask"].split(",")))
-        end_mask = list(map(int, attrs["end_mask"].split(",")))
-        if any(i != 0 for i in begin_mask + end_mask):
-            # adjust begin and end
-            begin = get_node_on_edge(graph, node, "1")
-            end = get_node_on_edge(graph, node, "2")
-            data_shape = list(map(int, attrs["inputs"]["0"]["dim"]))
-            begin_var = fold_const_on_node(graph, begin)
-            end_var = fold_const_on_node(graph, end)
-            for i, x in enumerate(begin_mask):
-                begin_var[i] = 0 if x != 0 else begin_var[i]
-            for i, x in enumerate(end_mask):
-                end_var[i] = data_shape[i] if x != 0 else end_var[i]
-            attrs["inputs"].pop("1")
-            attrs["inputs"].pop("2")
-            expand_const_on_node(graph, node, begin_var, "1")
-            expand_const_on_node(graph, node, end_var, "2")
-        if not attrs["shrink_axis_mask"]:
-            shrink_axis_mask = []
-        else:
-            shrink_axis_mask = list(map(int, attrs["shrink_axis_mask"].split(",")))
-        if any(i != 0 for i in shrink_axis_mask):
-            # add a squeeze
-            squeeze_node = f"{node}_squeeze"
-            outport = list(attrs["outputs"].keys())[0]
-            graph.add_node(
-                squeeze_node,
-                name=squeeze_node,
-                type="Squeeze",
-                version="opset1",
-                inputs={"0": attrs["outputs"][outport]},
-                outputs={"2": dict(name=f"{squeeze_node}/output2")},
-            )
-            for u, v, data in list(graph.out_edges(node, True)):
-                graph.add_edge(squeeze_node, v, src="2", dst=data["dst"])
-                graph.remove_edge(u, v)
-            graph.add_edge(node, squeeze_node, src=outport, dst="0")
-            (axis,) = np.nonzero(shrink_axis_mask)
-            expand_const_on_node(graph, squeeze_node, axis, "1")
-            attrs["shrink_axis_mask"] = ""
-
-
-@legalize.register
-class Interpolate(SingleNodeMutator):
-    """To Resize"""
-
-    def __init__(self):
-        super().__init__(pattern="Interpolate")
-
-    def trans(self, graph: nx.MultiDiGraph, node):
-        attrs = graph.nodes[node]
-        # get scales_or_size
-        scales_or_size = get_node_on_edge(graph, node, "1")
-        scales_or_size = fold_const_on_node(graph, scales_or_size)
-        # size to scales
-        input_dims = np.array(list(map(int, attrs["inputs"]["0"]["dim"])))
-        scales = scales_or_size
-        with suppress(ValueError):
-            np.iinfo(scales_or_size.dtype)
-            if scales.size < input_dims.size:
-                scales = np.concatenate(
-                    [input_dims[: input_dims.size - scales.size], scales]
-                )
-            scales = np.true_divide(scales, input_dims).astype("float32")
-        if scales.size < input_dims.size:
-            scales = np.concatenate(
-                [input_dims[: input_dims.size - scales.size], scales]
-            )
-        # make empty roi
-        attrs["inputs"]["1"].update(empty=True)
-        # make scales
-        expand_const_on_node(graph, node, scales, "2")
-
-
-@legalize.register
-class Squeeze(SingleNodeMutator):
-    """Cast axis from U64 to I64"""
-
-    def __init__(self):
-        super().__init__(pattern="Squeeze")
-
-    def trans(self, graph: nx.MultiDiGraph, node):
-        attrs = graph.nodes[node]
-        axis = get_node_on_edge(graph, node, "1")
-        axis_var = fold_const_on_node(graph, axis)
-        attrs["inputs"].pop("1")
-        expand_const_on_node(graph, node, axis_var.astype("int64"), "1")
+"""
+Copyright Wenyi Tang 2023
+
+:Author: Wenyi Tang
+:Email: wenyitang@outlook.com
+
+Split IR op to more than 1 onnx op
+"""
+
+import copy
+from contextlib import suppress
+from itertools import product
+
+import networkx as nx
+import numpy as np
+
+from openvino2onnx.mapping import PREC2DTYPE
+
+from .compose import legalize
+from .fold_const import expand_const_on_node, fold_const_on_node
+from .mutator import SingleNodeMutator
+
+
+@legalize.register
+class ShapeOf(SingleNodeMutator):
+    """Change ShapeOf to Const"""
+
+    def __init__(self):
+        super().__init__(pattern="ShapeOf")
+
+    def trans(self, graph: nx.MultiDiGraph, node):
+        attrs = graph.nodes[node]
+        graph.remove_edges_from(list(graph.in_edges(node)))
+        dims = [i["dim"] for i in attrs["inputs"].values()]
+        assert len(dims) == 1
+        dim = list(map(int, dims[0]))
+        output = attrs["outputs"].pop("1")
+        attrs["type"] = "Const"
+        attrs["data"] = np.array(dim, dtype=PREC2DTYPE[output["precision"]])
+        attrs["inputs"].clear()
+        attrs["outputs"]["0"] = output
+
+
+@legalize.register
+class Reshape(SingleNodeMutator):
+    """Calculate reshape accurate shape"""
+
+    def __init__(self):
+        super().__init__(pattern="Reshape")
+
+    def trans(self, graph: nx.MultiDiGraph, node):
+        attrs = graph.nodes[node]
+        # treat 0 as a wildcard to copy from the input on same axis
+        special_zero = attrs["special_zero"]
+        shape_is_const = False
+        with suppress(Exception):
+            shape = fold_const_on_node(graph, node, "1")
+            shape_is_const = True
+        if shape_is_const:
+            ref_data = np.empty(list(map(int, attrs["inputs"]["0"]["dim"])))
+            if special_zero:
+                for i, d in enumerate(shape):
+                    if d == 0:
+                        shape[i] = ref_data.shape[i]
+            shape = ref_data.reshape(shape).shape
+            attrs["inputs"].pop("1")
+            expand_const_on_node(graph, node, np.array(shape, "int64"), "1")
+
+
+@legalize.register
+class Unsqueeze(SingleNodeMutator):
+    """legalize axes shape"""
+
+    def __init__(self):
+        super().__init__(pattern="Unsqueeze")
+
+    def trans(self, graph: nx.MultiDiGraph, node):
+        attrs = graph.nodes[node]
+        axes = fold_const_on_node(graph, node, "1")
+        assert axes.ndim == 1
+        attrs["axes"] = axes.flatten()
+        attrs["inputs"].pop("1")
+        expand_const_on_node(graph, node, np.array(attrs["axes"], "int64"), "1")
+
+
+@legalize.register
+class MatMul(SingleNodeMutator):
+    """Split matmul to transpose + matmul"""
+
+    def __init__(self):
+        super().__init__(pattern="MatMul")
+
+    def trans(self, graph: nx.MultiDiGraph, node):
+        attrs = graph.nodes[node]
+        ports = ("a", "0"), ("b", "1")
+        for (u, v, data), (port, order) in product(graph.in_edges(node, True), ports):
+            if attrs[f"transpose_{port}"] == "true" and data["dst"] == order:
+                graph.remove_edge(u, v)
+                output = copy.deepcopy(attrs["inputs"][order])
+                output["dim"] = output["dim"][::-1]
+                output["name"] = "output1"
+                transpose = f"{node}_transpose_{port}"
+                graph.add_node(
+                    transpose,
+                    name=f"{attrs['name']}_transpose_{port}",
+                    type="Transpose",
+                    version="opset1",
+                    inputs={"0": attrs["inputs"][order]},
+                    outputs={"1": output},
+                    perm="1, 0",
+                )
+                graph.add_edge(u, transpose, src=data["src"], dst=order)
+                graph.add_edge(transpose, node, src="1", dst=data["dst"])
+
+
+@legalize.register
+class Transpose(SingleNodeMutator):
+    """Fold const input:1 as attribute perm."""
+
+    def __init__(self):
+        super().__init__(pattern="Transpose")
+
+    def trans(self, graph: nx.MultiDiGraph, node):
+        attrs = graph.nodes[node]
+        if "perm" in attrs:
+            return
+        # find a solo path to input:1
+        const = fold_const_on_node(graph, node, "1")
+        assert const.ndim == 1
+        attrs["inputs"].pop("1")
+        attrs.update(perm=",".join(map(str, const.tolist())))
+
+
+@legalize.register
+class Gather(SingleNodeMutator):
+    """Evaluate axis to attr"""
+
+    def __init__(self):
+        super().__init__(pattern="Gather")
+
+    def trans(self, graph: nx.MultiDiGraph, node):
+        attrs = graph.nodes[node]
+        const = fold_const_on_node(graph, node, "2")
+        assert const.size == 1
+        attrs["axis"] = int(const.flatten()[0])
+        attrs["inputs"].pop("2")
+
+
+@legalize.register
+class StridedSlice(SingleNodeMutator):
+    """Swap axes and steps"""
+
+    def __init__(self):
+        super().__init__(pattern="StridedSlice")
+
+    def trans(self, graph: nx.MultiDiGraph, node):
+        attrs = graph.nodes[node]
+        steps = fold_const_on_node(graph, node, "3")
+        assert steps.ndim == 1
+        attrs["inputs"]["3"].update(empty=True)
+        expand_const_on_node(graph, node, steps, "4")
+        begin_mask = list(map(int, attrs["begin_mask"].split(",")))
+        end_mask = list(map(int, attrs["end_mask"].split(",")))
+        if any(i != 0 for i in begin_mask + end_mask):
+            # adjust begin and end
+            data_shape = list(map(int, attrs["inputs"]["0"]["dim"]))
+            begin_var = fold_const_on_node(graph, node, "1")
+            end_var = fold_const_on_node(graph, node, "2")
+            for i, x in enumerate(begin_mask):
+                begin_var[i] = 0 if x != 0 else begin_var[i]
+            for i, x in enumerate(end_mask):
+                end_var[i] = data_shape[i] if x != 0 else end_var[i]
+            attrs["inputs"].pop("1")
+            attrs["inputs"].pop("2")
+            expand_const_on_node(graph, node, begin_var, "1")
+            expand_const_on_node(graph, node, end_var, "2")
+        if not attrs["shrink_axis_mask"]:
+            shrink_axis_mask = []
+        else:
+            shrink_axis_mask = list(map(int, attrs["shrink_axis_mask"].split(",")))
+        if any(i != 0 for i in shrink_axis_mask):
+            # add a squeeze
+            squeeze_node = f"{node}_squeeze"
+            outport = list(attrs["outputs"].keys())[0]
+            graph.add_node(
+                squeeze_node,
+                name=squeeze_node,
+                type="Squeeze",
+                version="opset1",
+                inputs={"0": attrs["outputs"][outport]},
+                outputs={"2": dict(name=f"{squeeze_node}/output2")},
+            )
+            for u, v, data in list(graph.out_edges(node, True)):
+                graph.add_edge(squeeze_node, v, src="2", dst=data["dst"])
+                graph.remove_edge(u, v)
+            graph.add_edge(node, squeeze_node, src=outport, dst="0")
+            (axis,) = np.nonzero(shrink_axis_mask)
+            expand_const_on_node(graph, squeeze_node, axis, "1")
+            attrs["shrink_axis_mask"] = ""
+
+
+@legalize.register
+class Interpolate(SingleNodeMutator):
+    """To Resize"""
+
+    def __init__(self):
+        super().__init__(pattern="Interpolate")
+
+    def trans(self, graph: nx.MultiDiGraph, node):
+        attrs = graph.nodes[node]
+        # get scales_or_size
+        scales_or_size = fold_const_on_node(graph, node, "1")
+        # size to scales
+        input_dims = np.array(list(map(int, attrs["inputs"]["0"]["dim"])))
+        scales = scales_or_size
+        with suppress(ValueError):
+            np.iinfo(scales_or_size.dtype)
+            if scales.size < input_dims.size:
+                scales = np.concatenate(
+                    [input_dims[: input_dims.size - scales.size], scales]
+                )
+            scales = np.true_divide(scales, input_dims).astype("float32")
+        if scales.size < input_dims.size:
+            scales = np.concatenate(
+                [input_dims[: input_dims.size - scales.size], scales]
+            )
+        # make empty roi
+        attrs["inputs"]["1"].update(empty=True)
+        # make scales
+        expand_const_on_node(graph, node, scales, "2")
+
+
+@legalize.register
+class Squeeze(SingleNodeMutator):
+    """Cast axis from U64 to I64"""
+
+    def __init__(self):
+        super().__init__(pattern="Squeeze")
+
+    def trans(self, graph: nx.MultiDiGraph, node):
+        attrs = graph.nodes[node]
+        axis_var = fold_const_on_node(graph, node, "1")
+        attrs["inputs"].pop("1")
+        expand_const_on_node(graph, node, axis_var.astype("int64"), "1")
+
+
+@legalize.register
+class Swish(SingleNodeMutator):
+    """Change swish to mul and sigmoid.
+
+    Swish(x) = x * sigmoid(x)
+    """
+
+    def __init__(self):
+        super().__init__(pattern="Swish")
+
+    def trans(self, graph: nx.MultiDiGraph, node):
+        attrs = graph.nodes[node]
+        preds = {k: graph[k][node] for k in graph.predecessors(node)}
+        succs = {k: graph[node][k] for k in graph.successors(node)}
+        # remove swish
+        graph.remove_node(node)
+        # add sigmoid
+        sigmoid_node = f"{node}_sigmoid"
+        graph.add_node(
+            sigmoid_node,
+            name=sigmoid_node,
+            type="Sigmoid",
+            version="opset1",
+            inputs=copy.deepcopy(attrs["inputs"]),
+            outputs=copy.deepcopy(attrs["outputs"]),
+        )
+        # add mul
+        mul_node = f"{node}_mul"
+        graph.add_node(
+            mul_node,
+            name=mul_node,
+            type="Multiply",
+            version="opset1",
+            inputs=copy.deepcopy(attrs["inputs"]),
+            outputs=copy.deepcopy(attrs["outputs"]),
+        )
+        mul_attrs = graph.nodes[mul_node]
+        mul_attrs["inputs"]["1"] = mul_attrs["inputs"]["0"]
+        mul_attrs["inputs"]["1"].update(id=1)
+        mul_attrs["outputs"]["2"] = mul_attrs["outputs"].pop("1")
+        mul_attrs["outputs"]["2"].update(id=2, name="output2")
+        # add edges back
+        graph.add_edge(sigmoid_node, mul_node, src="1", dst="1")
+        for i in preds:
+            graph.add_edge(i, sigmoid_node, src=preds[i][0]["src"], dst="0")
+            graph.add_edge(i, mul_node, src=preds[i][0]["src"], dst="0")
+        for i in succs:
+            graph.add_edge(mul_node, i, src="2", dst=succs[i][0]["dst"])
```

### Comparing `openvino2onnx-0.1.1/openvino2onnx/mapping.py` & `openvino2onnx-0.1.2/openvino2onnx/mapping.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/ops/__init__.py` & `openvino2onnx-0.1.2/openvino2onnx/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/ops/conv.py` & `openvino2onnx-0.1.2/openvino2onnx/ops/conv.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/ops/convert.py` & `openvino2onnx-0.1.2/openvino2onnx/ops/convert.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/ops/interpolate.py` & `openvino2onnx-0.1.2/openvino2onnx/ops/interpolate.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/ops/pool.py` & `openvino2onnx-0.1.2/openvino2onnx/ops/pool.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/openvino2onnx/ops/transpose.py` & `openvino2onnx-0.1.2/openvino2onnx/ops/transpose.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/pyproject.toml` & `openvino2onnx-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/tests/test.py` & `openvino2onnx-0.1.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `openvino2onnx-0.1.1/PKG-INFO` & `openvino2onnx-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openvino2onnx
-Version: 0.1.1
+Version: 0.1.2
 Summary: openvino2onnx is a tool to convert openvino IR format to ONNX.
 Author-email: Wenyi Tang <wenyitang@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: onnx >= 1.8.1
 Requires-Dist: networkx
```

