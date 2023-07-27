# Comparing `tmp/metapensiero.sphinx.patchdb-4.0.dev7.tar.gz` & `tmp/metapensiero.sphinx.patchdb-4.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapensiero.sphinx.patchdb-4.0.dev7.tar", last modified: Fri Jul 21 09:21:57 2023, max compression
+gzip compressed data, was "metapensiero.sphinx.patchdb-4.0.dev8.tar", last modified: Thu Jul 27 16:34:16 2023, max compression
```

## Comparing `metapensiero.sphinx.patchdb-4.0.dev7.tar` & `metapensiero.sphinx.patchdb-4.0.dev8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     3894 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/CHANGES.rst
--rw-r--r--   0        0        0      589 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/Makefile
--rw-r--r--   0        0        0    10656 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/OLDERCHANGES.rst
--rw-r--r--   0        0        0    30372 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/README.rst
--rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/flake.lock
--rw-r--r--   0        0        0     3760 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/flake.nix
--rw-r--r--   0        0        0     1745 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/pyproject.toml
--rw-r--r--   0        0        0      697 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/__init__.py
--rw-r--r--   0        0        0     7496 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/__init__.py
--rw-r--r--   0        0        0     3545 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/firebird.py
--rw-r--r--   0        0        0     4692 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/mysql.py
--rw-r--r--   0        0        0     4289 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/postgres.py
--rw-r--r--   0        0        0     1505 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/python.py
--rw-r--r--   0        0        0    17886 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/sql.py
--rw-r--r--   0        0        0     3858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/sqlite.py
--rw-r--r--   0        0        0     1546 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/locale/__init__.py
--rw-r--r--   0        0        0    13004 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po
--rw-r--r--   0        0        0      285 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/locale/mapping.cfg
--rw-r--r--   0        0        0     8858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot
--rw-r--r--   0        0        0     4730 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/manager.py
--rw-r--r--   0        0        0    14938 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/patch.py
--rw-r--r--   0        0        0     6155 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/planner.py
--rw-r--r--   0        0        0     9175 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/pup.py
--rw-r--r--   0        0        0    24368 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/script.py
--rw-r--r--   0        0        0     7312 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/states.py
--rw-r--r--   0        0        0     8148 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/fixtures.py
--rwxr-xr-x   0        0        0     1633 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/postgresql
--rw-r--r--   0        0        0     7111 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_bad.py
--rw-r--r--   0        0        0     4424 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_drops.py
--rw-r--r--   0        0        0     1182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_external_file.py
--rw-r--r--   0        0        0     3557 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_helpers.py
--rw-r--r--   0        0        0     1862 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_manager.py
--rw-r--r--   0        0        0     2284 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_modular.py
--rw-r--r--   0        0        0     3531 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_patch.py
--rw-r--r--   0        0        0     6685 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_planner.py
--rw-r--r--   0        0        0     2766 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_python.py
--rw-r--r--   0        0        0     7007 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_revisions.py
--rw-r--r--   0        0        0     4632 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_sql.py
--rw-r--r--   0        0        0     2291 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_sql_fb.py
--rw-r--r--   0        0        0     4328 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_sql_ms.py
--rw-r--r--   0        0        0     7639 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_sql_pg.py
--rw-r--r--   0        0        0     2835 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_states.py
--rw-r--r--   0        0        0     2094 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/tests/test_variables.py
--rw-r--r--   0        0        0    31467 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0     4109 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/CHANGES.rst
+-rw-r--r--   0        0        0      589 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/Makefile
+-rw-r--r--   0        0        0    10656 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/OLDERCHANGES.rst
+-rw-r--r--   0        0        0    31089 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/README.rst
+-rw-r--r--   0        0        0     2006 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/flake.lock
+-rw-r--r--   0        0        0     3760 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/flake.nix
+-rw-r--r--   0        0        0     1745 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0      697 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/__init__.py
+-rw-r--r--   0        0        0     7496 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/__init__.py
+-rw-r--r--   0        0        0     3545 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/firebird.py
+-rw-r--r--   0        0        0     4692 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/mysql.py
+-rw-r--r--   0        0        0     4289 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/postgres.py
+-rw-r--r--   0        0        0     1505 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/python.py
+-rw-r--r--   0        0        0    17964 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/sql.py
+-rw-r--r--   0        0        0     3858 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/sqlite.py
+-rw-r--r--   0        0        0     1546 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/__init__.py
+-rw-r--r--   0        0        0    13092 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po
+-rw-r--r--   0        0        0      285 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/mapping.cfg
+-rw-r--r--   0        0        0     8935 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot
+-rw-r--r--   0        0        0     4673 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/manager.py
+-rw-r--r--   0        0        0    14064 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/patch.py
+-rw-r--r--   0        0        0     9282 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/planner.py
+-rw-r--r--   0        0        0     9175 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/pup.py
+-rw-r--r--   0        0        0    24367 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/script.py
+-rw-r--r--   0        0        0     7312 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/states.py
+-rw-r--r--   0        0        0     8148 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/fixtures.py
+-rwxr-xr-x   0        0        0     1633 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/postgresql
+-rw-r--r--   0        0        0     7111 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_bad.py
+-rw-r--r--   0        0        0     4430 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_drops.py
+-rw-r--r--   0        0        0     1182 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_external_file.py
+-rw-r--r--   0        0        0     3557 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_helpers.py
+-rw-r--r--   0        0        0     1862 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_manager.py
+-rw-r--r--   0        0        0     2284 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_modular.py
+-rw-r--r--   0        0        0     3555 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_patch.py
+-rw-r--r--   0        0        0     8226 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_planner.py
+-rw-r--r--   0        0        0     2766 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_python.py
+-rw-r--r--   0        0        0     7007 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_revisions.py
+-rw-r--r--   0        0        0     4632 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql.py
+-rw-r--r--   0        0        0     2291 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_fb.py
+-rw-r--r--   0        0        0     4328 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_ms.py
+-rw-r--r--   0        0        0     7639 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_pg.py
+-rw-r--r--   0        0        0     2835 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_states.py
+-rw-r--r--   0        0        0     2094 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/tests/test_variables.py
+-rw-r--r--   0        0        0    32184 1980-01-01 00:00:00.000000 metapensiero.sphinx.patchdb-4.0.dev8/PKG-INFO
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/CHANGES.rst` & `metapensiero.sphinx.patchdb-4.0.dev8/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changes\ [#]_
 -------------
 
+4.0.dev8 (2023-07-27)
+~~~~~~~~~~~~~~~~~~~~~
+
+* Various fixes to the new ``Planner`` machinery
+
+* Add a new `replaces` option on the patches, as a better alternative to the kludge introduced
+  in version 4.0.dev3.
+
+
 4.0.dev7 (2023-07-21)
 ~~~~~~~~~~~~~~~~~~~~~
 
 * Fix nix packaging of sqlparse 0.4.4
 
 
 4.0.dev6 (2023-07-21)
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/Makefile` & `metapensiero.sphinx.patchdb-4.0.dev8/Makefile`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/OLDERCHANGES.rst` & `metapensiero.sphinx.patchdb-4.0.dev8/OLDERCHANGES.rst`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/README.rst` & `metapensiero.sphinx.patchdb-4.0.dev8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,27 @@
      :depends: Some function@1
      :brings: Some function@2
 
      DROP FUNCTION some_function(int, OUT int)
      ;;
      ;;INCLUDE: some_function.sql
 
+A particular case is when you actually need to *replace* something with something else, for example instead of upgrading the function above you want to replace it entirely. This is when the ``replaces`` option comes handy: it is almost equivalent to the ``depends`` option, except that it is not an error when an item specified with the former does not exist::
+
+  .. patchdb:script:: Some other function
+     :file: some_other_function.sql
+
+  .. patchdb:script:: Replace some function with a different one
+     :replaces: Some function@1
+     :brings: Some other function@1
+
+     DROP FUNCTION IF EXISTS some_function(int, OUT int)
+     ;;
+     ;;INCLUDE: some_other_function.sql
+
 
 Conditions
 ++++++++++
 
 The example shows also an usage of the conditions, allowing more than one variant of a script
 like::
 
@@ -291,16 +304,17 @@
 
 
 Dependencies
 ++++++++++++
 
 .. _master-table:
 
-The dependencies (that is, the *options* ``:brings:``, ``:depends:``, ``:drops:`` and
-``:preceeds:``) may be a paragraph containing a comma separated list of script ids, such as::
+The dependencies (that is, the *options* ``:brings:``, ``:depends:``, ``:drops:``,
+``:preceeds:`` and ``:replaces:``) may be a paragraph containing a comma separated list of
+script ids, such as::
 
   .. patchdb:script:: Create master table
 
      CREATE TABLE some_table (id INTEGER PRIMARY KEY, tt_id INTEGER)
 
   .. patchdb:script:: Create target table
 
@@ -392,17 +406,17 @@
        SUSPEND;
      END
 
 
 Patches
 ~~~~~~~
 
-A `patch` is a particular flavour of script, one that specifies a `brings` or a `drops`
-dependency list. Imagine that the `example above`__ was the first version of the database, and
-that the current version looks like the following::
+A `patch` is a particular flavour of script, one that specifies a `brings`, a `drops` or a
+`replaces` dependency list. Imagine that the `example above`__ was the first version of the
+database, and that the current version looks like the following::
 
   .. patchdb:script:: Create master table
      :revision: 2
 
      CREATE TABLE some_table (
        id INTEGER PRIMARY KEY,
        description VARCHAR(80),
@@ -487,16 +501,16 @@
        person_id INTEGER REFERENCES persons (id),
        street_address VARCHAR(80),
        city VARCHAR(80),
        telephone_number VARCHAR(80)
      )
 
   .. patchdb:script:: Migrate from customers to persons and person_addresses
+     :replaces: Create table customers@2
      :depends:
-        - Create table customers@2
         - Create table persons
         - Create table person_addresses
      :drops:
         - Create table customers
         - Add telephone number to customers table
 
      INSERT INTO persons (id, name) SELECT id, name FROM customers
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/flake.lock` & `metapensiero.sphinx.patchdb-4.0.dev8/flake.lock`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/flake.nix` & `metapensiero.sphinx.patchdb-4.0.dev8/flake.nix`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/pyproject.toml` & `metapensiero.sphinx.patchdb-4.0.dev8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "metapensiero.sphinx.patchdb"
 description = "Extract scripts from a reST document and apply them in order."
-version = "4.0.dev7"
+version = "4.0.dev8"
 authors = [
     { name = "Lele Gaifax", email = "lele@metapensiero.it" },
 ]
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/firebird.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/firebird.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/mysql.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/mysql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/postgres.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/postgres.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/python.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/python.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/sql.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # :Copyright: © 2014, 2016, 2017, 2019, 2021, 2023 Lele Gaifax
 #
 
 from collections import deque, namedtuple
 from datetime import datetime
 from hashlib import md5 as hash_factory
 from io import TextIOBase
+from logging import DEBUG
 
 from sqlparse import tokens, lexer
 
 from sqlparse.tokens import Comment, Keyword, Literal, Name, Punctuation, Whitespace
 from sqlparse import tokens
 from sqlparse.keywords import PROCESS_AS_KEYWORD
 from sqlparse.utils import consume
@@ -243,28 +244,25 @@
             self.commitTransaction()
 
             return State(hash.hexdigest(), last[0], last[1])
         else:
             self.commitTransaction()
 
     def isApplicable(self, patch):
-        """Check for CREATE scripts, that are surely *not* idempotent.
-        Exclude also patches which dependants do not yet exist.
+        """
+        Check for CREATE scripts, that are surely *not* idempotent.
         """
 
         if not patch.is_migration and self[patch.patchid]:
             for stmt in split_script(patch.script):
                 stmt = self.prepareStatement(stmt)
                 # If it's not a fake CREATE DOMAIN
                 if stmt is not None:
                     if statement_starts_with(stmt, ((Keyword.DDL, 'CREATE'),)):
                         return False, "contains a CREATE statement and it's already present"
-        elif patch.is_migration:
-            if all(self[depid] is None for depid, deprev in patch.depends):
-                return False, "all dependants do not exists yet"
         return True, None
 
     def apply(self, patch, options=None, patch_manager=None):
         """
         Try to execute the given `patch` script, which may be
         composed by one or more SQL statements separated by two
         consecutive semicomma ``;;`` on a line by their own::
@@ -289,15 +287,20 @@
             for i, stmt in enumerate(stmts):
                 if stmt:
                     stmt_lines = stmt.count('\n')
                     stmt = self.prepareStatement(self.replaceUserVariables(stmt))
                     if not stmt:
                         continue
 
-                    logger.debug("Executing '%s ...'" % stmt[:50])
+                    if logger.isEnabledFor(DEBUG):
+                        import re
+                        stripped_stmt = re.sub(r'\s+', ' ', stmt)
+                        if len(stripped_stmt) > 65:
+                            stripped_stmt = stripped_stmt[:63] + ' …'
+                        logger.debug("Executing %r ..." % stripped_stmt)
 
                     try:
                         cursor.execute(stmt)
                         current_line += stmt_lines + 1
                         last_good_point = i+1
                         self.savePoint(last_good_point)
                     except Exception as e:
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/contexts/sqlite.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/contexts/sqlite.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/locale/__init__.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/it/LC_MESSAGES/metapensiero-sphinx-patchdb.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # Copyright (C) 2016, 2017, 2019, 2021, 2022, 2023 Lele Gaifax
 # This file is distributed under the same license as the
 # metapensiero.sphinx.patchdb project.
 # Lele Gaifax <lele@metapensiero.it>, 2016.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev7\n"
+"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev8\n"
 "Report-Msgid-Bugs-To: lele@metapensiero.it\n"
-"POT-Creation-Date: 2023-06-04 17:23+0200\n"
-"PO-Revision-Date: 2023-06-04 17:26+0200\n"
+"POT-Creation-Date: 2023-07-27 18:30+0200\n"
+"PO-Revision-Date: 2023-07-27 18:31+0200\n"
 "Last-Translator: Lele Gaifax <lele@metapensiero.it>\n"
 "Language: it\n"
 "Language-Team: it <lele@metapensiero.it>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -24,51 +24,51 @@
 msgid ""
 "\n"
 "Error: %s"
 msgstr ""
 "\n"
 "Errore: %s"
 
-#: src/metapensiero/sphinx/patchdb/script.py:422
-#: src/metapensiero/sphinx/patchdb/script.py:444
+#: src/metapensiero/sphinx/patchdb/script.py:423
+#: src/metapensiero/sphinx/patchdb/script.py:445
 msgid " (any revision)"
 msgstr " (qualsiasi revisione)"
 
-#: src/metapensiero/sphinx/patchdb/script.py:294
-#: src/metapensiero/sphinx/patchdb/script.py:424
-#: src/metapensiero/sphinx/patchdb/script.py:446
+#: src/metapensiero/sphinx/patchdb/script.py:295
+#: src/metapensiero/sphinx/patchdb/script.py:425
+#: src/metapensiero/sphinx/patchdb/script.py:447
 #, python-format
 msgid " (revision %(revno)d)"
 msgstr " (revisione %(revno)d)"
 
-#: src/metapensiero/sphinx/patchdb/script.py:496
+#: src/metapensiero/sphinx/patchdb/script.py:498
 msgid "After any other script"
 msgstr "Dopo tutti gli altri script"
 
 #: src/metapensiero/sphinx/patchdb/pup.py:164
 msgid "Assume missing patches are already applied, do not re-execute them."
 msgstr "Assumi che gli script mancanti siano già stati applicati, non rieseguirli."
 
 #: src/metapensiero/sphinx/patchdb/pup.py:177
 msgid "Be quiet, emit only error messages."
 msgstr "Emetti solo messaggi di errore."
 
-#: src/metapensiero/sphinx/patchdb/script.py:494
+#: src/metapensiero/sphinx/patchdb/script.py:496
 msgid "Before any other script"
 msgstr "Prima di qualsiasi altro script"
 
-#: src/metapensiero/sphinx/patchdb/script.py:464
+#: src/metapensiero/sphinx/patchdb/script.py:466
 msgid "Brings"
 msgstr "Implementa"
 
-#: src/metapensiero/sphinx/patchdb/script.py:486
+#: src/metapensiero/sphinx/patchdb/script.py:488
 msgid "Condition"
 msgstr "Condizione"
 
-#: src/metapensiero/sphinx/patchdb/script.py:478
+#: src/metapensiero/sphinx/patchdb/script.py:480
 msgid "Conditions"
 msgstr "Condizioni"
 
 #: src/metapensiero/sphinx/patchdb/pup.py:132
 msgid "Database script applier"
 msgstr "Database script applier"
 
@@ -78,19 +78,19 @@
 " must be something like “varname=value”. This option may be given "
 "multiple times."
 msgstr ""
 "Definisce una variabile arbitraria usabile come “{{VARNAME}}” in uno "
 "script. VAR deve essere qualche cosa nella forma “nomevariabile=valore”. "
 "Questa opzione può essere specificata più di una volta."
 
-#: src/metapensiero/sphinx/patchdb/script.py:462
+#: src/metapensiero/sphinx/patchdb/script.py:463
 msgid "Depends on"
 msgstr "Dipende da"
 
-#: src/metapensiero/sphinx/patchdb/script.py:468
+#: src/metapensiero/sphinx/patchdb/script.py:470
 msgid "Direct dependants"
 msgstr "Dipendenze dirette"
 
 #: src/metapensiero/sphinx/patchdb/pup.py:175
 msgid "Don't apply patches, just list them."
 msgstr "Non applicare gli script, elencali solamente."
 
@@ -101,15 +101,15 @@
 msgstr[0] "Fatto, applicato %d script"
 msgstr[1] "Fatto, applicati %d script"
 
 #: src/metapensiero/sphinx/patchdb/pup.py:159
 msgid "Driver to access MySQL, defaults to “pymysql”."
 msgstr "Driver per accedere a MySQL, di default “pymysql”."
 
-#: src/metapensiero/sphinx/patchdb/script.py:465
+#: src/metapensiero/sphinx/patchdb/script.py:467
 msgid "Drops"
 msgstr "Elimina"
 
 #: src/metapensiero/sphinx/patchdb/pup.py:179
 msgid "Emit debug messages."
 msgstr "Emetti i messaggi di debug."
 
@@ -123,35 +123,35 @@
 msgstr "Errore: %s"
 
 #: src/metapensiero/sphinx/patchdb/pup.py:61
 #, python-format
 msgid "Error: could not apply %d scripts due to circular dependencies"
 msgstr "Errore: impossibile applicare %d script a causa di dipendenze circolari"
 
-#: src/metapensiero/sphinx/patchdb/script.py:492
+#: src/metapensiero/sphinx/patchdb/script.py:494
 msgid "Execute always"
 msgstr "Applicato ogni volta"
 
-#: src/metapensiero/sphinx/patchdb/script.py:233
+#: src/metapensiero/sphinx/patchdb/script.py:234
 msgid "File insertion disabled"
 msgstr "Inclusione disabilitata"
 
-#: src/metapensiero/sphinx/patchdb/script.py:506
+#: src/metapensiero/sphinx/patchdb/script.py:508
 msgid ""
 "Go on with the next script, skipping any succeding statements of the "
 "failing script"
 msgstr ""
 "Continua con il prossimo script, saltando le istruzioni successive a "
 "quella che ha generato l'errore"
 
 #: src/metapensiero/sphinx/patchdb/pup.py:153
 msgid "Host name where MySQL server runs, defaults to “localhost”."
 msgstr "Nome dell'host del server MySQL, di default “localhost”."
 
-#: src/metapensiero/sphinx/patchdb/script.py:510
+#: src/metapensiero/sphinx/patchdb/script.py:512
 msgid ""
 "Ignore the error and keeps going with the remaining statements in the "
 "script"
 msgstr "Ignora gli errore e prosegui con le istruzioni successive dello script"
 
 #: src/metapensiero/sphinx/patchdb/pup.py:167
 msgid ""
@@ -165,15 +165,15 @@
 "volta."
 
 #: src/metapensiero/sphinx/patchdb/pup.py:109
 #, python-format
 msgid "Invalid variable: %s"
 msgstr "Variabile non valida: %s"
 
-#: src/metapensiero/sphinx/patchdb/script.py:202
+#: src/metapensiero/sphinx/patchdb/script.py:203
 #, python-format
 msgid "Missing mandatory ID for the directive \"%s\"."
 msgstr "La direttiva \"%s\" richiede un ID."
 
 #: src/metapensiero/sphinx/patchdb/pup.py:135
 msgid ""
 "One or more archives containing collected scripts. May be either plain "
@@ -198,51 +198,55 @@
 " cosa, che di norma (oppure quando viene specificato “None”) non viene "
 "effettuato."
 
 #: src/metapensiero/sphinx/patchdb/pup.py:155
 msgid "Port number used by the MySQL server, defaults to “3306”."
 msgstr "Porta usata dal server MySQL, di default “3306”. "
 
-#: src/metapensiero/sphinx/patchdb/script.py:463
+#: src/metapensiero/sphinx/patchdb/script.py:465
 msgid "Preceeds"
 msgstr "Precede"
 
-#: src/metapensiero/sphinx/patchdb/script.py:653
+#: src/metapensiero/sphinx/patchdb/script.py:651
 #, python-format
 msgid "Reference to an unknown script: %(scriptid)r"
 msgstr "Riferimento a uno script sconosciuto: %(scriptid)r"
 
-#: src/metapensiero/sphinx/patchdb/script.py:219
+#: src/metapensiero/sphinx/patchdb/script.py:464
+msgid "Replaces"
+msgstr "Sostituisce"
+
+#: src/metapensiero/sphinx/patchdb/script.py:220
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: ID "
 "contains \"@\", not allowed"
 msgstr ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" alla riga %(lineno)d: ID "
 "contiene carattere non permesso \"@\""
 
-#: src/metapensiero/sphinx/patchdb/script.py:251
+#: src/metapensiero/sphinx/patchdb/script.py:252
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: ID is not "
 "unique, there is another one in \"%(other)s\"!"
 msgstr ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" alla riga %(lineno)d: ID non "
 "univoco, duplicato in \"%(other)s\"!"
 
-#: src/metapensiero/sphinx/patchdb/script.py:212
+#: src/metapensiero/sphinx/patchdb/script.py:213
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: ID is too "
 "long, maximum allowed length is %(maxlen)d characters!"
 msgstr ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" alla riga %(lineno)d: ID "
 "troppo lungo, massimo %(maxlen)d caratteri!"
 
-#: src/metapensiero/sphinx/patchdb/script.py:270
+#: src/metapensiero/sphinx/patchdb/script.py:271
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: bad option"
 " (%(error)s)"
 msgstr ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" alla riga %(lineno)d: opzione "
 "errata (%(error)s)"
@@ -252,15 +256,15 @@
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: circular "
 "include of file %(filename)r"
 msgstr ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" alla riga %(lineno)d: "
 "inclusione circolare del file %(filename)r"
 
-#: src/metapensiero/sphinx/patchdb/script.py:225
+#: src/metapensiero/sphinx/patchdb/script.py:226
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: content "
 "and :file: option are mutually exclusive"
 msgstr ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" alla riga %(lineno)d: "
 "impossibile specificare contemporaneamente contenuto e opzione :file:"
@@ -281,23 +285,23 @@
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: include "
 "file %(filename)r not found or unreadable"
 msgstr ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" alla riga %(lineno)d: "
 "impossibile includere %(filename)r, non esiste oppure non leggibile"
 
-#: src/metapensiero/sphinx/patchdb/script.py:289
+#: src/metapensiero/sphinx/patchdb/script.py:290
 msgid "Script ID: "
 msgstr "ID: "
 
-#: src/metapensiero/sphinx/patchdb/script.py:354
+#: src/metapensiero/sphinx/patchdb/script.py:355
 msgid "Script index"
 msgstr "Indice degli script"
 
-#: src/metapensiero/sphinx/patchdb/script.py:366
+#: src/metapensiero/sphinx/patchdb/script.py:367
 msgid "Scripts"
 msgstr "Script"
 
 #: src/metapensiero/sphinx/patchdb/pup.py:143
 msgid "Select the Firebird context."
 msgstr "Seleziona il contesto Firebird."
 
@@ -317,44 +321,44 @@
 msgid "Select the SQLite context."
 msgstr "Seleziona il contesto SQLite."
 
 #: src/metapensiero/sphinx/patchdb/pup.py:162
 msgid "Specify where to write the execution log."
 msgstr "Specifica dove scrivere il log dell'esecuzione."
 
-#: src/metapensiero/sphinx/patchdb/script.py:577
+#: src/metapensiero/sphinx/patchdb/script.py:575
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) brings an "
 "unknown script \"%(other)s\""
 msgstr ""
 "La %(scriptid)s (definita in %(docname)s alla riga %(lineno)s) implementa"
 " uno script sconosciuto \"%(other)s\""
 
