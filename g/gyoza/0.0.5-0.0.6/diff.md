# Comparing `tmp/gyoza-0.0.5.tar.gz` & `tmp/gyoza-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyoza-0.0.5.tar", last modified: Tue Jun 13 06:53:11 2023, max compression
+gzip compressed data, was "gyoza-0.0.6.tar", last modified: Thu Jul 27 14:26:36 2023, max compression
```

## Comparing `gyoza-0.0.5.tar` & `gyoza-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.191642 gyoza-0.0.5/
--rwxrwxrwx   0 timdick    (501) staff       (20)     1091 2023-06-02 09:45:10.000000 gyoza-0.0.5/LICENSE
--rw-r--r--   0 timdick    (501) staff       (20)      767 2023-06-13 06:53:11.191391 gyoza-0.0.5/PKG-INFO
--rwxr-xr-x   0 timdick    (501) staff       (20)      251 2023-06-11 16:18:38.000000 gyoza-0.0.5/README.md
--rwxr-xr-x   0 timdick    (501) staff       (20)      854 2023-06-13 06:52:52.000000 gyoza-0.0.5/pyproject.toml
--rw-r--r--   0 timdick    (501) staff       (20)       38 2023-06-13 06:53:11.191722 gyoza-0.0.5/setup.cfg
--rwxrwxrwx   0 timdick    (501) staff       (20)      173 2023-06-02 11:51:40.000000 gyoza-0.0.5/setup.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.184231 gyoza-0.0.5/src/
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.186305 gyoza-0.0.5/src/gyoza/
--rw-r--r--   0 timdick    (501) staff       (20)        0 2023-06-07 09:58:20.000000 gyoza-0.0.5/src/gyoza/__init__.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.189454 gyoza-0.0.5/src/gyoza/modelling/
--rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 11:33:16.000000 gyoza-0.0.5/src/gyoza/modelling/__init__.py
--rwxr-xr-x   0 timdick    (501) staff       (20)    19977 2023-06-11 16:18:38.000000 gyoza-0.0.5/src/gyoza/modelling/flow_layers.py
--rw-r--r--   0 timdick    (501) staff       (20)        0 2023-06-11 16:18:38.000000 gyoza-0.0.5/src/gyoza/modelling/losses.py
--rw-r--r--   0 timdick    (501) staff       (20)     9717 2023-06-11 16:18:38.000000 gyoza-0.0.5/src/gyoza/modelling/masks.py
--rw-r--r--   0 timdick    (501) staff       (20)     3396 2023-06-11 16:18:38.000000 gyoza-0.0.5/src/gyoza/modelling/standard_layers.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.189722 gyoza-0.0.5/src/gyoza/scripts/
--rwxr-xr-x   0 timdick    (501) staff       (20)      160 2023-06-13 06:44:04.000000 gyoza-0.0.5/src/gyoza/scripts/demo.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.190950 gyoza-0.0.5/src/gyoza/utilities/
--rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 12:24:09.000000 gyoza-0.0.5/src/gyoza/utilities/__init__.py
--rwxrwxrwx   0 timdick    (501) staff       (20)       40 2023-06-02 12:29:06.000000 gyoza-0.0.5/src/gyoza/utilities/file_management.py
--rwxrwxrwx   0 timdick    (501) staff       (20)     1064 2023-06-02 12:38:46.000000 gyoza-0.0.5/src/gyoza/utilities/math.py
--rw-r--r--   0 timdick    (501) staff       (20)     3746 2023-06-13 06:39:04.000000 gyoza-0.0.5/src/gyoza/utilities/tensors.py
-drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-06-13 06:53:11.187980 gyoza-0.0.5/src/gyoza.egg-info/
--rwxrwxrwx   0 timdick    (501) staff       (20)      767 2023-06-13 06:53:11.000000 gyoza-0.0.5/src/gyoza.egg-info/PKG-INFO
--rwxrwxrwx   0 timdick    (501) staff       (20)      548 2023-06-13 06:53:11.000000 gyoza-0.0.5/src/gyoza.egg-info/SOURCES.txt
--rwxrwxrwx   0 timdick    (501) staff       (20)        1 2023-06-13 06:53:11.000000 gyoza-0.0.5/src/gyoza.egg-info/dependency_links.txt
--rwxrwxrwx   0 timdick    (501) staff       (20)      100 2023-06-13 06:53:11.000000 gyoza-0.0.5/src/gyoza.egg-info/requires.txt
--rwxrwxrwx   0 timdick    (501) staff       (20)        6 2023-06-13 06:53:11.000000 gyoza-0.0.5/src/gyoza.egg-info/top_level.txt
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.483126 gyoza-0.0.6/
+-rwxrwxrwx   0 timdick    (501) staff       (20)     1091 2023-06-02 09:45:10.000000 gyoza-0.0.6/LICENSE
+-rw-r--r--   0 timdick    (501) staff       (20)     3007 2023-07-27 14:26:36.482730 gyoza-0.0.6/PKG-INFO
+-rwxr-xr-x   0 timdick    (501) staff       (20)     2620 2023-07-27 14:15:49.000000 gyoza-0.0.6/README.md
+-rwxr-xr-x   0 timdick    (501) staff       (20)      797 2023-07-27 14:23:46.000000 gyoza-0.0.6/pyproject.toml
+-rw-r--r--   0 timdick    (501) staff       (20)       38 2023-07-27 14:26:36.483271 gyoza-0.0.6/setup.cfg
+-rwxrwxrwx   0 timdick    (501) staff       (20)      173 2023-06-15 09:02:13.000000 gyoza-0.0.6/setup.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.474596 gyoza-0.0.6/src/
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.476491 gyoza-0.0.6/src/gyoza/
+-rw-r--r--   0 timdick    (501) staff       (20)        0 2023-06-07 09:58:20.000000 gyoza-0.0.6/src/gyoza/__init__.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.480899 gyoza-0.0.6/src/gyoza/modelling/
+-rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 11:33:16.000000 gyoza-0.0.6/src/gyoza/modelling/__init__.py
+-rw-r--r--   0 timdick    (501) staff       (20)    13578 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/modelling/data_iterators.py
+-rwxr-xr-x   0 timdick    (501) staff       (20)    42532 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/modelling/flow_layers.py
+-rw-r--r--   0 timdick    (501) staff       (20)    12575 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/modelling/losses.py
+-rw-r--r--   0 timdick    (501) staff       (20)     9161 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/modelling/masks.py
+-rw-r--r--   0 timdick    (501) staff       (20)     3173 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/modelling/standard_layers.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.482136 gyoza-0.0.6/src/gyoza/utilities/
+-rwxrwxrwx   0 timdick    (501) staff       (20)        0 2023-06-02 12:24:09.000000 gyoza-0.0.6/src/gyoza/utilities/__init__.py
+-rwxr-xr-x   0 timdick    (501) staff       (20)    11781 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/utilities/math.py
+-rw-r--r--   0 timdick    (501) staff       (20)     3987 2023-07-27 14:11:22.000000 gyoza-0.0.6/src/gyoza/utilities/tensors.py
+drwxr-xr-x   0 timdick    (501) staff       (20)        0 2023-07-27 14:26:36.478001 gyoza-0.0.6/src/gyoza.egg-info/
+-rwxrwxrwx   0 timdick    (501) staff       (20)     3007 2023-07-27 14:26:36.000000 gyoza-0.0.6/src/gyoza.egg-info/PKG-INFO
+-rwxrwxrwx   0 timdick    (501) staff       (20)      521 2023-07-27 14:26:36.000000 gyoza-0.0.6/src/gyoza.egg-info/SOURCES.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)        1 2023-07-27 14:26:36.000000 gyoza-0.0.6/src/gyoza.egg-info/dependency_links.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)       98 2023-07-27 14:26:36.000000 gyoza-0.0.6/src/gyoza.egg-info/requires.txt
+-rwxrwxrwx   0 timdick    (501) staff       (20)        6 2023-07-27 14:26:36.000000 gyoza-0.0.6/src/gyoza.egg-info/top_level.txt
```

### Comparing `gyoza-0.0.5/LICENSE` & `gyoza-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.5/pyproject.toml` & `gyoza-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gyoza"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Tim Dick", email="timdi@icloud.com" },
 ]
