# Comparing `tmp/py3seed-0.2.2.tar.gz` & `tmp/py3seed-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.2.2.tar", last modified: Fri Jul 21 09:05:34 2023, max compression
+gzip compressed data, was "py3seed-0.2.3.tar", last modified: Thu Jul 27 13:12:08 2023, max compression
```

## Comparing `py3seed-0.2.2.tar` & `py3seed-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.024086 py3seed-0.2.2/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.2/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-21 09:05:34.024207 py3seed-0.2.2/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.2/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.2/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-21 09:05:34.024801 py3seed-0.2.2/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.2/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.002187 py3seed-0.2.2/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.014601 py3seed-0.2.2/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.2/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.2/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.2/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.2/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.018261 py3seed-0.2.2/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.2/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    21146 2023-07-19 07:50:14.000000 py3seed-0.2.2/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.2/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.2/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.2/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.2/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.2/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.2/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14673 2023-07-19 03:29:37.000000 py3seed-0.2.2/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.2/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.017204 py3seed-0.2.2/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-21 09:05:33.000000 py3seed-0.2.2/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-21 09:05:34.023473 py3seed-0.2.2/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.2/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6599 2023-07-18 07:07:02.000000 py3seed-0.2.2/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.2/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.2/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.2/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.582430 py3seed-0.2.3/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.2.3/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-27 13:12:08.582744 py3seed-0.2.3/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.2.3/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.2.3/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-27 13:12:08.583961 py3seed-0.2.3/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.2.3/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.546386 py3seed-0.2.3/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.566645 py3seed-0.2.3/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.2.3/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.2.3/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.2.3/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7571 2023-07-21 09:02:47.000000 py3seed-0.2.3/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.573471 py3seed-0.2.3/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.2.3/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    20578 2023-07-26 12:37:30.000000 py3seed-0.2.3/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.2.3/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.2.3/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.2.3/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.2.3/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57700 2023-07-18 01:28:13.000000 py3seed-0.2.3/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.2.3/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14651 2023-07-27 13:10:29.000000 py3seed-0.2.3/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.2.3/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.572022 py3seed-0.2.3/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-27 13:12:08.000000 py3seed-0.2.3/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-27 13:12:08.581156 py3seed-0.2.3/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4032 2023-07-21 09:03:11.000000 py3seed-0.2.3/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6589 2023-07-22 05:05:45.000000 py3seed-0.2.3/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.2.3/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.2.3/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.2.3/tests/test_mongosupport.py
```

### Comparing `py3seed-0.2.2/LICENSE` & `py3seed-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/PKG-INFO` & `py3seed-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.2/setup.cfg` & `py3seed-0.2.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.2.2
+version = 0.2.3
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.2.2/src/py3seed/__init__.py` & `py3seed-0.2.3/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed/__main__.py` & `py3seed-0.2.3/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed/admin.py` & `py3seed-0.2.3/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed/cachesupport.py` & `py3seed-0.2.3/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed/commands/gen.py` & `py3seed-0.2.3/src/py3seed/commands/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,19 +126,18 @@
     env.globals['new_model'] = new_model
     env.globals['match_field'] = match_field
     env.globals['parse_layout_fields'] = parse_layout_fields
     #
     return env
 
 
-def _gen(ms: str, ds: str):
+def _gen(ds: str = None):
     """ Gen. """
-    include_models = [m.strip() for m in ms.split(',')] if ms else []
     include_domains = [d.strip() for d in ds.split(',')] if ds else []
-    logger.info(f'Gen for domain(s) {include_models} under domain(s) {include_domains}')
+    logger.info(f'Gen under domain(s) {include_domains}')
     # Domains should be project folders, i.e, [www, miniapp, android, ios, ...]
     for d in include_domains:
         if not os.path.exists(d):
             logger.error(f'Can not find domain {d}')
             return False
     #
     # Load all model's schema and views
@@ -211,18 +210,14 @@
                     **generate_names(name)
                 })
             # Views may be empty if no views match
             if not views:
                 continue
             #
             model_setting['views'] = views
-            # Filter model if include_models has value
-            if include_models and include_models.count(model_name) == 0:  # case-sensitive
-                continue
-            #
             model_settings[model_name] = model_setting
     #
     if not model_settings:
         logger.error('Can not find any models to gen')
         return False
     #
     # For each domain:
