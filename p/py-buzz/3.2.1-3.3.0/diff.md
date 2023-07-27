# Comparing `tmp/py-buzz-3.2.1.tar.gz` & `tmp/py_buzz-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-buzz-3.2.1.tar", max compression
+gzip compressed data, was "py_buzz-3.3.0.tar", max compression
```

## Comparing `py-buzz-3.2.1.tar` & `py_buzz-3.3.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1099 2022-06-20 23:10:37.179242 py-buzz-3.2.1/LICENSE.rst
--rw-r--r--   0        0        0     1996 2022-06-20 23:10:37.179242 py-buzz-3.2.1/README.rst
--rw-r--r--   0        0        0      394 2022-06-20 23:10:37.179242 py-buzz-3.2.1/buzz/__init__.py
--rw-r--r--   0        0        0     2535 2022-06-20 23:10:37.179242 py-buzz-3.2.1/buzz/base.py
--rw-r--r--   0        0        0        0 2022-06-20 23:10:37.179242 py-buzz-3.2.1/buzz/py.typed
--rw-r--r--   0        0        0    10034 2022-06-20 23:10:37.179242 py-buzz-3.2.1/buzz/tools.py
--rw-r--r--   0        0        0     1089 2022-06-20 23:10:37.183242 py-buzz-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     2751 2022-06-20 23:10:45.655808 py-buzz-3.2.1/setup.py
--rw-r--r--   0        0        0     2657 2022-06-20 23:10:45.656112 py-buzz-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2022-03-30 16:27:40.385941 py_buzz-3.3.0/LICENSE.rst
+-rw-r--r--   0        0        0     1996 2022-06-20 21:10:42.949372 py_buzz-3.3.0/README.rst
+-rw-r--r--   0        0        0      394 2022-06-20 21:10:42.949372 py_buzz-3.3.0/buzz/__init__.py
+-rw-r--r--   0        0        0     2535 2022-06-20 23:09:43.479472 py_buzz-3.3.0/buzz/base.py
+-rw-r--r--   0        0        0        0 2022-03-30 16:27:40.385941 py_buzz-3.3.0/buzz/py.typed
+-rw-r--r--   0        0        0    10824 2023-07-27 16:37:46.987907 py_buzz-3.3.0/buzz/tools.py
+-rw-r--r--   0        0        0     1089 2023-07-27 16:37:46.997907 py_buzz-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 py_buzz-3.3.0/PKG-INFO
```

### Comparing `py-buzz-3.2.1/LICENSE.rst` & `py_buzz-3.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `py-buzz-3.2.1/README.rst` & `py_buzz-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `py-buzz-3.2.1/buzz/base.py` & `py_buzz-3.3.0/buzz/base.py`

 * *Files identical despite different names*

### Comparing `py-buzz-3.2.1/buzz/tools.py` & `py_buzz-3.3.0/buzz/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,34 @@
 from typing import Any, Callable, Iterable, Iterator, Mapping, Optional, Tuple, Type, TypeVar, Union
 
 
 def noop(*_, **__):
     pass
 
 
+TExc = TypeVar("TExc", bound=Exception)
+
+
+def default_exc_builder(exc: Type[TExc], message: str, *args, **kwargs) -> TExc:
+    """
+    Build an exception instance using default behavior where message is passed as first positional argument.
+
+    Some exception types such as FastAPI's HTTPException do not take a message as the first positional argument, so
+    they will need a different exception builder.
+    """
+    return exc(message, *args, **kwargs)
+
+
 def require_condition(
     expr: Any,
     message: str,
     raise_exc_class: Type[Exception] = Exception,
     raise_args: Optional[Iterable[Any]] = None,
     raise_kwargs: Optional[Mapping[str, Any]] = None,
+    exc_builder: Callable[..., Exception] = default_exc_builder,
 ):
     """
     Assert that an expression is truthy. If the assertion fails, raise an exception with the supplied message.
 
     :param: message:          The failure message to attach to the raised Exception
     :param: expr:             The value that is checked for truthiness (usually an evaluated expression)
     :param: raise_exc_class:  The exception type to raise with the constructed message if the expression is falsey.
@@ -41,26 +55,27 @@
     """
     if raise_exc_class is None:
         raise ValueError("The raise_exc_class kwarg may not be None")
 
     if not expr:
         args = raise_args or []
         kwargs = raise_kwargs or {}
