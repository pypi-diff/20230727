# Comparing `tmp/kestrel-lang-1.7.2.tar.gz` & `tmp/kestrel-lang-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel-lang-1.7.2.tar", last modified: Wed Jul 26 16:15:02 2023, max compression
+gzip compressed data, was "kestrel-lang-1.7.3.tar", last modified: Thu Jul 27 01:47:34 2023, max compression
```

## Comparing `kestrel-lang-1.7.2.tar` & `kestrel-lang-1.7.3.tar`

### file list

```diff
@@ -1,110 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.524427 kestrel-lang-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-07-26 16:15:02.524427 kestrel-lang-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/bin/kestrel
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-26 16:15:02.524427 kestrel-lang-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.508427 kestrel-lang-1.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/src/kestrel/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/src/kestrel/absinterface/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/absinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/absinterface/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/src/kestrel/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/analytics/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/analytics/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/src/kestrel/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/prefetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/codegen/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.512427 kestrel-lang-1.7.2/src/kestrel/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/datasource/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/datasource/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/datasource/retstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/semantics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/semantics/completor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/semantics/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/semantics/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel/symboltable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/symboltable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/symboltable/symtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/symboltable/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/ecgpattern.lark
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/ecgpattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/kestrel.lark
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/syntax/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel_analytics_docker/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_docker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel_analytics_python/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_analytics_python/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel_datasource_stixbundle/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixbundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixbundle/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.516427 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.520427 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/transmitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.520427 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-07-26 16:15:02.000000 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-26 16:15:02.000000 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:15:02.000000 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-26 16:15:02.000000 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 16:15:02.000000 kestrel-lang-1.7.2/src/kestrel_lang.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:15:02.524427 kestrel-lang-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_find.py
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_command_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_python_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_records.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_stixshifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_stixshifter_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-26 16:14:44.000000 kestrel-lang-1.7.2/tests/test_timestamped.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.922964 kestrel-lang-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-07-27 01:47:34.922964 kestrel-lang-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/bin/kestrel
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/bin/stix-shifter-diag
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-27 01:47:34.926964 kestrel-lang-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.910963 kestrel-lang-1.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/absinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/absinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/absinterface/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/analytics/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/analytics/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/prefetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/codegen/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/datasource/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/datasource/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/datasource/retstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/semantics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/semantics/completor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/semantics/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/semantics/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.914963 kestrel-lang-1.7.3/src/kestrel/symboltable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/symboltable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/symboltable/symtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/symboltable/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/ecgpattern.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/ecgpattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/kestrel.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/syntax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_analytics_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_docker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_analytics_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_analytics_python/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_datasource_stixbundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixbundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixbundle/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-27 01:47:14.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/transmitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.918964 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-07-27 01:47:34.000000 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-27 01:47:34.000000 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 01:47:34.000000 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 01:47:34.000000 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 01:47:34.000000 kestrel-lang-1.7.3/src/kestrel_lang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:47:34.922964 kestrel-lang-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_command_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_python_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_stixshifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_stixshifter_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_stixshifter_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-27 01:47:15.000000 kestrel-lang-1.7.3/tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.7.2/AUTHORS.rst` & `kestrel-lang-1.7.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/LICENSE.md` & `kestrel-lang-1.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/PKG-INFO` & `kestrel-lang-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.7.2
+Version: 1.7.3
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
```

### Comparing `kestrel-lang-1.7.2/README.rst` & `kestrel-lang-1.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/setup.cfg` & `kestrel-lang-1.7.3/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kestrel-lang
-version = 1.7.2
+version = 1.7.3
 description = Kestrel Threat Hunting Language
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 keywords = 
 	domain specific language
 	cyber threat hunting
 	extended detection and response
@@ -20,15 +20,17 @@
 project_urls = 
 	Documentation = https://kestrel.readthedocs.io/
 
 [options]
 packages = find:
 package_dir = 
 	=src
-scripts = bin/kestrel
+scripts = 
+	bin/kestrel
+	bin/stix-shifter-diag
 python_requires = >= 3.8
 install_requires = 
 	typeguard>=4.0.0
 	pyyaml>=6.0
 	lxml>=4.9.3
 	lark>=1.1.5
 	pandas>=2.0.0
