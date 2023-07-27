# Comparing `tmp/Flask-Injector-0.8.0.tar.gz` & `tmp/Flask-Injector-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Injector-0.8.0.tar", last modified: Tue Oct 18 17:39:34 2016, max compression
+gzip compressed data, was "dist/Flask-Injector-0.9.0.tar", last modified: Thu Feb  9 14:26:08 2017, max compression
```

## Comparing `Flask-Injector-0.8.0.tar` & `Flask-Injector-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2016-10-18 17:39:34.000000 Flask-Injector-0.8.0/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2016-10-18 17:39:34.000000 Flask-Injector-0.8.0/Flask_Injector.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     7464 2016-10-18 17:39:33.000000 Flask-Injector-0.8.0/Flask_Injector.egg-info/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)      281 2016-10-18 17:39:33.000000 Flask-Injector-0.8.0/Flask_Injector.egg-info/SOURCES.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2016-10-18 17:39:33.000000 Flask-Injector-0.8.0/Flask_Injector.egg-info/dependency_links.txt
--rw-r--r--   0 kuba       (501) staff       (20)       22 2016-10-18 17:39:33.000000 Flask-Injector-0.8.0/Flask_Injector.egg-info/requires.txt
--rw-r--r--   0 kuba       (501) staff       (20)       15 2016-10-18 17:39:33.000000 Flask-Injector-0.8.0/Flask_Injector.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2016-10-18 16:46:09.000000 Flask-Injector-0.8.0/Flask_Injector.egg-info/zip-safe
--rw-r--r--   0 kuba       (501) staff       (20)       19 2016-10-18 16:46:09.000000 Flask-Injector-0.8.0/MANIFEST.in
--rw-r--r--   0 kuba       (501) staff       (20)     7464 2016-10-18 17:39:34.000000 Flask-Injector-0.8.0/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     5090 2016-10-18 17:33:48.000000 Flask-Injector-0.8.0/README.rst
--rw-r--r--   0 kuba       (501) staff       (20)    11981 2016-10-18 17:37:10.000000 Flask-Injector-0.8.0/flask_injector.py
--rw-r--r--   0 kuba       (501) staff       (20)       82 2016-10-18 17:39:34.000000 Flask-Injector-0.8.0/setup.cfg
--rw-r--r--   0 kuba       (501) staff       (20)     1588 2016-10-18 17:27:13.000000 Flask-Injector-0.8.0/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2017-02-09 14:26:08.000000 Flask-Injector-0.9.0/
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2017-02-09 14:26:08.000000 Flask-Injector-0.9.0/Flask_Injector.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2017-02-09 14:26:08.000000 Flask-Injector-0.9.0/Flask_Injector.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba       (501) staff       (20)     7464 2017-02-09 14:26:08.000000 Flask-Injector-0.9.0/Flask_Injector.egg-info/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)       30 2017-02-09 14:26:08.000000 Flask-Injector-0.9.0/Flask_Injector.egg-info/requires.txt
+-rw-r--r--   0 kuba       (501) staff       (20)      281 2017-02-09 14:26:08.000000 Flask-Injector-0.9.0/Flask_Injector.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       15 2017-02-09 14:26:08.000000 Flask-Injector-0.9.0/Flask_Injector.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2015-05-20 12:24:33.000000 Flask-Injector-0.9.0/Flask_Injector.egg-info/zip-safe
+-rw-r--r--   0 kuba       (501) staff       (20)    12886 2017-02-09 14:25:31.000000 Flask-Injector-0.9.0/flask_injector.py
+-rw-r--r--   0 kuba       (501) staff       (20)       19 2015-05-20 12:02:53.000000 Flask-Injector-0.9.0/MANIFEST.in
+-rw-r--r--   0 kuba       (501) staff       (20)     7464 2017-02-09 14:26:08.000000 Flask-Injector-0.9.0/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     5090 2017-01-23 21:42:36.000000 Flask-Injector-0.9.0/README.rst
+-rw-r--r--   0 kuba       (501) staff       (20)       82 2017-02-09 14:26:08.000000 Flask-Injector-0.9.0/setup.cfg
+-rw-r--r--   0 kuba       (501) staff       (20)     1599 2017-01-23 21:42:36.000000 Flask-Injector-0.9.0/setup.py
```

### Comparing `Flask-Injector-0.8.0/Flask_Injector.egg-info/PKG-INFO` & `Flask-Injector-0.9.0/Flask_Injector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Flask-Injector
-Version: 0.8.0
+Version: 0.9.0
 Summary: Adds Injector, a Dependency Injection framework, support to Flask.
 Home-page: https://github.com/alecthomas/flask_injector
 Author: Alec Thomas
 Author-email: alec@swapoff.org
 License: BSD
 Description: Flask-Injector
         ==============
