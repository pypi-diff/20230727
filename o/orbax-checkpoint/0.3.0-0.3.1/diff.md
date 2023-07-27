# Comparing `tmp/orbax_checkpoint-0.3.0.tar.gz` & `tmp/orbax_checkpoint-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax_checkpoint-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orbax_checkpoint-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orbax_checkpoint-0.3.0.tar` & `orbax_checkpoint-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,35 @@
--rw-r--r--   0        0        0    11357 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/LICENSE
--rw-r--r--   0        0        0      834 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/README.md
--rw-r--r--   0        0        0     2960 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2663 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2832 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5932 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     5692 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2188 2023-07-24 18:30:43.670362 orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    37382 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0    15104 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0    11915 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     4839 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0      740 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0     1576 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     2002 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/lazy_utils.py
--rw-r--r--   0        0        0     7672 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0     1129 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/msgpack_utils_test.py
--rw-r--r--   0        0        0    45194 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0      757 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/__init__.py
--rw-r--r--   0        0        0      757 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/testing/__init__.py
--rw-r--r--   0        0        0      147 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/testing/foo.proto
--rw-r--r--   0        0        0     1644 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/testing/foo_pb2.py
--rw-r--r--   0        0        0     1173 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/tree_metadata.proto
--rw-r--r--   0        0        0     2814 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto/tree_metadata_pb2.py
--rw-r--r--   0        0        0     3016 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto_checkpoint_handler.py
--rw-r--r--   0        0        0     2108 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/proto_checkpoint_handler_test.py
--rw-r--r--   0        0        0    33472 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5328 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0    11807 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    15155 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    26140 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    25612 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     8158 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     1153 2023-07-24 18:30:43.674362 orbax_checkpoint-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 orbax_checkpoint-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/LICENSE
+-rw-r--r--   0        0        0      834 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/README.md
+-rw-r--r--   0        0        0     2920 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2663 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2832 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     5803 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1440 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0     5692 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     2188 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    37385 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0    15252 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0    11915 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     4839 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0      740 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0     1576 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     2103 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     1821 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     7672 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0     1129 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/msgpack_utils_test.py
+-rw-r--r--   0        0        0    45194 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0      757 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto/__init__.py
+-rw-r--r--   0        0        0      757 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto/testing/__init__.py
+-rw-r--r--   0        0        0      136 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto/testing/foo.proto
+-rw-r--r--   0        0        0     1549 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto/testing/foo_pb2.py
+-rw-r--r--   0        0        0     3055 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto_checkpoint_handler.py
+-rw-r--r--   0        0        0     2108 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto_checkpoint_handler_test.py
+-rw-r--r--   0        0        0    30479 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     5109 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0    11807 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    15155 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    25970 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    24135 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0     8158 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     1153 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 orbax_checkpoint-0.3.1/PKG-INFO
```

### Comparing `orbax_checkpoint-0.3.0/LICENSE` & `orbax_checkpoint-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/README.md` & `orbax_checkpoint-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/__init__.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 """Defines exported symbols for the namespace package `orbax.checkpoint`."""
 
 import contextlib
 import functools
 
 from orbax.checkpoint import aggregate_handlers
 from orbax.checkpoint import checkpoint_utils
-from orbax.checkpoint import lazy_utils
 from orbax.checkpoint import msgpack_utils
 from orbax.checkpoint import test_utils
 from orbax.checkpoint import transform_utils
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
 from orbax.checkpoint.abstract_checkpointer import AbstractCheckpointer
 from orbax.checkpoint.array_checkpoint_handler import ArrayCheckpointHandler