-#: src/metapensiero/sphinx/patchdb/script.py:585
+#: src/metapensiero/sphinx/patchdb/script.py:583
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) brings "
 "script \"%(other)s\" to revision %(newrev)s, but it's still at revision "
 "%(currev)s"
 msgstr ""
 "La %(scriptid)s (definita in %(docname)s alla riga %(lineno)s) implementa"
 " lo script \"%(other)s\" alla revisione %(newrev)s, ma è ancora alla "
 "revisione %(currev)s"
 
-#: src/metapensiero/sphinx/patchdb/script.py:569
+#: src/metapensiero/sphinx/patchdb/script.py:567
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) depends on "
 "an unknown script \"%(other)s\""
 msgstr ""
 "Lo %(scriptid)s (definito in %(docname)s alla riga %(lineno)s) dipende da"
 " uno script sconosciuto \"%(other)s\""
 
-#: src/metapensiero/sphinx/patchdb/script.py:471
+#: src/metapensiero/sphinx/patchdb/script.py:473
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) references "
 "an unknown script \"%(other)s\""
 msgstr ""
 "Lo %(scriptid)s (definito in %(docname)s alla riga %(lineno)s) referenzia"
 " uno script sconosciuto \"%(other)s\""
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/locale/metapensiero-sphinx-patchdb.pot`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # This file is distributed under the same license as the
 # metapensiero.sphinx.patchdb project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev7\n"
+"Project-Id-Version: metapensiero.sphinx.patchdb 4.0.dev8\n"
 "Report-Msgid-Bugs-To: lele@metapensiero.it\n"
-"POT-Creation-Date: 2023-06-04 17:23+0200\n"
+"POT-Creation-Date: 2023-07-27 18:30+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
@@ -21,70 +21,70 @@
 #: src/metapensiero/sphinx/patchdb/pup.py:54
 #, python-format
 msgid ""
 "\n"
 "Error: %s"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:422
-#: src/metapensiero/sphinx/patchdb/script.py:444
+#: src/metapensiero/sphinx/patchdb/script.py:423
+#: src/metapensiero/sphinx/patchdb/script.py:445
 msgid " (any revision)"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:294
-#: src/metapensiero/sphinx/patchdb/script.py:424
-#: src/metapensiero/sphinx/patchdb/script.py:446
+#: src/metapensiero/sphinx/patchdb/script.py:295
+#: src/metapensiero/sphinx/patchdb/script.py:425
+#: src/metapensiero/sphinx/patchdb/script.py:447
 #, python-format
 msgid " (revision %(revno)d)"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:496
+#: src/metapensiero/sphinx/patchdb/script.py:498
 msgid "After any other script"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:164
 msgid "Assume missing patches are already applied, do not re-execute them."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:177
 msgid "Be quiet, emit only error messages."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:494
+#: src/metapensiero/sphinx/patchdb/script.py:496
 msgid "Before any other script"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:464
+#: src/metapensiero/sphinx/patchdb/script.py:466
 msgid "Brings"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:486
+#: src/metapensiero/sphinx/patchdb/script.py:488
 msgid "Condition"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:478
+#: src/metapensiero/sphinx/patchdb/script.py:480
 msgid "Conditions"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:132
 msgid "Database script applier"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:171
 msgid ""
 "Define an arbitrary variable usable as “{{VARNAME}}” within a script. VAR"
 " must be something like “varname=value”. This option may be given "
 "multiple times."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:462
+#: src/metapensiero/sphinx/patchdb/script.py:463
 msgid "Depends on"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:468
+#: src/metapensiero/sphinx/patchdb/script.py:470
 msgid "Direct dependants"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:175
 msgid "Don't apply patches, just list them."
 msgstr ""
 
@@ -95,15 +95,15 @@
 msgstr[0] ""
 msgstr[1] ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:159
 msgid "Driver to access MySQL, defaults to “pymysql”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:465
+#: src/metapensiero/sphinx/patchdb/script.py:467
 msgid "Drops"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:179
 msgid "Emit debug messages."
 msgstr ""
 
@@ -117,33 +117,33 @@
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:61
 #, python-format
 msgid "Error: could not apply %d scripts due to circular dependencies"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:492
+#: src/metapensiero/sphinx/patchdb/script.py:494
 msgid "Execute always"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:233
+#: src/metapensiero/sphinx/patchdb/script.py:234
 msgid "File insertion disabled"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:506
+#: src/metapensiero/sphinx/patchdb/script.py:508
 msgid ""
 "Go on with the next script, skipping any succeding statements of the "
 "failing script"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:153
 msgid "Host name where MySQL server runs, defaults to “localhost”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:510
+#: src/metapensiero/sphinx/patchdb/script.py:512
 msgid ""
 "Ignore the error and keeps going with the remaining statements in the "
 "script"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:167
 msgid ""
@@ -153,15 +153,15 @@
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:109
 #, python-format
 msgid "Invalid variable: %s"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:202
+#: src/metapensiero/sphinx/patchdb/script.py:203
 #, python-format
 msgid "Missing mandatory ID for the directive \"%s\"."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:135
 msgid ""
 "One or more archives containing collected scripts. May be either plain "
@@ -178,59 +178,63 @@
 "that by default (or by specifying “None”) does not happen."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:155
 msgid "Port number used by the MySQL server, defaults to “3306”."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:463
+#: src/metapensiero/sphinx/patchdb/script.py:465
 msgid "Preceeds"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:653
+#: src/metapensiero/sphinx/patchdb/script.py:651
 #, python-format
 msgid "Reference to an unknown script: %(scriptid)r"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:219
+#: src/metapensiero/sphinx/patchdb/script.py:464
+msgid "Replaces"
+msgstr ""
+
+#: src/metapensiero/sphinx/patchdb/script.py:220
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: ID "
 "contains \"@\", not allowed"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:251
+#: src/metapensiero/sphinx/patchdb/script.py:252
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: ID is not "
 "unique, there is another one in \"%(other)s\"!"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:212
+#: src/metapensiero/sphinx/patchdb/script.py:213
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: ID is too "
 "long, maximum allowed length is %(maxlen)d characters!"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:270
+#: src/metapensiero/sphinx/patchdb/script.py:271
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: bad option"
 " (%(error)s)"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:113
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: circular "
 "include of file %(filename)r"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:225
+#: src/metapensiero/sphinx/patchdb/script.py:226
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: content "
 "and :file: option are mutually exclusive"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/script.py:93
@@ -244,23 +248,23 @@
 #: src/metapensiero/sphinx/patchdb/script.py:87
 #, python-format
 msgid ""
 "Script \"%(scriptid)s\" in \"%(docname)s\" at line %(lineno)d: include "
 "file %(filename)r not found or unreadable"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:289
+#: src/metapensiero/sphinx/patchdb/script.py:290
 msgid "Script ID: "
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:354
+#: src/metapensiero/sphinx/patchdb/script.py:355
 msgid "Script index"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:366
+#: src/metapensiero/sphinx/patchdb/script.py:367
 msgid "Scripts"
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:143
 msgid "Select the Firebird context."
 msgstr ""
 
@@ -278,37 +282,37 @@
 msgid "Select the SQLite context."
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:162
 msgid "Specify where to write the execution log."
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:577
+#: src/metapensiero/sphinx/patchdb/script.py:575
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) brings an "
 "unknown script \"%(other)s\""
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:585
+#: src/metapensiero/sphinx/patchdb/script.py:583
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) brings "
 "script \"%(other)s\" to revision %(newrev)s, but it's still at revision "
 "%(currev)s"
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:569
+#: src/metapensiero/sphinx/patchdb/script.py:567
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) depends on "
 "an unknown script \"%(other)s\""
 msgstr ""
 
-#: src/metapensiero/sphinx/patchdb/script.py:471
+#: src/metapensiero/sphinx/patchdb/script.py:473
 #, python-format
 msgid ""
 "The %(scriptid)s (defined in %(docname)s at line %(lineno)s) references "
 "an unknown script \"%(other)s\""
 msgstr ""
 
 #: src/metapensiero/sphinx/patchdb/pup.py:40
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/manager.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #
 
 import json
 import logging
 from os.path import dirname, exists, relpath
 import pickle
 
-from .patch import DependencyError, sort_by_constraints
-
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)
 
 
 class DuplicatedScriptError(Exception):
     "Indicates that a script is not unique."
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/patch.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/patch.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,57 +2,57 @@
 # :Project:   PatchDB -- Patch object
 # :Created:   Fri Oct  3 01:13:20 2003
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
 # :Copyright: © 2003, 2009, 2010, 2012-2017, 2019, 2021, 2023 Lele Gaifax
 #
 
-from collections import defaultdict
-from graphlib import TopologicalSorter
 import logging
 
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)
 
 MAX_PATCHID_LEN = 100
 
 
 class DependencyError(Exception):
     "Indicate some problem with the dependencies."
 
 
-def compute_checksum(language, script, depends, preceeds, brings, drops, conditions,
+def compute_checksum(language, script, depends, replaces, preceeds, brings, drops, conditions,
                      onerror, revision, mimetype):
     """Compute a checksum from the script and its metadata.
 
     This is mainly needed to avoid repeated beautification of the same script.
     """
 
     from hashlib import md5
 
     return md5(b'#'.join((language.encode('ascii', 'ignore'),
                           script.encode('ascii', 'ignore'),
                           repr(depends).encode('ascii', 'ignore'),
+                          repr(replaces).encode('ascii', 'ignore'),
                           repr(preceeds).encode('ascii', 'ignore'),
                           repr(brings).encode('ascii', 'ignore'),
                           repr(drops).encode('ascii', 'ignore'),
                           repr(conditions).encode('ascii', 'ignore'),
+                          repr(onerror).encode('ascii', 'ignore'),
                           repr(revision).encode('ascii', 'ignore'),
                           repr(mimetype).encode('ascii', 'ignore')))).digest()
 
 
 class Patch:
     """
     Represent a single `patch`, that is some kind of arbitrary script
     written in some language, curried with some metadata.
     """
 
     def __init__(self, patchid, description, script, language, revision,
-                 depends, preceeds, brings, drops, conditions, onerror='abort',
+                 depends, replaces, preceeds, brings, drops, conditions, onerror='abort',
                  mimetype=None, always=False, autocommit=False,
                  source=None, line=None):
         self.patchid = patchid
         """The unique ID of this patch"""
 
         self.description = description
         """The description of the script"""
@@ -65,14 +65,17 @@
 
         self.revision = revision
         """The revision of the script"""
 
         self.depends = depends
         "List of tuples (ID,rev) of the patches this one depends on"
 
+        self.replaces = replaces
+        "List of tuples (ID,rev) of the patches this one replaces"
+
         self.preceeds = preceeds
         "List of tuples (ID,rev) of the patches that depend on this one"
 
         self.brings = brings
         "List of tuples (ID,rev) of the patches this one updates"
 
         self.drops = drops
@@ -93,16 +96,16 @@
 
         self.always = always
         "Whether the patch shall be executed always at each run, rather than only once."
 
         self.autocommit = autocommit
         "Whether the patch shall be executed in autocommit mode."
 
-        self.checksum = compute_checksum(language, script, depends, preceeds, brings, drops,
-                                         conditions, onerror, revision, mimetype)
+        self.checksum = compute_checksum(language, script, depends, replaces, preceeds, brings,
+                                         drops, conditions, onerror, revision, mimetype)
         "Checksum of the script, to track changes"
 
         self.source = source
         "The source file that defined this script."
 
         self.line = line
         "The line number where the script is defined."
@@ -150,14 +153,16 @@
             else:
                 return d[0]
 
         if self.always:
             res['always'] = self.always
         if self.depends:
             res['depends'] = [rr(d) for d in self.depends]
+        if self.replaces:
+            res['replaces'] = [rr(d) for d in self.replaces]
         if self.preceeds:
             res['preceeds'] = [rr(p) for p in self.preceeds]
         if self.brings:
             res['brings'] = [rr(b) for b in self.brings]
         if self.drops:
             res['drops'] = [rr(d) for d in self.drops]
         if self.conditions:
@@ -167,75 +172,71 @@
         if self.autocommit:
             res['autocommit'] = self.autocommit
 
         return res
 
     @property
     def is_migration(self):
-        return bool(self.brings or self.drops)
+        return bool(self.replaces or self.brings or self.drops)
 
     @property
     def is_placeholder(self):
         return not self.script
 
     def adjustUnspecifiedRevisions(self, pm, context):
         """
         Replace the non-specified revision numbers with the current known version of the patch.
 
+        :returns: a `(bool, str)` tuple,, ``True`` when the patch must be retained, ``False``
+                  to discard it and the reason
+
         Perform also some sanity checks: all `depends`, `brings` and `preceeds` must exist at
         this point.
         """
 
+        retain_reason = ''
         for i, (pid, rev) in enumerate(self.depends):
             p = pm[pid]
             if p is None:
+                reason = (f'defined in {self.source} at line {self.line}'
+                          f' depends on non existing "{pid}@{rev}"')
                 if self.is_migration:
-                    logger.debug('%s (defined in %s at line %s)'
-                                 ' depends on "%s@%s",'
-                                 ' which does not exist: applying anyway',
-                                 self, self.source, self.line, pid, rev)
-                    continue
-                raise DependencyError('%s (defined in %s at line %s)'
-                                      ' depends on "%s@%s",'
-                                      ' which does not exist.'
-                                      % (self, self.source, self.line, pid, rev))
+                    return False, reason
+                raise DependencyError(f'{self} {reason}')
             if rev is None:
                 self.depends[i] = (pid, p.revision)
             elif rev == '*':
                 current_rev = context[pid]
                 if current_rev is None:
                     self.depends[i] = (pid, p.revision)
                 else:
                     self.depends[i] = (pid, current_rev)
 
         for i, (pid, rev) in enumerate(self.brings):
             p = pm[pid]
             if p is None:
-                logger.debug('%s (defined in %s at line %s)'
-                             ' brings to "%s@%s",'
-                             ' which does not exist: applying anyway'
-                             % (self, self.source, self.line, pid, rev))
-                continue
+                reason = (f'defined in {self.source} at line {self.line},'
+                          f' brings to non existing "{pid}@{rev}"')
+                return False, reason
             if rev is None:
                 self.brings[i] = (pid, p.revision)
 
         for i, (pid, rev) in enumerate(self.preceeds):
             p = pm[pid]
             if p is None:
+                reason = (f'defined in {self.source} at line {self.line}'
+                          f' preceeds on non existing "{pid}@{rev}"')
                 if self.is_migration:
-                    logger.debug('%s (defined in %s at line %s) preceeds "%s@%s",'
-                                 ' which does not exist: applying anyway'
-                                 % (self, self.source, self.line, pid, rev))
-                else:
-                    raise DependencyError('%s (defined in %s at line %s) preceeds "%s@%s",'
-                                          ' which does not exist.'
-                                          % (self, self.source, self.line, pid, rev))
+                    return False, reason
+                raise DependencyError(f'{self} {reason}')
             if rev is None:
                 self.preceeds[i] = (pid, pm[pid].revision)
 
+        return True, retain_reason
+
     def beautify(self):
         "Compute a beautified and highlighted HTML version of the script."
 
         from pygments import highlight
         from pygments.lexers import get_lexer_by_name, get_lexer_for_mimetype
         from pygments.formatters import get_formatter_by_name
 
@@ -346,14 +347,19 @@
 
     try:
         depends = parse_deps(options.get('depends', ''), allow_star=True)
     except ValueError as e:
         raise ValueError("Error in script's depends option: %s" % str(e))
 
     try:
+        replaces = parse_deps(options.get('replaces', ''))
+    except ValueError as e:
+        raise ValueError("Error in script's replaces option: %s" % str(e))
+
+    try:
         preceeds = parse_deps(options.get('preceeds', ''))
     except ValueError as e:
         raise ValueError("Error in script's preceeds option: %s" % str(e))
 
     try:
         brings = parse_deps(options.get('brings', ''))
     except ValueError as e:
@@ -387,33 +393,9 @@
     if mimetype is None:
         if language == 'python':
             mimetype = 'application/x-python'
         elif language == 'sql':
             mimetype = 'text/x-sql'
 
     return Patch(patchid, description, script, language, revision,
-                 depends, preceeds, brings, drops, conditions, onerror, mimetype,
+                 depends, replaces, preceeds, brings, drops, conditions, onerror, mimetype,
                  always, autocommit, options.get('source'), options.get('line'))
-
-
-def sort_by_constraints(patches, manager):
-    "Reorder given `patches` taking into account their dependencies."
-
-    constraints = defaultdict(set)
-    for patch in patches:
-        if patch.is_placeholder:
-            # This is a "placeholder" patch and it has not been applied yet
-            logger.critical("%s has not been applied yet", patch)
-            raise DependencyError('%s has not been applied yet' % patch)
-        for otherid, otherrev in patch.depends:
-            other = manager[otherid]
-            if other in patches:
-                constraints[patch].add(other)
-        for otherid, otherrev in patch.preceeds:
-            other = manager[otherid]
-            if other in patches:
-                constraints[other].add(patch)
-
-    if constraints:
-        patches = tuple(TopologicalSorter(constraints).static_order())
-
-    return patches
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/pup.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/pup.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/script.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,15 @@
             'text/x-python',
             'text/x-python3',
             'text/x-sql',
             'text/x-sqlite3-console',
         )),
         'onerror': directives.unchanged_required,
         'preceeds': directives.unchanged_required,
+        'replaces': directives.unchanged_required,
         'revision': directives.nonnegative_int,
         }
 
     def run(self):
         """Implement ``script`` directive.
 
         The ``script`` directive introduces a piece of code, taken from its
@@ -251,15 +252,15 @@
                 _('Script "%(scriptid)s" in "%(docname)s" at line %(lineno)d:'
                   ' ID is not unique, there is another one in "%(other)s"!')
                 % dict(scriptid=scriptid, docname=env.docname, lineno=lineno,
                        other=scripts[scriptid]['docname']))
 
         self.already_seen_this_session.add(scriptid)
 
-        for option in ('brings', 'depends', 'drops', 'preceeds', 'conditions'):
+        for option in ('brings', 'depends', 'drops', 'conditions', 'preceeds', 'replaces'):
             if option in options:
                 elt = nodes.Element()
                 vl = ViewList(options[option].splitlines())
                 self.state.nested_parse(vl, self.content_offset, elt)
                 if isinstance(elt.children[0], nodes.bullet_list):
                     options[option] = [c.astext() for c in elt.children[0]]
 
@@ -456,14 +457,15 @@
         patch = scripts[node['scriptid']]['patch']
 
         dlist = nodes.definition_list()
 
         is_a_patch = bool(patch.brings) or bool(patch.drops)
         try:
             add_detail(dlist, _('Depends on'), patch.depends, strike_missing=is_a_patch)
+            add_detail(dlist, _('Replaces'), patch.replaces, strike_missing=is_a_patch)
             add_detail(dlist, _('Preceeds'), patch.preceeds, strike_missing=is_a_patch)
             add_detail(dlist, _('Brings'), patch.brings, strike_missing=is_a_patch)
             add_detail(dlist, _('Drops'), patch.drops, strike_missing=is_a_patch)
             rdeps = revdeps.get(patch.patchid, None)
             if rdeps:
                 add_detail(dlist, _('Direct dependants'), sorted(rdeps))
         except DependencyError as e:
@@ -555,20 +557,16 @@
     if not scripts or not app.config.patchdb_storage:
         return
 
     # Better safe than sorry: check dependencies and report anomalies
     for sid in scripts:
         patch = scripts[sid]['patch']
         if patch.depends:
-            if patch.drops:
-                dropped = {p[0] for p in patch.drops}
-            else:
-                dropped = ()
             for pid, rev in patch.depends:
-                if pid not in scripts and not pid in dropped:
+                if pid not in scripts:
                     logger.warning(
                         _('The %(scriptid)s (defined in %(docname)s at line %(lineno)s)'
                           ' depends on an unknown script "%(other)s"')
                         % dict(scriptid=patch, docname=patch.source, lineno=patch.line,
                                other=pid))
         if patch.brings:
             for pid, rev in patch.brings:
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/src/metapensiero/sphinx/patchdb/states.py` & `metapensiero.sphinx.patchdb-4.0.dev8/src/metapensiero/sphinx/patchdb/states.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/fixtures.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/postgresql` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/postgresql`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_bad.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_bad.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_drops.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_drops.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,16 @@
      street_address VARCHAR(80),
      city VARCHAR(80),
      telephone_number VARCHAR(80)
    )
    ;;
 
 .. patchdb:script:: Migrate from customers to persons and person_addresses
+   :replaces: Create table customers@2
    :depends:
-      - Create table customers@2
       - Create table persons
       - Create table person_addresses
    :drops:
       - Create table customers
       - Add telephone number to customers table
 
    INSERT INTO persons (id, name) SELECT id, name FROM customers
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_external_file.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_external_file.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_helpers.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_manager.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_modular.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_modular.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_patch.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
     third = pm['third']
     assert third.preceeds == [('fourth', 2)]
     third.adjustUnspecifiedRevisions(pm, context)
 
     try:
         fourth.adjustUnspecifiedRevisions(pm, context)
     except DependencyError as e:
-        assert 'script "fourth@1"' in str(e) and 'depends on "unknown@1"' in str(e)
+        assert 'script "fourth@1"' in str(e)
+        assert 'depends on non existing "unknown@1"' in str(e)
     else:
         assert False, "should raise a DependencyError"
 
     fifth = make_patch('fifth', 'script',
                        dict(depends="second@*"))
     pm['fifth'] = fifth
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_planner.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_planner.py`

 * *Files 14% similar despite different names*

