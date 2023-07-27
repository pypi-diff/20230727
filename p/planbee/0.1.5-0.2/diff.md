# Comparing `tmp/planbee-0.1.5.tar.gz` & `tmp/planbee-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planbee-0.1.5.tar", last modified: Fri Jul 14 10:08:03 2023, max compression
+gzip compressed data, was "planbee-0.2.tar", last modified: Thu Jul 27 13:31:32 2023, max compression
```

## Comparing `planbee-0.1.5.tar` & `planbee-0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 10:07:58.000000 planbee-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-14 10:08:03.381983 planbee-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-14 10:07:58.000000 planbee-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-14 10:08:03.381983 planbee-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-14 10:07:58.000000 planbee-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee/models/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/models/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee/scheduler/heuristic_solver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/heuristic_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/heuristic_solver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/heuristic_solver/task_allocator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/heuristic_solver/window_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/scheduler_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/task_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/task_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 10:07:58.000000 planbee-0.1.5/src/planbee/scheduler/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:08:03.381983 planbee-0.1.5/src/planbee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 10:08:03.000000 planbee-0.1.5/src/planbee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:32.935220 planbee-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-27 13:31:29.000000 planbee-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-27 13:31:32.939220 planbee-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-27 13:31:29.000000 planbee-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-27 13:31:32.939220 planbee-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-27 13:31:29.000000 planbee-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:32.927220 planbee-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:32.939220 planbee-0.2/src/planbee/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 13:31:32.939220 planbee-0.2/src/planbee/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:32.935220 planbee-0.2/src/planbee/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/models/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:32.935220 planbee-0.2/src/planbee/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/scheduler/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:32.935220 planbee-0.2/src/planbee/scheduler/heuristic_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/scheduler/heuristic_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/scheduler/heuristic_solver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/scheduler/heuristic_solver/task_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/scheduler/heuristic_solver/window_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/scheduler/scheduler_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/scheduler/task_batch_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/scheduler/task_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 13:31:29.000000 planbee-0.2/src/planbee/scheduler/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:31:32.931220 planbee-0.2/src/planbee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-27 13:31:32.000000 planbee-0.2/src/planbee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-27 13:31:32.000000 planbee-0.2/src/planbee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:31:32.000000 planbee-0.2/src/planbee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:31:32.000000 planbee-0.2/src/planbee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 13:31:32.000000 planbee-0.2/src/planbee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 13:31:32.000000 planbee-0.2/src/planbee.egg-info/top_level.txt
```

### Comparing `planbee-0.1.5/LICENSE` & `planbee-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `planbee-0.1.5/PKG-INFO` & `planbee-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planbee
-Version: 0.1.5
+Version: 0.2
 Summary: production / job shop / resource scheduler for Python
 Home-page: https://github.com/Yacobolo/PlanBee
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 License: UNKNOWN
 Description: # PlanBee 🐝
```

### Comparing `planbee-0.1.5/README.md` & `planbee-0.2/README.md`

 * *Files identical despite different names*

### Comparing `planbee-0.1.5/setup.py` & `planbee-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.5/src/planbee/models/resource.py` & `planbee-0.2/src/planbee/models/resource.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.5/src/planbee/models/task.py` & `planbee-0.2/src/planbee/models/task.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,99 @@
 from itertools import count
-from typing import Optional, Union
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, Field, PrivateAttr, validator
 
 from .resource import Resource
 
 
 class Task(BaseModel):
-    id: Union[int, str]
-    duration: int
-    priority: int
+    id: int | str
+    duration: int = Field(gt=0)
+    priority: int = Field(gt=0)
     resources: list[set[Resource]]