@@ -60,8 +59,8 @@
 # Convenient shorthand where instead of the following:
 #   `checkpointer = Checkpointer(PyTreeCheckpointer())`
 # we can just use:
 #   `checkpointer = PyTreeCheckpointer()`
 PyTreeCheckpointer = functools.partial(Checkpointer, PyTreeCheckpointHandler())
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.3.0'
+__version__ = '0.3.1'
```

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/abstract_checkpointer.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/abstract_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/aggregate_handlers.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/aggregate_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/array_checkpoint_handler.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,18 +126,14 @@
 
     Returns:
       The restored object.
     """
     del item
     if restore_args is None:
       restore_args = type_handlers.RestoreArgs()
-    if restore_args.lazy:
-      raise ValueError(
-          'Lazy restoration not supported for ArrayCheckpointHandler.'
-      )
 
     if (directory / self._checkpoint_name).is_file():
       result = self._aggregate_handler.deserialize(
           directory / self._checkpoint_name
       )
       result = result[_ELEMENT_KEY]
       if not self._is_supported_type(result):
```

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/async_checkpoint_handler.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/async_checkpointer.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/async_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_handler.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_manager.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     of the checkpoint. If `max_to_keep` is also set, then the retained
     checkpoints will be kept based on their quality, as measured by this
     function.
   best_mode:
     One of ['max', 'min']. The best metric is determine on the basis of this
     value.
   keep_checkpoints_without_metrics:
-    If False, checkpoints with metrics present
+    If False, checkpoints without metrics present
     are eligible for cleanup. Otherwise, they will never be deleted.
   step_prefix:
     If provided, step directories will take the form
     f'{step_prefix}_<step>'. Otherwise, they will simply be an integer <step>.
   step_format_fixed_length:
     If set, formats step with n digits (leading zeros).
     This makes sorting steps easier. Otherwise, step has no leading zeros.
```

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_utils.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,15 +371,17 @@
       )
     else:
       return type_handlers.RestoreArgs(restore_type=restore_type, dtype=dtype)
 
   return jax.tree_util.tree_map(_restore_args, target, axes_tree)
 
 
-def construct_restore_args(target: PyTree, sharding_tree: PyTree) -> PyTree:
+def construct_restore_args(
+    target: PyTree, sharding_tree: PyTree, set_global_shape: bool = True
+) -> PyTree:
   """Creates restore_args given a target PyTree.
 
   This method should be used in conjunction with a CheckpointManager or
   Checkpointer that wraps a PyTreeCheckpointHandler.
 
   For example::
 
@@ -408,28 +410,29 @@
   ignored.
 
   Args:
     target: The returned value will match the structure of `target`, will be
       used to set the desired dtype and restoration shape.
     sharding_tree: A PyTree matching `target` which will be used to set the
       restoration sharding.
+    set_global_shape: If true, set the `global_shape` field of ArrayRestoreArgs.
 
   Returns:
     A PyTree matching target of RestoreArgs (or ArrayRestoreArgs) objects.
   """
 
   def _restore_args(value: Any, sharding: jax.sharding.Sharding):
     restore_type = type(value)
     dtype = None
     if hasattr(value, 'dtype'):
       dtype = value.dtype
     if isinstance(value, jax.Array):
       return type_handlers.ArrayRestoreArgs(
           restore_type=restore_type,
           sharding=sharding,
-          global_shape=value.shape,
+          global_shape=value.shape if set_global_shape else None,
           dtype=value.dtype,
       )
     else:
       return type_handlers.RestoreArgs(restore_type=restore_type, dtype=dtype)
 
   return jax.tree_util.tree_map(_restore_args, target, sharding_tree)
```

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/checkpoint_utils_test.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/checkpointer.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/conftest.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/future.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/json_checkpoint_handler.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/msgpack_utils.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/msgpack_utils_test.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/msgpack_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax_checkpoint-0.3.1/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/proto/__init__.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/proto/testing/__init__.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/proto/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/proto/testing/foo_pb2.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/proto/testing/foo_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,20 +22,18 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\tfoo.proto\x12\x10orbax.checkpoint"9\n\x03\x46oo\x12\x10\n\x03\x62\x61r\x18\x01'
-    b' \x01(\tH\x00\x88\x01\x01\x12\x10\n\x03\x62\x61z\x18\x02'
-    b' \x01(\x05H\x01\x88\x01\x01\x42\x06\n\x04_barB\x06\n\x04_bazb\x06proto3'
+    b'\n\tfoo.proto\x12\x05orbax"\x1f\n\x03\x46oo\x12\x0b\n\x03\x62\x61r\x18\x01'
+    b' \x01(\t\x12\x0b\n\x03\x62\x61z\x18\x02 \x01(\x05'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'foo_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
-  _FOO._serialized_start = 31
-  _FOO._serialized_end = 88
+  _FOO._serialized_start = 20
+  _FOO._serialized_end = 51
 # @@protoc_insertion_point(module_scope)