-        raise raise_exc_class(message, *args, **kwargs)
+        raise exc_builder(raise_exc_class, message, *args, **kwargs)
 
 
 TNonNull = TypeVar("TNonNull")
 
 
 def enforce_defined(
     value: Optional[TNonNull],
     message: str = "Value was not defined (None)",
     raise_exc_class: Type[Exception] = Exception,
     raise_args: Optional[Iterable[Any]] = None,
     raise_kwargs: Optional[Mapping[str, Any]] = None,
+    exc_builder: Callable[..., Exception] = default_exc_builder,
 ) -> TNonNull:
     """
     Assert that a value is not None. If the assertion fails, raise an exception with the supplied message.
 
     :param: value:            The value that is checked to be non-null
     :param: message:          The failure message to attach to the raised Exception
     :param: expr:             The value that is checked for truthiness (usually an evaluated expression)
@@ -74,15 +89,15 @@
     :param: raise_kwargs:     Keyword args that will be passed when raising an instance of the ``raise_exc_class``.
     """
     if value is not None:
         return value
     else:
         args = raise_args or []
         kwargs = raise_kwargs or {}
-        raise raise_exc_class(message, *args, **kwargs)
+        raise exc_builder(raise_exc_class, message, *args, **kwargs)
 
 
 class _ExpressionChecker:
     """
     A utility class to be used with the ``check_expressions`` context manager.
     """
 
@@ -114,14 +129,15 @@
 
 @contextlib.contextmanager
 def check_expressions(
     main_message: str,
     raise_exc_class: Type[Exception] = Exception,
     raise_args: Optional[Iterable[Any]] = None,
     raise_kwargs: Optional[Mapping[str, Any]] = None,
+    exc_builder: Callable[..., Exception] = default_exc_builder,
 ):
     """
     Check a series of expressions inside of a context manager. If any fail an exception is raised that contains a
     main message and a description of each failing expression.
 
     :param: main message:      The main failure message to include in the constructed message that is passed to the
                                raised Exception
@@ -166,14 +182,15 @@
 
     require_condition(
         len(checker.problems) == 0,
         message,
         raise_exc_class=raise_exc_class,
         raise_args=raise_args,
         raise_kwargs=raise_kwargs,
+        exc_builder=exc_builder,
     )
 
 
 def reformat_exception(message: str, err: Exception) -> str:
     """
     Reformat an exception by adding a message to it and reporting the original exception name and message.
     """
@@ -204,14 +221,15 @@
     raise_exc_class: Union[Type[Exception], None] = Exception,
     raise_args: Optional[Iterable[Any]] = None,
     raise_kwargs: Optional[Mapping[str, Any]] = None,
     handle_exc_class: Union[Type[Exception], Tuple[Type[Exception], ...]] = Exception,
     do_finally: Callable[[], None] = noop,
     do_except: Callable[[DoExceptParams], None] = noop,
     do_else: Callable[[], None] = noop,
+    exc_builder: Callable[..., Exception] = default_exc_builder,
 ) -> Iterator[None]:
     """
     Provide a context manager that will intercept exceptions and repackage them with a message attached:
 
     Example:
 
     .. code-block:: python
@@ -235,15 +253,15 @@
                                Defaults to Exception (will handle all exceptions). May also be provided as a tuple
                                of multiple exception types to handle.
     :param: do_finally:        A function that should always be called at the end of the block.
                                Should take no parameters.
     :param: do_except:         A function that should be called only if there was an exception. Must accept one
                                parameter that is an instance of the ``DoExceptParams`` dataclass.
                                Note that the ``do_except`` method is passed the *original exception*.