-    resource_count: Union[int, str] = 1
-    predecessors: Optional[list["Task"]] = []
-    predecessor_delay: int = 0
-    batch_size: Optional[int] = None
-    quantity: Optional[int] = None
-    batch_id: Optional[int] = None
+    resource_count: int | str = 1
+    predecessors: list["Task"] = []
+    predecessor_delay: int = Field(0, gt=0)
+    batch_size: int = Field(None, gt=0)
+    quantity: int = Field(None, gt=0)
+    _batch_id: int = PrivateAttr(None)
+
+    @property
+    def uid(self) -> str:
+        """returns the unique id of the task"""
+        if self.batch_id is None:
+            return str(self.id)
+        else:
+            return f"{self.id}-{self.batch_id}"
+
+    @property
+    def batch_id(self):
+        """returns the batch id of the task"""
+        return self._batch_id
+
+    def __hash__(self):
+        return hash(self.uid)
+
+    def __eq__(self, other):
+        if isinstance(other, Task):
+            return self.uid == other.uid
+        return False
 
     @validator("resources", pre=True)
     def ensure_list(cls, v):
+        """ensures that the resources are in the form of a list of lists"""
         if not isinstance(v, list):  # if a single resource object is passed
             return [[v]]  # make it a list of list
         if (
             isinstance(v, list) and len(v) > 0 and not isinstance(v[0], list)
         ):  # if a list of resources is passed
             return [v]  # make it a list of list
         return v  # if a list of lists is passed, return as it is
 
+    @validator("resource_count", always=True)
+    def set_resource_count(cls, v, values):
+        """
+        sets the resource count of the task. If resource_count is set to "all", it is
+        set to the maximum number of resources in any resource group
+        """
+        if isinstance(v, str) and v.lower() == "all":
+            if "resources" in values:
+                return max(
+                    len(resource_group) for resource_group in values["resources"]
+                )
+
+        elif isinstance(v, int):
+            return v
+        else:
+            raise ValueError("Invalid value for resource_count.")
+
+    def set_batch_id(self, batch_id):
+        """sets the batch id of the task"""
+        self._batch_id = batch_id
+
     def get_resources(self):
+        """returns a list of all resources required for the task"""
         return [
             resource for resource_list in self.resources for resource in resource_list
         ]
 
     def get_resource_group_count(self):
+        """returns the number of resource groups required for the task"""
         return len(self.resources)
 
     def get_resource_group_indices(self) -> list[list[int]]:
         """
         returns a list of lists of indices of resources in each resource group
         """
         counter = count()
         return [[next(counter) for _ in sublist] for sublist in self.resources]
 
-    @validator("resource_count", always=True)
-    def set_resource_count(cls, v, values):
-        if isinstance(v, str) and v.lower() == "all":
-            if "resources" in values:
-                return max(
-                    len(resource_group) for resource_group in values["resources"]
-                )
-
-        elif isinstance(v, int):
-            return v
-        else:
-            raise ValueError("Invalid value for resource_count.")
+    def is_splittable(self):
+        """
+        Checks if the task is splittable into batches.
+        """
+        return (
+            self.batch_size is not None
+            and self.quantity is not None
+            and self.batch_size > 0
+            and self.quantity > self.batch_size
+        )
```

### Comparing `planbee-0.1.5/src/planbee/scheduler/heuristic_solver/main.py` & `planbee-0.2/src/planbee/scheduler/heuristic_solver/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,103 @@
 import numpy as np
 
+from ...models import Resource, Task
 from .task_allocator import TaskAllocator
 from .window_manager import WindowManager
 
 
 class HeuristicSolver:
-    def __init__(self, tasks, resources, task_order):
-        self.task_allocator = TaskAllocator()
+    def __init__(
+        self,
+        task_dict: dict[str, Task],
+        resources: set[Resource],
+        task_order: list[str],
+    ):
+        self.task_dict = task_dict
         self.task_order = task_order
