# Comparing `tmp/polymeasure-0.1.1.tar.gz` & `tmp/polymeasure-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymeasure-0.1.1.tar", last modified: Mon Jul 24 00:57:18 2023, max compression
+gzip compressed data, was "polymeasure-0.1.2.tar", last modified: Thu Jul 27 21:11:58 2023, max compression
```

## Comparing `polymeasure-0.1.1.tar` & `polymeasure-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 00:57:18.627510 polymeasure-0.1.1/
--rw-rw-rw-   0        0        0     1109 2023-07-22 12:44:08.000000 polymeasure-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5676 2023-07-24 00:57:18.627510 polymeasure-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5112 2023-07-23 11:15:31.000000 polymeasure-0.1.1/README.md
--rw-rw-rw-   0        0        0      644 2023-07-23 20:08:15.000000 polymeasure-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 00:57:18.627510 polymeasure-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 00:57:18.617511 polymeasure-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 00:57:18.622509 polymeasure-0.1.1/src/polymeasure/
--rw-rw-rw-   0        0        0      117 2023-07-22 12:44:08.000000 polymeasure-0.1.1/src/polymeasure/__init__.py
--rw-rw-rw-   0        0        0    42670 2023-07-24 00:51:10.000000 polymeasure-0.1.1/src/polymeasure/core.py
-drwxrwxrwx   0        0        0        0 2023-07-24 00:57:18.626510 polymeasure-0.1.1/src/polymeasure.egg-info/
--rw-rw-rw-   0        0        0     5676 2023-07-24 00:57:18.000000 polymeasure-0.1.1/src/polymeasure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-07-24 00:57:18.000000 polymeasure-0.1.1/src/polymeasure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 00:57:18.000000 polymeasure-0.1.1/src/polymeasure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-24 00:57:18.000000 polymeasure-0.1.1/src/polymeasure.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 21:11:58.339180 polymeasure-0.1.2/
+-rw-rw-rw-   0        0        0     1109 2023-07-22 12:44:08.000000 polymeasure-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5676 2023-07-27 21:11:58.338179 polymeasure-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5112 2023-07-23 11:15:31.000000 polymeasure-0.1.2/README.md
+-rw-rw-rw-   0        0        0      644 2023-07-27 21:09:28.000000 polymeasure-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 21:11:58.339180 polymeasure-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 21:11:58.323180 polymeasure-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 21:11:58.332180 polymeasure-0.1.2/src/polymeasure/
+-rw-rw-rw-   0        0        0      117 2023-07-22 12:44:08.000000 polymeasure-0.1.2/src/polymeasure/__init__.py
+-rw-rw-rw-   0        0        0    43122 2023-07-27 21:04:38.000000 polymeasure-0.1.2/src/polymeasure/core.py
+-rw-rw-rw-   0        0        0     2944 2023-07-27 21:09:28.000000 polymeasure-0.1.2/src/polymeasure/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:11:58.335179 polymeasure-0.1.2/src/polymeasure.egg-info/
+-rw-rw-rw-   0        0        0     5676 2023-07-27 21:11:58.000000 polymeasure-0.1.2/src/polymeasure.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-27 21:11:58.000000 polymeasure-0.1.2/src/polymeasure.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 21:11:58.000000 polymeasure-0.1.2/src/polymeasure.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-27 21:11:58.000000 polymeasure-0.1.2/src/polymeasure.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 21:11:58.337181 polymeasure-0.1.2/tests/
+-rw-rw-rw-   0        0        0      405 2023-07-24 01:15:59.000000 polymeasure-0.1.2/tests/test.py
```

### Comparing `polymeasure-0.1.1/LICENSE` & `polymeasure-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polymeasure-0.1.1/PKG-INFO` & `polymeasure-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymeasure
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python analysis package for building SQL expressions.
 Author-email: Josh Grant <jagmanjg@gmail.com>
 Project-URL: Homepage, https://github.com/jgrant-the-giant/polymeasure
 Project-URL: Bug Tracker, https://github.com/jgrant-the-giant/polymeasure/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `polymeasure-0.1.1/README.md` & `polymeasure-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `polymeasure-0.1.1/pyproject.toml` & `polymeasure-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polymeasure"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Josh Grant", email="jagmanjg@gmail.com" },
 ]
 description = "A python analysis package for building SQL expressions."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `polymeasure-0.1.1/src/polymeasure/core.py` & `polymeasure-0.1.2/src/polymeasure/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 def constant(value):
     def func():
         return value
 
     return func
 
 
-def make_as_list(maybe_vector, de_null=True, keep_none=False):
+def make_as_list(maybe_vector, filter_out_null=True, keep_none=False):
     if maybe_vector is None and not keep_none:
         maybe_null_vector = []
     elif maybe_vector is None and keep_none:
         return None
     elif isinstance(maybe_vector, str) and len(maybe_vector) == 0:
         maybe_null_vector = []
     elif isinstance(maybe_vector, list):
         maybe_null_vector = maybe_vector
     else:
         maybe_null_vector = [maybe_vector]
-    return [x for x in maybe_null_vector if x is not None or not de_null]
+    return [x for x in maybe_null_vector if x is not None or not filter_out_null]
 
 
 def make_statement(prefix, elements, separator=', \n', brackets=False, if_blank=''):
     """
     Returns a string expression like "prefix a1, a2, a3" with optional prefix, optional brackets, etc
     Args:
         prefix: prefix like select, where, etc)
@@ -101,15 +101,19 @@
         Args:
             include: list of strings
             exclude: list of strings
 
         Returns: boolean
 
         """
-        include_all = (len(include) == 0)
+        if include is None:
+            include_all = True
+            include = []
+        else:
+            include_all = False
 
         if self.source is not None and source is not None and not source in self.source:
             return False
 
         if len(self.lineage) == 0 and len(self.group_lineage) == 0:
             return True
 
@@ -203,24 +207,27 @@
             rows: Columns to return (defaults to args)
             star: Star string expression
         """
 
         if star is not None:
             dimensions = None
 
+        # Null dimension defaults to star expression
+        if dimensions is None:
+            star = True
+
         super(Rowset, self).__init__(dimensions=dimensions, rowset=True, star=star)
 
 
 class PolyMeasure:
 
     @staticmethod
     def _do_nothing(self, *args, **kwargs):
         return None
 
-
     @staticmethod
     def dimensional_join_primitive(column, outer_alias, inner, join_nulls):
         """
         Returns a string function returning join operators to connect inner measurements together.
         Args:
             column: What dimensions to connect on
             outer_alias: Outer alias to encode into this join primitive - future measures know to connect to this source
@@ -242,47 +249,46 @@
         return FilterExpression(expression_function, column, inner)
 
     @staticmethod
     def _parse_dim_argument(maybe_dimension):
         if isinstance(maybe_dimension, (tuple, list)):
             return_dim = Dimension(dimensions=maybe_dimension, rowset=False, star=False)
         elif isinstance(maybe_dimension, Dimension):
-            return_dim =  maybe_dimension
+            return_dim = maybe_dimension
         elif isinstance(maybe_dimension, str):
-            return_dim =  Dimension(dimensions=[maybe_dimension], rowset=False, star=False)
+            return_dim = Dimension(dimensions=[maybe_dimension], rowset=False, star=False)
         else:
             # wildcard dimension
-            return_dim =  Dimension(dimensions=None, rowset=False, star=False)
+            return_dim = Dimension(dimensions=[], rowset=False, star=False)
 
         return return_dim
 
-
     def _get_primitive_expression(self, inner_alias=None, override_name=None, update_columns=False):
 
         override_name = override_name if override_name is not None else self.name
         if len(self.outer) == 0:
             outer_primitive_expressions = []
         elif isinstance(self.outer[0], FunctionType):
             if update_columns:
-                outer_primitive_expressions = [override_name + ' = ' + self.outer[0](self=self, inner_alias=inner_alias)]
+                outer_primitive_expressions = [
+                    override_name + ' = ' + self.outer[0](self=self, inner_alias=inner_alias)]
             else:
                 outer_primitive_expressions = [self.outer[0](self=self, inner_alias=inner_alias) + ' ' + override_name]
         else:
             if update_columns:
                 outer_primitive_expressions = [override_name + ' = ' + self.outer[0]]
             else:
                 outer_primitive_expressions = [self.outer[0] + ' ' + override_name]
         return outer_primitive_expressions
 
     def _get_final_columnset(self):
         # Returns a list of columns including dimensions and outer measure names
         outer_dimension_list = self.outer_dimension.dimensions if self.outer_dimension.dimensions else []
         return outer_dimension_list + self.final_outer_columns
 
-
     def _process_where_argument(self, where):
         where_list = [self._get_filter(expression) for expression in make_as_list(where)]
         where_list = [filter_object for filter_object in where_list if filter_object is not None]
         return where_list
 
     @staticmethod
     def _check_primitive(measure_object):
@@ -303,22 +309,20 @@
             raise Exception
 
     def rename(self, name):
         measure_clone = copy(self)
         measure_clone.name = name
         return measure_clone
 
-
     def add_where(self, where):
         where = self._process_where_argument(where)
         measure_clone = copy(self)
         measure_clone.where = measure_clone.where + where
         return measure_clone
 
-
     @staticmethod
     def _to_polymeasure(measure_object):
         """
         Converts an object of flexible type into name and query data
         Args:
             measure_object:
 
@@ -345,23 +349,21 @@
             else:
                 measure = PolyMeasure(measure_object[0], measure_object[1], measure_object[2])
             return measure
         else:
             # There's no way to form a query so raise an error
             raise Exception
 
-
     def _get_filter(self, filter_object):
         """
-        Converts an object of flexible type into name and query data
+        Converts an object of flexible type into a FilterExpression
         Args:
-            measure:
+            filter_object: string or tuple
 
-        Returns:
-        Internal dummy class with necessary properties
+        Returns: FilterExpression
         """
 
         if isinstance(filter_object, str):
             return FilterExpression(filter_object, source=self.inner)
         elif isinstance(filter_object, FilterExpression):
             return filter_object
         elif isinstance(filter_object, (tuple, list)) and len(filter_object) > 0:
@@ -369,15 +371,14 @@
                 return FilterExpression(filter_object[0], lineage=None, source=self.inner)
             else:
                 return FilterExpression(*filter_object[:3])
         else:
             # Improperly formatted filter
             return None
 
-
     def __init__(
             self,
             name=None,
             outer=None,
             dim=None,
             inner=None,
             where=None, having=None, order_by=None, postfix=None,
@@ -548,15 +549,15 @@
 
         # Convert the dimensional argument to a Dimension object
         self.dim = self._parse_dim_argument(dim)
 
         self.having = having
         self.order_by = order_by
         self.postfix = postfix
-        self.include = make_as_list(include)
+        self.include = make_as_list(include, keep_none=True)
         self.exclude = make_as_list(exclude)
         self.join_nulls = join_nulls
         self.acquire_dimensions = acquire_dimensions
         self.redirect = redirect
         self.suppress_from = suppress_from
 
         """     
@@ -591,30 +592,29 @@
 
         # Create where FilterExpression objects (now that self.inner is defined)
         self.where = self._process_where_argument(where)
 
         # Determine the outer dimension
 
         if self.primitive:
-            self.outer = make_as_list(outer, de_null=True)
+            self.outer = make_as_list(outer, filter_out_null=True)
             self.outer_dimension = self.dim
         else:
             # The program would rather expire than put an invalid object inside outer and outer_dimension.
             self.outer = [self._to_polymeasure(measure) for measure in make_as_list(outer)]
             self.outer_dimension = self.dim
 
             if self.acquire_dimensions:
                 for measure in self.outer:
                     # For each outer measure collect the dimensions as named
                     # (the designer should ensure they are unique strings or duckdb will mangle)
                     # All the objects involved in this step should involve Dimenion objects which can handle the None
                     # and rowset silliness.
                     self.outer_dimension = self.outer_dimension.absorb_new_dimension(measure.outer_dimension)
 
-
         # This is quite rare - acquire the inner dimension if none was supplied from the left
         # (outer dimensions + self.dim)
         if not self.source and self.outer_dimension.rowset \
                 and self.outer_dimension.wildcard \
                 and self.inner is not None \
                 and self.inner.outer_dimension is not None:
             # self.outer_dimension = self.outer_dimension.absorb_new_dimension(self.inner.outer_dimension)
@@ -623,15 +623,14 @@
             #         [measure.name for measure in self.inner.outer], rowset=False
             #     )
             # )
             self.outer_dimension = self.outer_dimension.absorb_new_dimension(
                 Dimension(self.inner._get_final_columnset())
             )
 
-
         self.final_outer_columns = self._get_primitive_sql_names()
 
         pass
 
     def evaluate(
             self, where=None, pretty=False, update_columns=False):
 
@@ -725,15 +724,15 @@
         if star_expression is not None and star_expression:
             groupby_dimensions = [star_expression]
         else:
             groupby_dimensions = evaluate_dimensions if allow_grouping else []
 
         # null queries have well defined inner measures but they do not have a select statement from them..
         is_null_query = (wildcard_dimensions.dimensions is None and not wildcard_dimensions.rowset) and (
-            self.outer_dimension.wildcard and not self.outer_dimension.rowset)
+                self.outer_dimension.wildcard and not self.outer_dimension.rowset)
 
         # Treat this query as a source query, do not alias the final from statement
         evaluate_as_source = self._check_primitive(evaluate_inner) or is_null_query
 
         # filter these where statements using include/exclude and dimensionality
         # These where statements are given to outer and inner measures
         # self.where are added in afterwards..
@@ -754,15 +753,15 @@
             if expression.source != self.inner or bool(set(expression.lineage) & set(evaluate_dimensions))
         ]
 
         # Finally, only actually evaluate these filters if their inner statements are matched
         evaluate_where = [
             expression for expression in passthrough_where if (
                 expression.test_keep_filter(
-                    [], [], evaluate_inner
+                    None, [], evaluate_inner
                 )
             )
         ]
 
         # Calculate the dimensional join objects to be supplied to sub measures
         # This is done inside _evaluate, rather than _generate_primitive_sql, as only one group by is performed no matter
         # how many nested measures are created
@@ -856,16 +855,16 @@
                 evaluate_sql = f"{override_name} = ({evaluate_sql})"
             else:
                 # regular aliasing
                 evaluate_sql = f"({evaluate_sql}) {override_name}"
 
         return evaluate_sql
 
-
-    def _get_primitive_sql_list(self, where, depth, breadth, wildcard_inner, wildcard_dimensions, original_alias=None, update_columns=False):
+    def _get_primitive_sql_list(self, where, depth, breadth, wildcard_inner, wildcard_dimensions, original_alias=None,
+                                update_columns=False):
         """
         Returns a list of SQL select expressions built recursively from each primitive measure in self.outer.
 
         Args:
             where: The where filter clause context inherited from the parent measure, to be combined with self.where
             depth: The current integer depth of the subquery
             wildcard_inner: The inner clause inherited from the parent measure
@@ -939,16 +938,14 @@
                     passthrough_where + measure.where,
                     depth, breadth, wildcard_inner, wildcard_dimensions,
                     original_alias=original_alias, update_columns=update_columns
                 )
 
         return primitive_sql_list
 
-
-
     def _get_primitive_sql_names(self):
         """
         Returns a list of names of descendent outer measure names, used on initialisation.
         """
 
         primitive_sql_names = []
 
@@ -961,28 +958,29 @@
                     primitive_sql_names = primitive_sql_names + [measure.name]
                 else:
                     primitive_sql_names = primitive_sql_names + measure._get_primitive_sql_names()
 
         return primitive_sql_names
 
 
-
 def bound_objects(source):
     class BoundMeasure(PolyMeasure):
 
         def __init__(
                 self,
-                name, outer=None, dim=None, inner=None,
+                name=None, outer=None, dim=None, inner=None,
                 where=None, having=None, order_by=None, postfix=None,
-                include=None, exclude=None, join_nulls=True
+                include=None, exclude=None, join_nulls=True, acquire_dimensions=False,
+                redirect=None, suppress_from=False
         ):
             super().__init__(
-                name, outer=outer, dim=dim, inner=source, where=where, having=having,
-                order_by=order_by, postfix=postfix, include=include, exclude=exclude, join_nulls=join_nulls
+                name=name, outer=outer, dim=dim, inner=source, where=where, having=having,
+                order_by=order_by, postfix=postfix, include=include, exclude=exclude, join_nulls=join_nulls,
+                acquire_dimensions=acquire_dimensions, redirect=redirect, suppress_from=suppress_from
             )
 
     class BoundFilter(FilterExpression):
 
         def __init__(self, expression, lineage=None, group_lineage=None):
             super().__init__(expression, lineage=lineage, source=source, group_lineage=group_lineage)
 
-    return BoundMeasure, BoundFilter
+    return BoundMeasure, BoundFilter
```

### Comparing `polymeasure-0.1.1/src/polymeasure.egg-info/PKG-INFO` & `polymeasure-0.1.2/src/polymeasure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymeasure
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python analysis package for building SQL expressions.
 Author-email: Josh Grant <jagmanjg@gmail.com>
 Project-URL: Homepage, https://github.com/jgrant-the-giant/polymeasure
 Project-URL: Bug Tracker, https://github.com/jgrant-the-giant/polymeasure/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