@@ -495,27 +490,18 @@
                     os.remove(o_name)
 
 
 def main(args: List[str]) -> bool:
     """ Main. """
     parser = argparse.ArgumentParser(prog="pyseed gen")
     parser.add_argument(
-        '-m',
-        nargs='?',
-        metavar='models',
-        default=None,
-        help='Tells pyseed to generate action for specific models.'
-             'e.g,'
-             '-m User means generating all views for User model'
-    )
-    parser.add_argument(
         '-d',
         nargs='?',
         metavar='domains',
         default=None,
         help='Tells pyseed to generate action for specific domains.'
              'e.g,'
              '-d www means generating all models\' views under www domain'
              '-m User -d www means generating all views for User model under www domain'
     )
     parsed_args = parser.parse_args(args)
-    return _gen(parsed_args.m, parsed_args.d)
+    return _gen(parsed_args.d)
```

### Comparing `py3seed-0.2.2/src/py3seed/error.py` & `py3seed-0.2.3/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed/inflection.py` & `py3seed-0.2.3/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed/log.py` & `py3seed-0.2.3/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed/merge3.py` & `py3seed-0.2.3/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed/model.py` & `py3seed-0.2.3/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed/mongosupport.py` & `py3seed-0.2.3/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed/utils.py` & `py3seed-0.2.3/src/py3seed/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,20 +177,19 @@
             # Parse segment, first line is fields seperated by comma and the rest are layout of each field
             index_line = segment[0]
             columns = [_parse_column(c) for c in index_line.split(',')]
             #
             # Cut inner layout
             #
             if len(segment) > 1:
-                # logger.debug(f'{leading} Parsing level {level} segment:\n' + '\n'.join(segment))
+                # logger.debug(f'{leading}Parsing level {level} segment:\n' + '\n'.join(segment))
                 body_lines = segment[1:]
                 # Inject layout for each column
                 for j in range(0, len(columns)):
                     column = columns[j]
-                    col_name = column['name']
                     start_position = index_line.index(column['raw'])
                     if j < len(columns) - 1:
                         end_position = index_line.index(columns[j + 1]['name'])
                         col_lines = [l[start_position:end_position] for l in body_lines]
                     else:
                         col_lines = [l[start_position:] for l in body_lines]
                     # Remove empty lines
@@ -203,15 +202,15 @@
             # Parse inner layout and do validation
             #
             for j in range(0, len(columns)):
                 column = columns[j]
                 col_name = column['name']
                 #
                 col_lines = column.get('lines', None)
-                logger.debug(f'{leading} Column ({i},{j}): {col_name}' + (('\n' + '\n'.join(col_lines)) if col_lines else ''))
+                logger.debug(f'{leading}Column ({i},{j}): {col_name}' + (('\n' + '\n'.join(col_lines)) if col_lines else ''))
                 #
                 # Column name possible values:
                 # 1) blank column prints only a placeholder
                 # 2) hyphen(-) prints line separator, i.e, <hr/>
                 # 3) group column(integer/float) combines multiple fields
                 #
                 # Blank column
@@ -255,14 +254,15 @@
     def _parse_column(column_str):
         """ Parse column string, having params and format-span, e.g, a?param=1#4. """
         column_str = column_str.strip()
         ret = {
             'raw': column_str,
             'format': None,
             'span': None,
+            'params': {},
         }
         # Parse span at the end, e.g, a?param=1#summary4
         format_span_match = FORMAT_SPAN_REGEX.match(column_str)
         if format_span_match:
             column_str = format_span_match.group(1)
             if format_span_match.group(2):
                 ret.update({'format': format_span_match.group(2)})  # -> summary
```

### Comparing `py3seed-0.2.2/src/py3seed/websupport.py` & `py3seed-0.2.3/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.2.3/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.2.2/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.2.3/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/tests/test_cachesupport.py` & `py3seed-0.2.3/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/tests/test_gen.py` & `py3seed-0.2.3/tests/test_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 </body>
 </html>'''
     with open('www/templates/public/team-members.html', 'w', encoding='utf-8') as f:
         f.write(this)
     #
     # Generate
     #
-    _gen(None, None)
+    _gen()
     #
     # Test Cases
     #
     # public.py should be not changed, as public.py.0 exsits
     public_py = open('www/views/public.py', encoding='utf-8').read()
     assert public_py == '''""" public module. """
 from flask import Blueprint, render_template, jsonify
```

### Comparing `py3seed-0.2.2/tests/test_merge3.py` & `py3seed-0.2.3/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/tests/test_model.py` & `py3seed-0.2.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.2.2/tests/test_mongosupport.py` & `py3seed-0.2.3/tests/test_mongosupport.py`

 * *Files identical despite different names*

