# Comparing `tmp/prefab_classes-0.9.2.tar.gz` & `tmp/prefab_classes-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefab_classes-0.9.2.tar", last modified: Sun Apr 16 07:33:45 2023, max compression
+gzip compressed data, was "prefab_classes-0.9.3.tar", last modified: Thu Jul 27 12:06:27 2023, max compression
```

## Comparing `prefab_classes-0.9.2.tar` & `prefab_classes-0.9.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.685636 prefab_classes-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.685636 prefab_classes-0.9.2/src/prefab_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/src/prefab_classes/compiled/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/compiled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36138 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/compiled/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/compiled/rewrite_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/src/prefab_classes/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class_maker/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/autogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/method_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/dynamic/prefab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes/sentinels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.685636 prefab_classes-0.9.2/src/prefab_classes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-16 07:33:45.000000 prefab_classes-0.9.2/src/prefab_classes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-16 07:33:45.000000 prefab_classes-0.9.2/src/prefab_classes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:33:45.000000 prefab_classes-0.9.2/src/prefab_classes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-16 07:33:45.000000 prefab_classes-0.9.2/src/prefab_classes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-16 07:33:45.000000 prefab_classes-0.9.2/src/prefab_classes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/src/prefab_classes_hook/
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/src/prefab_classes_hook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:33:45.689636 prefab_classes-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-16 07:33:30.000000 prefab_classes-0.9.2/tests/test_versions_match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:06:27.553090 prefab_classes-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-07-27 12:06:27.553090 prefab_classes-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:06:27.553090 prefab_classes-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:06:27.549090 prefab_classes-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:06:27.549090 prefab_classes-0.9.3/src/prefab_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:06:27.549090 prefab_classes-0.9.3/src/prefab_classes/compiled/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/compiled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39507 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/compiled/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/compiled/rewrite_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:06:27.553090 prefab_classes-0.9.3/src/prefab_classes/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/dynamic/_attribute_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:06:27.553090 prefab_classes-0.9.3/src/prefab_classes/dynamic/_attribute_class_maker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/dynamic/autogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/dynamic/method_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/dynamic/prefab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes/sentinels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:06:27.549090 prefab_classes-0.9.3/src/prefab_classes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-07-27 12:06:27.000000 prefab_classes-0.9.3/src/prefab_classes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-27 12:06:27.000000 prefab_classes-0.9.3/src/prefab_classes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:06:27.000000 prefab_classes-0.9.3/src/prefab_classes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-27 12:06:27.000000 prefab_classes-0.9.3/src/prefab_classes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 12:06:27.000000 prefab_classes-0.9.3/src/prefab_classes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:06:27.553090 prefab_classes-0.9.3/src/prefab_classes_hook/
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/src/prefab_classes_hook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:06:27.553090 prefab_classes-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-27 12:06:16.000000 prefab_classes-0.9.3/tests/test_versions_match.py
```

### Comparing `prefab_classes-0.9.2/LICENSE.md` & `prefab_classes-0.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/PKG-INFO` & `prefab_classes-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefab_classes
-Version: 0.9.2
+Version: 0.9.3
 Summary: Boilerplate Generator for Classes
 Author: David C Ellis
 Project-URL: Homepage, https://github.com/davidcellis/PrefabClasses
 Project-URL: Documentation, https://prefabclasses.readthedocs.io/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `prefab_classes-0.9.2/README.md` & `prefab_classes-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/pyproject.toml` & `prefab_classes-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/_typing.py` & `prefab_classes-0.9.3/src/prefab_classes/_typing.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/compiled/generator.py` & `prefab_classes-0.9.3/src/prefab_classes/compiled/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ast
 from functools import cached_property
