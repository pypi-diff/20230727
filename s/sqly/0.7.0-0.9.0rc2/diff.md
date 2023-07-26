# Comparing `tmp/sqly-0.7.0.tar.gz` & `tmp/sqly-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqly-0.7.0.tar", last modified: Fri Nov 12 02:55:13 2021, max compression
+gzip compressed data, was "sqly-0.9.0rc2.tar", last modified: Wed Jul 26 23:01:33 2023, max compression
```

## Comparing `sqly-0.7.0.tar` & `sqly-0.9.0rc2.tar`

### file list

```diff
@@ -1,31 +1,28 @@
-drwxr-xr-x   0 sah       (1000) sah       (1000)        0 2021-11-12 02:55:13.296662 sqly-0.7.0/
--rwxr--r--   0 sah       (1000) sah       (1000)    16725 2021-11-05 01:01:43.000000 sqly-0.7.0/LICENSE
--rwxr--r--   0 sah       (1000) sah       (1000)       83 2021-11-06 19:06:59.000000 sqly-0.7.0/MANIFEST.in
--rw-r--r--   0 sah       (1000) sah       (1000)     2542 2021-11-12 02:55:13.298474 sqly-0.7.0/PKG-INFO
--rwxr--r--   0 sah       (1000) sah       (1000)     2015 2021-11-06 17:44:35.000000 sqly-0.7.0/README.md
--rwxr--r--   0 sah       (1000) sah       (1000)       46 2021-11-05 01:01:43.000000 sqly-0.7.0/pyproject.toml
-drwxr-xr-x   0 sah       (1000) sah       (1000)        0 2021-11-12 02:55:12.665979 sqly-0.7.0/req/
--rwxr--r--   0 sah       (1000) sah       (1000)       72 2021-11-06 18:43:36.000000 sqly-0.7.0/req/dev.txt
--rwxr--r--   0 sah       (1000) sah       (1000)       57 2021-11-12 01:58:49.000000 sqly-0.7.0/req/install.txt
--rwxr--r--   0 sah       (1000) sah       (1000)      448 2021-11-12 02:55:13.308351 sqly-0.7.0/setup.cfg
--rwxr--r--   0 sah       (1000) sah       (1000)      654 2021-11-12 02:54:34.000000 sqly-0.7.0/setup.json
--rwxr--r--   0 sah       (1000) sah       (1000)      992 2021-11-05 01:01:43.000000 sqly-0.7.0/setup.py
-drwxr-xr-x   0 sah       (1000) sah       (1000)        0 2021-11-12 02:55:12.999688 sqly-0.7.0/sqly/
--rw-r--r--   0 sah       (1000) sah       (1000)      144 2021-11-09 02:58:04.000000 sqly-0.7.0/sqly/__init__.py
--rw-r--r--   0 sah       (1000) sah       (1000)     2409 2021-11-10 01:35:31.000000 sqly-0.7.0/sqly/__main__.py
--rw-r--r--   0 sah       (1000) sah       (1000)     1239 2021-11-09 03:31:31.000000 sqly-0.7.0/sqly/database.py
--rw-r--r--   0 sah       (1000) sah       (1000)     4452 2021-11-09 02:58:04.000000 sqly-0.7.0/sqly/dialect.py
--rw-r--r--   0 sah       (1000) sah       (1000)     1056 2021-11-09 02:58:04.000000 sqly-0.7.0/sqly/lib.py
--rw-r--r--   0 sah       (1000) sah       (1000)    10836 2021-11-09 05:21:47.000000 sqly-0.7.0/sqly/migration.py
-drwxr-xr-x   0 sah       (1000) sah       (1000)        0 2021-11-12 02:55:13.256147 sqly-0.7.0/sqly/migrations/
--rw-r--r--   0 sah       (1000) sah       (1000)      731 2021-11-09 03:55:56.000000 sqly-0.7.0/sqly/migrations/20211105034808482_init.yaml
--rw-r--r--   0 sah       (1000) sah       (1000)     1304 2021-11-12 02:30:14.000000 sqly-0.7.0/sqly/query.py
--rw-r--r--   0 sah       (1000) sah       (1000)      115 2021-11-09 02:58:04.000000 sqly-0.7.0/sqly/settings.py
--rwxr--r--   0 sah       (1000) sah       (1000)     2614 2021-11-12 02:53:44.000000 sqly-0.7.0/sqly/sql.py
-drwxr-xr-x   0 sah       (1000) sah       (1000)        0 2021-11-12 02:55:13.211375 sqly-0.7.0/sqly.egg-info/
--rw-r--r--   0 sah       (1000) sah       (1000)     2542 2021-11-12 02:55:11.000000 sqly-0.7.0/sqly.egg-info/PKG-INFO
--rw-r--r--   0 sah       (1000) sah       (1000)      456 2021-11-12 02:55:12.000000 sqly-0.7.0/sqly.egg-info/SOURCES.txt
--rw-r--r--   0 sah       (1000) sah       (1000)        1 2021-11-12 02:55:11.000000 sqly-0.7.0/sqly.egg-info/dependency_links.txt
--rw-r--r--   0 sah       (1000) sah       (1000)       45 2021-11-12 02:55:12.000000 sqly-0.7.0/sqly.egg-info/entry_points.txt
--rw-r--r--   0 sah       (1000) sah       (1000)       72 2021-11-12 02:55:12.000000 sqly-0.7.0/sqly.egg-info/requires.txt
--rw-r--r--   0 sah       (1000) sah       (1000)        5 2021-11-12 02:55:12.000000 sqly-0.7.0/sqly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-26 23:01:32.000000 sqly-0.9.0rc2/setup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/sqly/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/sqly/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/migrations/20211105034808482_init.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/sqly/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/sqly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 23:01:33.000000 sqly-0.9.0rc2/sqly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:33.747182 sqly-0.9.0rc2/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 23:01:31.000000 sqly-0.9.0rc2/testapp/__init__.py
```

### Comparing `sqly-0.7.0/LICENSE` & `sqly-0.9.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqly-0.7.0/PKG-INFO` & `sqly-0.9.0rc2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: sqly
-Version: 0.7.0
+Version: 0.9.0rc2
 Summary: Write SQL in SQL