-description = "A package for invertible interpretable neural networks."
+description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "tensorflow >= 2.8.2",
+    "tensorflow >= 2.9",
     "matplotlib >= 3.5.3",
     "sphinx == 5.2.3",
     "sphinx-rtd-theme",
     "numpy >= 1.21.6",
     "build<0.10.0",
     "twine"
 ]
```

### Comparing `gyoza-0.0.5/src/gyoza/modelling/masks.py` & `gyoza-0.0.6/src/gyoza/modelling/masks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,103 @@
 import tensorflow as tf, numpy as np
 import gyoza.utilities.tensors as utt
 from abc import ABC
 from typing import List
 import copy as cp
 
 class Mask(tf.keras.Model, ABC):
-    """This class can be used to curate elements of a tensor x. As suggested by the name semi, half of x is selected
-    while the other half is not."""
+    """This class can be used to curate half of the elements of a tensor :math:`x`. An input :math:`x` to this layer is expected
+    to have ``shape`` along ``axes``. It is then flattened along these ``axes`` and the ``mask`` is applied. Thereafter, :math:`x`
+    is unflattened and returned. 
+    
+    :param axes: The axes along which the selection shall be applied.
+    :type axes: :class:`List[int]`
+    :param shape: The shape that input :math:`x` to this layer has along ``axes``.
+    :type shape: :class:`List[int]`
+    :param mask: The mask to be applied to data passing through this layer. Its shape is expected to be a vector with 
+        product(``shape``) many entries. 
+    :type mask: :class:`tensorflow.Tensor`
+    """
 
