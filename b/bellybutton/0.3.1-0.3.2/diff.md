# Comparing `tmp/bellybutton-0.3.1.tar.gz` & `tmp/bellybutton-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bellybutton-0.3.1.tar", last modified: Fri Nov 27 21:19:40 2020, max compression
+gzip compressed data, was "dist/bellybutton-0.3.2.tar", last modified: Thu Jul 27 15:14:58 2023, max compression
```

## Comparing `bellybutton-0.3.1.tar` & `bellybutton-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hchasestevens  (1000) hchasestevens  (1000)        0 2020-11-27 21:19:40.000000 bellybutton-0.3.1/
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)      751 2020-11-27 21:19:40.000000 bellybutton-0.3.1/PKG-INFO
-drwxr-xr-x   0 hchasestevens  (1000) hchasestevens  (1000)        0 2020-11-27 21:19:40.000000 bellybutton-0.3.1/bellybutton.egg-info/
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)      398 2020-11-27 21:19:40.000000 bellybutton-0.3.1/bellybutton.egg-info/SOURCES.txt
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)       12 2020-11-27 21:19:40.000000 bellybutton-0.3.1/bellybutton.egg-info/top_level.txt
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)       87 2020-11-27 21:19:40.000000 bellybutton-0.3.1/bellybutton.egg-info/requires.txt
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)      751 2020-11-27 21:19:40.000000 bellybutton-0.3.1/bellybutton.egg-info/PKG-INFO
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)       54 2020-11-27 21:19:40.000000 bellybutton-0.3.1/bellybutton.egg-info/entry_points.txt
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)        1 2020-11-27 21:19:40.000000 bellybutton-0.3.1/bellybutton.egg-info/dependency_links.txt
-drwxr-xr-x   0 hchasestevens  (1000) hchasestevens  (1000)        0 2020-11-27 21:19:40.000000 bellybutton-0.3.1/bellybutton/
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)     5249 2020-11-27 21:19:22.000000 bellybutton-0.3.1/bellybutton/parsing.py
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)        0 2020-11-27 21:19:22.000000 bellybutton-0.3.1/bellybutton/__init__.py
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)      138 2020-11-27 21:19:22.000000 bellybutton-0.3.1/bellybutton/exceptions.py
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)     6813 2020-11-27 21:19:22.000000 bellybutton-0.3.1/bellybutton/cli.py
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)       25 2020-11-27 21:19:22.000000 bellybutton-0.3.1/bellybutton/caching.py
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)     1312 2020-11-27 21:19:22.000000 bellybutton-0.3.1/bellybutton/initialization.py
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)     2772 2020-11-27 21:19:22.000000 bellybutton-0.3.1/bellybutton/linting.py
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)       38 2020-11-27 21:19:40.000000 bellybutton-0.3.1/setup.cfg
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)     1169 2020-11-27 21:19:22.000000 bellybutton-0.3.1/setup.py
--rw-r--r--   0 hchasestevens  (1000) hchasestevens  (1000)     5604 2020-11-27 21:19:22.000000 bellybutton-0.3.1/README.md
+drwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)        0 2023-07-27 15:14:58.000000 bellybutton-0.3.2/
+drwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)        0 2023-07-27 15:14:58.000000 bellybutton-0.3.2/bellybutton/
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)       25 2018-02-26 03:34:17.000000 bellybutton-0.3.2/bellybutton/caching.py
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)     7038 2023-07-27 15:12:45.000000 bellybutton-0.3.2/bellybutton/cli.py
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)      144 2018-02-17 16:35:24.000000 bellybutton-0.3.2/bellybutton/exceptions.py
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)     1371 2018-02-25 18:37:56.000000 bellybutton-0.3.2/bellybutton/initialization.py
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)     2856 2023-07-27 15:12:45.000000 bellybutton-0.3.2/bellybutton/linting.py
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)     5432 2023-07-27 15:12:45.000000 bellybutton-0.3.2/bellybutton/parsing.py
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)        0 2018-02-17 06:25:35.000000 bellybutton-0.3.2/bellybutton/__init__.py
+drwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)        0 2023-07-27 15:14:58.000000 bellybutton-0.3.2/bellybutton.egg-info/
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)        1 2023-07-27 15:14:58.000000 bellybutton-0.3.2/bellybutton.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)       54 2023-07-27 15:14:58.000000 bellybutton-0.3.2/bellybutton.egg-info/entry_points.txt
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)      751 2023-07-27 15:14:58.000000 bellybutton-0.3.2/bellybutton.egg-info/PKG-INFO
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)       87 2023-07-27 15:14:58.000000 bellybutton-0.3.2/bellybutton.egg-info/requires.txt
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)      398 2023-07-27 15:14:58.000000 bellybutton-0.3.2/bellybutton.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)       12 2023-07-27 15:14:58.000000 bellybutton-0.3.2/bellybutton.egg-info/top_level.txt
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)      751 2023-07-27 15:14:58.000000 bellybutton-0.3.2/PKG-INFO
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)     5731 2018-08-15 10:36:02.000000 bellybutton-0.3.2/README.md
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)       38 2023-07-27 15:14:58.000000 bellybutton-0.3.2/setup.cfg
+-rwxrwxrwx   0 hchasestevens  (1000) hchasestevens  (1000)     1205 2023-07-27 15:12:45.000000 bellybutton-0.3.2/setup.py
```

### Comparing `bellybutton-0.3.1/PKG-INFO` & `bellybutton-0.3.2/bellybutton.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellybutton
-Version: 0.3.1
+Version: 0.3.2
 Summary: Custom Python linting through AST expressions.
 Home-page: https://github.com/hchasestevens/bellybutton
 Author: H. Chase Stevens
 Author-email: chase@chasestevens.com
 License: MIT
 Description: UNKNOWN
 Platform: any
```

### Comparing `bellybutton-0.3.1/bellybutton.egg-info/PKG-INFO` & `bellybutton-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellybutton
-Version: 0.3.1
+Version: 0.3.2
 Summary: Custom Python linting through AST expressions.
 Home-page: https://github.com/hchasestevens/bellybutton
 Author: H. Chase Stevens
 Author-email: chase@chasestevens.com
 License: MIT
 Description: UNKNOWN
 Platform: any
