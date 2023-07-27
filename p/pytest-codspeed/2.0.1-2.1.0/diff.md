# Comparing `tmp/pytest_codspeed-2.0.1.tar.gz` & `tmp/pytest_codspeed-2.1.0.tar.gz`

## Comparing `pytest_codspeed-2.0.1.tar` & `pytest_codspeed-2.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/__init__.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/plugin.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/.gitignore
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/__init__.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/wrapper.c
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/wrapper.h
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/wrapper.pyi
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/LICENSE
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/README.md
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 pytest_codspeed-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/src/pytest_codspeed/__init__.py
+-rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/src/pytest_codspeed/plugin.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/src/pytest_codspeed/utils.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/src/pytest_codspeed/_wrapper/.gitignore
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/src/pytest_codspeed/_wrapper/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/src/pytest_codspeed/_wrapper/wrapper.c
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/src/pytest_codspeed/_wrapper/wrapper.h
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/src/pytest_codspeed/_wrapper/wrapper.pyi
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/README.md
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 pytest_codspeed-2.1.0/PKG-INFO
```

### Comparing `pytest_codspeed-2.0.1/src/pytest_codspeed/plugin.py` & `pytest_codspeed-2.1.0/src/pytest_codspeed/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     TypeVar,
     Union,
 )
 
 import pytest
 from _pytest.fixtures import FixtureManager
 
+from pytest_codspeed.utils import get_git_relative_uri
+
 from . import __version__
 from ._wrapper import get_lib
 
 if TYPE_CHECKING:
     from ._wrapper import LibType
 
 IS_PYTEST_BENCHMARK_INSTALLED = pkgutil.find_loader("pytest_benchmark") is not None
@@ -165,15 +167,20 @@
             else:
                 deselected.append(item)
         config.hook.pytest_deselected(items=deselected)
         items[:] = selected
 
 
 def _run_with_instrumentation(
-    lib: "LibType", nodeId: str, fn: Callable[..., Any], *args, **kwargs
+    lib: "LibType",
+    nodeId: str,
+    config: "pytest.Config",
+    fn: Callable[..., Any],
+    *args,
+    **kwargs,
 ):
     is_gc_enabled = gc.isenabled()
     if is_gc_enabled:
         gc.collect()
         gc.disable()
 
     result = None
@@ -181,20 +188,20 @@
     def __codspeed_root_frame__():
         nonlocal result
         result = fn(*args, **kwargs)
 
     if SUPPORTS_PERF_TRAMPOLINE:
         # Warmup CPython performance map cache
         __codspeed_root_frame__()
-
     lib.zero_stats()
     lib.start_instrumentation()
     __codspeed_root_frame__()
     lib.stop_instrumentation()
-    lib.dump_stats_at(f"{nodeId}".encode("ascii"))
+    uri = get_git_relative_uri(nodeId, config.rootpath)
+    lib.dump_stats_at(uri.encode("ascii"))
     if is_gc_enabled:
         gc.enable()
 
     return result
 
 
 @pytest.hookimpl(tryfirst=True)
@@ -222,15 +229,17 @@
     setup_report = ihook.pytest_runtest_makereport(item=item, call=setup_call)
     ihook.pytest_runtest_logreport(report=setup_report)
     reports.append(setup_report)
     # Run phase
     if setup_report.passed and not item.config.getoption("setuponly"):
         assert plugin.lib is not None
         runtest_call = pytest.CallInfo.from_call(
-            lambda: _run_with_instrumentation(plugin.lib, item.nodeid, item.runtest),
+            lambda: _run_with_instrumentation(
+                plugin.lib, item.nodeid, item.config, item.runtest
+            ),
             "call",
         )
         runtest_report = ihook.pytest_runtest_makereport(item=item, call=runtest_call)
         ihook.pytest_runtest_logreport(report=runtest_report)
         reports.append(runtest_report)
 
     # Teardown phase
@@ -253,20 +262,21 @@
 
     def __init__(self, request: "pytest.FixtureRequest"):
         self.extra_info: Dict = {}
 
         self._request = request
 
     def __call__(self, func: Callable[..., T], *args: Any, **kwargs: Any) -> T:
-        plugin = get_plugin(self._request.config)
+        config = self._request.config
+        plugin = get_plugin(config)
         plugin.benchmark_count += 1
         if plugin.is_codspeed_enabled and plugin.should_measure:
             assert plugin.lib is not None
             return _run_with_instrumentation(
-                plugin.lib, self._request.node.nodeid, func, *args, **kwargs
+                plugin.lib, self._request.node.nodeid, config, func, *args, **kwargs
             )
         else:
             return func(*args, **kwargs)
 
 
 @pytest.fixture(scope="function")
 def codspeed_benchmark(request: "pytest.FixtureRequest") -> Callable:
```

### Comparing `pytest_codspeed-2.0.1/src/pytest_codspeed/_wrapper/__init__.py` & `pytest_codspeed-2.1.0/src/pytest_codspeed/_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-2.0.1/.gitignore` & `pytest_codspeed-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-2.0.1/LICENSE` & `pytest_codspeed-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-2.0.1/README.md` & `pytest_codspeed-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-2.0.1/pyproject.toml` & `pytest_codspeed-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_codspeed-2.0.1/PKG-INFO` & `pytest_codspeed-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-codspeed
-Version: 2.0.1
+Version: 2.1.0
 Summary: Pytest plugin to create CodSpeed benchmarks
 Project-URL: Homepage, https://codspeed.io/
 Project-URL: Documentation, https://docs.codspeed.io/
 Project-URL: Source, https://github.com/CodSpeedHQ/pytest-codspeed
 Author-email: Arthur Pastel <arthur@codspeed.io>
 License: The MIT License (MIT)
```