-    def __init__(self, axes: List[int], mask: tf.Variable):
-        """Constructor for this class. Subclasses can use it to store attributes.
-        
-        :param axes: The axes along which the selection shall be applied.
-        :type axes: :class:`List[int]`
-        :param mask: The mask to be applied to data passing through this layer. It should be an untrainable tensorflow Variable.
-        :type mask: :class:`tensorflow.Variable`
-        """
+    def __init__(self, axes: List[int], shape: List[int], mask: tf.Tensor):
 
         # Super
         super(Mask, self).__init__()
 
-        self.__axes__ = axes
-        """(:class:List[int]`) - The axes along which the selection shall be applied."""
+        self.__axes__ = cp.copy(axes)
+        """(:class:`List[int]`) - The axes along which the selection shall be applied."""
+
+        self.__shape__ = cp.copy(shape)
+        """(:class:`List[int]`) - The shape that input :math:`x` to this layer has along ``axes``."""
 
+        mask = tf.cast(mask, dtype=tf.keras.backend.floatx())
+        mask = tf.reshape(mask, [-1]) # Ensure it is flattened
         self.__mask__ = mask
-        """(:class:`tensorflow.Tensor) - The mask to be applied to data passing through this layer."""
+        """(:class:`tensorflow.Tensor) - The mask to be applied to input :math:`x` to this layer."""
 
         self.__from_to__ = Mask.__compute_from_to__(mask=mask)
         """(:class:`tensorflow.Tensor) - A matrix that defines the mapping during :py:meth:`arrange` and :py:meth:`re_arrange`."""
 
-        self.__mat_mul__ = tf.keras.layers.Dense(units=self.__from_to__.shape[0], use_bias=False, activation=None)
-        """(:class:`tensorflow.keras.layers.core.dense.Dense`) - A simple dense layer used for matrix multiplication."""
-
-        self.__mat_mul__.build(input_shape=[self.__from_to__.shape[0]])
-        self.__mat_mul__.set_weights([self.__from_to__])
+        self.built = True # This is set to prevent a warning saying that serialzation for mask is skipped becuase mask is not built
 
     @staticmethod
     def __compute_from_to__(mask: tf.Tensor) -> tf.Tensor:
         """Sets up a matrix that can be used to arrange all elements of an input x (after flattening) such the ones marked with a 1 
         by the mask appear first while the ones marked with a zero occur last.
         
         :param mask: The mask that defines the mapping. It can be of arbitrary shape since it will be flattened internally.
         :type mask: tensorflow.Tensor.
         :return: from_to (tensorflow.Tensor) - The matrix that determines the mapping on flattened inputs. Note: to arrange elements
             of an input x one has to flatten x along the mask dimension first, then broadcast ``from_to`` to fit the new shape of x.
             After matrix multiplication of the two one needs to undo the flattening to get the arrange x."""
 
-        # Flatten mask
-        mask = tf.reshape(mask, [-1]) 
-
         # Determine indices
         from_indices = tf.concat([tf.where(mask), tf.where(1-mask)],0).numpy()[:,0].tolist()
         to_indices = list(range(len(from_indices)))
         
         # Set up matrix
         from_to = np.zeros(shape=[mask.shape[0],mask.shape[0]]) # Square matrix
         from_to[from_indices, to_indices] = 1