```

### Comparing `kestrel-lang-1.7.2/src/kestrel/__main__.py` & `kestrel-lang-1.7.3/src/kestrel/__main__.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/absinterface/manager.py` & `kestrel-lang-1.7.3/src/kestrel/absinterface/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/analytics/interface.py` & `kestrel-lang-1.7.3/src/kestrel/analytics/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/analytics/manager.py` & `kestrel-lang-1.7.3/src/kestrel/analytics/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/codegen/commands.py` & `kestrel-lang-1.7.3/src/kestrel/codegen/commands.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/codegen/data.py` & `kestrel-lang-1.7.3/src/kestrel/codegen/data.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/codegen/display.py` & `kestrel-lang-1.7.3/src/kestrel/codegen/display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/codegen/prefetch.py` & `kestrel-lang-1.7.3/src/kestrel/codegen/prefetch.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/codegen/queries.py` & `kestrel-lang-1.7.3/src/kestrel/codegen/queries.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/codegen/relations.py` & `kestrel-lang-1.7.3/src/kestrel/codegen/relations.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/codegen/summary.py` & `kestrel-lang-1.7.3/src/kestrel/codegen/summary.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/config.py` & `kestrel-lang-1.7.3/src/kestrel/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/config.yaml` & `kestrel-lang-1.7.3/src/kestrel/config.yaml`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/datasource/interface.py` & `kestrel-lang-1.7.3/src/kestrel/datasource/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/datasource/manager.py` & `kestrel-lang-1.7.3/src/kestrel/datasource/manager.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/datasource/retstruct.py` & `kestrel-lang-1.7.3/src/kestrel/datasource/retstruct.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/exceptions.py` & `kestrel-lang-1.7.3/src/kestrel/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             "please check data source configuration",
         )
 
 
 class DataSourceError(KestrelException):
     def __init__(self, error, suggestion=""):
         if not suggestion:
-            suggestion = "please check data source config or test the query manually"
+            suggestion = "please check data source config or diagnose with stix-shifter-diag command"
         super().__init__(
             error,
             suggestion,
         )
 
 
 class DataSourceInterfaceNotFound(KestrelException):
```

### Comparing `kestrel-lang-1.7.2/src/kestrel/semantics/completor.py` & `kestrel-lang-1.7.3/src/kestrel/semantics/completor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/semantics/processor.py` & `kestrel-lang-1.7.3/src/kestrel/semantics/processor.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/semantics/reference.py` & `kestrel-lang-1.7.3/src/kestrel/semantics/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/session.py` & `kestrel-lang-1.7.3/src/kestrel/session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/symboltable/variable.py` & `kestrel-lang-1.7.3/src/kestrel/symboltable/variable.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/syntax/ecgpattern.py` & `kestrel-lang-1.7.3/src/kestrel/syntax/ecgpattern.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/syntax/kestrel.lark` & `kestrel-lang-1.7.3/src/kestrel/syntax/kestrel.lark`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/syntax/parser.py` & `kestrel-lang-1.7.3/src/kestrel/syntax/parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/syntax/reference.py` & `kestrel-lang-1.7.3/src/kestrel/syntax/reference.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/syntax/utils.py` & `kestrel-lang-1.7.3/src/kestrel/syntax/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel/utils.py` & `kestrel-lang-1.7.3/src/kestrel/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,24 @@
         return s[1:-1].encode("utf-8").decode("unicode_escape")
 
 
 def lowered_str_list(xs):
     return [x.lower() for x in xs if isinstance(x, str)]
 
 
+def mask_value_in_nested_dict(d):
+    if d:
+        for k, v in d.items():
+            if isinstance(v, collections.abc.Mapping):
+                d[k] = mask_value_in_nested_dict(v)
+            elif isinstance(v, str):
+                d[k] = "********"
+    return d
+
+
 def update_nested_dict(dict_old, dict_new):
     if dict_new:
         for k, v in dict_new.items():
             if isinstance(v, collections.abc.Mapping) and k in dict_old:
                 dict_old[k] = update_nested_dict(dict_old[k], v)
             else:
                 dict_old[k] = v
```

### Comparing `kestrel-lang-1.7.2/src/kestrel_analytics_docker/config.py` & `kestrel-lang-1.7.3/src/kestrel_analytics_docker/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_analytics_docker/interface.py` & `kestrel-lang-1.7.3/src/kestrel_analytics_docker/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_analytics_python/config.py` & `kestrel-lang-1.7.3/src/kestrel_analytics_python/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_analytics_python/interface.py` & `kestrel-lang-1.7.3/src/kestrel_analytics_python/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_datasource_stixbundle/interface.py` & `kestrel-lang-1.7.3/src/kestrel_datasource_stixbundle/interface.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/config.py` & `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/config.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/connector.py` & `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/connector.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/interface.py` & `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,14 +88,20 @@
 
         $ export STIXSHIFTER_HOST101_CONNECTOR=elastic_ecs
         $ export STIXSHIFTER_HOST101_CONNECTION='{"host":"elastic.securitylog.company.com", "port":9200, "indices":"host101"}'
         $ export STIXSHIFTER_HOST101_CONFIG='{"auth":{"id":"VuaCfGcBCdbkQm-e5aOx", "api_key":"ui2lp2axTNmsyakw9tvNnw"}}'
 
 #. any in-session edit through the ``CONFIG`` command.
 