```

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/proto_checkpoint_handler.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/proto_checkpoint_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
       filename: file name given to the written file.
     """
     self._filename = filename
     self._executor = futures.ThreadPoolExecutor(max_workers=1)
 
   async def async_save(
       self, directory: epath.Path, item: message.Message
-  ) -> List[future.Future]:
+  ) -> Optional[List[future.Future]]:
     """Saves the given proto.
 
     Args:
       directory: save location directory.
       item: the proto to serialize.
 
     Returns:
@@ -65,16 +65,17 @@
     return [self._executor.submit(functools.partial(_save_fn, item))]
 
   def save(self, directory: epath.Path, item: message.Message):
     """Saves the provided item."""
 
     async def async_save(directory, item):
       commit_futures = await self.async_save(directory, item)
-      for f in commit_futures:
-        f.result()
+      if commit_futures:
+        for f in commit_futures:
+          f.result()
 
     asyncio.run(async_save(directory, item))
     utils.sync_global_devices("ProtoCheckpointHandler:save")
 
   def restore(
       self, directory: epath.Path, item: Optional[Type[message.Message]] = None
   ):
```

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/proto_checkpoint_handler_test.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/proto_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,22 +25,19 @@
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental.array_serialization import serialization
 import numpy as np
 from orbax.checkpoint import aggregate_handlers
-from orbax.checkpoint import lazy_utils
-from orbax.checkpoint import proto_checkpoint_handler
 from orbax.checkpoint import transform_utils
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
 from orbax.checkpoint.async_checkpoint_handler import AsyncCheckpointHandler
 from orbax.checkpoint.future import Future
-from orbax.checkpoint.proto import tree_metadata_pb2
 import tensorstore as ts
 
 
 PyTree = Any
 TupleKey = Tuple[str, ...]
 RestoreArgs = type_handlers.RestoreArgs
 ArrayRestoreArgs = type_handlers.ArrayRestoreArgs
@@ -48,18 +45,16 @@
 ParamInfo = type_handlers.ParamInfo
 TypeHandler = type_handlers.TypeHandler
 AggregateHandler = aggregate_handlers.AggregateHandler
 MsgpackHandler = aggregate_handlers.MsgpackHandler
 TransformFn = Callable[[PyTree, PyTree, PyTree], Tuple[PyTree, PyTree]]
 Transform = transform_utils.Transform
 RestoreTransform = transform_utils.RestoreTransform
-LazyValue = lazy_utils.LazyValue
-ProtoCheckpointHandler = proto_checkpoint_handler.ProtoCheckpointHandler
 
-_METADATA_FILE = 'tree_metadata'
+_TYPE_METADATA_FILE = 'type_metadata'
 _CHECKPOINT_FILE = 'checkpoint'
 
 
 async def _create_param_save_dir(param_info: ParamInfo, args: SaveArgs):
   # Directory will be unused.
   path = param_info.path
   if path is None or args.aggregate:
@@ -364,15 +359,14 @@
 @dataclasses.dataclass
 class _BatchRequest:
   """Represents a a request for batched serialization or deserialization."""
   handler: TypeHandler
   values: List[Any]
   infos: List[ParamInfo]
   args: List[Union[SaveArgs, RestoreArgs]]
-  lazy: bool = False
 
 
 def _batched_serialization_requests(
     tree: PyTree, param_infos: PyTree, args: PyTree
 ) -> List[_BatchRequest]:
   """Gets a list of batched serialization or deserialization requests."""
   result = []