-        from_to = tf.Variable(from_to, dtype=tf.float32)
+        from_to = tf.constant(from_to, dtype=tf.keras.backend.floatx())
 
         # Outputs
         return from_to
 
-    def apply(self, x: tf.Tensor, is_positive: bool = True) -> tf.Tensor:
+    def call(self, x: tf.Tensor, is_positive: bool = True) -> tf.Tensor:
         """Applies the binary mask of self to ``x``.
 
         :param x: The data to be masked. The expected shape of ``x`` depends on the axis and shape specified during initialization.
         :type x: :class:`tensorflow.Tensor`
         :param is_positive: Indicates whether the positive or negative mask version shall be applied, where negative == 1 - positive.
             Default is True.
         :type is_positive: bool, optional
         :return: x_masked (:class:`tensorflow.Tensor`) - The masked data of same shape as ``x``.
         """
 
-        # Parity
+        # Set parity of mask
         if is_positive: mask = self.__mask__
         else: mask = 1 - self.__mask__
+        
+        # Flatten x along self.__axes__ 
+        x_old_shape = cp.copy(x.shape)
+        x = utt.flatten_along_axes(x=x, axes=self.__axes__)
 
-        # Reshape mask to fit x
+        # Reshape mask
         axes = list(range(len(x.shape)))
-        for axis in self.__axes__: axes.remove(axis) 
-        mask = utt.expand_axes(x=mask, axes=axes)
-
-        # Apply mask to x
-        x_new = x * mask
+        axes.remove(self.__axes__[0])
+        mask = utt.expand_axes(x=mask, axes=axes) # Now has same shape as flat x along self.__axes__[0] and singleton everywhere else
+        
+        # Mask
+        x_masked = x * mask
 
+        # Unflatten to restore original shape
+        x_masked = tf.reshape(x_masked, shape=x_old_shape)
+        
         # Outputs
-        return x_new
+        return x_masked
 
     def arrange(self, x: tf.Tensor) -> tf.Tensor:
         """Arranges ``x`` into a vector such that all elements set to 0 by :py:meth:`mask` are enumerated first and all elements 
         that passed the mask are enumerated last.
 
         :param x: The data to be arranged. The shape is assumed to be compatible with :py:meth:`mask`.
         :type x: :class:`tensorflow.Tensor`
@@ -100,15 +108,15 @@
         # Flatten x along self.__axes__ to fit from_to 
         x = utt.flatten_along_axes(x=x, axes=self.__axes__)
 
         # Move self.__axes__[0] to end
         x = utt.swop_axes(x=x, from_axis=self.__axes__[0], to_axis=-1)
 
         # Matrix multiply
-        x_new = self.__mat_mul__(x[tf.newaxis])[0,:] # Use newaxis to ensure input has at least 2 axes which is required by dense layers
+        x_new = tf.linalg.matvec(tf.transpose(self.__from_to__, perm=[1,0]), x)
 
         # Move final axis to self.__axis__[0]
         x_new = utt.swop_axes(x=x_new, from_axis=-1, to_axis=self.__axes__[0])
 
         # Output
         return x_new
     
@@ -119,98 +127,78 @@
         :type x: :class:`tensorflow.Tensor`
         
         :return: x (tensorflow.Tensor) - The input to :py:meth:`arrange`."""
 
         # Move self.__axes__[0] to end
         x_new = utt.swop_axes(x=x_new, from_axis=self.__axes__[0], to_axis=-1)
         
-        # To invert arrange, we transpose multiplication with self.__from_to__
-        self.__mat_mul__.set_weights([tf.transpose(self.__from_to__, perm=[1,0])])
-        
         # Matrix multiply
-        x = self.__mat_mul__(x_new[tf.newaxis])[0,:] # Use newaxis to ensure input has at least 2 axes which is required by dense layers
-
-        # Undo the change to satistfy postcondition == precondition
-        self.__mat_mul__.set_weights([self.__from_to__])
-
+        x = tf.linalg.matvec(self.__from_to__, x_new)
+        
         # Move final axis to self.__axis__[0]
         x = utt.swop_axes(x=x, from_axis=-1, to_axis=self.__axes__[0])
 
         # Unflatten along self.__axes__