-Home-page: https://github.com/BlackEarth/sqly
+Home-page: https://github.com/kruxia/sqly
 Author: Sean Harrison
-Author-email: sah@blackearth.us
+Author-email: sah@kruxia.com
 License: MPL 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: migration
+Provides-Extra: psycopg
 Provides-Extra: test
 License-File: LICENSE
 
-# sqly
+# SQLY: write SQL in SQL
 
 SQL is a fantastic language — one of the most successful programming languages in the world. We should use it, not try to replace it with a bespoke DSL. 
 
 Yet there are a couple of things that are nice to have help with in constructing SQL queries:
 
 * **dialect-aware safe value substitution**: Every database interface has its own syntax for substituting values safely (not to allow SQL injection) — for example, `$1` or `?` or `:varname`. They also have different requirements for the format of the sql + values argument lists. I want to able to write my queries with the same value substituion syntax, regardless of which database interface I am using, and know that the SQL will be output correctly for my interface, and that the values will be passed to the database engine safely. 
 * **dynamic attributes**: In many applications, I don't know in advance which attributes I am going to select, insert, update, or filter by. I want to SELECT a given list of attributes, or filter WHERE a given key/value mapping, or UPDATE or INSERT particular attributes, without having to rewrite the SQL query.
 * **block composition**: Some SQL queries are very complex. I want to able to compose blocks of SQL into larger queries, so that I can manage this complexity effectively. (Most database query DSLs are unable to deal with complex queries, or they invent a hard-to-learn language for writing those queries. Learning SQL is a better use of our time, but it would be very helpful having some assistance managing/manipulating the different blocks in a query.)
 
-sqly:
+SQLY:
 
-* One class, `SQL`, with one field, `query`, and one method, `.render`, which takes one optional argument, `dialect`. 
 * Dynamic value replacement, rendered in one of the supported dialects: postgres (`$1`), sqlalchemy (`:varname`), embedded (`:varname`), mysql (`%(varname)s`), sqlite (`?`). Default style is embedded / `:varname`.
