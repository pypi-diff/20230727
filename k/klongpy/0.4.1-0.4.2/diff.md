# Comparing `tmp/klongpy-0.4.1.tar.gz` & `tmp/klongpy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klongpy-0.4.1.tar", last modified: Mon Jul 24 23:21:40 2023, max compression
+gzip compressed data, was "klongpy-0.4.2.tar", last modified: Wed Jul 26 22:46:24 2023, max compression
```

## Comparing `klongpy-0.4.1.tar` & `klongpy-0.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.4.1/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)    22574 2023-07-24 23:21:40.399690 klongpy-0.4.1/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)    21981 2023-07-24 23:20:23.000000 klongpy-0.4.1/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/klongpy/
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.4.1/klongpy/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.4.1/klongpy/adverbs.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.4.1/klongpy/backend.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    26102 2023-07-22 00:22:29.000000 klongpy-0.4.1/klongpy/core.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    30678 2023-07-22 00:22:29.000000 klongpy-0.4.1/klongpy/dyads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20648 2023-07-24 23:20:23.000000 klongpy-0.4.1/klongpy/interpreter.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.4.1/klongpy/monads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    16759 2023-07-22 00:22:29.000000 klongpy-0.4.1/klongpy/sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    15723 2023-07-24 23:20:23.000000 klongpy-0.4.1/klongpy/sys_fn_ipc.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2781 2023-07-24 23:20:23.000000 klongpy-0.4.1/klongpy/sys_fn_timer.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.4.1/klongpy/sys_var.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1558 2023-07-22 00:22:29.000000 klongpy-0.4.1/klongpy/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/klongpy/web/
--rw-rw-r--   0 brian     (1000) brian     (1000)       99 2023-07-22 00:22:29.000000 klongpy-0.4.1/klongpy/web/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4947 2023-07-24 23:20:23.000000 klongpy-0.4.1/klongpy/web/sys_fn_web.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/klongpy.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)    22574 2023-07-24 23:21:40.000000 klongpy-0.4.1/klongpy.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      711 2023-07-24 23:21:40.000000 klongpy-0.4.1/klongpy.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-07-24 23:21:40.000000 klongpy-0.4.1/klongpy.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      231 2023-07-24 23:21:40.000000 klongpy-0.4.1/klongpy.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-07-24 23:21:40.000000 klongpy-0.4.1/klongpy.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/scripts/
--rw-rw-r--   0 brian     (1000) brian     (1000)     7493 2023-07-22 00:22:29.000000 klongpy-0.4.1/scripts/kgpy
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-07-24 23:21:40.399690 klongpy-0.4.1/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1136 2023-07-24 23:20:23.000000 klongpy-0.4.1/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.4.1/tests/test_accel.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.4.1/tests/test_examples.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    24124 2023-07-22 00:22:29.000000 klongpy-0.4.1/tests/test_extra_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.4.1/tests/test_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2780 2023-06-29 18:49:02.000000 klongpy-0.4.1/tests/test_interop.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.4.1/tests/test_join_over.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.4.1/tests/test_prog.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.4.1/tests/test_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.4.1/tests/test_suite_file.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14714 2023-07-22 00:22:29.000000 klongpy-0.4.1/tests/test_sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.4.1/tests/test_util.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.4.2/LICENSE
+-rw-rw-r--   0 brian     (1000) brian     (1000)    23130 2023-07-26 22:46:24.901210 klongpy-0.4.2/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)    22576 2023-07-26 22:46:02.000000 klongpy-0.4.2/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/klongpy/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.4.2/klongpy/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.4.2/klongpy/adverbs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.4.2/klongpy/backend.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    26246 2023-07-26 22:46:02.000000 klongpy-0.4.2/klongpy/core.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    30678 2023-07-22 00:22:29.000000 klongpy-0.4.2/klongpy/dyads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    20565 2023-07-26 22:46:02.000000 klongpy-0.4.2/klongpy/interpreter.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.4.2/klongpy/monads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    16759 2023-07-22 00:22:29.000000 klongpy-0.4.2/klongpy/sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    16745 2023-07-26 22:46:02.000000 klongpy-0.4.2/klongpy/sys_fn_ipc.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3089 2023-07-26 22:46:02.000000 klongpy-0.4.2/klongpy/sys_fn_timer.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.4.2/klongpy/sys_var.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1558 2023-07-22 00:22:29.000000 klongpy-0.4.2/klongpy/utils.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/klongpy/web/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       99 2023-07-22 00:22:29.000000 klongpy-0.4.2/klongpy/web/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4947 2023-07-24 23:20:23.000000 klongpy-0.4.2/klongpy/web/sys_fn_web.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/klongpy.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    23130 2023-07-26 22:46:24.000000 klongpy-0.4.2/klongpy.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      711 2023-07-26 22:46:24.000000 klongpy-0.4.2/klongpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-07-26 22:46:24.000000 klongpy-0.4.2/klongpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      231 2023-07-26 22:46:24.000000 klongpy-0.4.2/klongpy.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-07-26 22:46:24.000000 klongpy-0.4.2/klongpy.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/scripts/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7493 2023-07-22 00:22:29.000000 klongpy-0.4.2/scripts/kgpy
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-07-26 22:46:24.901210 klongpy-0.4.2/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1136 2023-07-26 22:46:02.000000 klongpy-0.4.2/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.4.2/tests/test_accel.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.4.2/tests/test_examples.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    24124 2023-07-22 00:22:29.000000 klongpy-0.4.2/tests/test_extra_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.4.2/tests/test_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3196 2023-07-26 22:46:02.000000 klongpy-0.4.2/tests/test_interop.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.4.2/tests/test_join_over.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.4.2/tests/test_prog.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.4.2/tests/test_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.4.2/tests/test_suite_file.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14714 2023-07-22 00:22:29.000000 klongpy-0.4.2/tests/test_sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.4.2/tests/test_util.py
```

### Comparing `klongpy-0.4.1/LICENSE` & `klongpy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/PKG-INFO` & `klongpy-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python implementation of Klong language.
-Home-page: UNKNOWN
 Author: Brian Guarraci
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: cuda102
-Provides-Extra: cuda110
-Provides-Extra: cuda111
-Provides-Extra: cuda11x
-Provides-Extra: cuda12x
 Provides-Extra: cupy
