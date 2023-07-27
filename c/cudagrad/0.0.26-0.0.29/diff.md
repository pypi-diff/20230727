# Comparing `tmp/cudagrad-0.0.26.tar.gz` & `tmp/cudagrad-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.26.tar", last modified: Thu Jul 27 00:54:49 2023, max compression
+gzip compressed data, was "cudagrad-0.0.29.tar", last modified: Thu Jul 27 02:34:01 2023, max compression
```

## Comparing `cudagrad-0.0.26.tar` & `cudagrad-0.0.29.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 00:54:49.608209 cudagrad-0.0.26/
--rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.26/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-27 00:54:49.608009 cudagrad-0.0.26/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3170 2023-07-25 01:40:28.000000 cudagrad-0.0.26/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 00:54:49.605754 cudagrad-0.0.26/cudagrad/
--rw-r--r--   0 ryan       (501) staff       (20)       81 2023-07-27 00:50:13.000000 cudagrad-0.0.26/cudagrad/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     5187 2023-07-27 00:16:07.000000 cudagrad-0.0.26/cudagrad/mlp.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 00:54:49.606770 cudagrad-0.0.26/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-27 00:54:49.000000 cudagrad-0.0.26/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      331 2023-07-27 00:54:49.000000 cudagrad-0.0.26/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:54:49.000000 cudagrad-0.0.26/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.26/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       15 2023-07-27 00:54:49.000000 cudagrad-0.0.26/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-27 00:54:49.000000 cudagrad-0.0.26/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)      693 2023-07-27 00:29:37.000000 cudagrad-0.0.26/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-27 00:54:49.608281 cudagrad-0.0.26/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1659 2023-07-27 00:49:51.000000 cudagrad-0.0.26/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 00:54:49.607409 cudagrad-0.0.26/src/
--rw-r--r--   0 ryan       (501) staff       (20)     2944 2023-07-27 00:52:48.000000 cudagrad-0.0.26/src/bindings.cpp
--rw-r--r--   0 ryan       (501) staff       (20)    20537 2023-07-26 04:09:23.000000 cudagrad-0.0.26/src/cudagrad.hpp
--rw-r--r--   0 ryan       (501) staff       (20)      263 2023-07-26 03:31:20.000000 cudagrad-0.0.26/src/ops.cu
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 00:54:49.607739 cudagrad-0.0.26/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1078 2023-07-27 00:15:15.000000 cudagrad-0.0.26/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 02:34:01.290053 cudagrad-0.0.29/
+-rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.29/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-27 02:34:01.289933 cudagrad-0.0.29/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     3170 2023-07-25 01:40:28.000000 cudagrad-0.0.29/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 02:34:01.287444 cudagrad-0.0.29/cudagrad/
+-rw-r--r--   0 ryan       (501) staff       (20)      105 2023-07-27 00:57:57.000000 cudagrad-0.0.29/cudagrad/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5571 2023-07-27 02:29:43.000000 cudagrad-0.0.29/cudagrad/mlp.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 02:34:01.288484 cudagrad-0.0.29/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-27 02:34:01.000000 cudagrad-0.0.29/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      331 2023-07-27 02:34:01.000000 cudagrad-0.0.29/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 02:34:01.000000 cudagrad-0.0.29/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.29/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-27 02:34:01.000000 cudagrad-0.0.29/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-27 02:34:01.000000 cudagrad-0.0.29/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      754 2023-07-27 02:32:02.000000 cudagrad-0.0.29/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-27 02:34:01.290094 cudagrad-0.0.29/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1659 2023-07-27 00:49:51.000000 cudagrad-0.0.29/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 02:34:01.289293 cudagrad-0.0.29/src/
+-rw-r--r--   0 ryan       (501) staff       (20)     2944 2023-07-27 00:52:48.000000 cudagrad-0.0.29/src/bindings.cpp
+-rw-r--r--   0 ryan       (501) staff       (20)    20537 2023-07-26 04:09:23.000000 cudagrad-0.0.29/src/cudagrad.hpp
+-rw-r--r--   0 ryan       (501) staff       (20)      263 2023-07-26 03:31:20.000000 cudagrad-0.0.29/src/ops.cu
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-27 02:34:01.289626 cudagrad-0.0.29/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)     1078 2023-07-27 00:15:15.000000 cudagrad-0.0.29/tests/test.py
```

### Comparing `cudagrad-0.0.26/PKG-INFO` & `cudagrad-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.26
+Version: 0.0.29
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cudagrad-0.0.26/README.md` & `cudagrad-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.26/cudagrad/mlp.py` & `cudagrad-0.0.29/cudagrad/mlp.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,197 +2,201 @@
 # %%
 import random
 from typing import *  # type: ignore
 
 import matplotlib.pyplot as plt
 import numpy as np
 