+        self.task_allocator = TaskAllocator()
         self.window_manager = WindowManager(resources)
         self.task_vars = {
-            task.id: {
-                "task_id": task.id,
+            task_uid: {
+                "task_uid": task_uid,
                 "assigned_resource_ids": None,
                 "task_start": None,
                 "task_end": None,
                 "resource_intervals": None,
             }
-            for task in tasks
+            for task_uid in self.task_dict.keys()
         }
-        self.task_dict = {task.id: task for task in tasks}
 
     def solve(self):
         unscheduled_tasks = []
 
-        for task_id in self.task_order:
-            task = self.task_dict[task_id]
+        for task_uid in self.task_order:
+            task = self.task_dict[task_uid]
 
             # get task resources and windows dict
             task_resource_ids = np.array(
                 [resource.id for resource in task.get_resources()]
             )
 
             task_earliest_start = self._get_task_earliest_start(task)
 
             if task_earliest_start is None:
-                unscheduled_tasks.append(task_id)
+                unscheduled_tasks.append(task_uid)
                 continue
 
             task_resource_windows = self.window_manager.get_task_resource_windows(
                 task_resource_ids, task_earliest_start
             )
             if not task_resource_windows:
-                unscheduled_tasks.append(task_id)
+                unscheduled_tasks.append(task_uid)
                 continue
 
             # allocate task
             allocated_resource_windows_dict = self.task_allocator.allocate_task(
                 resource_windows=task_resource_windows,
                 resource_ids=task_resource_ids,
                 task_duration=task.duration,
                 resource_count=task.resource_count,
                 resource_group_indices=task.get_resource_group_indices(),
             )
 
             if not allocated_resource_windows_dict:
-                unscheduled_tasks.append(task_id)
+                unscheduled_tasks.append(task_uid)
                 continue
 
             resource_windows_min_max = self.min_max_dict_np(
                 allocated_resource_windows_dict
             )
 
             # update resource windows
             self.window_manager.update_resource_windows(resource_windows_min_max)
 
             # Append task values
             task_values = {
-                "task_id": task_id,
+                "task_uid": task_uid,
                 "assigned_resource_ids": list(allocated_resource_windows_dict.keys()),
                 "task_start": min(
                     start for start, _ in resource_windows_min_max.values()
                 ),
                 "task_end": max(end for _, end in resource_windows_min_max.values()),
                 "resource_intervals": allocated_resource_windows_dict.values(),
             }
-            self.task_vars[task_id] = task_values
+            self.task_vars[task_uid] = task_values
 
         return list(
             self.task_vars.values()
         )  # Return values of the dictionary as a list
 
     def _get_task_earliest_start(self, task):
         """
         Retuns the earliest start of a task based on the latest end of its predecessors.
         """
         task_ends = []
         for pred in task.predecessors:
-            task_end = self.task_vars[pred.id]["task_end"]
+            task_end = self.task_vars[pred.uid]["task_end"]
             if task_end is None:
                 return None
             task_ends.append(task_end + task.predecessor_delay)
 
         return max(task_ends, default=0)
 
     def min_max_dict_np(self, d):
```

### Comparing `planbee-0.1.5/src/planbee/scheduler/heuristic_solver/task_allocator.py` & `planbee-0.2/src/planbee/scheduler/heuristic_solver/task_allocator.py`

 * *Files identical despite different names*

### Comparing `planbee-0.1.5/src/planbee/scheduler/heuristic_solver/window_manager.py` & `planbee-0.2/src/planbee/scheduler/heuristic_solver/window_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,19 +89,17 @@
             slopes,
             trim_start,
             trim_end,
             start_idx,
             end_idx,
         )
         window = self._handle_mask_end(
-            window, overlap_windows, mask_end, slopes, trim_start, end_idx
-        )
-        window = self._handle_mask_start(
-            window, overlap_windows, mask_start, slopes, trim_end
+            window, overlap_windows, mask_end, trim_start, end_idx
         )
+        window = self._handle_mask_start(window, overlap_windows, mask_start, trim_end)
         window = self._delete_overlapped_windows(
             window, mask_delete, start_idx, end_idx
         )
 
         return window
 
     def _calculate_slopes(self, windows: np.ndarray) -> np.ndarray:
@@ -145,49 +143,45 @@
         return windows
 
     def _handle_mask_end(
         self,
         windows: np.ndarray,
         overlap_windows: np.ndarray,
         mask_end: np.ndarray,
-        slopes: np.ndarray,
         trim_start: int,
         end_idx: int,
     ) -> np.ndarray:
         """
         Handles the case where mask_end is True.
         """
         if np.any(mask_end):
-            slopes_end = slopes[mask_end]
             overlap_windows[mask_end, 1] = trim_start
             overlap_windows[mask_end, 2] = (
                 overlap_windows[mask_end, 1] - overlap_windows[mask_end, 0]
-            ) * slopes_end
+            )
             end_idx_temp = min(end_idx, windows.shape[0] - 1)  # handle out of bounds
             windows[end_idx_temp, 3] = -1
 
         return windows
 
     def _handle_mask_start(
         self,
         windows: np.ndarray,
         overlap_windows: np.ndarray,
         mask_start: np.ndarray,
-        slopes: np.ndarray,
         trim_end: int,
     ) -> np.ndarray:
         """
         Handles the case where mask_start is True.
         """
         if np.any(mask_start):
-            slopes_start = slopes[mask_start]
             overlap_windows[mask_start, 0] = trim_end
             overlap_windows[mask_start, 2] = (
                 overlap_windows[mask_start, 1] - overlap_windows[mask_start, 0]
-            ) * slopes_start
+            )
             overlap_windows[mask_start, 3] = -1
 
         return windows
 
     def _delete_overlapped_windows(
         self, windows: np.ndarray, mask_delete: np.ndarray, start_idx: int, end_idx: int
     ) -> np.ndarray:
```

### Comparing `planbee-0.1.5/src/planbee/scheduler/scheduler_result.py` & `planbee-0.2/src/planbee/scheduler/scheduler_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import seaborn as sns
 
 
 class SchedulerResult:
     def __init__(self, task_vars):
         self.task_vars = task_vars
         self.unscheduled_tasks = [
-            task["task_id"]
+            task["task_uid"]
             for task in self.task_vars
             if task["assigned_resource_ids"] is None
         ]
 
     def to_dict(self):
         return self.task_vars
 
@@ -26,39 +26,39 @@
             summary += f"\nNo available resources found for task ids: {', '.join(map(str, self.unscheduled_tasks))}"
         return summary
 
     def plot_resource_plan(self) -> None:
         df = self.get_resource_intervals_df()
 
         # Create a color dictionary for each unique resource for distinction in the plot
-        tasks = df["task_id"].unique()
+        tasks = df["task_uid"].unique()
         colors = sns.color_palette(
             "deep", len(tasks)
         )  # Using seaborn "dark" color palette
         color_dict = dict(zip(tasks, colors))
 
         # Set seaborn style
         sns.set_style("whitegrid")
 
         plt.figure(figsize=(12, 6))
 
-        for task_id, group_df in df.groupby("task_id"):
+        for task_uid, group_df in df.groupby("task_uid"):
             for task in group_df.itertuples():
                 plt.barh(
                     task.resource_id,
                     left=task.interval_start,
                     width=task.interval_end - task.interval_start,
-                    color=color_dict[task_id],
+                    color=color_dict[task_uid],
                     edgecolor="black",
                 )
                 plt.text(
                     x=(task.interval_start + task.interval_end)
                     / 2,  # x position, in the middle of task bar
                     y=task.resource_id,  # y position, on the resource line
-                    s=task.task_id,  # text string, which is task_id here
+                    s=task.task_uid,  # text string, which is task_uid here
                     va="center",  # vertical alignment
                     ha="center",  # horizontal alignment
                     color="black",  # text color
                     fontsize=10,
                 )  # font size
 
         plt.xlabel("Time")
@@ -73,10 +73,10 @@
         df = df.explode(["assigned_resource_ids", "resource_intervals"]).explode(
             "resource_intervals"
         )
         df = df.dropna()
         df["interval_start"] = df.resource_intervals.apply(lambda x: x[0])
         df["interval_end"] = df.resource_intervals.apply(lambda x: x[1])
         df = df.rename(columns={"assigned_resource_ids": "resource_id"})