@@ -382,19 +376,14 @@
     nonlocal result
     nonlocal grouped
     # Exclude from serialize/deserialize with TypeHandler if aggregated.
     if info.skip_deserialize:
       return
     if isinstance(arg, RestoreArgs):
       handler = type_handlers.get_type_handler(arg.restore_type)
-      # Lazy arguments must be restored individually, rather than as a batch.
-      # Thus, we create an individual _BatchRequest for each one.
-      if arg.lazy:
-        result += [_BatchRequest(handler, [value], [info], [arg], lazy=True)]
-        return
     else:
       handler = type_handlers.get_type_handler(type(value))
     if handler not in grouped:
       grouped[handler] = _BatchRequest(handler, [], [], [])
     request = grouped[handler]
     grouped[handler] = dataclasses.replace(
         request,
@@ -441,16 +430,15 @@
     transforms: Optional[PyTree],
     transforms_default_to_original: bool,
 ) -> PyTree:
   """Optionally transforms the restored PyTree to the structure of `item`.
 
   Args:
     item: a PyTree representing the result structure ("new tree structure").
-    restored: a PyTree representing the original tree structure. Note: this is a
-      tree of LazyValues.
+    restored: a PyTree representing the original tree structure.
     restore_args: tree of RestoreArgs, with the same structure as `item`.
     transforms: provides instructions on how to transform the input trees. See
       transform_utils.
     transforms_default_to_original: See transform_utils.
 
   Returns:
     A transformed PyTree.
@@ -486,40 +474,35 @@
 
   def __init__(
       self,
       aggregate_filename: Optional[str] = None,
       concurrent_gb: int = 96,
       use_ocdbt: bool = False,
       restore_with_serialized_types: bool = True,
-      write_tree_metadata: bool = False,
   ):
     """Creates PyTreeCheckpointHandler.
 
     Args:
       aggregate_filename: name that the aggregated checkpoint should be saved
         as.
       concurrent_gb: max concurrent GB that are allowed to be read.
       use_ocdbt: enables Tensorstore OCDBT driver.
       restore_with_serialized_types: If True, the values with unspecified
         restore types will be restored using the typing information in the
         checkpoint. Otherwise, arrays will be restored as either np.ndarray or
         jax.Array, and will ignore any typing information present in the
         checkpoint.
-      write_tree_metadata: Experimental feature. Do not use. Writes tree
-        metadata in protobuf format.
     """
     self._aggregate_handler = MsgpackHandler()
     if aggregate_filename is None:
       aggregate_filename = _CHECKPOINT_FILE
     self._aggregate_filename = aggregate_filename
     self._concurrent_gb = concurrent_gb
     self._use_ocdbt = use_ocdbt
     self._restore_with_serialized_types = restore_with_serialized_types
-    self._write_tree_metadata = write_tree_metadata
-    self._metadata_handler = ProtoCheckpointHandler(_METADATA_FILE)
 
   def _get_param_names(self, item: PyTree) -> PyTree:
     """Gets parameter names for PyTree elements."""
     return _get_param_names(item)
 
   def _get_param_infos(
       self, item: PyTree, directory: epath.Path, save_args: PyTree
@@ -564,51 +547,14 @@
       save_args: PyTree,
   ) -> Future:
     ser_item = _get_tree_for_aggregation(param_infos, save_args, item)
     return await self._aggregate_handler.serialize(
         directory / self._aggregate_filename, ser_item
     )
 
-  async def _write_metadata_file(
-      self,
-      directory: epath.Path,
-      item: PyTree,
-  ) -> List[Future]:
-    if not self._write_tree_metadata:
-      return []
-    flat_with_keys, _ = jax.tree_util.tree_flatten_with_path(
-        item, is_leaf=utils.is_empty_or_leaf
-    )
-    tree_metadata = tree_metadata_pb2.TreeMetadata()
-    for keypath, _ in flat_with_keys:
-      kv = tree_metadata.structure.add()
-      for k in keypath:
-        proto_k = kv.key.add()
-        proto_k.name = str(utils.get_key_name(k))
-        proto_k.type = utils.get_key_metadata_type(k)
-      value_metadata = kv.value
-      # TODO(b/289245667): Placeholder value.
-      value_metadata.type = 'None'
-    return await self._metadata_handler.async_save(directory, tree_metadata)
-
-  def _read_metadata_file(
-      self,
-      directory: epath.Path,
-  ) -> PyTree:
-    tree_metadata = self._metadata_handler.restore(
-        directory, tree_metadata_pb2.TreeMetadata
-    )
-    tree_metadata = typing.cast(tree_metadata_pb2.TreeMetadata, tree_metadata)
-    flat = []
-    for kv_pair in tree_metadata.structure:
-      keys, value = (kv_pair.key, kv_pair.value)
-      keypath = tuple([utils.keypath_from_key_metadata(key) for key in keys])
-      flat.append((keypath, value))
-    return utils.from_flattened_with_keypath(flat)
-
   async def async_save(
       self,
       directory: epath.Path,
       item: PyTree,
       save_args: Optional[PyTree] = None) -> Optional[List[Future]]:
     """Saves a PyTree from a given training step.
 
