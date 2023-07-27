# Comparing `tmp/kaiju_tasks-2.1.7-py3-none-any.whl.zip` & `tmp/kaiju_tasks-2.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18801 bytes, number of entries: 12
--rw-r--r--  2.0 unx      151 b- defN 23-Jul-27 19:42 kaiju_tasks/__init__.py
--rw-r--r--  2.0 unx     5386 b- defN 23-Jul-27 19:42 kaiju_tasks/gui.py
--rw-r--r--  2.0 unx    40431 b- defN 23-Jul-27 19:42 kaiju_tasks/services.py
--rw-r--r--  2.0 unx     6161 b- defN 23-Jul-27 19:42 kaiju_tasks/types.py
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-27 19:42 kaiju_tasks/tests/__init__.py
--rw-r--r--  2.0 unx     2272 b- defN 23-Jul-27 19:42 kaiju_tasks/tests/fixtures.py
--rw-r--r--  2.0 unx    15554 b- defN 23-Jul-27 19:42 kaiju_tasks/tests/test_tasks.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-27 19:43 kaiju_tasks-2.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     3212 b- defN 23-Jul-27 19:43 kaiju_tasks-2.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 19:43 kaiju_tasks-2.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-27 19:43 kaiju_tasks-2.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      976 b- defN 23-Jul-27 19:43 kaiju_tasks-2.1.7.dist-info/RECORD
-12 files, 74899 bytes uncompressed, 17163 bytes compressed:  77.1%
+Zip file size: 19012 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      151 b- defN 23-Jul-27 19:57 kaiju_tasks/__init__.py
+-rw-r--r--  2.0 unx     6119 b- defN 23-Jul-27 19:57 kaiju_tasks/gui.py
+-rw-r--r--  2.0 unx    40431 b- defN 23-Jul-27 19:57 kaiju_tasks/services.py
+-rw-r--r--  2.0 unx     6161 b- defN 23-Jul-27 19:57 kaiju_tasks/types.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-27 19:57 kaiju_tasks/tests/__init__.py
+-rw-r--r--  2.0 unx     2272 b- defN 23-Jul-27 19:57 kaiju_tasks/tests/fixtures.py
+-rw-r--r--  2.0 unx    15554 b- defN 23-Jul-27 19:57 kaiju_tasks/tests/test_tasks.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-27 19:57 kaiju_tasks-2.1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3212 b- defN 23-Jul-27 19:57 kaiju_tasks-2.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 19:57 kaiju_tasks-2.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-27 19:57 kaiju_tasks-2.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jul-27 19:57 kaiju_tasks-2.1.8.dist-info/RECORD
+12 files, 75632 bytes uncompressed, 17374 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_tasks/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_tasks/tests/test_tasks.py
 Comment: 
 
-Filename: kaiju_tasks-2.1.7.dist-info/LICENSE
+Filename: kaiju_tasks-2.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_tasks-2.1.7.dist-info/METADATA
+Filename: kaiju_tasks-2.1.8.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_tasks-2.1.7.dist-info/WHEEL
+Filename: kaiju_tasks-2.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_tasks-2.1.7.dist-info/top_level.txt
+Filename: kaiju_tasks-2.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_tasks-2.1.7.dist-info/RECORD
+Filename: kaiju_tasks-2.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_tasks/__init__.py

```diff
@@ -1,7 +1,7 @@
 from .types import *
 from .services import *
 from .gui import *
 
-__version__ = '2.1.7'
+__version__ = '2.1.8'
 __python_version__ = '3.11'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_tasks/gui.py

```diff
@@ -1,18 +1,21 @@
 import abc
 from typing import Iterable
 
 from croniter import croniter
-
-from kaiju_tools import ContextableService, PublicInterface, SERVICE_CLASS_REGISTRY
-from kaiju_model.fields import StringField, BooleanField, DateTimeField, IntegerField, JSONObjectField
+from kaiju_model.fields import BooleanField, DateTimeField, IntegerField, JSONObjectField, StringField
 from kaiju_model.grid.constructor import GridConstructor
 from kaiju_model.model import BaseModel
+from kaiju_tools import SERVICE_CLASS_REGISTRY, ContextableService, PublicInterface
 from kaiju_tools.exceptions import ValidationError
+from kaiju_tools.functions import get_short_uid
+
 from kaiju_tasks.services import TaskService
