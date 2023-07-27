# Comparing `tmp/rsoup-3.1.0.tar.gz` & `tmp/rsoup-3.1.1.tar.gz`

## Comparing `rsoup-3.1.0.tar` & `rsoup-3.1.1.tar`

### file list

```diff
@@ -1,70 +1,72 @@
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 rsoup-3.1.0/Cargo.toml
--rw-r--r--   0     1001      123     1856 2023-06-29 19:20:59.000000 rsoup-3.1.0/.github/workflows/ci.yml
--rw-r--r--   0     1001      123     1815 2023-06-29 19:20:59.000000 rsoup-3.1.0/.gitignore
--rw-r--r--   0     1001      123     1064 2023-06-29 19:20:59.000000 rsoup-3.1.0/LICENSE
--rw-r--r--   0     1001      123      118 2023-06-29 19:20:59.000000 rsoup-3.1.0/README.md
--rw-r--r--   0     1001      123     3490 2023-06-29 19:20:59.000000 rsoup-3.1.0/benches/context_recursive_extractor_benchmark.rs
--rw-r--r--   0     1001      123     1830 2023-06-29 19:20:59.000000 rsoup-3.1.0/benches/get_text.rs
--rw-r--r--   0     1001      123      827 2023-06-29 19:20:59.000000 rsoup-3.1.0/pyproject.toml
--rw-r--r--   0     1001      123        0 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/__init__.py
--rw-r--r--   0     1001      123     5477 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/core.pyi
--rw-r--r--   0     1001      123      586 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/exceptions.py
--rw-r--r--   0     1001      123      561 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/fetch_tables.py
--rw-r--r--   0     1001      123    15212 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/python/context_extractor.py
--rw-r--r--   0     1001      123        0 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/python/models/__init__.py
--rw-r--r--   0     1001      123     3091 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/python/models/context.py
--rw-r--r--   0     1001      123     9840 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/python/models/html_table.py
--rw-r--r--   0     1001      123    11141 2023-06-29 19:20:59.000000 rsoup-3.1.0/rsoup/python/table_extractor.py
--rw-r--r--   0     1001      123        4 2023-06-29 19:20:59.000000 rsoup-3.1.0/scripts/.gitignore
--rw-r--r--   0     1001      123      722 2023-06-29 19:20:59.000000 rsoup-3.1.0/scripts/gen_data.py
--rw-r--r--   0     1001      123     1528 2023-06-29 19:20:59.000000 rsoup-3.1.0/scripts/test_table_extractor.py
--rw-r--r--   0     1001      123     1072 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/error.rs
--rw-r--r--   0     1001      123    25491 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/context_v1.rs
--rw-r--r--   0     1001      123     4879 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/elementrefview.rs
--rw-r--r--   0     1001      123     1069 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/mod.rs
--rw-r--r--   0     1001      123    10224 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/table.rs
--rw-r--r--   0     1001      123    11019 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/text/get_rich_text.rs
--rw-r--r--   0     1001      123     3477 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/text/get_text_v1.rs
--rw-r--r--   0     1001      123     2691 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/text/get_text_v2.rs
--rw-r--r--   0     1001      123     3595 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/text/line.rs
--rw-r--r--   0     1001      123     1302 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/extractors/text/mod.rs
--rw-r--r--   0     1001      123      848 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/lib.rs
--rw-r--r--   0     1001      123     1042 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/mod.rs
--rw-r--r--   0     1001      123      404 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/range_iter.rs
--rw-r--r--   0     1001      123     5634 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/recursive_iter.rs
--rw-r--r--   0     1001      123     3474 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/tree/iterator.rs
--rw-r--r--   0     1001      123       39 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/tree/mod.rs
--rw-r--r--   0     1001      123     6158 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/tree/simple_tree.rs
--rw-r--r--   0     1001      123     1600 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/misc/url_converter.rs
--rw-r--r--   0     1001      123     4651 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/content_hierarchy.rs
--rw-r--r--   0     1001      123       61 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/mod.rs
--rw-r--r--   0     1001      123    13378 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/rich_text.rs
--rw-r--r--   0     1001      123     1824 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/cell.rs
--rw-r--r--   0     1001      123     2926 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/cell_iter.rs
--rw-r--r--   0     1001      123      158 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/mod.rs
--rw-r--r--   0     1001      123     2036 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/row.rs
--rw-r--r--   0     1001      123      591 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/row_iter.rs
--rw-r--r--   0     1001      123    13112 2023-06-29 19:20:59.000000 rsoup-3.1.0/src/models/table/table.rs
--rw-r--r--   0     1001      123        0 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/__init__.py
--rw-r--r--   0     1001      123      639 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/conftest.py
--rw-r--r--   0     1001      123        0 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/__init__.py
--rw-r--r--   0     1001      123       79 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/mod.rs
--rw-r--r--   0     1001      123     3639 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/test_context_extractor.rs
--rw-r--r--   0     1001      123     3052 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/test_table_extractor.py
--rw-r--r--   0     1001      123     1389 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/test_table_extractor.rs
--rw-r--r--   0     1001      123     3573 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/extractors/test_text_extractor.rs
--rw-r--r--   0     1001      123      511 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/main.rs
--rw-r--r--   0     1001      123        0 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/models/__init__.py
--rw-r--r--   0     1001      123       20 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/models/mod.rs
--rw-r--r--   0     1001      123     1889 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/models/test_table.rs
--rw-r--r--   0     1001      123      867 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/models/test_table_pickle.py
--rw-r--r--   0     1001      123    38251 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/extractors/context/list_highest_mountains.html
--rw-r--r--   0     1001      123      326 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/extractors/context/one-level.html
--rw-r--r--   0     1001      123      568 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/extractors/context/three-level.html
--rw-r--r--   0     1001      123     4917 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/extractors/table.html
--rw-r--r--   0     1001      123     1327 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/extractors/text.html
--rw-r--r--   0     1001      123     2648 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/table_span.html
--rw-r--r--   0     1001      123    77654 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html
--rw-r--r--   0     1001      123   381850 2023-06-29 19:20:59.000000 rsoup-3.1.0/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html
--rw-r--r--   0     1001      123    41375 2023-06-29 19:20:59.000000 rsoup-3.1.0/Cargo.lock
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 rsoup-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 rsoup-3.1.1/Cargo.toml
+-rw-r--r--   0     1001      123     2132 2023-07-27 00:23:25.000000 rsoup-3.1.1/.github/workflows/build.sh
+-rw-r--r--   0     1001      123     3089 2023-07-27 00:23:25.000000 rsoup-3.1.1/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123     3168 2023-07-27 00:23:25.000000 rsoup-3.1.1/.github/workflows/pydiscovery.py
+-rw-r--r--   0     1001      123     1815 2023-07-27 00:23:25.000000 rsoup-3.1.1/.gitignore
+-rw-r--r--   0     1001      123     1064 2023-07-27 00:23:25.000000 rsoup-3.1.1/LICENSE
+-rw-r--r--   0     1001      123      118 2023-07-27 00:23:25.000000 rsoup-3.1.1/README.md
+-rw-r--r--   0     1001      123     3490 2023-07-27 00:23:25.000000 rsoup-3.1.1/benches/context_recursive_extractor_benchmark.rs
+-rw-r--r--   0     1001      123     1830 2023-07-27 00:23:25.000000 rsoup-3.1.1/benches/get_text.rs
+-rw-r--r--   0     1001      123      860 2023-07-27 00:23:25.000000 rsoup-3.1.1/pyproject.toml
+-rw-r--r--   0     1001      123        0 2023-07-27 00:23:25.000000 rsoup-3.1.1/rsoup/__init__.py
+-rw-r--r--   0     1001      123     5477 2023-07-27 00:23:25.000000 rsoup-3.1.1/rsoup/core.pyi
+-rw-r--r--   0     1001      123      586 2023-07-27 00:23:25.000000 rsoup-3.1.1/rsoup/exceptions.py
+-rw-r--r--   0     1001      123      561 2023-07-27 00:23:25.000000 rsoup-3.1.1/rsoup/fetch_tables.py
+-rw-r--r--   0     1001      123    15212 2023-07-27 00:23:25.000000 rsoup-3.1.1/rsoup/python/context_extractor.py
+-rw-r--r--   0     1001      123        0 2023-07-27 00:23:25.000000 rsoup-3.1.1/rsoup/python/models/__init__.py
+-rw-r--r--   0     1001      123     3091 2023-07-27 00:23:25.000000 rsoup-3.1.1/rsoup/python/models/context.py
+-rw-r--r--   0     1001      123     9840 2023-07-27 00:23:25.000000 rsoup-3.1.1/rsoup/python/models/html_table.py
+-rw-r--r--   0     1001      123    11141 2023-07-27 00:23:25.000000 rsoup-3.1.1/rsoup/python/table_extractor.py
+-rw-r--r--   0     1001      123        4 2023-07-27 00:23:25.000000 rsoup-3.1.1/scripts/.gitignore
+-rw-r--r--   0     1001      123      722 2023-07-27 00:23:25.000000 rsoup-3.1.1/scripts/gen_data.py
+-rw-r--r--   0     1001      123     1528 2023-07-27 00:23:25.000000 rsoup-3.1.1/scripts/test_table_extractor.py
+-rw-r--r--   0     1001      123     1072 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/error.rs
+-rw-r--r--   0     1001      123    25491 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/extractors/context_v1.rs
+-rw-r--r--   0     1001      123     4879 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/extractors/elementrefview.rs
+-rw-r--r--   0     1001      123     1069 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/extractors/mod.rs
+-rw-r--r--   0     1001      123    10224 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/extractors/table.rs
+-rw-r--r--   0     1001      123    11019 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/extractors/text/get_rich_text.rs
+-rw-r--r--   0     1001      123     3477 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/extractors/text/get_text_v1.rs
+-rw-r--r--   0     1001      123     2691 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/extractors/text/get_text_v2.rs
+-rw-r--r--   0     1001      123     3595 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/extractors/text/line.rs
+-rw-r--r--   0     1001      123     1302 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/extractors/text/mod.rs
+-rw-r--r--   0     1001      123      848 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/lib.rs
+-rw-r--r--   0     1001      123     1042 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/misc/mod.rs
+-rw-r--r--   0     1001      123      404 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/misc/range_iter.rs
+-rw-r--r--   0     1001      123     5634 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/misc/recursive_iter.rs
+-rw-r--r--   0     1001      123     3474 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/misc/tree/iterator.rs
+-rw-r--r--   0     1001      123       39 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/misc/tree/mod.rs
+-rw-r--r--   0     1001      123     6158 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/misc/tree/simple_tree.rs
+-rw-r--r--   0     1001      123     1600 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/misc/url_converter.rs
+-rw-r--r--   0     1001      123     4651 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/models/content_hierarchy.rs
+-rw-r--r--   0     1001      123       61 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/models/mod.rs
+-rw-r--r--   0     1001      123    13378 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/models/rich_text.rs
+-rw-r--r--   0     1001      123     1824 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/models/table/cell.rs
+-rw-r--r--   0     1001      123     2926 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/models/table/cell_iter.rs
+-rw-r--r--   0     1001      123      158 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/models/table/mod.rs
+-rw-r--r--   0     1001      123     2036 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/models/table/row.rs
+-rw-r--r--   0     1001      123      591 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/models/table/row_iter.rs
+-rw-r--r--   0     1001      123    13112 2023-07-27 00:23:25.000000 rsoup-3.1.1/src/models/table/table.rs
+-rw-r--r--   0     1001      123        0 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/__init__.py
+-rw-r--r--   0     1001      123      639 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/conftest.py
+-rw-r--r--   0     1001      123        0 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/extractors/__init__.py
+-rw-r--r--   0     1001      123       79 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/extractors/mod.rs
+-rw-r--r--   0     1001      123     3639 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/extractors/test_context_extractor.rs
+-rw-r--r--   0     1001      123     3052 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/extractors/test_table_extractor.py
+-rw-r--r--   0     1001      123     1389 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/extractors/test_table_extractor.rs
+-rw-r--r--   0     1001      123     3573 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/extractors/test_text_extractor.rs
+-rw-r--r--   0     1001      123      511 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/main.rs
+-rw-r--r--   0     1001      123        0 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/models/__init__.py
+-rw-r--r--   0     1001      123       20 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/models/mod.rs
+-rw-r--r--   0     1001      123     1889 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/models/test_table.rs
+-rw-r--r--   0     1001      123      867 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/models/test_table_pickle.py
+-rw-r--r--   0     1001      123    38251 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/resources/extractors/context/list_highest_mountains.html
+-rw-r--r--   0     1001      123      326 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/resources/extractors/context/one-level.html
+-rw-r--r--   0     1001      123      568 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/resources/extractors/context/three-level.html
+-rw-r--r--   0     1001      123     4917 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/resources/extractors/table.html
+-rw-r--r--   0     1001      123     1327 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/resources/extractors/text.html
+-rw-r--r--   0     1001      123     2648 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/resources/table_span.html
+-rw-r--r--   0     1001      123    77654 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html
+-rw-r--r--   0     1001      123   381850 2023-07-27 00:23:25.000000 rsoup-3.1.1/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html
+-rw-r--r--   0     1001      123    41375 2023-07-27 00:23:25.000000 rsoup-3.1.1/Cargo.lock
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 rsoup-3.1.1/PKG-INFO
```