-        df = df[["task_id", "resource_id", "interval_start", "interval_end"]]
+        df = df[["task_uid", "resource_id", "interval_start", "interval_end"]]
         df = df.infer_objects()
         return df
```

### Comparing `planbee-0.1.5/src/planbee/scheduler/task_graph.py` & `planbee-0.2/src/planbee/scheduler/task_graph.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import networkx as nx
 
+from ..models import Task
+
 
 class TaskGraph:
-    def __init__(self, tasks):
-        self.tasks = {task.id: task for task in tasks}
+    def __init__(self, tasks_dict: dict[str, Task]):
+        self.tasks_dict = tasks_dict
         self.graph = self._create_task_graph()
 
     def _create_task_graph(self):
         """
         Creates a directed acyclic graph from the given tasks.
         """
         task_graph = nx.DiGraph()
-        for task in self.tasks.values():
-            task_graph.add_node(task.id, duration=task.duration, priority=task.priority)
+        for task in self.tasks_dict.values():
+            task_graph.add_node(
+                task.uid, duration=task.duration, priority=task.priority
+            )
             for predecessor in task.predecessors:
-                task_graph.add_edge(predecessor.id, task.id)
+                task_graph.add_edge(predecessor.uid, task.uid)
         return task_graph
 
     def _compute_longest_paths(self):
         """
         Computes the longest path for each node in the task graph using a topological
         sort.
         """
-        longest_path = {task_id: 0 for task_id in self.tasks}
+        longest_path = {task_uid: 0 for task_uid in self.tasks_dict}
         for task in nx.topological_sort(self.graph):
             duration = self.graph.nodes[task]["duration"]
             for predecessor in self.graph.predecessors(task):
                 longest_path[task] = max(
                     longest_path[task], longest_path[predecessor] + duration
                 )
         return longest_path
@@ -50,18 +54,18 @@
                     key=lambda n: (self.graph.nodes[n]["priority"], -longest_path[n]),
                 )
                 for predecessor in predecessors:
                     visit(predecessor)
                 result.append(node)
 
         for task in sorted(
-            self.tasks.values(),
-            key=lambda t: (self.graph.nodes[t.id]["priority"], -longest_path[t.id]),
+            self.tasks_dict.values(),
+            key=lambda t: (self.graph.nodes[t.uid]["priority"], -longest_path[t.uid]),
         ):
-            visit(task.id)
+            visit(task.uid)
 
         return result
 
     def get_task_order(self):
         """
         Returns a list of task IDs in the order required to complete them as quickly
         as possible while considering task priorities.
```

### Comparing `planbee-0.1.5/src/planbee.egg-info/PKG-INFO` & `planbee-0.2/src/planbee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planbee
-Version: 0.1.5
+Version: 0.2
 Summary: production / job shop / resource scheduler for Python
 Home-page: https://github.com/Yacobolo/PlanBee
 Author: Jacob Østergaard Nielsen
 Author-email: jaoe@oestergaard-as.dk
 License: UNKNOWN
 Description: # PlanBee 🐝
```

### Comparing `planbee-0.1.5/src/planbee.egg-info/SOURCES.txt` & `planbee-0.2/src/planbee.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 src/planbee.egg-info/top_level.txt
 src/planbee/models/__init__.py
 src/planbee/models/resource.py
 src/planbee/models/task.py
 src/planbee/scheduler/__init__.py
 src/planbee/scheduler/core.py
 src/planbee/scheduler/scheduler_result.py
+src/planbee/scheduler/task_batch_processor.py
 src/planbee/scheduler/task_graph.py
-src/planbee/scheduler/task_preprocessor.py
 src/planbee/scheduler/visualizations.py
 src/planbee/scheduler/heuristic_solver/__init__.py
 src/planbee/scheduler/heuristic_solver/main.py
 src/planbee/scheduler/heuristic_solver/task_allocator.py
 src/planbee/scheduler/heuristic_solver/window_manager.py
```