-        old_shape = x.shape[:self.__axes__[0]] + self.__mask__.shape + x.shape[self.__axes__[0]+1:]
+        old_shape = x.shape[:self.__axes__[0]] + self.__shape__ + x.shape[self.__axes__[0]+1:]
         x = tf.reshape(x, shape=old_shape)
 
         # Outputs
         return x
        
-class HeaviSide(Mask):
-    """Applies a one-dimensional Heaviside function of the shape 000111 to its input. Inputs are expected to have 1 spatial axes 
-    located at ``axes`` with ``shape`` many elements.
+class Heaviside(Mask):
+    """Applies a `Heaviside <https://en.wikipedia.org/wiki/Heaviside_step_function>`_ function to its input :math:`x`, e.g. 0001111. 
+    **IMPORTANT:** The Heaviside function is defined on a vector, yet by the requirement of :class:`Mask`, inputs :math:`x` to this 
+    layer are allowed to have more than one axis in ``axes``. As described in :class:`Mask`, an input :math:`x` is first flattened 
+    along ``axes`` and thus Heaviside can be applied. For background information see :class:`Mask`.
     
-    :param axes: The axes (here only one axis) along which the Heaviside mask shall be applied.
-    :type axes: :class:`List[int]`
-    :param shape: The number of units along ``axes``, e.g. [5] if an input x has shape [3,5,2] and ``axes`` == [1].
-    :type shape: :class:`List[int]`
+    :param shape: See base class :class:`Mask`.
+    :type shape: List[int]
+    :param axes: See base class :class:`Mask`.
+    :type axes: List[int]
     """
 
     def __init__(self, axes: int, shape: int):
         
-        # Input validity
-        assert len(axes) == 1, f"There must be one axis instead of {len(axes)} along which the Heaviside shall be applied."
-        assert len(shape) == 1, f"The shape input is equal to {shape}, but it must have one axis."
-
         # Set up mask
-        mask = np.ones(shape, dtype=np.float32)
+        mask = np.ones(shape=shape)
+        mask = np.reshape(mask, [-1]) # Flattening
         mask[:shape[0] // 2] = 0
-        mask = tf.Variable(initial_value=mask, trainable=False, dtype=tf.float32) 
+        mask = tf.constant(mask) 
 
         # Super
-        super(HeaviSide, self).__init__(axes=axes, mask=mask)
+        super(Heaviside, self).__init__(axes=axes, shape=shape, mask=mask)
 
-class SquareWave1D(Mask):
-    """Applies a one-dimensional square wave of the shape 010101 to its input. Inputs are expected to have 1 spatial axis located at
-    ``axes`` with ``shape`` many elements.
-    
-    :param axes: The axes (here only one axis) along which the square wave shall be applied.
+class CheckerBoard(Mask):
+    """Applies a `checkerboard <https://en.wikipedia.org/wiki/Check_(pattern)>`_ pattern to its input. Observe that it is equivalent 
+    to :class:`SquareWave` when ``shape`` == :math:`[m,n]` and :math:`n` is odd. Yet, when :math:`n` is even, :class:`SquareWave` has
+    columns of zeros alternating with columns of ones, whereas :class:`CheckerBoard` ensures a proper checker board pattern.
+        
+    :param axes: The **two** axes along which the checkerboard pattern shall be applied. Assumed to be consecutive indices, e.g. 
+        [2,3] or [3,4].
     :type axes: :class:`List[int]`
-    :param shape: The number of units along ``axes``, e.g. [5] if an input x has shape [3,5,2] and ``axes`` == [1].
+    :param shape: The shape of the mask along ``axes``, e.g. 64*32 if an input :math:`x` has shape [10,3,64,32] and ``axes`` == [2,3].
     :type shape: :class:`List[int]`
     """
 
-    def __init__(self, axes: int, shape: int):
+    def __init__(self, axes: List[int], shape: List[int]) -> None:
         
-        # Input validity
-        assert len(axes) == 1, f"There must be one axis instead of {len(axes)} along which the square-wave shall be applied."
-        assert len(shape) == 1, f"The shape input is equal to {shape}, but it must have one axis."
-
         # Set up mask