```

### Comparing `Flask-Injector-0.8.0/PKG-INFO` & `Flask-Injector-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Flask-Injector
-Version: 0.8.0
+Version: 0.9.0
 Summary: Adds Injector, a Dependency Injection framework, support to Flask.
 Home-page: https://github.com/alecthomas/flask_injector
 Author: Alec Thomas
 Author-email: alec@swapoff.org
 License: BSD
 Description: Flask-Injector
         ==============
```

### Comparing `Flask-Injector-0.8.0/README.rst` & `Flask-Injector-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-Injector-0.8.0/flask_injector.py` & `Flask-Injector-0.9.0/flask_injector.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,79 +5,78 @@
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 #
 # Author: Alec Thomas <alec@swapoff.org>
 import functools
+from typing import Any, Callable, cast, Dict, get_type_hints, Iterable, Union
 
 import flask
 try:
     import flask_restplus
 except ImportError:
-    flask_resplus = None
-from injector import Injector, inject
+    flask_restplus = None
+from injector import Binder, Injector, inject
 from flask import Config, Request
 from werkzeug.local import Local, LocalManager, LocalProxy
 from werkzeug.wrappers import Response
 from injector import Module, Provider, Scope, ScopeDecorator, singleton
 
-try:
-    from injector import _infer_injected_bindings
-except ImportError:
-    def _infer_bindings(injector, function):
-        return injector._infer_injected_bindings(function)
-else:
-    def _infer_bindings(injector, function):
-        return _infer_injected_bindings(function)
-
 
 __author__ = 'Alec Thomas <alec@swapoff.org>'
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __all__ = ['request', 'RequestScope', 'Config', 'Request', 'FlaskInjector', ]
 
 
-def wrap_fun(fun, injector):
+def wrap_fun(fun: Callable, injector: Injector) -> Callable:
     if isinstance(fun, LocalProxy):
         return fun
 
     # Important: this block needs to stay here so it's executed *before* the
     # hasattr(fun, '__call__') block below - otherwise things may crash.
     if hasattr(fun, '__bindings__'):
         return wrap_function(fun, injector)
 
     if hasattr(fun, '__call__') and not isinstance(fun, type):
-        bindings_from_annotations = _infer_bindings(injector, fun)
-        if bindings_from_annotations:
-            return wrap_fun(inject(**bindings_from_annotations)(fun), injector)
+        try:
+            type_hints = get_type_hints(fun)
+        except (AttributeError, TypeError):
+            # Some callables aren't introspectable with get_type_hints,
+            # let's assume they don't have anything to inject. The exception
+            # types handled here are what I encountered so far.
+            # It used to be AttributeError, then https://github.com/python/typing/pull/314
+            # changed it to TypeError.
+            wrap_it = False
+        except NameError:
+            wrap_it = True
+        else:
+            type_hints.pop('return', None)
+            wrap_it = type_hints != {}
+        if wrap_it:
+            return wrap_fun(inject(fun), injector)
 
     if hasattr(fun, 'view_class'):
         return wrap_class_based_view(fun, injector)
 
     return fun
 
 
-def wrap_function(fun, injector):
+def wrap_function(fun: Callable, injector: Injector):
     @functools.wraps(fun)
-    def wrapper(*args, **kwargs):
-        injections = injector.args_to_inject(
-            function=fun,
-            bindings=fun.__bindings__,
-            owner_key=fun.__module__,
-        )
-        return fun(*args, **dict(injections, **kwargs))
-
+    def wrapper(*args: Any, **kwargs: Any) -> Any:
+        return injector.call_with_injection(callable=fun, args=args, kwargs=kwargs)
     return wrapper
 
 