-* Dynamic attribute/value lists in `SELECT`,  `WHERE`, `INSERT`, and `UPDATE` syntax
-* Block composition
-
-
+* Dynamic attribute/value lists in `SELECT`,  `WHERE`, `INSERT`, and `UPDATE` syntax.
+* Block composition.
+* [DB-API 2.0](https://peps.python.org/pep-0249/) compatibility.
```

### Comparing `sqly-0.7.0/README.md` & `sqly-0.9.0rc2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# sqly
+# SQLY: write SQL in SQL
 
 SQL is a fantastic language — one of the most successful programming languages in the world. We should use it, not try to replace it with a bespoke DSL. 
 
 Yet there are a couple of things that are nice to have help with in constructing SQL queries:
 
 * **dialect-aware safe value substitution**: Every database interface has its own syntax for substituting values safely (not to allow SQL injection) — for example, `$1` or `?` or `:varname`. They also have different requirements for the format of the sql + values argument lists. I want to able to write my queries with the same value substituion syntax, regardless of which database interface I am using, and know that the SQL will be output correctly for my interface, and that the values will be passed to the database engine safely. 
 * **dynamic attributes**: In many applications, I don't know in advance which attributes I am going to select, insert, update, or filter by. I want to SELECT a given list of attributes, or filter WHERE a given key/value mapping, or UPDATE or INSERT particular attributes, without having to rewrite the SQL query.
 * **block composition**: Some SQL queries are very complex. I want to able to compose blocks of SQL into larger queries, so that I can manage this complexity effectively. (Most database query DSLs are unable to deal with complex queries, or they invent a hard-to-learn language for writing those queries. Learning SQL is a better use of our time, but it would be very helpful having some assistance managing/manipulating the different blocks in a query.)
 
-sqly:
+SQLY:
 
-* One class, `SQL`, with one field, `query`, and one method, `.render`, which takes one optional argument, `dialect`. 
 * Dynamic value replacement, rendered in one of the supported dialects: postgres (`$1`), sqlalchemy (`:varname`), embedded (`:varname`), mysql (`%(varname)s`), sqlite (`?`). Default style is embedded / `:varname`.
-* Dynamic attribute/value lists in `SELECT`,  `WHERE`, `INSERT`, and `UPDATE` syntax
-* Block composition
-
+* Dynamic attribute/value lists in `SELECT`,  `WHERE`, `INSERT`, and `UPDATE` syntax.
+* Block composition.
+* [DB-API 2.0](https://peps.python.org/pep-0249/) compatibility.
```

### Comparing `sqly-0.7.0/sqly/__main__.py` & `sqly-0.9.0rc2/sqly/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,85 +1,100 @@
+"""
+The `sqly.__main__` module provides the `sqly` command line command. This is the code
+reference documentation; see the [CLI Usage](../cli.md) document for usage information.
+"""
+# import json
 import os
 import sys
 
 import click
 import networkx as nx
 
-from .database import Database
+from .dialect import Dialect
 from .migration import Migration
 
 
 @click.group()
-def main():
+def sqly():  # pragma: no cover
     pass
 
 
-@main.command()
+@sqly.command()
 @click.option(
-    '--name', required=False, help="A couple words describing the Migration's purpose"
+    "-n",
+    "--name",
+    required=False,
+    help="A couple words describing the Migration's purpose",
 )
-@click.argument('app')
-@click.argument('other_apps', nargs=-1)
+@click.argument("app")
+@click.argument("other_apps", nargs=-1)
 def migration(app, other_apps, name):
     """
     Create a Migration in APP (importable python module) incorporating dependencies from
     OTHER_APPS
     """
     migration = Migration.create(app, *other_apps, name=name)
-    migration.save()
+    migration.save(exclude={"applied"})
     print(f"Created migration: {migration.key}")
-    print("    depends:\n      -", '\n      - '.join(migration.depends or '[]'))
+    print("    depends:\n      -", "\n      - ".join(migration.depends or "[]"))
 
 
-@main.command()
-@click.argument('apps', nargs=-1)
-@click.option('-i', '--include-depends', is_flag=True, help='Show dependencies')
+@sqly.command()
+@click.argument("apps", nargs=-1)
+@click.option("-i", "--include-depends", is_flag=True, help="Include dependencies")
 def migrations(apps, include_depends=False):
     """
     List the Migrations in APPS
     """
     for app in apps:
-        app_migrations = {
-            m.key: m
-            for m in Migration.app_migrations(app, include_depends=include_depends)
-        }
+        app_migrations = Migration.app_migrations(app, include_depends=include_depends)
         graph = Migration.graph(Migration.app_migrations(app, include_depends=True))
         for key in nx.lexicographical_topological_sort(graph):
             if key in app_migrations:
                 print(key)
                 migration = app_migrations[key]
                 if migration.depends and include_depends:
-                    print('\t=> ' + ', '.join(migration.depends))
+                    print("\t=> " + "\n\t=> ".join(migration.depends))
 
 
-@main.command()
-@click.argument('migration_key')
+@sqly.command()
+@click.argument("migration_key")
 @click.option(
-    '-d',
-    '--database-url',
+    "-u",
+    "--database-url",
     required=False,
     help="Datebase to migrate; default = env $DATABASE_URL",
 )
+@click.option("-d", "--dialect", required=False)
 @click.option(
-    '-r',
-    '--dryrun',
+    "-r",
+    "--dryrun",
     is_flag=True,
     help="If present, shows but does not run the migrations",
 )
-def migrate(migration_key, database_url=None, dryrun=False):
+def migrate(migration_key, database_url=None, dialect=None, dryrun=False):
     """
     Migrate database_url to the given MIGRATION_KEY (up or dn).
     """
-    database_url = database_url or os.getenv('DATABASE_URL')
+    database_url = database_url or os.getenv("DATABASE_URL")
+    dialect = dialect or os.getenv("DATABASE_DIALECT")
     if not database_url:
-        print('--database-url or env $DATABASE_URL must be set', file=sys.stderr)
+        print("--database-url or env $DATABASE_URL must be set", file=sys.stderr)
+        sys.exit(1)
+    if not dialect:
+        print("--dialect or env $DATABASE_DIALECT must be set", file=sys.stderr)
         sys.exit(1)
 
-    dialect = Database.connection_string_dialect(database_url)
-    database = Database(connection_string=database_url, dialect=dialect)
+    dialect = Dialect(dialect)
+    adaptor = dialect.adaptor()
+    # if dialect == Dialect.MYSQL:
+    #     conn_info = json.loads(database_url)
+    #     connection = adaptor.connect(**conn_info)
+    # else:
+    connection = adaptor.connect(database_url)
 
     migration = Migration.key_load(migration_key)
-    Migration.migrate(database, migration, dryrun=dryrun)
+    Migration.migrate(connection, dialect, migration, dryrun=dryrun)
 
 
-if __name__ == '__main__':
-    main()
+if __name__ == "__main__":  # pragma: no cover
+    sqly()
```

### Comparing `sqly-0.7.0/sqly.egg-info/PKG-INFO` & `sqly-0.9.0rc2/sqly.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: sqly
-Version: 0.7.0
+Version: 0.9.0rc2
 Summary: Write SQL in SQL
-Home-page: https://github.com/BlackEarth/sqly
+Home-page: https://github.com/kruxia/sqly
 Author: Sean Harrison
-Author-email: sah@blackearth.us
+Author-email: sah@kruxia.com
 License: MPL 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: migration
+Provides-Extra: psycopg
 Provides-Extra: test
 License-File: LICENSE
 
-# sqly
+# SQLY: write SQL in SQL
 
 SQL is a fantastic language — one of the most successful programming languages in the world. We should use it, not try to replace it with a bespoke DSL. 
 
 Yet there are a couple of things that are nice to have help with in constructing SQL queries:
 
 * **dialect-aware safe value substitution**: Every database interface has its own syntax for substituting values safely (not to allow SQL injection) — for example, `$1` or `?` or `:varname`. They also have different requirements for the format of the sql + values argument lists. I want to able to write my queries with the same value substituion syntax, regardless of which database interface I am using, and know that the SQL will be output correctly for my interface, and that the values will be passed to the database engine safely. 
 * **dynamic attributes**: In many applications, I don't know in advance which attributes I am going to select, insert, update, or filter by. I want to SELECT a given list of attributes, or filter WHERE a given key/value mapping, or UPDATE or INSERT particular attributes, without having to rewrite the SQL query.
 * **block composition**: Some SQL queries are very complex. I want to able to compose blocks of SQL into larger queries, so that I can manage this complexity effectively. (Most database query DSLs are unable to deal with complex queries, or they invent a hard-to-learn language for writing those queries. Learning SQL is a better use of our time, but it would be very helpful having some assistance managing/manipulating the different blocks in a query.)
 
-sqly:
+SQLY:
 
-* One class, `SQL`, with one field, `query`, and one method, `.render`, which takes one optional argument, `dialect`. 
 * Dynamic value replacement, rendered in one of the supported dialects: postgres (`$1`), sqlalchemy (`:varname`), embedded (`:varname`), mysql (`%(varname)s`), sqlite (`?`). Default style is embedded / `:varname`.
-* Dynamic attribute/value lists in `SELECT`,  `WHERE`, `INSERT`, and `UPDATE` syntax
-* Block composition
-
-
+* Dynamic attribute/value lists in `SELECT`,  `WHERE`, `INSERT`, and `UPDATE` syntax.
+* Block composition.
+* [DB-API 2.0](https://peps.python.org/pep-0249/) compatibility.
```

