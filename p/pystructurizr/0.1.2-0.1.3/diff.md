# Comparing `tmp/pystructurizr-0.1.2.tar.gz` & `tmp/pystructurizr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystructurizr-0.1.2.tar", last modified: Fri Jun 23 21:02:17 2023, max compression
+gzip compressed data, was "pystructurizr-0.1.3.tar", last modified: Thu Jul 27 19:03:08 2023, max compression
```

## Comparing `pystructurizr-0.1.2.tar` & `pystructurizr-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-23 21:02:17.039086 pystructurizr-0.1.2/
--rw-r--r--   0 niels      (501) staff       (20)     1091 2023-06-15 21:03:41.000000 pystructurizr-0.1.2/LICENSE.txt
--rw-r--r--   0 niels      (501) staff       (20)     4120 2023-06-23 21:02:17.038572 pystructurizr-0.1.2/PKG-INFO
--rw-r--r--   0 niels      (501) staff       (20)     3417 2023-06-15 21:10:05.000000 pystructurizr-0.1.2/README.md
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-23 21:02:17.026063 pystructurizr-0.1.2/example/
--rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:48:57.000000 pystructurizr-0.1.2/example/__init__.py
--rw-r--r--   0 niels      (501) staff       (20)     2492 2023-06-18 09:38:04.000000 pystructurizr-0.1.2/example/analysissystem.py
--rw-r--r--   0 niels      (501) staff       (20)      286 2023-06-18 09:39:00.000000 pystructurizr-0.1.2/example/analysisystem_containerview.py
--rw-r--r--   0 niels      (501) staff       (20)      197 2023-06-18 09:39:15.000000 pystructurizr-0.1.2/example/chatserver_componentview.py
--rw-r--r--   0 niels      (501) staff       (20)     1060 2023-06-17 18:06:20.000000 pystructurizr-0.1.2/example/chatsystem.py
--rw-r--r--   0 niels      (501) staff       (20)      194 2023-06-18 09:39:26.000000 pystructurizr-0.1.2/example/chatsystem_containerview.py
--rw-r--r--   0 niels      (501) staff       (20)      163 2023-06-11 13:15:48.000000 pystructurizr-0.1.2/example/systemlandscapeview.py
--rw-r--r--   0 niels      (501) staff       (20)      315 2023-06-17 10:47:22.000000 pystructurizr-0.1.2/example/users.py
--rw-r--r--   0 niels      (501) staff       (20)      606 2023-06-17 18:12:09.000000 pystructurizr-0.1.2/example/workspace.py
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-23 21:02:17.030977 pystructurizr-0.1.2/pystructurizr/
--rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:49:07.000000 pystructurizr-0.1.2/pystructurizr/__init__.py
--rw-r--r--   0 niels      (501) staff       (20)     3465 2023-06-23 21:00:26.000000 pystructurizr-0.1.2/pystructurizr/cli.py
--rw-r--r--   0 niels      (501) staff       (20)     1323 2023-06-23 21:00:26.000000 pystructurizr-0.1.2/pystructurizr/cli_helper.py
--rw-r--r--   0 niels      (501) staff       (20)     2251 2023-06-17 20:24:22.000000 pystructurizr-0.1.2/pystructurizr/cli_watcher.py
--rw-r--r--   0 niels      (501) staff       (20)     2516 2023-06-17 20:29:47.000000 pystructurizr-0.1.2/pystructurizr/cloudstorage.py
--rw-r--r--   0 niels      (501) staff       (20)    12129 2023-06-23 21:00:26.000000 pystructurizr-0.1.2/pystructurizr/dsl.py
--rw-r--r--   0 niels      (501) staff       (20)     1021 2023-06-23 21:00:26.000000 pystructurizr-0.1.2/pystructurizr/generator.py
--rw-r--r--   0 niels      (501) staff       (20)      249 2023-06-17 11:06:39.000000 pystructurizr-0.1.2/pystructurizr/index.html
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-23 21:02:17.036479 pystructurizr-0.1.2/pystructurizr.egg-info/
--rw-r--r--   0 niels      (501) staff       (20)     4120 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/PKG-INFO
--rw-r--r--   0 niels      (501) staff       (20)      726 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/SOURCES.txt
--rw-r--r--   0 niels      (501) staff       (20)        1 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/dependency_links.txt
--rw-r--r--   0 niels      (501) staff       (20)       57 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/entry_points.txt
--rw-r--r--   0 niels      (501) staff       (20)       80 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/requires.txt
--rw-r--r--   0 niels      (501) staff       (20)       22 2023-06-23 21:02:16.000000 pystructurizr-0.1.2/pystructurizr.egg-info/top_level.txt
--rw-r--r--   0 niels      (501) staff       (20)       38 2023-06-23 21:02:17.039266 pystructurizr-0.1.2/setup.cfg
--rw-r--r--   0 niels      (501) staff       (20)     1271 2023-06-23 21:01:37.000000 pystructurizr-0.1.2/setup.py
-drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-06-23 21:02:17.037453 pystructurizr-0.1.2/test/
--rw-r--r--   0 niels      (501) staff       (20)      675 2023-06-17 20:47:58.000000 pystructurizr-0.1.2/test/test_cli.py
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-07-27 19:03:08.916105 pystructurizr-0.1.3/
+-rw-r--r--   0 niels      (501) staff       (20)     1091 2023-06-15 21:03:41.000000 pystructurizr-0.1.3/LICENSE.txt
+-rw-r--r--   0 niels      (501) staff       (20)     4567 2023-07-27 19:03:08.915593 pystructurizr-0.1.3/PKG-INFO
+-rw-r--r--   0 niels      (501) staff       (20)     3864 2023-07-27 18:27:09.000000 pystructurizr-0.1.3/README.md
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-07-27 19:03:08.895146 pystructurizr-0.1.3/examples/
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-07-27 19:03:08.902027 pystructurizr-0.1.3/examples/module_example/
+-rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:48:57.000000 pystructurizr-0.1.3/examples/module_example/__init__.py
+-rw-r--r--   0 niels      (501) staff       (20)     2492 2023-06-18 09:38:04.000000 pystructurizr-0.1.3/examples/module_example/analysissystem.py
+-rw-r--r--   0 niels      (501) staff       (20)      265 2023-07-27 18:35:22.000000 pystructurizr-0.1.3/examples/module_example/analysisystem_containerview.py
+-rw-r--r--   0 niels      (501) staff       (20)      183 2023-07-27 18:40:32.000000 pystructurizr-0.1.3/examples/module_example/chatserver_componentview.py
+-rw-r--r--   0 niels      (501) staff       (20)     1287 2023-07-26 20:10:17.000000 pystructurizr-0.1.3/examples/module_example/chatsystem.py
+-rw-r--r--   0 niels      (501) staff       (20)      180 2023-07-27 18:40:44.000000 pystructurizr-0.1.3/examples/module_example/chatsystem_containerview.py
+-rw-r--r--   0 niels      (501) staff       (20)      156 2023-07-27 18:40:54.000000 pystructurizr-0.1.3/examples/module_example/systemlandscapeview.py
+-rw-r--r--   0 niels      (501) staff       (20)      315 2023-06-17 10:47:22.000000 pystructurizr-0.1.3/examples/module_example/users.py
+-rw-r--r--   0 niels      (501) staff       (20)      585 2023-07-27 18:35:36.000000 pystructurizr-0.1.3/examples/module_example/workspace.py
+-rw-r--r--   0 niels      (501) staff       (20)     2055 2023-07-27 18:05:23.000000 pystructurizr-0.1.3/examples/single_file_example.py
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-07-27 19:03:08.910823 pystructurizr-0.1.3/pystructurizr/
+-rw-r--r--   0 niels      (501) staff       (20)        0 2023-05-29 09:49:07.000000 pystructurizr-0.1.3/pystructurizr/__init__.py
+-rw-r--r--   0 niels      (501) staff       (20)     3465 2023-06-23 21:00:26.000000 pystructurizr-0.1.3/pystructurizr/cli.py
+-rw-r--r--   0 niels      (501) staff       (20)     1323 2023-06-23 21:00:26.000000 pystructurizr-0.1.3/pystructurizr/cli_helper.py
+-rw-r--r--   0 niels      (501) staff       (20)     2251 2023-06-17 20:24:22.000000 pystructurizr-0.1.3/pystructurizr/cli_watcher.py
+-rw-r--r--   0 niels      (501) staff       (20)     2516 2023-06-17 20:29:47.000000 pystructurizr-0.1.3/pystructurizr/cloudstorage.py
+-rw-r--r--   0 niels      (501) staff       (20)    15509 2023-07-27 18:10:57.000000 pystructurizr-0.1.3/pystructurizr/dsl.py
+-rw-r--r--   0 niels      (501) staff       (20)     1021 2023-07-27 18:05:34.000000 pystructurizr-0.1.3/pystructurizr/generator.py
+-rw-r--r--   0 niels      (501) staff       (20)      249 2023-06-17 11:06:39.000000 pystructurizr-0.1.3/pystructurizr/index.html
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-07-27 19:03:08.914105 pystructurizr-0.1.3/pystructurizr.egg-info/
+-rw-r--r--   0 niels      (501) staff       (20)     4567 2023-07-27 19:03:08.000000 pystructurizr-0.1.3/pystructurizr.egg-info/PKG-INFO
+-rw-r--r--   0 niels      (501) staff       (20)      902 2023-07-27 19:03:08.000000 pystructurizr-0.1.3/pystructurizr.egg-info/SOURCES.txt
+-rw-r--r--   0 niels      (501) staff       (20)        1 2023-07-27 19:03:08.000000 pystructurizr-0.1.3/pystructurizr.egg-info/dependency_links.txt
+-rw-r--r--   0 niels      (501) staff       (20)       57 2023-07-27 19:03:08.000000 pystructurizr-0.1.3/pystructurizr.egg-info/entry_points.txt
+-rw-r--r--   0 niels      (501) staff       (20)       80 2023-07-27 19:03:08.000000 pystructurizr-0.1.3/pystructurizr.egg-info/requires.txt
+-rw-r--r--   0 niels      (501) staff       (20)       14 2023-07-27 19:03:08.000000 pystructurizr-0.1.3/pystructurizr.egg-info/top_level.txt
+-rw-r--r--   0 niels      (501) staff       (20)       38 2023-07-27 19:03:08.916252 pystructurizr-0.1.3/setup.cfg
+-rw-r--r--   0 niels      (501) staff       (20)     1327 2023-07-27 18:59:50.000000 pystructurizr-0.1.3/setup.py
+drwxr-xr-x   0 niels      (501) staff       (20)        0 2023-07-27 19:03:08.914595 pystructurizr-0.1.3/test/
+-rw-r--r--   0 niels      (501) staff       (20)      675 2023-06-17 20:47:58.000000 pystructurizr-0.1.3/test/test_cli.py
```

### Comparing `pystructurizr-0.1.2/LICENSE.txt` & `pystructurizr-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.2/PKG-INFO` & `pystructurizr-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystructurizr
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python DSL inspired by Structurizr, intended for generating C4 diagrams
 Home-page: https://github.com/nielsvanspauwen/pystructurizr
 Author: Niels Vanspauwen
 Author-email: niels.vanspauwen@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -14,14 +14,18 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PyStructurizr
