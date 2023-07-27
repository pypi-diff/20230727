# Comparing `tmp/graphql_query-1.1.1.tar.gz` & `tmp/graphql_query-1.2.0.tar.gz`

## Comparing `graphql_query-1.1.1.tar` & `graphql_query-1.2.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.editorconfig
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 graphql_query-1.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 graphql_query-1.1.1/Makefile
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 graphql_query-1.1.1/SECURITY.md
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/workflows/check.yaml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/workflows/static.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/make.bat
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/api.rst
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/conf.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/examples.rst
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/index.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/intro.rst
--rw-r--r--   0        0        0    12568 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/usage.rst
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/examples/list_of_objects.rst
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/examples/with_gql.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/__info__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/__version__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/py.typed
--rw-r--r--   0        0        0    18575 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/types.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_argument.jinja2
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_arguments.jinja2
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_objects.jinja2
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_value.jinja2
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_values.jinja2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_variable.jinja2
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/directive.jinja2
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/field.jinja2
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/fragment.jinja2
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/inline_fragment.jinja2
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/operation.jinja2
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/query.jinja2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/variable.jinja2
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 graphql_query-1.1.1/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 graphql_query-1.1.1/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 graphql_query-1.1.1/requirements/requirements-test.txt
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 graphql_query-1.1.1/requirements/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/data.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_directive.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_exist_templates.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_field.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_fragment.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_graphql2python_query.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_inline_fragment.py
--rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_operation.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/arguments/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/arguments/data_arguments.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/arguments/test_arguments.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_argument/__init__.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_argument/test_argument.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_variable/__init__.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_variable/test_variable.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 graphql_query-1.1.1/LICENSE
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 graphql_query-1.1.1/README.md
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 graphql_query-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 graphql_query-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 graphql_query-1.2.0/.editorconfig
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 graphql_query-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 graphql_query-1.2.0/Makefile
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 graphql_query-1.2.0/SECURITY.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 graphql_query-1.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 graphql_query-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 graphql_query-1.2.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 graphql_query-1.2.0/.github/workflows/check.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 graphql_query-1.2.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 graphql_query-1.2.0/.github/workflows/static.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 graphql_query-1.2.0/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 graphql_query-1.2.0/docs/make.bat
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 graphql_query-1.2.0/docs/source/api.rst
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 graphql_query-1.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graphql_query-1.2.0/docs/source/examples.rst
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 graphql_query-1.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 graphql_query-1.2.0/docs/source/intro.rst
+-rw-r--r--   0        0        0    12568 2020-02-02 00:00:00.000000 graphql_query-1.2.0/docs/source/usage.rst
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 graphql_query-1.2.0/docs/source/examples/list_of_objects.rst
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 graphql_query-1.2.0/docs/source/examples/with_gql.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/__info__.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/__version__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/py.typed
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates.py
+-rw-r--r--   0        0        0    18164 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/types.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/argument_key_argument.jinja2
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/argument_key_arguments.jinja2
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/argument_key_objects.jinja2
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/argument_key_value.jinja2
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/argument_key_values.jinja2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/argument_key_variable.jinja2
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/directive.jinja2
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/field.jinja2
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/fragment.jinja2
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/inline_fragment.jinja2
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/operation.jinja2
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/query.jinja2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graphql_query-1.2.0/graphql_query/templates/variable.jinja2
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 graphql_query-1.2.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 graphql_query-1.2.0/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 graphql_query-1.2.0/requirements/requirements-test.txt
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 graphql_query-1.2.0/requirements/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/data.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_directive.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_exist_templates.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_field.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_fragment.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_graphql2python_query.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_inline_fragment.py
+-rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_operation.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/arguments/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/arguments/data_arguments.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/arguments/test_arguments.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_argument/__init__.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_argument/test_argument.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_variable/__init__.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 graphql_query-1.2.0/tests/test_variable/test_variable.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 graphql_query-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 graphql_query-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 graphql_query-1.2.0/README.md
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 graphql_query-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 graphql_query-1.2.0/PKG-INFO
```

### Comparing `graphql_query-1.1.1/CONTRIBUTING.md` & `graphql_query-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/Makefile` & `graphql_query-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `graphql_query-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/.github/workflows/check.yaml` & `graphql_query-1.2.0/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/.github/workflows/static.yaml` & `graphql_query-1.2.0/.github/workflows/static.yaml`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/docs/Makefile` & `graphql_query-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/docs/make.bat` & `graphql_query-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/docs/source/conf.py` & `graphql_query-1.2.0/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'graphql_query'
 copyright = '2022-2023, Denis A. Artyushin'
 author = 'Denis A. Artyushin'