@@ -628,16 +574,14 @@
       save_args: a PyTree matching `item` which consists of SaveArgs objects as
         values.
 
     Returns:
       A Future that will commit the data to `directory` when awaited. Copying
       the data from its source will be awaited in this function.
     """
-    item = await lazy_utils.maybe_get_tree_async(item)
-
     # Because of empty states, the user-provided args may not contain
     # all necessary arguments. These should be filled in with default args.
     save_args = jax.tree_util.tree_map(
         _maybe_set_default_save_args,
         item,
         item if save_args is None else save_args,
         is_leaf=utils.is_empty_or_leaf,
@@ -671,19 +615,18 @@
                 request.values, request.infos, request.args
             )
         ]
       # Await copy futures. Returns list of lists.
       commit_futures = await asyncio.gather(*serialize_ops)
       commit_futures, _ = jax.tree_util.tree_flatten(commit_futures)
 
-    metadata_commit_futures = await self._write_metadata_file(directory, item)
     aggregate_commit_future = await self._write_aggregate_file(
         directory, item, param_infos, save_args
     )
-    return commit_futures + [aggregate_commit_future] + metadata_commit_futures
+    return commit_futures + [aggregate_commit_future]
 
   def save(self, directory: epath.Path, item: Any, *args, **kwargs):
     """Saves the provided item.
 
     Blocks until both copy and commit complete.
 
     See async_save.
@@ -712,48 +655,29 @@
     """Deserializes values or gets them from the aggregate file."""
 
     # Handle parameters from aggregate file.
     def _process_aggregated_value(info, value, args):
       if info.skip_deserialize:
         value = _try_array_cast(value, args.dtype)
         value = _maybe_shard_array(value, args)
-      if args.lazy:
-        value = LazyValue(lazy_utils.identity(value))
       return value
 
-    def _lazy_get_fn(handler, infos, args):
-      async def _get_singular_value_from_handler():
-        result = await handler.deserialize(infos, args)
-        assert len(result) == 1
-        return result[0]
-
-      return _get_singular_value_from_handler
-
     structure = jax.tree_util.tree_map(
         _process_aggregated_value, param_infos, structure, restore_args
     )
 
     batch_requests = _batched_serialization_requests(
         structure, param_infos, restore_args
     )
     deserialized_batches = []
     deserialized_batches_ops = []
     for request in batch_requests:
-      if request.lazy:
-        deserialized_batches.append(
-            [
-                LazyValue(
-                    _lazy_get_fn(request.handler, request.infos, request.args)
-                )
-            ]
-        )
-      else:
-        deserialized_batches_ops.append(
-            request.handler.deserialize(request.infos, request.args)
-        )
+      deserialized_batches_ops.append(
+          request.handler.deserialize(request.infos, request.args)
+      )
     deserialized_batches += await asyncio.gather(*deserialized_batches_ops)
 
     flat_restored = utils.to_flat_dict(structure, sep='.')
     for request, deserialized in zip(batch_requests, deserialized_batches):
       for info, value in zip(request.infos, deserialized):
         flat_restored[info.name] = value
 
