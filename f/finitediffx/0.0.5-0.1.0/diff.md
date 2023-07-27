# Comparing `tmp/FiniteDiffX-0.0.5.tar.gz` & `tmp/finitediffx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiniteDiffX-0.0.5.tar", last modified: Thu Jun  8 12:45:48 2023, max compression
+gzip compressed data, was "finitediffx-0.1.0.tar", last modified: Thu Jul 27 14:07:00 2023, max compression
```

## Comparing `FiniteDiffX-0.0.5.tar` & `finitediffx-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9581 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/finitediffx/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/finitediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/finitediffx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/finitediffx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/finitediffx/_src/fgrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    24621 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/finitediffx/_src/finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/finitediffx/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/tests/test_fgrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/tests/test_finite_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:07:00.762382 finitediffx-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-27 14:06:44.000000 finitediffx-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-27 14:07:00.762382 finitediffx-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-27 14:06:44.000000 finitediffx-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:07:00.762382 finitediffx-0.1.0/finitediffx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-27 14:06:44.000000 finitediffx-0.1.0/finitediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:07:00.762382 finitediffx-0.1.0/finitediffx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-27 14:06:44.000000 finitediffx-0.1.0/finitediffx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-07-27 14:06:44.000000 finitediffx-0.1.0/finitediffx/_src/fgrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24729 2023-07-27 14:06:44.000000 finitediffx-0.1.0/finitediffx/_src/finite_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-27 14:06:44.000000 finitediffx-0.1.0/finitediffx/_src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:07:00.762382 finitediffx-0.1.0/finitediffx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-27 14:07:00.000000 finitediffx-0.1.0/finitediffx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 14:07:00.000000 finitediffx-0.1.0/finitediffx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:07:00.000000 finitediffx-0.1.0/finitediffx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 14:07:00.000000 finitediffx-0.1.0/finitediffx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 14:07:00.000000 finitediffx-0.1.0/finitediffx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-27 14:06:44.000000 finitediffx-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:07:00.762382 finitediffx-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:07:00.762382 finitediffx-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-07-27 14:06:44.000000 finitediffx-0.1.0/tests/test_fgrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-07-27 14:06:44.000000 finitediffx-0.1.0/tests/test_finite_diff.py
```

### Comparing `FiniteDiffX-0.0.5/LICENSE` & `finitediffx-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.5/finitediffx/__init__.py` & `finitediffx-0.1.0/finitediffx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,8 @@
     "value_and_fgrad",
     "Offset",
     "define_fdjvp",
     "generate_finitediff_coeffs",
 )
 
 
-__version__ = "0.0.5"
+__version__ = "0.1.0"
```

### Comparing `FiniteDiffX-0.0.5/finitediffx/_src/__init__.py` & `finitediffx-0.1.0/finitediffx/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.5/finitediffx/_src/fgrad.py` & `finitediffx-0.1.0/finitediffx/_src/fgrad.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,29 +17,30 @@
 import dataclasses as dc
 import functools as ft
 from typing import Any, Callable, Sequence, TypeVar, Union
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
+import numpy as np
 from typing_extensions import ParamSpec
 
 from finitediffx._src.utils import _generate_central_offsets, generate_finitediff_coeffs
 
 __all__ = ("fgrad", "Offset", "define_fdjvp", "value_and_fgrad")
 
 P = ParamSpec("P")
 T = TypeVar("T")
-constant_treedef = jtu.tree_structure(0)
 PyTree = Any
 
 
 @dc.dataclass(frozen=True)
 class Offset:
-    """Convinience class for finite difference offsets used inside `fgrad`
+    """Convinience class for finite difference offsets used inside :func:`.fgrad`
+    :func:`.value_and_fgrad`.
 
     Args:
         accuracy: The accuracy of the finite difference scheme. Must be >=2.
 
     Example:
         >>> import finitediffx as fdx
         >>> fdx.fgrad(lambda x: x**2, offsets=fdx.Offset(accuracy=2))(1.0)
@@ -49,69 +50,14 @@
     accuracy: int
 
 
 OffsetType = Union[jax.Array, Offset, PyTree]
 StepsizeType = Union[jax.Array, float, PyTree]
 
 