-        mask = np.ones(shape)
-        mask[::2] = 0
-        mask = tf.Variable(initial_value=mask, trainable=False, dtype=tf.float32) 
+        mask = np.zeros(shape) 
+        dimension_count = np.product(shape)
+        current_indices = [0] * len(shape)
+        mask[tuple(current_indices)] = np.sum(current_indices) % 2
+        for d in range(dimension_count):
+            # Increment index counter (with carry on to next axes if needed)
+            for s in range(len(shape)-1,-1,-1): 
+                if current_indices[s] == shape[s] - 1:
+                    current_indices[s] = 0
+                else:
+                    current_indices[s] += 1
+                    break
 
-        # Super
-        super(SquareWave1D, self).__init__(axes=axes, mask=mask)
+            mask[tuple(current_indices)] = np.sum(current_indices) % 2
 
-class SquareWave2D(Mask):
-    """Applies a two-dimensional square wave, also known as checkerboard pattern to its input. Inputs are expected to have 2 spatial
-    axes located at ``axes`` with ``shape`` units along those axes.
-        
-    :param axes: The two axes along which the square-wave pattern shall be applied. Assumed to be two consecutive indices.
-    :type axes: :class:`List[int]`
-    :param shape: The shape of the mask, e.g. 64*32 if an input x has shape [10,3,64,32] and ``axes`` == [2,3].
-    :type shape: :class:`List[int]`
-    """
-
-    def __init__(self, axes: List[int], shape: List[int]) -> None:
-        # Input validity
-        assert len(axes) == 2, f"There must be two axes instead of {len(axes)} along which the square-wave shall be applied."
-        assert axes[1] == axes[0] + 1, f"The axes {axes} have to be two consecutive indices."
-        assert len(shape) == 2, f"The shape input is equal to {shape}, but it must have two axes."
-
-        # Set up mask
-        mask = np.ones(shape) 
-        mask[1::2,1::2] = 0
-        mask[::2,::2] = 0
-        mask = tf.Variable(initial_value=mask, trainable=False, dtype=tf.float32) 
+        mask = np.reshape(mask, [-1]) # Flatten
+        mask = tf.constant(mask) 
         
         # Super
-        super(SquareWave2D, self).__init__(axes=axes, mask=mask)
+        super(CheckerBoard, self).__init__(axes=axes, shape=shape, mask=mask)
```

### Comparing `gyoza-0.0.5/src/gyoza/modelling/standard_layers.py` & `gyoza-0.0.6/src/gyoza/modelling/standard_layers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 import tensorflow as tf
 from typing import Dict, Any
 
 class BasicFullyConnectedNet(tf.keras.Model):
     """This class provides a basic fully connected network. It passes data through several :class:`tensorflow.keras.layers.Dense` 
     layers and applies optional batch normalization. 
     
-    :param int latent_channel_count: The number of channels maintained between intermediate layers. 
-    :param int output_channel_count: The number of channels of the final layer.
+    :param int latent_dimension_count: The number of dimensions maintained between intermediate layers. 
+    :param int output_dimension_count: The number of dimensions of the final layer.
     :param int depth: The number of layers to be used in between the input and output. If set to 0, there will only be a single 
         layer mapping from input to output. If set to 1, then there will be 1 intermediate layer, etc. 
     :param bool, optional use_tanh: Indicates whether each layer shall use the hyperbolic tangent activaction function. If set to False, 
         then a leaky relu is used. Defaults to False.
     :param bool, optional use_batch_normalization: Indicates whether each layer shall use batch normalization or not. Defaults to False.
     """
 
-    def __init__(self, latent_channel_count:int, output_channel_count:int, depth: int, use_tanh:bool=False, use_batch_normalization:bool=False):
+    def __init__(self, latent_dimension_count:int, output_dimension_count:int, depth: int):
         
         # Super
         super(BasicFullyConnectedNet, self).__init__()
         
         # Compile list of layers
-        channel_counts = [latent_channel_count] * depth + [output_channel_count]
+        dimension_counts = [latent_dimension_count] * depth + [output_dimension_count]
         layers = []
         for d in range(depth + 1):
-            layers.append(tf.keras.layers.Dense(units=channel_counts[d]))
-            if use_batch_normalization: layers.append(tf.keras.layers.BatchNormalization(channel_counts[d]), axis=-1)
-            if d < depth or not use_tanh: layers.append(tf.keras.layers.LeakyReLU())
-        
-        if use_tanh: layers.append(tf.keras.layers.Tanh())
+            layers.append(tf.keras.layers.Dense(units=dimension_counts[d]))
+            if d < depth: layers.append(tf.keras.layers.LeakyReLU())
         
         # Attributes
         self.sequential = tf.keras.Sequential(layers)
         """Attribute that refers to the :class:`tensorflow.keras.Sequential` model collecting all layers of self."""
 
     def call(self, x: tf.Tensor) -> tf.Tensor:
         """"""
         
         # Predict
         y_hat = self.sequential(x)
 
         # Outputs:
         return y_hat
     