@@ -791,16 +715,15 @@
       transform_fn: WARNING: NOT GENERALLY SUPPORTED. A function which accepts
         the `item` argument, a PyTree checkpoint structure and a PyTree of
         ParamInfos based on the checkpoint. Returns a transformed PyTree
         matching the desired return tree structure, and a matching ParamInfo
         tree.
 
     Returns:
-      A PyTree matching the structure of `item`. If `lazy` restoration is
-      enabled, leaves will be returned as `LazyValue`.
+      A PyTree matching the structure of `item`.
 
     Raises:
       FileNotFoundError: `directory` does not exist or is missing required files
       ValueError: `transforms` is provided without `item`.
       ValueError: `transforms` contains elements with `multi_value_fn`.
     """
     if not directory.exists():
@@ -882,8 +805,7 @@
             directory,
         )
         return utils.pytree_structure(directory)
 
   def close(self):
     """See superclass documentation."""
     self._aggregate_handler.close()
-    self._metadata_handler.close()
```

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/test_utils.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 from etils import epath
 import jax
 from jax import sharding
 from jax.experimental import pjit
 import jax.numpy as jnp
 import numpy as np
-from orbax.checkpoint import lazy_utils
 from orbax.checkpoint import pytree_checkpoint_handler
 from orbax.checkpoint import utils
 
 
 def save_fake_tmp_dir(
     directory: epath.Path,
     step: int,
@@ -77,19 +76,14 @@
     return pjit.pjit(function)(arr)
 
   return jax.tree_util.tree_map(f, tree)
 
 
 def assert_array_equal(testclass, v_expected, v_actual):
   """Asserts that two arrays are equal."""
-  if isinstance(v_expected, lazy_utils.LazyValue):
-    testclass.assertIsInstance(v_actual, lazy_utils.LazyValue)
-    v_expected = v_expected.get()
-    v_actual = v_actual.get()
-
   testclass.assertIsInstance(v_actual, type(v_expected))
   if isinstance(v_expected, jax.Array):
     testclass.assertEqual(
         len(v_expected.addressable_shards), len(v_actual.addressable_shards)
     )
     for shard_expected, shard_actual in zip(
         v_expected.addressable_shards, v_actual.addressable_shards
```

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/transform_utils.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/transform_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/transform_utils_test.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/type_handlers.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/type_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,27 +182,23 @@
   dtype: Optional[jnp.dtype] = None
 
 
 @dataclasses.dataclass
 class RestoreArgs:
   """Extra arguments that can be provided for restoration.
 