-def _evaluate_func_at_shifted_steps_along_argnum(
-    func: Callable[P, T],
-    *,
-    coeffs: jax.Array,
-    offsets: jax.Array,
-    argnum: int,
-    step_size: StepsizeType,
-    derivative: int,
-):
-    if not isinstance(argnum, int) or argnum < 0:
-        raise ValueError(f"argnum must be a non-negative integer, got {argnum}")
-
-    dxs = offsets * step_size
-    den = step_size**derivative
-
-    def wrapper(*args, **kwargs):
-        if not hasattr(args[argnum], "shape"):
-            # scalar perturbation
-            def perturb(h):
-                args_ = list(args)
-                args_[argnum] += h
-                return func(*args_, **kwargs)
-
-            return sum([coeff * perturb(dx) / den for coeff, dx in zip(coeffs, dxs)])
-
-        # elementwise perturbation
-        # should be much slower than jax.grad for large arrays
-        # but can be used for non-tracable code where jax.grad fails
-        def perturb(h):
-            xflat = jnp.array(args[argnum].flatten())
-            arange = jnp.arange(len(xflat))
-            shape = args[argnum].shape
-
-            def perturb_element(i):
-                xflat_ = xflat.at[i].add(h)
-                args_ = list(args)
-                args_[argnum] = xflat_.reshape(shape)
-                return func(*args_, **kwargs)
-
-            # `jax.vmap` can be used here and perform better
-            # but it would fail in case of non-tracable code
-            # may have try/excpet wiht `jax.errors.TracerArrayConversionError``
-            result = jnp.array([perturb_element(i) for i in arange])
-
-            # the function might return non-scalars
-            try:
-                return result.reshape(shape)
-            except Exception:
-                raise TypeError("Non scalar-output.")
-
-        return sum([coeff * perturb(dx) / den for coeff, dx in zip(coeffs, dxs)])
-
-    return wrapper
-
-
 def resolve_step_size(
     step_size: StepsizeType | Sequence[StepsizeType] | None,
     treedef: jtu.PyTreeDef,
     derivative: int,
 ) -> Sequence[StepsizeType] | StepsizeType:
     # return non-tuple values if length is None
     length = treedef.num_leaves
@@ -168,86 +114,181 @@
         f"- `jax.Array`\n"
         f"- tuple of `Offset` or `jax.Array` for tuple argnums.\n"
         f"- pytree with the same structure as the desired arg.\n"
         f"but got {type(offsets)=}"
     )
 
 
+def _perturb_flat_args(
+    *,
+    flat_func: Callable,
+    coeffs: jax.Array,
+    flat_offsets: jax.Array,
+    flat_argnum: int,
+    flat_step_size: jax.Array,
+    derivative: int,
+    average_gradients: bool = False,
+):
+    def flat_args_wrapper(*flat_args):
+        def scalar_perturb(*, h: float):
+            return flat_func(
+                *(
+                    flat_args[:flat_argnum]
+                    + (flat_args[flat_argnum] + h,)
+                    + flat_args[flat_argnum + 1 :]
+                )
+            )
+
+        def array_perturb(*, h: float) -> jax.Array:
+            # should be much slower than jax.grad for large arrays
+            # but can be used for non-tracable code where jax.grad fails
+            size = flat_args[flat_argnum].size
+            indices = jnp.arange(size)
+            shape = flat_args[flat_argnum].shape
+            flat_array = jnp.array(flat_args[flat_argnum].reshape(-1))
+
+            def perturb_element(index):
+                return flat_func(
+                    *(
+                        flat_args[:flat_argnum]
+                        + (flat_array.at[index].add(h).reshape(shape),)
+                        + flat_args[flat_argnum + 1 :]
+                    )
+                )
+
+            try:
+                # in case of tracable code (jax code)
+                result = jax.vmap(perturb_element)(indices)
+            except jax.errors.TracerArrayConversionError:
+                # non-tracable code e.g. numpy code
+                result = jnp.array([perturb_element(index) for index in indices])
+
+            if result.size > size:
+                raise TypeError("Non scalar-output.")
+
+            return result.reshape(shape)
+
+        def array_average_perturb(*, h: float) -> jax.Array:
+            # perturb the array all at once and average the result
+            # faster than array_perturb for large arrays but gives
+            # average gradient
+            shape = flat_args[flat_argnum].shape
+            size = flat_args[flat_argnum].size
+            result = flat_func(
+                *(
+                    flat_args[:flat_argnum]
+                    + ((flat_args[flat_argnum] + h),)
+                    + flat_args[flat_argnum + 1 :]
+                )
+            )
+
+            if result.size > size:
+                raise TypeError("Non scalar-output.")
+
+            result = jnp.broadcast_to(result, shape)
+            result = result / result.size
+            return result
+
+        perturb_func = (
+            (array_average_perturb if average_gradients else array_perturb)
+            if isinstance(flat_args[flat_argnum], (np.ndarray, jax.Array))
+            else scalar_perturb
+        )
+
+        return sum(
+            coeff * perturb_func(h=dx) / flat_step_size**derivative
+            for coeff, dx in zip(coeffs, flat_offsets * flat_step_size)
+        )
+
+    return flat_args_wrapper
+
+
 def _fgrad_along_argnum(
     func: Callable,
     *,
     argnum: int = 0,
     step_size: StepsizeType | None = None,
     offsets: OffsetType = Offset(accuracy=3),
     derivative: int = 1,
+    average_gradients: bool = False,
 ):