-class ChannelWiseConvolution2D(tf.keras.Model):
-    """This class provides a sequential convolutional neural network that applies the same spatial filters to each channel.
+class ChannelWiseConvolutionTwoAxes(tf.keras.Model):
+    """This class provides a sequential convolutional neural network that applies the same spatial filters to each dimension.
 
     :param layer_count: The number of layers.
     :type layer_count: int
     :param conv2D_kwargs: The kew-word arguments for the :class:`tensorflow.keras.layers.Conv2D` layers that are used here.
-        Important: The channel_axis is assumed to be the default, i.e. the last axis.
+        **Important**: The channel_axis is assumed to be the default, i.e. the last axis.
     """
 
     def __init__(self, layer_count:int = 3, conv2D_kwargs: Dict[str, Any] = {}):
 
         # Super
-        super(ChannelWiseConvolution2D, self).__init__()
+        super(ChannelWiseConvolutionTwoAxes, self).__init__()
 
         # Create layers
         layers = [None] * (layer_count + 2)
         layers[0] = tf.keras.layers.Lambda(lambda x: tf.transpose(x[:,tf.newaxis,:,:,:], [0,4,2,3,1]))
         for l in range(layer_count): layers[l+1] = tf.keras.layers.Conv2D(**conv2D_kwargs)
         layers[-1] = tf.keras.layers.Lambda(lambda x: tf.squeeze(tf.transpose(x, [0,4,2,3,1])))
```

### Comparing `gyoza-0.0.5/src/gyoza/utilities/tensors.py` & `gyoza-0.0.6/src/gyoza/utilities/tensors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import tensorflow as tf
 from typing import List
+import copy as cp
 
 def move_axis(x: tf.Tensor, from_index: int, to_index: int) -> tf.Tensor:
     """Moves an axis from from_index to to_index.
     
     :param x: A tensor of shape [..., k, ...] where k is at from_index.
     :type x: :class:`tensorflow.Tensor`
     :param from_index: The index of the axis before transposition.
     :type from_index: int
     :param to_index: The index of the axis after transposition.
     :type to_index: int
-    :return: x_new (:class:`tensorflow.Tensor`): The tensor x transposed such that shape [..., k, ...] is now at to_index."""
+    :return: x_new (:class:`tensorflow.Tensor`): The tensor x transposed such that shape [..., k, ...] now has k at to_index."""
  
+    # Input validity
+    if from_index == -1: from_index = len(x.shape)-1
+    if to_index == -1: to_index = len(x.shape)-1
+
     # Move axis
     new_order = list(range(len(x.shape)))
     del new_order[from_index]
     new_order.insert(to_index, from_index)
     x_new = tf.transpose(a=x, perm=new_order)
 
     # Outputs
@@ -63,19 +68,25 @@
     
     :param x: The input to be flattened. Assumed to have at least as many axes as indicated by ``axes``.
     :type x: :class:`tensorflow.Tensor`
     :param axes: The axes along which the input shall be flattened.
     :type axes: :class:`List[int]`
     :return: x_new (:class:`tensorflow.Tensor`) - The reshaped tensor ``x`` flattened along ``axes``."""
 
+    # Exception handling
+    if len(axes) == 0: return x
+
     # Reshape
     new_shape = list(x.shape)
-    new_shape[axes[0]] = tf.reduce_prod(x.shape[axes[0]:axes[-1]+1]).numpy()
-    for a in axes[1:]:
-        del new_shape[a]
+
+    new_shape[axes[0]] = 1
+    for a in axes: new_shape[axes[0]] *= x.shape[a]
+    axes = cp.copy(axes); axes.reverse()
+    for a in axes[:-1]: del new_shape[a]
+
     x_new = tf.reshape(x, new_shape) # Now has original shape except for axes which have been flattened
 
     # Outputs
     return x_new
 
 def swop_axes(x: tf.Tensor, from_axis: int, to_axis: int) -> tf.Tensor:
     """Swops axes of ``x``.
```