-  lazy:
-    If True, restores using LazyArray. The actual read operation will not be
-    performed until `get` is called for the restored LazyArray.
   restore_type:
     Specifies the object type of the restored parameter. The type
     must have a corresponding TypeHandler for restoration. Ignored if the
     parameter is restored from an aggregated checkpoint file.
   dtype:
     If provided, casts the parameter to the given dtype after restoring.
     Note that the parameter must be compatible with the given type (e.g.
     jnp.bfloat16 is not compatible with np.ndarray).
   """
-  lazy: bool = False
   # TODO(b/253238305) Consider deprecating this in favor of saving type
   # information in checkpoint metadata.
   restore_type: Any = np.ndarray
   dtype: Optional[jnp.dtype] = None
 
 
 class TypeHandler(abc.ABC):
```

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/utils.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,14 @@
 from typing import Any, List, Optional, Tuple, Union
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental import multihost_utils
 import numpy as np
-from orbax.checkpoint.proto import tree_metadata_pb2
-
 
 TMP_DIR_SUFFIX = '.orbax-checkpoint-tmp-'
 # prefix_1000.orbax-checkpoint-tmp-1010101
 # OR
 # 1000.orbax-checkpoint-tmp-1010101
 TMP_DIR_STEP_PATTERN = r'.*?_*?(\d+)\.orbax-checkpoint-tmp-\d+'
 # TODO(b/260759189): Deprecate this prefix when no longer in use by JAX MG.
@@ -95,29 +93,22 @@
   return _wrap(path.mkdir)(*args, parents=parents, exist_ok=exist_ok, **kwargs)
 
 
 def async_write_bytes(path: epath.Path, data: Any):
   return _wrap(path.write_bytes)(data)
 
 
-def async_write_text(path: epath.Path, data: Any):
-  return _wrap(path.write_text)(data)
-
-
 def async_exists(path: epath.Path):
   return _wrap(path.exists)()
 
 
 class EmptyNode:
   pass
 
 
-# TODO(b/289258695): Refactor many of the following functions into tree_util.py.
-
-
 def is_empty_or_leaf(x: Any) -> bool:
   try:
     children, _ = jax._src.tree_util.flatten_one_level(x)  # pylint: disable=protected-access
   except ValueError:
     return True  # Cannot flatten x; means it must be a leaf
   return not children
 
@@ -132,43 +123,14 @@
     return key.name
   elif isinstance(key, jax.tree_util.FlattenedIndexKey):
     return key.key
   else:
     raise ValueError(f'Unsupported KeyEntry: {type(key)}: "{key}"')
 
 
-def get_key_metadata_type(
-    key: Any,
-) -> tree_metadata_pb2.TreeMetadata.KeyValuePair.Key.KeyType:
-  """Translates the JAX key class into a proto enum."""
-  if isinstance(
-      key, (jax.tree_util.SequenceKey, jax.tree_util.FlattenedIndexKey)
-  ):
-    return tree_metadata_pb2.TreeMetadata.KeyValuePair.Key.KeyType.SEQUENCE
-  elif isinstance(key, (jax.tree_util.DictKey, jax.tree_util.GetAttrKey)):
-    return tree_metadata_pb2.TreeMetadata.KeyValuePair.Key.KeyType.DICT
-  else:
-    raise ValueError(f'Unsupported KeyEntry: {type(key)}: "{key}"')
-
-
-def keypath_from_key_metadata(
-    key: tree_metadata_pb2.TreeMetadata.KeyValuePair.Key,
-) -> Any:
-  """Converts from Key in TreeMetadata to JAX keypath class."""
-  if (
-      key.type
-      == tree_metadata_pb2.TreeMetadata.KeyValuePair.Key.KeyType.SEQUENCE
-  ):
-    return jax.tree_util.SequenceKey(int(key.name))
-  elif key.type == tree_metadata_pb2.TreeMetadata.KeyValuePair.Key.KeyType.DICT:
-    return jax.tree_util.DictKey(key.name)
-  else:
-    raise ValueError(f'Unsupported KeyEntry: {key.type}')
-
-
 def _is_dict_key(key) -> bool:
   return isinstance(key, (jax.tree_util.DictKey, jax.tree_util.GetAttrKey))
 
 
 def _is_sequence_key(key) -> bool:
   return isinstance(
       key, (jax.tree_util.FlattenedIndexKey, jax.tree_util.SequenceKey)
@@ -182,67 +144,14 @@
 def _extend_list(ls, idx, nextvalue):
   assert idx <= len(ls)
   if idx == len(ls):
     ls.append(nextvalue)
   return ls
 
 
-def from_flattened_with_keypath(flat_with_keys: PyTree) -> PyTree:
-  """Reconstructs a tree given the a flat dict with keypaths."""
-  # Accesses the first path element (arbitrary), first tuple element
-  # (keypath tuple), first key in keypath (outermost key in the PyTree).
-  outerkey = flat_with_keys[0][0][0]
-  if _is_dict_key(outerkey):
-    result = {}
-  elif _is_sequence_key(outerkey):
-    result = []
-  else:
-    result = None
-    _raise_unsupported_key_error(outerkey)
-
-  for keypath, value in flat_with_keys:
-    subtree = result
-    for i, key in enumerate(keypath):
-      if i == 0:
-        assert isinstance(key, type(outerkey))
-      if i == len(keypath) - 1:
-        if _is_dict_key(key):
-          assert isinstance(subtree, dict)
-          subtree[get_key_name(key)] = value
-        elif _is_sequence_key(key):
-          assert isinstance(subtree, list)
-          idx = get_key_name(key)
-          subtree = _extend_list(subtree, idx, value)
-      else:
-        nextkey = keypath[i + 1]
-        if _is_dict_key(nextkey):
-          nextvalue = {}
-        elif _is_sequence_key(nextkey):
-          nextvalue = []
-        else:
-          nextvalue = None
-          _raise_unsupported_key_error(nextkey)
-
-        if _is_dict_key(key):
-          assert isinstance(subtree, dict)
-          name = get_key_name(key)
-          if name not in subtree:
-            subtree[name] = nextvalue
-          subtree = subtree[name]
-        elif _is_sequence_key(key):
-          assert isinstance(subtree, list)
-          idx = get_key_name(key)
-          subtree = _extend_list(subtree, idx, nextvalue)
-          subtree = subtree[idx]
-        else:
-          _raise_unsupported_key_error(key)
-
-  return result
-
-
 def to_flat_dict(
     tree: PyTree, sep: Optional[str] = None, keep_empty_nodes: bool = False
 ) -> PyTree:
   """Converts a tree into a flattened dictionary.
 
   The nested keys are flattened to a tuple.
 