-    if not isinstance(argnum, int):
-        raise TypeError(f"argnum must be an integer, got {type(argnum)}")
-
     def wrapper(*args, **kwargs):
-        flat_args, arg_treedef = jtu.tree_flatten(args[argnum])
-        args_ = list(args)
+        # full args/kwargs
+        flat_args, flat_treedef = jtu.tree_flatten(args[argnum])
 
-        def func_wrapper(*leaves):
-            args_[argnum] = jtu.tree_unflatten(arg_treedef, leaves)
-            return func(*args_, **kwargs)
-
-        spec = dict(treedef=arg_treedef, derivative=derivative)
-        step_size_ = resolve_step_size(step_size, **spec)
-        offsets_ = resolve_offsets(offsets, **spec)
-
-        flat_result = [
-            _evaluate_func_at_shifted_steps_along_argnum(
-                func=func_wrapper,
+        def flat_func(*flat_args):
+            return func(
+                *(
+                    args[:argnum]
+                    + (jtu.tree_unflatten(flat_treedef, flat_args),)
+                    + args[argnum + 1 :]
+                ),
+                **kwargs,
+            )
+
+        step_size_ = resolve_step_size(step_size, flat_treedef, derivative)
+        offsets_ = resolve_offsets(offsets, flat_treedef, derivative)
+
+        flat_result = (
+            _perturb_flat_args(
+                flat_func=flat_func,
                 coeffs=generate_finitediff_coeffs(oi, derivative),
-                offsets=oi,
-                step_size=si,
+                flat_offsets=oi,
+                flat_step_size=si,
+                flat_argnum=i,
                 derivative=derivative,
-                argnum=i,
+                average_gradients=average_gradients,
             )(*flat_args)
             for i, (oi, si) in enumerate(zip(offsets_, step_size_))
-        ]
+        )
 
-        return jtu.tree_unflatten(arg_treedef, flat_result)
+        return jtu.tree_unflatten(flat_treedef, flat_result)
 
     return wrapper
 
 
 def value_and_fgrad(
-    func: Callable,
+    func: Callable[P, T],
     *,
     argnums: int | tuple[int, ...] = 0,
     step_size: StepsizeType | None = None,
     offsets: OffsetType = Offset(accuracy=3),
     derivative: int = 1,
     has_aux: bool = False,
-) -> Callable:
+    average_gradients: bool = False,
+):
     """Finite difference derivative of a function with respect to one of its arguments.
-    similar to jax.grad but with finite difference approximation
+
+    Similar to ``jax.value_and_grad`` but with finite difference approximation
 
     Args:
         func: function to differentiate
         argnums: argument number to differentiate. Defaults to 0.
             If a tuple is passed, the function is differentiated with respect to
             all the arguments in the tuple.
         step_size: step size for the finite difference stencil. If `None`, the step size
-            is set to `(2) ** (-23 / (2 * derivative))`
+            is set to ``(2) ** (-23 / (2 * derivative))``
         offsets: offsets for the finite difference stencil. Accepted types are:
-            - `jax.Array` defining location of function evaluation points.
-            - `Offset` with accuracy field to automatically generate offsets.
-            - pytree of `jax.Array`/`Offset` to define offsets for each argument
-                of the same pytree structure as argument defined by `argnums`.
+
+            - ``jax.Array`` defining location of function evaluation points.
+            - :class:`Offset` with accuracy field to automatically generate offsets.
+            - pytree of ``jax.Array``/ :class:`.Offset` to define offsets for
+              each argument of the same pytree structure as argument defined
+              by ``argnums``.
+
         derivative: derivative order. Defaults to 1.
-        has_aux: whether the function returns an auxiliary output. Defaults to False.
-            If True, the derivative function will return a tuple of the form:
-            ((value,aux), derivative) otherwise (value, derivative)
+        has_aux: whether the function returns an auxiliary output. Defaults to
+            ``False``. If True, the derivative function will return a tuple of
+            the form: ((value,aux), derivative) otherwise (value, derivative)
+        average_gradients: whether to average the array gradients. Yields faster
+            results. Defaults to ``False``.
 
     Returns:
-        Value and derivative of the function if `has_aux` is False.
-        If `has_aux` is True, the derivative function will return a tuple of the form:
+        Value and derivative of the function if ``has_aux`` is ``False``.
+        If ``has_aux`` is True, the derivative function will return a tuple of the form:
         ((value,aux), derivative)
 
     Example:
         >>> import finitediffx as fdx
         >>> import jax
         >>> import jax.numpy as jnp
         >>> def f(x, y):
@@ -274,14 +315,15 @@
         # fgrad(func, argnums=0)
         dfunc = _fgrad_along_argnum(
             func=func_,
             argnum=argnums,
             step_size=step_size,
             offsets=offsets,
             derivative=derivative,
+            average_gradients=average_gradients,
         )
 
         if has_aux is True:
 
             @ft.wraps(func)
             def wrapper(*a, **k):
                 value, aux = func(*a, **k)
@@ -295,38 +337,40 @@
 
         return wrapper
 
     if isinstance(argnums, tuple):
         # fgrad(func, argnums=(0,1))
         # return a tuple of derivatives evaluated at each argnum
         # this behavior is similar to jax.grad(func, argnums=(...))
+        if not all(isinstance(ai, int) for ai in argnums):
+            raise TypeError(f"{argnums=} must be an integer or a tuple of integers")
+
         if isinstance(offsets, tuple):
             if len(offsets) != len(argnums):
                 raise AssertionError("offsets must have the same length as argnums")
-            offsets_ = offsets
         else:
-            offsets_ = (offsets,) * len(argnums)
+            offsets = (offsets,) * len(argnums)
 
         if isinstance(step_size, tuple):
             if len(step_size) != len(argnums):
                 raise AssertionError("step_size must have the same length as argnums")
-            step_size_ = step_size
 
         else:
-            step_size_ = (step_size,) * len(argnums)
+            step_size = (step_size,) * len(argnums)
 
         dfuncs = [
             _fgrad_along_argnum(
                 func=func_,
                 argnum=ai,
                 step_size=si,
                 offsets=oi,
                 derivative=derivative,
+                average_gradients=average_gradients,
             )
-            for oi, si, ai in zip(offsets_, step_size_, argnums)
+            for oi, si, ai in zip(offsets, step_size, argnums)
         ]
 
         if has_aux:
 
             @ft.wraps(func)
             def wrapper(*a, **k):
                 # destructuring the tuple to ensure
@@ -349,64 +393,69 @@
     func: Callable,
     *,
     argnums: int | tuple[int, ...] = 0,
     step_size: StepsizeType | None = None,
     offsets: OffsetType = Offset(accuracy=3),
     derivative: int = 1,
     has_aux: bool = False,
+    average_gradients: bool = False,
 ) -> Callable:
     """Finite difference derivative of a function with respect to one of its arguments.