+from .cudagrad_bindings import *  # type: ignore
+
 # %matplotlib inline
 
 np.random.seed(1337)
 random.seed(1337)
-# %%
+
 from micrograd.engine import Value
 from micrograd.nn import MLP, Layer, Neuron
 
 # %%
-n = MLP(3, [1, 1])
-m = MLP(3, [2, 1])
-n, m
+if __name__ == "__main__":
+  # %%
+  n = MLP(3, [1, 1])
+  m = MLP(3, [2, 1])
+  n, m
 
 
-# %%
-class _:  # MLP
+  # %%
+  class _:  # MLP
     from typing import List
 
     def __init__(self, nin: int, nouts: List[int]):
-        sz = [nin] + nouts
-        self.layers = [
-            Layer(sz[i], sz[i + 1], nonlin=i != len(nouts) - 1)
-            for i in range(len(nouts))
-        ]
-
-
-# MLP CONSTRUCTOR
-# this is straightforward right, we make layers of
-# cin, cout combos but we only make #cout of them
-# each layers takes nin starting with nin, but then
-# all other layers take the nouts[i] of the previous
-
-# LINEAR OUTPUT
-# the last layers is linear so we can predict any number not just [0,int)
-
-# RELU LAYERS
-# ReLU (Rectified Linear Unit) introduces non-linearity into neural networks
-# due to its non-linear nature. The ReLU function is defined as:
-#
-# f(x) = max(0, x)
-#
-# without relus (or any non linear activation) nn's would be linear funtions
-
-
-#  By definition, the ReLU is 𝑚𝑎𝑥(0,𝑥). Therefore, if we split the domain from
-# (−∞,0] or [0,∞), then the function is linear. However, it's easy to see
-# that 𝑓(−1)+𝑓(1)≠𝑓(0). Hence, by definition, ReLU is not linear.
-# https://datascience.stackexchange.com/a/26481
-# %%
-def internals(n: MLP) -> None:
+      sz = [nin] + nouts
+      self.layers = [
+        Layer(sz[i], sz[i + 1], nonlin=i != len(nouts) - 1)
+        for i in range(len(nouts))
+      ]
+
+
+  # MLP CONSTRUCTOR
+  # this is straightforward right, we make layers of
+  # cin, cout combos but we only make #cout of them
+  # each layers takes nin starting with nin, but then
+  # all other layers take the nouts[i] of the previous
+
+  # LINEAR OUTPUT
+  # the last layers is linear so we can predict any number not just [0,int)
+
+  # RELU LAYERS
+  # ReLU (Rectified Linear Unit) introduces non-linearity into neural networks
+  # due to its non-linear nature. The ReLU function is defined as:
+  #
+  # f(x) = max(0, x)
+  #
+  # without relus (or any non linear activation) nn's would be linear funtions
+
+
+  #  By definition, the ReLU is 𝑚𝑎𝑥(0,𝑥). Therefore, if we split the domain from
+  # (−∞,0] or [0,∞), then the function is linear. However, it's easy to see
+  # that 𝑓(−1)+𝑓(1)≠𝑓(0). Hence, by definition, ReLU is not linear.
+  # https://datascience.stackexchange.com/a/26481
+  # %%
+  def internals(n: MLP) -> None:
     for layer in n.layers:
-        print(layer, "---")
-        for neuron in layer.neurons:
-            print(neuron, "*")
-            for value in neuron.parameters():  # .w and [.b]
-                print(value, ".")
-
-
-# %%
-
-internals(n)
-# MLP Diagram:
-#
-#   Input (3 features)
-#       ↓
-# Layer 1 (ReLUNeuron) # w: [0.2, 0.1, 0.3], b: 0.0
-#       ↓
-# Layer 2 (LinearNeuron) # w: [0.2], b: 0.0
-#       ↓
-#  Output (1 output)
+      print(layer, "---")
+      for neuron in layer.neurons:
+        print(neuron, "*")
+        for value in neuron.parameters():  # .w and [.b]
+          print(value, ".")
+
+
+  # %%
+
+  internals(n)
+  # MLP Diagram:
+  #
+  #   Input (3 features)
+  #       ↓
+  # Layer 1 (ReLUNeuron) # w: [0.2, 0.1, 0.3], b: 0.0
+  #       ↓
+  # Layer 2 (LinearNeuron) # w: [0.2], b: 0.0
+  #       ↓
+  #  Output (1 output)
+
+  # %%
+  internals(m)
+  # here's why this makes sense
+  # you take three inputs, every neuron needs 3 weights plus a bias
+  # but the number outputs of the first layer is two
+  # so you need two neurons in the first layer
+  # the linear layer gives two inputs and thus has two weights
+  # %%
+
+  xs = [[2.0, 3.0, -1.0], [3.0, -1.0, 0.5], [0.5, 1.0, 1.0], [1.0, 1.0, -1.0]]
+  ys = [1.0, -1.0, -1.0, 1.0]
+  # %%
 