+from kaiju_tasks.types import TaskStatus
+
 
 __all__ = ('TaskEditModel', 'TaskGridModel', 'TaskGUI')
 
 
 def generate_header(fields: Iterable) -> list:
     header = []
 
@@ -136,16 +139,36 @@
     async def update(self, id, grouping=False, **kws) -> True:
         task = await self.get(id, grouping=grouping)
         task.update(kws)
         async with self.edit_model(self.app, **task) as _:
             await self._tasks.update(id, data=kws, columns=[])
             return True
 
-    async def reset_task(self, id):
-        return await self._tasks.reset_task(id)
+    async def reset_task(self, id: str) -> bool:
+        """Reset task to IDLE and remove result / errors.
+
+        :returns: True if task has been restarted, False if it can't be restarted
+        """
+        restarted = await self._tasks.m_update(
+            id=[id],
+            data={
+                'status': TaskStatus.IDLE.value,
+                'executor_id': None,
+                'job_id': get_short_uid(),
+                'exit_code': None,
+                'error': None,
+                'retries': 0,
+                'next_run': 1,
+                'exec_deadline': None,
+                'stage': 0,
+                'result': [],
+            },
+            columns=['id'],
+        )
+        return bool(restarted)
 
     async def grid(self, query=None, conditions=None, page=1, per_page=24):
         offset = per_page * (page - 1)
         if conditions is None:
             conditions = {}
         if query:
             conditions['description'] = {'~': query}
```

## Comparing `kaiju_tasks-2.1.7.dist-info/LICENSE` & `kaiju_tasks-2.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_tasks-2.1.7.dist-info/METADATA` & `kaiju_tasks-2.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-tasks
-Version: 2.1.7
+Version: 2.1.8
 Summary: Service and user task management
 Home-page: https://gitlab.com/kaiju-python/kaiju-tasks
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `kaiju_tasks-2.1.7.dist-info/RECORD` & `kaiju_tasks-2.1.8.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-kaiju_tasks/__init__.py,sha256=oxlBcYW257ch8oGq_Vu5VNNFT9wuWbTq2pPRqQ0a2HU,151
-kaiju_tasks/gui.py,sha256=dt5zK17X52JX7n06ZMRfnlJoGh1xNdV50vkGqxLROZQ,5386
+kaiju_tasks/__init__.py,sha256=Ih9UnjM7iNyezQ9mouTN-04qF9aIIApPf0uaD3pfrI0,151
+kaiju_tasks/gui.py,sha256=SwPN_7GQkMDU7VUONXOCk7_tMBoyZTIflb60vxxjmRw,6119
 kaiju_tasks/services.py,sha256=spxIjehmr7-BN8OVF862vfhgrl20d3aE_AsdgoHfKdQ,40431
 kaiju_tasks/types.py,sha256=3JLF6ZsCXPFTcwZISQcwNUbTqJeGIpe24GRNa8i9lpE,6161
 kaiju_tasks/tests/__init__.py,sha256=WlPruePOcaMi5ikqn6GheE1Z-zYcysb9M1dj6SteWGY,42
 kaiju_tasks/tests/fixtures.py,sha256=7hLaDyE3Sjibnt5zZ9YNNJ2586541NRPC4Y3qIQzI2s,2272
 kaiju_tasks/tests/test_tasks.py,sha256=NT4kACEZeYw2OiNA9AwbKOVrfM1JLfnh7KefYUplF3s,15554
-kaiju_tasks-2.1.7.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_tasks-2.1.7.dist-info/METADATA,sha256=i5jqDMHGKDHs-xsr3xInvdmAnn_-5iQpDVU6BzRaag0,3212
-kaiju_tasks-2.1.7.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-kaiju_tasks-2.1.7.dist-info/top_level.txt,sha256=QyLogqOVVajJlalq6RfikGx5VGn_lLeTANJEsfZZlM0,12
-kaiju_tasks-2.1.7.dist-info/RECORD,,
+kaiju_tasks-2.1.8.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_tasks-2.1.8.dist-info/METADATA,sha256=Fxt3QpHc8NQQjKA2cJ2xaJrR2T9ilIhatf_jXzv_L5Q,3212
+kaiju_tasks-2.1.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+kaiju_tasks-2.1.8.dist-info/top_level.txt,sha256=QyLogqOVVajJlalq6RfikGx5VGn_lLeTANJEsfZZlM0,12
+kaiju_tasks-2.1.8.dist-info/RECORD,,
```