+from collections import defaultdict
 
 from ..constants import (
     PRE_INIT_FUNC,
     POST_INIT_FUNC,
     PREFAB_INIT_FUNC,
     DECORATOR_NAME,
     ATTRIBUTE_FUNCNAME,
@@ -65,14 +66,21 @@
     exclude_field: bool = attribute(default=False)
     annotation: "None | ast.expr" = attribute(default=None)
     attribute_func: bool = attribute(default=False)
 
     # Indicator that this Field should be made KW_ONLY
     _kw_only_flagged = attribute(default=False, init=False, repr=False)
 
+    # This keeps a history of all assignments that have been used to remove
+    # them from the AST after compilation
+    all_assignments: set[assignment_type] = attribute(default_factory=set, init=False, repr=False)
+
+    def __prefab_post_init__(self):
+        self.all_assignments.add(self.field)
+
     @cached_property
     def default_factory_call(self):
         return ast.Call(func=self.default_factory, args=[], keywords=[])
 
     def ast_attribute(
         self,
         obj_name="self",
@@ -82,14 +90,25 @@
         attrib = ast.Attribute(
             value=ast.Name(id=obj_name, ctx=ast.Load()),
             attr=self.name,
             ctx=ctx(),
         )
         return attrib
 
+    @property
+    def ast_annassign(self):
+        """
+        Get an annotated assignment with no value for this field or return None
+        """
+        if self.annotation:
+            name = ast.Name(id=self.name, ctx=ast.Store())
+            assign = ast.AnnAssign(target=name, annotation=self.annotation, value=None, simple=True)
+            return assign
+        return None
+
     @classmethod
     def from_keywords(cls, name, field, keywords, annotation=None):
         keys = {k.arg: k.value for k in keywords}
         default = keys.get("default", None)
         default_factory = keys.get("default_factory", None)
         try:
             init_ = keys["init"].value
@@ -274,20 +293,21 @@
 
     @cached_property
     def fields(self) -> dict[str, Field]:
         def funcid_or_none(value):
             """get .func.id or return None"""
             return getattr(getattr(value, "func", None), "id", None)
 
-        fields: list[Field] = []
+        fields: dict[str, Field] = {}
 
-        # If there are any plain assignments, annotated assignments that
-        # do not use attribute() calls must be removed to match 'dynamic'
-        # behaviour.
-        require_attribute_func = False
+        # This stores potential default values
+        # Given as plain assignments that are later typed
+        # Keep the assignments to be cleared later
+        potential_defaults: dict = {}
+        plain_assignments: dict[set[assignment_type]] = defaultdict(set)
 
         flag_kw_only = False
         for item in self.node.body:
             if isinstance(item, ast.AnnAssign):
                 # Test if something is a classvar
                 if _is_classvar(item):
                     continue
@@ -303,58 +323,108 @@
                 if funcid_or_none(item.value) == ATTRIBUTE_FUNCNAME:
                     field = Field.from_keywords(
                         name=field_name,
                         field=item,
                         keywords=item.value.keywords,
                         annotation=item.annotation,
                     )
+
+                    # Get any potential assignments to clear after generation
+                    old_field = fields.get(field_name, None)
+                    if old_field:
+                        field.all_assignments.update(old_field.all_assignments)
+                    else:
+                        field.all_assignments.update(plain_assignments[field_name])
+
                 else:
-                    field = Field(
-                        name=field_name,
-                        field=item,
-                        default=item.value,
-                        annotation=item.annotation,
-                    )
+                    if field_name in fields and item.value is None:
+                        # If the field exists and this is just an annotation
+                        # Update the field annotation
+                        field = fields[field_name]
+                        field.annotation = item.annotation
+                        field.all_assignments.add(item)
+                    else:
+                        # Otherwise make a new field
+                        field = Field(
+                            name=field_name,
+                            field=item,
+                            default=item.value,
+                            annotation=item.annotation,
+                        )
+
+                        old_field = fields.get(field_name, None)
+                        if old_field:
+                            field.all_assignments.update(old_field.all_assignments)
+                        elif field.default is None:
+                            field.default = potential_defaults.get(field_name, None)
+                            field.all_assignments.update(plain_assignments[field_name])
 
                 if self.kw_only:
                     field.kw_only = True
                 elif flag_kw_only:
                     # As KW_ONLY is ignored if plain assignments are used
                     # Just flag the field to be made KW_ONLY later if no
                     # plain assignments are used
                     field._kw_only_flagged = True
 
-                fields.append(field)
+                fields[field_name] = field
+
             elif (
                 isinstance(item, ast.Assign)
                 and len(item.targets) == 1
-                and isinstance(item.value, ast.Call)
             ):
                 field_name = getattr(item.targets[0], "id")
-                field = Field.from_keywords(
-                    name=field_name, field=item, keywords=item.value.keywords
-                )
-                if self.kw_only:
-                    field.kw_only = True
 
-                fields.append(field)
+                if (
+                        isinstance(item.value, ast.Call)
+                        and funcid_or_none(item.value) == ATTRIBUTE_FUNCNAME
+                ):
+                    # This is an attribute declaration
+                    field = Field.from_keywords(
+                        name=field_name, field=item, keywords=item.value.keywords
+                    )
+                    if self.kw_only:
+                        field.kw_only = True
 
-                # If an attribute function is used in a plain assignment
-                # then the function is required for all assignments.
-                require_attribute_func = True
+                    # If there is an old field copy the annotation and all assignment list over
+                    old_field = fields.get(field_name, None)
+                    if old_field:
+                        field.annotation = old_field.annotation
+                        field.all_assignments.update(old_field.all_assignments)
+                    else:
+                        # Otherwise copy potential plain assignments over
+                        field.all_assignments.update(plain_assignments[field_name])
+
+                    fields[field_name] = field
+                else:
+                    # This is a plain value
+                    old_field = fields.get(field_name, None)
+                    if old_field:
+                        # Update the default value and add to the list of all fields
+                        old_field.default = item.value
+                        old_field.all_assignments.add(item)
+                    else:
+                        # Store the non-annotated values in case they
+                        # subsequently get annotated
+                        potential_defaults[field_name] = item.value
+                        plain_assignments[field_name].add(item)
 
-        # Clear fields that are generated just by annotations
+        # If there are any plain assignments, annotated assignments that
+        # do not use attribute() calls must be removed to match 'dynamic'
+        # behaviour. KW_ONLY should only be used if all assignments are annotated.
+        require_attribute_func = any(v.annotation is None for v in fields.values())
         if require_attribute_func:
-            fields = [field for field in fields if field.attribute_func]
+            fields = {k: v for k, v in fields.items() if v.attribute_func}
         else:
-            for field in fields:
+            # Make relevant fields kw_only if no plain assignments used
+            for field in fields.values():
                 if field._kw_only_flagged:
                     field.kw_only = True
 
-        return {field.name: field for field in fields}
+        return fields
 
     @cached_property
     def parents(self) -> list[str]:
         parents = [
             getattr(item, "id")
             for item in self.node.bases
             if getattr(item, "id") != "object"  # Ignore inheritance from object
@@ -900,41 +970,38 @@
         :param prefabs: Details on all prefabs in this module - for handling inheritance
         """
 
         # Handle inheritance
         self.resolve_inheritance(prefabs)
 
         # Remove values from the body
-        # Keep the annotated values to re-insert the annotations later
-        body_annotations = []
         for item in self.field_list:
-            if isinstance(item.field, ast.AnnAssign):
-                body_annotations.append(item.field)
-            self.node.body.remove(item.field)
-
-        if self._flag_kw_only is not None:
-            body_annotations.append(self._flag_kw_only)
-            self.node.body.remove(self._flag_kw_only)
+            for assign in item.all_assignments:
+                self.node.body.remove(assign)
 
         # Build body
         body = []
         if not self.compile_plain:
             body.append(self.compile_flag)
             body.append(self.fields_assignment)
             # body.append(self.internals_assignment)
 
         if self.compile_slots and "__slots__" not in self.defined_attr_names:
             body.append(self.slots_assignment)
         if self.match_args and "__match_args__" not in self.defined_attr_names:
             body.append(self.match_args_assignment)
 
         # Re-insert annotations
-        for item in body_annotations:
-            item.value = None
-            body.append(item)
+        for item in self.field_list:
+            if item.ast_annassign:
+                body.append(item.ast_annassign)
+
+        if self._flag_kw_only is not None:
+            self.node.body.remove(self._flag_kw_only)
+            body.append(self._flag_kw_only)
 
         if (self.init and "__init__" not in self.defined_attr_names) or not self.init:
             body.append(self.init_method)
         if self.repr and "__repr__" not in self.defined_attr_names:
             body.append(self.repr_method)
         if self.eq and "__eq__" not in self.defined_attr_names:
             body.append(self.eq_method)
```

### Comparing `prefab_classes-0.9.2/src/prefab_classes/compiled/rewrite_source.py` & `prefab_classes-0.9.3/src/prefab_classes/compiled/rewrite_source.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class.py` & `prefab_classes-0.9.3/src/prefab_classes/dynamic/_attribute_class.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py` & `prefab_classes-0.9.3/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py` & `prefab_classes-0.9.3/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/dynamic/autogen.py` & `prefab_classes-0.9.3/src/prefab_classes/dynamic/autogen.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/dynamic/method_generators.py` & `prefab_classes-0.9.3/src/prefab_classes/dynamic/method_generators.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/dynamic/prefab.py` & `prefab_classes-0.9.3/src/prefab_classes/dynamic/prefab.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/exceptions.py` & `prefab_classes-0.9.3/src/prefab_classes/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/funcs.py` & `prefab_classes-0.9.3/src/prefab_classes/funcs.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes/sentinels.py` & `prefab_classes-0.9.3/src/prefab_classes/sentinels.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes.egg-info/PKG-INFO` & `prefab_classes-0.9.3/src/prefab_classes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefab-classes
-Version: 0.9.2
+Version: 0.9.3
 Summary: Boilerplate Generator for Classes
 Author: David C Ellis
 Project-URL: Homepage, https://github.com/davidcellis/PrefabClasses
 Project-URL: Documentation, https://prefabclasses.readthedocs.io/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `prefab_classes-0.9.2/src/prefab_classes.egg-info/SOURCES.txt` & `prefab_classes-0.9.3/src/prefab_classes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.2/src/prefab_classes_hook/__init__.py` & `prefab_classes-0.9.3/src/prefab_classes_hook/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 # We probably shouldn't be importing from here, but it also halves the import time.
 try:
     from _frozen_importlib_external import PathFinder, SourceFileLoader  # type: ignore
 except ImportError:
     from importlib.machinery import PathFinder, SourceFileLoader
 
-__version__ = "v0.9.2"
-PREFAB_MAGIC_BYTES = b"PREFAB_CLASSES_v0.9.2"
+__version__ = "v0.9.3"
+PREFAB_MAGIC_BYTES = b"PREFAB_CLASSES_v0.9.3"
 
 __all__ = ["prefab_compiler", "insert_prefab_importhook", "remove_prefab_importhook"]
 
 
 HOOK_REWRITE = "# COMPILE_PREFABS"
```