-    similar to jax.grad but with finite difference approximation
+
+    Similar to ``jax.grad`` but with finite difference approximation.
 
     Args:
         func: function to differentiate
         argnums: argument number to differentiate. Defaults to 0.
             If a tuple is passed, the function is differentiated with respect to
             all the arguments in the tuple.
         step_size: step size for the finite difference stencil. If `None`, the step size
             is set to `(2) ** (-23 / (2 * derivative))`
         offsets: offsets for the finite difference stencil. Accepted types are:
-            - `jax.Array` defining location of function evaluation points.
-            - `Offset` with accuracy field to automatically generate offsets.
-            - pytree of `jax.Array`/`Offset` to define offsets for each argument
-                of the same pytree structure as argument defined by `argnums`.
+
+            - ``jax.Array`` defining location of function evaluation points.
+            - :class:`.Offset` with accuracy field to automatically generate offsets.
+            - pytree of ``jax.Array``/:class:`.Offset` to define offsets for
+              each argument of the same pytree structure as argument defined
+              by ``argnums``.
+
         derivative: derivative order. Defaults to 1.
-        has_aux: whether the function returns an auxiliary output. Defaults to False.
-            If True, the derivative function will return a tuple of the form:
-            (derivative, aux) otherwise it will return only the derivative.
+        has_aux: whether the function returns an auxiliary output. Defaults to
+            ``False``. If ``True``, the derivative function will return a tuple
+            of the form: (derivative, aux) otherwise it will return only the derivative.
+        average_gradients: whether to average the array gradients. Yields faster
+            results. Defaults to ``False``.
 
     Returns:
-        Derivative of the function if `has_aux` is False, otherwise a tuple of
+        Derivative of the function if ``has_aux`` is ``False``, otherwise a tuple of
         the form: (derivative, aux)
 
     Example:
         >>> import finitediffx as fdx
         >>> import jax
         >>> import jax.numpy as jnp
-
         >>> def f(x, y):
         ...    return x**2 + y**2
-
         >>> df=fdx.fgrad(
         ...    func=f,
         ...    argnums=1,  # differentiate with respect to y
         ...    offsets=fdx.Offset(accuracy=2)  # use 2nd order accurate finite difference
         ... )
-
         >>> df(2.0, 3.0)
         Array(6., dtype=float32)
 
     """
     value_and_fgrad_func = value_and_fgrad(
         func=func,
         argnums=argnums,
         step_size=step_size,
         offsets=offsets,
         derivative=derivative,
         has_aux=has_aux,
+        average_gradients=average_gradients,
     )
 
     if has_aux:
 
         @ft.wraps(func)
         def wrapper(*a, **k):
             (_, aux), g = value_and_fgrad_func(*a, **k)
@@ -428,29 +477,29 @@
     step_size: tuple[float, ...] | float | None = None,
 ) -> Callable[P, T]:
     """Define the JVP rule for a function using finite difference.
 
     Args:
         func: function to define the JVP rule for
         offsets: offsets for the finite difference stencil. Accepted types are:
-            - `jax.Array` defining location of function evaluation points.
-            - `Offset` with accuracy field to automatically generate offsets.
-            - tuple of `Offset` or `jax.Array` defining offsets for each argument.
+            - ``jax.Array`` defining location of function evaluation points.
+            - :class:`.Offset` with accuracy field to automatically generate offsets.
+            - tuple of `Offset` or ``jax.Array`` defining offsets for each argument.
         step_size: step size for the finite difference stencil. Accepted types are:
-            - `float` defining the step size for all arguments.
-            - `tuple` of `float` defining the step size for each argument.
-            - `None` to use the default step size for each argument.
+            - ``float`` defining the step size for all arguments.
+            - ``tuple`` of ``float`` defining the step size for each argument.
+            - ``None`` to use the default step size for each argument.
 
     Returns:
         Callable: function with JVP rule defined using finite difference.
 
     Note:
-        - This function is motivated by [`JEP`](https://github.com/google/jax/issues/15425)
-        - This function can be used with `jax.pure_callback` to define the JVP
-            rule for a function that is not differentiable by JAX.
+        - This function is motivated by [``JEP``](https://github.com/google/jax/issues/15425)
+        - This function can be used with ``jax.pure_callback`` to define the JVP
+            rule for a function that is not differentiable by ``jax``.
 
         Example:
             >>> import jax
             >>> import jax.numpy as jnp
             >>> import finitediffx as fdx
             >>> import functools as ft
             >>> import numpy as onp
```

### Comparing `FiniteDiffX-0.0.5/finitediffx/_src/finite_diff.py` & `finitediffx-0.1.0/finitediffx/_src/finite_diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,35 +203,37 @@
         ...     dFdX = fdx.difference(F, step_size=dx, axis=0, accuracy=3, method="central")
         ...     dFdXdY = fdx.difference(dFdX, step_size=dy, axis=1, accuracy=3, method="central")
         ...     # 1d finite difference derivative
         ...     x = jnp.array([1.2, 1.3, 2.2, 3., 4.5, 5.5, 6., 7., 8., 20.])
         ...     print(fdx.difference(x, accuracy=1))
         [ 0.1   0.5   0.85  1.15  1.25  0.75  0.75  1.    6.5  12.  ]
 
-
     Note:
         Handling of boundary points is done by applying forward/backward difference
         to the first/last element and central difference to the interior elements.
         For the previous example, the following steps are performed:
 
-        - apply forward difference to the first element with accuracy 1
-        x_1 = 1.3-1.2 = 0.1
+        - Apply forward difference to the first element with accuracy
+
+            - ``x_1 = 1.3-1.2 = 0.1``
+
+        - Apply central difference to interior elements with accuracy 2
+
+            - ``x_2 = (2.2-1.2)/2 = 0.5``
+            - ``x_3 = (3.-1.3)/2 = 0.85``
+            - ``x_4 = (4.5-2.2)/2 = 1.15``
+            - ``x_5 = (5.5-3.)/2 = 1.25``
+            - ``x_6 = (6.-4.5)/2 = 0.75``
+            - ``x_7 = (7.-5.5)/2 = 0.75``
+            - ``x_8 = (8.-6.)/2 = 1.``
+            - ``x_9 = (20.-7.)/2 = 6.5``
 
-        - apply central difference to interior elements with accuracy 2
-        x_2 = (2.2-1.2)/2 = 0.5
-        x_3 = (3.-1.3)/2 = 0.85
-        x_4 = (4.5-2.2)/2 = 1.15
-        x_5 = (5.5-3.)/2 = 1.25
-        x_6 = (6.-4.5)/2 = 0.75
-        x_7 = (7.-5.5)/2 = 0.75
-        x_8 = (8.-6.)/2 = 1.
-        x_9 = (20.-7.)/2 = 6.5
+        - Apply backward difference to the last element with accuracy 1
 
-        - apply backward difference to the last element with accuracy 1
-        x_10 = 20.-8. = 12.
+            - ``x_10 = 20.-8. = 12.``
     """
     size = array.shape[axis]
 
     center_offsets = _generate_central_offsets(derivative, accuracy + 1)
     center_coeffs = generate_finitediff_coeffs(center_offsets, derivative)
 
     left_offsets = _generate_forward_offsets(derivative, accuracy)
@@ -379,15 +381,15 @@
         >>> with jax.experimental.enable_x64():
         ...    x, y = [jnp.linspace(-1, 1, 100)] * 2
         ...    dx, dy = x[1] - x[0], y[1] - y[0]
         ...    X, Y = jnp.meshgrid(x, y, indexing="ij")
         ...    F1 = X**2 * Y
         ...    F2 = 5 * X + jnp.sin(Y)
         ...    F = jnp.stack([F1, F2], axis=0)
-        ...    JF = jacobian(F, accuracy=4, step_size=(dx, dy))
+        ...    JF = fdx.jacobian(F, accuracy=4, step_size=(dx, dy))
         ...    JF_true = jnp.array([[2 * X * Y, X**2], [5*jnp.ones_like(X), jnp.cos(Y)]])
         ...    npt.assert_allclose(JF, JF_true, atol=1e-7)
     """
     accuracy = _check_and_return(accuracy, array.ndim - 1, "accuracy")
     step_size = _check_and_return(step_size, array.ndim - 1, "step_size")
 
     return jnp.stack(
@@ -427,15 +429,15 @@
         >>> import numpy.testing as npt
         >>> x, y = [jnp.linspace(0, 1, 100)] * 2
         >>> dx, dy = x[1] - x[0], y[1] - y[0]
         >>> X, Y = jnp.meshgrid(x, y, indexing="ij")
         >>> F1 = X**2 + Y**3
         >>> F2 = X**4 + Y**3
         >>> F = jnp.stack([F1, F2], axis=0) # 2D vector field F = (F1, F2)
-        >>> divZ = divergence(F,step_size=(dx,dy), accuracy=7, keepdims=False)
+        >>> divZ = fdx.divergence(F,step_size=(dx,dy), accuracy=7, keepdims=False)
         >>> divZ_true = 2*X + 3*Y**2  # (dF1/dx) + (dF2/dy)
         >>> npt.assert_allclose(divZ, divZ_true, atol=5e-4)
     """
     accuracy = _check_and_return(accuracy, array.ndim - 1, "accuracy")
     step_size = _check_and_return(step_size, array.ndim - 1, "step_size")
 
     result = sum(
@@ -729,11 +731,11 @@
             accuracy=accuracy,
             step_size=step_size,
             method=method,
             keepdims=keepdims,
         )
 
     raise ValueError(
-        f"`curl` is only implemented for 2D and 3D vector fields, got {array.ndim}D"
+        f"`curl` is only implemented for 2D and 3D vector fields, got {array.ndim=}"
         "for 2D vector fields, the leading axis must have a shape=2, "
         "for 3D vector fields, the leading axis must have a shape=3"
     )
```

### Comparing `FiniteDiffX-0.0.5/finitediffx/_src/utils.py` & `finitediffx-0.1.0/finitediffx/_src/utils.py`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.5/tests/test_fgrad.py` & `finitediffx-0.1.0/tests/test_fgrad.py`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.5/tests/test_finite_diff.py` & `finitediffx-0.1.0/tests/test_finite_diff.py`

 * *Files identical despite different names*