-Provides-Extra: repl
-Provides-Extra: rocm-4-3
+Provides-Extra: cuda12x
+Provides-Extra: cuda11x
+Provides-Extra: cuda111
+Provides-Extra: cuda110
+Provides-Extra: cuda102
 Provides-Extra: rocm-5-0
+Provides-Extra: rocm-4-3
+Provides-Extra: repl
 Provides-Extra: web
 License-File: LICENSE
 
 
 ![Unit Tests](https://github.com/briangu/klongpy/workflows/Unit%20Tests/badge.svg)
 
 # KlongPy
@@ -364,15 +362,15 @@
 
 ?> f::.cli(8888)
 remote[localhost:8888]:fn
 ?> f("avg::{(+/x)%#x}")
 :monad
 ?> f("avg(!100)")
 49.5
-?> :" Call a remote function and pass a local value (!100)
+?> :" Call a remote function and pass a local value (!100) "
 ?> data::!100
 [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
  24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47
  48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71
  72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95
  96 97 98 99]
 ?> f(:avg,,data)
@@ -451,14 +449,36 @@
 
 ```
 ?> f::.cli(8888)
 ?> .clic(f)
 1
 ```
 
+## Async function calls
+
+KlongPy supports async function calls.  While it works for local functions, its primarily for remote functions.
+
+To indicate a function call should be async, the .async() function wraps the function and the supplied callback is called when complete.
+
+Calling an async function results in 1, indicating it was executed.
+
+```
+?> fn::f(:avg)
+remote[localhost:8888]:avg:monad
+?> cb::{.d("remote done: ");.p(x)}
+:monad
+?> afn::.async(fn;cb)
+async:monad
+?> afn(!100)
+1
+?> remote done: 49.5
+```
+
+Note, the result of .async() is a function, so it's possible to reuse these.
+
 ## Synchronization
 
 While the IPC server I/O is async, the KlongPy interpreter is single-threaded.  All remote operations are synchronous to make it easy to use remote operations as part of a normal workflow.  Of course, when calling over to another KlongPy instance, you have no idea what state that instance is in, but within the calling instance operations will be sequential.
 
 # Web server
 
 KlongPy includes a simple web server module.  It's optional so you need to install the dependencies:
@@ -544,15 +564,15 @@
 ```
 1
 2
 3
 4
 5
 stopping timer
-``
+```
 
 
 # Performance
 
 The Klong language is simple, so the overhead is low.  The bulk of the compute time will likely be spent in NumPy doing actual work.
 
 Here's a contrived rough benchmark to show the magnitude differences between Python, KlongPy (CPU + GPU) and Numpy (CPU).
@@ -715,9 +735,7 @@
 :! :& :, :< :> :?
 ```
 
 # Acknowledgement
 
 HUGE thanks to Nils M Holm for his work on Klong and providing the foundations for this interesting project.
 
-
-
```

### Comparing `klongpy-0.4.1/README.md` & `klongpy-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -340,15 +340,15 @@
 
 ?> f::.cli(8888)
 remote[localhost:8888]:fn
 ?> f("avg::{(+/x)%#x}")
 :monad
 ?> f("avg(!100)")
 49.5
-?> :" Call a remote function and pass a local value (!100)
+?> :" Call a remote function and pass a local value (!100) "
 ?> data::!100
 [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
  24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47
  48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71
  72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95
  96 97 98 99]
 ?> f(:avg,,data)
@@ -427,14 +427,36 @@
 
 ```
 ?> f::.cli(8888)
 ?> .clic(f)
 1
 ```
 
+## Async function calls
+
+KlongPy supports async function calls.  While it works for local functions, its primarily for remote functions.
+
+To indicate a function call should be async, the .async() function wraps the function and the supplied callback is called when complete.
+
+Calling an async function results in 1, indicating it was executed.
+
+```
+?> fn::f(:avg)
+remote[localhost:8888]:avg:monad
+?> cb::{.d("remote done: ");.p(x)}
+:monad
+?> afn::.async(fn;cb)
+async:monad
+?> afn(!100)
+1
+?> remote done: 49.5
+```
+
+Note, the result of .async() is a function, so it's possible to reuse these.
+
 ## Synchronization
 
 While the IPC server I/O is async, the KlongPy interpreter is single-threaded.  All remote operations are synchronous to make it easy to use remote operations as part of a normal workflow.  Of course, when calling over to another KlongPy instance, you have no idea what state that instance is in, but within the calling instance operations will be sequential.
 
 # Web server
 
 KlongPy includes a simple web server module.  It's optional so you need to install the dependencies:
@@ -520,15 +542,15 @@
 ```
 1
 2
 3
 4
 5
 stopping timer
-``
+```
 
 
 # Performance
 
 The Klong language is simple, so the overhead is low.  The bulk of the compute time will likely be spent in NumPy doing actual work.
 
 Here's a contrived rough benchmark to show the magnitude differences between Python, KlongPy (CPU + GPU) and Numpy (CPU).
```

### Comparing `klongpy-0.4.1/klongpy/adverbs.py` & `klongpy-0.4.2/klongpy/adverbs.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/klongpy/backend.py` & `klongpy-0.4.2/klongpy/backend.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/klongpy/core.py` & `klongpy-0.4.2/klongpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 
 class KGFnWrapper:
     def __init__(self, klong, fn):
         self.klong = klong
         self.fn = fn
 
     def __call__(self, *args, **kwargs):
+        if len(args) != self.fn.arity:
+            raise RuntimeError(f"Klong function called with {len(args)} but expected {self.fn.arity}")
         fn_args = [np.asarray(x) if isinstance(x, list) else x for x in args]
         return self.klong.call(KGCall(self.fn.a, [*fn_args], self.fn.arity))
 
 
 class KGCall(KGFn):
     def __str__(self):
         return self.a.__str__() if issubclass(type(self.a), KGLambda) else super().__str__()
@@ -101,19 +103,19 @@
     lambda klong, x: klong(x)
 
     """
     def __init__(self, fn):
         self.fn = fn
         params = inspect.signature(self.fn, follow_wrapped=True).parameters
         self.args = [reserved_fn_symbol_map[x] for x in reserved_fn_args if x in params]
-        self.provide_klong = 'klong' in params
+        self._provide_klong = 'klong' in params
 
     def __call__(self, klong, ctx):
         params = [ctx[x] for x in self.args]
-        return self.fn(klong, *params) if self.provide_klong else self.fn(*params)
+        return self.fn(klong, *params) if self._provide_klong else self.fn(*params)
 
     def get_arity(self):
         return len(self.args)
 
     def __str__(self):
         return get_fn_arity_str(self.get_arity())
```

### Comparing `klongpy-0.4.1/klongpy/dyads.py` & `klongpy-0.4.2/klongpy/dyads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/klongpy/interpreter.py` & `klongpy-0.4.2/klongpy/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     def __setitem__(self, k, v):
         k = k if isinstance(k, KGSym) else KGSym(k)
         self._context[k] = v
 
     def __getitem__(self, k):
         k = k if isinstance(k, KGSym) else KGSym(k)
         r = self._context[k]
-        return KGFnWrapper(self, r) if isinstance(r, KGFn) and not isinstance(r, KGCall) else r
+        return KGFnWrapper(self, r) if issubclass(type(r), KGFn) else r
 
     def _get_op_fn(self, s, arity):
         return self._vm[s] if arity == 1 else self._vd[s]
 
     def _is_monad(self, s):
         return isinstance(s,KGOp) and in_map(s.a, self._vm)
 
@@ -539,33 +539,32 @@
 
         The fundamental design ideas include:
 
         * Python lists contain programs and NumPy arrays contain data.
         * Functions (KGFn) are not invoked unless they are KGCall instances, allowing for function definitions to be differentiated from invocations.
 
         """
-
         if isinstance(x, KGSym):
             try:
                 return self._context[x]
             except KeyError:
                 if x not in reserved_fn_symbols:
                     self._context[x] = x
                 return x
-        elif isinstance(x, KGCall) and not (x.is_op() or x.is_adverb_chain()):
-            return self._eval_fn(KGFn(x.a,x.args,x.arity))
         elif isinstance(x, KGFn):
             if x.is_op():
                 f = self._get_op_fn(x.a.a, x.a.arity)
                 fa = (x.args if isinstance(x.args, list) else [x.args]) if x.args is not None else x.args
                 _y = self.eval(fa[1]) if x.a.arity == 2 else None
                 _x = fa[0] if x.a.a == '::' else self.eval(fa[0])
                 return f(_x) if x.a.arity == 1 else f(_x, _y)
             elif x.is_adverb_chain():
                 return chain_adverbs(self, x.a)()
+            elif isinstance(x, KGCall):
+                return self._eval_fn(x)
         elif isinstance(x, KGCond):
             q = self.call(x[0])
             p = not ((is_number(q) and q == 0) or is_empty(q))
             return self.call(x[1]) if p else self.call(x[2])
         elif isinstance(x,list) and len(x) > 0:
             return [self.call(y) for y in x][-1]
         return x
```

### Comparing `klongpy-0.4.1/klongpy/monads.py` & `klongpy-0.4.2/klongpy/monads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/klongpy/sys_fn.py` & `klongpy-0.4.2/klongpy/sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/klongpy/sys_fn_ipc.py` & `klongpy-0.4.2/klongpy/sys_fn_ipc.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
 class KGRemoteFnProxy(KGLambda):
 
     def __init__(self, nc: NetworkClient, sym: KGSym, arity):
         self.nc = nc
         self.sym = sym
         self.args = reserved_fn_args[:arity]
-        self.provide_klong = False
 
     def __call__(self, _, ctx):
         params = [ctx[reserved_fn_symbol_map[x]] for x in reserved_fn_args[:len(self.args)]]
         return self.nc.call(KGRemoteFnCall(self.sym, params))
 
     def __str__(self):
         return f"{self.nc.__str__()}:{self.sym}{super().__str__()}"
@@ -478,14 +477,51 @@
     bind = parts[0] if len(parts) > 1 else None
     port = int(parts[0] if len(parts) == 1 else parts[1])
     if len(parts) == 1 and port == 0:
         return _ipc_tcp_server.shutdown_server()
     return _ipc_tcp_server.create_server(_main_loop, klong, bind, port)
 
 
+class KGAsyncCall(KGLambda):
+    def __init__(self, loop, fn, cb):
+        self.loop = loop
+        self.cb = cb
+        self.fn = fn
+        self.args = [reserved_fn_symbol_map[x] for x in reserved_fn_args[:fn.arity]]
+   
+    async def acall(self, klong, params):
+        r = klong.call(KGCall(self.fn.a, [*params], self.fn.arity))
+        self.cb(r)
+
+    def __call__(self, klong, ctx):
+        params = [ctx[x] for x in self.args]
+        self.loop.create_task(self.acall(klong, params))
+        return 1
+
+    def __str__(self):
+        return f"async:{super().__str__()}"
+
+
+def eval_sys_fn_create_async_wrapper(klong, x, y):
+    """
+
+        .async(x,y)                             [Async-function-wrapper]
+
+        Returns an async callable wrapper for the function "x" and calls "y"
+        when completed.
+
+    """
+    global _main_loop
+    if not issubclass(type(x),KGFn):
+        return "x must be a function"
+    if not issubclass(type(y),KGFn):
+        return "y must be a function"
+    return KGAsyncCall(_main_loop, x, KGFnWrapper(klong, y))
+
+
 def create_system_functions_ipc():
     def _get_name(s):
         i = s.index(".")
         return s[i : i + s[i:].index("(")]
 
     registry = {}
```

### Comparing `klongpy-0.4.1/klongpy/sys_fn_timer.py` & `klongpy-0.4.2/klongpy/sys_fn_timer.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,39 +21,47 @@
         self.delegate = None
         return 1
     
     def __str__(self):
         return f"timer:{self.name}:{self.interval}"
 
 
-def _call_periodic(loop, name, interval, callback):
+def _call_periodic(loop: asyncio.BaseEventLoop, name, interval, callback):
     start = loop.time()
 
     def run(handle, fn=callback):
         global _main_tid
         assert threading.current_thread().ident == _main_tid
         r = fn()
         if r:
-            handle.delegate = loop.call_later(interval - ((loop.time() - start) % interval), run, handle)
+            if interval == 0:
+                handle.delegate = loop.call_soon(run, handle)
+            else:
+                handle.delegate = loop.call_later(interval - ((loop.time() - start) % interval), run, handle)
         else:
             handle.cancel()
 
     periodic = KGTimerHandler(name, interval)
-    periodic.delegate = loop.call_at(start + interval, run, periodic)
+    if interval == 0:
+        periodic.delegate = loop.call_soon(run, periodic)
+    else:
+        periodic.delegate = loop.call_at(start + interval, run, periodic)
 
     return periodic
 
 
 def eval_sys_fn_timer(klong, x, y, z):
     """
     
         .timer(x, y, z)                                   [Create-timer]
 
         Create a timer named by "x" that repeats every "y" seconds and calls function "z".
 
+        An interval value of 0 indicates immediately callback (async).
+
         The callback function returns 1 to continue, 0 to stop time timer.
 
         Example:
 
             cb::{.p("hello")}
             th::.timer("greeting";1;cb)
 
@@ -69,16 +77,16 @@
             c::{.p("stopping timer");0}
             cb::{:[counter<20;u();c()]}
             th::.timer("count";1;cb)
 
     """
     global _main_loop
     y= int(y)
-    if y <= 0:
-        return "x must be non-zero integer"
+    if y < 0:
+        return "x must be a non-negative integer"
     z = z if isinstance(z, KGCall) else KGFnWrapper(klong, z) if isinstance(z, KGFn) else z
     if not callable(z):
         return "z must be a function"
     return _call_periodic(_main_loop, x, y, z)
 
 
 def eval_sys_fn_cancel_timer(x):
```

### Comparing `klongpy-0.4.1/klongpy/sys_var.py` & `klongpy-0.4.2/klongpy/sys_var.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/klongpy/utils.py` & `klongpy-0.4.2/klongpy/utils.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/klongpy/web/sys_fn_web.py` & `klongpy-0.4.2/klongpy/web/sys_fn_web.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/klongpy.egg-info/PKG-INFO` & `klongpy-0.4.2/klongpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python implementation of Klong language.
-Home-page: UNKNOWN
 Author: Brian Guarraci
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: cuda102
-Provides-Extra: cuda110
-Provides-Extra: cuda111
-Provides-Extra: cuda11x
-Provides-Extra: cuda12x
 Provides-Extra: cupy
-Provides-Extra: repl
-Provides-Extra: rocm-4-3
+Provides-Extra: cuda12x
+Provides-Extra: cuda11x
+Provides-Extra: cuda111
+Provides-Extra: cuda110
+Provides-Extra: cuda102
 Provides-Extra: rocm-5-0
+Provides-Extra: rocm-4-3
+Provides-Extra: repl
 Provides-Extra: web
 License-File: LICENSE
 
 
 ![Unit Tests](https://github.com/briangu/klongpy/workflows/Unit%20Tests/badge.svg)
 
 # KlongPy
@@ -364,15 +362,15 @@
 
 ?> f::.cli(8888)
 remote[localhost:8888]:fn
 ?> f("avg::{(+/x)%#x}")
 :monad
 ?> f("avg(!100)")
 49.5
-?> :" Call a remote function and pass a local value (!100)
+?> :" Call a remote function and pass a local value (!100) "
 ?> data::!100
 [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
  24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47
  48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71
  72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95
  96 97 98 99]
 ?> f(:avg,,data)
@@ -451,14 +449,36 @@
 
 ```
 ?> f::.cli(8888)
 ?> .clic(f)
 1
 ```
 
+## Async function calls
+
+KlongPy supports async function calls.  While it works for local functions, its primarily for remote functions.
+
+To indicate a function call should be async, the .async() function wraps the function and the supplied callback is called when complete.
+
+Calling an async function results in 1, indicating it was executed.
+
+```
+?> fn::f(:avg)
+remote[localhost:8888]:avg:monad
+?> cb::{.d("remote done: ");.p(x)}
+:monad
+?> afn::.async(fn;cb)
+async:monad
+?> afn(!100)
+1
+?> remote done: 49.5
+```
+
+Note, the result of .async() is a function, so it's possible to reuse these.
+
 ## Synchronization
 
 While the IPC server I/O is async, the KlongPy interpreter is single-threaded.  All remote operations are synchronous to make it easy to use remote operations as part of a normal workflow.  Of course, when calling over to another KlongPy instance, you have no idea what state that instance is in, but within the calling instance operations will be sequential.
 
 # Web server
 
 KlongPy includes a simple web server module.  It's optional so you need to install the dependencies:
@@ -544,15 +564,15 @@
 ```
 1
 2
 3
 4
 5
 stopping timer
-``
+```
 
 
 # Performance
 
 The Klong language is simple, so the overhead is low.  The bulk of the compute time will likely be spent in NumPy doing actual work.
 
 Here's a contrived rough benchmark to show the magnitude differences between Python, KlongPy (CPU + GPU) and Numpy (CPU).
@@ -715,9 +735,7 @@
 :! :& :, :< :> :?
 ```
 
 # Acknowledgement
 
 HUGE thanks to Nils M Holm for his work on Klong and providing the foundations for this interesting project.
 
-
-
```

### Comparing `klongpy-0.4.1/klongpy.egg-info/SOURCES.txt` & `klongpy-0.4.2/klongpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/scripts/kgpy` & `klongpy-0.4.2/scripts/kgpy`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/setup.py` & `klongpy-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 
 setup(
     name='klongpy',
     packages=['klongpy', 'klongpy.web'],
-    version='0.4.1',
+    version='0.4.2',
     description='Python implementation of Klong language.',
     author='Brian Guarraci',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `klongpy-0.4.1/tests/test_accel.py` & `klongpy-0.4.2/tests/test_accel.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/tests/test_examples.py` & `klongpy-0.4.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/tests/test_extra_suite.py` & `klongpy-0.4.2/tests/test_extra_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/tests/test_fn.py` & `klongpy-0.4.2/tests/test_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/tests/test_interop.py` & `klongpy-0.4.2/tests/test_interop.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,14 +30,27 @@
             del klong['foo']
 
     def test_python_lambda(self):
         klong = KlongInterpreter()
         klong['fn'] = lambda x: x+10
         self.assertEqual(klong('fn(2)'), 12)
 
+    def test_call_klong_python_lambda(self):
+        klong = KlongInterpreter()
+        klong['fn'] = lambda x: x+10
+        fn = klong['fn']
+        self.assertEqual(fn(1),11)
+
+    def test_invalid_call_klong_python_lambda(self):
+        klong = KlongInterpreter()
+        klong['fn'] = lambda x: x+10
+        fn = klong['fn']
+        with self.assertRaises(RuntimeError):
+            self.assertEqual(fn(1,2),11)
+
     def test_call_klong_fn_with_scalar(self):
         klong = KlongInterpreter()
         klong('fn::{x+10}')
         r = klong['fn'](2)
         self.assertEqual(r, 12)
 
     def test_call_klong_fn_with_multiple_scalars(self):
```

### Comparing `klongpy-0.4.1/tests/test_join_over.py` & `klongpy-0.4.2/tests/test_join_over.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/tests/test_prog.py` & `klongpy-0.4.2/tests/test_prog.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/tests/test_suite.py` & `klongpy-0.4.2/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/tests/test_suite_file.py` & `klongpy-0.4.2/tests/test_suite_file.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/tests/test_sys_fn.py` & `klongpy-0.4.2/tests/test_sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.1/tests/test_util.py` & `klongpy-0.4.2/tests/test_util.py`

 * *Files identical despite different names*