```

### Comparing `bellybutton-0.3.1/bellybutton/parsing.py` & `bellybutton-0.3.2/bellybutton/parsing.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-"""YAML parsing."""
-import re
-import ast
-import functools
-from collections import namedtuple
-
-import os
-import yaml
-from lxml.etree import XPath
-from astpath.search import find_in_ast, file_contents_to_xml_ast
-
-from bellybutton.exceptions import InvalidNode
-
-
-def constructor(tag=None, pattern=None):
-    """Register custom constructor with pyyaml."""
-    def decorator(f):
-        if tag is None or f is tag:
-            tag_ = '!{}'.format(f.__name__)
-        else:
-            tag_ = tag
-        yaml.add_constructor(tag_, f)
-        if pattern is not None:
-            yaml.add_implicit_resolver(tag_, re.compile(pattern))
-        return f
-    if callable(tag):  # little convenience hack to avoid empty arg list
-        return decorator(tag)
-    return decorator
-
-
-def _reraise_with_line_no(fn):
-    @functools.wraps(fn)
-    def wrapper(loader, node):
-        try:
-            return fn(loader, node)
-        except Exception as e:
-            msg = getattr(e, 'message', str(e))
-            raise InvalidNode(
-                "line {}: {}.".format(node.start_mark.line + 1, msg)
-            )
-    return wrapper
-
-
-@constructor(pattern=r'\~\+[/\\].+')
-@_reraise_with_line_no
-def glob(loader, node):
-    """Construct glob expressions."""
-    value = loader.construct_scalar(node)[len('~+/'):]
-    return os.path.join(
-        os.path.dirname(loader.name),
-        value
-    )
-
-
-# todo - all exprs return (parsed_expr, contents -> {lines})?
-
-@constructor(pattern=r'/.+')
-@_reraise_with_line_no
-def xpath(loader, node):
-    """Construct XPath expressions."""
-    value = loader.construct_scalar(node)
-    return XPath(value)
-
-
-@constructor
-@_reraise_with_line_no
-def regex(loader, node):
-    """Construct regular expressions."""
-    value = loader.construct_scalar(node)
-    return re.compile(value, re.MULTILINE)
-
-
-@constructor
-@_reraise_with_line_no
-def verbal(loader, node):
-    """Construct verbal expressions."""
-    values = loader.construct_sequence(node)
-    pass  # todo: verbal expressions
-
-
-@constructor
-@_reraise_with_line_no
-def chain(loader, node):
-    """Construct pipelines of other constructors."""
-    values = loader.construct_sequence(node)
-    pass  # todo: chain constructors (viz. xpath then regex)
-
-
-Settings = namedtuple('Settings', 'included excluded allow_ignore')
-
-
-@constructor
-def settings(loader, node):
-    values = loader.construct_mapping(node)
-    try:
-        return Settings(**values)
-    except TypeError:
-        for field in Settings._fields:
-            if field not in values:
-                raise InvalidNode(
-                    "!settings node missing required field `{}`.".format(field)
-                )
-        raise
-
-
-Rule = namedtuple('Rule', 'name description expr example instead settings')
-
-
-def validate_syntax(rule_clause, clause_type):
-    try:
-        ast.parse(rule_clause)
-    except SyntaxError as e:
-        raise InvalidNode("Invalid syntax in `{}` clause.".format(clause_type))
-
-
-def _reraise_with_rule_name(fn):
-    @functools.wraps(fn)
-    def wrapper(rule_name, *args, **kwargs):
-        try:
-            return fn(rule_name, *args, **kwargs)
-        except Exception as e:
-            msg = getattr(e, 'message', str(e))
-            raise InvalidNode("rule `{}`: {}".format(rule_name, msg))
-    return wrapper
-
-
-@_reraise_with_rule_name
-def parse_rule(rule_name, rule_values, default_settings=None):
-    rule_description = rule_values.get('description')
-    if rule_description is None:
-        raise InvalidNode("No description provided.")
-
-    rule_expr = rule_values.get('expr')
-    if rule_expr is None:
-        raise InvalidNode("No expression provided.".format(rule_name))
-    matches = (
-        lambda x: find_in_ast(
-            file_contents_to_xml_ast(x),
-            rule_expr.path,
-            return_lines=False
-        )
-        if isinstance(rule_expr, XPath)
-        else x.match
-    )
-
-    rule_example = rule_values.get('example')
-    if rule_example is not None:
-        validate_syntax(rule_example, clause_type='example')
-        if not matches(rule_example):
-            raise InvalidNode("`example` clause is not matched by expression.")
-
-    rule_instead = rule_values.get('instead')
-    if rule_instead is not None:
-        validate_syntax(rule_instead, clause_type='instead')
-        if matches(rule_instead):
-            raise InvalidNode("`instead` clause is matched by expression.")
-
-    rule_settings = rule_values.get('settings', default_settings)
-    if rule_settings is None:
-        raise InvalidNode("No settings or default settings specified.")
-    if not isinstance(rule_settings, Settings):
-        raise InvalidNode("Settings must be a !settings node.")
-
-    return Rule(
-        name=rule_name,
-        description=rule_description,
-        expr=rule_expr,
-        example=rule_example,
-        instead=rule_instead,
-        settings=rule_settings,
-    )
-
-
-def load_config(fileobj):
-    """Load bellybutton config file, returning a list of rules."""
-    loaded = yaml.load(fileobj, Loader = yaml.FullLoader)
-    default_settings = loaded.get('default_settings')
-    rules = [
-        parse_rule(rule_name, rule_values, default_settings)
-        for rule_name, rule_values in
-        loaded.get('rules', {}).items()
-    ]
-    return rules
+"""YAML parsing."""
+import re
+import ast
+import functools
+from collections import namedtuple
+
+import os
+import yaml
+from lxml.etree import XPath
+from astpath.search import find_in_ast, file_contents_to_xml_ast
+
+from bellybutton.exceptions import InvalidNode
+
+
+def constructor(tag=None, pattern=None):
+    """Register custom constructor with pyyaml."""
+    def decorator(f):
+        if tag is None or f is tag:
+            tag_ = '!{}'.format(f.__name__)
+        else:
+            tag_ = tag
+        yaml.add_constructor(tag_, f)
+        if pattern is not None:
+            yaml.add_implicit_resolver(tag_, re.compile(pattern))
+        return f
+    if callable(tag):  # little convenience hack to avoid empty arg list
+        return decorator(tag)
+    return decorator
+
+
+def _reraise_with_line_no(fn):
+    @functools.wraps(fn)
+    def wrapper(loader, node):
+        try:
+            return fn(loader, node)
+        except Exception as e:
+            msg = getattr(e, 'message', str(e))
+            raise InvalidNode(
+                "line {}: {}.".format(node.start_mark.line + 1, msg)
+            )
+    return wrapper
+
+
+@constructor(pattern=r'\~\+[/\\].+')
+@_reraise_with_line_no
+def glob(loader, node):
+    """Construct glob expressions."""
+    value = loader.construct_scalar(node)[len('~+/'):]
+    return os.path.join(
+        os.path.dirname(loader.name),
+        value
+    )
+
+
+# todo - all exprs return (parsed_expr, contents -> {lines})?
+
+@constructor(pattern=r'/.+')
+@_reraise_with_line_no
+def xpath(loader, node):
+    """Construct XPath expressions."""
+    value = loader.construct_scalar(node)
+    return XPath(value)
+
+
+@constructor
+@_reraise_with_line_no
+def regex(loader, node):
+    """Construct regular expressions."""
+    value = loader.construct_scalar(node)
+    return re.compile(value, re.MULTILINE)
+
+
+@constructor
+@_reraise_with_line_no
+def verbal(loader, node):
+    """Construct verbal expressions."""
+    values = loader.construct_sequence(node)
+    pass  # todo: verbal expressions
+
+
+@constructor
+@_reraise_with_line_no
+def chain(loader, node):
+    """Construct pipelines of other constructors."""
+    values = loader.construct_sequence(node)
+    pass  # todo: chain constructors (viz. xpath then regex)
+
+
+Settings = namedtuple('Settings', 'included excluded allow_ignore')
+
+
+@constructor
+def settings(loader, node):
+    values = loader.construct_mapping(node)
+    try:
+        return Settings(**values)
+    except TypeError:
+        for field in Settings._fields:
+            if field not in values:
+                raise InvalidNode(
+                    "!settings node missing required field `{}`.".format(field)
+                )
+        raise
+
+
+Rule = namedtuple('Rule', 'name description expr example instead settings')
+
+
+def validate_syntax(rule_clause, clause_type):
+    try:
+        ast.parse(rule_clause)
+    except SyntaxError as e:
+        raise InvalidNode("Invalid syntax in `{}` clause.".format(clause_type))
+
+
+def _reraise_with_rule_name(fn):
+    @functools.wraps(fn)
+    def wrapper(rule_name, *args, **kwargs):
+        try:
+            return fn(rule_name, *args, **kwargs)
+        except Exception as e:
+            msg = getattr(e, 'message', str(e))
+            raise InvalidNode("rule `{}`: {}".format(rule_name, msg))
+    return wrapper
+
+
+@_reraise_with_rule_name
+def parse_rule(rule_name, rule_values, default_settings=None):
+    rule_description = rule_values.get('description')
+    if rule_description is None:
+        raise InvalidNode("No description provided.")
+
+    rule_expr = rule_values.get('expr')
+    if rule_expr is None:
+        raise InvalidNode("No expression provided.".format(rule_name))
+    matches = (
+        lambda x: find_in_ast(
+            file_contents_to_xml_ast(x),
+            rule_expr.path,
+            return_lines=False
+        )
+        if isinstance(rule_expr, XPath)
+        else x.match
+    )
+
+    rule_example = rule_values.get('example')
+    if rule_example is not None:
+        validate_syntax(rule_example, clause_type='example')
+        if not matches(rule_example):
+            raise InvalidNode("`example` clause is not matched by expression.")
+
+    rule_instead = rule_values.get('instead')
+    if rule_instead is not None:
+        validate_syntax(rule_instead, clause_type='instead')
+        if matches(rule_instead):
+            raise InvalidNode("`instead` clause is matched by expression.")
+
+    rule_settings = rule_values.get('settings', default_settings)
+    if rule_settings is None:
+        raise InvalidNode("No settings or default settings specified.")
+    if not isinstance(rule_settings, Settings):
+        raise InvalidNode("Settings must be a !settings node.")
+
+    return Rule(
+        name=rule_name,
+        description=rule_description,
+        expr=rule_expr,
+        example=rule_example,
+        instead=rule_instead,
+        settings=rule_settings,
+    )
+
+
+def load_config(fileobj):
+    """Load bellybutton config file, returning a list of rules."""
+    loaded = yaml.load(fileobj, Loader = yaml.FullLoader)
+    default_settings = loaded.get('default_settings')
+    rules = [
+        parse_rule(rule_name, rule_values, default_settings)
+        for rule_name, rule_values in
+        loaded.get('rules', {}).items()
+    ]
+    return rules
```

### Comparing `bellybutton-0.3.1/bellybutton/cli.py` & `bellybutton-0.3.2/bellybutton/cli.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-"""Command-line interface."""
-
-from __future__ import print_function
-
-import os
-import sys
-import argparse
-import subprocess
-from collections import namedtuple
-from textwrap import dedent
-
-from bellybutton.exceptions import InvalidNode
-from bellybutton.linting import lint_file
-from bellybutton.parsing import load_config
-
-try:
-    from itertools import zip_longest
-except ImportError:
-    from itertools import izip_longest as zip_longest
-
-from bellybutton.initialization import generate_config
-
-
-PARSER = argparse.ArgumentParser()
-SUBPARSERS = PARSER.add_subparsers()
-
-
-LintingFailure = namedtuple('LintingFailure', 'failure path lineno line rule')
-
-
-def success(msg):
-    return "\033[92m{}\033[0m".format(msg)
-
-
-def error(msg):
-    return "\033[91m{}\033[0m".format(msg)
-
-
-def cli_command(fn):
-    """Register function as subcommand."""
-    command = SUBPARSERS.add_parser(fn.__name__, description=fn.__doc__)
-    command.set_defaults(func=fn)
-
-    unspecified = object()
-    args = reversed(list(zip_longest(
-        reversed(fn.__code__.co_varnames[:fn.__code__.co_argcount]),
-        reversed(fn.__defaults__),
-        fillvalue=unspecified
-    )))
-    for argument_name, default_value in args:
-        argument_name = argument_name.replace('_', '-')
-        if default_value is unspecified:
-            command.add_argument(argument_name)
-            continue
-
-        args = ['--{}'.format(argument_name)]
-        kwargs = dict(
-            default=default_value,
-            required=False,
-        )
-        if type(default_value) is bool:
-            kwargs['action'] = 'store_{!r}'.format(not default_value).lower()
-            args.append('-{}'.format(argument_name[0]))
-        else:
-            kwargs['type'] = type(default_value)
-
-        command.add_argument(
-            *args,
-            **kwargs
-        )
-
-    return fn
-
-
-@cli_command
-def init(project_directory='.', force=False):
-    """Initialize bellybutton config for project."""
-    config_path = os.path.join(project_directory, '.bellybutton.yml')
-    if os.path.exists(config_path) and not force:
-        message = 'ERROR: Path `{}` already initialized (use --force to ignore).'
-        print(error(message.format(config_path)))
-        return 1
-
-    config = generate_config(
-        directory
-        for directory in os.listdir(project_directory)
-        if os.path.isdir(os.path.join(project_directory, directory))
-        and directory.startswith('test')
-    )
-    with open(config_path, 'w') as f:
-        f.write(config)
-    return 0
-
-
-def walk_python_files(root_dir):
-    """Walk the specified directory, yielding paths for python source files."""
-    return (
-        os.path.join(root, fname)
-        for root, _, fnames in os.walk(root_dir)
-        for fname in fnames
-        if os.path.splitext(fname)[-1] == '.py'
-    )
-
-
-def open_python_files(filepaths):
-    """For each specified filepath, yield (path, content) pairs."""
-    for filepath in sorted(filepaths):
-        with open(filepath, 'r') as f:
-            contents = f.read()
-        yield filepath, contents
-
-
-def get_git_modified(project_directory):
-    """Get all modified filepaths between current ref and origin/master."""
-    subprocess.check_call(
-        'git -C "{}" fetch origin'.format(project_directory),
-        shell=True
-    )
-    diff_cmd = 'git -C "{}" diff {{}} --name-only'.format(os.path.abspath(project_directory))
-    return frozenset(
-        os.path.abspath(path)
-        for diff in ('--staged', 'origin/master...')
-        for path in subprocess.check_output(
-            diff_cmd.format(diff),
-            shell=True
-        ).decode('utf-8').strip().splitlines()
-        if os.path.splitext(path)[-1] == '.py'
-    )
-
-
-def linting_failures(filepaths, rules):
-    """Given a set of filepaths and a set of rules, yield all rule violations."""
-    failures = 0
-    files = open_python_files(filepaths)
-    for filepath, file_contents in files:
-        linting_results = list(lint_file(filepath, file_contents, rules))
-        if not linting_results:
-            continue
-        failure_results = (
-            result
-            for result in linting_results
-            if not result.succeeded
-        )
-        for failure in failure_results:
-            failures += 1
-            lines = file_contents.splitlines()
-            yield LintingFailure(
-                failure=failure,
-                path=filepath,
-                lineno=failure.lineno,
-                line=lines[min(failure.lineno, len(lines)) - 1] if lines else '',
-                rule=failure.rule,
-            )
-
-
-@cli_command
-def lint(modified_only=False, project_directory='.', verbose=False):
-    """Lint project."""
-    config_path = os.path.abspath(
-        os.path.join(project_directory, '.bellybutton.yml')
-    )
-    try:
-        with open(config_path, 'r') as f:
-            rules = load_config(f)
-    except IOError:
-        message = "ERROR: Configuration file path `{}` does not exist."
-        print(error(message.format(config_path)))
-        return 1
-    except InvalidNode as e:
-        message = "ERROR: {}, {}"
-        exc_message = getattr(e, 'message', str(e))
-        print(error(message.format(config_path, exc_message)))
-        return 1
-
-    if verbose:
-        failure_message = dedent("""
-        \033[95m{path}:{lineno}\033[0m\t\033[1;95;4m{rule.name}\033[0m
-        \033[1mDescription\033[0m: {rule.description}
-        \033[1mLine\033[0m:
-        {line}
-        \033[1mExample\033[0m:
-        {rule.example}
-        \033[1mInstead\033[0m:
-        {rule.instead}
-        """).lstrip()
-    else:
-        failure_message = "{path}:{lineno}\t{rule.name}: {rule.description}"
-
-    failures = 0
-    filepath_source = get_git_modified if modified_only else walk_python_files
-    filepaths = list(filepath_source(os.path.abspath(project_directory)))
-    for failure in linting_failures(filepaths, rules):
-        failures += 1
-        print(failure_message.format(
-            path=os.path.relpath(failure.path, project_directory),
-            lineno=failure.lineno,
-            line=failure.line,
-            rule=failure.rule
-        ))
-
-    final_message = "Linting {} ({} rule{}, {} file{}, {} violation{}).".format(
-        'failed' if failures else 'succeeded',
-        len(rules),
-        '' if len(rules) == 1 else 's',
-        len(filepaths),
-        '' if len(filepaths) == 1 else 's',
-        failures,
-        '' if failures == 1 else 's',
-    )
-    print((error if failures else success)(final_message))
-    return 1 if failures else 0
-
-
-def main():
-    """Entrypoint for CLI."""
-    args = PARSER.parse_args()
-    exit_code = args.func(**{
-        arg: getattr(args, arg)
-        for arg in args.func.__code__.co_varnames[:args.func.__code__.co_argcount]
-    })
-    sys.exit(exit_code)
-
-
-if __name__ == '__main__':
-    main()
+"""Command-line interface."""
+
+from __future__ import print_function
+
+import os
+import sys
+import argparse
+import subprocess
+from collections import namedtuple
+from textwrap import dedent
+
+from bellybutton.exceptions import InvalidNode
+from bellybutton.linting import lint_file
+from bellybutton.parsing import load_config
+
+try:
+    from itertools import zip_longest
+except ImportError:
+    from itertools import izip_longest as zip_longest
+
+from bellybutton.initialization import generate_config
+
+
+PARSER = argparse.ArgumentParser()
+SUBPARSERS = PARSER.add_subparsers()
+
+
+LintingFailure = namedtuple('LintingFailure', 'failure path lineno line rule')
+
+
+def success(msg):
+    return "\033[92m{}\033[0m".format(msg)
+
+
+def error(msg):
+    return "\033[91m{}\033[0m".format(msg)
+
+
+def cli_command(fn):
+    """Register function as subcommand."""
+    command = SUBPARSERS.add_parser(fn.__name__, description=fn.__doc__)
+    command.set_defaults(func=fn)
+
+    unspecified = object()
+    args = reversed(list(zip_longest(
+        reversed(fn.__code__.co_varnames[:fn.__code__.co_argcount]),
+        reversed(fn.__defaults__),
+        fillvalue=unspecified
+    )))
+    for argument_name, default_value in args:
+        argument_name = argument_name.replace('_', '-')
+        if default_value is unspecified:
+            command.add_argument(argument_name)
+            continue
+
+        args = ['--{}'.format(argument_name)]
+        kwargs = dict(
+            default=default_value,
+            required=False,
+        )
+        if type(default_value) is bool:
+            kwargs['action'] = 'store_{!r}'.format(not default_value).lower()
+            args.append('-{}'.format(argument_name[0]))
+        else:
+            kwargs['type'] = type(default_value)
+
+        command.add_argument(
+            *args,
+            **kwargs
+        )
+
+    return fn
+
+
+@cli_command
+def init(project_directory='.', force=False):
+    """Initialize bellybutton config for project."""
+    config_path = os.path.join(project_directory, '.bellybutton.yml')
+    if os.path.exists(config_path) and not force:
+        message = 'ERROR: Path `{}` already initialized (use --force to ignore).'
+        print(error(message.format(config_path)))
+        return 1
+
+    config = generate_config(
+        directory
+        for directory in os.listdir(project_directory)
+        if os.path.isdir(os.path.join(project_directory, directory))
+        and directory.startswith('test')
+    )
+    with open(config_path, 'w') as f:
+        f.write(config)
+    return 0
+
+
+def walk_python_files(root_dir):
+    """Walk the specified directory, yielding paths for python source files."""
+    return (
+        os.path.join(root, fname)
+        for root, _, fnames in os.walk(root_dir)
+        for fname in fnames
+        if os.path.splitext(fname)[-1] == '.py'
+    )
+
+
+def open_python_files(filepaths):
+    """For each specified filepath, yield (path, content) pairs."""
+    for filepath in sorted(filepaths):
+        with open(filepath, 'r') as f:
+            contents = f.read()
+        yield filepath, contents
+
+
+def get_git_modified(project_directory):
+    """Get all modified filepaths between current ref and origin/master."""
+    subprocess.check_call(
+        'git -C "{}" fetch origin'.format(project_directory),
+        shell=True
+    )
+    diff_cmd = 'git -C "{}" diff {{}} --name-only'.format(os.path.abspath(project_directory))
+    return frozenset(
+        os.path.abspath(path)
+        for diff in ('--staged', 'origin/master...')
+        for path in subprocess.check_output(
+            diff_cmd.format(diff),
+            shell=True
+        ).decode('utf-8').strip().splitlines()
+        if os.path.splitext(path)[-1] == '.py'
+    )
+
+
+def linting_failures(filepaths, rules):
+    """Given a set of filepaths and a set of rules, yield all rule violations."""
+    failures = 0
+    files = open_python_files(filepaths)
+    for filepath, file_contents in files:
+        linting_results = list(lint_file(filepath, file_contents, rules))
+        if not linting_results:
+            continue
+        failure_results = (
+            result
+            for result in linting_results
+            if not result.succeeded
+        )
+        for failure in failure_results:
+            failures += 1
+            lines = file_contents.splitlines()
+            yield LintingFailure(
+                failure=failure,
+                path=filepath,
+                lineno=failure.lineno,
+                line=lines[min(failure.lineno, len(lines)) - 1] if lines else '',
+                rule=failure.rule,
+            )
+
+
+@cli_command
+def lint(modified_only=False, project_directory='.', verbose=False):
+    """Lint project."""
+    config_path = os.path.abspath(
+        os.path.join(project_directory, '.bellybutton.yml')
+    )
+    try:
+        with open(config_path, 'r') as f:
+            rules = load_config(f)
+    except IOError:
+        message = "ERROR: Configuration file path `{}` does not exist."
+        print(error(message.format(config_path)))
+        return 1
+    except InvalidNode as e:
+        message = "ERROR: {}, {}"
+        exc_message = getattr(e, 'message', str(e))
+        print(error(message.format(config_path, exc_message)))
+        return 1
+
+    if verbose:
+        failure_message = dedent("""
+        \033[95m{path}:{lineno}\033[0m\t\033[1;95;4m{rule.name}\033[0m
+        \033[1mDescription\033[0m: {rule.description}
+        \033[1mLine\033[0m:
+        {line}
+        \033[1mExample\033[0m:
+        {rule.example}
+        \033[1mInstead\033[0m:
+        {rule.instead}
+        """).lstrip()
+    else:
+        failure_message = "{path}:{lineno}\t{rule.name}: {rule.description}"
+
+    failures = 0
+    filepath_source = get_git_modified if modified_only else walk_python_files
+    filepaths = list(filepath_source(os.path.abspath(project_directory)))
+    for failure in linting_failures(filepaths, rules):
+        failures += 1
+        print(failure_message.format(
+            path=os.path.relpath(failure.path, project_directory),
+            lineno=failure.lineno,
+            line=failure.line,
+            rule=failure.rule
+        ))
+
+    final_message = "Linting {} ({} rule{}, {} file{}, {} violation{}).".format(
+        'failed' if failures else 'succeeded',
+        len(rules),
+        '' if len(rules) == 1 else 's',
+        len(filepaths),
+        '' if len(filepaths) == 1 else 's',
+        failures,
+        '' if failures == 1 else 's',
+    )
+    print((error if failures else success)(final_message))
+    return 1 if failures else 0
+
+
+def main():
+    """Entrypoint for CLI."""
+    args = PARSER.parse_args()
+    exit_code = args.func(**{
+        arg: getattr(args, arg)
+        for arg in args.func.__code__.co_varnames[:args.func.__code__.co_argcount]
+    })
+    sys.exit(exit_code)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `bellybutton-0.3.1/bellybutton/initialization.py` & `bellybutton-0.3.2/bellybutton/initialization.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-"""Initialization of new bellybutton configuration files."""
-
-import os
-
-
-INIT_TEMPLATE = '''settings:
-  all_files: &all_files !settings
-    included:
-      - ~+/*
-    excluded:
-      - ~+/.tox/*
-    allow_ignore: yes
-{test_block}
-default_settings: *{default_settings}
-
-rules:
-  ExampleRule:
-    description: "Empty module."
-    expr: /Module/body[not(./*)]
-    example: ""
-    instead: |
-      """This module has a docstring."""
-'''
-
-TESTS_SETTINGS_TEMPLATE = """
-  tests_only: &tests_only !settings
-    included:
-      {test_dirs}
-    excluded: 
-      - ~+/.tox/*
-    allow_ignore: yes
-
-  excluding_tests: &excluding_tests !settings
-    included:
-      - ~+/*
-    excluded:
-      {test_dirs}
-      - ~+/.tox/*
-    allow_ignore: yes
-"""
-
-
-def generate_config(test_directories):
-    """Generate configuration, given test directories."""
-    test_dirs_block = '\n      '.join(
-        "- ~+/{}".format(os.path.join(test_dir, '*'))
-        for test_dir in test_directories
-    )
-    if test_dirs_block:
-        test_settings = TESTS_SETTINGS_TEMPLATE.format(
-            test_dirs=test_dirs_block
-        )
-    else:
-        test_settings = ''
-    config = INIT_TEMPLATE.format(
-        test_block=test_settings,
-        default_settings='excluding_tests' if test_settings else 'all_files'
-    )
-    return config
+"""Initialization of new bellybutton configuration files."""
+
+import os
+
+
+INIT_TEMPLATE = '''settings:
+  all_files: &all_files !settings
+    included:
+      - ~+/*
+    excluded:
+      - ~+/.tox/*
+    allow_ignore: yes
+{test_block}
+default_settings: *{default_settings}
+
+rules:
+  ExampleRule:
+    description: "Empty module."
+    expr: /Module/body[not(./*)]
+    example: ""
+    instead: |
+      """This module has a docstring."""
+'''
+
+TESTS_SETTINGS_TEMPLATE = """
+  tests_only: &tests_only !settings
+    included:
+      {test_dirs}
+    excluded: 
+      - ~+/.tox/*
+    allow_ignore: yes
+
+  excluding_tests: &excluding_tests !settings
+    included:
+      - ~+/*
+    excluded:
+      {test_dirs}
+      - ~+/.tox/*
+    allow_ignore: yes
+"""
+
+
+def generate_config(test_directories):
+    """Generate configuration, given test directories."""
+    test_dirs_block = '\n      '.join(
+        "- ~+/{}".format(os.path.join(test_dir, '*'))
+        for test_dir in test_directories
+    )
+    if test_dirs_block:
+        test_settings = TESTS_SETTINGS_TEMPLATE.format(
+            test_dirs=test_dirs_block
+        )
+    else:
+        test_settings = ''
+    config = INIT_TEMPLATE.format(
+        test_block=test_settings,
+        default_settings='excluding_tests' if test_settings else 'all_files'
+    )
+    return config
```