-# %%
-internals(m)
-# here's why this makes sense
-# you take three inputs, every neuron needs 3 weights plus a bias
-# but the number outputs of the first layer is two
-# so you need two neurons in the first layer
-# the linear layer gives two inputs and thus has two weights
-# %%
-
-xs = [[2.0, 3.0, -1.0], [3.0, -1.0, 0.5], [0.5, 1.0, 1.0], [1.0, 1.0, -1.0]]
-ys = [1.0, -1.0, -1.0, 1.0]
-# %%
-
-nn = MLP(3, [4, 4, 1])  # i think this ignores our random seed sadly
-for _ in range(50):
+  nn = MLP(3, [4, 4, 1])  # i think this ignores our random seed sadly
+  for _ in range(50):
     ypred = [nn(x) for x in xs]
     loss = sum((a - b) ** 2 for a, b in zip(ypred, ys))
     for p in nn.parameters():
-        p.grad = 0.0
+      p.grad = 0.0
     loss.backward()
     for p in nn.parameters():
-        p.data += -0.05 * p.grad
+      p.data += -0.05 * p.grad
     print(_ + 1, loss.data, [f"{x.data:1.2f}" for x in ypred])
-# %%
-
-import random
-
-import cudagrad
-from cudagrad import Tensor, tensor
+  # %%
 
+  import random
 
-class Module:
-    def zero_grad(self):
-        for p in self.parameters():
-            p.grad = 0
-
-    def parameters(self):
-        return []
-
-
-class Neuron(Module):
-    def __init__(self, nin, nonlin=True):
-        self.w = [tensor([1], [random.uniform(-1, 1)]) for _ in range(nin)]
-        self.b = tensor([1], [0])
-        self.nonlin = nonlin
-
-    def __call__(self, x):
-        ans = tensor([1], [0])
-        for elem_x in x:
-            for elem_w in self.w:
-                if type(elem_x) != Tensor:
-                    elem_x = tensor([1], [elem_x])
-                ans = ans + (elem_w * elem_x)
-        ans = ans + self.b
-        return ans
-        # act = sum((wi*xi for wi,xi in zip(self.w, x)), self.b)
-        # return act.relu() if self.nonlin else act
+  # import cudagrad
+  # from cudagrad import Tensor, tensor
 
-    def parameters(self):
-        return self.w + [self.b]
 