-    :param: do_else:           A function taht should be called only if there were no exceptions encountered.
+    :param: do_else:           A function that should be called only if there were no exceptions encountered.
     """
     try:
         yield
     except handle_exc_class as err:
         try:
             final_message = reformat_exception(message, err)
         except Exception as msg_err:
@@ -251,12 +269,12 @@
 
         trace = get_traceback()
 
         do_except(DoExceptParams(err, final_message, trace))  # type: ignore # For packport of dataclasses in python3.6
         if raise_exc_class is not None:
             args = raise_args or []
             kwargs = raise_kwargs or {}
-            raise raise_exc_class(final_message, *args, **kwargs).with_traceback(trace) from err
+            raise exc_builder(raise_exc_class, final_message, *args, **kwargs).with_traceback(trace) from err
     else:
         do_else()
     finally:
         do_finally()
```

### Comparing `py-buzz-3.2.1/pyproject.toml` & `py_buzz-3.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-buzz"
-version = "3.2.1"
+version = "3.3.0"
 description = "\"That's not flying, it's falling with style\": Exceptions with extras"
 authors = ["Tucker Beck <tucker.beck@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 packages = [
     { include = 'buzz' }
 ]
```

### Comparing `py-buzz-3.2.1/setup.py` & `py_buzz-3.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,69 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: py-buzz
+Version: 3.3.0
+Summary: "That's not flying, it's falling with style": Exceptions with extras
+License: MIT
+Author: Tucker Beck
+Author-email: tucker.beck@gmail.com
+Requires-Python: >=3.6.2,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dataclasses (>=0.8,<0.9) ; python_version >= "3.6" and python_version < "3.7"
+Description-Content-Type: text/x-rst
+
+.. image::  https://badge.fury.io/py/py-buzz.svg
+   :target: https://badge.fury.io/py/py-buzz
+   :alt:    Latest Version
+
+.. image::  https://travis-ci.org/dusktreader/py-buzz.svg?branch=integration
+   :target: https://travis-ci.org/dusktreader/py-buzz
+   :alt:    Build Status
+
+.. image::  https://readthedocs.org/projects/py-buzz/badge/?version=latest
+   :target: http://py-buzz.readthedocs.io/en/latest/?badge=latest
+   :alt:    Documentation Status
+
+*********
+ py-buzz
+*********
+
+------------------------------------------------------------------
+That's not flying, it's falling with style: Exceptions with extras
+------------------------------------------------------------------
+
+py-buzz supplies some useful tools to use with python exceptions as well
+as a base Buzz exception class that includes them as classmethods.
+
+py-buzz is fully equipped with exception tools that are written over and over
+again in python projects such as:
+
+* checking conditions and raising errors on failure (``require_conditon``)
+* checking that values are defined and raising errors if not (``enforce_defined``)
+* catching exceptions wrapping them in clearer exception types with better error
+  messages (``handle_errors``)
+* checking many conditions and reporting which ones failed
+  (``check_expressions``)
+
+Buzz can be used as a stand-alone exception class, but it is best used as a
+bass class for custom exceptions within a project. This allows the user to
+focus on creating a set of Exceptions that provide complete coverage for issues
+within their application without having to re-write convenience functions
+themselves.
+
+Super-quick Start
+-----------------
+ - requirements: `python3.6+`
+ - install through pip: `$ pip install py-buzz`
+ - minimal usage example: `examples/with_buzz_class.py <https://github.com/dusktreader/py-buzz/tree/master/examples/with_buzz_class.py>`_
 
-packages = \
-['buzz']
+Documentation
+-------------
 
-package_data = \
-{'': ['*']}
+The complete documentation can be found at the
+`py-buzz home page <http://py-buzz.readthedocs.io>`_
 
-extras_require = \
-{':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.8,<0.9']}
-
-setup_kwargs = {
-    'name': 'py-buzz',
-    'version': '3.2.1',
-    'description': '"That\'s not flying, it\'s falling with style": Exceptions with extras',
-    'long_description': ".. image::  https://badge.fury.io/py/py-buzz.svg\n   :target: https://badge.fury.io/py/py-buzz\n   :alt:    Latest Version\n\n.. image::  https://travis-ci.org/dusktreader/py-buzz.svg?branch=integration\n   :target: https://travis-ci.org/dusktreader/py-buzz\n   :alt:    Build Status\n\n.. image::  https://readthedocs.org/projects/py-buzz/badge/?version=latest\n   :target: http://py-buzz.readthedocs.io/en/latest/?badge=latest\n   :alt:    Documentation Status\n\n*********\n py-buzz\n*********\n\n------------------------------------------------------------------\nThat's not flying, it's falling with style: Exceptions with extras\n------------------------------------------------------------------\n\npy-buzz supplies some useful tools to use with python exceptions as well\nas a base Buzz exception class that includes them as classmethods.\n\npy-buzz is fully equipped with exception tools that are written over and over\nagain in python projects such as:\n\n* checking conditions and raising errors on failure (``require_conditon``)\n* checking that values are defined and raising errors if not (``enforce_defined``)\n* catching exceptions wrapping them in clearer exception types with better error\n  messages (``handle_errors``)\n* checking many conditions and reporting which ones failed\n  (``check_expressions``)\n\nBuzz can be used as a stand-alone exception class, but it is best used as a\nbass class for custom exceptions within a project. This allows the user to\nfocus on creating a set of Exceptions that provide complete coverage for issues\nwithin their application without having to re-write convenience functions\nthemselves.\n\nSuper-quick Start\n-----------------\n - requirements: `python3.6+`\n - install through pip: `$ pip install py-buzz`\n - minimal usage example: `examples/with_buzz_class.py <https://github.com/dusktreader/py-buzz/tree/master/examples/with_buzz_class.py>`_\n\nDocumentation\n-------------\n\nThe complete documentation can be found at the\n`py-buzz home page <http://py-buzz.readthedocs.io>`_\n",
-    'author': 'Tucker Beck',
-    'author_email': 'tucker.beck@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6.2,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