```diff
@@ -104,20 +104,20 @@
 
 
 def test_planner_3():
     ctx = DummyExecutionContext({})
     pm = PatchManager()
 
     persons = make_patch('persons', 'script',
-                       dict(language='test'))
+                         dict(language='test'))
     pm['persons'] = persons
 
     addresses = make_patch('addresses', 'script',
-                        dict(language='test',
-                             depends='persons'))
+                           dict(language='test',
+                                depends='persons'))
     pm['addresses'] = addresses
 
     migration = make_patch('migration', 'script',
                            dict(language='test',
                                 depends=('customers@2', 'persons', 'addresses'),
                                 drops=('customers', 'add phone numbers to customers')))
     pm['migration'] = migration
@@ -132,20 +132,20 @@
 def test_planner_4():
     # V1
 
     ctx = DummyExecutionContext({})
     pm = PatchManager()
 
     parents = make_patch('parents', 'script',
-                       dict(language='test'))
+                         dict(language='test'))
     pm['parents'] = parents
 
     children = make_patch('children', 'script',
-                        dict(language='test',
-                             depends='parents'))
+                          dict(language='test',
+                               depends='parents'))
     pm['children'] = children
 
     data = make_patch('data', 'script',
                       dict(language='test',
                            depends=('parents', 'children')))
     pm['data'] = data
 
@@ -196,7 +196,66 @@
     pm['counter'] = counter
 
     planner = ExecutionPlanner(pm, ctx)
     assert tuple(planner) == (
         counter,
         migration,
     )
+
+
+def test_already_met_deps():
+    ctx = DummyExecutionContext({'dep1': 1, 'dep2': 2})
+    pm = PatchManager()
+
+    dep1 = make_patch('dep1', 'script',
+                      dict(language='test'))
+    pm['dep1'] = dep1
+
+    a = make_patch('a', 'script',
+                   dict(language='test',
+                        depends=('dep1@1', 'dep2@3')))
+    pm['a'] = a
+
+    b = make_patch('b', 'script',
+                   dict(language='test',
+                        depends=('dep1@1', 'dep2@2')))
+    pm['b'] = b
+
+    newdep2 = make_patch('dep2', 'script',
+                         dict(language='test',
+                              revision=3,
+                              depends='dep1'))
+    pm['dep2'] = newdep2
+
+    planner = ExecutionPlanner(pm, ctx)
+    assert tuple(planner) == (
+        b,
+        newdep2,
+        a,
+    )
+
+    always_first = make_patch('always_first', 'script',
+                              dict(language='test',
+                                   always='first'))
+    pm['always_first'] = always_first
+
+    planner = ExecutionPlanner(pm, ctx)
+    assert tuple(planner) == (
+        always_first,
+        b,
+        newdep2,
+        a,
+    )
+
+    always_last = make_patch('always_last', 'script',
+                              dict(language='test',
+                                   always='last'))
+    pm['always_last'] = always_last
+
+    planner = ExecutionPlanner(pm, ctx)
+    assert tuple(planner) == (
+        always_first,
+        b,
+        newdep2,
+        a,
+        always_last,
+    )
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_python.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_revisions.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_revisions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # :Project:   PatchDB -- Test for multiple revisions of script
 # :Created:   mer 24 feb 2016 17:30:26 CET
 # :Author:    Lele Gaifax <lele@metapensiero.it>
 # :License:   GNU General Public License version 3 or later
-# :Copyright: © 2016, 2017 Lele Gaifax
+# :Copyright: © 2016, 2017, 2023 Lele Gaifax
 #
 
 import fixtures
 
 
 FIRST_REV = """
 Multiple revisions
@@ -203,17 +203,16 @@
    create table new_table (
      id integer primary key
    )
    ;;
    insert into new_table (id) values (0)
 
 .. patchdb:script:: Rename old_table to new_table
-   :depends: Create old table@1
-   :brings:
-     - Create new table@1
+   :replaces: Create old table@1
+   :brings: Create new table@1
 
    alter table old_table rename to new_table
    ;;
    insert into new_table (id) values (3)
 """
```

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_sql.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_sql_fb.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_fb.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_sql_ms.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_ms.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_sql_pg.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_sql_pg.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_states.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_states.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/tests/test_variables.py` & `metapensiero.sphinx.patchdb-4.0.dev8/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `metapensiero.sphinx.patchdb-4.0.dev7/PKG-INFO` & `metapensiero.sphinx.patchdb-4.0.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metapensiero.sphinx.patchdb
-Version: 4.0.dev7
+Version: 4.0.dev8
 Summary: Extract scripts from a reST document and apply them in order.
 License: GPL-3.0-or-later
 Author-email: Lele Gaifax <lele@metapensiero.it>
 Requires-Python: >=3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Sphinx :: Extension
@@ -208,14 +208,27 @@
      :depends: Some function@1
      :brings: Some function@2
 
      DROP FUNCTION some_function(int, OUT int)
      ;;
      ;;INCLUDE: some_function.sql
 
+A particular case is when you actually need to *replace* something with something else, for example instead of upgrading the function above you want to replace it entirely. This is when the ``replaces`` option comes handy: it is almost equivalent to the ``depends`` option, except that it is not an error when an item specified with the former does not exist::
+
+  .. patchdb:script:: Some other function
+     :file: some_other_function.sql
+
+  .. patchdb:script:: Replace some function with a different one
+     :replaces: Some function@1
+     :brings: Some other function@1
+
+     DROP FUNCTION IF EXISTS some_function(int, OUT int)
+     ;;
+     ;;INCLUDE: some_other_function.sql
+
 
 Conditions
 ++++++++++
 
 The example shows also an usage of the conditions, allowing more than one variant of a script
 like::
 
@@ -316,16 +329,17 @@
 
 
 Dependencies
 ++++++++++++
 
 .. _master-table:
 
-The dependencies (that is, the *options* ``:brings:``, ``:depends:``, ``:drops:`` and
-``:preceeds:``) may be a paragraph containing a comma separated list of script ids, such as::
+The dependencies (that is, the *options* ``:brings:``, ``:depends:``, ``:drops:``,
+``:preceeds:`` and ``:replaces:``) may be a paragraph containing a comma separated list of
+script ids, such as::
 
   .. patchdb:script:: Create master table
 
      CREATE TABLE some_table (id INTEGER PRIMARY KEY, tt_id INTEGER)
 
   .. patchdb:script:: Create target table
 
@@ -417,17 +431,17 @@
        SUSPEND;
      END
 
 
 Patches
 ~~~~~~~
 
-A `patch` is a particular flavour of script, one that specifies a `brings` or a `drops`
-dependency list. Imagine that the `example above`__ was the first version of the database, and
-that the current version looks like the following::
+A `patch` is a particular flavour of script, one that specifies a `brings`, a `drops` or a
+`replaces` dependency list. Imagine that the `example above`__ was the first version of the
+database, and that the current version looks like the following::
 
   .. patchdb:script:: Create master table
      :revision: 2
 
      CREATE TABLE some_table (
        id INTEGER PRIMARY KEY,
        description VARCHAR(80),
@@ -512,16 +526,16 @@
        person_id INTEGER REFERENCES persons (id),
        street_address VARCHAR(80),
        city VARCHAR(80),
        telephone_number VARCHAR(80)
      )
 
   .. patchdb:script:: Migrate from customers to persons and person_addresses
+     :replaces: Create table customers@2
      :depends:
-        - Create table customers@2
         - Create table persons
         - Create table person_addresses
      :drops:
         - Create table customers
         - Add telephone number to customers table
 
      INSERT INTO persons (id, name) SELECT id, name FROM customers
```

