# Comparing `tmp/clargs-0.5.3.tar.gz` & `tmp/clargs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clargs-0.5.3.tar", last modified: Tue Jul 18 14:21:24 2023, max compression
+gzip compressed data, was "clargs-0.6.0.tar", last modified: Thu Jul 27 10:38:46 2023, max compression
```

## Comparing `clargs-0.5.3.tar` & `clargs-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:24.950466 clargs-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:24.946467 clargs-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:24.946467 clargs-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-18 14:21:15.000000 clargs-0.5.3/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-18 14:21:15.000000 clargs-0.5.3/.github/workflows/upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 14:21:15.000000 clargs-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 14:21:15.000000 clargs-0.5.3/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-18 14:21:24.950466 clargs-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-07-18 14:21:15.000000 clargs-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:24.950466 clargs-0.5.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-18 14:21:15.000000 clargs-0.5.3/examples/0_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-18 14:21:15.000000 clargs-0.5.3/examples/1_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-18 14:21:15.000000 clargs-0.5.3/examples/2_show_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-18 14:21:15.000000 clargs-0.5.3/examples/3_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-18 14:21:15.000000 clargs-0.5.3/examples/4_parse_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    20370 2023-07-18 14:21:15.000000 clargs-0.5.3/examples/5_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-18 14:21:15.000000 clargs-0.5.3/examples/__generate_example_output__.sh
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-18 14:21:15.000000 clargs-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:21:24.950466 clargs-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:24.946467 clargs-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:24.950466 clargs-0.5.3/src/clargs/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-18 14:21:15.000000 clargs-0.5.3/src/clargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-07-18 14:21:15.000000 clargs-0.5.3/src/clargs/aap_from_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-18 14:21:15.000000 clargs-0.5.3/src/clargs/clargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-18 14:21:15.000000 clargs-0.5.3/src/clargs/docsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-18 14:21:15.000000 clargs-0.5.3/src/clargs/helper_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:24.950466 clargs-0.5.3/src/clargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-18 14:21:24.000000 clargs-0.5.3/src/clargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 14:21:24.000000 clargs-0.5.3/src/clargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:21:24.000000 clargs-0.5.3/src/clargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 14:21:24.000000 clargs-0.5.3/src/clargs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:21:24.950466 clargs-0.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-18 14:21:15.000000 clargs-0.5.3/test/test_docsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23344 2023-07-18 14:21:15.000000 clargs-0.5.3/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 14:21:15.000000 clargs-0.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.697434 clargs-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.693434 clargs-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.693434 clargs-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-27 10:38:36.000000 clargs-0.6.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 10:38:36.000000 clargs-0.6.0/.github/workflows/upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 10:38:36.000000 clargs-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 10:38:36.000000 clargs-0.6.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 10:38:46.697434 clargs-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-07-27 10:38:36.000000 clargs-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.697434 clargs-0.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/0_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/1_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/2_show_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/3_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/4_parse_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20370 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/5_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-27 10:38:36.000000 clargs-0.6.0/examples/__generate_example_output__.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 10:38:36.000000 clargs-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 10:38:46.697434 clargs-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.693434 clargs-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.697434 clargs-0.6.0/src/clargs/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-27 10:38:36.000000 clargs-0.6.0/src/clargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-07-27 10:38:36.000000 clargs-0.6.0/src/clargs/aap_from_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-27 10:38:36.000000 clargs-0.6.0/src/clargs/clargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-27 10:38:36.000000 clargs-0.6.0/src/clargs/docsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-27 10:38:36.000000 clargs-0.6.0/src/clargs/helper_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.697434 clargs-0.6.0/src/clargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 10:38:46.000000 clargs-0.6.0/src/clargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-27 10:38:46.000000 clargs-0.6.0/src/clargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:38:46.000000 clargs-0.6.0/src/clargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 10:38:46.000000 clargs-0.6.0/src/clargs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:38:46.697434 clargs-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-27 10:38:36.000000 clargs-0.6.0/test/test_docsparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24402 2023-07-27 10:38:36.000000 clargs-0.6.0/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-27 10:38:36.000000 clargs-0.6.0/tox.ini
```

### Comparing `clargs-0.5.3/.github/workflows/run-tests.yml` & `clargs-0.6.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/.github/workflows/upload.yml` & `clargs-0.6.0/.github/workflows/upload.yml`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/LICENCE.txt` & `clargs-0.6.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/PKG-INFO` & `clargs-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clargs
-Version: 0.5.3
+Version: 0.6.0
 Summary: Easily generate commandline apps from your functions, based on type hints
 Author-email: Claude <pypi@claude.nl>
 Project-URL: Homepage, https://github.com/reinhrst/clargs
 Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clargs-0.5.3/README.md` & `clargs-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/examples/0_basic.py` & `clargs-0.6.0/examples/0_basic.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/examples/1_flags.py` & `clargs-0.6.0/examples/1_flags.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/examples/2_show_defaults.py` & `clargs-0.6.0/examples/2_show_defaults.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/examples/3_list.py` & `clargs-0.6.0/examples/3_list.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/examples/4_parse_groups.py` & `clargs-0.6.0/examples/4_parse_groups.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/examples/5_logging.py` & `clargs-0.6.0/examples/5_logging.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/examples/__generate_example_output__.sh` & `clargs-0.6.0/examples/__generate_example_output__.sh`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/pyproject.toml` & `clargs-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/src/clargs/__init__.py` & `clargs-0.6.0/src/clargs/__init__.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/src/clargs/aap_from_data.py` & `clargs-0.6.0/src/clargs/aap_from_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     def has_default(self) -> bool:
         return self.param.default is not inspect.Parameter.empty
 
     def get_all_param_names(self) -> t.Sequence[str]:
         has_custom_name = self.extra_info.name is not clargs.NOT_SET
         param_name_with_replacement = (
             self.param.name.replace("_", "-")
-            if self.settings.replace_underscore_with_dash
+            if self.settings.replace_underscore_with_dash and self.arg_type_is_flag()
             else self.param.name
         )
         param_name = t.cast(
             str,
             self.extra_info.name
             if has_custom_name
             else ("" if self.arg_type_is_positional() else self.settings.flag_prefix)
```

### Comparing `clargs-0.5.3/src/clargs/clargs.py` & `clargs-0.6.0/src/clargs/clargs.py`

 * *Files 10% similar despite different names*

```diff
@@ -270,17 +270,26 @@
             new_args_and_aap_s.append((new_names, aap))
         return new_args_and_aap_s
 
     @staticmethod
     def run(args):
         logger.debug("Received parsed args %s", args)
         assert "_clargs_func_" in args
-        return args._clargs_func_(
-            **{k: v for k, v in vars(args).items() if k != "_clargs_func_"}
-        )
+        function = args._clargs_func_
+        positional_parameters = [
+            param
+            for param in inspect.signature(function).parameters.values()
+            if param.kind == inspect.Parameter.POSITIONAL_ONLY
+        ]
+        argsdict = vars(args)
+        args = {p.name: argsdict[p.name] for p in positional_parameters}
+        kwargs = {
+            k: v for k, v in argsdict.items() if k != "_clargs_func_" and k not in args
+        }
+        return function(*args.values(), **kwargs)
 
     def create_parser_and_run(self, func: t.Callable[..., RET], args=None) -> RET:
         parser = self.create_parser(func)
         return Clargs.run(parser.parse_args(args))
 
 
 def create_parser(func: t.Callable) -> argparse.ArgumentParser:
```

### Comparing `clargs-0.5.3/src/clargs/docsparser.py` & `clargs-0.6.0/src/clargs/docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/src/clargs/helper_types.py` & `clargs-0.6.0/src/clargs/helper_types.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/src/clargs.egg-info/PKG-INFO` & `clargs-0.6.0/src/clargs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clargs
-Version: 0.5.3
+Version: 0.6.0
 Summary: Easily generate commandline apps from your functions, based on type hints
 Author-email: Claude <pypi@claude.nl>
 Project-URL: Homepage, https://github.com/reinhrst/clargs
 Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clargs-0.5.3/src/clargs.egg-info/SOURCES.txt` & `clargs-0.6.0/src/clargs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/test/test_docsparser.py` & `clargs-0.6.0/test/test_docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.5.3/test/test_simple.py` & `clargs-0.6.0/test/test_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,43 @@
         parser = clargs.create_parser(function)
         args = parser.parse_args(["--my-number", "3"])
         self.assertEqual(vars(args), {"_clargs_func_": function, "my_number": 3})
         self.assertEqual(clargs.run(args), 3)
         with self.assertExit(msg="unrecognized arguments: --my_number 3"):
             args = parser.parse_args(["--my_number", "3"])
 
+    def test_positional_param_name_with_underscore(self):
+        def function(my_number: int = 2):
+            return my_number
+
+        parser = clargs.create_parser(function)
+        args = parser.parse_args(["3"])
+        self.assertEqual(vars(args), {"_clargs_func_": function, "my_number": 3})
+        self.assertEqual(clargs.run(args), 3)
+
+    def test_positional_only_param(self):
+        def function(mynumber: int = 2, /):
+            return mynumber
+
+        parser = clargs.create_parser(function)
+        args = parser.parse_args(["3"])
+        self.assertEqual(vars(args), {"_clargs_func_": function, "mynumber": 3})
+        self.assertEqual(clargs.run(args), 3)
+
+    def test_mixed_params(self):
+        def function(a: int, /, b: int, *, c: int):
+            return a + b + c
+
+        parser = clargs.create_parser(function)
+        args = parser.parse_args(["3", "5", "--c", "7"])
+        self.assertEqual(
+            vars(args), {"_clargs_func_": function, "a": 3, "b": 5, "c": 7}
+        )
+        self.assertEqual(clargs.run(args), 15)
+
 
 class TestBooleans(Base):
     def test_boolean(self):
         def function(flag: bool):
             pass
 
         parser = clargs.create_parser(function)
```