-version = '1.1.1'
+version = '1.2.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinxarg.ext',
     'sphinx.ext.autodoc',
```

### Comparing `graphql_query-1.1.1/docs/source/index.rst` & `graphql_query-1.2.0/docs/source/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 .. image:: https://img.shields.io/github/v/tag/denisart/graphql-query
   :alt: tag
 .. image:: https://img.shields.io/github/last-commit/denisart/graphql-query/master
   :alt: last-commit
 .. image:: https://img.shields.io/github/license/denisart/graphql-query
   :alt: license
 
-**graphql_query** is complete GraphQL query string builder for python. With **graphql_query**
+**graphql_query** is complete GraphQL query string builder for python (based on pydantic v2). With **graphql_query**
 you can
 
 - generate a GraphQL query string from a python class;
 - use and share similar Arguments, Variables and e.t.c between different queries;
 - easily add new fields to your query;
 - add Fragments and Directives to queries;
```

### Comparing `graphql_query-1.1.1/docs/source/usage.rst` & `graphql_query-1.2.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/docs/source/examples/list_of_objects.rst` & `graphql_query-1.2.0/docs/source/examples/list_of_objects.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/docs/source/examples/with_gql.rst` & `graphql_query-1.2.0/docs/source/examples/with_gql.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/graphql_query/__init__.py` & `graphql_query-1.2.0/graphql_query/__init__.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/graphql_query/types.py` & `graphql_query-1.2.0/graphql_query/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,29 @@
-import os
 import sys
-from pathlib import Path
 from typing import Any, List, Optional, Union
 
-from jinja2 import Environment, FileSystemLoader, Template
-from pydantic import BaseModel
+from pydantic import BaseModel as PydanticBaseModel
 from pydantic import Field as PydanticField
 
+from .templates import (
+    _template_key_value,
+    _template_key_values,
+    _template_key_argument,
+    _template_key_variable,
+    _template_key_arguments,
+    _template_key_objects,
+    _template_directive,
+    _template_variable,
+    _template_operation,
+    _template_query,
+    _template_fragment,
+    _template_inline_fragment,
+    _template_field,
+)
+
 if sys.version_info >= (3, 10):
     from typing import TypeGuard
 else:
     # Use TypeGuard from typing_extensions for python <= 3.9
     from typing_extensions import TypeGuard
 
 __all__ = [
@@ -21,29 +34,20 @@
     "InlineFragment",
     "Fragment",
     "Query",
     "Operation",
 ]
 
 
-# templates setting for render of classes
-TEMPLATES_FOLDER = Path(os.path.join(os.path.dirname(__file__), "templates/"))
-
-template_env = Environment(loader=FileSystemLoader(searchpath=TEMPLATES_FOLDER))
-
-
-class _GraphQL2PythonQuery(BaseModel):
+class _GraphQL2PythonQuery(PydanticBaseModel):
     """An abstract class for GraphQL query type."""
 
     class Config:
-        # pylint: disable=too-few-public-methods
-        smart_union = True
         extra = "forbid"
         arbitrary_types_allowed = True
-        allow_reuse = True
 
     @staticmethod
     def _line_shift(text: str) -> str:
         return "\n  ".join(text.split("\n"))
 
     def _render_field(self, field: Union[str, 'Field', 'InlineFragment', 'Fragment']) -> str:
         if isinstance(field, str):