-def wrap_class_based_view(fun, injector):
-    cls = fun.view_class
+def wrap_class_based_view(fun: Callable, injector: Injector) -> Callable:
+    cls = cast(Any, fun).view_class
     name = fun.__name__
 
-    closure_contents = (c.cell_contents for c in fun.__closure__)
+    closure_contents = (c.cell_contents for c in cast(Any, fun).__closure__)
     fun_closure = dict(zip(fun.__code__.co_freevars, closure_contents))
     try:
         class_kwargs = fun_closure['class_kwargs']
     except KeyError:
         # Most likely flask_restful resource, we'll see in a second
         flask_restful_api = fun_closure['self']
         # flask_restful wraps ResourceClass.as_view() result in its own wrapper
@@ -120,44 +119,44 @@
         class_kwargs['api'] = flask_restful_api
 
     # This section is flask.views.View.as_view code modified to make the injection
     # possible without relying on modifying view function in place
     # Copyright (c) 2014 by Armin Ronacher and Flask contributors, see Flask
     # license for details
 
-    def view(*args, **kwargs):
+    def view(*args: Any, **kwargs: Any) -> Any:
         self = injector.create_object(cls, additional_kwargs=class_kwargs)
         return self.dispatch_request(*args, **kwargs)
 
     if cls.decorators:
         view.__name__ = name
         view.__module__ = cls.__module__
         for decorator in cls.decorators:
             view = decorator(view)
 
     # We attach the view class to the view function for two reasons:
     # first of all it allows us to easily figure out what class-based
     # view this thing came from, secondly it's also used for instantiating
     # the view class so you can actually replace it with something else
     # for testing purposes and debugging.
-    view.view_class = cls
+    cast(Any, view).view_class = cls
     view.__name__ = name
     view.__doc__ = cls.__doc__
     view.__module__ = cls.__module__
-    view.methods = cls.methods
+    cast(Any, view).methods = cls.methods
 
     fun = view
 
     if flask_restful_api:
         return wrap_flask_restful_resource(fun, flask_restful_api, injector)
 
     return fun
 
 
-def wrap_flask_restful_resource(fun, flask_restful_api, injector):
+def wrap_flask_restful_resource(fun: Callable, flask_restful_api, injector: Injector) -> Callable:
     """
     This is needed because of how flask_restful views are registered originally.
 
     :type flask_restful_api: :class:`flask_restful.Api`
     """
     from flask_restful.utils import unpack
 
@@ -188,32 +187,32 @@
     SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
     CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
     OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
     OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
     """
 
     @functools.wraps(fun)
-    def wrapper(*args, **kwargs):
+    def wrapper(*args: Any, **kwargs: Any) -> Any:
         resp = fun(*args, **kwargs)
         if isinstance(resp, Response):  # There may be a better way to test
             return resp
         data, code, headers = unpack(resp)
         return flask_restful_api.make_response(data, code, headers=headers)
 
     # end of flask_restful code
 
     return wrapper
 
 
 class CachedProviderWrapper(Provider):
-    def __init__(self, old_provider):
+    def __init__(self, old_provider: Provider) -> None:
         self._old_provider = old_provider
-        self._cache = {}
+        self._cache = {}  # type: Dict[int, Any]
 
-    def get(self, injector):
+    def get(self, injector: Injector) -> Any:
         key = id(injector)
         try:
             return self._cache[key]
         except KeyError:
             instance = self._cache[key] = self._old_provider.get(injector)
             return instance
 
@@ -222,45 +221,53 @@
     """A scope whose object lifetime is tied to a request.
 
     @request
     class Session:
         pass
     """
 
-    def cleanup(self):
+    # We don't want to assign here, just provide type hints
+    if False:
+        _local_manager = None  # type: LocalManager
+        _locals = None  # type: Local
+
+    def cleanup(self) -> None:
         self._local_manager.cleanup()
 
-    def prepare(self):
+    def prepare(self) -> None:
         self._locals.scope = {}
 
-    def configure(self):
+    def configure(self) -> None:
         self._locals = Local()
         self._local_manager = LocalManager([self._locals])
         self.prepare()
 
-    def get(self, key, provider):
+    def get(self, key: Any, provider: Provider) -> Any:
         try:
             return self._locals.scope[key]
         except KeyError:
             new_provider = self._locals.scope[key] = CachedProviderWrapper(provider)
             return new_provider
 
 
 request = ScopeDecorator(RequestScope)
 
 
+_ModuleT = Union[Callable[[Binder], Any], Module]
+
+
 class FlaskInjector:
     def __init__(
         self,
-        app,
-        modules=[],
-        injector=None,
-        request_scope_class=RequestScope,
-        use_annotations=None,
-    ):
+        app: flask.Flask,
+        modules: Iterable[_ModuleT] = [],
+        injector: Injector = None,
+        request_scope_class: type = RequestScope,
+        use_annotations: bool = None,
+    ) -> None:
         """Initializes Injector for the application.
 
         .. note::
 
             Needs to be called *after* all views, signal handlers, template globals
             and context processors are registered.
 