+[![license](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)
+[![PyPI version](https://badge.fury.io/py/pystructurizr.svg)](https://badge.fury.io/py/pystructurizr)
+[![Pylint](https://github.com/nielsvanspauwen/pystructurizr/actions/workflows/pylint.yml/badge.svg?branch=master)](https://github.com/nielsvanspauwen/pystructurizr/actions/workflows/pylint.yml)
+
 PyStructurizr provides a Python DSL inspired by [Structurizr](https://structurizr.com/), and is intended for generating C4 diagrams.
 
 ## Overview
 [Structurizr](https://structurizr.com/) builds upon "diagrams as code", allowing you to create multiple software architecture diagrams from a single model. A popular way of creating Structurizr workspaces is the Structurizr DSL.
 
 However, Structurizr DSL has some downsides:
 
@@ -55,23 +59,24 @@
 ```
 
 In PyStructurizr, this becomes:
 ```python
 from pystructurizr.dsl import Workspace
 
 # Create the model(s)
-workspace = Workspace()
-user = workspace.Model("Users").Person("User")
-software_system = workspace.Model("System").SoftwareSystem("Software System")
-webapp = software_system.Container("Web Application")
-db = software_system.Container("Database")
-
-# Define the relationships
-user.uses(webapp, "Uses")
-webapp.uses(db, "Reads from and writes to")
+with Workspace() as workspace:
+    with workspace.Model(name="model") as model:
+        user = model.Person("User")
+        with model.SoftwareSystem("Software System") as software_system:
+            webapp = software_system.Container("Web Application")
+            db = software_system.Container("Database")
+
+    # Define the relationships
+    user.uses(webapp, "Uses")
+    webapp.uses(db, "Reads from and writes to")
 
 # Create a view onto the model
 workspace.ContainerView(
     software_system, 
     "My Container View",
     "The container view of our simply software system."
 )
```

### Comparing `pystructurizr-0.1.2/README.md` & `pystructurizr-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # PyStructurizr
+[![license](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)
+[![PyPI version](https://badge.fury.io/py/pystructurizr.svg)](https://badge.fury.io/py/pystructurizr)
+[![Pylint](https://github.com/nielsvanspauwen/pystructurizr/actions/workflows/pylint.yml/badge.svg?branch=master)](https://github.com/nielsvanspauwen/pystructurizr/actions/workflows/pylint.yml)
+
 PyStructurizr provides a Python DSL inspired by [Structurizr](https://structurizr.com/), and is intended for generating C4 diagrams.
 
 ## Overview
 [Structurizr](https://structurizr.com/) builds upon "diagrams as code", allowing you to create multiple software architecture diagrams from a single model. A popular way of creating Structurizr workspaces is the Structurizr DSL.
 
 However, Structurizr DSL has some downsides:
 
@@ -36,23 +40,24 @@
 ```
 
 In PyStructurizr, this becomes:
 ```python
 from pystructurizr.dsl import Workspace
 
 # Create the model(s)
-workspace = Workspace()
-user = workspace.Model("Users").Person("User")
-software_system = workspace.Model("System").SoftwareSystem("Software System")
-webapp = software_system.Container("Web Application")
-db = software_system.Container("Database")
-
-# Define the relationships
-user.uses(webapp, "Uses")
-webapp.uses(db, "Reads from and writes to")
+with Workspace() as workspace:
+    with workspace.Model(name="model") as model:
+        user = model.Person("User")
+        with model.SoftwareSystem("Software System") as software_system:
+            webapp = software_system.Container("Web Application")
+            db = software_system.Container("Database")
+
+    # Define the relationships
+    user.uses(webapp, "Uses")
+    webapp.uses(db, "Reads from and writes to")
 
 # Create a view onto the model
 workspace.ContainerView(
     software_system, 
     "My Container View",
     "The container view of our simply software system."
 )
```

### Comparing `pystructurizr-0.1.2/example/analysissystem.py` & `pystructurizr-0.1.3/examples/module_example/analysissystem.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.2/example/workspace.py` & `pystructurizr-0.1.3/examples/module_example/workspace.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pystructurizr.dsl import Workspace
 
-from example.users import users
-from example.chatsystem import chat
-from example.analysissystem import analytics
+from .users import users
+from .chatsystem import chat
+from .analysissystem import analytics
 
 workspace = Workspace()
 workspace.Model(users)
 workspace.Model(chat)
 workspace.Model(analytics)
 
 analytics.uses(chat, "Derives insights from")
```

### Comparing `pystructurizr-0.1.2/pystructurizr/cli.py` & `pystructurizr-0.1.3/pystructurizr/cli.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.2/pystructurizr/cli_helper.py` & `pystructurizr-0.1.3/pystructurizr/cli_helper.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.2/pystructurizr/cli_watcher.py` & `pystructurizr-0.1.3/pystructurizr/cli_watcher.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.2/pystructurizr/cloudstorage.py` & `pystructurizr-0.1.3/pystructurizr/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.2/pystructurizr/dsl.py` & `pystructurizr-0.1.3/pystructurizr/dsl.py`

 * *Files 14% similar despite different names*

```diff
@@ -104,82 +104,187 @@
         for rel in self.relationships:
             rel.dump(dumper)
 
 
 class Container(Element):
     def __init__(self, name: str, description: Optional[str]=None, technology: Optional[str]=None, tags: Optional[List[str]]=None):
         super().__init__(name, description, technology, tags)
-        self.components = []
+        self.elements = []
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
 
     # pylint: disable=invalid-name
     def Component(self, *args, **kwargs) -> Component:
         if args and isinstance(args[0], Component):
             component = args[0]
         else:
             component = Component(*args, **kwargs)
-        self.components.append(component)
+        self.elements.append(component)
         return component
 
+    # pylint: disable=invalid-name
+    def Group(self, *args, **kwargs) -> "Group":
+        if args and isinstance(args[0], Group):
+            g = args[0]
+        else:
+            g = Group(*args, **kwargs)
+        self.elements.append(g)
+        return g
+
     def dump(self, dumper: Dumper) -> None:
         dumper.add(f'{self.instname} = Container "{self.name}" "{self.description}" {{')
         dumper.indent()
         if self.technology:
             dumper.add(f'technology "{self.technology}"')
         if self.tags:
             dumper.add(f'tags "{", ".join(self.tags)}"')
-        for component in self.components:
-            component.dump(dumper)
+        for el in self.elements:
+            el.dump(dumper)
         dumper.outdent()
         dumper.add('}')
 
     def dump_relationships(self, dumper: Dumper) -> None:
         for rel in self.relationships:
             rel.dump(dumper)
-        for component in self.components:
-            component.dump_relationships(dumper)
+        for el in self.elements:
+            el.dump_relationships(dumper)
 
 
 class SoftwareSystem(Element):
     def __init__(self, name: str, description: Optional[str]=None, technology: Optional[str]=None, tags: Optional[List[str]]=None):
         super().__init__(name, description, technology, tags)
-        self.containers = []
+        self.elements = []
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
 
     # pylint: disable=invalid-name
     def Container(self, *args, **kwargs) -> Container:
         if args and isinstance(args[0], Container):
             container = args[0]
         else:
             container = Container(*args, **kwargs)
-        self.containers.append(container)
+        self.elements.append(container)
         return container
 
+    # pylint: disable=invalid-name
+    def Group(self, *args, **kwargs) -> "Group":
+        if args and isinstance(args[0], Group):
+            g = args[0]
+        else:
+            g = Group(*args, **kwargs)
+        self.elements.append(g)
+        return g
+
     def dump(self, dumper: Dumper) -> None:
         dumper.add(f'{self.instname} = SoftwareSystem "{self.name}" "{self.description}" {{')
         dumper.indent()
         if self.technology:
             dumper.add(f'technology "{self.technology}"')
         if self.tags:
             dumper.add(f'tags "{", ".join(self.tags)}"')
-        for container in self.containers:
-            container.dump(dumper)
+        for el in self.elements:
+            el.dump(dumper)
         dumper.outdent()
         dumper.add('}')
 
     def dump_relationships(self, dumper: Dumper) -> None:
         for rel in self.relationships:
             rel.dump(dumper)
-        for container in self.containers:
-            container.dump_relationships(dumper)
+        for el in self.elements:
+            el.dump_relationships(dumper)
+
+
+class Group(Element):
+    def __init__(self, name: str):
+        super().__init__(name)
+        self.elements = []
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
+    # pylint: disable=invalid-name
+    def Person(self, *args, **kwargs) -> Person:
+        if args and isinstance(args[0], Person):
+            person = args[0]
+        else:
+            person = Person(*args, **kwargs)
+        self.elements.append(person)
+        return person
+
+    # pylint: disable=invalid-name
+    def SoftwareSystem(self, *args, **kwargs) -> SoftwareSystem:
+        if args and isinstance(args[0], SoftwareSystem):
+            system = args[0]
+        else:
+            system = SoftwareSystem(*args, **kwargs)
+        self.elements.append(system)
+        return system
+
+    # pylint: disable=invalid-name
+    def Container(self, *args, **kwargs) -> Container:
+        if args and isinstance(args[0], Container):
+            container = args[0]
+        else:
+            container = Container(*args, **kwargs)
+        self.elements.append(container)
+        return container
+
+    # pylint: disable=invalid-name
+    def Component(self, *args, **kwargs) -> Component:
+        if args and isinstance(args[0], Component):
+            component = args[0]
+        else:
+            component = Component(*args, **kwargs)
+        self.elements.append(component)
+        return component
+
+    # pylint: disable=invalid-name
+    def Group(self, *args, **kwargs) -> "Group":
+        if args and isinstance(args[0], Group):
+            g = args[0]
+        else:
+            g = Group(*args, **kwargs)
+        self.elements.append(g)
+        return g
+
+    def dump(self, dumper: Dumper) -> None:
+        dumper.add(f'group "{self.name}" {{')
+        dumper.indent()
+        for element in self.elements:
+            element.dump(dumper)
+        dumper.outdent()
+        dumper.add('}')
+
+    def dump_relationships(self, dumper: Dumper) -> None:
+        for element in self.elements:
+            element.dump_relationships(dumper)
 
 
 class Model(Element):
     def __init__(self, name: str):
         super().__init__(name)
         self.elements = []
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
     # pylint: disable=invalid-name
     def Person(self, *args, **kwargs) -> Person:
         if args and isinstance(args[0], Person):
             person = args[0]
         else:
             person = Person(*args, **kwargs)
         self.elements.append(person)
@@ -190,14 +295,23 @@
         if args and isinstance(args[0], SoftwareSystem):
             system = args[0]
         else:
             system = SoftwareSystem(*args, **kwargs)
         self.elements.append(system)
         return system
 
+    # pylint: disable=invalid-name
+    def Group(self, *args, **kwargs) -> Group:
+        if args and isinstance(args[0], Group):
+            g = args[0]
+        else:
+            g = Group(*args, **kwargs)
+        self.elements.append(g)
+        return g
+
     def dump(self, dumper: Dumper) -> None:
         for element in self.elements:
             element.dump(dumper)
 
     def dump_relationships(self, dumper: Dumper) -> None:
         for element in self.elements:
             element.dump_relationships(dumper)
@@ -299,20 +413,31 @@
                 "background": "#ffffff"
             }, {
                 "tag": "database",
                 "shape": "Cylinder"
             }
         )
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
     def dump(self, dumper: Dumper = Dumper()) -> None:
         dumper.add('workspace {')
         dumper.indent()
 
         dumper.add('model {')
         dumper.indent()
+        dumper.add('properties {')
+        dumper.indent()
+        dumper.add('"structurizr.groupSeparator" "/"')
+        dumper.outdent()
+        dumper.add('}')
         for model in self.models:
             model.dump(dumper)
         for model in self.models:
             model.dump_relationships(dumper)
         dumper.outdent()
         dumper.add('}')
```

### Comparing `pystructurizr-0.1.2/pystructurizr/generator.py` & `pystructurizr-0.1.3/pystructurizr/generator.py`

 * *Files identical despite different names*

### Comparing `pystructurizr-0.1.2/pystructurizr.egg-info/PKG-INFO` & `pystructurizr-0.1.3/pystructurizr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystructurizr
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python DSL inspired by Structurizr, intended for generating C4 diagrams
 Home-page: https://github.com/nielsvanspauwen/pystructurizr
 Author: Niels Vanspauwen
 Author-email: niels.vanspauwen@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -14,14 +14,18 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PyStructurizr
+[![license](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)
+[![PyPI version](https://badge.fury.io/py/pystructurizr.svg)](https://badge.fury.io/py/pystructurizr)
+[![Pylint](https://github.com/nielsvanspauwen/pystructurizr/actions/workflows/pylint.yml/badge.svg?branch=master)](https://github.com/nielsvanspauwen/pystructurizr/actions/workflows/pylint.yml)
+
 PyStructurizr provides a Python DSL inspired by [Structurizr](https://structurizr.com/), and is intended for generating C4 diagrams.
 
 ## Overview
 [Structurizr](https://structurizr.com/) builds upon "diagrams as code", allowing you to create multiple software architecture diagrams from a single model. A popular way of creating Structurizr workspaces is the Structurizr DSL.
 
 However, Structurizr DSL has some downsides:
 
@@ -55,23 +59,24 @@
 ```
 
 In PyStructurizr, this becomes:
 ```python
 from pystructurizr.dsl import Workspace
 
 # Create the model(s)
-workspace = Workspace()
-user = workspace.Model("Users").Person("User")
-software_system = workspace.Model("System").SoftwareSystem("Software System")
-webapp = software_system.Container("Web Application")
-db = software_system.Container("Database")
-
-# Define the relationships
-user.uses(webapp, "Uses")
-webapp.uses(db, "Reads from and writes to")
+with Workspace() as workspace:
+    with workspace.Model(name="model") as model:
+        user = model.Person("User")
+        with model.SoftwareSystem("Software System") as software_system:
+            webapp = software_system.Container("Web Application")
+            db = software_system.Container("Database")
+
+    # Define the relationships
+    user.uses(webapp, "Uses")
+    webapp.uses(db, "Reads from and writes to")
 
 # Create a view onto the model
 workspace.ContainerView(
     software_system, 
     "My Container View",
     "The container view of our simply software system."
 )
```

### Comparing `pystructurizr-0.1.2/pystructurizr.egg-info/SOURCES.txt` & `pystructurizr-0.1.3/pystructurizr.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 LICENSE.txt
 README.md
 setup.py
-example/__init__.py
-example/analysissystem.py
-example/analysisystem_containerview.py
-example/chatserver_componentview.py
-example/chatsystem.py
-example/chatsystem_containerview.py
-example/systemlandscapeview.py
-example/users.py
-example/workspace.py
+examples/single_file_example.py
+examples/module_example/__init__.py
+examples/module_example/analysissystem.py
+examples/module_example/analysisystem_containerview.py
+examples/module_example/chatserver_componentview.py
+examples/module_example/chatsystem.py
+examples/module_example/chatsystem_containerview.py
+examples/module_example/systemlandscapeview.py
+examples/module_example/users.py
+examples/module_example/workspace.py
 pystructurizr/__init__.py
 pystructurizr/cli.py
 pystructurizr/cli_helper.py
 pystructurizr/cli_watcher.py
 pystructurizr/cloudstorage.py
 pystructurizr/dsl.py
 pystructurizr/generator.py
```

### Comparing `pystructurizr-0.1.2/setup.py` & `pystructurizr-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
+found_packages = find_packages()
+print(found_packages)
+
 setup(
     name='pystructurizr',
-    version='0.1.2',
+    version='0.1.3',
     description='A Python DSL inspired by Structurizr, intended for generating C4 diagrams',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Niels Vanspauwen',
     author_email='niels.vanspauwen@gmail.com',
     license='MIT',
     url='https://github.com/nielsvanspauwen/pystructurizr',
```

### Comparing `pystructurizr-0.1.2/test/test_cli.py` & `pystructurizr-0.1.3/test/test_cli.py`

 * *Files identical despite different names*