@@ -89,22 +93,20 @@
 
     """
 
     name: str
     type: str
     default: Optional[str] = PydanticField(default=None)
 
-    _template: Template = template_env.get_template("variable.jinja2")
-
     def render(self) -> str:
-        return self._template.render(name=self.name, type=self.type, default=self.default)
+        return _template_variable.render(name=self.name, type=self.type, default=self.default)
 
 
 class Argument(_GraphQL2PythonQuery):
-    """GraphQL argument type.
+    """GraphQL Argument type.
 
     See https://graphql.org/learn/queries/#arguments for more details.
 
     Attributes:
         name: A name of the argument.
         value: The argument value.
 
@@ -160,86 +162,106 @@
 
     """
 
     name: str
     value: Union[
         str,
         int,
+        bool,
         'Argument',
         Variable,
         List[str],
         List[int],
+        List[bool],
         List['Argument'],
         List[List['Argument']],
     ]
 
-    _template_key_value: Template = template_env.get_template("argument_key_value.jinja2")
-    _template_key_values: Template = template_env.get_template("argument_key_values.jinja2")
-    _template_key_argument: Template = template_env.get_template("argument_key_argument.jinja2")
-    _template_key_variable: Template = template_env.get_template("argument_key_variable.jinja2")
-    _template_key_arguments: Template = template_env.get_template("argument_key_arguments.jinja2")
-    _template_key_objects: Template = template_env.get_template("argument_key_objects.jinja2")
-
     @staticmethod
     def _check_is_list_of_str(values: List[Any]) -> TypeGuard[List[str]]:
         return all(isinstance(value, str) for value in values)
 
     @staticmethod
+    def _check_is_list_of_int(values: List[Any]) -> TypeGuard[List[int]]:
+        return all(isinstance(value, int) for value in values)
+
+    @staticmethod
+    def _check_is_list_of_bool(values: List[Any]) -> TypeGuard[List[bool]]:
+        return all(isinstance(value, bool) for value in values)
+
+    @staticmethod
     def _check_is_list_of_arguments(values: List[Any]) -> TypeGuard[List['Argument']]:
         return all(isinstance(value, Argument) for value in values)
 
     @staticmethod
     def _check_is_list_of_list(values: List[Any]) -> TypeGuard[List[List[Any]]]:
         return all(isinstance(value, list) for value in values)
 
-    def _render_for_str(self, name: str, value: str) -> str:
-        return self._template_key_value.render(name=name, value=value)
+    @staticmethod
+    def _render_for_str(name: str, value: str) -> str:
+        return _template_key_value.render(name=name, value=value)
 
-    def _render_for_int(self, name: str, value: int) -> str:
-        return self._template_key_value.render(name=name, value=str(value))
+    @staticmethod
+    def _render_for_int(name: str, value: int) -> str:
+        return _template_key_value.render(name=name, value=str(value))
 
-    def _render_for_argument(self, name: str, value: 'Argument') -> str:
-        return self._template_key_argument.render(name=name, argument=self._line_shift(value.render()))
+    @staticmethod
+    def _render_for_list_str(name: str, value: List[str]) -> str:
+        return _template_key_values.render(name=name, values=value)
+
+    @staticmethod
+    def _render_for_list_bool(name: str, value: List[bool]) -> str:
+        return _template_key_values.render(name=name, values=[str(v).lower() for v in value])
 
-    def _render_for_list_str(self, name: str, value: List[str]) -> str:
-        return self._template_key_values.render(name=name, values=value)
+    @staticmethod
+    def _render_for_variable(name: str, value: Variable) -> str:
+        return _template_key_variable.render(name=name, value=value.name)
+
+    def _render_for_argument(self, name: str, value: 'Argument') -> str:
+        return _template_key_argument.render(name=name, argument=self._line_shift(value.render()))
 
     def _render_for_list_argument(self, name: str, value: List['Argument']) -> str:
-        return self._template_key_arguments.render(
+        return _template_key_arguments.render(
             name=name, arguments=[self._line_shift(argument.render()) for argument in value]
         )
 
     def _render_for_list_list_argument(self, name: str, value: List[List['Argument']]) -> str:
-        return self._template_key_objects.render(
+        return _template_key_objects.render(
             name=name,
             list_arguments=[
                 [self._line_shift(self._line_shift(argument.render())) for argument in arguments] for arguments in value
             ],
         )
 
-    def _render_for_variable(self, name: str, value: Variable) -> str:
-        return self._template_key_variable.render(name=name, value=value.name)
-
     def render(self) -> str:
         if isinstance(self.value, str):
             return self._render_for_str(self.name, self.value)
 
+        if isinstance(self.value, bool):
+            return self._render_for_str(self.name, str(self.value).lower())
+
         if isinstance(self.value, int):
             return self._render_for_int(self.name, self.value)
 
         if isinstance(self.value, Argument):
             return self._render_for_argument(self.name, self.value)
 
         if isinstance(self.value, Variable):
             return self._render_for_variable(self.name, self.value)
 
         if isinstance(self.value, list):
             if self._check_is_list_of_str(self.value):
                 return self._render_for_list_str(self.name, self.value)
 
+            if self._check_is_list_of_bool(self.value):
+                return self._render_for_list_bool(self.name, self.value)
+
+            if self._check_is_list_of_int(self.value):
+                return self._render_for_list_str(self.name, [str(v) for v in self.value])
+
             if self._check_is_list_of_arguments(self.value):
                 return self._render_for_list_argument(self.name, self.value)
 
             if self._check_is_list_of_list(self.value):
                 if all(self._check_is_list_of_arguments(v) for v in self.value):
                     return self._render_for_list_list_argument(self.name, self.value)
 
@@ -281,19 +303,18 @@
         ... )
 
     """
 
     name: str
     arguments: List[Argument] = PydanticField(default_factory=list)
 
-    _template_directive: Template = template_env.get_template("directive.jinja2")
-
     def render(self) -> str:
-        return self._template_directive.render(
-            name=self.name, arguments=[self._line_shift(argument.render()) for argument in self.arguments]
+        return _template_directive.render(
+            name=self.name,
+            arguments=[self._line_shift(argument.render()) for argument in self.arguments],
         )
 
 
 class Field(_GraphQL2PythonQuery):
     """GraphQL Field type.
 
     See https://graphql.org/learn/queries/#fields for more details.
@@ -347,18 +368,16 @@
     name: str
     alias: Optional[str] = PydanticField(default=None)
     arguments: List[Argument] = PydanticField(default_factory=list)
     fields: List[Union[str, 'Field', 'InlineFragment', 'Fragment']] = PydanticField(default_factory=list)
     directives: List[Directive] = PydanticField(default_factory=list)
     typename: bool = PydanticField(default=False, description="Add meta field `__typename` to sub-fields.")
 
-    _template: Template = template_env.get_template("field.jinja2")
-
     def render(self) -> str:
-        return self._template.render(
+        return _template_field.render(
             name=self.name,
             alias=self.alias,
             arguments=[self._line_shift(argument.render()) for argument in self.arguments],
             fields=[self._render_field(field) for field in self.fields],
             directives=[directive.render() for directive in self.directives],
             typename=self.typename,
         )
@@ -401,18 +420,16 @@
     """
 
     type: str
     arguments: List[Argument] = PydanticField(default_factory=list)
     fields: List[Union[str, 'Field', 'InlineFragment', 'Fragment']] = PydanticField(default_factory=list)
     typename: bool = PydanticField(default=False, description="Add meta field `__typename` to sub-fields.")
 
-    _template: Template = template_env.get_template("inline_fragment.jinja2")
-
     def render(self) -> str:
-        return self._template.render(
+        return _template_inline_fragment.render(
             type=self.type,
             arguments=[self._line_shift(argument.render()) for argument in self.arguments],
             fields=[self._render_field(field) for field in self.fields],
             typename=self.typename,
         )
 
 
@@ -461,18 +478,16 @@
     """
 
     name: str
     type: str
     fields: List[Union[str, 'Field', 'InlineFragment', 'Fragment']] = PydanticField(default_factory=list)
     typename: bool = PydanticField(default=False, description="Add meta field `__typename` to sub-fields")
 
-    _template: Template = template_env.get_template("fragment.jinja2")
-
     def render(self) -> str:
-        return self._template.render(
+        return _template_fragment.render(
             name=self.name,
             type=self.type,
             fields=[self._render_field(field) for field in self.fields],
             typename=self.typename,
         )
 
 
@@ -516,28 +531,26 @@
 
     name: str
     alias: Optional[str] = PydanticField(default=None)
     arguments: List[Argument] = PydanticField(default_factory=list)
     typename: bool = PydanticField(default=False, description="Add meta field `__typename` to the query.")
     fields: List[Union[str, 'Field', 'InlineFragment', 'Fragment']] = PydanticField(default_factory=list)
 
-    _template: Template = template_env.get_template("query.jinja2")
-
     def render(self) -> str:
-        return self._template.render(
+        return _template_query.render(
             name=self.name,
             alias=self.alias,
             arguments=[self._line_shift(argument.render()) for argument in self.arguments],
             typename=self.typename,
             fields=[self._render_field(field) for field in self.fields],
         )
 
 
 class Operation(_GraphQL2PythonQuery):
-    """GraphQL operation type.
+    """GraphQL Operation type.
 
     See https://graphql.org/learn/queries/ for more details.
 
     Attributes:
         type: A operation type.
         name: An optional operation name.
         variables: All operation variables.
@@ -586,27 +599,15 @@
         default_factory=list, description="https://graphql.org/learn/queries/#fragments"
     )
     queries: List[Query] = PydanticField(default_factory=list, description="Queries for this GraphQL operation.")
     fragments: List[Fragment] = PydanticField(
         default_factory=list, description="https://graphql.org/learn/queries/#fragments"
     )
 
-    _template: Template = template_env.get_template("operation.jinja2")
-    _supported_types = ["query", "mutation", "subscription"]
-
     def render(self) -> str:
-        return self._template.render(
+        return _template_operation.render(
             type=self.type,
             name=self.name,
             variables=[self._line_shift(variable.render()) for variable in self.variables],
             queries=[self._line_shift(query.render()) for query in self.queries],
             fragments=[fragment.render() for fragment in self.fragments],
         )
-
-
-Variable.update_forward_refs()
-Argument.update_forward_refs()
-Field.update_forward_refs()
-InlineFragment.update_forward_refs()
-Fragment.update_forward_refs()
-Query.update_forward_refs()
-Operation.update_forward_refs()
```

### Comparing `graphql_query-1.1.1/requirements/requirements-dev.txt` & `graphql_query-1.2.0/requirements/requirements-dev.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,73 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=requirements/requirements-dev.txt --resolver=backtracking pyproject.toml
 #
-astroid==2.15.5
+annotated-types==0.5.0
+    # via pydantic
+astroid==2.15.6
     # via pylint
-black==23.3.0
+black==23.7.0
     # via graphql_query (pyproject.toml)
-click==8.1.3
+click==8.1.6
     # via black
-dill==0.3.6
+dill==0.3.7
     # via pylint
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
     # via graphql_query (pyproject.toml)
 lazy-object-proxy==1.9.0
     # via astroid
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 mccabe==0.7.0
     # via pylint
-mypy==1.3.0
+mypy==1.4.1
     # via graphql_query (pyproject.toml)
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
 packaging==23.1
     # via black
 pathspec==0.11.1
     # via black
-platformdirs==3.5.1
+platformdirs==3.9.1
     # via
     #   black
     #   pylint
-pydantic==1.10.8
+pydantic==2.1.1
     # via
     #   graphql_query (pyproject.toml)
     #   pylint-pydantic
-pylint==2.17.4
+pydantic-core==2.4.0
+    # via pydantic
+pylint==2.17.5
     # via
     #   pylint-plugin-utils
     #   pylint-pydantic
 pylint-plugin-utils==0.8.2
     # via pylint-pydantic
-pylint-pydantic==0.1.8
+pylint-pydantic==0.2.4
     # via graphql_query (pyproject.toml)
-ruff==0.0.270
+ruff==0.0.280
     # via graphql_query (pyproject.toml)
 tomli==2.0.1
     # via
     #   black
     #   mypy
     #   pylint
-tomlkit==0.11.8
+tomlkit==0.12.0
     # via pylint
-typing-extensions==4.6.2
+typing-extensions==4.7.1
     # via
     #   astroid
     #   mypy
     #   pydantic
-wheel==0.40.0
+    #   pydantic-core
+wheel==0.41.0
     # via graphql_query (pyproject.toml)
 wrapt==1.15.0
     # via astroid
```

### Comparing `graphql_query-1.1.1/requirements/requirements-docs.txt` & `graphql_query-1.2.0/requirements/requirements-docs.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=docs --output-file=requirements/requirements-docs.txt --resolver=backtracking pyproject.toml
 #
 alabaster==0.7.13
     # via sphinx
+annotated-types==0.5.0
+    # via pydantic
 babel==2.12.1
     # via sphinx
-certifi==2023.5.7
+certifi==2023.7.22
     # via requests
 cffi==1.15.1
     # via cryptography
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-cryptography==41.0.0
+cryptography==41.0.2
     # via pyjwt
 docutils==0.18.1
     # via
     #   sphinx
     #   sphinx-rtd-theme
 github3-py==4.0.1
     # via sphinxcontrib-github
@@ -26,25 +28,27 @@
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via
     #   graphql_query (pyproject.toml)
     #   sphinx
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 packaging==23.1
     # via sphinx
 pycparser==2.21
     # via cffi
-pydantic==1.10.8
+pydantic==2.1.1
     # via graphql_query (pyproject.toml)
+pydantic-core==2.4.0
+    # via pydantic
 pygments==2.15.1
     # via sphinx
-pyjwt[crypto]==2.7.0
+pyjwt[crypto]==2.8.0
     # via github3-py
 python-dateutil==2.8.2
     # via github3-py
 requests==2.31.0
     # via
     #   github3-py
     #   sphinx
@@ -57,15 +61,15 @@
     #   graphql_query (pyproject.toml)
     #   sphinx-argparse
     #   sphinx-rtd-theme
     #   sphinxcontrib-github
     #   sphinxcontrib-jquery
 sphinx-argparse==0.4.0
     # via graphql_query (pyproject.toml)
-sphinx-rtd-theme==1.2.1
+sphinx-rtd-theme==1.2.2
     # via graphql_query (pyproject.toml)
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-github==0.1.3
     # via graphql_query (pyproject.toml)
@@ -75,13 +79,15 @@
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-typing-extensions==4.6.2
-    # via pydantic
+typing-extensions==4.7.1
+    # via
+    #   pydantic
+    #   pydantic-core
 uritemplate==4.1.1
     # via github3-py
-urllib3==2.0.2
+urllib3==2.0.4
     # via requests
```

### Comparing `graphql_query-1.1.1/requirements/requirements-test.txt` & `graphql_query-1.2.0/requirements/requirements-test.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/requirements-test.txt --resolver=backtracking pyproject.toml
 #
+annotated-types==0.5.0
+    # via pydantic
 coverage[toml]==7.2.7
     # via pytest-cov
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via pytest
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via graphql_query (pyproject.toml)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
 packaging==23.1
     # via pytest
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
-pydantic==1.10.8
+pydantic==2.1.1
     # via graphql_query (pyproject.toml)
-pytest==7.3.1
+pydantic-core==2.4.0
+    # via pydantic
+pytest==7.4.0
     # via
     #   graphql_query (pyproject.toml)
     #   pytest-cov
     #   pytest-mock
 pytest-cov==4.1.0
     # via graphql_query (pyproject.toml)
-pytest-mock==3.10.0
+pytest-mock==3.11.1
     # via graphql_query (pyproject.toml)
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-typing-extensions==4.6.2
-    # via pydantic
+typing-extensions==4.7.1
+    # via
+    #   pydantic
+    #   pydantic-core
```

### Comparing `graphql_query-1.1.1/tests/data.py` & `graphql_query-1.2.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/tests/test_directive.py` & `graphql_query-1.2.0/tests/test_directive.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/tests/test_exist_templates.py` & `graphql_query-1.2.0/tests/test_exist_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from jinja2 import Template
 
-from graphql_query.types import template_env
+from graphql_query.templates import template_env
 
 
 @pytest.mark.parametrize(
     "template_name",
     [
         # for Variable
         "variable.jinja2",
```

### Comparing `graphql_query-1.1.1/tests/test_field.py` & `graphql_query-1.2.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/tests/test_fragment.py` & `graphql_query-1.2.0/tests/test_fragment.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/tests/test_inline_fragment.py` & `graphql_query-1.2.0/tests/test_inline_fragment.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/tests/test_operation.py` & `graphql_query-1.2.0/tests/test_operation.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/tests/test_query.py` & `graphql_query-1.2.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/tests/arguments/data_arguments.py` & `graphql_query-1.2.0/tests/arguments/data_arguments.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/tests/test_argument/test_argument.py` & `graphql_query-1.2.0/tests/test_argument/test_argument.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,26 +12,37 @@
 
 def test_value_is_int():
     assert Argument(name="length", value=911).render() == 'length: 911'
     assert Argument(name="length", value=0).render() == 'length: 0'
     assert Argument(name="length", value=-1).render() == 'length: -1'
 
 
+def test_value_is_bool():
+    assert Argument(name="some", value=True).render() == 'some: true'
+    assert Argument(name="some", value=False).render() == 'some: false'
+
+
 def test_value_is_list_str():
     assert Argument(name="someListArgument", value=['"123"']).render() == 'someListArgument: ["123"]'
     assert Argument(name="someListArgument", value=[]).render() == 'someListArgument: []'
     assert Argument(name="someListArgument", value=['"123", "456"']).render() == 'someListArgument: ["123", "456"]'
 
 
 def test_value_is_list_int():
     assert Argument(name="someListArgument", value=[123]).render() == 'someListArgument: [123]'
     assert Argument(name="someListArgument", value=[]).render() == 'someListArgument: []'
     assert Argument(name="someListArgument", value=[123, 456]).render() == 'someListArgument: [123, 456]'
 
 
+def test_value_is_list_bool():
+    assert Argument(name="someListArgument", value=[True, False]).render() == 'someListArgument: [true, false]'
+    assert Argument(name="someListArgument", value=[True]).render() == 'someListArgument: [true]'
+    assert Argument(name="someListArgument", value=[False]).render() == 'someListArgument: [false]'
+
+
 @pytest.mark.parametrize(
     "name, value, result",
     [
         ("filter", Argument(name="field", value=123), "filter: {\n  field: 123\n}"),
         ("filter", Argument(name="field", value="VALUE"), "filter: {\n  field: VALUE\n}"),
         ("filter", Argument(name="field", value='"value"'), 'filter: {\n  field: "value"\n}'),
         ("filter", Argument(name="field", value=[123, -456]), "filter: {\n  field: [123, -456]\n}"),
```

### Comparing `graphql_query-1.1.1/tests/test_variable/test_variable.py` & `graphql_query-1.2.0/tests/test_variable/test_variable.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/.gitignore` & `graphql_query-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/LICENSE` & `graphql_query-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/README.md` & `graphql_query-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.1/pyproject.toml` & `graphql_query-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Environment :: Console",
     "Environment :: MacOS X",
     "Framework :: Pydantic",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.7"
 dependencies = [
-    "pydantic>=1.10, <1.11",
+    "pydantic>=2",
     "jinja2>=3.1, <3.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/denisart/graphql-query"
 Documentation = "https://denisart.github.io/graphql-query/"
```

### Comparing `graphql_query-1.1.1/PKG-INFO` & `graphql_query-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphql_query
-Version: 1.1.1
+Version: 1.2.0
 Summary: Complete GraphQL query string generation for python.
 Project-URL: Homepage, https://github.com/denisart/graphql-query
 Project-URL: Documentation, https://denisart.github.io/graphql-query/
 Project-URL: Source, https://github.com/denisart/graphql-query
 Author-email: "Denis A. Artyushin" <artyushinden@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: jinja2<3.2,>=3.1
-Requires-Dist: pydantic<1.11,>=1.10
+Requires-Dist: pydantic>=2
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint-pydantic; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: wheel; extra == 'dev'
 Provides-Extra: docs
```