-    def __repr__(self):
-        return f"{'ReLU' if self.nonlin else 'Linear'}Neuron({len(self.w)})"
-
-
-# %%
-print(Neuron(2)([0.5, 0.2]).data)
-print(Neuron(2)([tensor([1], [0.5]), tensor([1], [0.2])]).data)
-# Layer(1, 2)
-# MLP(2, [2, 1])
-
-
-# %%
-class Layer(Module):
-    def __init__(self, nin, nout, **kwargs):
-        self.neurons = [Neuron(nin, **kwargs) for _ in range(nout)]
-
-    def __call__(self, x):
-        out = [n(x) for n in self.neurons]
-        return out[0] if len(out) == 1 else out
-
-    def parameters(self):
-        return [p for n in self.neurons for p in n.parameters()]
-
-    def __repr__(self):
-        return f"Layer of [{', '.join(str(n) for n in self.neurons)}]"
-
-
-class MLP(Module):
-    def __init__(self, nin, nouts):
-        sz = [nin] + nouts
-        self.layers = [
-            Layer(sz[i], sz[i + 1], nonlin=i != len(nouts) - 1)
-            for i in range(len(nouts))
-        ]
-
-    def __call__(self, x):
-        for layer in self.layers:
-            x = layer(x)
-        return x
-
-    def parameters(self):
-        return [p for layer in self.layers for p in layer.parameters()]
-
-    def __repr__(self):
-        return f"MLP of [{', '.join(str(layer) for layer in self.layers)}]"
-
-
-# %%
-nn = MLP(3, [4, 4, 1])  # i think this ignores our random seed sadly
-for _ in range(50):
-    ypred = [nn(x) for x in xs]
-    loss = sum((a - b) ** 2 for a, b in zip(ypred, ys))
-    for p in nn.parameters():
-        p.grad = 0.0
-    loss.backward()
-    for p in nn.parameters():
-        p.data += -0.05 * p.grad
-    print(_ + 1, loss.data, [f"{x.data:1.2f}" for x in ypred])
+  class Module:
+      def zero_grad(self):
+          for p in self.parameters():
+              p.grad = 0
+
+      def parameters(self):
+          return []
+
+
+  class Neuron(Module):
+      def __init__(self, nin, nonlin=True):
+          self.w = [tensor([1], [random.uniform(-1, 1)]) for _ in range(nin)]
+          self.b = tensor([1], [0])
+          self.nonlin = nonlin
+
+      def __call__(self, x):
+          ans = tensor([1], [0])
+          for elem_x in x:
+              for elem_w in self.w:
+                  if type(elem_x) != Tensor:
+                      elem_x = tensor([1], [elem_x])
+                  ans = ans + (elem_w * elem_x)
+          ans = ans + self.b
+          return ans
+          # act = sum((wi*xi for wi,xi in zip(self.w, x)), self.b)
+          # return act.relu() if self.nonlin else act
+
+      def parameters(self):
+          return self.w + [self.b]
+
+      def __repr__(self):
+          return f"{'ReLU' if self.nonlin else 'Linear'}Neuron({len(self.w)})"
+
+
+  # %%
+  print(Neuron(2)([0.5, 0.2]).data)
+  print(Neuron(2)([tensor([1], [0.5]), tensor([1], [0.2])]).data)
+  # Layer(1, 2)
+  # MLP(2, [2, 1])
+
+
+  # # %%
+  # class Layer(Module):
+  #     def __init__(self, nin, nout, **kwargs):
+  #         self.neurons = [Neuron(nin, **kwargs) for _ in range(nout)]
+
+  #     def __call__(self, x):
+  #         out = [n(x) for n in self.neurons]
+  #         return out[0] if len(out) == 1 else out
+
+  #     def parameters(self):
+  #         return [p for n in self.neurons for p in n.parameters()]
+
+  #     def __repr__(self):
+  #         return f"Layer of [{', '.join(str(n) for n in self.neurons)}]"
+
+
+  # class MLP(Module):
+  #     def __init__(self, nin, nouts):
+  #         sz = [nin] + nouts
+  #         self.layers = [
+  #             Layer(sz[i], sz[i + 1], nonlin=i != len(nouts) - 1)
+  #             for i in range(len(nouts))
+  #         ]
+
+  #     def __call__(self, x):
+  #         for layer in self.layers:
+  #             x = layer(x)
+  #         return x
+
+  #     def parameters(self):
+  #         return [p for layer in self.layers for p in layer.parameters()]
+
+  #     def __repr__(self):
+  #         return f"MLP of [{', '.join(str(layer) for layer in self.layers)}]"
+
+
+  # # %%
+  # # nn = MLP(3, [4, 4, 1])  # i think this ignores our random seed sadly
+  # # for _ in range(50):
+  # #     ypred = [nn(x) for x in xs]
+  # #     loss = sum((a - b) ** 2 for a, b in zip(ypred, ys))
+  # #     for p in nn.parameters():
+  # #         p.grad = 0.0
+  # #     loss.backward()
+  # #     for p in nn.parameters():
+  # #         p.data += -0.05 * p.grad
+  # #     print(_ + 1, loss.data, [f"{x.data:1.2f}" for x in ypred])
```

### Comparing `cudagrad-0.0.26/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.29/cudagrad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.26
+Version: 0.0.29
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cudagrad-0.0.26/pyproject.toml` & `cudagrad-0.0.29/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [build-system]
 requires = [ "setuptools>=40.8.0", "wheel", "pybind11>=2.10.1", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.26"
+version = "0.0.29"
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
+# TEMP while we implement mlp
+dependencies = [ "micrograd",]
 [[project.authors]]
 name = "Ryan Moore"
 email = "moorethreads@hey.com"
 
 [project.urls]
 Homepage = "https://github.com/yrom1/cudagrad"
 "Bug Tracker" = "https://github.com/yrom1/cudagrad/issues"
```

### Comparing `cudagrad-0.0.26/setup.py` & `cudagrad-0.0.29/setup.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.26/src/bindings.cpp` & `cudagrad-0.0.29/src/bindings.cpp`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.26/src/cudagrad.hpp` & `cudagrad-0.0.29/src/cudagrad.hpp`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.26/tests/test.py` & `cudagrad-0.0.29/tests/test.py`

 * *Files identical despite different names*

