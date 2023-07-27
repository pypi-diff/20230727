# Comparing `tmp/pe-0.4.0.tar.gz` & `tmp/pe-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-0.4.0.tar", last modified: Sun Jun  4 20:10:15 2023, max compression
+gzip compressed data, was "pe-0.5.0.tar", last modified: Thu Jul 27 04:58:28 2023, max compression
```

## Comparing `pe-0.4.0.tar` & `pe-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:10:15.158856 pe-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-04 20:10:06.000000 pe-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-06-04 20:10:15.158856 pe-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-04 20:10:06.000000 pe-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:10:15.154855 pe-0.4.0/pe/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-04 20:10:06.000000 pe-0.4.0/pe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)  1115685 2023-06-04 20:10:14.000000 pe-0.4.0/pe/_cy_machine.c
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_cy_machine.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_py_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-04 20:10:06.000000 pe-0.4.0/pe/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-04 20:10:06.000000 pe-0.4.0/pe/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-04 20:10:06.000000 pe-0.4.0/pe/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-04 20:10:06.000000 pe-0.4.0/pe/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-06-04 20:10:06.000000 pe-0.4.0/pe/packrat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:10:15.154855 pe-0.4.0/pe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-06-04 20:10:15.000000 pe-0.4.0/pe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-04 20:10:15.000000 pe-0.4.0/pe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:10:15.000000 pe-0.4.0/pe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:10:15.000000 pe-0.4.0/pe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-04 20:10:15.000000 pe-0.4.0/pe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 20:10:06.000000 pe-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-04 20:10:15.158856 pe-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-06-04 20:10:06.000000 pe-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:10:15.158856 pe-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-04 20:10:06.000000 pe-0.4.0/test/test__definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-04 20:10:06.000000 pe-0.4.0/test/test__match.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-04 20:10:06.000000 pe-0.4.0/test/test__optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-04 20:10:06.000000 pe-0.4.0/test/test__parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-04 20:10:06.000000 pe-0.4.0/test/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-04 20:10:06.000000 pe-0.4.0/test/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-04 20:10:06.000000 pe-0.4.0/test/test_pe.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-04 20:10:06.000000 pe-0.4.0/test/test_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:58:28.518116 pe-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-27 04:58:21.000000 pe-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-07-27 04:58:28.518116 pe-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-27 04:58:21.000000 pe-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:58:28.514116 pe-0.5.0/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 04:58:21.000000 pe-0.5.0/pe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_autoignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1125436 2023-07-27 04:58:28.000000 pe-0.5.0/pe/_cy_machine.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_cy_machine.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_disarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14016 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_py_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-27 04:58:21.000000 pe-0.5.0/pe/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-27 04:58:21.000000 pe-0.5.0/pe/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-27 04:58:21.000000 pe-0.5.0/pe/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-27 04:58:21.000000 pe-0.5.0/pe/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-07-27 04:58:21.000000 pe-0.5.0/pe/packrat.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 04:58:21.000000 pe-0.5.0/pe/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:58:28.518116 pe-0.5.0/pe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-07-27 04:58:28.000000 pe-0.5.0/pe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-27 04:58:28.000000 pe-0.5.0/pe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 04:58:28.000000 pe-0.5.0/pe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 04:58:28.000000 pe-0.5.0/pe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-27 04:58:28.000000 pe-0.5.0/pe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-27 04:58:21.000000 pe-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-27 04:58:28.522116 pe-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-07-27 04:58:21.000000 pe-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 04:58:28.518116 pe-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-27 04:58:21.000000 pe-0.5.0/test/test__definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-27 04:58:21.000000 pe-0.5.0/test/test__disarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-27 04:58:21.000000 pe-0.5.0/test/test__match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-27 04:58:21.000000 pe-0.5.0/test/test__optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-27 04:58:21.000000 pe-0.5.0/test/test__parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-27 04:58:21.000000 pe-0.5.0/test/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-27 04:58:21.000000 pe-0.5.0/test/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-27 04:58:21.000000 pe-0.5.0/test/test_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-27 04:58:21.000000 pe-0.5.0/test/test_regression.py
```

### Comparing `pe-0.4.0/LICENSE` & `pe-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/PKG-INFO` & `pe-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library for Parsing Expression Grammars (PEG)
 Home-page: https://github.com/goodmami/pe/
 Author: Michael Wayne Goodman
 Author-email: goodman.m.w@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/goodmami/pe/blob/main/docs/README.md
 Project-URL: Changelog, https://github.com/goodmami/pe/blob/main/CHANGELOG.md
@@ -131,14 +131,17 @@
 
 # (extension) binding
 name:e       # bind result of e to 'name'
 
 # grammars
 Name <- ...  # define a rule named 'Name'
 ... <- Name  # refer to rule named 'Name'
+
+# (extension) auto-ignore
+X <  e1 e2   # define a rule 'X' with auto-ignore
 ```
 
 ## Matching Inputs with Parsing Expressions
 
 When a parsing expression matches an input, it returns a `Match`
 object, which is similar to those of Python's
 [re](https://docs.python.org/3/library/re.html) module for regular
@@ -209,29 +212,43 @@
 func(sep.join(match.groups()), **match.groupdict())
 ```
 
 [Action]: docs/api/pe.actions.md#Action
 [Pack]: docs/api/pe.actions.md#Pack
 [Join]: docs/api/pe.actions.md#Join
 
+### Auto-ignore
+
+The grammar can be defined such that some rules ignore occurrences of
+a pattern between sequence items. Most commonly, this is used to
+ignore whitespace, so the default ignore pattern is simple whitespace.
+
+```python
+>>> pe.match("X <- 'a' 'b'", "a b")  # regular rule does not match
+>>> pe.match("X <  'a' 'b'", "a b")  # auto-ignore rule matches
+<Match object; span=(0, 3), match='a b'>
+
+```
+
+This feature can help to make grammars more readable.
 
 ### Example
 
 Here is one way to parse a list of comma-separated integers:
 
 ```python
 >>> from pe.actions import Pack
 >>> p = pe.compile(
 ...   r'''
 ...     Start  <- "[" Values? "]"
 ...     Values <- Int ("," Int)*
-...     Int    <- ~( "-"? ("0" / [1-9] [0-9]*) )
+...     Int    <  ~( "-"? ("0" / [1-9] [0-9]*) )
 ...   ''',
 ...   actions={'Values': Pack(list), 'Int': int})
->>> m = p.match('[5,10,-15]')
+>>> m = p.match('[5, 10, -15]')
 >>> m.value()
 [5, 10, -15]
 
 ```
 
 ## Similar Projects
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pe Version: 0.4.0 Summary: Library for Parsing
+Metadata-Version: 2.1 Name: pe Version: 0.5.0 Summary: Library for Parsing
 Expression Grammars (PEG) Home-page: https://github.com/goodmami/pe/ Author:
 Michael Wayne Goodman Author-email: goodman.m.w@gmail.com License: MIT Project-
 URL: Documentation, https://github.com/goodmami/pe/blob/main/docs/README.md
 Project-URL: Changelog, https://github.com/goodmami/pe/blob/main/CHANGELOG.md
 Keywords: peg,parsing,text Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
@@ -48,15 +48,16 @@
 terminals . # any single character "abc" # string literal 'abc' # string
 literal [abc] # character class # repeating expressions e # exactly one e? #
 zero or one (optional) e* # zero or more e+ # one or more # combining
 expressions e1 e2 # sequence of e1 and e2 e1 / e2 # ordered choice of e1 and e2
 (e) # subexpression # lookahead &e # positive lookahead !e # negative lookahead
 # (extension) capture substring ~e # result of e is matched substring #
 (extension) binding name:e # bind result of e to 'name' # grammars Name <- ...
-# define a rule named 'Name' ... <- Name # refer to rule named 'Name' ``` ##
+# define a rule named 'Name' ... <- Name # refer to rule named 'Name' #
+(extension) auto-ignore X < e1 e2 # define a rule 'X' with auto-ignore ``` ##
 Matching Inputs with Parsing Expressions When a parsing expression matches an
 input, it returns a `Match` object, which is similar to those of Python's [re]
 (https://docs.python.org/3/library/re.html) module for regular expressions. By
 default, nothing is captured, but the capture operator (`~`) emits the
 substring of the matching expression, similar to regular expression's capturing
 groups: ```python >>> e = pe.compile(r'[0-9] [.] [0-9]') >>> m = e.match('1.4')
 >>> m.group() '1.4' >>> m.groups() () >>> e = pe.compile(r'~([0-9] [.] [0-9])')
@@ -74,20 +75,26 @@
 are cleared. For more control, **pe** provides the [Action] class and a number
 of subclasses for various use-cases. These actions have access to more
 information about a parse result and more control over the match. For example,
 the [Pack] class takes a function and calls it with the emitted values packed
 into a list: ``` python func(match.groups()) ``` And the [Join] class joins all
 emitted strings with a separator: ``` python func(sep.join(match.groups()),
 **match.groupdict()) ``` [Action]: docs/api/pe.actions.md#Action [Pack]: docs/
-api/pe.actions.md#Pack [Join]: docs/api/pe.actions.md#Join ### Example Here is
-one way to parse a list of comma-separated integers: ```python >>> from
-pe.actions import Pack >>> p = pe.compile( ... r''' ... Start <- "[" Values?
-"]" ... Values <- Int ("," Int)* ... Int <- ~( "-"? ("0" / [1-9] [0-9]*) ) ...
-''', ... actions={'Values': Pack(list), 'Int': int}) >>> m = p.match('[5,10,-
-15]') >>> m.value() [5, 10, -15] ``` ## Similar Projects - [Lark](https://
-github.com/lark-parser/lark) (Python) - [nom](https://github.com/Geal/nom)
-(Rust) - [Parsimonious](https://github.com/erikrose/parsimonious) (Python) -
-[Rosie](https://rosie-lang.org/) (Multiple bindings) - [TatSu](https://
-tatsu.readthedocs.io/en/stable/) (Python) - [PEG.js](https://github.com/pegjs/
-pegjs) (Javascript) - [Pegged](https://github.com/PhilippeSigaud/Pegged) (D) -
-[pegen](https://github.com/gvanrossum/pegen) (Python / C) - [LPeg] (Lua)
-[LPeg]: http://www.inf.puc-rio.br/~roberto/lpeg/
+api/pe.actions.md#Pack [Join]: docs/api/pe.actions.md#Join ### Auto-ignore The
+grammar can be defined such that some rules ignore occurrences of a pattern
+between sequence items. Most commonly, this is used to ignore whitespace, so
+the default ignore pattern is simple whitespace. ```python >>> pe.match("X <-
+'a' 'b'", "a b") # regular rule does not match >>> pe.match("X < 'a' 'b'", "a
+b") # auto-ignore rule matches
+ span=(0, 3), match='a b'> ``` This feature can help to make grammars more
+readable. ### Example Here is one way to parse a list of comma-separated
+integers: ```python >>> from pe.actions import Pack >>> p = pe.compile( ...
+r''' ... Start <- "[" Values? "]" ... Values <- Int ("," Int)* ... Int < ~( "-
+"? ("0" / [1-9] [0-9]*) ) ... ''', ... actions={'Values': Pack(list), 'Int':
+int}) >>> m = p.match('[5, 10, -15]') >>> m.value() [5, 10, -15] ``` ## Similar
+Projects - [Lark](https://github.com/lark-parser/lark) (Python) - [nom](https:/
+/github.com/Geal/nom) (Rust) - [Parsimonious](https://github.com/erikrose/
+parsimonious) (Python) - [Rosie](https://rosie-lang.org/) (Multiple bindings) -
+[TatSu](https://tatsu.readthedocs.io/en/stable/) (Python) - [PEG.js](https://
+github.com/pegjs/pegjs) (Javascript) - [Pegged](https://github.com/
+PhilippeSigaud/Pegged) (D) - [pegen](https://github.com/gvanrossum/pegen)
+(Python / C) - [LPeg] (Lua) [LPeg]: http://www.inf.puc-rio.br/~roberto/lpeg/
```

### Comparing `pe-0.4.0/README.md` & `pe-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,17 @@
 
 # (extension) binding
 name:e       # bind result of e to 'name'
 
 # grammars
 Name <- ...  # define a rule named 'Name'
 ... <- Name  # refer to rule named 'Name'
+
+# (extension) auto-ignore
+X <  e1 e2   # define a rule 'X' with auto-ignore
 ```
 
 ## Matching Inputs with Parsing Expressions
 
 When a parsing expression matches an input, it returns a `Match`
 object, which is similar to those of Python's
 [re](https://docs.python.org/3/library/re.html) module for regular
@@ -180,29 +183,43 @@
 func(sep.join(match.groups()), **match.groupdict())
 ```
 
 [Action]: docs/api/pe.actions.md#Action
 [Pack]: docs/api/pe.actions.md#Pack
 [Join]: docs/api/pe.actions.md#Join
 
+### Auto-ignore
+
+The grammar can be defined such that some rules ignore occurrences of
+a pattern between sequence items. Most commonly, this is used to
+ignore whitespace, so the default ignore pattern is simple whitespace.
+
+```python
+>>> pe.match("X <- 'a' 'b'", "a b")  # regular rule does not match
+>>> pe.match("X <  'a' 'b'", "a b")  # auto-ignore rule matches
+<Match object; span=(0, 3), match='a b'>
+
+```
+
+This feature can help to make grammars more readable.
 
 ### Example
 
 Here is one way to parse a list of comma-separated integers:
 
 ```python
 >>> from pe.actions import Pack
 >>> p = pe.compile(
 ...   r'''
 ...     Start  <- "[" Values? "]"
 ...     Values <- Int ("," Int)*
-...     Int    <- ~( "-"? ("0" / [1-9] [0-9]*) )
+...     Int    <  ~( "-"? ("0" / [1-9] [0-9]*) )
 ...   ''',
 ...   actions={'Values': Pack(list), 'Int': int})
->>> m = p.match('[5,10,-15]')
+>>> m = p.match('[5, 10, -15]')
 >>> m.value()
 [5, 10, -15]
 
 ```
 
 ## Similar Projects
```

#### html2text {}

```diff
@@ -32,15 +32,16 @@
 terminals . # any single character "abc" # string literal 'abc' # string
 literal [abc] # character class # repeating expressions e # exactly one e? #
 zero or one (optional) e* # zero or more e+ # one or more # combining
 expressions e1 e2 # sequence of e1 and e2 e1 / e2 # ordered choice of e1 and e2
 (e) # subexpression # lookahead &e # positive lookahead !e # negative lookahead
 # (extension) capture substring ~e # result of e is matched substring #
 (extension) binding name:e # bind result of e to 'name' # grammars Name <- ...
-# define a rule named 'Name' ... <- Name # refer to rule named 'Name' ``` ##
+# define a rule named 'Name' ... <- Name # refer to rule named 'Name' #
+(extension) auto-ignore X < e1 e2 # define a rule 'X' with auto-ignore ``` ##
 Matching Inputs with Parsing Expressions When a parsing expression matches an
 input, it returns a `Match` object, which is similar to those of Python's [re]
 (https://docs.python.org/3/library/re.html) module for regular expressions. By
 default, nothing is captured, but the capture operator (`~`) emits the
 substring of the matching expression, similar to regular expression's capturing
 groups: ```python >>> e = pe.compile(r'[0-9] [.] [0-9]') >>> m = e.match('1.4')
 >>> m.group() '1.4' >>> m.groups() () >>> e = pe.compile(r'~([0-9] [.] [0-9])')
@@ -58,20 +59,26 @@
 are cleared. For more control, **pe** provides the [Action] class and a number
 of subclasses for various use-cases. These actions have access to more
 information about a parse result and more control over the match. For example,
 the [Pack] class takes a function and calls it with the emitted values packed
 into a list: ``` python func(match.groups()) ``` And the [Join] class joins all
 emitted strings with a separator: ``` python func(sep.join(match.groups()),
 **match.groupdict()) ``` [Action]: docs/api/pe.actions.md#Action [Pack]: docs/
-api/pe.actions.md#Pack [Join]: docs/api/pe.actions.md#Join ### Example Here is
-one way to parse a list of comma-separated integers: ```python >>> from
-pe.actions import Pack >>> p = pe.compile( ... r''' ... Start <- "[" Values?
-"]" ... Values <- Int ("," Int)* ... Int <- ~( "-"? ("0" / [1-9] [0-9]*) ) ...
-''', ... actions={'Values': Pack(list), 'Int': int}) >>> m = p.match('[5,10,-
-15]') >>> m.value() [5, 10, -15] ``` ## Similar Projects - [Lark](https://
-github.com/lark-parser/lark) (Python) - [nom](https://github.com/Geal/nom)
-(Rust) - [Parsimonious](https://github.com/erikrose/parsimonious) (Python) -
-[Rosie](https://rosie-lang.org/) (Multiple bindings) - [TatSu](https://
-tatsu.readthedocs.io/en/stable/) (Python) - [PEG.js](https://github.com/pegjs/
-pegjs) (Javascript) - [Pegged](https://github.com/PhilippeSigaud/Pegged) (D) -
-[pegen](https://github.com/gvanrossum/pegen) (Python / C) - [LPeg] (Lua)
-[LPeg]: http://www.inf.puc-rio.br/~roberto/lpeg/
+api/pe.actions.md#Pack [Join]: docs/api/pe.actions.md#Join ### Auto-ignore The
+grammar can be defined such that some rules ignore occurrences of a pattern
+between sequence items. Most commonly, this is used to ignore whitespace, so
+the default ignore pattern is simple whitespace. ```python >>> pe.match("X <-
+'a' 'b'", "a b") # regular rule does not match >>> pe.match("X < 'a' 'b'", "a
+b") # auto-ignore rule matches
+ span=(0, 3), match='a b'> ``` This feature can help to make grammars more
+readable. ### Example Here is one way to parse a list of comma-separated
+integers: ```python >>> from pe.actions import Pack >>> p = pe.compile( ...
+r''' ... Start <- "[" Values? "]" ... Values <- Int ("," Int)* ... Int < ~( "-
+"? ("0" / [1-9] [0-9]*) ) ... ''', ... actions={'Values': Pack(list), 'Int':
+int}) >>> m = p.match('[5, 10, -15]') >>> m.value() [5, 10, -15] ``` ## Similar
+Projects - [Lark](https://github.com/lark-parser/lark) (Python) - [nom](https:/
+/github.com/Geal/nom) (Rust) - [Parsimonious](https://github.com/erikrose/
+parsimonious) (Python) - [Rosie](https://rosie-lang.org/) (Multiple bindings) -
+[TatSu](https://tatsu.readthedocs.io/en/stable/) (Python) - [PEG.js](https://
+github.com/pegjs/pegjs) (Javascript) - [Pegged](https://github.com/
+PhilippeSigaud/Pegged) (D) - [pegen](https://github.com/gvanrossum/pegen)
+(Python / C) - [LPeg] (Lua) [LPeg]: http://www.inf.puc-rio.br/~roberto/lpeg/
```

### Comparing `pe-0.4.0/pe/__init__.py` & `pe-0.5.0/pe/__init__.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/pe/_constants.py` & `pe-0.5.0/pe/_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,32 @@
     OPT = (_auto(), 5, 'Quantified')   # (OPT, (expr,))
     STR = (_auto(), 5, 'Quantified')   # (STR, (expr,))
     PLS = (_auto(), 5, 'Quantified')   # (PLS, (expr,))
     AND = (_auto(), 4, 'Valued')       # (AND, (expr,))
     NOT = (_auto(), 4, 'Valued')       # (NOT, (expr,))
     CAP = (_auto(), 4, 'Valued')       # (CAP, (expr,))
     BND = (_auto(), 4, 'Valued')       # (BND, (expr, name))
+    IGN = (_auto(), 4, 'Valued')       # (IGN, (expr,))
     SEQ = (_auto(), 3, 'Sequential')   # (SEQ, (exprs,))
     RUL = (_auto(), 2, 'Applicative')  # (RUL, (expr, action, name))
     CHC = (_auto(), 1, 'Prioritized')  # (CHC, (exprs,))
     DEF = (_auto(), 0, 'Definitive')   # (DEF, (expr, name))
     DBG = (_auto(), -1, 'Debug')       # (DBG, (expr,))
 
     @property
     def precedence(self):
         return self.value[1]
 
     @property
     def type(self):
         return self.value[2]
 
+    def is_unary(self):
+        return self.type not in {'Sequential', 'Prioritized'}
+
 
 class Flag(enum.Flag):
     NONE = 0
     DEBUG = _auto()  # print debugging info for compiled expression
     STRICT = _auto()  # raise error on match failure
     MEMOIZE = _auto()  # use a packrat memo
     INLINE = _auto()  # inline non-recursive rules
```

### Comparing `pe-0.4.0/pe/_cy_machine.c` & `pe-0.5.0/pe/_cy_machine.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "pe._cy_machine",
         "sources": [
@@ -18,16 +18,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -94,15 +94,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -378,17 +378,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -458,14 +455,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -985,15 +987,15 @@
 struct __pyx_t_2pe_11_cy_machine_State;
 struct __pyx_opt_args_2pe_11_cy_machine_7Scanner_scan;
 struct __pyx_defaults;
 typedef struct __pyx_defaults __pyx_defaults;
 struct __pyx_defaults1;
 typedef struct __pyx_defaults1 __pyx_defaults1;
 
-/* "pe/_cy_machine.pyx":31
+/* "pe/_cy_machine.pyx":34
  * # Parser ###############################################################
  * 
  * cdef enum OpCode:             # <<<<<<<<<<<<<<
  *     FAIL = -1
  *     PASS = 0
  */
 enum __pyx_t_2pe_11_cy_machine_OpCode {
@@ -1007,15 +1009,15 @@
   __pyx_e_2pe_11_cy_machine_CALL = 6,
   __pyx_e_2pe_11_cy_machine_RETURN = 7,
   __pyx_e_2pe_11_cy_machine_JUMP = 8,
   __pyx_e_2pe_11_cy_machine_SCAN = 9,
   __pyx_e_2pe_11_cy_machine_NOOP = 10
 };
 
-/* "pe/_cy_machine.pyx":46
+/* "pe/_cy_machine.pyx":49
  * 
  * 
  * cdef struct State:             # <<<<<<<<<<<<<<
  *     int opidx
  *     int pos
  */
 struct __pyx_t_2pe_11_cy_machine_State {
@@ -1023,46 +1025,47 @@
   int pos;
   int mark;
   int argidx;
   int kwidx;
   struct __pyx_t_2pe_11_cy_machine_State *prev;
 };
 
-/* "pe/_cy_machine.pyx":88
+/* "pe/_cy_machine.pyx":91
  * 
  * cdef class Scanner:
  *     cpdef int scan(self, str s, int pos=0) except -2:             # <<<<<<<<<<<<<<
  *         try:
  *             return self._scan(s, pos, len(s))
  */
 struct __pyx_opt_args_2pe_11_cy_machine_7Scanner_scan {
   int __pyx_n;
   int pos;
 };
 struct __pyx_defaults {
+  PyObject *__pyx_arg_ignore;
   PyObject *__pyx_arg_flags;
 };
 struct __pyx_defaults1 {
   PyObject *__pyx_arg_flags;
 };
 
-/* "pe/_cy_machine.pyx":87
+/* "pe/_cy_machine.pyx":90
  * 
  * 
  * cdef class Scanner:             # <<<<<<<<<<<<<<
  *     cpdef int scan(self, str s, int pos=0) except -2:
  *         try:
  */
 struct __pyx_obj_2pe_11_cy_machine_Scanner {
   PyObject_HEAD
   struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner *__pyx_vtab;
 };
 
 
-/* "pe/_cy_machine.pyx":98
+/* "pe/_cy_machine.pyx":101
  * 
  * 
  * cdef class Instruction:             # <<<<<<<<<<<<<<
  *     cdef public:
  *         OpCode opcode
  */
 struct __pyx_obj_2pe_11_cy_machine_Instruction {
@@ -1073,55 +1076,55 @@
   int marking;
   int capturing;
   PyObject *action;
   PyObject *name;
 };
 
 
-/* "pe/_cy_machine.pyx":177
+/* "pe/_cy_machine.pyx":183
  * 
  * 
  * cdef class _Parser:             # <<<<<<<<<<<<<<
  *     cdef list pi
  * 
  */
 struct __pyx_obj_2pe_11_cy_machine__Parser {
   PyObject_HEAD
   struct __pyx_vtabstruct_2pe_11_cy_machine__Parser *__pyx_vtab;
   PyObject *pi;
 };
 
 
-/* "pe/_cy_machine.pyx":515
+/* "pe/_cy_machine.pyx":521
  * # Scanners #############################################################
  * 
  * cdef class Dot(Scanner):             # <<<<<<<<<<<<<<
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         if pos < slen:
  */
 struct __pyx_obj_2pe_11_cy_machine_Dot {
   struct __pyx_obj_2pe_11_cy_machine_Scanner __pyx_base;
 };
 
 
-/* "pe/_cy_machine.pyx":522
+/* "pe/_cy_machine.pyx":528
  * 
  * 
  * cdef class Literal(Scanner):             # <<<<<<<<<<<<<<
  *     cdef str _x
  *     cdef int _xlen
  */
 struct __pyx_obj_2pe_11_cy_machine_Literal {
   struct __pyx_obj_2pe_11_cy_machine_Scanner __pyx_base;
   PyObject *_x;
   int _xlen;
 };
 
 
-/* "pe/_cy_machine.pyx":537
+/* "pe/_cy_machine.pyx":543
  * 
  * 
  * cdef class CharacterClass(Scanner):             # <<<<<<<<<<<<<<
  *     cdef:
  *         str _chars, _ranges
  */
 struct __pyx_obj_2pe_11_cy_machine_CharacterClass {
@@ -1131,56 +1134,56 @@
   int _rangelen;
   int _negate;
   int mincount;
   int maxcount;
 };
 
 
-/* "pe/_cy_machine.pyx":589
+/* "pe/_cy_machine.pyx":595
  * 
  * 
  * cdef class Regex(Scanner):             # <<<<<<<<<<<<<<
  *     cdef object _regex
  * 
  */
 struct __pyx_obj_2pe_11_cy_machine_Regex {
   struct __pyx_obj_2pe_11_cy_machine_Scanner __pyx_base;
   PyObject *_regex;
 };
 
 
-/* "pe/_cy_machine.pyx":545
+/* "pe/_cy_machine.pyx":551
  *         int mincount, maxcount
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         list ranges,
  */
 struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct____init__ {
   PyObject_HEAD
   PyObject *__pyx_v_ranges;
 };
 
 
-/* "pe/_cy_machine.pyx":552
+/* "pe/_cy_machine.pyx":558
  *         int maxcount = 1
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)             # <<<<<<<<<<<<<<
  *         self._ranges = ''.join(a+b for a, b in ranges if b)
  *         self._rangelen = len(self._ranges)
  */
 struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr {
   PyObject_HEAD
   struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct____init__ *__pyx_outer_scope;
   PyObject *__pyx_v_a;
   PyObject *__pyx_v_b;
 };
 
 
-/* "pe/_cy_machine.pyx":553
+/* "pe/_cy_machine.pyx":559
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)
  *         self._ranges = ''.join(a+b for a, b in ranges if b)             # <<<<<<<<<<<<<<
  *         self._rangelen = len(self._ranges)
  *         self._negate = negate
  */
 struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr {
@@ -1188,87 +1191,87 @@
   struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct____init__ *__pyx_outer_scope;
   PyObject *__pyx_v_a;
   PyObject *__pyx_v_b;
 };
 
 
 
-/* "pe/_cy_machine.pyx":87
+/* "pe/_cy_machine.pyx":90
  * 
  * 
  * cdef class Scanner:             # <<<<<<<<<<<<<<
  *     cpdef int scan(self, str s, int pos=0) except -2:
  *         try:
  */
 
 struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner {
   int (*scan)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_2pe_11_cy_machine_7Scanner_scan *__pyx_optional_args);
   int (*_scan)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int);
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner *__pyx_vtabptr_2pe_11_cy_machine_Scanner;
 
 
-/* "pe/_cy_machine.pyx":177
+/* "pe/_cy_machine.pyx":183
  * 
  * 
  * cdef class _Parser:             # <<<<<<<<<<<<<<
  *     cdef list pi
  * 
  */
 
 struct __pyx_vtabstruct_2pe_11_cy_machine__Parser {
   int (*match)(struct __pyx_obj_2pe_11_cy_machine__Parser *, int, PyObject *, int, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch);
   struct __pyx_t_2pe_11_cy_machine_State *(*_match)(struct __pyx_obj_2pe_11_cy_machine__Parser *, int, PyObject *, int, PyObject *, PyObject *, PyObject *, struct __pyx_t_2pe_11_cy_machine_State *);
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine__Parser *__pyx_vtabptr_2pe_11_cy_machine__Parser;
 
 
-/* "pe/_cy_machine.pyx":515
+/* "pe/_cy_machine.pyx":521
  * # Scanners #############################################################
  * 
  * cdef class Dot(Scanner):             # <<<<<<<<<<<<<<
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         if pos < slen:
  */
 
 struct __pyx_vtabstruct_2pe_11_cy_machine_Dot {
   struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner __pyx_base;
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_Dot *__pyx_vtabptr_2pe_11_cy_machine_Dot;
 
 
-/* "pe/_cy_machine.pyx":522
+/* "pe/_cy_machine.pyx":528
  * 
  * 
  * cdef class Literal(Scanner):             # <<<<<<<<<<<<<<
  *     cdef str _x
  *     cdef int _xlen
  */
 
 struct __pyx_vtabstruct_2pe_11_cy_machine_Literal {
   struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner __pyx_base;
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_Literal *__pyx_vtabptr_2pe_11_cy_machine_Literal;
 
 
-/* "pe/_cy_machine.pyx":537
+/* "pe/_cy_machine.pyx":543
  * 
  * 
  * cdef class CharacterClass(Scanner):             # <<<<<<<<<<<<<<
  *     cdef:
  *         str _chars, _ranges
  */
 
 struct __pyx_vtabstruct_2pe_11_cy_machine_CharacterClass {
   struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner __pyx_base;
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_CharacterClass *__pyx_vtabptr_2pe_11_cy_machine_CharacterClass;
 
 
-/* "pe/_cy_machine.pyx":589
+/* "pe/_cy_machine.pyx":595
  * 
  * 
  * cdef class Regex(Scanner):             # <<<<<<<<<<<<<<
  *     cdef object _regex
  * 
  */
 
@@ -2159,14 +2162,15 @@
 static const char __pyx_k_COMMON[] = "COMMON";
 static const char __pyx_k_INLINE[] = "INLINE";
 static const char __pyx_k_Parser[] = "_Parser";
 static const char __pyx_k_action[] = "action";
 static const char __pyx_k_append[] = "append";
 static const char __pyx_k_cclass[] = "cclass";
 static const char __pyx_k_common[] = "common";
+static const char __pyx_k_ignore[] = "ignore";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_inline[] = "inline";
 static const char __pyx_k_insert[] = "insert";
 static const char __pyx_k_kwargs[] = "kwargs";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_negate[] = "negate";
@@ -2212,36 +2216,42 @@
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_capturing[] = "capturing";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_pe__match[] = "pe._match";
 static const char __pyx_k_pe__types[] = "pe._types";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
+static const char __pyx_k_Definition[] = "Definition";
 static const char __pyx_k_IndexError[] = "IndexError";
+static const char __pyx_k_autoignore[] = "autoignore";
 static const char __pyx_k_pe__errors[] = "pe._errors";
 static const char __pyx_k_pe__parser[] = "pe._parser";
 static const char __pyx_k_pe_actions[] = "pe.actions";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_Instruction[] = "Instruction";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_definitions[] = "definitions";
 static const char __pyx_k_pe__grammar[] = "pe._grammar";
+static const char __pyx_k_pe_patterns[] = "pe.patterns";
 static const char __pyx_k_make_program[] = "_make_program";
 static const char __pyx_k_pe__optimize[] = "pe._optimize";
 static const char __pyx_k_pe_operators[] = "pe.operators";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_MachineParser[] = "MachineParser";
 static const char __pyx_k_NO_CAP_OR_ACT[] = "NO_CAP_OR_ACT";
 static const char __pyx_k_pe__constants[] = "pe._constants";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_CharacterClass[] = "CharacterClass";
+static const char __pyx_k_DEFAULT_IGNORE[] = "DEFAULT_IGNORE";
+static const char __pyx_k_pe__autoignore[] = "pe._autoignore";
 static const char __pyx_k_pe__cy_machine[] = "pe._cy_machine";
+static const char __pyx_k_pe__definition[] = "pe._definition";
 static const char __pyx_k_captured_choice[] = "captured_choice";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_modified_grammar[] = "modified_grammar";
 static const char __pyx_k_pyx_unpickle_Dot[] = "__pyx_unpickle_Dot";
 static const char __pyx_k_invalid_operation[] = "invalid operation: ";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
@@ -2274,15 +2284,17 @@
 static PyObject *__pyx_n_s_Bind;
 static PyObject *__pyx_n_s_Binding;
 static PyObject *__pyx_n_s_CAP;
 static PyObject *__pyx_n_s_CHC;
 static PyObject *__pyx_n_s_CLS;
 static PyObject *__pyx_n_s_COMMON;
 static PyObject *__pyx_n_s_CharacterClass;
+static PyObject *__pyx_n_s_DEFAULT_IGNORE;
 static PyObject *__pyx_n_s_DOT;
+static PyObject *__pyx_n_s_Definition;
 static PyObject *__pyx_n_s_Dict;
 static PyObject *__pyx_n_s_Dot;
 static PyObject *__pyx_n_s_Error;
 static PyObject *__pyx_n_s_Flag;
 static PyObject *__pyx_n_s_Grammar;
 static PyObject *__pyx_n_s_INLINE;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
@@ -2331,14 +2343,15 @@
 static PyObject *__pyx_n_s_Union;
 static PyObject *__pyx_kp_u__2;
 static PyObject *__pyx_n_s__49;
 static PyObject *__pyx_n_s_action;
 static PyObject *__pyx_n_s_and;
 static PyObject *__pyx_n_s_append;
 static PyObject *__pyx_n_s_args;
+static PyObject *__pyx_n_s_autoignore;
 static PyObject *__pyx_n_s_bnd;
 static PyObject *__pyx_n_s_cap;
 static PyObject *__pyx_n_s_captured_choice;
 static PyObject *__pyx_n_s_capturing;
 static PyObject *__pyx_n_s_cclass;
 static PyObject *__pyx_n_s_chc;
 static PyObject *__pyx_n_s_cline_in_traceback;
@@ -2357,14 +2370,15 @@
 static PyObject *__pyx_n_s_enum;
 static PyObject *__pyx_n_s_flags;
 static PyObject *__pyx_n_s_genexpr;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_grammar;
 static PyObject *__pyx_n_s_head;
 static PyObject *__pyx_n_s_idx;
+static PyObject *__pyx_n_s_ignore;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_index;
 static PyObject *__pyx_n_s_index_2;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_init___locals_genexpr;
 static PyObject *__pyx_n_s_inline;
 static PyObject *__pyx_n_s_insert;
@@ -2394,25 +2408,28 @@
 static PyObject *__pyx_n_s_oploc;
 static PyObject *__pyx_n_s_opt;
 static PyObject *__pyx_n_s_optimize;
 static PyObject *__pyx_n_s_parser;
 static PyObject *__pyx_n_s_parsing_instructions;
 static PyObject *__pyx_n_s_pat;
 static PyObject *__pyx_n_s_pattern;
+static PyObject *__pyx_n_s_pe__autoignore;
 static PyObject *__pyx_n_s_pe__constants;
 static PyObject *__pyx_n_s_pe__cy_machine;
 static PyObject *__pyx_kp_s_pe__cy_machine_pyx;
+static PyObject *__pyx_n_s_pe__definition;
 static PyObject *__pyx_n_s_pe__errors;
 static PyObject *__pyx_n_s_pe__grammar;
 static PyObject *__pyx_n_s_pe__match;
 static PyObject *__pyx_n_s_pe__optimize;
 static PyObject *__pyx_n_s_pe__parser;
 static PyObject *__pyx_n_s_pe__types;
 static PyObject *__pyx_n_s_pe_actions;
 static PyObject *__pyx_n_s_pe_operators;
+static PyObject *__pyx_n_s_pe_patterns;
 static PyObject *__pyx_n_s_pi;
 static PyObject *__pyx_n_s_pi_2;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pis;
 static PyObject *__pyx_n_s_pis_2;
 static PyObject *__pyx_n_s_pls;
 static PyObject *__pyx_kp_u_pop_from_empty_stack;
@@ -2485,15 +2502,15 @@
 static int __pyx_pf_2pe_11_cy_machine_11Instruction_6action_4__del__(struct __pyx_obj_2pe_11_cy_machine_Instruction *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_11Instruction_4name___get__(struct __pyx_obj_2pe_11_cy_machine_Instruction *__pyx_v_self); /* proto */
 static int __pyx_pf_2pe_11_cy_machine_11Instruction_4name_2__set__(struct __pyx_obj_2pe_11_cy_machine_Instruction *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_2pe_11_cy_machine_11Instruction_4name_4__del__(struct __pyx_obj_2pe_11_cy_machine_Instruction *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_11Instruction_2__reduce_cython__(struct __pyx_obj_2pe_11_cy_machine_Instruction *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_11Instruction_4__setstate_cython__(struct __pyx_obj_2pe_11_cy_machine_Instruction *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_50__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_grammar, PyObject *__pyx_v_flags); /* proto */
+static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_grammar, PyObject *__pyx_v_ignore, PyObject *__pyx_v_flags); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser_2start(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser_4__contains__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_52__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser_6match(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_s, int __pyx_v_pos, CYTHON_UNUSED PyObject *__pyx_v_flags); /* proto */
 static int __pyx_pf_2pe_11_cy_machine_7_Parser___init__(struct __pyx_obj_2pe_11_cy_machine__Parser *__pyx_v_self, PyObject *__pyx_v_pi); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_7_Parser_2match(struct __pyx_obj_2pe_11_cy_machine__Parser *__pyx_v_self, int __pyx_v_idx, PyObject *__pyx_v_s, int __pyx_v_pos, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, PyObject *__pyx_v_memo); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_7_Parser_4__reduce_cython__(struct __pyx_obj_2pe_11_cy_machine__Parser *__pyx_v_self); /* proto */
@@ -2635,15 +2652,15 @@
 static PyObject *__pyx_codeobj__59;
 static PyObject *__pyx_codeobj__61;
 static PyObject *__pyx_codeobj__63;
 static PyObject *__pyx_codeobj__65;
 static PyObject *__pyx_codeobj__67;
 /* Late includes */
 
-/* "pe/_cy_machine.pyx":55
+/* "pe/_cy_machine.pyx":58
  * 
  * 
  * cdef State* push(             # <<<<<<<<<<<<<<
  *     int opidx,
  *     int pos,
  */
 
@@ -2653,116 +2670,116 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("push", 0);
 
-  /* "pe/_cy_machine.pyx":63
+  /* "pe/_cy_machine.pyx":66
  *     State* prev
  * ) except NULL:
  *     cdef State* state = <State*>PyMem_Malloc(sizeof(State))             # <<<<<<<<<<<<<<
  *     if not state:
  *         raise MemoryError()
  */
   __pyx_v_state = ((struct __pyx_t_2pe_11_cy_machine_State *)PyMem_Malloc((sizeof(struct __pyx_t_2pe_11_cy_machine_State))));
 
-  /* "pe/_cy_machine.pyx":64
+  /* "pe/_cy_machine.pyx":67
  * ) except NULL:
  *     cdef State* state = <State*>PyMem_Malloc(sizeof(State))
  *     if not state:             # <<<<<<<<<<<<<<
  *         raise MemoryError()
  *     state.opidx = opidx
  */
   __pyx_t_1 = ((!(__pyx_v_state != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pe/_cy_machine.pyx":65
+    /* "pe/_cy_machine.pyx":68
  *     cdef State* state = <State*>PyMem_Malloc(sizeof(State))
  *     if not state:
  *         raise MemoryError()             # <<<<<<<<<<<<<<
  *     state.opidx = opidx
  *     state.pos = pos
  */
-    PyErr_NoMemory(); __PYX_ERR(0, 65, __pyx_L1_error)
+    PyErr_NoMemory(); __PYX_ERR(0, 68, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":64
+    /* "pe/_cy_machine.pyx":67
  * ) except NULL:
  *     cdef State* state = <State*>PyMem_Malloc(sizeof(State))
  *     if not state:             # <<<<<<<<<<<<<<
  *         raise MemoryError()
  *     state.opidx = opidx
  */
   }
 
-  /* "pe/_cy_machine.pyx":66
+  /* "pe/_cy_machine.pyx":69
  *     if not state:
  *         raise MemoryError()
  *     state.opidx = opidx             # <<<<<<<<<<<<<<
  *     state.pos = pos
  *     state.mark = mark
  */
   __pyx_v_state->opidx = __pyx_v_opidx;
 
-  /* "pe/_cy_machine.pyx":67
+  /* "pe/_cy_machine.pyx":70
  *         raise MemoryError()
  *     state.opidx = opidx
  *     state.pos = pos             # <<<<<<<<<<<<<<
  *     state.mark = mark
  *     state.argidx = argidx
  */
   __pyx_v_state->pos = __pyx_v_pos;
 
-  /* "pe/_cy_machine.pyx":68
+  /* "pe/_cy_machine.pyx":71
  *     state.opidx = opidx
  *     state.pos = pos
  *     state.mark = mark             # <<<<<<<<<<<<<<
  *     state.argidx = argidx
  *     state.kwidx = kwidx
  */
   __pyx_v_state->mark = __pyx_v_mark;
 
-  /* "pe/_cy_machine.pyx":69
+  /* "pe/_cy_machine.pyx":72
  *     state.pos = pos
  *     state.mark = mark
  *     state.argidx = argidx             # <<<<<<<<<<<<<<
  *     state.kwidx = kwidx
  *     state.prev = prev
  */
   __pyx_v_state->argidx = __pyx_v_argidx;
 
-  /* "pe/_cy_machine.pyx":70
+  /* "pe/_cy_machine.pyx":73
  *     state.mark = mark
  *     state.argidx = argidx
  *     state.kwidx = kwidx             # <<<<<<<<<<<<<<
  *     state.prev = prev
  *     return state
  */
   __pyx_v_state->kwidx = __pyx_v_kwidx;
 
-  /* "pe/_cy_machine.pyx":71
+  /* "pe/_cy_machine.pyx":74
  *     state.argidx = argidx
  *     state.kwidx = kwidx
  *     state.prev = prev             # <<<<<<<<<<<<<<
  *     return state
  * 
  */
   __pyx_v_state->prev = __pyx_v_prev;
 
-  /* "pe/_cy_machine.pyx":72
+  /* "pe/_cy_machine.pyx":75
  *     state.kwidx = kwidx
  *     state.prev = prev
  *     return state             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_state;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":55
+  /* "pe/_cy_machine.pyx":58
  * 
  * 
  * cdef State* push(             # <<<<<<<<<<<<<<
  *     int opidx,
  *     int pos,
  */
 
@@ -2771,15 +2788,15 @@
   __Pyx_AddTraceback("pe._cy_machine.push", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":75
+/* "pe/_cy_machine.pyx":78
  * 
  * 
  * cdef State* pop(State* state) except? NULL:             # <<<<<<<<<<<<<<
  *     if not state:
  *         raise Error('pop from empty stack')
  */
 
@@ -2793,91 +2810,91 @@
   PyObject *__pyx_t_4 = NULL;
   struct __pyx_t_2pe_11_cy_machine_State *__pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pop", 0);
 
-  /* "pe/_cy_machine.pyx":76
+  /* "pe/_cy_machine.pyx":79
  * 
  * cdef State* pop(State* state) except? NULL:
  *     if not state:             # <<<<<<<<<<<<<<
  *         raise Error('pop from empty stack')
  *     cdef State* prev = state.prev
  */
   __pyx_t_1 = ((!(__pyx_v_state != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pe/_cy_machine.pyx":77
+    /* "pe/_cy_machine.pyx":80
  * cdef State* pop(State* state) except? NULL:
  *     if not state:
  *         raise Error('pop from empty stack')             # <<<<<<<<<<<<<<
  *     cdef State* prev = state.prev
  *     PyMem_Free(state)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Error); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Error); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_pop_from_empty_stack) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_pop_from_empty_stack);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 77, __pyx_L1_error)
+    __PYX_ERR(0, 80, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":76
+    /* "pe/_cy_machine.pyx":79
  * 
  * cdef State* pop(State* state) except? NULL:
  *     if not state:             # <<<<<<<<<<<<<<
  *         raise Error('pop from empty stack')
  *     cdef State* prev = state.prev
  */
   }
 
-  /* "pe/_cy_machine.pyx":78
+  /* "pe/_cy_machine.pyx":81
  *     if not state:
  *         raise Error('pop from empty stack')
  *     cdef State* prev = state.prev             # <<<<<<<<<<<<<<
  *     PyMem_Free(state)
  *     return prev
  */
   __pyx_t_5 = __pyx_v_state->prev;
   __pyx_v_prev = __pyx_t_5;
 
-  /* "pe/_cy_machine.pyx":79
+  /* "pe/_cy_machine.pyx":82
  *         raise Error('pop from empty stack')
  *     cdef State* prev = state.prev
  *     PyMem_Free(state)             # <<<<<<<<<<<<<<
  *     return prev
  * 
  */
   PyMem_Free(__pyx_v_state);
 
-  /* "pe/_cy_machine.pyx":80
+  /* "pe/_cy_machine.pyx":83
  *     cdef State* prev = state.prev
  *     PyMem_Free(state)
  *     return prev             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_prev;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":75
+  /* "pe/_cy_machine.pyx":78
  * 
  * 
  * cdef State* pop(State* state) except? NULL:             # <<<<<<<<<<<<<<
  *     if not state:
  *         raise Error('pop from empty stack')
  */
 
@@ -2889,15 +2906,15 @@
   __Pyx_AddTraceback("pe._cy_machine.pop", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":88
+/* "pe/_cy_machine.pyx":91
  * 
  * cdef class Scanner:
  *     cpdef int scan(self, str s, int pos=0) except -2:             # <<<<<<<<<<<<<<
  *         try:
  *             return self._scan(s, pos, len(s))
  */
 
@@ -2931,18 +2948,18 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_scan); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_scan); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_2pe_11_cy_machine_7Scanner_1scan)) {
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_4 = __pyx_t_1; __pyx_t_5 = NULL;
         __pyx_t_6 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
           if (likely(__pyx_t_5)) {
@@ -2952,47 +2969,47 @@
             __Pyx_DECREF_SET(__pyx_t_4, function);
             __pyx_t_6 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_s, __pyx_t_3};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
           PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_s, __pyx_t_3};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else
         #endif
         {
-          __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 88, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           if (__pyx_t_5) {
             __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
           }
           __Pyx_INCREF(__pyx_v_s);
           __Pyx_GIVEREF(__pyx_v_s);
           PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_s);
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_3);
           __pyx_t_3 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 91, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_6;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -3003,15 +3020,15 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "pe/_cy_machine.pyx":89
+  /* "pe/_cy_machine.pyx":92
  * cdef class Scanner:
  *     cpdef int scan(self, str s, int pos=0) except -2:
  *         try:             # <<<<<<<<<<<<<<
  *             return self._scan(s, pos, len(s))
  *         except IndexError:
  */
   {
@@ -3019,31 +3036,31 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10);
     __Pyx_XGOTREF(__pyx_t_8);
     __Pyx_XGOTREF(__pyx_t_9);
     __Pyx_XGOTREF(__pyx_t_10);
     /*try:*/ {
 
-      /* "pe/_cy_machine.pyx":90
+      /* "pe/_cy_machine.pyx":93
  *     cpdef int scan(self, str s, int pos=0) except -2:
  *         try:
  *             return self._scan(s, pos, len(s))             # <<<<<<<<<<<<<<
  *         except IndexError:
  *             return FAILURE
  */
       if (unlikely(__pyx_v_s == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 90, __pyx_L3_error)
+        __PYX_ERR(0, 93, __pyx_L3_error)
       }
-      __pyx_t_11 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_s); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 90, __pyx_L3_error)
-      __pyx_t_6 = ((struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner *)__pyx_v_self->__pyx_vtab)->_scan(__pyx_v_self, __pyx_v_s, __pyx_v_pos, __pyx_t_11); if (unlikely(__pyx_t_6 == ((int)-2))) __PYX_ERR(0, 90, __pyx_L3_error)
+      __pyx_t_11 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_s); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 93, __pyx_L3_error)
+      __pyx_t_6 = ((struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner *)__pyx_v_self->__pyx_vtab)->_scan(__pyx_v_self, __pyx_v_s, __pyx_v_pos, __pyx_t_11); if (unlikely(__pyx_t_6 == ((int)-2))) __PYX_ERR(0, 93, __pyx_L3_error)
       __pyx_r = __pyx_t_6;
       goto __pyx_L7_try_return;
 
-      /* "pe/_cy_machine.pyx":89
+      /* "pe/_cy_machine.pyx":92
  * cdef class Scanner:
  *     cpdef int scan(self, str s, int pos=0) except -2:
  *         try:             # <<<<<<<<<<<<<<
  *             return self._scan(s, pos, len(s))
  *         except IndexError:
  */
     }
@@ -3051,30 +3068,30 @@
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "pe/_cy_machine.pyx":91
+    /* "pe/_cy_machine.pyx":94
  *         try:
  *             return self._scan(s, pos, len(s))
  *         except IndexError:             # <<<<<<<<<<<<<<
  *             return FAILURE
  * 
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError);
     if (__pyx_t_6) {
       __Pyx_AddTraceback("pe._cy_machine.Scanner.scan", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_4) < 0) __PYX_ERR(0, 91, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_4) < 0) __PYX_ERR(0, 94, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GOTREF(__pyx_t_4);
 
-      /* "pe/_cy_machine.pyx":92
+      /* "pe/_cy_machine.pyx":95
  *             return self._scan(s, pos, len(s))
  *         except IndexError:
  *             return FAILURE             # <<<<<<<<<<<<<<
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  */
       __pyx_r = -1;
@@ -3082,15 +3099,15 @@
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       goto __pyx_L6_except_return;
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "pe/_cy_machine.pyx":89
+    /* "pe/_cy_machine.pyx":92
  * cdef class Scanner:
  *     cpdef int scan(self, str s, int pos=0) except -2:
  *         try:             # <<<<<<<<<<<<<<
  *             return self._scan(s, pos, len(s))
  *         except IndexError:
  */
     __Pyx_XGIVEREF(__pyx_t_8);
@@ -3108,15 +3125,15 @@
     __Pyx_XGIVEREF(__pyx_t_8);
     __Pyx_XGIVEREF(__pyx_t_9);
     __Pyx_XGIVEREF(__pyx_t_10);
     __Pyx_ExceptionReset(__pyx_t_8, __pyx_t_9, __pyx_t_10);
     goto __pyx_L0;
   }
 
-  /* "pe/_cy_machine.pyx":88
+  /* "pe/_cy_machine.pyx":91
  * 
  * cdef class Scanner:
  *     cpdef int scan(self, str s, int pos=0) except -2:             # <<<<<<<<<<<<<<
  *         try:
  *             return self._scan(s, pos, len(s))
  */
 
@@ -3169,41 +3186,41 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pos);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "scan") < 0)) __PYX_ERR(0, 88, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "scan") < 0)) __PYX_ERR(0, 91, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_s = ((PyObject*)values[0]);
     if (values[1]) {
-      __pyx_v_pos = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
+      __pyx_v_pos = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 91, __pyx_L3_error)
     } else {
       __pyx_v_pos = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("scan", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 88, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("scan", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 91, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine.Scanner.scan", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyUnicode_Type), 1, "s", 1))) __PYX_ERR(0, 88, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyUnicode_Type), 1, "s", 1))) __PYX_ERR(0, 91, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_7Scanner_scan(((struct __pyx_obj_2pe_11_cy_machine_Scanner *)__pyx_v_self), __pyx_v_s, __pyx_v_pos);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -3220,16 +3237,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("scan", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 1;
   __pyx_t_2.pos = __pyx_v_pos;
-  __pyx_t_1 = __pyx_vtabptr_2pe_11_cy_machine_Scanner->scan(__pyx_v_self, __pyx_v_s, 1, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((int)-2))) __PYX_ERR(0, 88, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_1 = __pyx_vtabptr_2pe_11_cy_machine_Scanner->scan(__pyx_v_self, __pyx_v_s, 1, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((int)-2))) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3238,38 +3255,38 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":94
+/* "pe/_cy_machine.pyx":97
  *             return FAILURE
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         return FAILURE
  * 
  */
 
 static int __pyx_f_2pe_11_cy_machine_7Scanner__scan(CYTHON_UNUSED struct __pyx_obj_2pe_11_cy_machine_Scanner *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_s, CYTHON_UNUSED int __pyx_v_pos, CYTHON_UNUSED int __pyx_v_slen) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_scan", 0);
 
-  /* "pe/_cy_machine.pyx":95
+  /* "pe/_cy_machine.pyx":98
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         return FAILURE             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = -1;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":94
+  /* "pe/_cy_machine.pyx":97
  *             return FAILURE
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         return FAILURE
  * 
  */
 
@@ -3562,15 +3579,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":108
+/* "pe/_cy_machine.pyx":111
  *         str name
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         OpCode opcode,
  */
 
@@ -3590,33 +3607,33 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_opcode,&__pyx_n_s_oploc,&__pyx_n_s_scanner,&__pyx_n_s_marking,&__pyx_n_s_capturing,&__pyx_n_s_action,&__pyx_n_s_name,0};
     PyObject* values[7] = {0,0,0,0,0,0,0};
 
-    /* "pe/_cy_machine.pyx":112
+    /* "pe/_cy_machine.pyx":115
  *         OpCode opcode,
  *         short oploc=1,
  *         Scanner scanner=None,             # <<<<<<<<<<<<<<
  *         bint marking=False,
  *         bint capturing=False,
  */
     values[2] = (PyObject *)((struct __pyx_obj_2pe_11_cy_machine_Scanner *)Py_None);
 
-    /* "pe/_cy_machine.pyx":115
+    /* "pe/_cy_machine.pyx":118
  *         bint marking=False,
  *         bint capturing=False,
  *         object action=None,             # <<<<<<<<<<<<<<
  *         str name=None
  *     ):
  */
     values[5] = ((PyObject *)Py_None);
 
-    /* "pe/_cy_machine.pyx":116
+    /* "pe/_cy_machine.pyx":119
  *         bint capturing=False,
  *         object action=None,
  *         str name=None             # <<<<<<<<<<<<<<
  *     ):
  *         self.opcode = opcode
  */
     values[6] = ((PyObject*)Py_None);
@@ -3680,15 +3697,15 @@
         case  6:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name);
           if (value) { values[6] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 108, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 111, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
@@ -3701,63 +3718,63 @@
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_opcode = ((enum __pyx_t_2pe_11_cy_machine_OpCode)__Pyx_PyInt_As_enum____pyx_t_2pe_11_cy_machine_OpCode(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L3_error)
+    __pyx_v_opcode = ((enum __pyx_t_2pe_11_cy_machine_OpCode)__Pyx_PyInt_As_enum____pyx_t_2pe_11_cy_machine_OpCode(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
     if (values[1]) {
-      __pyx_v_oploc = __Pyx_PyInt_As_short(values[1]); if (unlikely((__pyx_v_oploc == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L3_error)
+      __pyx_v_oploc = __Pyx_PyInt_As_short(values[1]); if (unlikely((__pyx_v_oploc == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
     } else {
       __pyx_v_oploc = ((short)1);
     }
     __pyx_v_scanner = ((struct __pyx_obj_2pe_11_cy_machine_Scanner *)values[2]);
     if (values[3]) {
-      __pyx_v_marking = __Pyx_PyObject_IsTrue(values[3]); if (unlikely((__pyx_v_marking == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L3_error)
+      __pyx_v_marking = __Pyx_PyObject_IsTrue(values[3]); if (unlikely((__pyx_v_marking == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L3_error)
     } else {
 
-      /* "pe/_cy_machine.pyx":113
+      /* "pe/_cy_machine.pyx":116
  *         short oploc=1,
  *         Scanner scanner=None,
  *         bint marking=False,             # <<<<<<<<<<<<<<
  *         bint capturing=False,
  *         object action=None,
  */
       __pyx_v_marking = ((int)0);
     }
     if (values[4]) {
-      __pyx_v_capturing = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_capturing == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
+      __pyx_v_capturing = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_capturing == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L3_error)
     } else {
 
-      /* "pe/_cy_machine.pyx":114
+      /* "pe/_cy_machine.pyx":117
  *         Scanner scanner=None,
  *         bint marking=False,
  *         bint capturing=False,             # <<<<<<<<<<<<<<
  *         object action=None,
  *         str name=None
  */
       __pyx_v_capturing = ((int)0);
     }
     __pyx_v_action = values[5];
     __pyx_v_name = ((PyObject*)values[6]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 108, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 7, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 111, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine.Instruction.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_scanner), __pyx_ptype_2pe_11_cy_machine_Scanner, 1, "scanner", 0))) __PYX_ERR(0, 112, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_scanner), __pyx_ptype_2pe_11_cy_machine_Scanner, 1, "scanner", 0))) __PYX_ERR(0, 115, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 119, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_11Instruction___init__(((struct __pyx_obj_2pe_11_cy_machine_Instruction *)__pyx_v_self), __pyx_v_opcode, __pyx_v_oploc, __pyx_v_scanner, __pyx_v_marking, __pyx_v_capturing, __pyx_v_action, __pyx_v_name);
 
-  /* "pe/_cy_machine.pyx":108
+  /* "pe/_cy_machine.pyx":111
  *         str name
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         OpCode opcode,
  */
 
@@ -3771,104 +3788,104 @@
 }
 
 static int __pyx_pf_2pe_11_cy_machine_11Instruction___init__(struct __pyx_obj_2pe_11_cy_machine_Instruction *__pyx_v_self, enum __pyx_t_2pe_11_cy_machine_OpCode __pyx_v_opcode, short __pyx_v_oploc, struct __pyx_obj_2pe_11_cy_machine_Scanner *__pyx_v_scanner, int __pyx_v_marking, int __pyx_v_capturing, PyObject *__pyx_v_action, PyObject *__pyx_v_name) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pe/_cy_machine.pyx":118
+  /* "pe/_cy_machine.pyx":121
  *         str name=None
  *     ):
  *         self.opcode = opcode             # <<<<<<<<<<<<<<
  *         self.oploc = oploc
  *         self.scanner = scanner
  */
   __pyx_v_self->opcode = __pyx_v_opcode;
 
-  /* "pe/_cy_machine.pyx":119
+  /* "pe/_cy_machine.pyx":122
  *     ):
  *         self.opcode = opcode
  *         self.oploc = oploc             # <<<<<<<<<<<<<<
  *         self.scanner = scanner
  *         self.marking = marking
  */
   __pyx_v_self->oploc = __pyx_v_oploc;
 
-  /* "pe/_cy_machine.pyx":120
+  /* "pe/_cy_machine.pyx":123
  *         self.opcode = opcode
  *         self.oploc = oploc
  *         self.scanner = scanner             # <<<<<<<<<<<<<<
  *         self.marking = marking
  *         self.capturing = capturing
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_scanner));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_scanner));
   __Pyx_GOTREF(__pyx_v_self->scanner);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->scanner));
   __pyx_v_self->scanner = __pyx_v_scanner;
 
-  /* "pe/_cy_machine.pyx":121
+  /* "pe/_cy_machine.pyx":124
  *         self.oploc = oploc
  *         self.scanner = scanner
  *         self.marking = marking             # <<<<<<<<<<<<<<
  *         self.capturing = capturing
  *         self.action = action
  */
   __pyx_v_self->marking = __pyx_v_marking;
 
-  /* "pe/_cy_machine.pyx":122
+  /* "pe/_cy_machine.pyx":125
  *         self.scanner = scanner
  *         self.marking = marking
  *         self.capturing = capturing             # <<<<<<<<<<<<<<
  *         self.action = action
  *         self.name = name
  */
   __pyx_v_self->capturing = __pyx_v_capturing;
 
-  /* "pe/_cy_machine.pyx":123
+  /* "pe/_cy_machine.pyx":126
  *         self.marking = marking
  *         self.capturing = capturing
  *         self.action = action             # <<<<<<<<<<<<<<
  *         self.name = name
  * 
  */
   __Pyx_INCREF(__pyx_v_action);
   __Pyx_GIVEREF(__pyx_v_action);
   __Pyx_GOTREF(__pyx_v_self->action);
   __Pyx_DECREF(__pyx_v_self->action);
   __pyx_v_self->action = __pyx_v_action;
 
-  /* "pe/_cy_machine.pyx":124
+  /* "pe/_cy_machine.pyx":127
  *         self.capturing = capturing
  *         self.action = action
  *         self.name = name             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_INCREF(__pyx_v_name);
   __Pyx_GIVEREF(__pyx_v_name);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = __pyx_v_name;
 
-  /* "pe/_cy_machine.pyx":108
+  /* "pe/_cy_machine.pyx":111
  *         str name
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         OpCode opcode,
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":100
+/* "pe/_cy_machine.pyx":103
  * cdef class Instruction:
  *     cdef public:
  *         OpCode opcode             # <<<<<<<<<<<<<<
  *         short oploc
  *         Scanner scanner
  */
 
@@ -3890,15 +3907,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_v_self->opcode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_v_self->opcode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3928,29 +3945,29 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   enum __pyx_t_2pe_11_cy_machine_OpCode __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = ((enum __pyx_t_2pe_11_cy_machine_OpCode)__Pyx_PyInt_As_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_v_value)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_1 = ((enum __pyx_t_2pe_11_cy_machine_OpCode)__Pyx_PyInt_As_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_v_value)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 103, __pyx_L1_error)
   __pyx_v_self->opcode = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pe._cy_machine.Instruction.opcode.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":101
+/* "pe/_cy_machine.pyx":104
  *     cdef public:
  *         OpCode opcode
  *         short oploc             # <<<<<<<<<<<<<<
  *         Scanner scanner
  *         bint marking
  */
 
@@ -3972,15 +3989,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_short(__pyx_v_self->oploc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_short(__pyx_v_self->oploc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4010,29 +4027,29 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   short __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_short(__pyx_v_value); if (unlikely((__pyx_t_1 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_short(__pyx_v_value); if (unlikely((__pyx_t_1 == (short)-1) && PyErr_Occurred())) __PYX_ERR(0, 104, __pyx_L1_error)
   __pyx_v_self->oploc = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pe._cy_machine.Instruction.oploc.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":102
+/* "pe/_cy_machine.pyx":105
  *         OpCode opcode
  *         short oploc
  *         Scanner scanner             # <<<<<<<<<<<<<<
  *         bint marking
  *         bint capturing
  */
 
@@ -4082,15 +4099,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(((__pyx_v_value) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_value, __pyx_ptype_2pe_11_cy_machine_Scanner))))) __PYX_ERR(0, 102, __pyx_L1_error)
+  if (!(likely(((__pyx_v_value) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_value, __pyx_ptype_2pe_11_cy_machine_Scanner))))) __PYX_ERR(0, 105, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->scanner);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->scanner));
   __pyx_v_self->scanner = ((struct __pyx_obj_2pe_11_cy_machine_Scanner *)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -4132,15 +4149,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":103
+/* "pe/_cy_machine.pyx":106
  *         short oploc
  *         Scanner scanner
  *         bint marking             # <<<<<<<<<<<<<<
  *         bint capturing
  *         object action
  */
 
@@ -4162,15 +4179,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->marking); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->marking); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4200,29 +4217,29 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L1_error)
   __pyx_v_self->marking = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pe._cy_machine.Instruction.marking.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":104
+/* "pe/_cy_machine.pyx":107
  *         Scanner scanner
  *         bint marking
  *         bint capturing             # <<<<<<<<<<<<<<
  *         object action
  *         str name
  */
 
@@ -4244,15 +4261,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->capturing); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->capturing); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4282,29 +4299,29 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
   __pyx_v_self->capturing = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pe._cy_machine.Instruction.capturing.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":105
+/* "pe/_cy_machine.pyx":108
  *         bint marking
  *         bint capturing
  *         object action             # <<<<<<<<<<<<<<
  *         str name
  * 
  */
 
@@ -4391,15 +4408,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":106
+/* "pe/_cy_machine.pyx":109
  *         bint capturing
  *         object action
  *         str name             # <<<<<<<<<<<<<<
  * 
  *     def __init__(
  */
 
@@ -4449,15 +4466,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 109, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -4840,38 +4857,41 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":132
+/* "pe/_cy_machine.pyx":135
  * class MachineParser(Parser):
  * 
  *     def __init__(self, grammar: Grammar,             # <<<<<<<<<<<<<<
+ *                  ignore: Optional[Definition] = DEFAULT_IGNORE,
  *                  flags: Flag = Flag.NONE):
- *         super().__init__(grammar, flags=flags)
  */
 
 static PyObject *__pyx_pf_2pe_11_cy_machine_50__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_ignore);
+  __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_ignore);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_ignore);
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_flags);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_flags);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_flags);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self)->__pyx_arg_flags);
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_2, 1, Py_None);
   __pyx_t_1 = 0;
@@ -4893,30 +4913,34 @@
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2pe_11_cy_machine_13MachineParser_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_2pe_11_cy_machine_13MachineParser_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2pe_11_cy_machine_13MachineParser_1__init__, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_2pe_11_cy_machine_13MachineParser_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_grammar = 0;
+  PyObject *__pyx_v_ignore = 0;
   PyObject *__pyx_v_flags = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_grammar,&__pyx_n_s_flags,0};
-    PyObject* values[3] = {0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_grammar,&__pyx_n_s_ignore,&__pyx_n_s_flags,0};
+    PyObject* values[4] = {0,0,0,0};
     __pyx_defaults *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self);
-    values[2] = __pyx_dynamic_args->__pyx_arg_flags;
+    values[2] = __pyx_dynamic_args->__pyx_arg_ignore;
+    values[3] = __pyx_dynamic_args->__pyx_arg_flags;
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
@@ -4927,322 +4951,389 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_grammar)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 132, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, 1); __PYX_ERR(0, 135, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flags);
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ignore);
           if (value) { values[2] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flags);
+          if (value) { values[3] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 132, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 135, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_self = values[0];
     __pyx_v_grammar = values[1];
-    __pyx_v_flags = values[2];
+    __pyx_v_ignore = values[2];
+    __pyx_v_flags = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 132, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 135, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine.MachineParser.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2pe_11_cy_machine_13MachineParser___init__(__pyx_self, __pyx_v_self, __pyx_v_grammar, __pyx_v_flags);
+  __pyx_r = __pyx_pf_2pe_11_cy_machine_13MachineParser___init__(__pyx_self, __pyx_v_self, __pyx_v_grammar, __pyx_v_ignore, __pyx_v_flags);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_grammar, PyObject *__pyx_v_flags) {
+static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_grammar, PyObject *__pyx_v_ignore, PyObject *__pyx_v_flags) {
   PyObject *__pyx_v_pi = NULL;
   PyObject *__pyx_v_index = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *(*__pyx_t_6)(PyObject *);
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *(*__pyx_t_7)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
   __Pyx_INCREF(__pyx_v_grammar);
 
-  /* "pe/_cy_machine.pyx":134
- *     def __init__(self, grammar: Grammar,
+  /* "pe/_cy_machine.pyx":138
+ *                  ignore: Optional[Definition] = DEFAULT_IGNORE,
  *                  flags: Flag = Flag.NONE):
  *         super().__init__(grammar, flags=flags)             # <<<<<<<<<<<<<<
  * 
- *         grammar = optimize(grammar,
+ *         grammar = autoignore(grammar, ignore)
  */
   __pyx_t_1 = __Pyx_CyFunction_GetClassObj(__pyx_self);
-  if (!__pyx_t_1) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 134, __pyx_L1_error) }
+  if (!__pyx_t_1) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 138, __pyx_L1_error) }
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_v_self);
   __Pyx_GIVEREF(__pyx_v_self);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_self);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_init); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_grammar);
   __Pyx_GIVEREF(__pyx_v_grammar);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_grammar);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flags, __pyx_v_flags) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flags, __pyx_v_flags) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":136
+  /* "pe/_cy_machine.pyx":140
  *         super().__init__(grammar, flags=flags)
  * 
+ *         grammar = autoignore(grammar, ignore)             # <<<<<<<<<<<<<<
+ * 
+ *         grammar = optimize(grammar,
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_autoignore); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_1 = NULL;
+  __pyx_t_5 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_5 = 1;
+    }
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_grammar, __pyx_v_ignore};
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_GOTREF(__pyx_t_4);
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_grammar, __pyx_v_ignore};
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_GOTREF(__pyx_t_4);
+  } else
+  #endif
+  {
+    __pyx_t_2 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (__pyx_t_1) {
+      __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1); __pyx_t_1 = NULL;
+    }
+    __Pyx_INCREF(__pyx_v_grammar);
+    __Pyx_GIVEREF(__pyx_v_grammar);
+    PyTuple_SET_ITEM(__pyx_t_2, 0+__pyx_t_5, __pyx_v_grammar);
+    __Pyx_INCREF(__pyx_v_ignore);
+    __Pyx_GIVEREF(__pyx_v_ignore);
+    PyTuple_SET_ITEM(__pyx_t_2, 1+__pyx_t_5, __pyx_v_ignore);
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF_SET(__pyx_v_grammar, __pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "pe/_cy_machine.pyx":142
+ *         grammar = autoignore(grammar, ignore)
+ * 
  *         grammar = optimize(grammar,             # <<<<<<<<<<<<<<
  *                            inline=flags & Flag.INLINE,
  *                            common=flags & Flag.COMMON,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_optimize); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_optimize); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_grammar);
   __Pyx_GIVEREF(__pyx_v_grammar);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_grammar);
 
-  /* "pe/_cy_machine.pyx":137
+  /* "pe/_cy_machine.pyx":143
  * 
  *         grammar = optimize(grammar,
  *                            inline=flags & Flag.INLINE,             # <<<<<<<<<<<<<<
  *                            common=flags & Flag.COMMON,
  *                            regex=False)
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Flag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INLINE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_And(__pyx_v_flags, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_inline, __pyx_t_2) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Flag); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_INLINE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyNumber_And(__pyx_v_flags, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_inline, __pyx_t_1) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":138
+  /* "pe/_cy_machine.pyx":144
  *         grammar = optimize(grammar,
  *                            inline=flags & Flag.INLINE,
  *                            common=flags & Flag.COMMON,             # <<<<<<<<<<<<<<
  *                            regex=False)
  *         # if flags & Flag.DEBUG:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Flag); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_COMMON); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_And(__pyx_v_flags, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_common, __pyx_t_2) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Flag); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_COMMON); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyNumber_And(__pyx_v_flags, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_common, __pyx_t_1) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":139
+  /* "pe/_cy_machine.pyx":145
  *                            inline=flags & Flag.INLINE,
  *                            common=flags & Flag.COMMON,
  *                            regex=False)             # <<<<<<<<<<<<<<
  *         # if flags & Flag.DEBUG:
  *         #     grammar = debug(grammar)
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_regex, Py_False) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_regex, Py_False) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":136
- *         super().__init__(grammar, flags=flags)
+  /* "pe/_cy_machine.pyx":142
+ *         grammar = autoignore(grammar, ignore)
  * 
  *         grammar = optimize(grammar,             # <<<<<<<<<<<<<<
  *                            inline=flags & Flag.INLINE,
  *                            common=flags & Flag.COMMON,
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF_SET(__pyx_v_grammar, __pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF_SET(__pyx_v_grammar, __pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":142
+  /* "pe/_cy_machine.pyx":148
  *         # if flags & Flag.DEBUG:
  *         #     grammar = debug(grammar)
  *         self.modified_grammar = grammar             # <<<<<<<<<<<<<<
  * 
  *         pi, index = _make_program(grammar)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_modified_grammar, __pyx_v_grammar) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_modified_grammar, __pyx_v_grammar) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":144
+  /* "pe/_cy_machine.pyx":150
  *         self.modified_grammar = grammar
  * 
  *         pi, index = _make_program(grammar)             # <<<<<<<<<<<<<<
  *         self._parser = _Parser(pi)
  *         self._index = index
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_make_program); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_make_program); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_v_grammar) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_grammar);
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_grammar) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_grammar);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
-    PyObject* sequence = __pyx_t_2;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
+    PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 144, __pyx_L1_error)
+      __PYX_ERR(0, 150, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
-      __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
+      __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
-      __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
+      __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
     }
-    __Pyx_INCREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 144, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_4 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 144, __pyx_L1_error)
+    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext;
-    index = 0; __pyx_t_1 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_1)) goto __pyx_L3_unpacking_failed;
-    __Pyx_GOTREF(__pyx_t_1);
-    index = 1; __pyx_t_3 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_7 = Py_TYPE(__pyx_t_4)->tp_iternext;
+    index = 0; __pyx_t_2 = __pyx_t_7(__pyx_t_4); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
+    __Pyx_GOTREF(__pyx_t_2);
+    index = 1; __pyx_t_3 = __pyx_t_7(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_4), 2) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
-    __pyx_t_6 = NULL;
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_4), 2) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+    __pyx_t_7 = NULL;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_6 = NULL;
+    __pyx_t_7 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 144, __pyx_L1_error)
+    __PYX_ERR(0, 150, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
-  __pyx_v_pi = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_v_pi = __pyx_t_2;
+  __pyx_t_2 = 0;
   __pyx_v_index = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":145
+  /* "pe/_cy_machine.pyx":151
  * 
  *         pi, index = _make_program(grammar)
  *         self._parser = _Parser(pi)             # <<<<<<<<<<<<<<
  *         self._index = index
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine__Parser), __pyx_v_pi); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_parser, __pyx_t_2) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine__Parser), __pyx_v_pi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_parser, __pyx_t_1) < 0) __PYX_ERR(0, 151, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":146
+  /* "pe/_cy_machine.pyx":152
  *         pi, index = _make_program(grammar)
  *         self._parser = _Parser(pi)
  *         self._index = index             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_index, __pyx_v_index) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_index, __pyx_v_index) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":132
+  /* "pe/_cy_machine.pyx":135
  * class MachineParser(Parser):
  * 
  *     def __init__(self, grammar: Grammar,             # <<<<<<<<<<<<<<
+ *                  ignore: Optional[Definition] = DEFAULT_IGNORE,
  *                  flags: Flag = Flag.NONE):
- *         super().__init__(grammar, flags=flags)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("pe._cy_machine.MachineParser.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XDECREF(__pyx_v_grammar);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":149
+/* "pe/_cy_machine.pyx":155
  * 
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         return self.grammar.start
  * 
  */
 
@@ -5266,32 +5357,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("start", 0);
 
-  /* "pe/_cy_machine.pyx":150
+  /* "pe/_cy_machine.pyx":156
  *     @property
  *     def start(self):
  *         return self.grammar.start             # <<<<<<<<<<<<<<
  * 
  *     def __contains__(self, name: str) -> bool:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_grammar); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_grammar); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":149
+  /* "pe/_cy_machine.pyx":155
  * 
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         return self.grammar.start
  * 
  */
 
@@ -5303,15 +5394,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":152
+/* "pe/_cy_machine.pyx":158
  *         return self.grammar.start
  * 
  *     def __contains__(self, name: str) -> bool:             # <<<<<<<<<<<<<<
  *         return name in self._index
  * 
  */
 
@@ -5346,38 +5437,38 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__contains__", 1, 2, 2, 1); __PYX_ERR(0, 152, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__contains__", 1, 2, 2, 1); __PYX_ERR(0, 158, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__contains__") < 0)) __PYX_ERR(0, 152, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__contains__") < 0)) __PYX_ERR(0, 158, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_name = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__contains__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 152, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__contains__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 158, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine.MachineParser.__contains__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 152, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 158, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_13MachineParser_4__contains__(__pyx_self, __pyx_v_self, __pyx_v_name);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5391,33 +5482,33 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__contains__", 0);
 
-  /* "pe/_cy_machine.pyx":153
+  /* "pe/_cy_machine.pyx":159
  * 
  *     def __contains__(self, name: str) -> bool:
  *         return name in self._index             # <<<<<<<<<<<<<<
  * 
  *     def match(self,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_v_name, __pyx_t_1, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_v_name, __pyx_t_1, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":152
+  /* "pe/_cy_machine.pyx":158
  *         return self.grammar.start
  * 
  *     def __contains__(self, name: str) -> bool:             # <<<<<<<<<<<<<<
  *         return name in self._index
  * 
  */
 
@@ -5428,15 +5519,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":155
+/* "pe/_cy_machine.pyx":161
  *         return name in self._index
  * 
  *     def match(self,             # <<<<<<<<<<<<<<
  *               str s,
  *               int pos = 0,
  */
 
@@ -5447,40 +5538,40 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 0);
   __Pyx_XDECREF(__pyx_r);
 
-  /* "pe/_cy_machine.pyx":157
+  /* "pe/_cy_machine.pyx":163
  *     def match(self,
  *               str s,
  *               int pos = 0,             # <<<<<<<<<<<<<<
  *               flags: Flag = Flag.NONE) -> Union[Match, None]:
  *         memo: Union[Memo, None] = None
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(((int)0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(((int)0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "pe/_cy_machine.pyx":155
+  /* "pe/_cy_machine.pyx":161
  *         return name in self._index
  * 
  *     def match(self,             # <<<<<<<<<<<<<<
  *               str s,
  *               int pos = 0,
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_flags);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_flags);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_self)->__pyx_arg_flags);
   __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_1, 1, Py_None);
   __pyx_t_2 = 0;
@@ -5539,15 +5630,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_s)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 0, 2, 4, 1); __PYX_ERR(0, 155, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 0, 2, 4, 1); __PYX_ERR(0, 161, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pos);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -5555,15 +5646,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flags);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "match") < 0)) __PYX_ERR(0, 155, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "match") < 0)) __PYX_ERR(0, 161, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -5572,29 +5663,29 @@
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_self = values[0];
     __pyx_v_s = ((PyObject*)values[1]);
     if (values[2]) {
-      __pyx_v_pos = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L3_error)
+      __pyx_v_pos = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L3_error)
     } else {
       __pyx_v_pos = ((int)((int)0));
     }
     __pyx_v_flags = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("match", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 155, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("match", 0, 2, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 161, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine.MachineParser.match", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyUnicode_Type), 1, "s", 1))) __PYX_ERR(0, 156, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyUnicode_Type), 1, "s", 1))) __PYX_ERR(0, 162, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_13MachineParser_6match(__pyx_self, __pyx_v_self, __pyx_v_s, __pyx_v_pos, __pyx_v_flags);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5620,79 +5711,79 @@
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("match", 0);
 
-  /* "pe/_cy_machine.pyx":159
+  /* "pe/_cy_machine.pyx":165
  *               int pos = 0,
  *               flags: Flag = Flag.NONE) -> Union[Match, None]:
  *         memo: Union[Memo, None] = None             # <<<<<<<<<<<<<<
  *         args: List[Any] = []
  *         kwargs: List[_Binding] = []
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_memo = Py_None;
 
-  /* "pe/_cy_machine.pyx":160
+  /* "pe/_cy_machine.pyx":166
  *               flags: Flag = Flag.NONE) -> Union[Match, None]:
  *         memo: Union[Memo, None] = None
  *         args: List[Any] = []             # <<<<<<<<<<<<<<
  *         kwargs: List[_Binding] = []
  *         idx = self._index[self.start]
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_args = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":161
+  /* "pe/_cy_machine.pyx":167
  *         memo: Union[Memo, None] = None
  *         args: List[Any] = []
  *         kwargs: List[_Binding] = []             # <<<<<<<<<<<<<<
  *         idx = self._index[self.start]
  *         end = self._parser.match(idx, s, pos, args, kwargs, memo)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_kwargs = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":162
+  /* "pe/_cy_machine.pyx":168
  *         args: List[Any] = []
  *         kwargs: List[_Binding] = []
  *         idx = self._index[self.start]             # <<<<<<<<<<<<<<
  *         end = self._parser.match(idx, s, pos, args, kwargs, memo)
  *         if end < 0:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_idx = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":163
+  /* "pe/_cy_machine.pyx":169
  *         kwargs: List[_Binding] = []
  *         idx = self._index[self.start]
  *         end = self._parser.match(idx, s, pos, args, kwargs, memo)             # <<<<<<<<<<<<<<
  *         if end < 0:
  *             return None
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_parser); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_parser); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -5701,31 +5792,31 @@
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[7] = {__pyx_t_4, __pyx_v_idx, __pyx_v_s, __pyx_t_2, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 6+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 6+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
     PyObject *__pyx_temp[7] = {__pyx_t_4, __pyx_v_idx, __pyx_v_s, __pyx_t_2, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 6+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 6+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(6+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(6+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_idx);
     __Pyx_GIVEREF(__pyx_v_idx);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_idx);
@@ -5740,100 +5831,100 @@
     __Pyx_INCREF(__pyx_v_kwargs);
     __Pyx_GIVEREF(__pyx_v_kwargs);
     PyTuple_SET_ITEM(__pyx_t_6, 4+__pyx_t_5, __pyx_v_kwargs);
     __Pyx_INCREF(__pyx_v_memo);
     __Pyx_GIVEREF(__pyx_v_memo);
     PyTuple_SET_ITEM(__pyx_t_6, 5+__pyx_t_5, __pyx_v_memo);
     __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_end = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":164
+  /* "pe/_cy_machine.pyx":170
  *         idx = self._index[self.start]
  *         end = self._parser.match(idx, s, pos, args, kwargs, memo)
  *         if end < 0:             # <<<<<<<<<<<<<<
  *             return None
  *         else:
  */
-  __pyx_t_3 = PyObject_RichCompare(__pyx_v_end, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_v_end, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_7) {
 
-    /* "pe/_cy_machine.pyx":165
+    /* "pe/_cy_machine.pyx":171
  *         end = self._parser.match(idx, s, pos, args, kwargs, memo)
  *         if end < 0:
  *             return None             # <<<<<<<<<<<<<<
  *         else:
  *             return Match(
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":164
+    /* "pe/_cy_machine.pyx":170
  *         idx = self._index[self.start]
  *         end = self._parser.match(idx, s, pos, args, kwargs, memo)
  *         if end < 0:             # <<<<<<<<<<<<<<
  *             return None
  *         else:
  */
   }
 
-  /* "pe/_cy_machine.pyx":167
+  /* "pe/_cy_machine.pyx":173
  *             return None
  *         else:
  *             return Match(             # <<<<<<<<<<<<<<
  *                 s,
  *                 pos,
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "pe/_cy_machine.pyx":169
+    /* "pe/_cy_machine.pyx":175
  *             return Match(
  *                 s,
  *                 pos,             # <<<<<<<<<<<<<<
  *                 end,
  *                 self.grammar[self.start],
  */
-    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 169, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
 
-    /* "pe/_cy_machine.pyx":171
+    /* "pe/_cy_machine.pyx":177
  *                 pos,
  *                 end,
  *                 self.grammar[self.start],             # <<<<<<<<<<<<<<
  *                 args,
  *                 dict(kwargs)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_grammar); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_grammar); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 177, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pe/_cy_machine.pyx":173
+    /* "pe/_cy_machine.pyx":179
  *                 self.grammar[self.start],
  *                 args,
  *                 dict(kwargs)             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_2 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -5842,35 +5933,35 @@
         __Pyx_DECREF_SET(__pyx_t_1, function);
         __pyx_t_5 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[7] = {__pyx_t_2, __pyx_v_s, __pyx_t_6, __pyx_v_end, __pyx_t_8, __pyx_v_args, __pyx_t_4};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 6+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 6+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
       PyObject *__pyx_temp[7] = {__pyx_t_2, __pyx_v_s, __pyx_t_6, __pyx_v_end, __pyx_t_8, __pyx_v_args, __pyx_t_4};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 6+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 6+__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     {
-      __pyx_t_9 = PyTuple_New(6+__pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_9 = PyTuple_New(6+__pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 173, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (__pyx_t_2) {
         __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_2); __pyx_t_2 = NULL;
       }
       __Pyx_INCREF(__pyx_v_s);
       __Pyx_GIVEREF(__pyx_v_s);
       PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_5, __pyx_v_s);
@@ -5885,25 +5976,25 @@
       __Pyx_GIVEREF(__pyx_v_args);
       PyTuple_SET_ITEM(__pyx_t_9, 4+__pyx_t_5, __pyx_v_args);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_9, 5+__pyx_t_5, __pyx_t_4);
       __pyx_t_6 = 0;
       __pyx_t_8 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "pe/_cy_machine.pyx":155
+  /* "pe/_cy_machine.pyx":161
  *         return name in self._index
  * 
  *     def match(self,             # <<<<<<<<<<<<<<
  *               str s,
  *               int pos = 0,
  */
 
@@ -5925,15 +6016,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XDECREF(__pyx_v_end);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":180
+/* "pe/_cy_machine.pyx":186
  *     cdef list pi
  * 
  *     def __init__(self, list pi):             # <<<<<<<<<<<<<<
  *         self.pi = pi
  * 
  */
 
@@ -5962,32 +6053,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pi)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 180, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 186, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_pi = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 180, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 186, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine._Parser.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pi), (&PyList_Type), 1, "pi", 1))) __PYX_ERR(0, 180, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pi), (&PyList_Type), 1, "pi", 1))) __PYX_ERR(0, 186, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_7_Parser___init__(((struct __pyx_obj_2pe_11_cy_machine__Parser *)__pyx_v_self), __pyx_v_pi);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -5996,42 +6087,42 @@
 }
 
 static int __pyx_pf_2pe_11_cy_machine_7_Parser___init__(struct __pyx_obj_2pe_11_cy_machine__Parser *__pyx_v_self, PyObject *__pyx_v_pi) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pe/_cy_machine.pyx":181
+  /* "pe/_cy_machine.pyx":187
  * 
  *     def __init__(self, list pi):
  *         self.pi = pi             # <<<<<<<<<<<<<<
  * 
  *     cpdef int match(
  */
   __Pyx_INCREF(__pyx_v_pi);
   __Pyx_GIVEREF(__pyx_v_pi);
   __Pyx_GOTREF(__pyx_v_self->pi);
   __Pyx_DECREF(__pyx_v_self->pi);
   __pyx_v_self->pi = __pyx_v_pi;
 
-  /* "pe/_cy_machine.pyx":180
+  /* "pe/_cy_machine.pyx":186
  *     cdef list pi
  * 
  *     def __init__(self, list pi):             # <<<<<<<<<<<<<<
  *         self.pi = pi
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":183
+/* "pe/_cy_machine.pyx":189
  *         self.pi = pi
  * 
  *     cpdef int match(             # <<<<<<<<<<<<<<
  *         self,
  *         int idx,
  */
 
@@ -6068,20 +6159,20 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_2pe_11_cy_machine_7_Parser_3match)) {
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 183, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
           if (likely(__pyx_t_6)) {
@@ -6091,33 +6182,33 @@
             __Pyx_DECREF_SET(__pyx_t_5, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[7] = {__pyx_t_6, __pyx_t_3, __pyx_v_s, __pyx_t_4, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo};
-          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 6+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 6+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
           PyObject *__pyx_temp[7] = {__pyx_t_6, __pyx_t_3, __pyx_v_s, __pyx_t_4, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo};
-          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 6+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 6+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         } else
         #endif
         {
-          __pyx_t_8 = PyTuple_New(6+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 183, __pyx_L1_error)
+          __pyx_t_8 = PyTuple_New(6+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 189, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (__pyx_t_6) {
             __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
           }
           __Pyx_GIVEREF(__pyx_t_3);
           PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
           __Pyx_INCREF(__pyx_v_s);
@@ -6132,20 +6223,20 @@
           __Pyx_GIVEREF(__pyx_v_kwargs);
           PyTuple_SET_ITEM(__pyx_t_8, 4+__pyx_t_7, __pyx_v_kwargs);
           __Pyx_INCREF(__pyx_v_memo);
           __Pyx_GIVEREF(__pyx_v_memo);
           PyTuple_SET_ITEM(__pyx_t_8, 5+__pyx_t_7, __pyx_v_memo);
           __pyx_t_3 = 0;
           __pyx_t_4 = 0;
-          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_7;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -6156,94 +6247,94 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "pe/_cy_machine.pyx":193
+  /* "pe/_cy_machine.pyx":199
  *     ) except -2:
  *         cdef State* state
  *         cdef int retval = -1             # <<<<<<<<<<<<<<
  *         state = push(0, 0, -1, 0, 0, NULL)     # failure (top backtrack entry)
  *         state = push(-1, -1, -1, 0, 0, state)  # success
  */
   __pyx_v_retval = -1;
 
-  /* "pe/_cy_machine.pyx":194
+  /* "pe/_cy_machine.pyx":200
  *         cdef State* state
  *         cdef int retval = -1
  *         state = push(0, 0, -1, 0, 0, NULL)     # failure (top backtrack entry)             # <<<<<<<<<<<<<<
  *         state = push(-1, -1, -1, 0, 0, state)  # success
  *         try:
  */
-  __pyx_t_9 = __pyx_f_2pe_11_cy_machine_push(0, 0, -1, 0, 0, NULL); if (unlikely(__pyx_t_9 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 194, __pyx_L1_error)
+  __pyx_t_9 = __pyx_f_2pe_11_cy_machine_push(0, 0, -1, 0, 0, NULL); if (unlikely(__pyx_t_9 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 200, __pyx_L1_error)
   __pyx_v_state = __pyx_t_9;
 
-  /* "pe/_cy_machine.pyx":195
+  /* "pe/_cy_machine.pyx":201
  *         cdef int retval = -1
  *         state = push(0, 0, -1, 0, 0, NULL)     # failure (top backtrack entry)
  *         state = push(-1, -1, -1, 0, 0, state)  # success             # <<<<<<<<<<<<<<
  *         try:
  *             state = self._match(idx, s, pos, args, kwargs, memo, state)
  */
-  __pyx_t_9 = __pyx_f_2pe_11_cy_machine_push(-1, -1, -1, 0, 0, __pyx_v_state); if (unlikely(__pyx_t_9 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_9 = __pyx_f_2pe_11_cy_machine_push(-1, -1, -1, 0, 0, __pyx_v_state); if (unlikely(__pyx_t_9 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 201, __pyx_L1_error)
   __pyx_v_state = __pyx_t_9;
 
-  /* "pe/_cy_machine.pyx":196
+  /* "pe/_cy_machine.pyx":202
  *         state = push(0, 0, -1, 0, 0, NULL)     # failure (top backtrack entry)
  *         state = push(-1, -1, -1, 0, 0, state)  # success
  *         try:             # <<<<<<<<<<<<<<
  *             state = self._match(idx, s, pos, args, kwargs, memo, state)
  *             retval = state.pos
  */
   /*try:*/ {
 
-    /* "pe/_cy_machine.pyx":197
+    /* "pe/_cy_machine.pyx":203
  *         state = push(-1, -1, -1, 0, 0, state)  # success
  *         try:
  *             state = self._match(idx, s, pos, args, kwargs, memo, state)             # <<<<<<<<<<<<<<
  *             retval = state.pos
  *         finally:
  */
-    __pyx_t_9 = ((struct __pyx_vtabstruct_2pe_11_cy_machine__Parser *)__pyx_v_self->__pyx_vtab)->_match(__pyx_v_self, __pyx_v_idx, __pyx_v_s, __pyx_v_pos, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo, __pyx_v_state); if (unlikely(__pyx_t_9 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 197, __pyx_L4_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_2pe_11_cy_machine__Parser *)__pyx_v_self->__pyx_vtab)->_match(__pyx_v_self, __pyx_v_idx, __pyx_v_s, __pyx_v_pos, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo, __pyx_v_state); if (unlikely(__pyx_t_9 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 203, __pyx_L4_error)
     __pyx_v_state = __pyx_t_9;
 
-    /* "pe/_cy_machine.pyx":198
+    /* "pe/_cy_machine.pyx":204
  *         try:
  *             state = self._match(idx, s, pos, args, kwargs, memo, state)
  *             retval = state.pos             # <<<<<<<<<<<<<<
  *         finally:
  *             while state:
  */
     __pyx_t_7 = __pyx_v_state->pos;
     __pyx_v_retval = __pyx_t_7;
   }
 
-  /* "pe/_cy_machine.pyx":200
+  /* "pe/_cy_machine.pyx":206
  *             retval = state.pos
  *         finally:
  *             while state:             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *         return retval
  */
   /*finally:*/ {
     /*normal exit:*/{
       while (1) {
         __pyx_t_10 = (__pyx_v_state != 0);
         if (!__pyx_t_10) break;
 
-        /* "pe/_cy_machine.pyx":201
+        /* "pe/_cy_machine.pyx":207
  *         finally:
  *             while state:
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *         return retval
  * 
  */
-        __pyx_t_9 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_9 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
+        __pyx_t_9 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_9 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L1_error)
         __pyx_v_state = __pyx_t_9;
       }
       goto __pyx_L5;
     }
     __pyx_L4_error:;
     /*exception exit:*/{
       __Pyx_PyThreadState_declare
@@ -6263,33 +6354,33 @@
       __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_XGOTREF(__pyx_t_16);
       __Pyx_XGOTREF(__pyx_t_17);
       __Pyx_XGOTREF(__pyx_t_18);
       __pyx_t_7 = __pyx_lineno; __pyx_t_11 = __pyx_clineno; __pyx_t_12 = __pyx_filename;
       {
 
-        /* "pe/_cy_machine.pyx":200
+        /* "pe/_cy_machine.pyx":206
  *             retval = state.pos
  *         finally:
  *             while state:             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *         return retval
  */
         while (1) {
           __pyx_t_10 = (__pyx_v_state != 0);
           if (!__pyx_t_10) break;
 
-          /* "pe/_cy_machine.pyx":201
+          /* "pe/_cy_machine.pyx":207
  *         finally:
  *             while state:
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *         return retval
  * 
  */
-          __pyx_t_9 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_9 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L9_error)
+          __pyx_t_9 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_9 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 207, __pyx_L9_error)
           __pyx_v_state = __pyx_t_9;
         }
       }
       if (PY_MAJOR_VERSION >= 3) {
         __Pyx_XGIVEREF(__pyx_t_16);
         __Pyx_XGIVEREF(__pyx_t_17);
         __Pyx_XGIVEREF(__pyx_t_18);
@@ -6314,25 +6405,25 @@
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
       __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0;
       goto __pyx_L1_error;
     }
     __pyx_L5:;
   }
 
-  /* "pe/_cy_machine.pyx":202
+  /* "pe/_cy_machine.pyx":208
  *             while state:
  *                 state = pop(state)
  *         return retval             # <<<<<<<<<<<<<<
  * 
  *     cdef State* _match(
  */
   __pyx_r = __pyx_v_retval;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":183
+  /* "pe/_cy_machine.pyx":189
  *         self.pi = pi
  * 
  *     cpdef int match(             # <<<<<<<<<<<<<<
  *         self,
  *         int idx,
  */
 
@@ -6394,73 +6485,73 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_idx)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_s)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 1); __PYX_ERR(0, 183, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 1); __PYX_ERR(0, 189, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 2); __PYX_ERR(0, 183, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 2); __PYX_ERR(0, 189, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_args)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 3); __PYX_ERR(0, 183, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 3); __PYX_ERR(0, 189, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kwargs)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 4); __PYX_ERR(0, 183, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 4); __PYX_ERR(0, 189, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_memo)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 5); __PYX_ERR(0, 183, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 5); __PYX_ERR(0, 189, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "match") < 0)) __PYX_ERR(0, 183, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "match") < 0)) __PYX_ERR(0, 189, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
     }
-    __pyx_v_idx = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_idx == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 185, __pyx_L3_error)
+    __pyx_v_idx = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_idx == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 191, __pyx_L3_error)
     __pyx_v_s = ((PyObject*)values[1]);
-    __pyx_v_pos = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L3_error)
+    __pyx_v_pos = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 193, __pyx_L3_error)
     __pyx_v_args = ((PyObject*)values[3]);
     __pyx_v_kwargs = ((PyObject*)values[4]);
     __pyx_v_memo = ((PyObject*)values[5]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 183, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 189, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine._Parser.match", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyUnicode_Type), 1, "s", 1))) __PYX_ERR(0, 186, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_args), (&PyList_Type), 1, "args", 1))) __PYX_ERR(0, 188, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kwargs), (&PyList_Type), 1, "kwargs", 1))) __PYX_ERR(0, 189, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_memo), (&PyDict_Type), 1, "memo", 1))) __PYX_ERR(0, 190, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyUnicode_Type), 1, "s", 1))) __PYX_ERR(0, 192, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_args), (&PyList_Type), 1, "args", 1))) __PYX_ERR(0, 194, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kwargs), (&PyList_Type), 1, "kwargs", 1))) __PYX_ERR(0, 195, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_memo), (&PyDict_Type), 1, "memo", 1))) __PYX_ERR(0, 196, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_7_Parser_2match(((struct __pyx_obj_2pe_11_cy_machine__Parser *)__pyx_v_self), __pyx_v_idx, __pyx_v_s, __pyx_v_pos, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -6474,16 +6565,16 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("match", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_2pe_11_cy_machine_7_Parser_match(__pyx_v_self, __pyx_v_idx, __pyx_v_s, __pyx_v_pos, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo, 1); if (unlikely(__pyx_t_1 == ((int)-2))) __PYX_ERR(0, 183, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_2pe_11_cy_machine_7_Parser_match(__pyx_v_self, __pyx_v_idx, __pyx_v_s, __pyx_v_pos, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo, 1); if (unlikely(__pyx_t_1 == ((int)-2))) __PYX_ERR(0, 189, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6492,15 +6583,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":204
+/* "pe/_cy_machine.pyx":210
  *         return retval
  * 
  *     cdef State* _match(             # <<<<<<<<<<<<<<
  *         self,
  *         int idx,
  */
 
@@ -6529,714 +6620,714 @@
   PyObject *__pyx_t_15 = NULL;
   PyObject *(*__pyx_t_16)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_match", 0);
 
-  /* "pe/_cy_machine.pyx":214
+  /* "pe/_cy_machine.pyx":220
  *         State* state,
  *     ) except NULL:
  *         if s is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         if args is None:
  */
   __pyx_t_1 = (__pyx_v_s == ((PyObject*)Py_None));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "pe/_cy_machine.pyx":215
+    /* "pe/_cy_machine.pyx":221
  *     ) except NULL:
  *         if s is None:
  *             raise TypeError             # <<<<<<<<<<<<<<
  *         if args is None:
  *             raise TypeError
  */
     __Pyx_Raise(__pyx_builtin_TypeError, 0, 0, 0);
-    __PYX_ERR(0, 215, __pyx_L1_error)
+    __PYX_ERR(0, 221, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":214
+    /* "pe/_cy_machine.pyx":220
  *         State* state,
  *     ) except NULL:
  *         if s is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         if args is None:
  */
   }
 
-  /* "pe/_cy_machine.pyx":216
+  /* "pe/_cy_machine.pyx":222
  *         if s is None:
  *             raise TypeError
  *         if args is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         if kwargs is None:
  */
   __pyx_t_2 = (__pyx_v_args == ((PyObject*)Py_None));
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pe/_cy_machine.pyx":217
+    /* "pe/_cy_machine.pyx":223
  *             raise TypeError
  *         if args is None:
  *             raise TypeError             # <<<<<<<<<<<<<<
  *         if kwargs is None:
  *             raise TypeError
  */
     __Pyx_Raise(__pyx_builtin_TypeError, 0, 0, 0);
-    __PYX_ERR(0, 217, __pyx_L1_error)
+    __PYX_ERR(0, 223, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":216
+    /* "pe/_cy_machine.pyx":222
  *         if s is None:
  *             raise TypeError
  *         if args is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         if kwargs is None:
  */
   }
 
-  /* "pe/_cy_machine.pyx":218
+  /* "pe/_cy_machine.pyx":224
  *         if args is None:
  *             raise TypeError
  *         if kwargs is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         # lookup optimizations
  */
   __pyx_t_1 = (__pyx_v_kwargs == ((PyObject*)Py_None));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "pe/_cy_machine.pyx":219
+    /* "pe/_cy_machine.pyx":225
  *             raise TypeError
  *         if kwargs is None:
  *             raise TypeError             # <<<<<<<<<<<<<<
  *         # lookup optimizations
  *         pi = self.pi
  */
     __Pyx_Raise(__pyx_builtin_TypeError, 0, 0, 0);
-    __PYX_ERR(0, 219, __pyx_L1_error)
+    __PYX_ERR(0, 225, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":218
+    /* "pe/_cy_machine.pyx":224
  *         if args is None:
  *             raise TypeError
  *         if kwargs is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         # lookup optimizations
  */
   }
 
-  /* "pe/_cy_machine.pyx":221
+  /* "pe/_cy_machine.pyx":227
  *             raise TypeError
  *         # lookup optimizations
  *         pi = self.pi             # <<<<<<<<<<<<<<
  *         # cdef OpCode opcode
  *         cdef int slen = len(s)
  */
   __pyx_t_3 = __pyx_v_self->pi;
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_pi = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":223
+  /* "pe/_cy_machine.pyx":229
  *         pi = self.pi
  *         # cdef OpCode opcode
  *         cdef int slen = len(s)             # <<<<<<<<<<<<<<
  *         cdef Instruction instr
  *         while state:
  */
   if (unlikely(__pyx_v_s == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 223, __pyx_L1_error)
+    __PYX_ERR(0, 229, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_s); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_s); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 229, __pyx_L1_error)
   __pyx_v_slen = __pyx_t_4;
 
-  /* "pe/_cy_machine.pyx":225
+  /* "pe/_cy_machine.pyx":231
  *         cdef int slen = len(s)
  *         cdef Instruction instr
  *         while state:             # <<<<<<<<<<<<<<
  *             instr = pi[idx]
  * 
  */
   while (1) {
     __pyx_t_2 = (__pyx_v_state != 0);
     if (!__pyx_t_2) break;
 
-    /* "pe/_cy_machine.pyx":226
+    /* "pe/_cy_machine.pyx":232
  *         cdef Instruction instr
  *         while state:
  *             instr = pi[idx]             # <<<<<<<<<<<<<<
  * 
  *             if instr.marking:
  */
     if (unlikely(__pyx_v_pi == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 226, __pyx_L1_error)
+      __PYX_ERR(0, 232, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_pi, __pyx_v_idx, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 226, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_pi, __pyx_v_idx, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_2pe_11_cy_machine_Instruction))))) __PYX_ERR(0, 226, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_2pe_11_cy_machine_Instruction))))) __PYX_ERR(0, 232, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_instr, ((struct __pyx_obj_2pe_11_cy_machine_Instruction *)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "pe/_cy_machine.pyx":228
+    /* "pe/_cy_machine.pyx":234
  *             instr = pi[idx]
  * 
  *             if instr.marking:             # <<<<<<<<<<<<<<
  *                 state = push(0, -1, pos, len(args), len(kwargs), state)
  * 
  */
     __pyx_t_2 = (__pyx_v_instr->marking != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":229
+      /* "pe/_cy_machine.pyx":235
  * 
  *             if instr.marking:
  *                 state = push(0, -1, pos, len(args), len(kwargs), state)             # <<<<<<<<<<<<<<
  * 
  *             if instr.opcode == SCAN:
  */
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 229, __pyx_L1_error)
+        __PYX_ERR(0, 235, __pyx_L1_error)
       }
-      __pyx_t_4 = PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 229, __pyx_L1_error)
+      __pyx_t_4 = PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
       if (unlikely(__pyx_v_kwargs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 229, __pyx_L1_error)
+        __PYX_ERR(0, 235, __pyx_L1_error)
       }
-      __pyx_t_5 = PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 229, __pyx_L1_error)
-      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_push(0, -1, __pyx_v_pos, __pyx_t_4, __pyx_t_5, __pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 229, __pyx_L1_error)
+      __pyx_t_5 = PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 235, __pyx_L1_error)
+      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_push(0, -1, __pyx_v_pos, __pyx_t_4, __pyx_t_5, __pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 235, __pyx_L1_error)
       __pyx_v_state = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":228
+      /* "pe/_cy_machine.pyx":234
  *             instr = pi[idx]
  * 
  *             if instr.marking:             # <<<<<<<<<<<<<<
  *                 state = push(0, -1, pos, len(args), len(kwargs), state)
  * 
  */
     }
 
-    /* "pe/_cy_machine.pyx":231
+    /* "pe/_cy_machine.pyx":237
  *                 state = push(0, -1, pos, len(args), len(kwargs), state)
  * 
  *             if instr.opcode == SCAN:             # <<<<<<<<<<<<<<
  *                 pos = instr.scanner._scan(s, pos, slen)
  *                 if pos < 0:
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_SCAN) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":232
+      /* "pe/_cy_machine.pyx":238
  * 
  *             if instr.opcode == SCAN:
  *                 pos = instr.scanner._scan(s, pos, slen)             # <<<<<<<<<<<<<<
  *                 if pos < 0:
  *                     idx = FAILURE
  */
-      __pyx_t_7 = ((struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner *)__pyx_v_instr->scanner->__pyx_vtab)->_scan(__pyx_v_instr->scanner, __pyx_v_s, __pyx_v_pos, __pyx_v_slen); if (unlikely(__pyx_t_7 == ((int)-2))) __PYX_ERR(0, 232, __pyx_L1_error)
+      __pyx_t_7 = ((struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner *)__pyx_v_instr->scanner->__pyx_vtab)->_scan(__pyx_v_instr->scanner, __pyx_v_s, __pyx_v_pos, __pyx_v_slen); if (unlikely(__pyx_t_7 == ((int)-2))) __PYX_ERR(0, 238, __pyx_L1_error)
       __pyx_v_pos = __pyx_t_7;
 
-      /* "pe/_cy_machine.pyx":233
+      /* "pe/_cy_machine.pyx":239
  *             if instr.opcode == SCAN:
  *                 pos = instr.scanner._scan(s, pos, slen)
  *                 if pos < 0:             # <<<<<<<<<<<<<<
  *                     idx = FAILURE
  * 
  */
       __pyx_t_2 = ((__pyx_v_pos < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "pe/_cy_machine.pyx":234
+        /* "pe/_cy_machine.pyx":240
  *                 pos = instr.scanner._scan(s, pos, slen)
  *                 if pos < 0:
  *                     idx = FAILURE             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == BRANCH:
  */
         __pyx_v_idx = -1;
 
-        /* "pe/_cy_machine.pyx":233
+        /* "pe/_cy_machine.pyx":239
  *             if instr.opcode == SCAN:
  *                 pos = instr.scanner._scan(s, pos, slen)
  *                 if pos < 0:             # <<<<<<<<<<<<<<
  *                     idx = FAILURE
  * 
  */
       }
 
-      /* "pe/_cy_machine.pyx":231
+      /* "pe/_cy_machine.pyx":237
  *                 state = push(0, -1, pos, len(args), len(kwargs), state)
  * 
  *             if instr.opcode == SCAN:             # <<<<<<<<<<<<<<
  *                 pos = instr.scanner._scan(s, pos, slen)
  *                 if pos < 0:
  */
       goto __pyx_L9;
     }
 
-    /* "pe/_cy_machine.pyx":236
+    /* "pe/_cy_machine.pyx":242
  *                     idx = FAILURE
  * 
  *             elif instr.opcode == BRANCH:             # <<<<<<<<<<<<<<
  *                 state = push(idx + instr.oploc, pos, -1, len(args), len(kwargs), state)
  *                 idx += 1
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_BRANCH) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":237
+      /* "pe/_cy_machine.pyx":243
  * 
  *             elif instr.opcode == BRANCH:
  *                 state = push(idx + instr.oploc, pos, -1, len(args), len(kwargs), state)             # <<<<<<<<<<<<<<
  *                 idx += 1
  *                 continue
  */
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 237, __pyx_L1_error)
+        __PYX_ERR(0, 243, __pyx_L1_error)
       }
-      __pyx_t_5 = PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 237, __pyx_L1_error)
+      __pyx_t_5 = PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 243, __pyx_L1_error)
       if (unlikely(__pyx_v_kwargs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 237, __pyx_L1_error)
+        __PYX_ERR(0, 243, __pyx_L1_error)
       }
-      __pyx_t_4 = PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 237, __pyx_L1_error)
-      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_push((__pyx_v_idx + __pyx_v_instr->oploc), __pyx_v_pos, -1, __pyx_t_5, __pyx_t_4, __pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 237, __pyx_L1_error)
+      __pyx_t_4 = PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 243, __pyx_L1_error)
+      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_push((__pyx_v_idx + __pyx_v_instr->oploc), __pyx_v_pos, -1, __pyx_t_5, __pyx_t_4, __pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 243, __pyx_L1_error)
       __pyx_v_state = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":238
+      /* "pe/_cy_machine.pyx":244
  *             elif instr.opcode == BRANCH:
  *                 state = push(idx + instr.oploc, pos, -1, len(args), len(kwargs), state)
  *                 idx += 1             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_v_idx = (__pyx_v_idx + 1);
 
-      /* "pe/_cy_machine.pyx":239
+      /* "pe/_cy_machine.pyx":245
  *                 state = push(idx + instr.oploc, pos, -1, len(args), len(kwargs), state)
  *                 idx += 1
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == CALL:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":236
+      /* "pe/_cy_machine.pyx":242
  *                     idx = FAILURE
  * 
  *             elif instr.opcode == BRANCH:             # <<<<<<<<<<<<<<
  *                 state = push(idx + instr.oploc, pos, -1, len(args), len(kwargs), state)
  *                 idx += 1
  */
     }
 
-    /* "pe/_cy_machine.pyx":241
+    /* "pe/_cy_machine.pyx":247
  *                 continue
  * 
  *             elif instr.opcode == CALL:             # <<<<<<<<<<<<<<
  *                 state = push(idx + 1, -1, -1, -1, -1, state)
  *                 idx = instr.oploc
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_CALL) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":242
+      /* "pe/_cy_machine.pyx":248
  * 
  *             elif instr.opcode == CALL:
  *                 state = push(idx + 1, -1, -1, -1, -1, state)             # <<<<<<<<<<<<<<
  *                 idx = instr.oploc
  *                 continue
  */
-      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_push((__pyx_v_idx + 1), -1, -1, -1, -1, __pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 242, __pyx_L1_error)
+      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_push((__pyx_v_idx + 1), -1, -1, -1, -1, __pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 248, __pyx_L1_error)
       __pyx_v_state = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":243
+      /* "pe/_cy_machine.pyx":249
  *             elif instr.opcode == CALL:
  *                 state = push(idx + 1, -1, -1, -1, -1, state)
  *                 idx = instr.oploc             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_t_8 = __pyx_v_instr->oploc;
       __pyx_v_idx = __pyx_t_8;
 
-      /* "pe/_cy_machine.pyx":244
+      /* "pe/_cy_machine.pyx":250
  *                 state = push(idx + 1, -1, -1, -1, -1, state)
  *                 idx = instr.oploc
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == COMMIT:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":241
+      /* "pe/_cy_machine.pyx":247
  *                 continue
  * 
  *             elif instr.opcode == CALL:             # <<<<<<<<<<<<<<
  *                 state = push(idx + 1, -1, -1, -1, -1, state)
  *                 idx = instr.oploc
  */
     }
 
-    /* "pe/_cy_machine.pyx":246
+    /* "pe/_cy_machine.pyx":252
  *                 continue
  * 
  *             elif instr.opcode == COMMIT:             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *                 idx += instr.oploc
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_COMMIT) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":247
+      /* "pe/_cy_machine.pyx":253
  * 
  *             elif instr.opcode == COMMIT:
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *                 idx += instr.oploc
  *                 continue
  */
-      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L1_error)
+      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 253, __pyx_L1_error)
       __pyx_v_state = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":248
+      /* "pe/_cy_machine.pyx":254
  *             elif instr.opcode == COMMIT:
  *                 state = pop(state)
  *                 idx += instr.oploc             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_v_idx = (__pyx_v_idx + __pyx_v_instr->oploc);
 
-      /* "pe/_cy_machine.pyx":249
+      /* "pe/_cy_machine.pyx":255
  *                 state = pop(state)
  *                 idx += instr.oploc
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == UPDATE:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":246
+      /* "pe/_cy_machine.pyx":252
  *                 continue
  * 
  *             elif instr.opcode == COMMIT:             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *                 idx += instr.oploc
  */
     }
 
-    /* "pe/_cy_machine.pyx":251
+    /* "pe/_cy_machine.pyx":257
  *                 continue
  * 
  *             elif instr.opcode == UPDATE:             # <<<<<<<<<<<<<<
  *                 state.pos = pos
  *                 state.argidx = len(args)
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_UPDATE) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":252
+      /* "pe/_cy_machine.pyx":258
  * 
  *             elif instr.opcode == UPDATE:
  *                 state.pos = pos             # <<<<<<<<<<<<<<
  *                 state.argidx = len(args)
  *                 state.kwidx = len(kwargs)
  */
       __pyx_v_state->pos = __pyx_v_pos;
 
-      /* "pe/_cy_machine.pyx":253
+      /* "pe/_cy_machine.pyx":259
  *             elif instr.opcode == UPDATE:
  *                 state.pos = pos
  *                 state.argidx = len(args)             # <<<<<<<<<<<<<<
  *                 state.kwidx = len(kwargs)
  *                 idx += instr.oploc
  */
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 253, __pyx_L1_error)
+        __PYX_ERR(0, 259, __pyx_L1_error)
       }
-      __pyx_t_4 = PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 253, __pyx_L1_error)
+      __pyx_t_4 = PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 259, __pyx_L1_error)
       __pyx_v_state->argidx = __pyx_t_4;
 
-      /* "pe/_cy_machine.pyx":254
+      /* "pe/_cy_machine.pyx":260
  *                 state.pos = pos
  *                 state.argidx = len(args)
  *                 state.kwidx = len(kwargs)             # <<<<<<<<<<<<<<
  *                 idx += instr.oploc
  *                 continue
  */
       if (unlikely(__pyx_v_kwargs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 254, __pyx_L1_error)
+        __PYX_ERR(0, 260, __pyx_L1_error)
       }
-      __pyx_t_4 = PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 254, __pyx_L1_error)
+      __pyx_t_4 = PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 260, __pyx_L1_error)
       __pyx_v_state->kwidx = __pyx_t_4;
 
-      /* "pe/_cy_machine.pyx":255
+      /* "pe/_cy_machine.pyx":261
  *                 state.argidx = len(args)
  *                 state.kwidx = len(kwargs)
  *                 idx += instr.oploc             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_v_idx = (__pyx_v_idx + __pyx_v_instr->oploc);
 
-      /* "pe/_cy_machine.pyx":256
+      /* "pe/_cy_machine.pyx":262
  *                 state.kwidx = len(kwargs)
  *                 idx += instr.oploc
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == RESTORE:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":251
+      /* "pe/_cy_machine.pyx":257
  *                 continue
  * 
  *             elif instr.opcode == UPDATE:             # <<<<<<<<<<<<<<
  *                 state.pos = pos
  *                 state.argidx = len(args)
  */
     }
 
-    /* "pe/_cy_machine.pyx":258
+    /* "pe/_cy_machine.pyx":264
  *                 continue
  * 
  *             elif instr.opcode == RESTORE:             # <<<<<<<<<<<<<<
  *                 pos = state.pos
  *                 state = pop(state)
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_RESTORE) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":259
+      /* "pe/_cy_machine.pyx":265
  * 
  *             elif instr.opcode == RESTORE:
  *                 pos = state.pos             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *                 idx += instr.oploc
  */
       __pyx_t_7 = __pyx_v_state->pos;
       __pyx_v_pos = __pyx_t_7;
 
-      /* "pe/_cy_machine.pyx":260
+      /* "pe/_cy_machine.pyx":266
  *             elif instr.opcode == RESTORE:
  *                 pos = state.pos
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *                 idx += instr.oploc
  *                 continue
  */
-      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 260, __pyx_L1_error)
+      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 266, __pyx_L1_error)
       __pyx_v_state = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":261
+      /* "pe/_cy_machine.pyx":267
  *                 pos = state.pos
  *                 state = pop(state)
  *                 idx += instr.oploc             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_v_idx = (__pyx_v_idx + __pyx_v_instr->oploc);
 
-      /* "pe/_cy_machine.pyx":262
+      /* "pe/_cy_machine.pyx":268
  *                 state = pop(state)
  *                 idx += instr.oploc
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == FAILTWICE:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":258
+      /* "pe/_cy_machine.pyx":264
  *                 continue
  * 
  *             elif instr.opcode == RESTORE:             # <<<<<<<<<<<<<<
  *                 pos = state.pos
  *                 state = pop(state)
  */
     }
 
-    /* "pe/_cy_machine.pyx":264
+    /* "pe/_cy_machine.pyx":270
  *                 continue
  * 
  *             elif instr.opcode == FAILTWICE:             # <<<<<<<<<<<<<<
  *                 pos = state.pos
  *                 state = pop(state)
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_FAILTWICE) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":265
+      /* "pe/_cy_machine.pyx":271
  * 
  *             elif instr.opcode == FAILTWICE:
  *                 pos = state.pos             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *                 idx = FAILURE
  */
       __pyx_t_7 = __pyx_v_state->pos;
       __pyx_v_pos = __pyx_t_7;
 
-      /* "pe/_cy_machine.pyx":266
+      /* "pe/_cy_machine.pyx":272
  *             elif instr.opcode == FAILTWICE:
  *                 pos = state.pos
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *                 idx = FAILURE
  * 
  */
-      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 266, __pyx_L1_error)
+      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 272, __pyx_L1_error)
       __pyx_v_state = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":267
+      /* "pe/_cy_machine.pyx":273
  *                 pos = state.pos
  *                 state = pop(state)
  *                 idx = FAILURE             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == RETURN:
  */
       __pyx_v_idx = -1;
 
-      /* "pe/_cy_machine.pyx":264
+      /* "pe/_cy_machine.pyx":270
  *                 continue
  * 
  *             elif instr.opcode == FAILTWICE:             # <<<<<<<<<<<<<<
  *                 pos = state.pos
  *                 state = pop(state)
  */
       goto __pyx_L9;
     }
 
-    /* "pe/_cy_machine.pyx":269
+    /* "pe/_cy_machine.pyx":275
  *                 idx = FAILURE
  * 
  *             elif instr.opcode == RETURN:             # <<<<<<<<<<<<<<
  *                 idx = state.opidx
  *                 state = pop(state)
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_RETURN) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":270
+      /* "pe/_cy_machine.pyx":276
  * 
  *             elif instr.opcode == RETURN:
  *                 idx = state.opidx             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *                 continue
  */
       __pyx_t_7 = __pyx_v_state->opidx;
       __pyx_v_idx = __pyx_t_7;
 
-      /* "pe/_cy_machine.pyx":271
+      /* "pe/_cy_machine.pyx":277
  *             elif instr.opcode == RETURN:
  *                 idx = state.opidx
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
-      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 271, __pyx_L1_error)
+      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 277, __pyx_L1_error)
       __pyx_v_state = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":272
+      /* "pe/_cy_machine.pyx":278
  *                 idx = state.opidx
  *                 state = pop(state)
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == PASS:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":269
+      /* "pe/_cy_machine.pyx":275
  *                 idx = FAILURE
  * 
  *             elif instr.opcode == RETURN:             # <<<<<<<<<<<<<<
  *                 idx = state.opidx
  *                 state = pop(state)
  */
     }
 
-    /* "pe/_cy_machine.pyx":274
+    /* "pe/_cy_machine.pyx":280
  *                 continue
  * 
  *             elif instr.opcode == PASS:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_PASS) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":275
+      /* "pe/_cy_machine.pyx":281
  * 
  *             elif instr.opcode == PASS:
  *                 break             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == FAIL:
  */
       goto __pyx_L7_break;
 
-      /* "pe/_cy_machine.pyx":274
+      /* "pe/_cy_machine.pyx":280
  *                 continue
  * 
  *             elif instr.opcode == PASS:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
     }
 
-    /* "pe/_cy_machine.pyx":277
+    /* "pe/_cy_machine.pyx":283
  *                 break
  * 
  *             elif instr.opcode == FAIL:             # <<<<<<<<<<<<<<
  *                 idx = FAILURE
  * 
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_FAIL) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":278
+      /* "pe/_cy_machine.pyx":284
  * 
  *             elif instr.opcode == FAIL:
  *                 idx = FAILURE             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode != NOOP:
  */
       __pyx_v_idx = -1;
 
-      /* "pe/_cy_machine.pyx":277
+      /* "pe/_cy_machine.pyx":283
  *                 break
  * 
  *             elif instr.opcode == FAIL:             # <<<<<<<<<<<<<<
  *                 idx = FAILURE
  * 
  */
       goto __pyx_L9;
     }
 
-    /* "pe/_cy_machine.pyx":280
+    /* "pe/_cy_machine.pyx":286
  *                 idx = FAILURE
  * 
  *             elif instr.opcode != NOOP:             # <<<<<<<<<<<<<<
  *                 raise Error(f'invalid operation: {instr.opcode}')
  * 
  */
     __pyx_t_2 = ((__pyx_v_instr->opcode != __pyx_e_2pe_11_cy_machine_NOOP) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "pe/_cy_machine.pyx":281
+      /* "pe/_cy_machine.pyx":287
  * 
  *             elif instr.opcode != NOOP:
  *                 raise Error(f'invalid operation: {instr.opcode}')             # <<<<<<<<<<<<<<
  * 
  *             if idx == FAILURE:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_Error); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_Error); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 287, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = __Pyx_PyUnicode_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_v_instr->opcode, 0, ' ', 'd'); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyUnicode_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_v_instr->opcode, 0, ' ', 'd'); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 287, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_invalid_operation, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_invalid_operation, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 287, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -7244,42 +7335,42 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_3 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 281, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 287, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(0, 281, __pyx_L1_error)
+      __PYX_ERR(0, 287, __pyx_L1_error)
 
-      /* "pe/_cy_machine.pyx":280
+      /* "pe/_cy_machine.pyx":286
  *                 idx = FAILURE
  * 
  *             elif instr.opcode != NOOP:             # <<<<<<<<<<<<<<
  *                 raise Error(f'invalid operation: {instr.opcode}')
  * 
  */
     }
     __pyx_L9:;
 
-    /* "pe/_cy_machine.pyx":283
+    /* "pe/_cy_machine.pyx":289
  *                 raise Error(f'invalid operation: {instr.opcode}')
  * 
  *             if idx == FAILURE:             # <<<<<<<<<<<<<<
  *                 # pos is >= 0 only for backtracking entries
  *                 while state and state.pos < 0:
  */
     __pyx_t_2 = ((__pyx_v_idx == -1L) != 0);
     if (__pyx_t_2) {
 
-      /* "pe/_cy_machine.pyx":285
+      /* "pe/_cy_machine.pyx":291
  *             if idx == FAILURE:
  *                 # pos is >= 0 only for backtracking entries
  *                 while state and state.pos < 0:             # <<<<<<<<<<<<<<
  *                     state = pop(state)
  *                 idx = state.opidx
  */
       while (1) {
@@ -7290,246 +7381,246 @@
           goto __pyx_L14_bool_binop_done;
         }
         __pyx_t_1 = ((__pyx_v_state->pos < 0) != 0);
         __pyx_t_2 = __pyx_t_1;
         __pyx_L14_bool_binop_done:;
         if (!__pyx_t_2) break;
 
-        /* "pe/_cy_machine.pyx":286
+        /* "pe/_cy_machine.pyx":292
  *                 # pos is >= 0 only for backtracking entries
  *                 while state and state.pos < 0:
  *                     state = pop(state)             # <<<<<<<<<<<<<<
  *                 idx = state.opidx
  *                 pos = state.pos
  */
-        __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 286, __pyx_L1_error)
+        __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 292, __pyx_L1_error)
         __pyx_v_state = __pyx_t_6;
       }
 
-      /* "pe/_cy_machine.pyx":287
+      /* "pe/_cy_machine.pyx":293
  *                 while state and state.pos < 0:
  *                     state = pop(state)
  *                 idx = state.opidx             # <<<<<<<<<<<<<<
  *                 pos = state.pos
  *                 args[state.argidx:] = []
  */
       __pyx_t_7 = __pyx_v_state->opidx;
       __pyx_v_idx = __pyx_t_7;
 
-      /* "pe/_cy_machine.pyx":288
+      /* "pe/_cy_machine.pyx":294
  *                     state = pop(state)
  *                 idx = state.opidx
  *                 pos = state.pos             # <<<<<<<<<<<<<<
  *                 args[state.argidx:] = []
  *                 if kwargs:
  */
       __pyx_t_7 = __pyx_v_state->pos;
       __pyx_v_pos = __pyx_t_7;
 
-      /* "pe/_cy_machine.pyx":289
+      /* "pe/_cy_machine.pyx":295
  *                 idx = state.opidx
  *                 pos = state.pos
  *                 args[state.argidx:] = []             # <<<<<<<<<<<<<<
  *                 if kwargs:
  *                     kwargs[state.kwidx:] = []
  */
-      __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 289, __pyx_L1_error)
+      __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 295, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 289, __pyx_L1_error)
+        __PYX_ERR(0, 295, __pyx_L1_error)
       }
-      if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_t_3, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 289, __pyx_L1_error)
+      if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_t_3, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 295, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "pe/_cy_machine.pyx":290
+      /* "pe/_cy_machine.pyx":296
  *                 pos = state.pos
  *                 args[state.argidx:] = []
  *                 if kwargs:             # <<<<<<<<<<<<<<
  *                     kwargs[state.kwidx:] = []
  *                 state = pop(state)  # pop backtracking entry
  */
       __pyx_t_2 = (__pyx_v_kwargs != Py_None)&&(PyList_GET_SIZE(__pyx_v_kwargs) != 0);
       if (__pyx_t_2) {
 
-        /* "pe/_cy_machine.pyx":291
+        /* "pe/_cy_machine.pyx":297
  *                 args[state.argidx:] = []
  *                 if kwargs:
  *                     kwargs[state.kwidx:] = []             # <<<<<<<<<<<<<<
  *                 state = pop(state)  # pop backtracking entry
  *             else:
  */
-        __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 291, __pyx_L1_error)
+        __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 297, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         if (unlikely(__pyx_v_kwargs == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 291, __pyx_L1_error)
+          __PYX_ERR(0, 297, __pyx_L1_error)
         }
-        if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_3, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 291, __pyx_L1_error)
+        if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_3, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 297, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "pe/_cy_machine.pyx":290
+        /* "pe/_cy_machine.pyx":296
  *                 pos = state.pos
  *                 args[state.argidx:] = []
  *                 if kwargs:             # <<<<<<<<<<<<<<
  *                     kwargs[state.kwidx:] = []
  *                 state = pop(state)  # pop backtracking entry
  */
       }
 
-      /* "pe/_cy_machine.pyx":292
+      /* "pe/_cy_machine.pyx":298
  *                 if kwargs:
  *                     kwargs[state.kwidx:] = []
  *                 state = pop(state)  # pop backtracking entry             # <<<<<<<<<<<<<<
  *             else:
  *                 if instr.capturing:
  */
-      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 292, __pyx_L1_error)
+      __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 298, __pyx_L1_error)
       __pyx_v_state = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":283
+      /* "pe/_cy_machine.pyx":289
  *                 raise Error(f'invalid operation: {instr.opcode}')
  * 
  *             if idx == FAILURE:             # <<<<<<<<<<<<<<
  *                 # pos is >= 0 only for backtracking entries
  *                 while state and state.pos < 0:
  */
       goto __pyx_L11;
     }
 
-    /* "pe/_cy_machine.pyx":294
+    /* "pe/_cy_machine.pyx":300
  *                 state = pop(state)  # pop backtracking entry
  *             else:
  *                 if instr.capturing:             # <<<<<<<<<<<<<<
  *                     args[state.argidx:] = [s[state.mark:pos]]
  *                     kwargs[state.kwidx:] = []
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_instr->capturing != 0);
       if (__pyx_t_2) {
 
-        /* "pe/_cy_machine.pyx":295
+        /* "pe/_cy_machine.pyx":301
  *             else:
  *                 if instr.capturing:
  *                     args[state.argidx:] = [s[state.mark:pos]]             # <<<<<<<<<<<<<<
  *                     kwargs[state.kwidx:] = []
  *                     state = pop(state)
  */
         if (unlikely(__pyx_v_s == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 295, __pyx_L1_error)
+          __PYX_ERR(0, 301, __pyx_L1_error)
         }
-        __pyx_t_3 = __Pyx_PyUnicode_Substring(__pyx_v_s, __pyx_v_state->mark, __pyx_v_pos); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 295, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyUnicode_Substring(__pyx_v_s, __pyx_v_state->mark, __pyx_v_pos); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 301, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_9 = PyList_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 295, __pyx_L1_error)
+        __pyx_t_9 = PyList_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 301, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         __Pyx_GIVEREF(__pyx_t_3);
         PyList_SET_ITEM(__pyx_t_9, 0, __pyx_t_3);
         __pyx_t_3 = 0;
         if (unlikely(__pyx_v_args == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 295, __pyx_L1_error)
+          __PYX_ERR(0, 301, __pyx_L1_error)
         }
-        if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_t_9, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 295, __pyx_L1_error)
+        if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_t_9, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 301, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-        /* "pe/_cy_machine.pyx":296
+        /* "pe/_cy_machine.pyx":302
  *                 if instr.capturing:
  *                     args[state.argidx:] = [s[state.mark:pos]]
  *                     kwargs[state.kwidx:] = []             # <<<<<<<<<<<<<<
  *                     state = pop(state)
  * 
  */
-        __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 296, __pyx_L1_error)
+        __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 302, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (unlikely(__pyx_v_kwargs == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 296, __pyx_L1_error)
+          __PYX_ERR(0, 302, __pyx_L1_error)
         }
-        if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_9, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 296, __pyx_L1_error)
+        if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_9, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 302, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-        /* "pe/_cy_machine.pyx":297
+        /* "pe/_cy_machine.pyx":303
  *                     args[state.argidx:] = [s[state.mark:pos]]
  *                     kwargs[state.kwidx:] = []
  *                     state = pop(state)             # <<<<<<<<<<<<<<
  * 
  *                 if instr.action is not None:
  */
-        __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L1_error)
+        __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 303, __pyx_L1_error)
         __pyx_v_state = __pyx_t_6;
 
-        /* "pe/_cy_machine.pyx":294
+        /* "pe/_cy_machine.pyx":300
  *                 state = pop(state)  # pop backtracking entry
  *             else:
  *                 if instr.capturing:             # <<<<<<<<<<<<<<
  *                     args[state.argidx:] = [s[state.mark:pos]]
  *                     kwargs[state.kwidx:] = []
  */
       }
 
-      /* "pe/_cy_machine.pyx":299
+      /* "pe/_cy_machine.pyx":305
  *                     state = pop(state)
  * 
  *                 if instr.action is not None:             # <<<<<<<<<<<<<<
  *                     _args, _kwargs = instr.action(
  *                         s,
  */
       __pyx_t_2 = (__pyx_v_instr->action != Py_None);
       __pyx_t_1 = (__pyx_t_2 != 0);
       if (__pyx_t_1) {
 
-        /* "pe/_cy_machine.pyx":302
+        /* "pe/_cy_machine.pyx":308
  *                     _args, _kwargs = instr.action(
  *                         s,
  *                         state.mark,             # <<<<<<<<<<<<<<
  *                         pos,
  *                         args[state.argidx:],
  */
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_state->mark); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 302, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_state->mark); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 308, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
 
-        /* "pe/_cy_machine.pyx":303
+        /* "pe/_cy_machine.pyx":309
  *                         s,
  *                         state.mark,
  *                         pos,             # <<<<<<<<<<<<<<
  *                         args[state.argidx:],
  *                         dict(kwargs[state.kwidx:])
  */
-        __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 303, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 309, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
 
-        /* "pe/_cy_machine.pyx":304
+        /* "pe/_cy_machine.pyx":310
  *                         state.mark,
  *                         pos,
  *                         args[state.argidx:],             # <<<<<<<<<<<<<<
  *                         dict(kwargs[state.kwidx:])
  *                     )
  */
         if (unlikely(__pyx_v_args == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 304, __pyx_L1_error)
+          __PYX_ERR(0, 310, __pyx_L1_error)
         }
-        __pyx_t_10 = __Pyx_PyList_GetSlice(__pyx_v_args, __pyx_v_state->argidx, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 304, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyList_GetSlice(__pyx_v_args, __pyx_v_state->argidx, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 310, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
 
-        /* "pe/_cy_machine.pyx":305
+        /* "pe/_cy_machine.pyx":311
  *                         pos,
  *                         args[state.argidx:],
  *                         dict(kwargs[state.kwidx:])             # <<<<<<<<<<<<<<
  *                     )
  *                     args[state.argidx:] = _args
  */
         if (unlikely(__pyx_v_kwargs == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 305, __pyx_L1_error)
+          __PYX_ERR(0, 311, __pyx_L1_error)
         }
-        __pyx_t_12 = __Pyx_PyList_GetSlice(__pyx_v_kwargs, __pyx_v_state->kwidx, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 305, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyList_GetSlice(__pyx_v_kwargs, __pyx_v_state->kwidx, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 311, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_12); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 305, __pyx_L1_error)
+        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_12); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 311, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_INCREF(__pyx_v_instr->action);
         __pyx_t_12 = __pyx_v_instr->action; __pyx_t_14 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
           __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_12);
@@ -7540,37 +7631,37 @@
             __Pyx_DECREF_SET(__pyx_t_12, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_12)) {
           PyObject *__pyx_temp[6] = {__pyx_t_14, __pyx_v_s, __pyx_t_3, __pyx_t_11, __pyx_t_10, __pyx_t_13};
-          __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_7, 5+__pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 300, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_7, 5+__pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 306, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_12)) {
           PyObject *__pyx_temp[6] = {__pyx_t_14, __pyx_v_s, __pyx_t_3, __pyx_t_11, __pyx_t_10, __pyx_t_13};
-          __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_7, 5+__pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 300, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_7, 5+__pyx_t_7); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 306, __pyx_L1_error)
           __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         } else
         #endif
         {
-          __pyx_t_15 = PyTuple_New(5+__pyx_t_7); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 300, __pyx_L1_error)
+          __pyx_t_15 = PyTuple_New(5+__pyx_t_7); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 306, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_15);
           if (__pyx_t_14) {
             __Pyx_GIVEREF(__pyx_t_14); PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_14); __pyx_t_14 = NULL;
           }
           __Pyx_INCREF(__pyx_v_s);
           __Pyx_GIVEREF(__pyx_v_s);
           PyTuple_SET_ITEM(__pyx_t_15, 0+__pyx_t_7, __pyx_v_s);
@@ -7582,248 +7673,248 @@
           PyTuple_SET_ITEM(__pyx_t_15, 3+__pyx_t_7, __pyx_t_10);
           __Pyx_GIVEREF(__pyx_t_13);
           PyTuple_SET_ITEM(__pyx_t_15, 4+__pyx_t_7, __pyx_t_13);
           __pyx_t_3 = 0;
           __pyx_t_11 = 0;
           __pyx_t_10 = 0;
           __pyx_t_13 = 0;
-          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_15, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 300, __pyx_L1_error)
+          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_15, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 306, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         }
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         if ((likely(PyTuple_CheckExact(__pyx_t_9))) || (PyList_CheckExact(__pyx_t_9))) {
           PyObject* sequence = __pyx_t_9;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 300, __pyx_L1_error)
+            __PYX_ERR(0, 306, __pyx_L1_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_12 = PyTuple_GET_ITEM(sequence, 0); 
             __pyx_t_15 = PyTuple_GET_ITEM(sequence, 1); 
           } else {
             __pyx_t_12 = PyList_GET_ITEM(sequence, 0); 
             __pyx_t_15 = PyList_GET_ITEM(sequence, 1); 
           }
           __Pyx_INCREF(__pyx_t_12);
           __Pyx_INCREF(__pyx_t_15);
           #else
-          __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 300, __pyx_L1_error)
+          __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 306, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_15 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 300, __pyx_L1_error)
+          __pyx_t_15 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 306, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_15);
           #endif
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_13 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 300, __pyx_L1_error)
+          __pyx_t_13 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 306, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           __pyx_t_16 = Py_TYPE(__pyx_t_13)->tp_iternext;
           index = 0; __pyx_t_12 = __pyx_t_16(__pyx_t_13); if (unlikely(!__pyx_t_12)) goto __pyx_L19_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_12);
           index = 1; __pyx_t_15 = __pyx_t_16(__pyx_t_13); if (unlikely(!__pyx_t_15)) goto __pyx_L19_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_15);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_16(__pyx_t_13), 2) < 0) __PYX_ERR(0, 300, __pyx_L1_error)
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_16(__pyx_t_13), 2) < 0) __PYX_ERR(0, 306, __pyx_L1_error)
           __pyx_t_16 = NULL;
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           goto __pyx_L20_unpacking_done;
           __pyx_L19_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __pyx_t_16 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 300, __pyx_L1_error)
+          __PYX_ERR(0, 306, __pyx_L1_error)
           __pyx_L20_unpacking_done:;
         }
 
-        /* "pe/_cy_machine.pyx":300
+        /* "pe/_cy_machine.pyx":306
  * 
  *                 if instr.action is not None:
  *                     _args, _kwargs = instr.action(             # <<<<<<<<<<<<<<
  *                         s,
  *                         state.mark,
  */
         __Pyx_XDECREF_SET(__pyx_v__args, __pyx_t_12);
         __pyx_t_12 = 0;
         __Pyx_XDECREF_SET(__pyx_v__kwargs, __pyx_t_15);
         __pyx_t_15 = 0;
 
-        /* "pe/_cy_machine.pyx":307
+        /* "pe/_cy_machine.pyx":313
  *                         dict(kwargs[state.kwidx:])
  *                     )
  *                     args[state.argidx:] = _args             # <<<<<<<<<<<<<<
  *                     if not _kwargs:
  *                         kwargs[state.kwidx:] = []
  */
         if (unlikely(__pyx_v_args == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 307, __pyx_L1_error)
+          __PYX_ERR(0, 313, __pyx_L1_error)
         }
-        if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_v__args, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 307, __pyx_L1_error)
+        if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_v__args, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 313, __pyx_L1_error)
 
-        /* "pe/_cy_machine.pyx":308
+        /* "pe/_cy_machine.pyx":314
  *                     )
  *                     args[state.argidx:] = _args
  *                     if not _kwargs:             # <<<<<<<<<<<<<<
  *                         kwargs[state.kwidx:] = []
  *                     else:
  */
-        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v__kwargs); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 308, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v__kwargs); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 314, __pyx_L1_error)
         __pyx_t_2 = ((!__pyx_t_1) != 0);
         if (__pyx_t_2) {
 
-          /* "pe/_cy_machine.pyx":309
+          /* "pe/_cy_machine.pyx":315
  *                     args[state.argidx:] = _args
  *                     if not _kwargs:
  *                         kwargs[state.kwidx:] = []             # <<<<<<<<<<<<<<
  *                     else:
  *                         kwargs[state.kwidx:] = _kwargs.items()
  */
-          __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 309, __pyx_L1_error)
+          __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 315, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           if (unlikely(__pyx_v_kwargs == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-            __PYX_ERR(0, 309, __pyx_L1_error)
+            __PYX_ERR(0, 315, __pyx_L1_error)
           }
-          if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_9, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 309, __pyx_L1_error)
+          if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_9, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 315, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-          /* "pe/_cy_machine.pyx":308
+          /* "pe/_cy_machine.pyx":314
  *                     )
  *                     args[state.argidx:] = _args
  *                     if not _kwargs:             # <<<<<<<<<<<<<<
  *                         kwargs[state.kwidx:] = []
  *                     else:
  */
           goto __pyx_L21;
         }
 
-        /* "pe/_cy_machine.pyx":311
+        /* "pe/_cy_machine.pyx":317
  *                         kwargs[state.kwidx:] = []
  *                     else:
  *                         kwargs[state.kwidx:] = _kwargs.items()             # <<<<<<<<<<<<<<
  *                     state = pop(state)
  * 
  */
         /*else*/ {
-          __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v__kwargs, __pyx_n_s_items); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 311, __pyx_L1_error)
+          __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v__kwargs, __pyx_n_s_items); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 317, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_15);
           __pyx_t_12 = NULL;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_15))) {
             __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_15);
             if (likely(__pyx_t_12)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
               __Pyx_INCREF(__pyx_t_12);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_15, function);
             }
           }
           __pyx_t_9 = (__pyx_t_12) ? __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_t_12) : __Pyx_PyObject_CallNoArg(__pyx_t_15);
           __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 311, __pyx_L1_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 317, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
           if (unlikely(__pyx_v_kwargs == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-            __PYX_ERR(0, 311, __pyx_L1_error)
+            __PYX_ERR(0, 317, __pyx_L1_error)
           }
-          if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_9, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 311, __pyx_L1_error)
+          if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_9, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 317, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
         __pyx_L21:;
 
-        /* "pe/_cy_machine.pyx":312
+        /* "pe/_cy_machine.pyx":318
  *                     else:
  *                         kwargs[state.kwidx:] = _kwargs.items()
  *                     state = pop(state)             # <<<<<<<<<<<<<<
  * 
  *                 idx += 1
  */
-        __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 312, __pyx_L1_error)
+        __pyx_t_6 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 318, __pyx_L1_error)
         __pyx_v_state = __pyx_t_6;
 
-        /* "pe/_cy_machine.pyx":299
+        /* "pe/_cy_machine.pyx":305
  *                     state = pop(state)
  * 
  *                 if instr.action is not None:             # <<<<<<<<<<<<<<
  *                     _args, _kwargs = instr.action(
  *                         s,
  */
       }
 
-      /* "pe/_cy_machine.pyx":314
+      /* "pe/_cy_machine.pyx":320
  *                     state = pop(state)
  * 
  *                 idx += 1             # <<<<<<<<<<<<<<
  * 
  *         if not state:
  */
       __pyx_v_idx = (__pyx_v_idx + 1);
     }
     __pyx_L11:;
     __pyx_L6_continue:;
   }
   __pyx_L7_break:;
 
-  /* "pe/_cy_machine.pyx":316
+  /* "pe/_cy_machine.pyx":322
  *                 idx += 1
  * 
  *         if not state:             # <<<<<<<<<<<<<<
  *             state = push(0, -1, -1, 0, 0, NULL)
  *         else:
  */
   __pyx_t_2 = ((!(__pyx_v_state != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "pe/_cy_machine.pyx":317
+    /* "pe/_cy_machine.pyx":323
  * 
  *         if not state:
  *             state = push(0, -1, -1, 0, 0, NULL)             # <<<<<<<<<<<<<<
  *         else:
  *             state.pos = pos
  */
-    __pyx_t_6 = __pyx_f_2pe_11_cy_machine_push(0, -1, -1, 0, 0, NULL); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 317, __pyx_L1_error)
+    __pyx_t_6 = __pyx_f_2pe_11_cy_machine_push(0, -1, -1, 0, 0, NULL); if (unlikely(__pyx_t_6 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 323, __pyx_L1_error)
     __pyx_v_state = __pyx_t_6;
 
-    /* "pe/_cy_machine.pyx":316
+    /* "pe/_cy_machine.pyx":322
  *                 idx += 1
  * 
  *         if not state:             # <<<<<<<<<<<<<<
  *             state = push(0, -1, -1, 0, 0, NULL)
  *         else:
  */
     goto __pyx_L22;
   }
 
-  /* "pe/_cy_machine.pyx":319
+  /* "pe/_cy_machine.pyx":325
  *             state = push(0, -1, -1, 0, 0, NULL)
  *         else:
  *             state.pos = pos             # <<<<<<<<<<<<<<
  *         return state
  * 
  */
   /*else*/ {
     __pyx_v_state->pos = __pyx_v_pos;
   }
   __pyx_L22:;
 
-  /* "pe/_cy_machine.pyx":320
+  /* "pe/_cy_machine.pyx":326
  *         else:
  *             state.pos = pos
  *         return state             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_state;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":204
+  /* "pe/_cy_machine.pyx":210
  *         return retval
  * 
  *     cdef State* _match(             # <<<<<<<<<<<<<<
  *         self,
  *         int idx,
  */
 
@@ -8137,15 +8228,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":330
+/* "pe/_cy_machine.pyx":336
  * 
  * 
  * def _make_program(grammar) -> Tuple[_Program, _Index]:             # <<<<<<<<<<<<<<
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  */
 
@@ -8183,289 +8274,289 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_make_program", 0);
 
-  /* "pe/_cy_machine.pyx":332
+  /* "pe/_cy_machine.pyx":338
  * def _make_program(grammar) -> Tuple[_Program, _Index]:
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}             # <<<<<<<<<<<<<<
  *     pis: _Program = []
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_index = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":333
+  /* "pe/_cy_machine.pyx":339
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  *     pis: _Program = []             # <<<<<<<<<<<<<<
  * 
  *     pis.append(Instruction(FAIL))  # special instruction for general failure
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 339, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_pis = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":335
+  /* "pe/_cy_machine.pyx":341
  *     pis: _Program = []
  * 
  *     pis.append(Instruction(FAIL))  # special instruction for general failure             # <<<<<<<<<<<<<<
  *     for name in grammar.definitions:
  *         index[name] = len(pis)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAIL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAIL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":336
+  /* "pe/_cy_machine.pyx":342
  * 
  *     pis.append(Instruction(FAIL))  # special instruction for general failure
  *     for name in grammar.definitions:             # <<<<<<<<<<<<<<
  *         index[name] = len(pis)
  *         _pis = _parsing_instructions(grammar[name])
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_grammar, __pyx_n_s_definitions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_grammar, __pyx_n_s_definitions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
     __pyx_t_1 = __pyx_t_2; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 342, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 336, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 342, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 342, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 342, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_5(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 336, __pyx_L1_error)
+          else __PYX_ERR(0, 342, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":337
+    /* "pe/_cy_machine.pyx":343
  *     pis.append(Instruction(FAIL))  # special instruction for general failure
  *     for name in grammar.definitions:
  *         index[name] = len(pis)             # <<<<<<<<<<<<<<
  *         _pis = _parsing_instructions(grammar[name])
  *         pis.extend(_pis)
  */
-    __pyx_t_6 = PyList_GET_SIZE(__pyx_v_pis); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 337, __pyx_L1_error)
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
+    __pyx_t_6 = PyList_GET_SIZE(__pyx_v_pis); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 343, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (unlikely(PyDict_SetItem(__pyx_v_index, __pyx_v_name, __pyx_t_2) < 0)) __PYX_ERR(0, 337, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_index, __pyx_v_name, __pyx_t_2) < 0)) __PYX_ERR(0, 343, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":338
+    /* "pe/_cy_machine.pyx":344
  *     for name in grammar.definitions:
  *         index[name] = len(pis)
  *         _pis = _parsing_instructions(grammar[name])             # <<<<<<<<<<<<<<
  *         pis.extend(_pis)
  *         pis.append(Instruction(RETURN))
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 338, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 344, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_grammar, __pyx_v_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 338, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_grammar, __pyx_v_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 344, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_2 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_9, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_8);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF_SET(__pyx_v__pis, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":339
+    /* "pe/_cy_machine.pyx":345
  *         index[name] = len(pis)
  *         _pis = _parsing_instructions(grammar[name])
  *         pis.extend(_pis)             # <<<<<<<<<<<<<<
  *         pis.append(Instruction(RETURN))
  * 
  */
-    __pyx_t_3 = __Pyx_PyList_Extend(__pyx_v_pis, __pyx_v__pis); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 339, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyList_Extend(__pyx_v_pis, __pyx_v__pis); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 345, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":340
+    /* "pe/_cy_machine.pyx":346
  *         _pis = _parsing_instructions(grammar[name])
  *         pis.extend(_pis)
  *         pis.append(Instruction(RETURN))             # <<<<<<<<<<<<<<
  * 
  *     # add locations to calls
  */
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RETURN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RETURN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 346, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 340, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_7); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 340, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_7); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 346, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "pe/_cy_machine.pyx":336
+    /* "pe/_cy_machine.pyx":342
  * 
  *     pis.append(Instruction(FAIL))  # special instruction for general failure
  *     for name in grammar.definitions:             # <<<<<<<<<<<<<<
  *         index[name] = len(pis)
  *         _pis = _parsing_instructions(grammar[name])
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":343
+  /* "pe/_cy_machine.pyx":349
  * 
  *     # add locations to calls
  *     for pi in pis:             # <<<<<<<<<<<<<<
  *         if pi.opcode == CALL:
  *             pi.oploc = index[pi.name]
  */
   __pyx_t_1 = __pyx_v_pis; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
   for (;;) {
     if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_7); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 343, __pyx_L1_error)
+    __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_7); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 349, __pyx_L1_error)
     #else
-    __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 343, __pyx_L1_error)
+    __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 349, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_pi, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "pe/_cy_machine.pyx":344
+    /* "pe/_cy_machine.pyx":350
  *     # add locations to calls
  *     for pi in pis:
  *         if pi.opcode == CALL:             # <<<<<<<<<<<<<<
  *             pi.oploc = index[pi.name]
  * 
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = PyObject_RichCompare(__pyx_t_7, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_8 = PyObject_RichCompare(__pyx_t_7, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     if (__pyx_t_10) {
 
-      /* "pe/_cy_machine.pyx":345
+      /* "pe/_cy_machine.pyx":351
  *     for pi in pis:
  *         if pi.opcode == CALL:
  *             pi.oploc = index[pi.name]             # <<<<<<<<<<<<<<
  * 
  *     pis.append(Instruction(PASS))  # success condition
  */
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 345, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 351, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_index, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_index, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 351, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_oploc, __pyx_t_2) < 0) __PYX_ERR(0, 345, __pyx_L1_error)
+      if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_oploc, __pyx_t_2) < 0) __PYX_ERR(0, 351, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "pe/_cy_machine.pyx":344
+      /* "pe/_cy_machine.pyx":350
  *     # add locations to calls
  *     for pi in pis:
  *         if pi.opcode == CALL:             # <<<<<<<<<<<<<<
  *             pi.oploc = index[pi.name]
  * 
  */
     }
 
-    /* "pe/_cy_machine.pyx":343
+    /* "pe/_cy_machine.pyx":349
  * 
  *     # add locations to calls
  *     for pi in pis:             # <<<<<<<<<<<<<<
  *         if pi.opcode == CALL:
  *             pi.oploc = index[pi.name]
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":347
+  /* "pe/_cy_machine.pyx":353
  *             pi.oploc = index[pi.name]
  * 
  *     pis.append(Instruction(PASS))  # success condition             # <<<<<<<<<<<<<<
  * 
  *     return pis, index
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_PASS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_PASS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 347, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":349
+  /* "pe/_cy_machine.pyx":355
  *     pis.append(Instruction(PASS))  # success condition
  * 
  *     return pis, index             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_pis);
   __Pyx_GIVEREF(__pyx_v_pis);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_pis);
   __Pyx_INCREF(__pyx_v_index);
   __Pyx_GIVEREF(__pyx_v_index);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_index);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":330
+  /* "pe/_cy_machine.pyx":336
  * 
  * 
  * def _make_program(grammar) -> Tuple[_Program, _Index]:             # <<<<<<<<<<<<<<
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  */
 
@@ -8485,15 +8576,15 @@
   __Pyx_XDECREF(__pyx_v__pis);
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":352
+/* "pe/_cy_machine.pyx":358
  * 
  * 
  * def _dot(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Dot())]
  * 
  */
 
@@ -8518,49 +8609,49 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_dot", 0);
 
-  /* "pe/_cy_machine.pyx":353
+  /* "pe/_cy_machine.pyx":359
  * 
  * def _dot(defn):
  *     return [Instruction(SCAN, scanner=Dot())]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Dot)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Dot)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_3) < 0) __PYX_ERR(0, 353, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_3) < 0) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 359, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":352
+  /* "pe/_cy_machine.pyx":358
  * 
  * 
  * def _dot(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Dot())]
  * 
  */
 
@@ -8573,15 +8664,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":356
+/* "pe/_cy_machine.pyx":362
  * 
  * 
  * def _lit(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]
  * 
  */
 
@@ -8607,55 +8698,55 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lit", 0);
 
-  /* "pe/_cy_machine.pyx":357
+  /* "pe/_cy_machine.pyx":363
  * 
  * def _lit(defn):
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Literal), __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Literal), __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_3) < 0) __PYX_ERR(0, 357, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_3) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":356
+  /* "pe/_cy_machine.pyx":362
  * 
  * 
  * def _lit(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]
  * 
  */
 
@@ -8669,15 +8760,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":360
+/* "pe/_cy_machine.pyx":366
  * 
  * 
  * def _cls(defn, mincount=1, maxcount=1):             # <<<<<<<<<<<<<<
  *     cclass = CharacterClass(
  *         defn.args[0],
  */
 
@@ -8727,15 +8818,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_maxcount);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_cls") < 0)) __PYX_ERR(0, 360, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_cls") < 0)) __PYX_ERR(0, 366, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -8746,15 +8837,15 @@
     }
     __pyx_v_defn = values[0];
     __pyx_v_mincount = values[1];
     __pyx_v_maxcount = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_cls", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 360, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_cls", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 366, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine._cls", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2pe_11_cy_machine_6_cls(__pyx_self, __pyx_v_defn, __pyx_v_mincount, __pyx_v_maxcount);
 
@@ -8772,121 +8863,121 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_cls", 0);
 
-  /* "pe/_cy_machine.pyx":362
+  /* "pe/_cy_machine.pyx":368
  * def _cls(defn, mincount=1, maxcount=1):
  *     cclass = CharacterClass(
  *         defn.args[0],             # <<<<<<<<<<<<<<
  *         negate=defn.args[1],
  *         mincount=mincount,
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":361
+  /* "pe/_cy_machine.pyx":367
  * 
  * def _cls(defn, mincount=1, maxcount=1):
  *     cclass = CharacterClass(             # <<<<<<<<<<<<<<
  *         defn.args[0],
  *         negate=defn.args[1],
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":363
+  /* "pe/_cy_machine.pyx":369
  *     cclass = CharacterClass(
  *         defn.args[0],
  *         negate=defn.args[1],             # <<<<<<<<<<<<<<
  *         mincount=mincount,
  *         maxcount=maxcount
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_negate, __pyx_t_4) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_negate, __pyx_t_4) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":364
+  /* "pe/_cy_machine.pyx":370
  *         defn.args[0],
  *         negate=defn.args[1],
  *         mincount=mincount,             # <<<<<<<<<<<<<<
  *         maxcount=maxcount
  *     )
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_mincount, __pyx_v_mincount) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_mincount, __pyx_v_mincount) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":365
+  /* "pe/_cy_machine.pyx":371
  *         negate=defn.args[1],
  *         mincount=mincount,
  *         maxcount=maxcount             # <<<<<<<<<<<<<<
  *     )
  *     return [Instruction(SCAN, scanner=cclass)]
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_maxcount, __pyx_v_maxcount) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_maxcount, __pyx_v_maxcount) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":361
+  /* "pe/_cy_machine.pyx":367
  * 
  * def _cls(defn, mincount=1, maxcount=1):
  *     cclass = CharacterClass(             # <<<<<<<<<<<<<<
  *         defn.args[0],
  *         negate=defn.args[1],
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_CharacterClass), __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_CharacterClass), __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_cclass = ((struct __pyx_obj_2pe_11_cy_machine_CharacterClass *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":367
+  /* "pe/_cy_machine.pyx":373
  *         maxcount=maxcount
  *     )
  *     return [Instruction(SCAN, scanner=cclass)]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scanner, ((PyObject *)__pyx_v_cclass)) < 0) __PYX_ERR(0, 367, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scanner, ((PyObject *)__pyx_v_cclass)) < 0) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":360
+  /* "pe/_cy_machine.pyx":366
  * 
  * 
  * def _cls(defn, mincount=1, maxcount=1):             # <<<<<<<<<<<<<<
  *     cclass = CharacterClass(
  *         defn.args[0],
  */
 
@@ -8901,15 +8992,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_cclass);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":370
+/* "pe/_cy_machine.pyx":376
  * 
  * 
  * def _rgx(defn):             # <<<<<<<<<<<<<<
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  */
 
@@ -8939,119 +9030,119 @@
   PyObject *(*__pyx_t_5)(PyObject *);
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_rgx", 0);
 
-  /* "pe/_cy_machine.pyx":371
+  /* "pe/_cy_machine.pyx":377
  * 
  * def _rgx(defn):
  *     pat, flags = defn.args             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 377, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 371, __pyx_L1_error)
+      __PYX_ERR(0, 377, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 377, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 371, __pyx_L1_error)
+    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_5 = Py_TYPE(__pyx_t_4)->tp_iternext;
     index = 0; __pyx_t_2 = __pyx_t_5(__pyx_t_4); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_5(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_5(__pyx_t_4), 2) < 0) __PYX_ERR(0, 371, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_5(__pyx_t_4), 2) < 0) __PYX_ERR(0, 377, __pyx_L1_error)
     __pyx_t_5 = NULL;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 371, __pyx_L1_error)
+    __PYX_ERR(0, 377, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_pat = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_flags = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":372
+  /* "pe/_cy_machine.pyx":378
  * def _rgx(defn):
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_pat);
   __Pyx_GIVEREF(__pyx_v_pat);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_pat);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flags, __pyx_v_flags) < 0) __PYX_ERR(0, 372, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Regex), __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 372, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flags, __pyx_v_flags) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Regex), __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_6) < 0) __PYX_ERR(0, 372, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_6) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_6);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_6);
   __pyx_t_6 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":370
+  /* "pe/_cy_machine.pyx":376
  * 
  * 
  * def _rgx(defn):             # <<<<<<<<<<<<<<
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  */
 
@@ -9068,15 +9159,15 @@
   __Pyx_XDECREF(__pyx_v_pat);
   __Pyx_XDECREF(__pyx_v_flags);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":375
+/* "pe/_cy_machine.pyx":381
  * 
  * 
  * def _opt(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -9104,26 +9195,26 @@
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_opt", 0);
 
-  /* "pe/_cy_machine.pyx":376
+  /* "pe/_cy_machine.pyx":382
  * 
  * def _opt(defn):
  *     pi = _parsing_instructions(defn.args[0])             # <<<<<<<<<<<<<<
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 382, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 382, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 382, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9131,88 +9222,88 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_pi = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":377
+  /* "pe/_cy_machine.pyx":383
  * def _opt(defn):
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),             # <<<<<<<<<<<<<<
  *             *pi,
  *             Instruction(COMMIT, 1)]
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 377, __pyx_L1_error)
-  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_5 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_5 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":378
+  /* "pe/_cy_machine.pyx":384
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,             # <<<<<<<<<<<<<<
  *             Instruction(COMMIT, 1)]
  * 
  */
-  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
+  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 384, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":379
+  /* "pe/_cy_machine.pyx":385
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  *             Instruction(COMMIT, 1)]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 385, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 385, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_int_1);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 385, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_3) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_3) < 0) __PYX_ERR(0, 385, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":375
+  /* "pe/_cy_machine.pyx":381
  * 
  * 
  * def _opt(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -9227,15 +9318,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":382
+/* "pe/_cy_machine.pyx":388
  * 
  * 
  * def _str(defn): return _rpt(defn, 0)             # <<<<<<<<<<<<<<
  * def _pls(defn): return _rpt(defn, 1)
  * 
  */
 
@@ -9262,15 +9353,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_str", 0);
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rpt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rpt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9279,40 +9370,40 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_defn, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_defn, __pyx_int_0};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_defn);
     __Pyx_GIVEREF(__pyx_v_defn);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_defn);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_int_0);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -9327,15 +9418,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":383
+/* "pe/_cy_machine.pyx":389
  * 
  * def _str(defn): return _rpt(defn, 0)
  * def _pls(defn): return _rpt(defn, 1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
 
@@ -9362,15 +9453,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_pls", 0);
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rpt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rpt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9379,40 +9470,40 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_defn, __pyx_int_1};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 389, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_defn, __pyx_int_1};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 389, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 389, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_defn);
     __Pyx_GIVEREF(__pyx_v_defn);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_defn);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_int_1);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 389, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -9427,15 +9518,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":386
+/* "pe/_cy_machine.pyx":392
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
 
@@ -9470,32 +9561,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_defn)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mincount)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_rpt", 1, 2, 2, 1); __PYX_ERR(0, 386, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_rpt", 1, 2, 2, 1); __PYX_ERR(0, 392, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_rpt") < 0)) __PYX_ERR(0, 386, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_rpt") < 0)) __PYX_ERR(0, 392, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_defn = values[0];
     __pyx_v_mincount = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_rpt", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 386, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_rpt", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 392, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine._rpt", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2pe_11_cy_machine_16_rpt(__pyx_self, __pyx_v_defn, __pyx_v_mincount);
 
@@ -9518,26 +9609,26 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_rpt", 0);
 
-  /* "pe/_cy_machine.pyx":387
+  /* "pe/_cy_machine.pyx":393
  * 
  * def _rpt(defn, mincount):
  *     pis = _parsing_instructions(defn.args[0])             # <<<<<<<<<<<<<<
  *     if (len(pis) == 1
  *         and pis[0].opcode == SCAN
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -9545,353 +9636,353 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_pis = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":388
+  /* "pe/_cy_machine.pyx":394
  * def _rpt(defn, mincount):
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1             # <<<<<<<<<<<<<<
  *         and pis[0].opcode == SCAN
  *         and isinstance(pis[0].scanner, CharacterClass)
  */
-  __pyx_t_6 = PyObject_Length(__pyx_v_pis); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_6 = PyObject_Length(__pyx_v_pis); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 394, __pyx_L1_error)
   __pyx_t_7 = ((__pyx_t_6 == 1) != 0);
   if (__pyx_t_7) {
   } else {
     __pyx_t_5 = __pyx_t_7;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":389
+  /* "pe/_cy_machine.pyx":395
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  *         and pis[0].opcode == SCAN             # <<<<<<<<<<<<<<
  *         and isinstance(pis[0].scanner, CharacterClass)
  *         and not (pis[0].marking or pis[0].capturing)
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_opcode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_opcode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_7) {
   } else {
     __pyx_t_5 = __pyx_t_7;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":390
+  /* "pe/_cy_machine.pyx":396
  *     if (len(pis) == 1
  *         and pis[0].opcode == SCAN
  *         and isinstance(pis[0].scanner, CharacterClass)             # <<<<<<<<<<<<<<
  *         and not (pis[0].marking or pis[0].capturing)
  *         and pis[0].action is None
  */
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_7 = __Pyx_TypeCheck(__pyx_t_1, __pyx_ptype_2pe_11_cy_machine_CharacterClass); 
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (__pyx_t_8) {
   } else {
     __pyx_t_5 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":391
+  /* "pe/_cy_machine.pyx":397
  *         and pis[0].opcode == SCAN
  *         and isinstance(pis[0].scanner, CharacterClass)
  *         and not (pis[0].marking or pis[0].capturing)             # <<<<<<<<<<<<<<
  *         and pis[0].action is None
  *     ):
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_marking); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_marking); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!__pyx_t_7) {
   } else {
     __pyx_t_8 = __pyx_t_7;
     goto __pyx_L9_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_capturing); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_capturing); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 397, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_8 = __pyx_t_7;
   __pyx_L9_bool_binop_done:;
   __pyx_t_7 = ((!__pyx_t_8) != 0);
   if (__pyx_t_7) {
   } else {
     __pyx_t_5 = __pyx_t_7;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":392
+  /* "pe/_cy_machine.pyx":398
  *         and isinstance(pis[0].scanner, CharacterClass)
  *         and not (pis[0].marking or pis[0].capturing)
  *         and pis[0].action is None             # <<<<<<<<<<<<<<
  *     ):
  *         pi = pis[0]
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_action); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 392, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_action); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_7 = (__pyx_t_4 == Py_None);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_8 = (__pyx_t_7 != 0);
   __pyx_t_5 = __pyx_t_8;
   __pyx_L4_bool_binop_done:;
 
-  /* "pe/_cy_machine.pyx":388
+  /* "pe/_cy_machine.pyx":394
  * def _rpt(defn, mincount):
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1             # <<<<<<<<<<<<<<
  *         and pis[0].opcode == SCAN
  *         and isinstance(pis[0].scanner, CharacterClass)
  */
   if (__pyx_t_5) {
 
-    /* "pe/_cy_machine.pyx":394
+    /* "pe/_cy_machine.pyx":400
  *         and pis[0].action is None
  *     ):
  *         pi = pis[0]             # <<<<<<<<<<<<<<
  *         pi.scanner.mincount = mincount
  *         pi.scanner.maxcount = -1
  */
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 394, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_v_pi = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "pe/_cy_machine.pyx":395
+    /* "pe/_cy_machine.pyx":401
  *     ):
  *         pi = pis[0]
  *         pi.scanner.mincount = mincount             # <<<<<<<<<<<<<<
  *         pi.scanner.maxcount = -1
  *         return [Instruction(SCAN,
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 395, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 401, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_t_4, __pyx_n_s_mincount, __pyx_v_mincount) < 0) __PYX_ERR(0, 395, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_t_4, __pyx_n_s_mincount, __pyx_v_mincount) < 0) __PYX_ERR(0, 401, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pe/_cy_machine.pyx":396
+    /* "pe/_cy_machine.pyx":402
  *         pi = pis[0]
  *         pi.scanner.mincount = mincount
  *         pi.scanner.maxcount = -1             # <<<<<<<<<<<<<<
  *         return [Instruction(SCAN,
  *                             scanner=pi.scanner,
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 396, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 402, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_t_4, __pyx_n_s_maxcount, __pyx_int_neg_1) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_t_4, __pyx_n_s_maxcount, __pyx_int_neg_1) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pe/_cy_machine.pyx":397
+    /* "pe/_cy_machine.pyx":403
  *         pi.scanner.mincount = mincount
  *         pi.scanner.maxcount = -1
  *         return [Instruction(SCAN,             # <<<<<<<<<<<<<<
  *                             scanner=pi.scanner,
  *                             marking=pi.marking,
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 397, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pe/_cy_machine.pyx":398
+    /* "pe/_cy_machine.pyx":404
  *         pi.scanner.maxcount = -1
  *         return [Instruction(SCAN,
  *                             scanner=pi.scanner,             # <<<<<<<<<<<<<<
  *                             marking=pi.marking,
  *                             capturing=pi.capturing,
  */
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 398, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 404, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scanner, __pyx_t_2) < 0) __PYX_ERR(0, 398, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scanner, __pyx_t_2) < 0) __PYX_ERR(0, 404, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":399
+    /* "pe/_cy_machine.pyx":405
  *         return [Instruction(SCAN,
  *                             scanner=pi.scanner,
  *                             marking=pi.marking,             # <<<<<<<<<<<<<<
  *                             capturing=pi.capturing,
  *                             action=pi.action)]
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_marking); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 399, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_marking); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_marking, __pyx_t_2) < 0) __PYX_ERR(0, 398, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_marking, __pyx_t_2) < 0) __PYX_ERR(0, 404, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":400
+    /* "pe/_cy_machine.pyx":406
  *                             scanner=pi.scanner,
  *                             marking=pi.marking,
  *                             capturing=pi.capturing,             # <<<<<<<<<<<<<<
  *                             action=pi.action)]
  *     return [*(pis * mincount),
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_capturing); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 400, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_capturing); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_capturing, __pyx_t_2) < 0) __PYX_ERR(0, 398, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_capturing, __pyx_t_2) < 0) __PYX_ERR(0, 404, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":401
+    /* "pe/_cy_machine.pyx":407
  *                             marking=pi.marking,
  *                             capturing=pi.capturing,
  *                             action=pi.action)]             # <<<<<<<<<<<<<<
  *     return [*(pis * mincount),
  *             Instruction(BRANCH, len(pis) + 2),
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_action, __pyx_t_2) < 0) __PYX_ERR(0, 398, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_action, __pyx_t_2) < 0) __PYX_ERR(0, 404, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":397
+    /* "pe/_cy_machine.pyx":403
  *         pi.scanner.mincount = mincount
  *         pi.scanner.maxcount = -1
  *         return [Instruction(SCAN,             # <<<<<<<<<<<<<<
  *                             scanner=pi.scanner,
  *                             marking=pi.marking,
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 397, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_2);
     PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
     __pyx_t_2 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":388
+    /* "pe/_cy_machine.pyx":394
  * def _rpt(defn, mincount):
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1             # <<<<<<<<<<<<<<
  *         and pis[0].opcode == SCAN
  *         and isinstance(pis[0].scanner, CharacterClass)
  */
   }
 
-  /* "pe/_cy_machine.pyx":402
+  /* "pe/_cy_machine.pyx":408
  *                             capturing=pi.capturing,
  *                             action=pi.action)]
  *     return [*(pis * mincount),             # <<<<<<<<<<<<<<
  *             Instruction(BRANCH, len(pis) + 2),
  *             *pis,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_v_pis, __pyx_v_mincount); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Multiply(__pyx_v_pis, __pyx_v_mincount); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_t_4 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":403
+  /* "pe/_cy_machine.pyx":409
  *                             action=pi.action)]
  *     return [*(pis * mincount),
  *             Instruction(BRANCH, len(pis) + 2),             # <<<<<<<<<<<<<<
  *             *pis,
  *             Instruction(UPDATE, -len(pis))]
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = PyObject_Length(__pyx_v_pis); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 403, __pyx_L1_error)
-  __pyx_t_1 = PyInt_FromSsize_t((__pyx_t_6 + 2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_6 = PyObject_Length(__pyx_v_pis); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t((__pyx_t_6 + 2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_4, __pyx_t_1) < 0) __PYX_ERR(0, 403, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_4, __pyx_t_1) < 0) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":404
+  /* "pe/_cy_machine.pyx":410
  *     return [*(pis * mincount),
  *             Instruction(BRANCH, len(pis) + 2),
  *             *pis,             # <<<<<<<<<<<<<<
  *             Instruction(UPDATE, -len(pis))]
  * 
  */
-  if (__Pyx_PyList_Extend(__pyx_t_4, __pyx_v_pis) < 0) __PYX_ERR(0, 404, __pyx_L1_error)
+  if (__Pyx_PyList_Extend(__pyx_t_4, __pyx_v_pis) < 0) __PYX_ERR(0, 410, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":405
+  /* "pe/_cy_machine.pyx":411
  *             Instruction(BRANCH, len(pis) + 2),
  *             *pis,
  *             Instruction(UPDATE, -len(pis))]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_UPDATE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_UPDATE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = PyObject_Length(__pyx_v_pis); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 405, __pyx_L1_error)
-  __pyx_t_3 = PyInt_FromSsize_t((-__pyx_t_6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_6 = PyObject_Length(__pyx_v_pis); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t((-__pyx_t_6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_4, __pyx_t_3) < 0) __PYX_ERR(0, 405, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_4, __pyx_t_3) < 0) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":386
+  /* "pe/_cy_machine.pyx":392
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
 
@@ -9907,15 +9998,15 @@
   __Pyx_XDECREF(__pyx_v_pis);
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":408
+/* "pe/_cy_machine.pyx":414
  * 
  * 
  * def _sym(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(CALL, name=defn.args[0])]
  * 
  */
 
@@ -9941,52 +10032,52 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_sym", 0);
 
-  /* "pe/_cy_machine.pyx":409
+  /* "pe/_cy_machine.pyx":415
  * 
  * def _sym(defn):
  *     return [Instruction(CALL, name=defn.args[0])]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 409, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 415, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":408
+  /* "pe/_cy_machine.pyx":414
  * 
  * 
  * def _sym(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(CALL, name=defn.args[0])]
  * 
  */
 
@@ -10000,15 +10091,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":412
+/* "pe/_cy_machine.pyx":418
  * 
  * 
  * def _and(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -10036,26 +10127,26 @@
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_and", 0);
 
-  /* "pe/_cy_machine.pyx":413
+  /* "pe/_cy_machine.pyx":419
  * 
  * def _and(defn):
  *     pi = _parsing_instructions(defn.args[0])             # <<<<<<<<<<<<<<
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -10063,103 +10154,103 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_pi = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":414
+  /* "pe/_cy_machine.pyx":420
  * def _and(defn):
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),             # <<<<<<<<<<<<<<
  *             *pi,
  *             Instruction(RESTORE, 2),
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 414, __pyx_L1_error)
-  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_5 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_5 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":415
+  /* "pe/_cy_machine.pyx":421
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,             # <<<<<<<<<<<<<<
  *             Instruction(RESTORE, 2),
  *             Instruction(FAIL)]
  */
-  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 415, __pyx_L1_error)
+  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 421, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":416
+  /* "pe/_cy_machine.pyx":422
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  *             Instruction(RESTORE, 2),             # <<<<<<<<<<<<<<
  *             Instruction(FAIL)]
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RESTORE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RESTORE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_int_2);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_3) < 0) __PYX_ERR(0, 416, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_3) < 0) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":417
+  /* "pe/_cy_machine.pyx":423
  *             *pi,
  *             Instruction(RESTORE, 2),
  *             Instruction(FAIL)]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAIL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAIL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_4) < 0) __PYX_ERR(0, 417, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_4) < 0) __PYX_ERR(0, 423, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":412
+  /* "pe/_cy_machine.pyx":418
  * 
  * 
  * def _and(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -10174,15 +10265,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":420
+/* "pe/_cy_machine.pyx":426
  * 
  * 
  * def _not(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -10210,26 +10301,26 @@
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_not", 0);
 
-  /* "pe/_cy_machine.pyx":421
+  /* "pe/_cy_machine.pyx":427
  * 
  * def _not(defn):
  *     pi = _parsing_instructions(defn.args[0])             # <<<<<<<<<<<<<<
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -10237,80 +10328,80 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 421, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_pi = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":422
+  /* "pe/_cy_machine.pyx":428
  * def _not(defn):
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),             # <<<<<<<<<<<<<<
  *             *pi,
  *             Instruction(FAILTWICE)]
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 422, __pyx_L1_error)
-  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_5 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_5 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":423
+  /* "pe/_cy_machine.pyx":429
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,             # <<<<<<<<<<<<<<
  *             Instruction(FAILTWICE)]
  * 
  */
-  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 423, __pyx_L1_error)
+  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 429, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":424
+  /* "pe/_cy_machine.pyx":430
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  *             Instruction(FAILTWICE)]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAILTWICE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAILTWICE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_4) < 0) __PYX_ERR(0, 424, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_4) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":420
+  /* "pe/_cy_machine.pyx":426
  * 
  * 
  * def _not(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -10325,15 +10416,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":427
+/* "pe/_cy_machine.pyx":433
  * 
  * 
  * def _cap(defn):             # <<<<<<<<<<<<<<
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  */
 
@@ -10368,52 +10459,52 @@
   int __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_cap", 0);
 
-  /* "pe/_cy_machine.pyx":428
+  /* "pe/_cy_machine.pyx":434
  * 
  * def _cap(defn):
  *     captured_choice = defn.args[0].op == Operator.CHC             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if not pis[0].marking:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_op); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_op); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Operator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Operator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CHC); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CHC); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_captured_choice = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":429
+  /* "pe/_cy_machine.pyx":435
  * def _cap(defn):
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])             # <<<<<<<<<<<<<<
  *     if not pis[0].marking:
  *         pis[0].marking = True
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -10421,80 +10512,80 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 429, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_pis = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":430
+  /* "pe/_cy_machine.pyx":436
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  *     if not pis[0].marking:             # <<<<<<<<<<<<<<
  *         pis[0].marking = True
  *     else:
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 436, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_marking); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_marking); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 436, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 436, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_6 = ((!__pyx_t_5) != 0);
   if (__pyx_t_6) {
 
-    /* "pe/_cy_machine.pyx":431
+    /* "pe/_cy_machine.pyx":437
  *     pis = _parsing_instructions(defn.args[0])
  *     if not pis[0].marking:
  *         pis[0].marking = True             # <<<<<<<<<<<<<<
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 431, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_t_3, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_t_3, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "pe/_cy_machine.pyx":430
+    /* "pe/_cy_machine.pyx":436
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  *     if not pis[0].marking:             # <<<<<<<<<<<<<<
  *         pis[0].marking = True
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "pe/_cy_machine.pyx":433
+  /* "pe/_cy_machine.pyx":439
  *         pis[0].marking = True
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))             # <<<<<<<<<<<<<<
  *     pi = pis[-1]
  *     if (not pi.capturing
  */
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pis, __pyx_n_s_insert); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 433, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pis, __pyx_n_s_insert); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
-    __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 439, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 439, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
@@ -10505,202 +10596,202 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_int_0, __pyx_t_7};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_int_0, __pyx_t_7};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     } else
     #endif
     {
-      __pyx_t_1 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_INCREF(__pyx_int_0);
       __Pyx_GIVEREF(__pyx_int_0);
       PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_8, __pyx_int_0);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_8, __pyx_t_7);
       __pyx_t_7 = 0;
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 439, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "pe/_cy_machine.pyx":434
+  /* "pe/_cy_machine.pyx":440
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]             # <<<<<<<<<<<<<<
  *     if (not pi.capturing
  *         and pi.action is None
  */
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 434, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_pi = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":435
+  /* "pe/_cy_machine.pyx":441
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]
  *     if (not pi.capturing             # <<<<<<<<<<<<<<
  *         and pi.action is None
  *         and pi.opcode not in NO_CAP_OR_ACT
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_capturing); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_capturing); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 441, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 441, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_9 = ((!__pyx_t_5) != 0);
   if (__pyx_t_9) {
   } else {
     __pyx_t_6 = __pyx_t_9;
     goto __pyx_L5_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":436
+  /* "pe/_cy_machine.pyx":442
  *     pi = pis[-1]
  *     if (not pi.capturing
  *         and pi.action is None             # <<<<<<<<<<<<<<
  *         and pi.opcode not in NO_CAP_OR_ACT
  *         and not captured_choice
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 442, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_9 = (__pyx_t_3 == Py_None);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = (__pyx_t_9 != 0);
   if (__pyx_t_5) {
   } else {
     __pyx_t_6 = __pyx_t_5;
     goto __pyx_L5_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":437
+  /* "pe/_cy_machine.pyx":443
  *     if (not pi.capturing
  *         and pi.action is None
  *         and pi.opcode not in NO_CAP_OR_ACT             # <<<<<<<<<<<<<<
  *         and not captured_choice
  *     ):
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 437, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_CAP_OR_ACT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 437, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_CAP_OR_ACT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_t_3, __pyx_t_2, Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 437, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_t_3, __pyx_t_2, Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_9 = (__pyx_t_5 != 0);
   if (__pyx_t_9) {
   } else {
     __pyx_t_6 = __pyx_t_9;
     goto __pyx_L5_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":438
+  /* "pe/_cy_machine.pyx":444
  *         and pi.action is None
  *         and pi.opcode not in NO_CAP_OR_ACT
  *         and not captured_choice             # <<<<<<<<<<<<<<
  *     ):
  *         pis[-1].capturing = True
  */
-  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_captured_choice); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 438, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_captured_choice); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 444, __pyx_L1_error)
   __pyx_t_5 = ((!__pyx_t_9) != 0);
   __pyx_t_6 = __pyx_t_5;
   __pyx_L5_bool_binop_done:;
 
-  /* "pe/_cy_machine.pyx":435
+  /* "pe/_cy_machine.pyx":441
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]
  *     if (not pi.capturing             # <<<<<<<<<<<<<<
  *         and pi.action is None
  *         and pi.opcode not in NO_CAP_OR_ACT
  */
   if (__pyx_t_6) {
 
-    /* "pe/_cy_machine.pyx":440
+    /* "pe/_cy_machine.pyx":446
  *         and not captured_choice
  *     ):
  *         pis[-1].capturing = True             # <<<<<<<<<<<<<<
  *     else:
  *         pis.append(Instruction(NOOP, capturing=True))
  */
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 440, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 446, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_t_2, __pyx_n_s_capturing, Py_True) < 0) __PYX_ERR(0, 440, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_t_2, __pyx_n_s_capturing, Py_True) < 0) __PYX_ERR(0, 446, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":435
+    /* "pe/_cy_machine.pyx":441
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]
  *     if (not pi.capturing             # <<<<<<<<<<<<<<
  *         and pi.action is None
  *         and pi.opcode not in NO_CAP_OR_ACT
  */
     goto __pyx_L4;
   }
 
-  /* "pe/_cy_machine.pyx":442
+  /* "pe/_cy_machine.pyx":448
  *         pis[-1].capturing = True
  *     else:
  *         pis.append(Instruction(NOOP, capturing=True))             # <<<<<<<<<<<<<<
  *     return pis
  * 
  */
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_capturing, Py_True) < 0) __PYX_ERR(0, 442, __pyx_L1_error)
-    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_capturing, Py_True) < 0) __PYX_ERR(0, 448, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_10 = __Pyx_PyObject_Append(__pyx_v_pis, __pyx_t_1); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Append(__pyx_v_pis, __pyx_t_1); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 448, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L4:;
 
-  /* "pe/_cy_machine.pyx":443
+  /* "pe/_cy_machine.pyx":449
  *     else:
  *         pis.append(Instruction(NOOP, capturing=True))
  *     return pis             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_pis);
   __pyx_r = __pyx_v_pis;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":427
+  /* "pe/_cy_machine.pyx":433
  * 
  * 
  * def _cap(defn):             # <<<<<<<<<<<<<<
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  */
 
@@ -10718,15 +10809,15 @@
   __Pyx_XDECREF(__pyx_v_pis);
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":446
+/* "pe/_cy_machine.pyx":452
  * 
  * 
  * def _bnd(defn):             # <<<<<<<<<<<<<<
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))
  * 
  */
 
@@ -10758,36 +10849,36 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_bnd", 0);
 
-  /* "pe/_cy_machine.pyx":447
+  /* "pe/_cy_machine.pyx":453
  * 
  * def _bnd(defn):
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Rule); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Rule); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Bind); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Bind); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_8, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_8, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_8)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -10795,15 +10886,15 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_5 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_9);
   __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   __pyx_t_10 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_7)) {
@@ -10813,44 +10904,44 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_10 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_10, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_10, __pyx_t_5);
     __pyx_t_6 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
@@ -10860,22 +10951,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 447, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":446
+  /* "pe/_cy_machine.pyx":452
  * 
  * 
  * def _bnd(defn):             # <<<<<<<<<<<<<<
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))
  * 
  */
 
@@ -10894,15 +10985,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":450
+/* "pe/_cy_machine.pyx":456
  * 
  * 
  * def _seq(defn):             # <<<<<<<<<<<<<<
  *     head = [pi
  *             for d in defn.args[0][:-1]
  */
 
@@ -10937,170 +11028,170 @@
   Py_ssize_t __pyx_t_8;
   PyObject *(*__pyx_t_9)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_seq", 0);
 
-  /* "pe/_cy_machine.pyx":451
+  /* "pe/_cy_machine.pyx":457
  * 
  * def _seq(defn):
  *     head = [pi             # <<<<<<<<<<<<<<
  *             for d in defn.args[0][:-1]
  *             for pi in _parsing_instructions(d)]
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 451, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "pe/_cy_machine.pyx":452
+    /* "pe/_cy_machine.pyx":458
  * def _seq(defn):
  *     head = [pi
  *             for d in defn.args[0][:-1]             # <<<<<<<<<<<<<<
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 452, __pyx_L5_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L5_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, -1L, NULL, NULL, &__pyx_slice_, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 452, __pyx_L5_error)
+    __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, -1L, NULL, NULL, &__pyx_slice_, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
       __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L5_error)
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 452, __pyx_L5_error)
+      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 458, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 452, __pyx_L5_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 458, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 452, __pyx_L5_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 452, __pyx_L5_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 458, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 452, __pyx_L5_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_5(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 452, __pyx_L5_error)
+            else __PYX_ERR(0, 458, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_d, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "pe/_cy_machine.pyx":453
+      /* "pe/_cy_machine.pyx":459
  *     head = [pi
  *             for d in defn.args[0][:-1]
  *             for pi in _parsing_instructions(d)]             # <<<<<<<<<<<<<<
  *     tail = _parsing_instructions(defn.args[0][-1])
  *     return head + tail
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 453, __pyx_L5_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 459, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
         }
       }
       __pyx_t_2 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_7genexpr__pyx_v_d) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_7genexpr__pyx_v_d);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L5_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
         __pyx_t_6 = __pyx_t_2; __Pyx_INCREF(__pyx_t_6); __pyx_t_8 = 0;
         __pyx_t_9 = NULL;
       } else {
-        __pyx_t_8 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 453, __pyx_L5_error)
+        __pyx_t_8 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 459, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_9 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 453, __pyx_L5_error)
+        __pyx_t_9 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 459, __pyx_L5_error)
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       for (;;) {
         if (likely(!__pyx_t_9)) {
           if (likely(PyList_CheckExact(__pyx_t_6))) {
             if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_6)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_2 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 453, __pyx_L5_error)
+            __pyx_t_2 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 459, __pyx_L5_error)
             #else
-            __pyx_t_2 = PySequence_ITEM(__pyx_t_6, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L5_error)
+            __pyx_t_2 = PySequence_ITEM(__pyx_t_6, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L5_error)
             __Pyx_GOTREF(__pyx_t_2);
             #endif
           } else {
             if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 453, __pyx_L5_error)
+            __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_8); __Pyx_INCREF(__pyx_t_2); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 459, __pyx_L5_error)
             #else
-            __pyx_t_2 = PySequence_ITEM(__pyx_t_6, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L5_error)
+            __pyx_t_2 = PySequence_ITEM(__pyx_t_6, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L5_error)
             __Pyx_GOTREF(__pyx_t_2);
             #endif
           }
         } else {
           __pyx_t_2 = __pyx_t_9(__pyx_t_6);
           if (unlikely(!__pyx_t_2)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 453, __pyx_L5_error)
+              else __PYX_ERR(0, 459, __pyx_L5_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_2);
         }
         __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_pi, __pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "pe/_cy_machine.pyx":451
+        /* "pe/_cy_machine.pyx":457
  * 
  * def _seq(defn):
  *     head = [pi             # <<<<<<<<<<<<<<
  *             for d in defn.args[0][:-1]
  *             for pi in _parsing_instructions(d)]
  */
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_pi))) __PYX_ERR(0, 451, __pyx_L5_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_7genexpr__pyx_v_pi))) __PYX_ERR(0, 457, __pyx_L5_error)
 
-        /* "pe/_cy_machine.pyx":453
+        /* "pe/_cy_machine.pyx":459
  *     head = [pi
  *             for d in defn.args[0][:-1]
  *             for pi in _parsing_instructions(d)]             # <<<<<<<<<<<<<<
  *     tail = _parsing_instructions(defn.args[0][-1])
  *     return head + tail
  */
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "pe/_cy_machine.pyx":452
+      /* "pe/_cy_machine.pyx":458
  * def _seq(defn):
  *     head = [pi
  *             for d in defn.args[0][:-1]             # <<<<<<<<<<<<<<
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])
  */
     }
@@ -11113,29 +11204,29 @@
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_pi); __pyx_7genexpr__pyx_v_pi = 0;
     goto __pyx_L1_error;
     __pyx_L10_exit_scope:;
   } /* exit inner scope */
   __pyx_v_head = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":454
+  /* "pe/_cy_machine.pyx":460
  *             for d in defn.args[0][:-1]
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])             # <<<<<<<<<<<<<<
  *     return head + tail
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_2, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 454, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_2, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -11143,35 +11234,35 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_tail = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":455
+  /* "pe/_cy_machine.pyx":461
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])
  *     return head + tail             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyNumber_Add(__pyx_v_head, __pyx_v_tail); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 455, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_v_head, __pyx_v_tail); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":450
+  /* "pe/_cy_machine.pyx":456
  * 
  * 
  * def _seq(defn):             # <<<<<<<<<<<<<<
  *     head = [pi
  *             for d in defn.args[0][:-1]
  */
 
@@ -11190,15 +11281,15 @@
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_d);
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":458
+/* "pe/_cy_machine.pyx":464
  * 
  * 
  * def _chc(defn):             # <<<<<<<<<<<<<<
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  */
 
@@ -11232,237 +11323,237 @@
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_chc", 0);
 
-  /* "pe/_cy_machine.pyx":459
+  /* "pe/_cy_machine.pyx":465
  * 
  * def _chc(defn):
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]             # <<<<<<<<<<<<<<
  *     pi = pis[-1]
  *     for _pi in reversed(pis[:-1]):
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 459, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 465, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L5_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L5_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
       __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 459, __pyx_L5_error)
+      __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 465, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 459, __pyx_L5_error)
+      __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 465, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 459, __pyx_L5_error)
+          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 465, __pyx_L5_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L5_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         } else {
           if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 459, __pyx_L5_error)
+          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 465, __pyx_L5_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L5_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_5(__pyx_t_2);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 459, __pyx_L5_error)
+            else __PYX_ERR(0, 465, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_d, __pyx_t_3);
       __pyx_t_3 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 459, __pyx_L5_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 465, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
         }
       }
       __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_8genexpr1__pyx_v_d) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_8genexpr1__pyx_v_d);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L5_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 465, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 459, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 465, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_d); __pyx_8genexpr1__pyx_v_d = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_d); __pyx_8genexpr1__pyx_v_d = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_pis = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":460
+  /* "pe/_cy_machine.pyx":466
  * def _chc(defn):
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]             # <<<<<<<<<<<<<<
  *     for _pi in reversed(pis[:-1]):
  *         pi = [Instruction(BRANCH, len(_pi) + 2),
  */
-  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_pi = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":461
+  /* "pe/_cy_machine.pyx":467
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  *     for _pi in reversed(pis[:-1]):             # <<<<<<<<<<<<<<
  *         pi = [Instruction(BRANCH, len(_pi) + 2),
  *               *_pi,
  */
-  __pyx_t_1 = __Pyx_PyList_GetSlice(__pyx_v_pis, 0, -1L); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyList_GetSlice(__pyx_v_pis, 0, -1L); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = PyList_GET_SIZE(__pyx_t_2) - 1;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (__pyx_t_4 < 0) break;
     if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4--; if (unlikely(0 < 0)) __PYX_ERR(0, 461, __pyx_L1_error)
+    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4--; if (unlikely(0 < 0)) __PYX_ERR(0, 467, __pyx_L1_error)
     #else
-    __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4--; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+    __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4--; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     #endif
     __Pyx_XDECREF_SET(__pyx_v__pi, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pe/_cy_machine.pyx":462
+    /* "pe/_cy_machine.pyx":468
  *     pi = pis[-1]
  *     for _pi in reversed(pis[:-1]):
  *         pi = [Instruction(BRANCH, len(_pi) + 2),             # <<<<<<<<<<<<<<
  *               *_pi,
  *               Instruction(COMMIT, len(pi) + 1),
  */
-    __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = PyObject_Length(__pyx_v__pi); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 462, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_8 + 2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_8 = PyObject_Length(__pyx_v__pi); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 468, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_8 + 2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_6);
     __pyx_t_3 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 462, __pyx_L1_error)
+    __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_6);
     PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_6);
     __pyx_t_6 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "pe/_cy_machine.pyx":463
+    /* "pe/_cy_machine.pyx":469
  *     for _pi in reversed(pis[:-1]):
  *         pi = [Instruction(BRANCH, len(_pi) + 2),
  *               *_pi,             # <<<<<<<<<<<<<<
  *               Instruction(COMMIT, len(pi) + 1),
  *               *pi]
  */
-    if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v__pi) < 0) __PYX_ERR(0, 463, __pyx_L1_error)
+    if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v__pi) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":464
+    /* "pe/_cy_machine.pyx":470
  *         pi = [Instruction(BRANCH, len(_pi) + 2),
  *               *_pi,
  *               Instruction(COMMIT, len(pi) + 1),             # <<<<<<<<<<<<<<
  *               *pi]
  *     return pi
  */
-    __pyx_t_7 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 464, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 464, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_8 + 1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 464, __pyx_L1_error)
+    __pyx_t_8 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 470, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_8 + 1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_6);
     __pyx_t_7 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 464, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_6) < 0) __PYX_ERR(0, 464, __pyx_L1_error)
+    if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_6) < 0) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "pe/_cy_machine.pyx":465
+    /* "pe/_cy_machine.pyx":471
  *               *_pi,
  *               Instruction(COMMIT, len(pi) + 1),
  *               *pi]             # <<<<<<<<<<<<<<
  *     return pi
  * 
  */
-    if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 465, __pyx_L1_error)
+    if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_pi, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pe/_cy_machine.pyx":461
+    /* "pe/_cy_machine.pyx":467
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  *     for _pi in reversed(pis[:-1]):             # <<<<<<<<<<<<<<
  *         pi = [Instruction(BRANCH, len(_pi) + 2),
  *               *_pi,
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":466
+  /* "pe/_cy_machine.pyx":472
  *               Instruction(COMMIT, len(pi) + 1),
  *               *pi]
  *     return pi             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_pi);
   __pyx_r = __pyx_v_pi;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":458
+  /* "pe/_cy_machine.pyx":464
  * 
  * 
  * def _chc(defn):             # <<<<<<<<<<<<<<
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  */
 
@@ -11481,15 +11572,15 @@
   __Pyx_XDECREF(__pyx_v__pi);
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_d);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":469
+/* "pe/_cy_machine.pyx":475
  * 
  * 
  * def _rul(defn):             # <<<<<<<<<<<<<<
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  */
 
@@ -11527,30 +11618,30 @@
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_rul", 0);
 
-  /* "pe/_cy_machine.pyx":470
+  /* "pe/_cy_machine.pyx":476
  * 
  * def _rul(defn):
  *     subdefn, action, _ = defn.args             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(subdefn)
  *     if action is None:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 470, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 470, __pyx_L1_error)
+      __PYX_ERR(0, 476, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 2); 
     } else {
@@ -11558,177 +11649,177 @@
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyList_GET_ITEM(sequence, 2); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 470, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 476, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 470, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 476, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 470, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 476, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 470, __pyx_L1_error)
+    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 476, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = Py_TYPE(__pyx_t_5)->tp_iternext;
     index = 0; __pyx_t_2 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 2; __pyx_t_4 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_4)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 470, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 476, __pyx_L1_error)
     __pyx_t_6 = NULL;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 470, __pyx_L1_error)
+    __PYX_ERR(0, 476, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_subdefn = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_action = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v__ = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":471
+  /* "pe/_cy_machine.pyx":477
  * def _rul(defn):
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)             # <<<<<<<<<<<<<<
  *     if action is None:
  *         return pis
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 471, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 477, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_subdefn) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_subdefn);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 471, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 477, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_pis = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":472
+  /* "pe/_cy_machine.pyx":478
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  *     if action is None:             # <<<<<<<<<<<<<<
  *         return pis
  *     pi = pis[0]
  */
   __pyx_t_7 = (__pyx_v_action == Py_None);
   __pyx_t_8 = (__pyx_t_7 != 0);
   if (__pyx_t_8) {
 
-    /* "pe/_cy_machine.pyx":473
+    /* "pe/_cy_machine.pyx":479
  *     pis = _parsing_instructions(subdefn)
  *     if action is None:
  *         return pis             # <<<<<<<<<<<<<<
  *     pi = pis[0]
  *     if not pi.marking:
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_pis);
     __pyx_r = __pyx_v_pis;
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":472
+    /* "pe/_cy_machine.pyx":478
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  *     if action is None:             # <<<<<<<<<<<<<<
  *         return pis
  *     pi = pis[0]
  */
   }
 
-  /* "pe/_cy_machine.pyx":474
+  /* "pe/_cy_machine.pyx":480
  *     if action is None:
  *         return pis
  *     pi = pis[0]             # <<<<<<<<<<<<<<
  *     if not pi.marking:
  *         pi.marking = True
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_pi = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":475
+  /* "pe/_cy_machine.pyx":481
  *         return pis
  *     pi = pis[0]
  *     if not pi.marking:             # <<<<<<<<<<<<<<
  *         pi.marking = True
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_marking); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_marking); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 481, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 481, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_7 = ((!__pyx_t_8) != 0);
   if (__pyx_t_7) {
 
-    /* "pe/_cy_machine.pyx":476
+    /* "pe/_cy_machine.pyx":482
  *     pi = pis[0]
  *     if not pi.marking:
  *         pi.marking = True             # <<<<<<<<<<<<<<
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))
  */
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 476, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":475
+    /* "pe/_cy_machine.pyx":481
  *         return pis
  *     pi = pis[0]
  *     if not pi.marking:             # <<<<<<<<<<<<<<
  *         pi.marking = True
  *     else:
  */
     goto __pyx_L6;
   }
 
-  /* "pe/_cy_machine.pyx":478
+  /* "pe/_cy_machine.pyx":484
  *         pi.marking = True
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))             # <<<<<<<<<<<<<<
  *     pi = pis[-1]
  *     if pi.action is None and pi.opcode not in NO_CAP_OR_ACT:
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pis, __pyx_n_s_insert); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 478, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pis, __pyx_n_s_insert); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 478, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 478, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
@@ -11739,150 +11830,150 @@
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_9 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_int_0, __pyx_t_5};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 484, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_int_0, __pyx_t_5};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 484, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     {
-      __pyx_t_2 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 478, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 484, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       if (__pyx_t_3) {
         __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3); __pyx_t_3 = NULL;
       }
       __Pyx_INCREF(__pyx_int_0);
       __Pyx_GIVEREF(__pyx_int_0);
       PyTuple_SET_ITEM(__pyx_t_2, 0+__pyx_t_9, __pyx_int_0);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_2, 1+__pyx_t_9, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 484, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L6:;
 
-  /* "pe/_cy_machine.pyx":479
+  /* "pe/_cy_machine.pyx":485
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]             # <<<<<<<<<<<<<<
  *     if pi.action is None and pi.opcode not in NO_CAP_OR_ACT:
  *         pi.action = action
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 479, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF_SET(__pyx_v_pi, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":480
+  /* "pe/_cy_machine.pyx":486
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]
  *     if pi.action is None and pi.opcode not in NO_CAP_OR_ACT:             # <<<<<<<<<<<<<<
  *         pi.action = action
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_8 = (__pyx_t_1 == Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_10 = (__pyx_t_8 != 0);
   if (__pyx_t_10) {
   } else {
     __pyx_t_7 = __pyx_t_10;
     goto __pyx_L8_bool_binop_done;
   }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_NO_CAP_OR_ACT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_NO_CAP_OR_ACT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_t_4, Py_NE)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_10 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_t_4, Py_NE)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_8 = (__pyx_t_10 != 0);
   __pyx_t_7 = __pyx_t_8;
   __pyx_L8_bool_binop_done:;
   if (__pyx_t_7) {
 
-    /* "pe/_cy_machine.pyx":481
+    /* "pe/_cy_machine.pyx":487
  *     pi = pis[-1]
  *     if pi.action is None and pi.opcode not in NO_CAP_OR_ACT:
  *         pi.action = action             # <<<<<<<<<<<<<<
  *     else:
  *         pis.append(Instruction(NOOP, action=action))
  */
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_action, __pyx_v_action) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_action, __pyx_v_action) < 0) __PYX_ERR(0, 487, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":480
+    /* "pe/_cy_machine.pyx":486
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]
  *     if pi.action is None and pi.opcode not in NO_CAP_OR_ACT:             # <<<<<<<<<<<<<<
  *         pi.action = action
  *     else:
  */
     goto __pyx_L7;
   }
 
-  /* "pe/_cy_machine.pyx":483
+  /* "pe/_cy_machine.pyx":489
  *         pi.action = action
  *     else:
  *         pis.append(Instruction(NOOP, action=action))             # <<<<<<<<<<<<<<
  *     return pis
  * 
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 483, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 483, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 483, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_action, __pyx_v_action) < 0) __PYX_ERR(0, 483, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 483, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_action, __pyx_v_action) < 0) __PYX_ERR(0, 489, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_11 = __Pyx_PyObject_Append(__pyx_v_pis, __pyx_t_2); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 483, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_Append(__pyx_v_pis, __pyx_t_2); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L7:;
 
-  /* "pe/_cy_machine.pyx":484
+  /* "pe/_cy_machine.pyx":490
  *     else:
  *         pis.append(Instruction(NOOP, action=action))
  *     return pis             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_pis);
   __pyx_r = __pyx_v_pis;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":469
+  /* "pe/_cy_machine.pyx":475
  * 
  * 
  * def _rul(defn):             # <<<<<<<<<<<<<<
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  */
 
@@ -11902,15 +11993,15 @@
   __Pyx_XDECREF(__pyx_v_pis);
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":506
+/* "pe/_cy_machine.pyx":512
  * 
  * 
  * def _parsing_instructions(defn):  # noqa: C901             # <<<<<<<<<<<<<<
  *     try:
  *         return _op_map[defn.op](defn)
  */
 
@@ -11943,15 +12034,15 @@
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parsing_instructions", 0);
 
-  /* "pe/_cy_machine.pyx":507
+  /* "pe/_cy_machine.pyx":513
  * 
  * def _parsing_instructions(defn):  # noqa: C901
  *     try:             # <<<<<<<<<<<<<<
  *         return _op_map[defn.op](defn)
  *     except KeyError:
  */
   {
@@ -11959,27 +12050,27 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "pe/_cy_machine.pyx":508
+      /* "pe/_cy_machine.pyx":514
  * def _parsing_instructions(defn):  # noqa: C901
  *     try:
  *         return _op_map[defn.op](defn)             # <<<<<<<<<<<<<<
  *     except KeyError:
  *         raise Error(f'invalid definition: {defn!r}')
  */
       __Pyx_XDECREF(__pyx_r);
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_op_map); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 508, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_op_map); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 514, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_op); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 508, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_op); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 514, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 508, __pyx_L3_error)
+      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 514, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_6)) {
@@ -11987,62 +12078,62 @@
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
       __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_6, __pyx_v_defn) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_defn);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L3_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_r = __pyx_t_4;
       __pyx_t_4 = 0;
       goto __pyx_L7_try_return;
 
-      /* "pe/_cy_machine.pyx":507
+      /* "pe/_cy_machine.pyx":513
  * 
  * def _parsing_instructions(defn):  # noqa: C901
  *     try:             # <<<<<<<<<<<<<<
  *         return _op_map[defn.op](defn)
  *     except KeyError:
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "pe/_cy_machine.pyx":509
+    /* "pe/_cy_machine.pyx":515
  *     try:
  *         return _op_map[defn.op](defn)
  *     except KeyError:             # <<<<<<<<<<<<<<
  *         raise Error(f'invalid definition: {defn!r}')
  * 
  */
     __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
     if (__pyx_t_8) {
       __Pyx_AddTraceback("pe._cy_machine._parsing_instructions", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_7, &__pyx_t_6) < 0) __PYX_ERR(0, 509, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_7, &__pyx_t_6) < 0) __PYX_ERR(0, 515, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_6);
 
-      /* "pe/_cy_machine.pyx":510
+      /* "pe/_cy_machine.pyx":516
  *         return _op_map[defn.op](defn)
  *     except KeyError:
  *         raise Error(f'invalid definition: {defn!r}')             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_Error); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 510, __pyx_L5_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_Error); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 516, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(__pyx_v_defn), __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 510, __pyx_L5_except_error)
+      __pyx_t_10 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(__pyx_v_defn), __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 516, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_invalid_definition, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 510, __pyx_L5_except_error)
+      __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_invalid_definition, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 516, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -12050,25 +12141,25 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_5 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 510, __pyx_L5_except_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 516, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(0, 510, __pyx_L5_except_error)
+      __PYX_ERR(0, 516, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "pe/_cy_machine.pyx":507
+    /* "pe/_cy_machine.pyx":513
  * 
  * def _parsing_instructions(defn):  # noqa: C901
  *     try:             # <<<<<<<<<<<<<<
  *         return _op_map[defn.op](defn)
  *     except KeyError:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -12080,15 +12171,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "pe/_cy_machine.pyx":506
+  /* "pe/_cy_machine.pyx":512
  * 
  * 
  * def _parsing_instructions(defn):  # noqa: C901             # <<<<<<<<<<<<<<
  *     try:
  *         return _op_map[defn.op](defn)
  */
 
@@ -12105,68 +12196,68 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":516
+/* "pe/_cy_machine.pyx":522
  * 
  * cdef class Dot(Scanner):
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         if pos < slen:
  *             return pos + 1
  */
 
 static int __pyx_f_2pe_11_cy_machine_3Dot__scan(CYTHON_UNUSED struct __pyx_obj_2pe_11_cy_machine_Dot *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_s, int __pyx_v_pos, int __pyx_v_slen) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("_scan", 0);
 
-  /* "pe/_cy_machine.pyx":517
+  /* "pe/_cy_machine.pyx":523
  * cdef class Dot(Scanner):
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         if pos < slen:             # <<<<<<<<<<<<<<
  *             return pos + 1
  *         return FAILURE
  */
   __pyx_t_1 = ((__pyx_v_pos < __pyx_v_slen) != 0);
   if (__pyx_t_1) {
 
-    /* "pe/_cy_machine.pyx":518
+    /* "pe/_cy_machine.pyx":524
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         if pos < slen:
  *             return pos + 1             # <<<<<<<<<<<<<<
  *         return FAILURE
  * 
  */
     __pyx_r = (__pyx_v_pos + 1);
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":517
+    /* "pe/_cy_machine.pyx":523
  * cdef class Dot(Scanner):
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         if pos < slen:             # <<<<<<<<<<<<<<
  *             return pos + 1
  *         return FAILURE
  */
   }
 
-  /* "pe/_cy_machine.pyx":519
+  /* "pe/_cy_machine.pyx":525
  *         if pos < slen:
  *             return pos + 1
  *         return FAILURE             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = -1;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":516
+  /* "pe/_cy_machine.pyx":522
  * 
  * cdef class Dot(Scanner):
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         if pos < slen:
  *             return pos + 1
  */
 
@@ -12459,15 +12550,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":526
+/* "pe/_cy_machine.pyx":532
  *     cdef int _xlen
  * 
  *     def __init__(self, str x):             # <<<<<<<<<<<<<<
  *         self._x = x
  *         self._xlen = len(x)
  */
 
@@ -12496,32 +12587,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_x)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 526, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 532, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_x = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 526, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 532, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine.Literal.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_x), (&PyUnicode_Type), 1, "x", 1))) __PYX_ERR(0, 526, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_x), (&PyUnicode_Type), 1, "x", 1))) __PYX_ERR(0, 532, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_7Literal___init__(((struct __pyx_obj_2pe_11_cy_machine_Literal *)__pyx_v_self), __pyx_v_x);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -12534,42 +12625,42 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pe/_cy_machine.pyx":527
+  /* "pe/_cy_machine.pyx":533
  * 
  *     def __init__(self, str x):
  *         self._x = x             # <<<<<<<<<<<<<<
  *         self._xlen = len(x)
  * 
  */
   __Pyx_INCREF(__pyx_v_x);
   __Pyx_GIVEREF(__pyx_v_x);
   __Pyx_GOTREF(__pyx_v_self->_x);
   __Pyx_DECREF(__pyx_v_self->_x);
   __pyx_v_self->_x = __pyx_v_x;
 
-  /* "pe/_cy_machine.pyx":528
+  /* "pe/_cy_machine.pyx":534
  *     def __init__(self, str x):
  *         self._x = x
  *         self._xlen = len(x)             # <<<<<<<<<<<<<<
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  */
   if (unlikely(__pyx_v_x == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 528, __pyx_L1_error)
+    __PYX_ERR(0, 534, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_x); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_x); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 534, __pyx_L1_error)
   __pyx_v_self->_xlen = __pyx_t_1;
 
-  /* "pe/_cy_machine.pyx":526
+  /* "pe/_cy_machine.pyx":532
  *     cdef int _xlen
  * 
  *     def __init__(self, str x):             # <<<<<<<<<<<<<<
  *         self._x = x
  *         self._xlen = len(x)
  */
 
@@ -12580,15 +12671,15 @@
   __Pyx_AddTraceback("pe._cy_machine.Literal.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":530
+/* "pe/_cy_machine.pyx":536
  *         self._xlen = len(x)
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         cdef int end = pos + self._xlen
  *         if s[pos:end] != self._x:
  */
 
@@ -12600,71 +12691,71 @@
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_scan", 0);
 
-  /* "pe/_cy_machine.pyx":531
+  /* "pe/_cy_machine.pyx":537
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         cdef int end = pos + self._xlen             # <<<<<<<<<<<<<<
  *         if s[pos:end] != self._x:
  *             return FAILURE
  */
   __pyx_v_end = (__pyx_v_pos + __pyx_v_self->_xlen);
 
-  /* "pe/_cy_machine.pyx":532
+  /* "pe/_cy_machine.pyx":538
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         cdef int end = pos + self._xlen
  *         if s[pos:end] != self._x:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         return end
  */
   if (unlikely(__pyx_v_s == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 532, __pyx_L1_error)
+    __PYX_ERR(0, 538, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_v_s, __pyx_v_pos, __pyx_v_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_v_s, __pyx_v_pos, __pyx_v_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_v_self->_x, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 532, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_v_self->_x, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "pe/_cy_machine.pyx":533
+    /* "pe/_cy_machine.pyx":539
  *         cdef int end = pos + self._xlen
  *         if s[pos:end] != self._x:
  *             return FAILURE             # <<<<<<<<<<<<<<
  *         return end
  * 
  */
     __pyx_r = -1;
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":532
+    /* "pe/_cy_machine.pyx":538
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         cdef int end = pos + self._xlen
  *         if s[pos:end] != self._x:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         return end
  */
   }
 
-  /* "pe/_cy_machine.pyx":534
+  /* "pe/_cy_machine.pyx":540
  *         if s[pos:end] != self._x:
  *             return FAILURE
  *         return end             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_end;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":530
+  /* "pe/_cy_machine.pyx":536
  *         self._xlen = len(x)
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         cdef int end = pos + self._xlen
  *         if s[pos:end] != self._x:
  */
 
@@ -12972,15 +13063,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":545
+/* "pe/_cy_machine.pyx":551
  *         int mincount, maxcount
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         list ranges,
  */
 
@@ -13036,15 +13127,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_maxcount);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 545, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 551, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -13053,49 +13144,49 @@
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_ranges = ((PyObject*)values[0]);
     if (values[1]) {
-      __pyx_v_negate = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_negate == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 548, __pyx_L3_error)
+      __pyx_v_negate = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_negate == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 554, __pyx_L3_error)
     } else {
 
-      /* "pe/_cy_machine.pyx":548
+      /* "pe/_cy_machine.pyx":554
  *         self,
  *         list ranges,
  *         bint negate = False,             # <<<<<<<<<<<<<<
  *         int mincount = 1,
  *         int maxcount = 1
  */
       __pyx_v_negate = ((int)0);
     }
     if (values[2]) {
-      __pyx_v_mincount = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_mincount == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 549, __pyx_L3_error)
+      __pyx_v_mincount = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_mincount == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 555, __pyx_L3_error)
     } else {
       __pyx_v_mincount = ((int)1);
     }
     if (values[3]) {
-      __pyx_v_maxcount = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_maxcount == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 550, __pyx_L3_error)
+      __pyx_v_maxcount = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_maxcount == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 556, __pyx_L3_error)
     } else {
       __pyx_v_maxcount = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 545, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 551, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine.CharacterClass.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ranges), (&PyList_Type), 1, "ranges", 1))) __PYX_ERR(0, 547, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ranges), (&PyList_Type), 1, "ranges", 1))) __PYX_ERR(0, 553, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_14CharacterClass___init__(((struct __pyx_obj_2pe_11_cy_machine_CharacterClass *)__pyx_v_self), __pyx_v_ranges, __pyx_v_negate, __pyx_v_mincount, __pyx_v_maxcount);
 
-  /* "pe/_cy_machine.pyx":545
+  /* "pe/_cy_machine.pyx":551
  *         int mincount, maxcount
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         list ranges,
  */
 
@@ -13105,15 +13196,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pe/_cy_machine.pyx":552
+/* "pe/_cy_machine.pyx":558
  *         int maxcount = 1
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)             # <<<<<<<<<<<<<<
  *         self._ranges = ''.join(a+b for a, b in ranges if b)
  *         self._rangelen = len(self._ranges)
  */
 
@@ -13125,23 +13216,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr *)__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_1_genexpr(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 552, __pyx_L1_error)
+    __PYX_ERR(0, 558, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct____init__ *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_init___locals_genexpr, __pyx_n_s_pe__cy_machine); if (unlikely(!gen)) __PYX_ERR(0, 552, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_init___locals_genexpr, __pyx_n_s_pe__cy_machine); if (unlikely(!gen)) __PYX_ERR(0, 558, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13174,89 +13265,89 @@
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 552, __pyx_L1_error)
-  __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 552, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 558, __pyx_L1_error)
+  __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_r);
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_ranges)) { __Pyx_RaiseClosureNameError("ranges"); __PYX_ERR(0, 552, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_ranges)) { __Pyx_RaiseClosureNameError("ranges"); __PYX_ERR(0, 558, __pyx_L1_error) }
   if (unlikely(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_ranges == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 552, __pyx_L1_error)
+    __PYX_ERR(0, 558, __pyx_L1_error)
   }
   __pyx_t_1 = __pyx_cur_scope->__pyx_outer_scope->__pyx_v_ranges; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
   for (;;) {
     if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 552, __pyx_L1_error)
+    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 558, __pyx_L1_error)
     #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 552, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 558, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
       PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 552, __pyx_L1_error)
+        __PYX_ERR(0, 558, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       #else
-      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 552, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 552, __pyx_L1_error)
+      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       #endif
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 552, __pyx_L1_error)
+      __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_7 = Py_TYPE(__pyx_t_6)->tp_iternext;
       index = 0; __pyx_t_4 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_4)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
       index = 1; __pyx_t_5 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_5)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_5);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 552, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 558, __pyx_L1_error)
       __pyx_t_7 = NULL;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L7_unpacking_done;
       __pyx_L6_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 552, __pyx_L1_error)
+      __PYX_ERR(0, 558, __pyx_L1_error)
       __pyx_L7_unpacking_done:;
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_a);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_a, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_b);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_b, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_b); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 552, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_b); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 558, __pyx_L1_error)
     __pyx_t_9 = ((!__pyx_t_8) != 0);
     if (__pyx_t_9) {
-      if (unlikely(__Pyx_ListComp_Append(__pyx_r, (PyObject*)__pyx_cur_scope->__pyx_v_a))) __PYX_ERR(0, 552, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_r, (PyObject*)__pyx_cur_scope->__pyx_v_a))) __PYX_ERR(0, 558, __pyx_L1_error)
     }
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   goto __pyx_L0;
@@ -13276,15 +13367,15 @@
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___5generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pe/_cy_machine.pyx":553
+/* "pe/_cy_machine.pyx":559
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)
  *         self._ranges = ''.join(a+b for a, b in ranges if b)             # <<<<<<<<<<<<<<
  *         self._rangelen = len(self._ranges)
  *         self._negate = negate
  */
 
@@ -13296,23 +13387,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr *)__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_2_genexpr(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 553, __pyx_L1_error)
+    __PYX_ERR(0, 559, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct____init__ *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___5generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_init___locals_genexpr, __pyx_n_s_pe__cy_machine); if (unlikely(!gen)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___5generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_init___locals_genexpr, __pyx_n_s_pe__cy_machine); if (unlikely(!gen)) __PYX_ERR(0, 559, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13344,90 +13435,90 @@
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 553, __pyx_L1_error)
-  __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 553, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_r);
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_ranges)) { __Pyx_RaiseClosureNameError("ranges"); __PYX_ERR(0, 553, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_ranges)) { __Pyx_RaiseClosureNameError("ranges"); __PYX_ERR(0, 559, __pyx_L1_error) }
   if (unlikely(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_ranges == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 553, __pyx_L1_error)
+    __PYX_ERR(0, 559, __pyx_L1_error)
   }
   __pyx_t_1 = __pyx_cur_scope->__pyx_outer_scope->__pyx_v_ranges; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
   for (;;) {
     if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 559, __pyx_L1_error)
     #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 559, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
       PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 553, __pyx_L1_error)
+        __PYX_ERR(0, 559, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       #else
-      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 553, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 559, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 553, __pyx_L1_error)
+      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 559, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       #endif
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 553, __pyx_L1_error)
+      __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 559, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_7 = Py_TYPE(__pyx_t_6)->tp_iternext;
       index = 0; __pyx_t_4 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_4)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
       index = 1; __pyx_t_5 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_5)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_5);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 559, __pyx_L1_error)
       __pyx_t_7 = NULL;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L7_unpacking_done;
       __pyx_L6_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 553, __pyx_L1_error)
+      __PYX_ERR(0, 559, __pyx_L1_error)
       __pyx_L7_unpacking_done:;
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_a);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_a, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_b);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_b, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_b); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 553, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_b); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 559, __pyx_L1_error)
     if (__pyx_t_8) {
-      __pyx_t_3 = PyNumber_Add(__pyx_cur_scope->__pyx_v_a, __pyx_cur_scope->__pyx_v_b); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 553, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_cur_scope->__pyx_v_a, __pyx_cur_scope->__pyx_v_b); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 559, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_r, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 553, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_r, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 559, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
@@ -13447,15 +13538,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":545
+/* "pe/_cy_machine.pyx":551
  *         int mincount, maxcount
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         list ranges,
  */
 
@@ -13472,109 +13563,109 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
   __pyx_cur_scope = (struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct____init__ *)__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct____init__(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct____init__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct____init__ *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 545, __pyx_L1_error)
+    __PYX_ERR(0, 551, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_ranges = __pyx_v_ranges;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_ranges);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_ranges);
 
-  /* "pe/_cy_machine.pyx":552
+  /* "pe/_cy_machine.pyx":558
  *         int maxcount = 1
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)             # <<<<<<<<<<<<<<
  *         self._ranges = ''.join(a+b for a, b in ranges if b)
  *         self._rangelen = len(self._ranges)
  */
-  __pyx_t_1 = __pyx_pf_2pe_11_cy_machine_14CharacterClass_8__init___genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 552, __pyx_L1_error)
+  __pyx_t_1 = __pyx_pf_2pe_11_cy_machine_14CharacterClass_8__init___genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 552, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 552, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_chars);
   __Pyx_DECREF(__pyx_v_self->_chars);
   __pyx_v_self->_chars = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":553
+  /* "pe/_cy_machine.pyx":559
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)
  *         self._ranges = ''.join(a+b for a, b in ranges if b)             # <<<<<<<<<<<<<<
  *         self._rangelen = len(self._ranges)
  *         self._negate = negate
  */
-  __pyx_t_1 = __pyx_pf_2pe_11_cy_machine_14CharacterClass_8__init___3genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 553, __pyx_L1_error)
+  __pyx_t_1 = __pyx_pf_2pe_11_cy_machine_14CharacterClass_8__init___3genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 553, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 553, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_ranges);
   __Pyx_DECREF(__pyx_v_self->_ranges);
   __pyx_v_self->_ranges = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":554
+  /* "pe/_cy_machine.pyx":560
  *         self._chars = ''.join(a for a, b in ranges if not b)
  *         self._ranges = ''.join(a+b for a, b in ranges if b)
  *         self._rangelen = len(self._ranges)             # <<<<<<<<<<<<<<
  *         self._negate = negate
  *         self.mincount = mincount
  */
   __pyx_t_1 = __pyx_v_self->_ranges;
   __Pyx_INCREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 554, __pyx_L1_error)
+    __PYX_ERR(0, 560, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 554, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->_rangelen = __pyx_t_3;
 
-  /* "pe/_cy_machine.pyx":555
+  /* "pe/_cy_machine.pyx":561
  *         self._ranges = ''.join(a+b for a, b in ranges if b)
  *         self._rangelen = len(self._ranges)
  *         self._negate = negate             # <<<<<<<<<<<<<<
  *         self.mincount = mincount
  *         self.maxcount = maxcount
  */
   __pyx_v_self->_negate = __pyx_v_negate;
 
-  /* "pe/_cy_machine.pyx":556
+  /* "pe/_cy_machine.pyx":562
  *         self._rangelen = len(self._ranges)
  *         self._negate = negate
  *         self.mincount = mincount             # <<<<<<<<<<<<<<
  *         self.maxcount = maxcount
  * 
  */
   __pyx_v_self->mincount = __pyx_v_mincount;
 
-  /* "pe/_cy_machine.pyx":557
+  /* "pe/_cy_machine.pyx":563
  *         self._negate = negate
  *         self.mincount = mincount
  *         self.maxcount = maxcount             # <<<<<<<<<<<<<<
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  */
   __pyx_v_self->maxcount = __pyx_v_maxcount;
 
-  /* "pe/_cy_machine.pyx":545
+  /* "pe/_cy_machine.pyx":551
  *         int mincount, maxcount
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         list ranges,
  */
 
@@ -13590,15 +13681,15 @@
   __Pyx_XDECREF(__pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___2generator);
   __Pyx_XDECREF(__pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___5generator1);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":559
+/* "pe/_cy_machine.pyx":565
  *         self.maxcount = maxcount
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         cdef Py_UCS4 c
  *         cdef str ranges = self._ranges
  */
 
@@ -13619,56 +13710,56 @@
   long __pyx_t_6;
   Py_UCS4 __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_scan", 0);
 
-  /* "pe/_cy_machine.pyx":561
+  /* "pe/_cy_machine.pyx":567
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         cdef Py_UCS4 c
  *         cdef str ranges = self._ranges             # <<<<<<<<<<<<<<
  *         cdef bint matched
  *         cdef int mincount = self.mincount
  */
   __pyx_t_1 = __pyx_v_self->_ranges;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_ranges = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":563
+  /* "pe/_cy_machine.pyx":569
  *         cdef str ranges = self._ranges
  *         cdef bint matched
  *         cdef int mincount = self.mincount             # <<<<<<<<<<<<<<
  *         cdef int maxcount = self.maxcount
  *         cdef int i = 0
  */
   __pyx_t_2 = __pyx_v_self->mincount;
   __pyx_v_mincount = __pyx_t_2;
 
-  /* "pe/_cy_machine.pyx":564
+  /* "pe/_cy_machine.pyx":570
  *         cdef bint matched
  *         cdef int mincount = self.mincount
  *         cdef int maxcount = self.maxcount             # <<<<<<<<<<<<<<
  *         cdef int i = 0
  *         while maxcount and pos < slen:
  */
   __pyx_t_2 = __pyx_v_self->maxcount;
   __pyx_v_maxcount = __pyx_t_2;
 
-  /* "pe/_cy_machine.pyx":565
+  /* "pe/_cy_machine.pyx":571
  *         cdef int mincount = self.mincount
  *         cdef int maxcount = self.maxcount
  *         cdef int i = 0             # <<<<<<<<<<<<<<
  *         while maxcount and pos < slen:
  *             c = s[pos]
  */
   __pyx_v_i = 0;
 
-  /* "pe/_cy_machine.pyx":566
+  /* "pe/_cy_machine.pyx":572
  *         cdef int maxcount = self.maxcount
  *         cdef int i = 0
  *         while maxcount and pos < slen:             # <<<<<<<<<<<<<<
  *             c = s[pos]
  *             matched = False
  */
   while (1) {
@@ -13679,245 +13770,245 @@
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_4 = ((__pyx_v_pos < __pyx_v_slen) != 0);
     __pyx_t_3 = __pyx_t_4;
     __pyx_L5_bool_binop_done:;
     if (!__pyx_t_3) break;
 
-    /* "pe/_cy_machine.pyx":567
+    /* "pe/_cy_machine.pyx":573
  *         cdef int i = 0
  *         while maxcount and pos < slen:
  *             c = s[pos]             # <<<<<<<<<<<<<<
  *             matched = False
  *             if c in self._chars:
  */
-    __pyx_t_5 = __Pyx_GetItemInt_Unicode(__pyx_v_s, __pyx_v_pos, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_5 == (Py_UCS4)-1)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt_Unicode(__pyx_v_s, __pyx_v_pos, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_5 == (Py_UCS4)-1)) __PYX_ERR(0, 573, __pyx_L1_error)
     __pyx_v_c = __pyx_t_5;
 
-    /* "pe/_cy_machine.pyx":568
+    /* "pe/_cy_machine.pyx":574
  *         while maxcount and pos < slen:
  *             c = s[pos]
  *             matched = False             # <<<<<<<<<<<<<<
  *             if c in self._chars:
  *                 matched = True
  */
     __pyx_v_matched = 0;
 
-    /* "pe/_cy_machine.pyx":569
+    /* "pe/_cy_machine.pyx":575
  *             c = s[pos]
  *             matched = False
  *             if c in self._chars:             # <<<<<<<<<<<<<<
  *                 matched = True
  *             else:
  */
     if (unlikely(__pyx_v_self->_chars == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument of type 'NoneType' is not iterable");
-      __PYX_ERR(0, 569, __pyx_L1_error)
+      __PYX_ERR(0, 575, __pyx_L1_error)
     }
     __pyx_t_3 = ((__Pyx_UnicodeContainsUCS4(__pyx_v_self->_chars, __pyx_v_c)) != 0);
     if (__pyx_t_3) {
 
-      /* "pe/_cy_machine.pyx":570
+      /* "pe/_cy_machine.pyx":576
  *             matched = False
  *             if c in self._chars:
  *                 matched = True             # <<<<<<<<<<<<<<
  *             else:
  *                 while i < self._rangelen:
  */
       __pyx_v_matched = 1;
 
-      /* "pe/_cy_machine.pyx":569
+      /* "pe/_cy_machine.pyx":575
  *             c = s[pos]
  *             matched = False
  *             if c in self._chars:             # <<<<<<<<<<<<<<
  *                 matched = True
  *             else:
  */
       goto __pyx_L7;
     }
 
-    /* "pe/_cy_machine.pyx":572
+    /* "pe/_cy_machine.pyx":578
  *                 matched = True
  *             else:
  *                 while i < self._rangelen:             # <<<<<<<<<<<<<<
  *                     if ranges[i] <= c <= ranges[i+1]:
  *                         matched = True
  */
     /*else*/ {
       while (1) {
         __pyx_t_3 = ((__pyx_v_i < __pyx_v_self->_rangelen) != 0);
         if (!__pyx_t_3) break;
 
-        /* "pe/_cy_machine.pyx":573
+        /* "pe/_cy_machine.pyx":579
  *             else:
  *                 while i < self._rangelen:
  *                     if ranges[i] <= c <= ranges[i+1]:             # <<<<<<<<<<<<<<
  *                         matched = True
  *                         break
  */
-        __pyx_t_5 = __Pyx_GetItemInt_Unicode(__pyx_v_ranges, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_5 == (Py_UCS4)-1)) __PYX_ERR(0, 573, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_GetItemInt_Unicode(__pyx_v_ranges, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_5 == (Py_UCS4)-1)) __PYX_ERR(0, 579, __pyx_L1_error)
         __pyx_t_3 = (__pyx_t_5 <= __pyx_v_c);
         if (__pyx_t_3) {
           __pyx_t_6 = (__pyx_v_i + 1);
-          __pyx_t_7 = __Pyx_GetItemInt_Unicode(__pyx_v_ranges, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(__pyx_t_7 == (Py_UCS4)-1)) __PYX_ERR(0, 573, __pyx_L1_error)
+          __pyx_t_7 = __Pyx_GetItemInt_Unicode(__pyx_v_ranges, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(__pyx_t_7 == (Py_UCS4)-1)) __PYX_ERR(0, 579, __pyx_L1_error)
           __pyx_t_3 = (__pyx_v_c <= __pyx_t_7);
         }
         __pyx_t_4 = (__pyx_t_3 != 0);
         if (__pyx_t_4) {
 
-          /* "pe/_cy_machine.pyx":574
+          /* "pe/_cy_machine.pyx":580
  *                 while i < self._rangelen:
  *                     if ranges[i] <= c <= ranges[i+1]:
  *                         matched = True             # <<<<<<<<<<<<<<
  *                         break
  *                     i += 2
  */
           __pyx_v_matched = 1;
 
-          /* "pe/_cy_machine.pyx":575
+          /* "pe/_cy_machine.pyx":581
  *                     if ranges[i] <= c <= ranges[i+1]:
  *                         matched = True
  *                         break             # <<<<<<<<<<<<<<
  *                     i += 2
  *             if matched ^ self._negate:
  */
           goto __pyx_L9_break;
 
-          /* "pe/_cy_machine.pyx":573
+          /* "pe/_cy_machine.pyx":579
  *             else:
  *                 while i < self._rangelen:
  *                     if ranges[i] <= c <= ranges[i+1]:             # <<<<<<<<<<<<<<
  *                         matched = True
  *                         break
  */
         }
 
-        /* "pe/_cy_machine.pyx":576
+        /* "pe/_cy_machine.pyx":582
  *                         matched = True
  *                         break
  *                     i += 2             # <<<<<<<<<<<<<<
  *             if matched ^ self._negate:
  *                 pos += 1
  */
         __pyx_v_i = (__pyx_v_i + 2);
       }
       __pyx_L9_break:;
     }
     __pyx_L7:;
 
-    /* "pe/_cy_machine.pyx":577
+    /* "pe/_cy_machine.pyx":583
  *                         break
  *                     i += 2
  *             if matched ^ self._negate:             # <<<<<<<<<<<<<<
  *                 pos += 1
  *                 maxcount -= 1
  */
     __pyx_t_4 = ((__pyx_v_matched ^ __pyx_v_self->_negate) != 0);
     if (__pyx_t_4) {
 
-      /* "pe/_cy_machine.pyx":578
+      /* "pe/_cy_machine.pyx":584
  *                     i += 2
  *             if matched ^ self._negate:
  *                 pos += 1             # <<<<<<<<<<<<<<
  *                 maxcount -= 1
  *                 mincount -= 1
  */
       __pyx_v_pos = (__pyx_v_pos + 1);
 
-      /* "pe/_cy_machine.pyx":579
+      /* "pe/_cy_machine.pyx":585
  *             if matched ^ self._negate:
  *                 pos += 1
  *                 maxcount -= 1             # <<<<<<<<<<<<<<
  *                 mincount -= 1
  *                 i = 0
  */
       __pyx_v_maxcount = (__pyx_v_maxcount - 1);
 
-      /* "pe/_cy_machine.pyx":580
+      /* "pe/_cy_machine.pyx":586
  *                 pos += 1
  *                 maxcount -= 1
  *                 mincount -= 1             # <<<<<<<<<<<<<<
  *                 i = 0
  *             else:
  */
       __pyx_v_mincount = (__pyx_v_mincount - 1);
 
-      /* "pe/_cy_machine.pyx":581
+      /* "pe/_cy_machine.pyx":587
  *                 maxcount -= 1
  *                 mincount -= 1
  *                 i = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 break
  */
       __pyx_v_i = 0;
 
-      /* "pe/_cy_machine.pyx":577
+      /* "pe/_cy_machine.pyx":583
  *                         break
  *                     i += 2
  *             if matched ^ self._negate:             # <<<<<<<<<<<<<<
  *                 pos += 1
  *                 maxcount -= 1
  */
       goto __pyx_L11;
     }
 
-    /* "pe/_cy_machine.pyx":583
+    /* "pe/_cy_machine.pyx":589
  *                 i = 0
  *             else:
  *                 break             # <<<<<<<<<<<<<<
  *         if mincount > 0:
  *             return FAILURE
  */
     /*else*/ {
       goto __pyx_L4_break;
     }
     __pyx_L11:;
   }
   __pyx_L4_break:;
 
-  /* "pe/_cy_machine.pyx":584
+  /* "pe/_cy_machine.pyx":590
  *             else:
  *                 break
  *         if mincount > 0:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         return pos
  */
   __pyx_t_4 = ((__pyx_v_mincount > 0) != 0);
   if (__pyx_t_4) {
 
-    /* "pe/_cy_machine.pyx":585
+    /* "pe/_cy_machine.pyx":591
  *                 break
  *         if mincount > 0:
  *             return FAILURE             # <<<<<<<<<<<<<<
  *         return pos
  * 
  */
     __pyx_r = -1;
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":584
+    /* "pe/_cy_machine.pyx":590
  *             else:
  *                 break
  *         if mincount > 0:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         return pos
  */
   }
 
-  /* "pe/_cy_machine.pyx":586
+  /* "pe/_cy_machine.pyx":592
  *         if mincount > 0:
  *             return FAILURE
  *         return pos             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_pos;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":559
+  /* "pe/_cy_machine.pyx":565
  *         self.maxcount = maxcount
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         cdef Py_UCS4 c
  *         cdef str ranges = self._ranges
  */
 
@@ -13928,15 +14019,15 @@
   __pyx_r = -2;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ranges);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":543
+/* "pe/_cy_machine.pyx":549
  *         bint _negate
  *     cdef public:
  *         int mincount, maxcount             # <<<<<<<<<<<<<<
  * 
  *     def __init__(
  */
 
@@ -13958,15 +14049,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->mincount); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->mincount); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 549, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13996,15 +14087,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 549, __pyx_L1_error)
   __pyx_v_self->mincount = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pe._cy_machine.CharacterClass.mincount.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -14032,15 +14123,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->maxcount); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->maxcount); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 549, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14070,15 +14161,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 549, __pyx_L1_error)
   __pyx_v_self->maxcount = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pe._cy_machine.CharacterClass.maxcount.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -14415,15 +14506,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":592
+/* "pe/_cy_machine.pyx":598
  *     cdef object _regex
  * 
  *     def __init__(self, str pattern, int flags=0):             # <<<<<<<<<<<<<<
  *         self._regex = re.compile(pattern, flags=flags)
  * 
  */
 
@@ -14461,41 +14552,41 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flags);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 592, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 598, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_pattern = ((PyObject*)values[0]);
     if (values[1]) {
-      __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 592, __pyx_L3_error)
+      __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 598, __pyx_L3_error)
     } else {
       __pyx_v_flags = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 592, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 598, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pe._cy_machine.Regex.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pattern), (&PyUnicode_Type), 1, "pattern", 1))) __PYX_ERR(0, 592, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pattern), (&PyUnicode_Type), 1, "pattern", 1))) __PYX_ERR(0, 598, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_5Regex___init__(((struct __pyx_obj_2pe_11_cy_machine_Regex *)__pyx_v_self), __pyx_v_pattern, __pyx_v_flags);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -14511,49 +14602,49 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pe/_cy_machine.pyx":593
+  /* "pe/_cy_machine.pyx":599
  * 
  *     def __init__(self, str pattern, int flags=0):
  *         self._regex = re.compile(pattern, flags=flags)             # <<<<<<<<<<<<<<
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_re); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_re); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_compile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_compile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_pattern);
   __Pyx_GIVEREF(__pyx_v_pattern);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_pattern);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flags, __pyx_t_4) < 0) __PYX_ERR(0, 593, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flags, __pyx_t_4) < 0) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->_regex);
   __Pyx_DECREF(__pyx_v_self->_regex);
   __pyx_v_self->_regex = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":592
+  /* "pe/_cy_machine.pyx":598
  *     cdef object _regex
  * 
  *     def __init__(self, str pattern, int flags=0):             # <<<<<<<<<<<<<<
  *         self._regex = re.compile(pattern, flags=flags)
  * 
  */
 
@@ -14568,15 +14659,15 @@
   __Pyx_AddTraceback("pe._cy_machine.Regex.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":595
+/* "pe/_cy_machine.pyx":601
  *         self._regex = re.compile(pattern, flags=flags)
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         m = self._regex.match(s, pos=pos)
  *         if m is None:
  */
 
@@ -14592,104 +14683,104 @@
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_scan", 0);
 
-  /* "pe/_cy_machine.pyx":596
+  /* "pe/_cy_machine.pyx":602
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         m = self._regex.match(s, pos=pos)             # <<<<<<<<<<<<<<
  *         if m is None:
  *             return FAILURE
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_regex, __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_regex, __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_s);
   __Pyx_GIVEREF(__pyx_v_s);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_s);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_pos, __pyx_t_4) < 0) __PYX_ERR(0, 596, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_pos, __pyx_t_4) < 0) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_m = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":597
+  /* "pe/_cy_machine.pyx":603
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         m = self._regex.match(s, pos=pos)
  *         if m is None:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         else:
  */
   __pyx_t_5 = (__pyx_v_m == Py_None);
   __pyx_t_6 = (__pyx_t_5 != 0);
   if (__pyx_t_6) {
 
-    /* "pe/_cy_machine.pyx":598
+    /* "pe/_cy_machine.pyx":604
  *         m = self._regex.match(s, pos=pos)
  *         if m is None:
  *             return FAILURE             # <<<<<<<<<<<<<<
  *         else:
  *             return m.end()
  */
     __pyx_r = -1;
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":597
+    /* "pe/_cy_machine.pyx":603
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         m = self._regex.match(s, pos=pos)
  *         if m is None:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         else:
  */
   }
 
-  /* "pe/_cy_machine.pyx":600
+  /* "pe/_cy_machine.pyx":606
  *             return FAILURE
  *         else:
  *             return m.end()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_m, __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_m, __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 600, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_7;
     goto __pyx_L0;
   }
 
-  /* "pe/_cy_machine.pyx":595
+  /* "pe/_cy_machine.pyx":601
  *         self._regex = re.compile(pattern, flags=flags)
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         m = self._regex.match(s, pos=pos)
  *         if m is None:
  */
 
@@ -17906,15 +17997,15 @@
   p = ((struct __pyx_obj_2pe_11_cy_machine_Scanner *)o);
   p->__pyx_vtab = __pyx_vtabptr_2pe_11_cy_machine_Scanner;
   return o;
 }
 
 static void __pyx_tp_dealloc_2pe_11_cy_machine_Scanner(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_2pe_11_cy_machine_Scanner[] = {
@@ -18011,15 +18102,15 @@
   p->name = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_2pe_11_cy_machine_Instruction(PyObject *o) {
   struct __pyx_obj_2pe_11_cy_machine_Instruction *p = (struct __pyx_obj_2pe_11_cy_machine_Instruction *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->scanner);
   Py_CLEAR(p->action);
   Py_CLEAR(p->name);
@@ -18249,15 +18340,15 @@
   p->pi = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_2pe_11_cy_machine__Parser(PyObject *o) {
   struct __pyx_obj_2pe_11_cy_machine__Parser *p = (struct __pyx_obj_2pe_11_cy_machine__Parser *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->pi);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -18457,15 +18548,15 @@
   p->_x = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_2pe_11_cy_machine_Literal(PyObject *o) {
   struct __pyx_obj_2pe_11_cy_machine_Literal *p = (struct __pyx_obj_2pe_11_cy_machine_Literal *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->_x);
   __pyx_tp_dealloc_2pe_11_cy_machine_Scanner(o);
 }
 
@@ -18558,15 +18649,15 @@
   p->_ranges = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_2pe_11_cy_machine_CharacterClass(PyObject *o) {
   struct __pyx_obj_2pe_11_cy_machine_CharacterClass *p = (struct __pyx_obj_2pe_11_cy_machine_CharacterClass *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->_chars);
   Py_CLEAR(p->_ranges);
   __pyx_tp_dealloc_2pe_11_cy_machine_Scanner(o);
 }
@@ -18693,15 +18784,15 @@
   p->_regex = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_2pe_11_cy_machine_Regex(PyObject *o) {
   struct __pyx_obj_2pe_11_cy_machine_Regex *p = (struct __pyx_obj_2pe_11_cy_machine_Regex *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_regex);
   if (PyType_IS_GC(__pyx_ptype_2pe_11_cy_machine_Scanner)) PyObject_GC_Track(o);
   __pyx_tp_dealloc_2pe_11_cy_machine_Scanner(o);
@@ -19210,15 +19301,17 @@
   {&__pyx_n_s_Bind, __pyx_k_Bind, sizeof(__pyx_k_Bind), 0, 0, 1, 1},
   {&__pyx_n_s_Binding, __pyx_k_Binding, sizeof(__pyx_k_Binding), 0, 0, 1, 1},
   {&__pyx_n_s_CAP, __pyx_k_CAP, sizeof(__pyx_k_CAP), 0, 0, 1, 1},
   {&__pyx_n_s_CHC, __pyx_k_CHC, sizeof(__pyx_k_CHC), 0, 0, 1, 1},
   {&__pyx_n_s_CLS, __pyx_k_CLS, sizeof(__pyx_k_CLS), 0, 0, 1, 1},
   {&__pyx_n_s_COMMON, __pyx_k_COMMON, sizeof(__pyx_k_COMMON), 0, 0, 1, 1},
   {&__pyx_n_s_CharacterClass, __pyx_k_CharacterClass, sizeof(__pyx_k_CharacterClass), 0, 0, 1, 1},
+  {&__pyx_n_s_DEFAULT_IGNORE, __pyx_k_DEFAULT_IGNORE, sizeof(__pyx_k_DEFAULT_IGNORE), 0, 0, 1, 1},
   {&__pyx_n_s_DOT, __pyx_k_DOT, sizeof(__pyx_k_DOT), 0, 0, 1, 1},
+  {&__pyx_n_s_Definition, __pyx_k_Definition, sizeof(__pyx_k_Definition), 0, 0, 1, 1},
   {&__pyx_n_s_Dict, __pyx_k_Dict, sizeof(__pyx_k_Dict), 0, 0, 1, 1},
   {&__pyx_n_s_Dot, __pyx_k_Dot, sizeof(__pyx_k_Dot), 0, 0, 1, 1},
   {&__pyx_n_s_Error, __pyx_k_Error, sizeof(__pyx_k_Error), 0, 0, 1, 1},
   {&__pyx_n_s_Flag, __pyx_k_Flag, sizeof(__pyx_k_Flag), 0, 0, 1, 1},
   {&__pyx_n_s_Grammar, __pyx_k_Grammar, sizeof(__pyx_k_Grammar), 0, 0, 1, 1},
   {&__pyx_n_s_INLINE, __pyx_k_INLINE, sizeof(__pyx_k_INLINE), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
@@ -19267,14 +19360,15 @@
   {&__pyx_n_s_Union, __pyx_k_Union, sizeof(__pyx_k_Union), 0, 0, 1, 1},
   {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {&__pyx_n_s__49, __pyx_k__49, sizeof(__pyx_k__49), 0, 0, 1, 1},
   {&__pyx_n_s_action, __pyx_k_action, sizeof(__pyx_k_action), 0, 0, 1, 1},
   {&__pyx_n_s_and, __pyx_k_and, sizeof(__pyx_k_and), 0, 0, 1, 1},
   {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
+  {&__pyx_n_s_autoignore, __pyx_k_autoignore, sizeof(__pyx_k_autoignore), 0, 0, 1, 1},
   {&__pyx_n_s_bnd, __pyx_k_bnd, sizeof(__pyx_k_bnd), 0, 0, 1, 1},
   {&__pyx_n_s_cap, __pyx_k_cap, sizeof(__pyx_k_cap), 0, 0, 1, 1},
   {&__pyx_n_s_captured_choice, __pyx_k_captured_choice, sizeof(__pyx_k_captured_choice), 0, 0, 1, 1},
   {&__pyx_n_s_capturing, __pyx_k_capturing, sizeof(__pyx_k_capturing), 0, 0, 1, 1},
   {&__pyx_n_s_cclass, __pyx_k_cclass, sizeof(__pyx_k_cclass), 0, 0, 1, 1},
   {&__pyx_n_s_chc, __pyx_k_chc, sizeof(__pyx_k_chc), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
@@ -19293,14 +19387,15 @@
   {&__pyx_n_s_enum, __pyx_k_enum, sizeof(__pyx_k_enum), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
   {&__pyx_n_s_genexpr, __pyx_k_genexpr, sizeof(__pyx_k_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_grammar, __pyx_k_grammar, sizeof(__pyx_k_grammar), 0, 0, 1, 1},
   {&__pyx_n_s_head, __pyx_k_head, sizeof(__pyx_k_head), 0, 0, 1, 1},
   {&__pyx_n_s_idx, __pyx_k_idx, sizeof(__pyx_k_idx), 0, 0, 1, 1},
+  {&__pyx_n_s_ignore, __pyx_k_ignore, sizeof(__pyx_k_ignore), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
   {&__pyx_n_s_index_2, __pyx_k_index_2, sizeof(__pyx_k_index_2), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_init___locals_genexpr, __pyx_k_init___locals_genexpr, sizeof(__pyx_k_init___locals_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_inline, __pyx_k_inline, sizeof(__pyx_k_inline), 0, 0, 1, 1},
   {&__pyx_n_s_insert, __pyx_k_insert, sizeof(__pyx_k_insert), 0, 0, 1, 1},
@@ -19330,25 +19425,28 @@
   {&__pyx_n_s_oploc, __pyx_k_oploc, sizeof(__pyx_k_oploc), 0, 0, 1, 1},
   {&__pyx_n_s_opt, __pyx_k_opt, sizeof(__pyx_k_opt), 0, 0, 1, 1},
   {&__pyx_n_s_optimize, __pyx_k_optimize, sizeof(__pyx_k_optimize), 0, 0, 1, 1},
   {&__pyx_n_s_parser, __pyx_k_parser, sizeof(__pyx_k_parser), 0, 0, 1, 1},
   {&__pyx_n_s_parsing_instructions, __pyx_k_parsing_instructions, sizeof(__pyx_k_parsing_instructions), 0, 0, 1, 1},
   {&__pyx_n_s_pat, __pyx_k_pat, sizeof(__pyx_k_pat), 0, 0, 1, 1},
   {&__pyx_n_s_pattern, __pyx_k_pattern, sizeof(__pyx_k_pattern), 0, 0, 1, 1},
+  {&__pyx_n_s_pe__autoignore, __pyx_k_pe__autoignore, sizeof(__pyx_k_pe__autoignore), 0, 0, 1, 1},
   {&__pyx_n_s_pe__constants, __pyx_k_pe__constants, sizeof(__pyx_k_pe__constants), 0, 0, 1, 1},
   {&__pyx_n_s_pe__cy_machine, __pyx_k_pe__cy_machine, sizeof(__pyx_k_pe__cy_machine), 0, 0, 1, 1},
   {&__pyx_kp_s_pe__cy_machine_pyx, __pyx_k_pe__cy_machine_pyx, sizeof(__pyx_k_pe__cy_machine_pyx), 0, 0, 1, 0},
+  {&__pyx_n_s_pe__definition, __pyx_k_pe__definition, sizeof(__pyx_k_pe__definition), 0, 0, 1, 1},
   {&__pyx_n_s_pe__errors, __pyx_k_pe__errors, sizeof(__pyx_k_pe__errors), 0, 0, 1, 1},
   {&__pyx_n_s_pe__grammar, __pyx_k_pe__grammar, sizeof(__pyx_k_pe__grammar), 0, 0, 1, 1},
   {&__pyx_n_s_pe__match, __pyx_k_pe__match, sizeof(__pyx_k_pe__match), 0, 0, 1, 1},
   {&__pyx_n_s_pe__optimize, __pyx_k_pe__optimize, sizeof(__pyx_k_pe__optimize), 0, 0, 1, 1},
   {&__pyx_n_s_pe__parser, __pyx_k_pe__parser, sizeof(__pyx_k_pe__parser), 0, 0, 1, 1},
   {&__pyx_n_s_pe__types, __pyx_k_pe__types, sizeof(__pyx_k_pe__types), 0, 0, 1, 1},
   {&__pyx_n_s_pe_actions, __pyx_k_pe_actions, sizeof(__pyx_k_pe_actions), 0, 0, 1, 1},
   {&__pyx_n_s_pe_operators, __pyx_k_pe_operators, sizeof(__pyx_k_pe_operators), 0, 0, 1, 1},
+  {&__pyx_n_s_pe_patterns, __pyx_k_pe_patterns, sizeof(__pyx_k_pe_patterns), 0, 0, 1, 1},
   {&__pyx_n_s_pi, __pyx_k_pi, sizeof(__pyx_k_pi), 0, 0, 1, 1},
   {&__pyx_n_s_pi_2, __pyx_k_pi_2, sizeof(__pyx_k_pi_2), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pis, __pyx_k_pis, sizeof(__pyx_k_pis), 0, 0, 1, 1},
   {&__pyx_n_s_pis_2, __pyx_k_pis_2, sizeof(__pyx_k_pis_2), 0, 0, 1, 1},
   {&__pyx_n_s_pls, __pyx_k_pls, sizeof(__pyx_k_pls), 0, 0, 1, 1},
   {&__pyx_kp_u_pop_from_empty_stack, __pyx_k_pop_from_empty_stack, sizeof(__pyx_k_pop_from_empty_stack), 0, 1, 0, 0},
@@ -19400,38 +19498,38 @@
   {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
   {&__pyx_n_u_unicode, __pyx_k_unicode, sizeof(__pyx_k_unicode), 0, 1, 0, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 148, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 65, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 91, __pyx_L1_error)
-  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 134, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 215, __pyx_L1_error)
-  __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 461, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 138, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 221, __pyx_L1_error)
+  __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 467, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 515, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "pe/_cy_machine.pyx":452
+  /* "pe/_cy_machine.pyx":458
  * def _seq(defn):
  *     head = [pi
  *             for d in defn.args[0][:-1]             # <<<<<<<<<<<<<<
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])
  */
-  __pyx_slice_ = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 452, __pyx_L1_error)
+  __pyx_slice_ = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice_);
   __Pyx_GIVEREF(__pyx_slice_);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
@@ -19453,277 +19551,277 @@
   __pyx_tuple__7 = PyTuple_Pack(3, __pyx_int_29182842, __pyx_int_186251340, __pyx_int_93565377); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_111070186, __pyx_int_235489902, __pyx_int_20010746); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "pe/_cy_machine.pyx":132
+  /* "pe/_cy_machine.pyx":135
  * class MachineParser(Parser):
  * 
  *     def __init__(self, grammar: Grammar,             # <<<<<<<<<<<<<<
+ *                  ignore: Optional[Definition] = DEFAULT_IGNORE,
  *                  flags: Flag = Flag.NONE):
- *         super().__init__(grammar, flags=flags)
  */
-  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_grammar, __pyx_n_s_flags, __pyx_n_s_pi, __pyx_n_s_index_2); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_grammar, __pyx_n_s_ignore, __pyx_n_s_flags, __pyx_n_s_pi, __pyx_n_s_index_2); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_init, 132, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(4, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_init, 135, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 135, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":149
+  /* "pe/_cy_machine.pyx":155
  * 
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         return self.grammar.start
  * 
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_start, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_start, 155, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 155, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":152
+  /* "pe/_cy_machine.pyx":158
  *         return self.grammar.start
  * 
  *     def __contains__(self, name: str) -> bool:             # <<<<<<<<<<<<<<
  *         return name in self._index
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_name); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_name); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_contains, 152, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_contains, 158, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 158, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":155
+  /* "pe/_cy_machine.pyx":161
  *         return name in self._index
  * 
  *     def match(self,             # <<<<<<<<<<<<<<
  *               str s,
  *               int pos = 0,
  */
-  __pyx_tuple__15 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_s, __pyx_n_s_pos, __pyx_n_s_flags, __pyx_n_s_memo, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_idx, __pyx_n_s_end); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_s, __pyx_n_s_pos, __pyx_n_s_flags, __pyx_n_s_memo, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_idx, __pyx_n_s_end); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(4, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_match, 155, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(4, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_match, 161, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 161, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":330
+  /* "pe/_cy_machine.pyx":336
  * 
  * 
  * def _make_program(grammar) -> Tuple[_Program, _Index]:             # <<<<<<<<<<<<<<
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  */
-  __pyx_tuple__17 = PyTuple_Pack(6, __pyx_n_s_grammar, __pyx_n_s_index_2, __pyx_n_s_pis, __pyx_n_s_name, __pyx_n_s_pis_2, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(6, __pyx_n_s_grammar, __pyx_n_s_index_2, __pyx_n_s_pis, __pyx_n_s_name, __pyx_n_s_pis_2, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_make_program, 330, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_make_program, 336, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 336, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":352
+  /* "pe/_cy_machine.pyx":358
  * 
  * 
  * def _dot(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Dot())]
  * 
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_dot, 352, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_dot, 358, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 358, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":356
+  /* "pe/_cy_machine.pyx":362
  * 
  * 
  * def _lit(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]
  * 
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_lit, 356, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_lit, 362, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 362, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":360
+  /* "pe/_cy_machine.pyx":366
  * 
  * 
  * def _cls(defn, mincount=1, maxcount=1):             # <<<<<<<<<<<<<<
  *     cclass = CharacterClass(
  *         defn.args[0],
  */
-  __pyx_tuple__23 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_maxcount, __pyx_n_s_cclass); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_maxcount, __pyx_n_s_cclass); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cls, 360, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cls, 366, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 366, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":370
+  /* "pe/_cy_machine.pyx":376
  * 
  * 
  * def _rgx(defn):             # <<<<<<<<<<<<<<
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  */
-  __pyx_tuple__25 = PyTuple_Pack(3, __pyx_n_s_defn, __pyx_n_s_pat, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(3, __pyx_n_s_defn, __pyx_n_s_pat, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rgx, 370, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rgx, 376, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 376, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":375
+  /* "pe/_cy_machine.pyx":381
  * 
  * 
  * def _opt(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_tuple__27 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 381, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_opt, 375, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_opt, 381, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 381, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":382
+  /* "pe/_cy_machine.pyx":388
  * 
  * 
  * def _str(defn): return _rpt(defn, 0)             # <<<<<<<<<<<<<<
  * def _pls(defn): return _rpt(defn, 1)
  * 
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_str, 382, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_str, 388, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 388, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":383
+  /* "pe/_cy_machine.pyx":389
  * 
  * def _str(defn): return _rpt(defn, 0)
  * def _pls(defn): return _rpt(defn, 1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_pls, 383, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_pls, 389, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 389, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":386
+  /* "pe/_cy_machine.pyx":392
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
-  __pyx_tuple__33 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rpt, 386, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rpt, 392, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 392, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":408
+  /* "pe/_cy_machine.pyx":414
  * 
  * 
  * def _sym(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(CALL, name=defn.args[0])]
  * 
  */
-  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_sym, 408, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_sym, 414, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 414, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":412
+  /* "pe/_cy_machine.pyx":418
  * 
  * 
  * def _and(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_tuple__37 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_and, 412, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_and, 418, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 418, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":420
+  /* "pe/_cy_machine.pyx":426
  * 
  * 
  * def _not(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_tuple__39 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_not, 420, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_not, 426, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 426, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":427
+  /* "pe/_cy_machine.pyx":433
  * 
  * 
  * def _cap(defn):             # <<<<<<<<<<<<<<
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  */
-  __pyx_tuple__41 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_captured_choice, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_captured_choice, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cap, 427, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cap, 433, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 433, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":446
+  /* "pe/_cy_machine.pyx":452
  * 
  * 
  * def _bnd(defn):             # <<<<<<<<<<<<<<
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))
  * 
  */
-  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_bnd, 446, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_bnd, 452, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 452, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":450
+  /* "pe/_cy_machine.pyx":456
  * 
  * 
  * def _seq(defn):             # <<<<<<<<<<<<<<
  *     head = [pi
  *             for d in defn.args[0][:-1]
  */
-  __pyx_tuple__45 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_head, __pyx_n_s_tail, __pyx_n_s_d, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_tuple__45 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_head, __pyx_n_s_tail, __pyx_n_s_d, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_seq, 450, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_seq, 456, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 456, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":458
+  /* "pe/_cy_machine.pyx":464
  * 
  * 
  * def _chc(defn):             # <<<<<<<<<<<<<<
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  */
-  __pyx_tuple__47 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_pis, __pyx_n_s_pi, __pyx_n_s_pi_2, __pyx_n_s_d); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_pis, __pyx_n_s_pi, __pyx_n_s_pi_2, __pyx_n_s_d); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__47);
   __Pyx_GIVEREF(__pyx_tuple__47);
-  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_chc, 458, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(1, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_chc, 464, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 464, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":469
+  /* "pe/_cy_machine.pyx":475
  * 
  * 
  * def _rul(defn):             # <<<<<<<<<<<<<<
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  */
-  __pyx_tuple__50 = PyTuple_Pack(6, __pyx_n_s_defn, __pyx_n_s_subdefn, __pyx_n_s_action, __pyx_n_s__49, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_tuple__50 = PyTuple_Pack(6, __pyx_n_s_defn, __pyx_n_s_subdefn, __pyx_n_s_action, __pyx_n_s__49, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 475, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__50);
   __Pyx_GIVEREF(__pyx_tuple__50);
-  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rul, 469, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rul, 475, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 475, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":506
+  /* "pe/_cy_machine.pyx":512
  * 
  * 
  * def _parsing_instructions(defn):  # noqa: C901             # <<<<<<<<<<<<<<
  *     try:
  *         return _op_map[defn.op](defn)
  */
-  __pyx_tuple__52 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__52);
   __Pyx_GIVEREF(__pyx_tuple__52);
-  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_parsing_instructions, 506, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_parsing_instructions, 512, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 512, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Scanner(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
   __pyx_tuple__54 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -19828,126 +19926,126 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_2pe_11_cy_machine_Scanner = &__pyx_vtable_2pe_11_cy_machine_Scanner;
   __pyx_vtable_2pe_11_cy_machine_Scanner.scan = (int (*)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_2pe_11_cy_machine_7Scanner_scan *__pyx_optional_args))__pyx_f_2pe_11_cy_machine_7Scanner_scan;
   __pyx_vtable_2pe_11_cy_machine_Scanner._scan = (int (*)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int))__pyx_f_2pe_11_cy_machine_7Scanner__scan;
-  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_Scanner) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_Scanner) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2pe_11_cy_machine_Scanner.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2pe_11_cy_machine_Scanner.tp_dictoffset && __pyx_type_2pe_11_cy_machine_Scanner.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2pe_11_cy_machine_Scanner.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine_Scanner.tp_dict, __pyx_vtabptr_2pe_11_cy_machine_Scanner) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Scanner, (PyObject *)&__pyx_type_2pe_11_cy_machine_Scanner) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_Scanner) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine_Scanner.tp_dict, __pyx_vtabptr_2pe_11_cy_machine_Scanner) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Scanner, (PyObject *)&__pyx_type_2pe_11_cy_machine_Scanner) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_Scanner) < 0) __PYX_ERR(0, 90, __pyx_L1_error)
   __pyx_ptype_2pe_11_cy_machine_Scanner = &__pyx_type_2pe_11_cy_machine_Scanner;
-  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_Instruction) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_Instruction) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2pe_11_cy_machine_Instruction.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2pe_11_cy_machine_Instruction.tp_dictoffset && __pyx_type_2pe_11_cy_machine_Instruction.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2pe_11_cy_machine_Instruction.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Instruction, (PyObject *)&__pyx_type_2pe_11_cy_machine_Instruction) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_Instruction) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Instruction, (PyObject *)&__pyx_type_2pe_11_cy_machine_Instruction) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_Instruction) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __pyx_ptype_2pe_11_cy_machine_Instruction = &__pyx_type_2pe_11_cy_machine_Instruction;
   __pyx_vtabptr_2pe_11_cy_machine__Parser = &__pyx_vtable_2pe_11_cy_machine__Parser;
   __pyx_vtable_2pe_11_cy_machine__Parser.match = (int (*)(struct __pyx_obj_2pe_11_cy_machine__Parser *, int, PyObject *, int, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch))__pyx_f_2pe_11_cy_machine_7_Parser_match;
   __pyx_vtable_2pe_11_cy_machine__Parser._match = (struct __pyx_t_2pe_11_cy_machine_State *(*)(struct __pyx_obj_2pe_11_cy_machine__Parser *, int, PyObject *, int, PyObject *, PyObject *, PyObject *, struct __pyx_t_2pe_11_cy_machine_State *))__pyx_f_2pe_11_cy_machine_7_Parser__match;
-  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2pe_11_cy_machine__Parser.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2pe_11_cy_machine__Parser.tp_dictoffset && __pyx_type_2pe_11_cy_machine__Parser.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2pe_11_cy_machine__Parser.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine__Parser.tp_dict, __pyx_vtabptr_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Parser, (PyObject *)&__pyx_type_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 177, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine__Parser.tp_dict, __pyx_vtabptr_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Parser, (PyObject *)&__pyx_type_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
   __pyx_ptype_2pe_11_cy_machine__Parser = &__pyx_type_2pe_11_cy_machine__Parser;
   __pyx_vtabptr_2pe_11_cy_machine_Dot = &__pyx_vtable_2pe_11_cy_machine_Dot;
   __pyx_vtable_2pe_11_cy_machine_Dot.__pyx_base = *__pyx_vtabptr_2pe_11_cy_machine_Scanner;
   __pyx_vtable_2pe_11_cy_machine_Dot.__pyx_base._scan = (int (*)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int))__pyx_f_2pe_11_cy_machine_3Dot__scan;
   __pyx_type_2pe_11_cy_machine_Dot.tp_base = __pyx_ptype_2pe_11_cy_machine_Scanner;
-  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 521, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2pe_11_cy_machine_Dot.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2pe_11_cy_machine_Dot.tp_dictoffset && __pyx_type_2pe_11_cy_machine_Dot.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2pe_11_cy_machine_Dot.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine_Dot.tp_dict, __pyx_vtabptr_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Dot, (PyObject *)&__pyx_type_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 515, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine_Dot.tp_dict, __pyx_vtabptr_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 521, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Dot, (PyObject *)&__pyx_type_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 521, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 521, __pyx_L1_error)
   __pyx_ptype_2pe_11_cy_machine_Dot = &__pyx_type_2pe_11_cy_machine_Dot;
   __pyx_vtabptr_2pe_11_cy_machine_Literal = &__pyx_vtable_2pe_11_cy_machine_Literal;
   __pyx_vtable_2pe_11_cy_machine_Literal.__pyx_base = *__pyx_vtabptr_2pe_11_cy_machine_Scanner;
   __pyx_vtable_2pe_11_cy_machine_Literal.__pyx_base._scan = (int (*)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int))__pyx_f_2pe_11_cy_machine_7Literal__scan;
   __pyx_type_2pe_11_cy_machine_Literal.tp_base = __pyx_ptype_2pe_11_cy_machine_Scanner;
-  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 522, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2pe_11_cy_machine_Literal.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2pe_11_cy_machine_Literal.tp_dictoffset && __pyx_type_2pe_11_cy_machine_Literal.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2pe_11_cy_machine_Literal.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine_Literal.tp_dict, __pyx_vtabptr_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 522, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Literal, (PyObject *)&__pyx_type_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 522, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 522, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine_Literal.tp_dict, __pyx_vtabptr_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Literal, (PyObject *)&__pyx_type_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
   __pyx_ptype_2pe_11_cy_machine_Literal = &__pyx_type_2pe_11_cy_machine_Literal;
   __pyx_vtabptr_2pe_11_cy_machine_CharacterClass = &__pyx_vtable_2pe_11_cy_machine_CharacterClass;
   __pyx_vtable_2pe_11_cy_machine_CharacterClass.__pyx_base = *__pyx_vtabptr_2pe_11_cy_machine_Scanner;
   __pyx_vtable_2pe_11_cy_machine_CharacterClass.__pyx_base._scan = (int (*)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int))__pyx_f_2pe_11_cy_machine_14CharacterClass__scan;
   __pyx_type_2pe_11_cy_machine_CharacterClass.tp_base = __pyx_ptype_2pe_11_cy_machine_Scanner;
-  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 537, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2pe_11_cy_machine_CharacterClass.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2pe_11_cy_machine_CharacterClass.tp_dictoffset && __pyx_type_2pe_11_cy_machine_CharacterClass.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2pe_11_cy_machine_CharacterClass.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine_CharacterClass.tp_dict, __pyx_vtabptr_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 537, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CharacterClass, (PyObject *)&__pyx_type_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 537, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 537, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine_CharacterClass.tp_dict, __pyx_vtabptr_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CharacterClass, (PyObject *)&__pyx_type_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
   __pyx_ptype_2pe_11_cy_machine_CharacterClass = &__pyx_type_2pe_11_cy_machine_CharacterClass;
   __pyx_vtabptr_2pe_11_cy_machine_Regex = &__pyx_vtable_2pe_11_cy_machine_Regex;
   __pyx_vtable_2pe_11_cy_machine_Regex.__pyx_base = *__pyx_vtabptr_2pe_11_cy_machine_Scanner;
   __pyx_vtable_2pe_11_cy_machine_Regex.__pyx_base._scan = (int (*)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int))__pyx_f_2pe_11_cy_machine_5Regex__scan;
   __pyx_type_2pe_11_cy_machine_Regex.tp_base = __pyx_ptype_2pe_11_cy_machine_Scanner;
-  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 589, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 595, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2pe_11_cy_machine_Regex.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2pe_11_cy_machine_Regex.tp_dictoffset && __pyx_type_2pe_11_cy_machine_Regex.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2pe_11_cy_machine_Regex.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine_Regex.tp_dict, __pyx_vtabptr_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 589, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Regex, (PyObject *)&__pyx_type_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 589, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 589, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2pe_11_cy_machine_Regex.tp_dict, __pyx_vtabptr_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 595, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Regex, (PyObject *)&__pyx_type_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 595, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 595, __pyx_L1_error)
   __pyx_ptype_2pe_11_cy_machine_Regex = &__pyx_type_2pe_11_cy_machine_Regex;
-  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct____init__) < 0) __PYX_ERR(0, 545, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct____init__) < 0) __PYX_ERR(0, 551, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2pe_11_cy_machine___pyx_scope_struct____init__.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2pe_11_cy_machine___pyx_scope_struct____init__.tp_dictoffset && __pyx_type_2pe_11_cy_machine___pyx_scope_struct____init__.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2pe_11_cy_machine___pyx_scope_struct____init__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct____init__ = &__pyx_type_2pe_11_cy_machine___pyx_scope_struct____init__;
-  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 552, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 558, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr = &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr;
-  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 559, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr.tp_dictoffset && __pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr = &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr;
@@ -20328,15 +20426,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pe/_cy_machine.pyx":17
  * from pe._constants import Operator, Flag
  * from pe._errors import Error
  * from pe._match import Match             # <<<<<<<<<<<<<<
  * from pe._types import Memo
- * from pe._grammar import Grammar
+ * from pe._definition import Definition
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_Match);
   __Pyx_GIVEREF(__pyx_n_s_Match);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Match);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_pe__match, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
@@ -20348,16 +20446,16 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pe/_cy_machine.pyx":18
  * from pe._errors import Error
  * from pe._match import Match
  * from pe._types import Memo             # <<<<<<<<<<<<<<
+ * from pe._definition import Definition
  * from pe._grammar import Grammar
- * from pe._parser import Parser
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Memo);
   __Pyx_GIVEREF(__pyx_n_s_Memo);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Memo);
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_pe__types, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
@@ -20368,924 +20466,1018 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Memo, __pyx_t_2) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pe/_cy_machine.pyx":19
  * from pe._match import Match
  * from pe._types import Memo
- * from pe._grammar import Grammar             # <<<<<<<<<<<<<<
+ * from pe._definition import Definition             # <<<<<<<<<<<<<<
+ * from pe._grammar import Grammar
  * from pe._parser import Parser
- * from pe._optimize import optimize
  */
   __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_INCREF(__pyx_n_s_Grammar);
-  __Pyx_GIVEREF(__pyx_n_s_Grammar);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Grammar);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_pe__grammar, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_Definition);
+  __Pyx_GIVEREF(__pyx_n_s_Definition);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Definition);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_pe__definition, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Grammar); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Definition); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Grammar, __pyx_t_1) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Definition, __pyx_t_1) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pe/_cy_machine.pyx":20
  * from pe._types import Memo
- * from pe._grammar import Grammar
- * from pe._parser import Parser             # <<<<<<<<<<<<<<
+ * from pe._definition import Definition
+ * from pe._grammar import Grammar             # <<<<<<<<<<<<<<
+ * from pe._parser import Parser
  * from pe._optimize import optimize
- * from pe.actions import Action, Bind
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s_Parser_2);
-  __Pyx_GIVEREF(__pyx_n_s_Parser_2);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Parser_2);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pe__parser, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_Grammar);
+  __Pyx_GIVEREF(__pyx_n_s_Grammar);
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Grammar);
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pe__grammar, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Parser_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Grammar); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Parser_2, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Grammar, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "pe/_cy_machine.pyx":21
+ * from pe._definition import Definition
+ * from pe._grammar import Grammar
+ * from pe._parser import Parser             # <<<<<<<<<<<<<<
+ * from pe._optimize import optimize
+ * from pe._autoignore import autoignore
+ */
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_n_s_Parser_2);
+  __Pyx_GIVEREF(__pyx_n_s_Parser_2);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Parser_2);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_pe__parser, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Parser_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Parser_2, __pyx_t_1) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "pe/_cy_machine.pyx":22
  * from pe._grammar import Grammar
  * from pe._parser import Parser
  * from pe._optimize import optimize             # <<<<<<<<<<<<<<
+ * from pe._autoignore import autoignore
  * from pe.actions import Action, Bind
- * from pe.operators import Rule
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_optimize);
   __Pyx_GIVEREF(__pyx_n_s_optimize);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_optimize);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_pe__optimize, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_optimize);
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pe__optimize, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_optimize); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_optimize, __pyx_t_2) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "pe/_cy_machine.pyx":23
+ * from pe._parser import Parser
+ * from pe._optimize import optimize
+ * from pe._autoignore import autoignore             # <<<<<<<<<<<<<<
+ * from pe.actions import Action, Bind
+ * from pe.operators import Rule
+ */
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_n_s_autoignore);
+  __Pyx_GIVEREF(__pyx_n_s_autoignore);
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_autoignore);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_pe__autoignore, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_optimize); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_autoignore); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_optimize, __pyx_t_1) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_autoignore, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":22
- * from pe._parser import Parser
+  /* "pe/_cy_machine.pyx":24
  * from pe._optimize import optimize
+ * from pe._autoignore import autoignore
  * from pe.actions import Action, Bind             # <<<<<<<<<<<<<<
  * from pe.operators import Rule
- * 
+ * from pe.patterns import DEFAULT_IGNORE
  */
-  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Action);
   __Pyx_GIVEREF(__pyx_n_s_Action);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Action);
   __Pyx_INCREF(__pyx_n_s_Bind);
   __Pyx_GIVEREF(__pyx_n_s_Bind);
   PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_Bind);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pe_actions, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pe_actions, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Action); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Action); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Action, __pyx_t_2) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Action, __pyx_t_2) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Bind); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Bind); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Bind, __pyx_t_2) < 0) __PYX_ERR(0, 22, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Bind, __pyx_t_2) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":23
- * from pe._optimize import optimize
+  /* "pe/_cy_machine.pyx":25
+ * from pe._autoignore import autoignore
  * from pe.actions import Action, Bind
  * from pe.operators import Rule             # <<<<<<<<<<<<<<
- * 
+ * from pe.patterns import DEFAULT_IGNORE
  * 
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_Rule);
   __Pyx_GIVEREF(__pyx_n_s_Rule);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Rule);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_pe_operators, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_pe_operators, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Rule); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Rule); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Rule, __pyx_t_1) < 0) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Rule, __pyx_t_1) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":83
+  /* "pe/_cy_machine.pyx":26
+ * from pe.actions import Action, Bind
+ * from pe.operators import Rule
+ * from pe.patterns import DEFAULT_IGNORE             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_n_s_DEFAULT_IGNORE);
+  __Pyx_GIVEREF(__pyx_n_s_DEFAULT_IGNORE);
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_DEFAULT_IGNORE);
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pe_patterns, __pyx_t_2, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_DEFAULT_IGNORE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DEFAULT_IGNORE, __pyx_t_2) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "pe/_cy_machine.pyx":86
  * 
  * 
  * _Binding = Tuple[str, Any]             # <<<<<<<<<<<<<<
  * _Index = Dict[str, int]
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Tuple); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Any); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Tuple); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&PyUnicode_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyUnicode_Type)));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&PyUnicode_Type)));
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Binding, __pyx_t_1) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Binding, __pyx_t_2) < 0) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":84
+  /* "pe/_cy_machine.pyx":87
  * 
  * _Binding = Tuple[str, Any]
  * _Index = Dict[str, int]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Dict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)(&PyUnicode_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyUnicode_Type)));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&PyUnicode_Type)));
   __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
   __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
   PyTuple_SET_ITEM(__pyx_t_3, 1, ((PyObject *)(&PyInt_Type)));
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Index, __pyx_t_2) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Index, __pyx_t_1) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":127
+  /* "pe/_cy_machine.pyx":130
  * 
  * 
  * _Program = List[Instruction]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_List); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_2, ((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_List); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_1, ((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Program, __pyx_t_3) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Program, __pyx_t_3) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":130
+  /* "pe/_cy_machine.pyx":133
  * 
  * 
  * class MachineParser(Parser):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, grammar: Grammar,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Parser_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Parser_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_3, __pyx_t_2, __pyx_n_s_MachineParser, __pyx_n_s_MachineParser, (PyObject *) NULL, __pyx_n_s_pe__cy_machine, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_3, __pyx_t_1, __pyx_n_s_MachineParser, __pyx_n_s_MachineParser, (PyObject *) NULL, __pyx_n_s_pe__cy_machine, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
-  /* "pe/_cy_machine.pyx":132
+  /* "pe/_cy_machine.pyx":135
  * class MachineParser(Parser):
  * 
  *     def __init__(self, grammar: Grammar,             # <<<<<<<<<<<<<<
+ *                  ignore: Optional[Definition] = DEFAULT_IGNORE,
  *                  flags: Flag = Flag.NONE):
- *         super().__init__(grammar, flags=flags)
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Grammar); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Grammar); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_grammar, __pyx_t_6) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_grammar, __pyx_t_6) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "pe/_cy_machine.pyx":133
+  /* "pe/_cy_machine.pyx":136
  * 
  *     def __init__(self, grammar: Grammar,
- *                  flags: Flag = Flag.NONE):             # <<<<<<<<<<<<<<
+ *                  ignore: Optional[Definition] = DEFAULT_IGNORE,             # <<<<<<<<<<<<<<
+ *                  flags: Flag = Flag.NONE):
  *         super().__init__(grammar, flags=flags)
- * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Flag); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Optional); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_flags, __pyx_t_6) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Definition); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_ignore, __pyx_t_8) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+
+  /* "pe/_cy_machine.pyx":137
+ *     def __init__(self, grammar: Grammar,
+ *                  ignore: Optional[Definition] = DEFAULT_IGNORE,
+ *                  flags: Flag = Flag.NONE):             # <<<<<<<<<<<<<<
+ *         super().__init__(grammar, flags=flags)
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Flag); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_flags, __pyx_t_8) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":132
+  /* "pe/_cy_machine.pyx":135
  * class MachineParser(Parser):
  * 
  *     def __init__(self, grammar: Grammar,             # <<<<<<<<<<<<<<
+ *                  ignore: Optional[Definition] = DEFAULT_IGNORE,
  *                  flags: Flag = Flag.NONE):
- *         super().__init__(grammar, flags=flags)
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_1__init__, 0, __pyx_n_s_MachineParser___init, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 132, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_INCREF(__pyx_t_6);
-  PyList_Append(__pyx_t_4, __pyx_t_6);
-  __Pyx_GIVEREF(__pyx_t_6);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_6, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_1__init__, 0, __pyx_n_s_MachineParser___init, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_INCREF(__pyx_t_8);
+  PyList_Append(__pyx_t_4, __pyx_t_8);
+  __Pyx_GIVEREF(__pyx_t_8);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_8, sizeof(__pyx_defaults), 2)) __PYX_ERR(0, 135, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":133
+  /* "pe/_cy_machine.pyx":136
  * 
  *     def __init__(self, grammar: Grammar,
+ *                  ignore: Optional[Definition] = DEFAULT_IGNORE,             # <<<<<<<<<<<<<<
+ *                  flags: Flag = Flag.NONE):
+ *         super().__init__(grammar, flags=flags)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_DEFAULT_IGNORE); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_8)->__pyx_arg_ignore = __pyx_t_7;
+  __Pyx_GIVEREF(__pyx_t_7);
+  __pyx_t_7 = 0;
+
+  /* "pe/_cy_machine.pyx":137
+ *     def __init__(self, grammar: Grammar,
+ *                  ignore: Optional[Definition] = DEFAULT_IGNORE,
  *                  flags: Flag = Flag.NONE):             # <<<<<<<<<<<<<<
  *         super().__init__(grammar, flags=flags)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Flag); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Flag); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_NONE); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 133, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_NONE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_6)->__pyx_arg_flags = __pyx_t_8;
-  __Pyx_GIVEREF(__pyx_t_8);
-  __pyx_t_8 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_6, __pyx_pf_2pe_11_cy_machine_50__defaults__);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_5);
+  __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_8)->__pyx_arg_flags = __pyx_t_6;
+  __Pyx_GIVEREF(__pyx_t_6);
+  __pyx_t_6 = 0;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_8, __pyx_pf_2pe_11_cy_machine_50__defaults__);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_8, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_init, __pyx_t_6) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_8) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":149
+  /* "pe/_cy_machine.pyx":155
  * 
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         return self.grammar.start
  * 
  */
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_3start, 0, __pyx_n_s_MachineParser_start, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_8 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_3start, 0, __pyx_n_s_MachineParser_start, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
 
-  /* "pe/_cy_machine.pyx":148
+  /* "pe/_cy_machine.pyx":154
  *         self._index = index
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def start(self):
  *         return self.grammar.start
  */
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_start, __pyx_t_5) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_start, __pyx_t_5) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":152
+  /* "pe/_cy_machine.pyx":158
  *         return self.grammar.start
  * 
  *     def __contains__(self, name: str) -> bool:             # <<<<<<<<<<<<<<
  *         return name in self._index
  * 
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_name, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_5__contains__, 0, __pyx_n_s_MachineParser___contains, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_name, __pyx_n_u_unicode) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, ((PyObject*)&PyBool_Type)) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_5__contains__, 0, __pyx_n_s_MachineParser___contains, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_8, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_contains, __pyx_t_6) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_contains, __pyx_t_8) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":155
+  /* "pe/_cy_machine.pyx":161
  *         return name in self._index
  * 
  *     def match(self,             # <<<<<<<<<<<<<<
  *               str s,
  *               int pos = 0,
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 155, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
 
-  /* "pe/_cy_machine.pyx":158
+  /* "pe/_cy_machine.pyx":164
  *               str s,
  *               int pos = 0,
  *               flags: Flag = Flag.NONE) -> Union[Match, None]:             # <<<<<<<<<<<<<<
  *         memo: Union[Memo, None] = None
  *         args: List[Any] = []
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Flag); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Flag); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flags, __pyx_t_5) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_flags, __pyx_t_5) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Union); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Union); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Match); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 158, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Match); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_7, 1, Py_None);
-  __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 158, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_t_8) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_return, __pyx_t_6) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "pe/_cy_machine.pyx":155
+  /* "pe/_cy_machine.pyx":161
  *         return name in self._index
  * 
  *     def match(self,             # <<<<<<<<<<<<<<
  *               str s,
  *               int pos = 0,
  */
-  __pyx_t_8 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_7match, 0, __pyx_n_s_MachineParser_match, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 155, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_8, sizeof(__pyx_defaults1), 1)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13MachineParser_7match, 0, __pyx_n_s_MachineParser_match, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_6, sizeof(__pyx_defaults1), 1)) __PYX_ERR(0, 161, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":158
+  /* "pe/_cy_machine.pyx":164
  *               str s,
  *               int pos = 0,
  *               flags: Flag = Flag.NONE) -> Union[Match, None]:             # <<<<<<<<<<<<<<
  *         memo: Union[Memo, None] = None
  *         args: List[Any] = []
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Flag); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Flag); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_NONE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_NONE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_8)->__pyx_arg_flags = __pyx_t_5;
+  __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_6)->__pyx_arg_flags = __pyx_t_5;
   __Pyx_GIVEREF(__pyx_t_5);
   __pyx_t_5 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_8, __pyx_pf_2pe_11_cy_machine_52__defaults__);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_8, __pyx_t_6);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_match, __pyx_t_8) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_6, __pyx_pf_2pe_11_cy_machine_52__defaults__);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_8);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_match, __pyx_t_6) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "pe/_cy_machine.pyx":130
+  /* "pe/_cy_machine.pyx":133
  * 
  * 
  * class MachineParser(Parser):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, grammar: Grammar,
  */
-  __pyx_t_8 = __Pyx_Py3ClassCreate(__pyx_t_3, __pyx_n_s_MachineParser, __pyx_t_2, __pyx_t_1, NULL, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 130, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  if (__Pyx_CyFunction_InitClassCell(__pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_Py3ClassCreate(__pyx_t_3, __pyx_n_s_MachineParser, __pyx_t_1, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (__Pyx_CyFunction_InitClassCell(__pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MachineParser, __pyx_t_8) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MachineParser, __pyx_t_6) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":327
+  /* "pe/_cy_machine.pyx":333
  * # Captures and actions cannot be placed on these operators because of
  * # their effect on the stack
  * NO_CAP_OR_ACT = {CALL, COMMIT, UPDATE, RESTORE, FAILTWICE, RETURN}             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 327, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 327, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_UPDATE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RESTORE); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 327, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAILTWICE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 327, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RETURN); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_UPDATE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_6 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RESTORE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = PySet_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAILTWICE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_8 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RETURN); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_5 = PySet_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PySet_Add(__pyx_t_5, __pyx_t_2) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PySet_Add(__pyx_t_5, __pyx_t_3) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PySet_Add(__pyx_t_5, __pyx_t_1) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_5, __pyx_t_1) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PySet_Add(__pyx_t_5, __pyx_t_8) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PySet_Add(__pyx_t_5, __pyx_t_4) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PySet_Add(__pyx_t_5, __pyx_t_6) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_5, __pyx_t_3) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PySet_Add(__pyx_t_5, __pyx_t_2) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PySet_Add(__pyx_t_5, __pyx_t_6) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NO_CAP_OR_ACT, __pyx_t_5) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_5, __pyx_t_4) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PySet_Add(__pyx_t_5, __pyx_t_8) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NO_CAP_OR_ACT, __pyx_t_5) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":330
+  /* "pe/_cy_machine.pyx":336
  * 
  * 
  * def _make_program(grammar) -> Tuple[_Program, _Index]:             # <<<<<<<<<<<<<<
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_1_make_program, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_1_make_program, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_make_program, __pyx_t_5) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_make_program, __pyx_t_5) < 0) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":352
+  /* "pe/_cy_machine.pyx":358
  * 
  * 
  * def _dot(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Dot())]
  * 
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_3_dot, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_3_dot, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dot, __pyx_t_5) < 0) __PYX_ERR(0, 352, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dot, __pyx_t_5) < 0) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":356
+  /* "pe/_cy_machine.pyx":362
  * 
  * 
  * def _lit(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]
  * 
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_5_lit, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_5_lit, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lit, __pyx_t_5) < 0) __PYX_ERR(0, 356, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lit, __pyx_t_5) < 0) __PYX_ERR(0, 362, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":360
+  /* "pe/_cy_machine.pyx":366
  * 
  * 
  * def _cls(defn, mincount=1, maxcount=1):             # <<<<<<<<<<<<<<
  *     cclass = CharacterClass(
  *         defn.args[0],
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_7_cls, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_7_cls, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cls, __pyx_t_5) < 0) __PYX_ERR(0, 360, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cls, __pyx_t_5) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":370
+  /* "pe/_cy_machine.pyx":376
  * 
  * 
  * def _rgx(defn):             # <<<<<<<<<<<<<<
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_9_rgx, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_9_rgx, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rgx, __pyx_t_5) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rgx, __pyx_t_5) < 0) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":375
+  /* "pe/_cy_machine.pyx":381
  * 
  * 
  * def _opt(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_11_opt, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_11_opt, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 381, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_opt, __pyx_t_5) < 0) __PYX_ERR(0, 375, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_opt, __pyx_t_5) < 0) __PYX_ERR(0, 381, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":382
+  /* "pe/_cy_machine.pyx":388
  * 
  * 
  * def _str(defn): return _rpt(defn, 0)             # <<<<<<<<<<<<<<
  * def _pls(defn): return _rpt(defn, 1)
  * 
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_13_str, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_13_str, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_str, __pyx_t_5) < 0) __PYX_ERR(0, 382, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_str, __pyx_t_5) < 0) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":383
+  /* "pe/_cy_machine.pyx":389
  * 
  * def _str(defn): return _rpt(defn, 0)
  * def _pls(defn): return _rpt(defn, 1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_15_pls, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_15_pls, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pls, __pyx_t_5) < 0) __PYX_ERR(0, 383, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pls, __pyx_t_5) < 0) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":386
+  /* "pe/_cy_machine.pyx":392
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_17_rpt, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_17_rpt, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rpt, __pyx_t_5) < 0) __PYX_ERR(0, 386, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rpt, __pyx_t_5) < 0) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":408
+  /* "pe/_cy_machine.pyx":414
  * 
  * 
  * def _sym(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(CALL, name=defn.args[0])]
  * 
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_19_sym, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_19_sym, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sym, __pyx_t_5) < 0) __PYX_ERR(0, 408, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sym, __pyx_t_5) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":412
+  /* "pe/_cy_machine.pyx":418
  * 
  * 
  * def _and(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_21_and, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_21_and, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_and, __pyx_t_5) < 0) __PYX_ERR(0, 412, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_and, __pyx_t_5) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":420
+  /* "pe/_cy_machine.pyx":426
  * 
  * 
  * def _not(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_23_not, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_23_not, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_not, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_not, __pyx_t_5) < 0) __PYX_ERR(0, 426, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":427
+  /* "pe/_cy_machine.pyx":433
  * 
  * 
  * def _cap(defn):             # <<<<<<<<<<<<<<
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_25_cap, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_25_cap, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cap, __pyx_t_5) < 0) __PYX_ERR(0, 427, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cap, __pyx_t_5) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":446
+  /* "pe/_cy_machine.pyx":452
  * 
  * 
  * def _bnd(defn):             # <<<<<<<<<<<<<<
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))
  * 
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_27_bnd, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_27_bnd, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_bnd, __pyx_t_5) < 0) __PYX_ERR(0, 446, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_bnd, __pyx_t_5) < 0) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":450
+  /* "pe/_cy_machine.pyx":456
  * 
  * 
  * def _seq(defn):             # <<<<<<<<<<<<<<
  *     head = [pi
  *             for d in defn.args[0][:-1]
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_29_seq, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_29_seq, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_seq, __pyx_t_5) < 0) __PYX_ERR(0, 450, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_seq, __pyx_t_5) < 0) __PYX_ERR(0, 456, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":458
+  /* "pe/_cy_machine.pyx":464
  * 
  * 
  * def _chc(defn):             # <<<<<<<<<<<<<<
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_31_chc, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_31_chc, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_chc, __pyx_t_5) < 0) __PYX_ERR(0, 458, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_chc, __pyx_t_5) < 0) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":469
+  /* "pe/_cy_machine.pyx":475
  * 
  * 
  * def _rul(defn):             # <<<<<<<<<<<<<<
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_33_rul, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_33_rul, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 475, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rul, __pyx_t_5) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rul, __pyx_t_5) < 0) __PYX_ERR(0, 475, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":488
+  /* "pe/_cy_machine.pyx":494
  * 
  * _op_map = {
  *     Operator.DOT: _dot,             # <<<<<<<<<<<<<<
  *     Operator.LIT: _lit,
  *     Operator.CLS: _cls,
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(15); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 488, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(15); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 488, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_DOT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_DOT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_dot); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 488, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_dot); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":489
+  /* "pe/_cy_machine.pyx":495
  * _op_map = {
  *     Operator.DOT: _dot,
  *     Operator.LIT: _lit,             # <<<<<<<<<<<<<<
  *     Operator.CLS: _cls,
  *     Operator.RGX: _rgx,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 489, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_LIT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_LIT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 495, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_lit); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 489, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_lit); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":490
+  /* "pe/_cy_machine.pyx":496
  *     Operator.DOT: _dot,
  *     Operator.LIT: _lit,
  *     Operator.CLS: _cls,             # <<<<<<<<<<<<<<
  *     Operator.RGX: _rgx,
  *     Operator.OPT: _opt,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 490, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_CLS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 490, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 496, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_CLS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_cls); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 490, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_cls); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 496, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":491
+  /* "pe/_cy_machine.pyx":497
  *     Operator.LIT: _lit,
  *     Operator.CLS: _cls,
  *     Operator.RGX: _rgx,             # <<<<<<<<<<<<<<
  *     Operator.OPT: _opt,
  *     Operator.STR: _str,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 491, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_RGX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_RGX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_rgx); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 491, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_rgx); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":492
+  /* "pe/_cy_machine.pyx":498
  *     Operator.CLS: _cls,
  *     Operator.RGX: _rgx,
  *     Operator.OPT: _opt,             # <<<<<<<<<<<<<<
  *     Operator.STR: _str,
  *     Operator.PLS: _pls,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 492, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_OPT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 492, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_OPT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_opt); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 492, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_opt); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":493
+  /* "pe/_cy_machine.pyx":499
  *     Operator.RGX: _rgx,
  *     Operator.OPT: _opt,
  *     Operator.STR: _str,             # <<<<<<<<<<<<<<
  *     Operator.PLS: _pls,
  *     Operator.SYM: _sym,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 493, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_STR); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 499, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_STR); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_str); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 493, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_str); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 499, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":494
+  /* "pe/_cy_machine.pyx":500
  *     Operator.OPT: _opt,
  *     Operator.STR: _str,
  *     Operator.PLS: _pls,             # <<<<<<<<<<<<<<
  *     Operator.SYM: _sym,
  *     Operator.AND: _and,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 494, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_PLS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 500, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_PLS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_pls); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 494, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_pls); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 500, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":495
+  /* "pe/_cy_machine.pyx":501
  *     Operator.STR: _str,
  *     Operator.PLS: _pls,
  *     Operator.SYM: _sym,             # <<<<<<<<<<<<<<
  *     Operator.AND: _and,
  *     Operator.NOT: _not,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 495, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_SYM); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 495, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 501, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_SYM); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_sym); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 495, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_sym); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 501, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":496
+  /* "pe/_cy_machine.pyx":502
  *     Operator.PLS: _pls,
  *     Operator.SYM: _sym,
  *     Operator.AND: _and,             # <<<<<<<<<<<<<<
  *     Operator.NOT: _not,
  *     Operator.CAP: _cap,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 496, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_AND); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 496, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_AND); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_and); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 496, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_and); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":497
+  /* "pe/_cy_machine.pyx":503
  *     Operator.SYM: _sym,
  *     Operator.AND: _and,
  *     Operator.NOT: _not,             # <<<<<<<<<<<<<<
  *     Operator.CAP: _cap,
  *     Operator.BND: _bnd,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_NOT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 497, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_NOT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_not); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_not); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":498
+  /* "pe/_cy_machine.pyx":504
  *     Operator.AND: _and,
  *     Operator.NOT: _not,
  *     Operator.CAP: _cap,             # <<<<<<<<<<<<<<
  *     Operator.BND: _bnd,
  *     Operator.SEQ: _seq,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 498, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_CAP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 504, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_CAP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_cap); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 498, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_cap); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 504, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":499
+  /* "pe/_cy_machine.pyx":505
  *     Operator.NOT: _not,
  *     Operator.CAP: _cap,
  *     Operator.BND: _bnd,             # <<<<<<<<<<<<<<
  *     Operator.SEQ: _seq,
  *     Operator.CHC: _chc,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 499, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_BND); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 499, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_BND); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_bnd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 499, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_bnd); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":500
+  /* "pe/_cy_machine.pyx":506
  *     Operator.CAP: _cap,
  *     Operator.BND: _bnd,
  *     Operator.SEQ: _seq,             # <<<<<<<<<<<<<<
  *     Operator.CHC: _chc,
  *     Operator.RUL: _rul,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 500, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_SEQ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 500, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_SEQ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_seq); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 500, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_seq); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":501
+  /* "pe/_cy_machine.pyx":507
  *     Operator.BND: _bnd,
  *     Operator.SEQ: _seq,
  *     Operator.CHC: _chc,             # <<<<<<<<<<<<<<
  *     Operator.RUL: _rul,
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 501, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_CHC); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 501, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_CHC); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_chc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 501, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_chc); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":502
+  /* "pe/_cy_machine.pyx":508
  *     Operator.SEQ: _seq,
  *     Operator.CHC: _chc,
  *     Operator.RUL: _rul,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Operator); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 502, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_RUL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_RUL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_rul); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 502, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_6) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_rul); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_op_map, __pyx_t_5) < 0) __PYX_ERR(0, 487, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_op_map, __pyx_t_5) < 0) __PYX_ERR(0, 493, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pe/_cy_machine.pyx":506
+  /* "pe/_cy_machine.pyx":512
  * 
  * 
  * def _parsing_instructions(defn):  # noqa: C901             # <<<<<<<<<<<<<<
  *     try:
  *         return _op_map[defn.op](defn)
  */
-  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_35_parsing_instructions, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_5 = PyCFunction_NewEx(&__pyx_mdef_2pe_11_cy_machine_35_parsing_instructions, NULL, __pyx_n_s_pe__cy_machine); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parsing_instructions, __pyx_t_5) < 0) __PYX_ERR(0, 506, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parsing_instructions, __pyx_t_5) < 0) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Scanner(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
```

### Comparing `pe-0.4.0/pe/_cy_machine.pyx` & `pe-0.5.0/pe/_cy_machine.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 
 from cpython.mem cimport PyMem_Malloc, PyMem_Free
 
 from pe._constants import Operator, Flag
 from pe._errors import Error
 from pe._match import Match
 from pe._types import Memo
+from pe._definition import Definition
 from pe._grammar import Grammar
 from pe._parser import Parser
 from pe._optimize import optimize
+from pe._autoignore import autoignore
 from pe.actions import Action, Bind
 from pe.operators import Rule
+from pe.patterns import DEFAULT_IGNORE
 
 
 DEF FAILURE = -1
 
 
 # Parser ###############################################################
 
@@ -126,17 +129,20 @@
 
 _Program = List[Instruction]
 
 
 class MachineParser(Parser):
 
     def __init__(self, grammar: Grammar,
+                 ignore: Optional[Definition] = DEFAULT_IGNORE,
                  flags: Flag = Flag.NONE):
         super().__init__(grammar, flags=flags)
 
+        grammar = autoignore(grammar, ignore)
+
         grammar = optimize(grammar,
                            inline=flags & Flag.INLINE,
                            common=flags & Flag.COMMON,
                            regex=False)
         # if flags & Flag.DEBUG:
         #     grammar = debug(grammar)
         self.modified_grammar = grammar
```

### Comparing `pe-0.4.0/pe/_debug.py` & `pe-0.5.0/pe/_debug.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/pe/_definition.py` & `pe-0.5.0/pe/_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 STR = Operator.STR
 PLS = Operator.PLS
 AND = Operator.AND
 NOT = Operator.NOT
 CAP = Operator.CAP
 BND = Operator.BND
 SEQ = Operator.SEQ
+IGN = Operator.IGN
 CHC = Operator.CHC
 RUL = Operator.RUL
 DEF = Operator.DEF
 DBG = Operator.DBG
 
 
 class Definition:
@@ -83,14 +84,15 @@
     STR: ('', '', '*'),
     PLS: ('', '', '+'),
     AND: ('&', '', ''),
     NOT: ('!', '', ''),
     CAP: ('~', '', ''),
     BND: ('{}:', '', ''),
     SEQ: ('', ' ', ''),
+    IGN: ('<', '', ''),
     CHC: ('', ' / ', ''),
     RUL: ('', '', '  -> {}'),
 }
 
 
 def _format_recursive(defn: Definition, prev_op: Operator) -> str:
     op = defn.op
@@ -122,14 +124,15 @@
     STR: _format_recursive,
     PLS: _format_recursive,
     AND: _format_recursive,
     NOT: _format_recursive,
     CAP: _format_recursive,
     BND: _format_recursive,
     SEQ: _format_recursive,
+    IGN: _format_recursive,
     CHC: _format_recursive,
     RUL: _format_recursive,
     DBG: _format_debug,
 }
 
 
 def _format(defn: Definition,
```

### Comparing `pe-0.4.0/pe/_errors.py` & `pe-0.5.0/pe/_errors.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/pe/_escape.py` & `pe-0.5.0/pe/_escape.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/pe/_functions.py` & `pe-0.5.0/pe/_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 
 from typing import Union, Dict, Callable, Optional
 
 from pe.actions import Action
 from pe._constants import Flag
+from pe._definition import Definition
 from pe._errors import Error
 from pe._parser import Parser
 from pe._grammar import Grammar
 from pe._parse import loads
+from pe.patterns import DEFAULT_IGNORE
 
 _FuncMap = Dict[str, Union[Action, Callable]]
 
 
 def compile(source: Union[str, Grammar],
             actions: Optional[_FuncMap] = None,
             parser: str = 'packrat',
+            ignore: Optional[Definition] = DEFAULT_IGNORE,
             flags: Flag = Flag.OPTIMIZE) -> Parser:
     """Compile the parsing expression or grammar in *source*."""
     parsername = parser.lower()
     if parsername == 'packrat':
         from pe.packrat import PackratParser as parser_class
     elif parsername == 'machine':
         from pe.machine import MachineParser as parser_class  # type: ignore
@@ -35,33 +38,35 @@
         start, defmap = loads(source)
         g = Grammar(defmap, actions=actions, start=start)
 
     if flags & Flag.DEBUG:
         print('## Grammar ##')
         print(g)
 
-    p = parser_class(g, flags=flags)
+    p = parser_class(g, ignore=ignore, flags=flags)
 
     if (flags & Flag.DEBUG) and (flags & Flag.OPTIMIZE):
         print('## Modified Grammar ##')
         print(p.modified_grammar)
 
     return p
 
 
 def match(pattern: str,
           string: str,
           actions: Optional[_FuncMap] = None,
           parser: str = 'packrat',
+          ignore: Optional[Definition] = DEFAULT_IGNORE,
           flags: Flag = Flag.MEMOIZE):
     """Compile *pattern* and match *string* against it.
 
     Example:
         >>> import pe
         >>> pe.match(r'"-"? [1-9] [0-9]*', '-12345').group()
         '-12345'
     """
     expr = compile(pattern,
                    actions=actions,
                    parser=parser,
+                   ignore=ignore,
                    flags=Flag.OPTIMIZE)
     return expr.match(string, flags=flags)
```

### Comparing `pe-0.4.0/pe/_grammar.py` & `pe-0.5.0/pe/_grammar.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/pe/_match.py` & `pe-0.5.0/pe/_match.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/pe/_optimize.py` & `pe-0.5.0/pe/_optimize.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/pe/_parse.py` & `pe-0.5.0/pe/_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,19 @@
   action
 
 The syntax is defined as follows::
 
   # Hierarchical syntax
   Start      <- Spacing (Grammar / Expression) EndOfFile
   Grammar    <- Definition+
-  Definition <- Identifier Operator Expression
-  Operator   <- LEFTARROW
+  Definition <- Identifier defop:Operator Expression
+  Operator   <- LEFTARROW / LEFTANGLE
   Expression <- Sequence (SLASH Sequence)*
-  Sequence   <- Evaluated*
-  Evaluated  <- (prefix:Prefix)? Quantified
+  Sequence   <- Valued*
+  Valued     <- (prefix:Prefix)? Quantified
   Prefix     <- AND / NOT / TILDE / Binding
   Binding    <- Identifier COLON
   Quantified <- Primary (quantifier:Quantifier)?
   Quantifier <- QUESTION / STAR / PLUS
   Primary    <- Name / Group / Literal / Class / DOT
   Name       <- Identifier !Operator
   Group      <- OPEN Expression CLOSE
@@ -48,14 +48,15 @@
               / '\\' 'u' Hex Hex Hex Hex
               / '\\' 'U' Hex Hex Hex Hex Hex Hex Hex Hex
               / !'\\' .
   Oct        <- [0-7]
   Hex        <- [0-9a-fA-F]
 
   LEFTARROW  <- '<-' Spacing
+  LEFTANGLE  <- '<' Space Spacing
   SLASH      <- '/' Spacing
   AND        <- '&' Spacing
   NOT        <- '!' Spacing
   TILDE      <- '~' Spacing
   COLON      <- ':' Spacing
   QUESTION   <- '?' Spacing
   STAR       <- '*' Spacing
@@ -87,14 +88,15 @@
     Plus,
     And,
     Not,
     Capture,
     Bind,
     Sequence,
     Choice,
+    AutoIgnore,
     SymbolTable,
 )
 from pe.packrat import PackratParser
 from pe.actions import Constant, Pack, Warn
 
 
 def _make_literal(s):
@@ -137,45 +139,53 @@
         return exprs[0]
     elif len(exprs) > 1:
         return Choice(*exprs)
     else:
         raise Error(f'empty choice: {exprs}')
 
 
+def _make_definition(identifier, expr, defop=None):
+    if defop is not None:
+        return (identifier, defop(expr))
+    return (identifier, expr)
+
+
 V = SymbolTable()
 
 # Hierarchical syntax
 V.Start = Sequence(V.Spacing, Choice(V.Grammar, V.Expression), V.EOF)
 V.Grammar = Plus(V.Definition)
-V.Definition = Sequence(V.Identifier, V.LEFTARROW, V.Expression)
+V.Definition = Sequence(
+    V.Identifier, Bind(V.Operator, name='defop'), V.Expression
+)
 V.Expression = Sequence(V.Sequence, Star(Sequence(V.SLASH, V.Sequence)))
 V.Sequence = Plus(V.Valued)
 V.Valued = Sequence(Optional(Bind(V.Prefix, name='prefix')), V.Quantified)
 V.Prefix = Choice(V.AND, V.NOT, V.TILDE, V.Binding)
 V.Binding = Sequence(V.Identifier, ':', V.Spacing)
 V.Quantified = Sequence(
     V.Primary, Optional(Bind(V.Quantifier, name='quantifier'))
 )
 V.Quantifier = Choice(V.QUESTION, V.STAR, V.PLUS)
 V.Primary = Choice(V.Name, V.Group, V.Literal, V.Class, V.DOT)
-V.Name = Sequence(V.Identifier, V.Spacing, Not(V.LEFTARROW))
+V.Name = Sequence(V.Identifier, V.Spacing, Not(V.Operator))
 V.Group = Sequence(V.OPEN, V.Expression, V.CLOSE)
 V.Literal = Sequence(
     Choice(
         Capture(Sequence("'", Star(Sequence(Not("'"), V.Char)), "'")),
         Capture(Sequence('"', Star(Sequence(Not('"'), V.Char)), '"'))),
     V.Spacing
 )
 V.Class = Sequence(
     '[', Capture(Star(Sequence(Not(']'), V.Range))), ']', V.Spacing
 )
 
 # Non-recursive patterns
 
-# V.Operator = Choice(V.LEFTARROW)
+V.Operator = Choice(V.LEFTARROW, V.LEFTANGLE)
 V.Special = Class('tnvfr"\'[]\\\\')
 V.Oct = Class('0-7')
 V.Hex = Class('0-9a-fA-F')
 V.Octal = Sequence(V.Oct, Optional(V.Oct), Optional(V.Oct))
 V.UTF8 = Sequence('x', *([V.Hex] * 2))
 V.UTF16 = Sequence('u', *([V.Hex] * 4))
 V.UTF32 = Sequence('U', *([V.Hex] * 8))
@@ -190,14 +200,15 @@
 V.Identifier = Sequence(
     Capture(Sequence(V.IdentStart, Star(V.IdentCont))), V.Spacing
 )
 
 # Tokens
 
 V.LEFTARROW = Sequence('<-', V.Spacing)
+V.LEFTANGLE = Sequence('<', V.Space, V.Spacing)
 V.SLASH = Sequence('/', V.Spacing)
 V.AND = Sequence('&', V.Spacing)
 V.NOT = Sequence('!', V.Spacing)
 V.TILDE = Sequence('~', V.Spacing)
 V.QUESTION = Sequence('?', V.Spacing)
 V.STAR = Sequence('*', V.Spacing)
 V.PLUS = Sequence('+', V.Spacing)
@@ -213,29 +224,30 @@
 V.EOF = Not(Dot())
 V.EOL = Choice('\r\n', '\n', '\r')
 
 PEG = Grammar(
     definitions=V,
     actions={
         'Grammar': Pack(tuple),
-        'Definition': Pack(tuple),
+        'Definition': _make_definition,
         'Expression': Pack(_make_prioritized),
         'Sequence': Pack(_make_sequential),
         'Valued': _make_valued,
         'AND': Constant(And),
         'NOT': Constant(Not),
         'TILDE': Constant(Capture),
         'Binding': _make_binder,
         'Quantified': _make_quantified,
         'QUESTION': Constant(Optional),
         'STAR': Constant(Star),
         'PLUS': Constant(Plus),
         'Name': Nonterminal,
         'Literal': _make_literal,
         'Class': _make_class,
+        'LEFTANGLE': Constant(AutoIgnore),
         'DOT': Constant(Dot()),
         'RangeEndWarn': Warn(
             'The second character in a range may be an unescaped "]", '
             'but this is often a mistake. Silence this warning by '
             'escaping the hyphen (\\-) or the right bracket (\\]), '
             'depending on what was intended.')
     }
```

### Comparing `pe-0.4.0/pe/_parser.py` & `pe-0.5.0/pe/_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 
-from typing import Union
+from typing import Union, Optional
 
 from pe._constants import Flag
 from pe._match import Match
 from pe._definition import Definition
 from pe._grammar import Grammar
 
 
 class Parser:
     grammar: Grammar
     modified_grammar: Grammar
     flags: Flag
 
     def __init__(self,
                  grammar: Union[Grammar, Definition],
+                 ignore: Optional[Definition] = None,
                  flags: Flag = Flag.NONE):
         if isinstance(grammar, Definition):
             grammar = Grammar({'Start': grammar})
         self.grammar = grammar
         self.modified_grammar = grammar  # may be reassigned later
         self.flags = flags
```

### Comparing `pe-0.4.0/pe/_py_machine.py` & `pe-0.5.0/pe/_py_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 from enum import IntEnum
 import re
 
 from pe._constants import FAIL as FAILURE, Operator, Flag
 from pe._errors import Error
 from pe._match import Match
 from pe._types import Memo
+from pe._definition import Definition
 from pe._grammar import Grammar
 from pe._parser import Parser
 from pe._optimize import optimize
+from pe._autoignore import autoignore
 from pe.actions import Action, Bind
 from pe.operators import Rule
+from pe.patterns import DEFAULT_IGNORE
 
 
 # Parser ###############################################################
 
 class OpCode(IntEnum):
     FAIL = -1
     PASS = 0
@@ -90,17 +93,20 @@
 ) -> _Instruction:
     return (opcode, oploc, scanner, marking, capturing, action, name)
 
 
 class MachineParser(Parser):
 
     def __init__(self, grammar: Grammar,
+                 ignore: Optional[Definition] = DEFAULT_IGNORE,
                  flags: Flag = Flag.NONE):
         super().__init__(grammar, flags=flags)
 
+        grammar = autoignore(grammar, ignore)
+
         grammar = optimize(grammar,
                            inline=flags & Flag.INLINE,
                            common=flags & Flag.COMMON,
                            regex=flags & Flag.REGEX)
         # if flags & Flag.DEBUG:
         #     grammar = debug(grammar)
         self.modified_grammar = grammar
```

### Comparing `pe-0.4.0/pe/actions.py` & `pe-0.5.0/pe/actions.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/pe/operators.py` & `pe-0.5.0/pe/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 STR = Operator.STR
 PLS = Operator.PLS
 AND = Operator.AND
 NOT = Operator.NOT
 CAP = Operator.CAP
 BND = Operator.BND
 SEQ = Operator.SEQ
+IGN = Operator.IGN
 CHC = Operator.CHC
 RUL = Operator.RUL
 DBG = Operator.DBG
 
 
 _Def = Union[str, Definition]
 
@@ -160,14 +161,18 @@
     return Definition(RUL, (_validate(expression), action, name))
 
 
 def Debug(expression: _Def):
     return Definition(DBG, (_validate(expression),))
 
 
+def AutoIgnore(expression: _Def):
+    return Definition(IGN, (_validate(expression),))
+
+
 class SymbolTable(Dict[str, Definition]):
     """Dictionary subclass for simplifying grammar construction."""
 
     def __setattr__(self, name: str, value: Definition) -> None:
         dict.__setitem__(self, name, value)
 
     def __getattr__(self, name: str) -> Definition:
```

### Comparing `pe-0.4.0/pe/packrat.py` & `pe-0.5.0/pe/packrat.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,27 +22,36 @@
 from pe._errors import Error, ParseError
 from pe._definition import Definition
 from pe._match import Match, determine
 from pe._types import RawMatch, Memo
 from pe._grammar import Grammar
 from pe._parser import Parser
 from pe._optimize import optimize, regex
+from pe._autoignore import autoignore
 from pe._debug import debug
 from pe._misc import ansicolor
 from pe.actions import Action
+from pe.patterns import DEFAULT_IGNORE
 
 
 _Matcher = Callable[[str, int, Memo], RawMatch]
 
 
 class PackratParser(Parser):
 
-    def __init__(self, grammar: Grammar, flags: Flag = Flag.NONE):
+    def __init__(
+        self,
+        grammar: Grammar,
+        ignore: Optional[Definition] = DEFAULT_IGNORE,
+        flags: Flag = Flag.NONE
+    ):
         super().__init__(grammar, flags=flags)
 
+        grammar = autoignore(grammar, ignore)
+
         grammar = optimize(grammar,
                            inline=flags & Flag.INLINE,
                            common=flags & Flag.COMMON,
                            regex=flags & Flag.REGEX)
         if flags & Flag.DEBUG:
             grammar = debug(grammar)
         self.modified_grammar = grammar
@@ -287,30 +296,49 @@
         subdef: Definition
         action: Action
         name: str
         subdef, action, name = definition.args
         expression = self._def_to_expr(subdef)
         return Rule(name, expression, action)
 
+    @staticmethod
+    def _format_snippet(text: str) -> str:
+        """Escape any characters that create large amounts of whitespace,
+        mainly line breaking characters like newlines but also tabs.
+        """
+        offending_characters = str.maketrans({
+            "\n": r"\n",  # newline
+            "\r": r"\r",  # carriage return
+            "\v": r"\v",  # vertical tab
+            "\t": r"\t",  # horizontal tab
+            "\f": r"\f",  # form feed
+            "\u0085": r"\u0085",  # NEL next line
+            "\u2028": r"\u2028",  # \N{LINE SEPARATOR}
+            "\u2029": r"\u2029",  # \N{PARAGRAPH SEPARATOR}
+        })
+        return text.translate(offending_characters)
+
     def _debug(self, definition: Definition) -> _Matcher:
         subdef: Definition = definition.args[0]
         expression = self._def_to_expr(subdef)
 
         def _match(s: str, pos: int, memo: Memo) -> RawMatch:
             # for proper printing, only terminals can print after
             # knowing the result
+            snippet = self._format_snippet(s[pos:pos+10])[:10].ljust(12)
+
             if subdef.op.precedence == 6 and subdef.op != Operator.SYM:
                 end, args, kwargs = expression(s, pos, memo)
                 indent = ' ' * len(inspect.stack(0))
                 color = 'green' if end >= 0 else 'red'
                 defstr = ansicolor(color, str(subdef))
-                print(f'{s[pos:pos+10]:<12} | {indent}{defstr}')
+                print(f'{snippet} | {indent}{defstr}')
             else:
-                print('{:<12} | {}{!s}'.format(
-                    s[pos:pos+10],
+                print('{} | {}{!s}'.format(
+                    snippet,
                     ' ' * len(inspect.stack(0)),
                     str(subdef)))
                 end, args, kwargs = expression(s, pos, memo)
             return end, args, kwargs
 
         return _match
```

### Comparing `pe-0.4.0/pe.egg-info/PKG-INFO` & `pe-0.5.0/pe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe
-Version: 0.4.0
+Version: 0.5.0
 Summary: Library for Parsing Expression Grammars (PEG)
 Home-page: https://github.com/goodmami/pe/
 Author: Michael Wayne Goodman
 Author-email: goodman.m.w@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/goodmami/pe/blob/main/docs/README.md
 Project-URL: Changelog, https://github.com/goodmami/pe/blob/main/CHANGELOG.md
@@ -131,14 +131,17 @@
 
 # (extension) binding
 name:e       # bind result of e to 'name'
 
 # grammars
 Name <- ...  # define a rule named 'Name'
 ... <- Name  # refer to rule named 'Name'
+
+# (extension) auto-ignore
+X <  e1 e2   # define a rule 'X' with auto-ignore
 ```
 
 ## Matching Inputs with Parsing Expressions
 
 When a parsing expression matches an input, it returns a `Match`
 object, which is similar to those of Python's
 [re](https://docs.python.org/3/library/re.html) module for regular
@@ -209,29 +212,43 @@
 func(sep.join(match.groups()), **match.groupdict())
 ```
 
 [Action]: docs/api/pe.actions.md#Action
 [Pack]: docs/api/pe.actions.md#Pack
 [Join]: docs/api/pe.actions.md#Join
 
+### Auto-ignore
+
+The grammar can be defined such that some rules ignore occurrences of
+a pattern between sequence items. Most commonly, this is used to
+ignore whitespace, so the default ignore pattern is simple whitespace.
+
+```python
+>>> pe.match("X <- 'a' 'b'", "a b")  # regular rule does not match
+>>> pe.match("X <  'a' 'b'", "a b")  # auto-ignore rule matches
+<Match object; span=(0, 3), match='a b'>
+
+```
+
+This feature can help to make grammars more readable.
 
 ### Example
 
 Here is one way to parse a list of comma-separated integers:
 
 ```python
 >>> from pe.actions import Pack
 >>> p = pe.compile(
 ...   r'''
 ...     Start  <- "[" Values? "]"
 ...     Values <- Int ("," Int)*
-...     Int    <- ~( "-"? ("0" / [1-9] [0-9]*) )
+...     Int    <  ~( "-"? ("0" / [1-9] [0-9]*) )
 ...   ''',
 ...   actions={'Values': Pack(list), 'Int': int})
->>> m = p.match('[5,10,-15]')
+>>> m = p.match('[5, 10, -15]')
 >>> m.value()
 [5, 10, -15]
 
 ```
 
 ## Similar Projects
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pe Version: 0.4.0 Summary: Library for Parsing
+Metadata-Version: 2.1 Name: pe Version: 0.5.0 Summary: Library for Parsing
 Expression Grammars (PEG) Home-page: https://github.com/goodmami/pe/ Author:
 Michael Wayne Goodman Author-email: goodman.m.w@gmail.com License: MIT Project-
 URL: Documentation, https://github.com/goodmami/pe/blob/main/docs/README.md
 Project-URL: Changelog, https://github.com/goodmami/pe/blob/main/CHANGELOG.md
 Keywords: peg,parsing,text Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
@@ -48,15 +48,16 @@
 terminals . # any single character "abc" # string literal 'abc' # string
 literal [abc] # character class # repeating expressions e # exactly one e? #
 zero or one (optional) e* # zero or more e+ # one or more # combining
 expressions e1 e2 # sequence of e1 and e2 e1 / e2 # ordered choice of e1 and e2
 (e) # subexpression # lookahead &e # positive lookahead !e # negative lookahead
 # (extension) capture substring ~e # result of e is matched substring #
 (extension) binding name:e # bind result of e to 'name' # grammars Name <- ...
-# define a rule named 'Name' ... <- Name # refer to rule named 'Name' ``` ##
+# define a rule named 'Name' ... <- Name # refer to rule named 'Name' #
+(extension) auto-ignore X < e1 e2 # define a rule 'X' with auto-ignore ``` ##
 Matching Inputs with Parsing Expressions When a parsing expression matches an
 input, it returns a `Match` object, which is similar to those of Python's [re]
 (https://docs.python.org/3/library/re.html) module for regular expressions. By
 default, nothing is captured, but the capture operator (`~`) emits the
 substring of the matching expression, similar to regular expression's capturing
 groups: ```python >>> e = pe.compile(r'[0-9] [.] [0-9]') >>> m = e.match('1.4')
 >>> m.group() '1.4' >>> m.groups() () >>> e = pe.compile(r'~([0-9] [.] [0-9])')
@@ -74,20 +75,26 @@
 are cleared. For more control, **pe** provides the [Action] class and a number
 of subclasses for various use-cases. These actions have access to more
 information about a parse result and more control over the match. For example,
 the [Pack] class takes a function and calls it with the emitted values packed
 into a list: ``` python func(match.groups()) ``` And the [Join] class joins all
 emitted strings with a separator: ``` python func(sep.join(match.groups()),
 **match.groupdict()) ``` [Action]: docs/api/pe.actions.md#Action [Pack]: docs/
-api/pe.actions.md#Pack [Join]: docs/api/pe.actions.md#Join ### Example Here is
-one way to parse a list of comma-separated integers: ```python >>> from
-pe.actions import Pack >>> p = pe.compile( ... r''' ... Start <- "[" Values?
-"]" ... Values <- Int ("," Int)* ... Int <- ~( "-"? ("0" / [1-9] [0-9]*) ) ...
-''', ... actions={'Values': Pack(list), 'Int': int}) >>> m = p.match('[5,10,-
-15]') >>> m.value() [5, 10, -15] ``` ## Similar Projects - [Lark](https://
-github.com/lark-parser/lark) (Python) - [nom](https://github.com/Geal/nom)
-(Rust) - [Parsimonious](https://github.com/erikrose/parsimonious) (Python) -
-[Rosie](https://rosie-lang.org/) (Multiple bindings) - [TatSu](https://
-tatsu.readthedocs.io/en/stable/) (Python) - [PEG.js](https://github.com/pegjs/
-pegjs) (Javascript) - [Pegged](https://github.com/PhilippeSigaud/Pegged) (D) -
-[pegen](https://github.com/gvanrossum/pegen) (Python / C) - [LPeg] (Lua)
-[LPeg]: http://www.inf.puc-rio.br/~roberto/lpeg/
+api/pe.actions.md#Pack [Join]: docs/api/pe.actions.md#Join ### Auto-ignore The
+grammar can be defined such that some rules ignore occurrences of a pattern
+between sequence items. Most commonly, this is used to ignore whitespace, so
+the default ignore pattern is simple whitespace. ```python >>> pe.match("X <-
+'a' 'b'", "a b") # regular rule does not match >>> pe.match("X < 'a' 'b'", "a
+b") # auto-ignore rule matches
+ span=(0, 3), match='a b'> ``` This feature can help to make grammars more
+readable. ### Example Here is one way to parse a list of comma-separated
+integers: ```python >>> from pe.actions import Pack >>> p = pe.compile( ...
+r''' ... Start <- "[" Values? "]" ... Values <- Int ("," Int)* ... Int < ~( "-
+"? ("0" / [1-9] [0-9]*) ) ... ''', ... actions={'Values': Pack(list), 'Int':
+int}) >>> m = p.match('[5, 10, -15]') >>> m.value() [5, 10, -15] ``` ## Similar
+Projects - [Lark](https://github.com/lark-parser/lark) (Python) - [nom](https:/
+/github.com/Geal/nom) (Rust) - [Parsimonious](https://github.com/erikrose/
+parsimonious) (Python) - [Rosie](https://rosie-lang.org/) (Multiple bindings) -
+[TatSu](https://tatsu.readthedocs.io/en/stable/) (Python) - [PEG.js](https://
+github.com/pegjs/pegjs) (Javascript) - [Pegged](https://github.com/
+PhilippeSigaud/Pegged) (D) - [pegen](https://github.com/gvanrossum/pegen)
+(Python / C) - [LPeg] (Lua) [LPeg]: http://www.inf.puc-rio.br/~roberto/lpeg/
```

### Comparing `pe-0.4.0/pe.egg-info/SOURCES.txt` & `pe-0.5.0/pe.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 pe/__init__.py
+pe/_autoignore.py
 pe/_constants.py
 pe/_cy_machine.c
 pe/_cy_machine.pyx
 pe/_debug.py
 pe/_definition.py
+pe/_disarm.py
 pe/_errors.py
 pe/_escape.py
 pe/_functions.py
 pe/_grammar.py
 pe/_match.py
 pe/_meta.py
 pe/_misc.py
@@ -21,20 +23,22 @@
 pe/_parser.py
 pe/_py_machine.py
 pe/_types.py
 pe/actions.py
 pe/machine.py
 pe/operators.py
 pe/packrat.py
+pe/patterns.py
 pe.egg-info/PKG-INFO
 pe.egg-info/SOURCES.txt
 pe.egg-info/dependency_links.txt
 pe.egg-info/not-zip-safe
 pe.egg-info/top_level.txt
 test/test__definition.py
+test/test__disarm.py
 test/test__match.py
 test/test__optimize.py
 test/test__parse.py
 test/test_operators.py
 test/test_parsers.py
 test/test_pe.py
 test/test_regression.py
```

### Comparing `pe-0.4.0/setup.cfg` & `pe-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/setup.py` & `pe-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/test/test__match.py` & `pe-0.5.0/test/test__match.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/test/test__optimize.py` & `pe-0.5.0/test/test__optimize.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/test/test__parse.py` & `pe-0.5.0/test/test__parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Star,
     Plus,
     Nonterminal,
     And,
     Not,
     Capture,
     Bind,
+    AutoIgnore,
 )
 from pe._parse import loads
 
 
 def eloads(s):
     start, defmap = loads(s)
     return defmap[start]
@@ -118,14 +119,21 @@
     assert loads('''
         A   <- "a" Bee
         Bee <- "b"
     ''') == ('A', {'A': Sequence('a', Nonterminal('Bee')),
                    'Bee': Literal('b')})
 
 
+def test_loads_autoignore_def():
+    assert loads('A <  "a"') == ('A', {'A': AutoIgnore('a')})
+    assert loads('A <  ~"a"') == ('A', {'A': AutoIgnore(Capture('a'))})
+    assert loads('A <  "a"*') == ('A', {'A': AutoIgnore(Star('a'))})
+    assert loads('A <  "a" "b"') == ('A', {'A': AutoIgnore(Sequence('a', 'b'))})
+
+
 def test_loads_error():
     with pytest.raises(GrammarError):
         loads('')
     with pytest.raises(GrammarError):
         loads('A <- +"a"')
     with pytest.raises(GrammarError):
         loads('A <- "a"+*')
```

### Comparing `pe-0.4.0/test/test_operators.py` & `pe-0.5.0/test/test_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Star,
     Plus,
     Nonterminal,
     And,
     Not,
     Capture,
     Bind,
+    AutoIgnore,
 )
 
 
 def test_Dot():
     assert Dot() == Def(Op.DOT, ())
 
 
@@ -92,7 +93,12 @@
     assert Capture(Dot()) == Def(Op.CAP, (Dot(),))
     assert Capture('foo') == Capture(Literal('foo'))
 
 
 def test_Bind():
     assert Bind(Dot(), name='x') == Def(Op.BND, (Dot(), 'x'))
     assert Bind('foo', name='bar') == Bind(Literal('foo'), name='bar')
+
+
+def test_AutoIgnore():
+    assert AutoIgnore(Dot()) == Def(Op.IGN, (Dot(),))
+    assert AutoIgnore('foo') == AutoIgnore(Literal('foo'))
```

### Comparing `pe-0.4.0/test/test_parsers.py` & `pe-0.5.0/test/test_parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     And,
     Not,
     Bind as Bnd,
     Capture as Cap,
     Sequence as Seq,
     Choice as Chc,
     Rule as Rul,
+    AutoIgnore as Ign,
 )
 from pe._grammar import Grammar
 from pe.actions import Pack
 from pe.packrat import PackratParser
 from pe._py_machine import MachineParser as PyMachineParser
 try:
     from pe._cy_machine import MachineParser as CyMachineParser
@@ -135,14 +136,25 @@
 
     # Regression tests for Machine Parser
     ('Rgr0', Cap(Sym('abc')), 'a',      0, 1,    (('a',), {}, 'a')),
     ('Rgr1', Cap(Sym('abcs')), 'aaa',   0, 3,    (('aaa',), {}, 'aaa')),
     ('Rgr2', Seq(abc, Not(Dot())),
                               'a',      0, 1,    _blank),
 
+    ('Ign0', Ign(abc),        'a',      0, 1,    _blank),
+    ('Ign1', Ign(abc),        ' a  ',   0, 4,    _blank),
+    ('Ign2', Ign(abc),        ' x  ',   0, FAIL, None),
+    ('Ign3', Ign(abseq),      ' a b ',  0, 5,    _blank),
+    ('Ign4', Ign(Pls(xyz)),   ' xy ',   0, 4,    _blank),
+    ('Ign5', Ign(Pls(xyz)),   ' x y ',  0, 3,    _blank),
+    ('Ign6', Ign(Str(xyz)),   ' a ',    0, 1,    _blank),
+    ('Ign7', Ign(Pls(abseq)), ' abab ', 0, 6,    _blank),
+    ('Ign8', Ign(Pls(abseq)), ' ab ab', 0, 4,    _blank),
+    ('Ign9', Ign(Pls(abseq)), 'a ba b', 0, FAIL, None),
+
 ]
 
 
 @pytest.mark.parametrize('parser,dfn,input,pos,end,match',
                          [(parser,) + row[1:]
                           for parser in [PackratParser,
                                          PyMachineParser,
@@ -161,7 +173,13 @@
         assert m is None
     else:
         groups, groupdict, value = match
         assert m.end() == end
         assert m.groups() == groups
         assert m.groupdict() == groupdict
         assert m.value() == value
+
+
+def test_snippet_escaping():
+    input = "😊\nあ\rA\vB\tC\fD\u0085E\u2028F\u2029"
+    output = r"😊\nあ\rA\vB\tC\fD\u0085E\u2028F\u2029"
+    assert PackratParser._format_snippet(input) == output
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pe-0.4.0/test/test_pe.py` & `pe-0.5.0/test/test_pe.py`

 * *Files identical despite different names*

### Comparing `pe-0.4.0/test/test_regression.py` & `pe-0.5.0/test/test_regression.py`

 * *Files identical despite different names*