### Comparing `rsoup-3.1.0/Cargo.toml` & `rsoup-3.1.1/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 base64 = "0.13.0"
 criterion = "0.3.6"
 ego-tree = "0.6.2"
 hashbrown = { version = "0.12.3", features = ["serde"] }
 lazy_static = "1.4.0"
 phf = { version = "0.11.0", features = ["macros"] }
 postcard = { version = "1.0.1", features = ["alloc"] }
-pyo3 = { version = "0.16.3", features = ["anyhow", "hashbrown", "serde"] } 
+pyo3 = { version = "0.16.3", features = ["anyhow", "hashbrown", "serde"] }
 regex = "1.6.0"
 scraper = "0.17.1"
 serde = "1.0.143"
 serde_json = { version = "1.0.83", features = ["preserve_order"] }
 smallvec = "1.9.0"
 thiserror = "1.0.32"
 url = "2.2.2"
 
 [features]
 extension-module = ["pyo3/extension-module"]
-default = ["extension-module"]
 
 [[bench]]
 # name = "context_recursive_extractor_benchmark"
 name = "get_text"
 harness = false
```

### Comparing `rsoup-3.1.0/.gitignore` & `rsoup-3.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/LICENSE` & `rsoup-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/benches/context_recursive_extractor_benchmark.rs` & `rsoup-3.1.1/benches/context_recursive_extractor_benchmark.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/benches/get_text.rs` & `rsoup-3.1.1/benches/get_text.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/pyproject.toml` & `rsoup-3.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 [project]
 name = "rsoup"