+Once you added data source profiles into ``stixshifter.yaml``, you can test the data source with command:
+
+.. code-block:: console
+
+    $ stix-shifter-diag data_source_name
+
 If you launch Kestrel in debug mode, STIX-shifter debug mode is still not
 enabled by default. To record debug level logs of STIX-shifter, create
 environment variable ``KESTREL_STIXSHIFTER_DEBUG`` with any value.
 
 .. _STIX-shifter: https://github.com/opencybersecurityalliance/stix-shifter
 .. _elastic_ecs config: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/stix_shifter_modules/elastic_ecs/configuration/lang_en.json
 .. _stix_shifter_modules/lang_en.json: https://github.com/opencybersecurityalliance/stix-shifter/blob/develop/stix_shifter_modules/lang_en.json
```

### Comparing `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/multiproc.py` & `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/multiproc.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/query.py` & `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/query.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/translator.py` & `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/translator.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/transmitter.py` & `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/transmitter.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_datasource_stixshifter/worker/utils.py` & `kestrel-lang-1.7.3/src/kestrel_datasource_stixshifter/worker/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/src/kestrel_lang.egg-info/PKG-INFO` & `kestrel-lang-1.7.3/src/kestrel_lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kestrel-lang
-Version: 1.7.2
+Version: 1.7.3
 Summary: Kestrel Threat Hunting Language
 Home-page: https://github.com/opencybersecurityalliance/kestrel-lang
 License: Apache 2.0 License
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Keywords: domain specific language,cyber threat hunting,extended detection and response
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
```

### Comparing `kestrel-lang-1.7.2/src/kestrel_lang.egg-info/SOURCES.txt` & `kestrel-lang-1.7.3/src/kestrel_lang.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 AUTHORS.rst
 LICENSE.md
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 bin/kestrel
+bin/stix-shifter-diag
 src/kestrel/__init__.py
 src/kestrel/__main__.py
 src/kestrel/config.py
 src/kestrel/config.yaml
 src/kestrel/exceptions.py
 src/kestrel/session.py
 src/kestrel/utils.py
@@ -50,14 +51,15 @@
 src/kestrel_analytics_python/config.py
 src/kestrel_analytics_python/interface.py
 src/kestrel_datasource_stixbundle/__init__.py
 src/kestrel_datasource_stixbundle/interface.py
 src/kestrel_datasource_stixshifter/__init__.py
 src/kestrel_datasource_stixshifter/config.py
 src/kestrel_datasource_stixshifter/connector.py
+src/kestrel_datasource_stixshifter/diagnosis.py
 src/kestrel_datasource_stixshifter/interface.py
 src/kestrel_datasource_stixshifter/multiproc.py
 src/kestrel_datasource_stixshifter/query.py
 src/kestrel_datasource_stixshifter/worker/__init__.py
 src/kestrel_datasource_stixshifter/worker/translator.py
 src/kestrel_datasource_stixshifter/worker/transmitter.py
 src/kestrel_datasource_stixshifter/worker/utils.py
@@ -83,9 +85,10 @@
 tests/test_exceptions.py
 tests/test_expressions.py
 tests/test_parser.py
 tests/test_python_analytics.py
 tests/test_records.py
 tests/test_session.py
 tests/test_stixshifter.py
+tests/test_stixshifter_diagnosis.py
 tests/test_stixshifter_translator.py
 tests/test_timestamped.py
```

### Comparing `kestrel-lang-1.7.2/tests/test_command_assign.py` & `kestrel-lang-1.7.3/tests/test_command_assign.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_command_disp.py` & `kestrel-lang-1.7.3/tests/test_command_disp.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_command_find.py` & `kestrel-lang-1.7.3/tests/test_command_find.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_command_get.py` & `kestrel-lang-1.7.3/tests/test_command_get.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_command_group.py` & `kestrel-lang-1.7.3/tests/test_command_group.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_command_internal.py` & `kestrel-lang-1.7.3/tests/test_command_internal.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_command_join.py` & `kestrel-lang-1.7.3/tests/test_command_join.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_command_load.py` & `kestrel-lang-1.7.3/tests/test_command_load.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_command_merge.py` & `kestrel-lang-1.7.3/tests/test_command_merge.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_command_new.py` & `kestrel-lang-1.7.3/tests/test_command_new.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_command_save.py` & `kestrel-lang-1.7.3/tests/test_command_save.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_completion.py` & `kestrel-lang-1.7.3/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_display.py` & `kestrel-lang-1.7.3/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_exceptions.py` & `kestrel-lang-1.7.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_expressions.py` & `kestrel-lang-1.7.3/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_parser.py` & `kestrel-lang-1.7.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_python_analytics.py` & `kestrel-lang-1.7.3/tests/test_python_analytics.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_records.py` & `kestrel-lang-1.7.3/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_session.py` & `kestrel-lang-1.7.3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_stixshifter.py` & `kestrel-lang-1.7.3/tests/test_stixshifter.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_stixshifter_translator.py` & `kestrel-lang-1.7.3/tests/test_stixshifter_translator.py`

 * *Files identical despite different names*

### Comparing `kestrel-lang-1.7.2/tests/test_timestamped.py` & `kestrel-lang-1.7.3/tests/test_timestamped.py`

 * *Files identical despite different names*