@@ -282,57 +289,57 @@
             )
         if not injector:
             kwargs = {}
             if use_annotations is not None:
                 kwargs['use_annotations'] = use_annotations
             injector = Injector(**kwargs)
 
-        for module in (
-                [FlaskModule(app=app, request_scope_class=request_scope_class)] +
-                list(modules)):
+        modules = list(modules)
+        modules.insert(0, FlaskModule(app=app, request_scope_class=request_scope_class))
+        for module in modules:
             injector.binder.install(module)
 
         for container in (
                 app.view_functions,
                 app.before_request_funcs,
                 app.after_request_funcs,
                 app.teardown_request_funcs,
                 app.template_context_processors,
                 app.jinja_env.globals,
                 app.error_handler_spec,
         ):
             process_dict(container, injector)
 
-        def reset_request_scope_before(*args, **kwargs):
+        def reset_request_scope_before(*args: Any, **kwargs: Any) -> None:
             injector.get(request_scope_class).prepare()
 
-        def reset_request_scope_after(*args, **kwargs):
+        def reset_request_scope_after(*args: Any, **kwargs: Any) -> None:
             injector.get(request_scope_class).cleanup()
 
         app.before_request_funcs.setdefault(
             None, []).insert(0, reset_request_scope_before)
         app.teardown_request(reset_request_scope_after)
 
         self.injector = injector
         self.app = app
 
 
-def process_dict(d, injector):
+def process_dict(d: Dict, injector: Injector) -> None:
     for key, value in d.items():
         if isinstance(value, list):
             value[:] = [wrap_fun(fun, injector) for fun in value]
         elif hasattr(value, '__call__'):
             d[key] = wrap_fun(value, injector)
         elif isinstance(value, dict):
             process_dict(value, injector)
 
 
 class FlaskModule(Module):
-    def __init__(self, app, request_scope_class=RequestScope):
+    def __init__(self, app: flask.Flask, request_scope_class: type = RequestScope) -> None:
         self.app = app
         self.request_scope_class = request_scope_class
 
-    def configure(self, binder):
+    def configure(self, binder: Binder) -> None:
         binder.bind_scope(self.request_scope_class)
         binder.bind(flask.Flask, to=self.app, scope=singleton)
         binder.bind(Config, to=self.app.config, scope=singleton)
         binder.bind(Request, to=lambda: flask.request)
```

### Comparing `Flask-Injector-0.8.0/setup.py` & `Flask-Injector-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         author='Alec Thomas',
         author_email='alec@swapoff.org',
         description='Adds Injector, a Dependency Injection framework, support to Flask.',
         long_description=long_description,
         py_modules=['flask_injector'],
         zip_safe=True,
         platforms='any',
-        install_requires=['Flask', 'injector>=0.9.0'],
+        install_requires=['Flask', 'injector>=0.10.0', 'typing'],
         keywords=['Dependency Injection', 'Flask'],
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
             'Topic :: Software Development :: Testing',
```