-version = "3.1.0"
-authors = [
-  { name = "Binh Vu", email = "binh@toan2.com" },
-]
+version = "3.1.1"
+authors = [{ name = "Binh Vu", email = "binh@toan2.com" }]
 description = "A library for web scraper that handles text correctly and is very fast (Rust backend)"
 readme = "README.md"
 license = { file = "LICENSE" }
 
 requires-python = ">=3.8"
 
 classifiers = [
@@ -27,11 +25,12 @@
     'pytest >= 7.1.3, < 8.0.0',
     'pytest-cov >= 4.0.0, < 5.0.0',
     'black >= 22.10.0, < 23.0.0',
 ]
 
 [tool.maturin]
 module-name = "rsoup.core"
+features = ["pyo3/extension-module"]
 
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
-build-backend = "maturin"
+build-backend = "maturin"
```

### Comparing `rsoup-3.1.0/rsoup/core.pyi` & `rsoup-3.1.1/rsoup/core.pyi`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/rsoup/exceptions.py` & `rsoup-3.1.1/rsoup/exceptions.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/rsoup/fetch_tables.py` & `rsoup-3.1.1/rsoup/fetch_tables.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/rsoup/python/context_extractor.py` & `rsoup-3.1.1/rsoup/python/context_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/rsoup/python/models/context.py` & `rsoup-3.1.1/rsoup/python/models/context.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/rsoup/python/models/html_table.py` & `rsoup-3.1.1/rsoup/python/models/html_table.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/rsoup/python/table_extractor.py` & `rsoup-3.1.1/rsoup/python/table_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/scripts/gen_data.py` & `rsoup-3.1.1/scripts/gen_data.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/scripts/test_table_extractor.py` & `rsoup-3.1.1/scripts/test_table_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/error.rs` & `rsoup-3.1.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/extractors/context_v1.rs` & `rsoup-3.1.1/src/extractors/context_v1.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/extractors/elementrefview.rs` & `rsoup-3.1.1/src/extractors/elementrefview.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/extractors/mod.rs` & `rsoup-3.1.1/src/extractors/mod.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/extractors/table.rs` & `rsoup-3.1.1/src/extractors/table.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/extractors/text/get_rich_text.rs` & `rsoup-3.1.1/src/extractors/text/get_rich_text.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/extractors/text/get_text_v1.rs` & `rsoup-3.1.1/src/extractors/text/get_text_v1.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/extractors/text/get_text_v2.rs` & `rsoup-3.1.1/src/extractors/text/get_text_v2.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/extractors/text/line.rs` & `rsoup-3.1.1/src/extractors/text/line.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/extractors/text/mod.rs` & `rsoup-3.1.1/src/extractors/text/mod.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/lib.rs` & `rsoup-3.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/misc/mod.rs` & `rsoup-3.1.1/src/misc/mod.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/misc/recursive_iter.rs` & `rsoup-3.1.1/src/misc/recursive_iter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/misc/tree/iterator.rs` & `rsoup-3.1.1/src/misc/tree/iterator.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/misc/tree/simple_tree.rs` & `rsoup-3.1.1/src/misc/tree/simple_tree.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/misc/url_converter.rs` & `rsoup-3.1.1/src/misc/url_converter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/models/content_hierarchy.rs` & `rsoup-3.1.1/src/models/content_hierarchy.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/models/rich_text.rs` & `rsoup-3.1.1/src/models/rich_text.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/models/table/cell.rs` & `rsoup-3.1.1/src/models/table/cell.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/models/table/cell_iter.rs` & `rsoup-3.1.1/src/models/table/cell_iter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/models/table/row.rs` & `rsoup-3.1.1/src/models/table/row.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/models/table/row_iter.rs` & `rsoup-3.1.1/src/models/table/row_iter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/src/models/table/table.rs` & `rsoup-3.1.1/src/models/table/table.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/conftest.py` & `rsoup-3.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/extractors/test_context_extractor.rs` & `rsoup-3.1.1/tests/extractors/test_context_extractor.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/extractors/test_table_extractor.py` & `rsoup-3.1.1/tests/extractors/test_table_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/extractors/test_table_extractor.rs` & `rsoup-3.1.1/tests/extractors/test_table_extractor.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/extractors/test_text_extractor.rs` & `rsoup-3.1.1/tests/extractors/test_text_extractor.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/models/test_table.rs` & `rsoup-3.1.1/tests/models/test_table.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/models/test_table_pickle.py` & `rsoup-3.1.1/tests/models/test_table_pickle.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/resources/extractors/context/list_highest_mountains.html` & `rsoup-3.1.1/tests/resources/extractors/context/list_highest_mountains.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/resources/extractors/context/three-level.html` & `rsoup-3.1.1/tests/resources/extractors/context/three-level.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/resources/extractors/table.html` & `rsoup-3.1.1/tests/resources/extractors/table.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/resources/extractors/text.html` & `rsoup-3.1.1/tests/resources/extractors/text.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/resources/table_span.html` & `rsoup-3.1.1/tests/resources/table_span.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html` & `rsoup-3.1.1/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html` & `rsoup-3.1.1/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/Cargo.lock` & `rsoup-3.1.1/Cargo.lock`

 * *Files identical despite different names*

### Comparing `rsoup-3.1.0/PKG-INFO` & `rsoup-3.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsoup
-Version: 3.1.0
+Version: 3.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: beautifulsoup4 >=4.9.3, <5.0.0
 Requires-Dist: html5lib >=1.1.0, <2.0.0
 Requires-Dist: requests >=2.28.0, <3.0.0
 Requires-Dist: tabulate >=0.8.10
 Requires-Dist: pytest >=7.1.3, <8.0.0 ; extra == 'dev'
```