@@ -286,15 +195,63 @@
 
   Returns:
     The serialized PyTree.
   """
   flat_with_keys, _ = jax.tree_util.tree_flatten_with_path(
       tree, is_leaf=is_empty_or_leaf if keep_empty_nodes else None
   )
-  return from_flattened_with_keypath(flat_with_keys)
+  # Accesses the first path element (arbitrary), first tuple element
+  # (keypath tuple), first key in keypath (outermost key in the PyTree).
+  outerkey = flat_with_keys[0][0][0]
+  if _is_dict_key(outerkey):
+    result = {}
+  elif _is_sequence_key(outerkey):
+    result = []
+  else:
+    result = None
+    _raise_unsupported_key_error(outerkey)
+
+  for keypath, value in flat_with_keys:
+    subtree = result
+    for i, key in enumerate(keypath):
+      if i == 0:
+        assert isinstance(key, type(outerkey))
+      if i == len(keypath) - 1:
+        if _is_dict_key(key):
+          assert isinstance(subtree, dict)
+          subtree[get_key_name(key)] = value
+        elif _is_sequence_key(key):
+          assert isinstance(subtree, list)
+          idx = get_key_name(key)
+          subtree = _extend_list(subtree, idx, value)
+      else:
+        nextkey = keypath[i + 1]
+        if _is_dict_key(nextkey):
+          nextvalue = {}
+        elif _is_sequence_key(nextkey):
+          nextvalue = []
+        else:
+          nextvalue = None
+          _raise_unsupported_key_error(nextkey)
+
+        if _is_dict_key(key):
+          assert isinstance(subtree, dict)
+          name = get_key_name(key)
+          if name not in subtree:
+            subtree[name] = nextvalue
+          subtree = subtree[name]
+        elif _is_sequence_key(key):
+          assert isinstance(subtree, list)
+          idx = get_key_name(key)
+          subtree = _extend_list(subtree, idx, nextvalue)
+          subtree = subtree[idx]
+        else:
+          _raise_unsupported_key_error(key)
+
+  return result
 
 
 def deserialize_tree(
     serialized: PyTree, target: PyTree, keep_empty_nodes: bool = False
 ) -> PyTree:
   """Deserializes a PyTree to the same structure as `target`."""
```

### Comparing `orbax_checkpoint-0.3.0/orbax/checkpoint/utils_test.py` & `orbax_checkpoint-0.3.1/orbax/checkpoint/utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/pyproject.toml` & `orbax_checkpoint-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.0/PKG-INFO` & `orbax_checkpoint-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.3.0
+Version: 0.3.1
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