### Comparing `bellybutton-0.3.1/bellybutton/linting.py` & `bellybutton-0.3.2/bellybutton/linting.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-"""Linting engine."""
-
-import re
-import fnmatch
-import tokenize
-from collections import namedtuple
-from operator import attrgetter
-
-from astpath import find_in_ast, file_contents_to_xml_ast
-from lxml.etree import XPath
-
-try:
-    from re import Pattern as pattern_type
-except ImportError:
-    from re import _pattern_type as pattern_type
-
-LintingResult = namedtuple('LintingResult', 'rule filepath succeeded lineno')
-
-
-def get_ignored_lines(file_contents):
-    """Return set of line numbers to be ignored when linting."""
-    it = iter(file_contents.splitlines(True))
-    tokens = tokenize.generate_tokens(lambda: next(it))
-    return frozenset(
-        line
-        for token_type, token, (line, _), _, _ in tokens
-        if token_type is tokenize.COMMENT
-        if re.search(r'bb:\s?ignore', token)
-    )
-
-
-def rule_settings_match(rule, filepath):
-    """Return whether rule should be executed on file."""
-    should_be_included = any(
-        fnmatch.fnmatch(filepath, included_pattern)
-        for included_pattern in rule.settings.included
-    )
-    should_be_excluded = any(
-        fnmatch.fnmatch(filepath, excluded_pattern)
-        for excluded_pattern in rule.settings.excluded
-    )
-    return should_be_included and not should_be_excluded
-
-
-def lint_file(filepath, file_contents, rules):
-    """Run rules against file, yielding any failures."""
-    matching_rules = [
-        rule
-        for rule in rules
-        if rule_settings_match(rule, filepath)
-    ]
-    if not matching_rules:
-        return
-
-    ignored_lines = get_ignored_lines(file_contents)
-    xml_ast = file_contents_to_xml_ast(file_contents)  # todo - use caching module?
-
-    for rule in sorted(matching_rules, key=attrgetter('name')):
-        # TODO - hacky - need to find better way to do this (while keeping chain)
-        # TODO - possibly having both filepath and contents/input supplied?
-        if isinstance(rule.expr, XPath):
-            matching_lines = set(find_in_ast(
-                xml_ast,
-                rule.expr.path,
-                return_lines=True
-            ))
-        elif isinstance(rule.expr, pattern_type):
-            matching_lines = {
-                file_contents[:match.start()].count('\n') + 1  # TODO - slow
-                for match in re.finditer(rule.expr, file_contents)
-            }
-        elif callable(rule.expr):
-            matching_lines = set(rule.expr(file_contents))
-        else:
-            continue  # todo - maybe throw here?
-
-        if rule.settings.allow_ignore:
-            matching_lines -= ignored_lines
-
-        if not matching_lines:
-            yield LintingResult(rule, filepath, succeeded=True, lineno=None)
-
-        for line in matching_lines:
-            yield LintingResult(rule, filepath, succeeded=False, lineno=line)
+"""Linting engine."""
+
+import re
+import fnmatch
+import tokenize
+from collections import namedtuple
+from operator import attrgetter
+
+from astpath import find_in_ast, file_contents_to_xml_ast
+from lxml.etree import XPath
+
+try:
+    from re import Pattern as pattern_type
+except ImportError:
+    from re import _pattern_type as pattern_type
+
+LintingResult = namedtuple('LintingResult', 'rule filepath succeeded lineno')
+
+
+def get_ignored_lines(file_contents):
+    """Return set of line numbers to be ignored when linting."""
+    it = iter(file_contents.splitlines(True))
+    tokens = tokenize.generate_tokens(lambda: next(it))
+    return frozenset(
+        line
+        for token_type, token, (line, _), _, _ in tokens
+        if token_type is tokenize.COMMENT
+        if re.search(r'bb:\s?ignore', token)
+    )
+
+
+def rule_settings_match(rule, filepath):
+    """Return whether rule should be executed on file."""
+    should_be_included = any(
+        fnmatch.fnmatch(filepath, included_pattern)
+        for included_pattern in rule.settings.included
+    )
+    should_be_excluded = any(
+        fnmatch.fnmatch(filepath, excluded_pattern)
+        for excluded_pattern in rule.settings.excluded
+    )
+    return should_be_included and not should_be_excluded
+
+
+def lint_file(filepath, file_contents, rules):
+    """Run rules against file, yielding any failures."""
+    matching_rules = [
+        rule
+        for rule in rules
+        if rule_settings_match(rule, filepath)
+    ]
+    if not matching_rules:
+        return
+
+    ignored_lines = get_ignored_lines(file_contents)
+    xml_ast = file_contents_to_xml_ast(file_contents)  # todo - use caching module?
+
+    for rule in sorted(matching_rules, key=attrgetter('name')):
+        # TODO - hacky - need to find better way to do this (while keeping chain)
+        # TODO - possibly having both filepath and contents/input supplied?
+        if isinstance(rule.expr, XPath):
+            matching_lines = set(find_in_ast(
+                xml_ast,
+                rule.expr.path,
+                return_lines=True
+            ))
+        elif isinstance(rule.expr, pattern_type):
+            matching_lines = {
+                file_contents[:match.start()].count('\n') + 1  # TODO - slow
+                for match in re.finditer(rule.expr, file_contents)
+            }
+        elif callable(rule.expr):
+            matching_lines = set(rule.expr(file_contents))
+        else:
+            continue  # todo - maybe throw here?
+
+        if rule.settings.allow_ignore:
+            matching_lines -= ignored_lines
+
+        if not matching_lines:
+            yield LintingResult(rule, filepath, succeeded=True, lineno=None)
+
+        for line in matching_lines:
+            yield LintingResult(rule, filepath, succeeded=False, lineno=line)
```

### Comparing `bellybutton-0.3.1/setup.py` & `bellybutton-0.3.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from setuptools import setup
-
-setup(
-    name='bellybutton',
-    packages=['bellybutton'],
-    platforms='any',
-    version='0.3.1',
-    description='Custom Python linting through AST expressions.',
-    author='H. Chase Stevens',
-    author_email='chase@chasestevens.com',
-    url='https://github.com/hchasestevens/bellybutton',
-    license='MIT',
-    install_requires=[
-        'astpath[xpath]==0.6.1',
-        'pyyaml>=4.0,<6.0',
-        'lxml>=4.1.1',
-    ],
-    tests_require=['pytest>=3.1.2', 'future>=0.16.0'],
-    extras_require={'dev': ['pytest==3.1.2', 'future>=0.16.0']},
-    entry_points={
-        'console_scripts': [
-            'bellybutton = bellybutton.cli:main',
-        ],
-    },
-    classifiers=[
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Intended Audience :: Developers',
-        'Operating System :: OS Independent',
-        'License :: OSI Approved :: MIT License',
-    ]
-)
+from setuptools import setup
+
+setup(
+    name='bellybutton',
+    packages=['bellybutton'],
+    platforms='any',
+    version='0.3.2',
+    description='Custom Python linting through AST expressions.',
+    author='H. Chase Stevens',
+    author_email='chase@chasestevens.com',
+    url='https://github.com/hchasestevens/bellybutton',
+    license='MIT',
+    install_requires=[
+        'astpath[xpath]==0.6.1',
+        'pyyaml>=4.0,<7.0',
+        'lxml>=4.1.1',
+    ],
+    tests_require=['pytest>=3.1.2', 'future>=0.16.0'],
+    extras_require={'dev': ['pytest==3.1.2', 'future>=0.16.0']},
+    entry_points={
+        'console_scripts': [
+            'bellybutton = bellybutton.cli:main',
+        ],
+    },
+    classifiers=[
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 2',
+        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Intended Audience :: Developers',
+        'Operating System :: OS Independent',
+        'License :: OSI Approved :: MIT License',
+    ]
+)
```

### Comparing `bellybutton-0.3.1/README.md` & `bellybutton-0.3.2/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-# bellybutton
-
-[![Build Status](https://travis-ci.org/hchasestevens/bellybutton.svg?branch=master)](https://travis-ci.org/hchasestevens/bellybutton) [![PyPI version](https://badge.fury.io/py/bellybutton.svg)](https://badge.fury.io/py/bellybutton) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bellybutton.svg)
-
-<img src="demo.gif" width="642">
-
-`bellybutton` is a customizable, easy-to-configure linting engine for Python. 
-
-## What is this good for?
-
-Tools like [pylint](https://www.pylint.org/) and [flake8](http://flake8.pycqa.org/en/latest/#) provide, 
-out-of-the-box, a wide variety of rules for enforcing Python best practices, ensuring PEP-8 compliance, 
-and avoiding frequent sources of bugs. However, many projects have project-specific candidates for 
-static analysis, such as internal style guides, areas of deprecated functionality, or common sources 
-of error. This is especially true of those projects with many contributors or with large or legacy 
-codebases.
-
-`bellybutton` allows custom linting rules to be specified on a per-project basis and detected as part of
-your normal build, test and deployment process and, further, makes specifying these rules highly 
-accessible, greatly lowering the cost of adoption.
-
-Give `bellybutton` a try if:
-* You find yourself making the same PR comments over and over again
-* You need a means of gradually deprecating legacy functionality
-* You're looking to build a self-enforcing style guide
-* Your project needs to onboard new or junior developers more quickly and effectively
-* You have Python nitpicks that go beyond what standard linting tools enforce
-
-## Installation & getting started 
-
-`bellybutton` can be installed via:
-```bash
-pip install bellybutton
-```
-
-Once installed, running
-```bash
-bellybutton init
-```
-in your project's root directory will create a `.bellybutton.yml` configuration file with an example 
-rule for you to begin adapting. `bellybutton` will also try to provide additional rule settings based
-on the directory structure of your project.
-
-Once you have configured `bellybutton` for your project, running 
-```bash
-bellybutton lint
-```
-will lint the project against the rules specified in your `.bellybutton.yml`. Additionally, running
-```bash
-bellybutton lint --modified-only
-```
-will, if using git, only lint those files that differ from `origin/master`.
-
-For adding `bellybutton` to your CI pipeline, take a look at this repository's [tox configuration](tox.ini)
-and [.travis.yml](.travis.yml) as an example.
-
-## Concepts
-
-### Rules
-
-Rules in `bellybutton` supply patterns that should be caught and cause linting to fail. Rules as specified
-in your `.bellybutton.yml` configuration must consist of:
-* A description `description`, expressing the meaning of the rule
-* An expression `expr`, specifying the pattern to be caught - either as an 
-[astpath](https://github.com/hchasestevens/astpath) expression or as a regular expression (`!regex ...`).
-
-Additionally, the key used for the rule within the `rules` mapping serves as its name.
-
-Rules may also consist of:
-* Settings `settings` that specify on which files the rule is to be enforced, as well as whether it can be
-ignored via a `# bb: ignore` comment
-* An example `example` of Python code that would be matched by the rule
-* A counter-example `instead` of an alternative piece of code, for guiding the developer in fixing their
-linting error.
-
-These `example` and `instead` clauses are checked at run-time to ensure that they respectively are and are not
-matched by the rule's `expr`.
-
-As an example, a rule to lint for a deprecated function call using an [astpath](https://github.com/hchasestevens/astpath) expression might look like:
-```yaml
-DeprecatedFnCall:
-  description: `deprecated_fn` will be deprecated in v9.1.2. Please use `new_fn` instead.
-  expr: //Call[func/Name/@id='deprecated_fn']
-  example: "deprecated_fn(*values)"
-  instead: "new_fn(values)"
-```
-
-### Settings
-
-`!settings` nodes specify:
-* `included` paths on which rules are to be run, using [glob notation](https://docs.python.org/3.6/library/glob.html)
-* `excluded` paths on which rules are not to be run (even when matching the `included` paths)
-* A boolean `allow_ignore` which determines whether rules can be ignored, providing the line matching the
-rule has a `# bb: ignore` comment.
-
-Additionally, at the root level of `.bellybutton.yml`, a `default_settings` setting may be specified which
-will be used by rules without explicit settings. Each rule must either have a `settings` parameter or be
-able to fall back on the `default_settings`.
-
-As an example, a `!settings` node to lint only a specific module might look like:
-```yaml
-my_module_settings: !settings
-  included:
-    - ~+/my_package/my_module.py
-  excluded: []
-  allow_ignore: no
-```
-
-## Example usage
-
-Check out this repository's [`.bellybutton.yml`](.bellybutton.yml) as an example `bellybutton` configuration file, 
-and [`astpath`'s README](https://github.com/hchasestevens/astpath/blob/master/README.md) for examples of the types 
-of patterns you can lint for using `bellybutton`.
-
-## Development status
-
-`bellybutton` is in an alpha release and, as such, is missing some key features, documentation, 
-and full test coverage. Further, `bellybutton` is not optimized for performance on extremely large 
-codebases and may contain breaking bugs. Please report any bugs encountered.
-
-### Known issues:
-* The `!chain` and `!verbal` expression nodes are not yet implemented
-
-## Contacts
-
-* Name: [H. Chase Stevens](http://www.chasestevens.com)
-* Twitter: [@hchasestevens](https://twitter.com/hchasestevens)
+# bellybutton
+
+[![Build Status](https://travis-ci.org/hchasestevens/bellybutton.svg?branch=master)](https://travis-ci.org/hchasestevens/bellybutton) [![PyPI version](https://badge.fury.io/py/bellybutton.svg)](https://badge.fury.io/py/bellybutton) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bellybutton.svg)
+
+<img src="demo.gif" width="642">
+
+`bellybutton` is a customizable, easy-to-configure linting engine for Python. 
+
+## What is this good for?
+
+Tools like [pylint](https://www.pylint.org/) and [flake8](http://flake8.pycqa.org/en/latest/#) provide, 
+out-of-the-box, a wide variety of rules for enforcing Python best practices, ensuring PEP-8 compliance, 
+and avoiding frequent sources of bugs. However, many projects have project-specific candidates for 
+static analysis, such as internal style guides, areas of deprecated functionality, or common sources 
+of error. This is especially true of those projects with many contributors or with large or legacy 
+codebases.
+
+`bellybutton` allows custom linting rules to be specified on a per-project basis and detected as part of
+your normal build, test and deployment process and, further, makes specifying these rules highly 
+accessible, greatly lowering the cost of adoption.
+
+Give `bellybutton` a try if:
+* You find yourself making the same PR comments over and over again
+* You need a means of gradually deprecating legacy functionality
+* You're looking to build a self-enforcing style guide
+* Your project needs to onboard new or junior developers more quickly and effectively
+* You have Python nitpicks that go beyond what standard linting tools enforce
+
+## Installation & getting started 
+
+`bellybutton` can be installed via:
+```bash
+pip install bellybutton
+```
+
+Once installed, running
+```bash
+bellybutton init
+```
+in your project's root directory will create a `.bellybutton.yml` configuration file with an example 
+rule for you to begin adapting. `bellybutton` will also try to provide additional rule settings based
+on the directory structure of your project.
+
+Once you have configured `bellybutton` for your project, running 
+```bash
+bellybutton lint
+```
+will lint the project against the rules specified in your `.bellybutton.yml`. Additionally, running
+```bash
+bellybutton lint --modified-only
+```
+will, if using git, only lint those files that differ from `origin/master`.
+
+For adding `bellybutton` to your CI pipeline, take a look at this repository's [tox configuration](tox.ini)
+and [.travis.yml](.travis.yml) as an example.
+
+## Concepts
+
+### Rules
+
+Rules in `bellybutton` supply patterns that should be caught and cause linting to fail. Rules as specified
+in your `.bellybutton.yml` configuration must consist of:
+* A description `description`, expressing the meaning of the rule
+* An expression `expr`, specifying the pattern to be caught - either as an 
+[astpath](https://github.com/hchasestevens/astpath) expression or as a regular expression (`!regex ...`).
+
+Additionally, the key used for the rule within the `rules` mapping serves as its name.
+
+Rules may also consist of:
+* Settings `settings` that specify on which files the rule is to be enforced, as well as whether it can be
+ignored via a `# bb: ignore` comment
+* An example `example` of Python code that would be matched by the rule
+* A counter-example `instead` of an alternative piece of code, for guiding the developer in fixing their
+linting error.
+
+These `example` and `instead` clauses are checked at run-time to ensure that they respectively are and are not
+matched by the rule's `expr`.
+
+As an example, a rule to lint for a deprecated function call using an [astpath](https://github.com/hchasestevens/astpath) expression might look like:
+```yaml
+DeprecatedFnCall:
+  description: `deprecated_fn` will be deprecated in v9.1.2. Please use `new_fn` instead.
+  expr: //Call[func/Name/@id='deprecated_fn']
+  example: "deprecated_fn(*values)"
+  instead: "new_fn(values)"
+```
+
+### Settings
+
+`!settings` nodes specify:
+* `included` paths on which rules are to be run, using [glob notation](https://docs.python.org/3.6/library/glob.html)
+* `excluded` paths on which rules are not to be run (even when matching the `included` paths)
+* A boolean `allow_ignore` which determines whether rules can be ignored, providing the line matching the
+rule has a `# bb: ignore` comment.
+
+Additionally, at the root level of `.bellybutton.yml`, a `default_settings` setting may be specified which
+will be used by rules without explicit settings. Each rule must either have a `settings` parameter or be
+able to fall back on the `default_settings`.
+
+As an example, a `!settings` node to lint only a specific module might look like:
+```yaml
+my_module_settings: !settings
+  included:
+    - ~+/my_package/my_module.py
+  excluded: []
+  allow_ignore: no
+```
+
+## Example usage
+
+Check out this repository's [`.bellybutton.yml`](.bellybutton.yml) as an example `bellybutton` configuration file, 
+and [`astpath`'s README](https://github.com/hchasestevens/astpath/blob/master/README.md) for examples of the types 
+of patterns you can lint for using `bellybutton`.
+
+## Development status
+
+`bellybutton` is in an alpha release and, as such, is missing some key features, documentation, 
+and full test coverage. Further, `bellybutton` is not optimized for performance on extremely large 
+codebases and may contain breaking bugs. Please report any bugs encountered.
+
+### Known issues:
+* The `!chain` and `!verbal` expression nodes are not yet implemented
+
+## Contacts
+
+* Name: [H. Chase Stevens](http://www.chasestevens.com)
+* Twitter: [@hchasestevens](https://twitter.com/hchasestevens)
```

