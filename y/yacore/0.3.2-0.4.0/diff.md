# Comparing `tmp/yacore-0.3.2.tar.gz` & `tmp/yacore-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yacore-0.3.2.tar", last modified: Wed Jul 26 00:33:04 2023, max compression
+gzip compressed data, was "yacore-0.4.0.tar", last modified: Wed Jul 26 22:31:52 2023, max compression
```

## Comparing `yacore-0.3.2.tar` & `yacore-0.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:33:04.691516 yacore-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 00:32:50.000000 yacore-0.3.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-26 00:32:50.000000 yacore-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-26 00:33:04.691516 yacore-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-26 00:32:50.000000 yacore-0.3.2/history.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 00:32:50.000000 yacore-0.3.2/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-26 00:32:50.000000 yacore-0.3.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-26 00:32:50.000000 yacore-0.3.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 00:33:04.691516 yacore-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-26 00:32:50.000000 yacore-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:33:04.691516 yacore-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-26 00:32:50.000000 yacore-0.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-26 00:32:50.000000 yacore-0.3.2/tests/test_db_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-26 00:32:50.000000 yacore-0.3.2/tests/test_deepmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-26 00:32:50.000000 yacore-0.3.2/tests/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-26 00:32:50.000000 yacore-0.3.2/tests/test_net_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:33:04.691516 yacore-0.3.2/yacore/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:33:04.691516 yacore-0.3.2/yacore/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:33:04.691516 yacore-0.3.2/yacore/db/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/db/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/db/postgresql/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/db/postgresql/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/injector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:33:04.691516 yacore-0.3.2/yacore/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/log/loguru.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/log/stdlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:33:04.691516 yacore-0.3.2/yacore/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:33:04.691516 yacore-0.3.2/yacore/net/http/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/net/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/net/http/server.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 00:32:50.000000 yacore-0.3.2/yacore/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:33:04.691516 yacore-0.3.2/yacore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-26 00:33:04.000000 yacore-0.3.2/yacore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 00:33:04.000000 yacore-0.3.2/yacore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:33:04.000000 yacore-0.3.2/yacore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 00:33:04.000000 yacore-0.3.2/yacore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-26 00:33:04.000000 yacore-0.3.2/yacore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:33:04.000000 yacore-0.3.2/yacore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:52.384920 yacore-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 22:31:37.000000 yacore-0.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-26 22:31:37.000000 yacore-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-26 22:31:52.384920 yacore-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-26 22:31:37.000000 yacore-0.4.0/history.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 22:31:37.000000 yacore-0.4.0/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-26 22:31:37.000000 yacore-0.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-26 22:31:37.000000 yacore-0.4.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:31:52.384920 yacore-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-26 22:31:37.000000 yacore-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:52.376921 yacore-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-26 22:31:37.000000 yacore-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-26 22:31:37.000000 yacore-0.4.0/tests/test_db_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-26 22:31:37.000000 yacore-0.4.0/tests/test_deepmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-26 22:31:37.000000 yacore-0.4.0/tests/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-26 22:31:37.000000 yacore-0.4.0/tests/test_net_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:52.380921 yacore-0.4.0/yacore/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:52.380921 yacore-0.4.0/yacore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:52.380921 yacore-0.4.0/yacore/db/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/db/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/db/postgresql/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/db/postgresql/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/injector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:52.384920 yacore-0.4.0/yacore/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/log/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/log/stdlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:52.384920 yacore-0.4.0/yacore/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:52.384920 yacore-0.4.0/yacore/net/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/net/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/net/http/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 22:31:37.000000 yacore-0.4.0/yacore/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:31:52.380921 yacore-0.4.0/yacore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-26 22:31:52.000000 yacore-0.4.0/yacore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 22:31:52.000000 yacore-0.4.0/yacore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:31:52.000000 yacore-0.4.0/yacore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 22:31:52.000000 yacore-0.4.0/yacore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-26 22:31:52.000000 yacore-0.4.0/yacore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 22:31:52.000000 yacore-0.4.0/yacore.egg-info/top_level.txt
```

### Comparing `yacore-0.3.2/PKG-INFO` & `yacore-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yacore
-Version: 0.3.2
+Version: 0.4.0
 Summary: yet another core library
 Home-page: https://github.com/pohmelie/yacore
 Author: pohmelie
 Author-email: multisosnooley@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yacore-0.3.2/history.md` & `yacore-0.4.0/history.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 0.4.0 (27-07-2023)
+- remove all `is_flag` options, since they conflict with `cock` library getting options from file
+- `net.http.server`: `healthcheck` endpoint is disabled by default
+
 # 0.3.2 (25-07-2023)
 - add default to `is_flag=True` options to allow it in `get_options_defaults` result
 - add option to disable healthcheck endpoint in `net.http.server`
 
 # 0.3.1 (25-07-2023)
 - fix `importlib.resources` deprication warning
```

### Comparing `yacore-0.3.2/license.txt` & `yacore-0.4.0/license.txt`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/readme.md` & `yacore-0.4.0/readme.md`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/setup.py` & `yacore-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/tests/conftest.py` & `yacore-0.4.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         "db_postgresql_pool_min_size": 0,
         "db_postgresql_port": 2345,
         "db_postgresql_user": "user",
         "executors_cpu_threads_count": 1,
         "executors_io_threads_count": 2,
         "log_level": "debug",
         "net_http_build_info": "test-build-info",
+        "net_http_enable_healthcheck": True,
         "net_http_healthcheck_name": "test_name",
         "net_http_hide_methods_description_route": False,
         "net_http_host": "127.0.0.1",
         "net_http_port": unused_tcp_port,
     })
     register(lambda: "version", name="version")
     register(lambda: cfg, name="config")
```

### Comparing `yacore-0.3.2/tests/test_db_postgresql.py` & `yacore-0.4.0/tests/test_db_postgresql.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/tests/test_deepmerge.py` & `yacore-0.4.0/tests/test_deepmerge.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/tests/test_executors.py` & `yacore-0.4.0/tests/test_executors.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/tests/test_net_http.py` & `yacore-0.4.0/tests/test_net_http.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/yacore/db/postgresql/fixtures.py` & `yacore-0.4.0/yacore/db/postgresql/fixtures.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/yacore/db/postgresql/postgresql.py` & `yacore-0.4.0/yacore/db/postgresql/postgresql.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/yacore/executors.py` & `yacore-0.4.0/yacore/executors.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/yacore/log/loguru.py` & `yacore-0.4.0/yacore/log/loguru.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/yacore/log/stdlib.py` & `yacore-0.4.0/yacore/log/stdlib.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/yacore/net/http/client.py` & `yacore-0.4.0/yacore/net/http/client.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.2/yacore/net/http/server.py` & `yacore-0.4.0/yacore/net/http/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 ACCESS_LOG_DEFAULT_FORMAT = '%(h)s %(l)s %(l)s %(t)s "%(r)s" %(s)s %(b)s "%(f)s" "%(a)s"'
 
 net_http_options = build_options_from_dict({
     "net-http": {
         "host": Option(default="0.0.0.0"),
         "port": Option(default=80, type=int),
-        "disable_healthcheck": Option(default=False, is_flag=True),
+        "enable_healthcheck": Option(default=False, type=bool),
         "healthcheck_name": Option(default="noname"),
         "access_log_format": Option(default=ACCESS_LOG_DEFAULT_FORMAT),
-        "hide_methods_description_route": Option(default=False, is_flag=True),
+        "hide_methods_description_route": Option(default=False, type=bool),
         "build_info": Option(default="noinfo"),
     },
 })
 
 
 class HealthCheck(BaseModel):
     ok: bool
@@ -44,20 +44,20 @@
             "data": data,
         },
     )
 
 
 class NetHttpServer(ServiceMixin):
 
-    def __init__(self, host=None, port=80, *, disable_healthcheck=False, healthcheck_name="noname", version="unknown",
+    def __init__(self, host=None, port=80, *, enable_healthcheck=False, healthcheck_name="noname", version="unknown",
                  build_info="noinfo", access_log_format=ACCESS_LOG_DEFAULT_FORMAT,
                  hide_methods_description_route=False):
         self.host = host
         self.port = port
-        self.disable_healthcheck = disable_healthcheck
+        self.enable_healthcheck = enable_healthcheck
         self.healthcheck = HealthCheck(
             ok=True,
             name=healthcheck_name,
             version=version,
             build_info=build_info,
         )
 
@@ -75,15 +75,15 @@
             if self.hide_methods_description_route:
                 self.app = FastAPI(openapi_url=None, docs_url=None, redoc_url=None)
             else:
                 self.app = FastAPI()
         self.app.add_exception_handler(Exception, self.error_handler)
         self.app.add_exception_handler(StarletteHTTPException, self.exception_handler)
         self.app.add_exception_handler(RequestValidationError, self.validation_handler)
-        if not self.disable_healthcheck:
+        if self.enable_healthcheck:
             self.add_get("/healthcheck", self.get_healthcheck)
         self.add_task(serve(
             self.app,
             self.hypercorn_config,
             shutdown_trigger=asyncio.Future,  # no signal handling
         ))
 
@@ -124,14 +124,14 @@
 
 @register(name="net_http_server", singleton=True)
 @inject
 def net_http_server_from_config(config, version):
     return NetHttpServer(
         host=config.net_http_host,
         port=config.net_http_port,
-        disable_healthcheck=config.net_http_disable_healthcheck,
+        enable_healthcheck=config.net_http_enable_healthcheck,
         healthcheck_name=config.net_http_healthcheck_name,
         version=version,
         build_info=config.net_http_build_info,
         access_log_format=config.net_http_access_log_format,
         hide_methods_description_route=config.net_http_hide_methods_description_route,
     )
```

### Comparing `yacore-0.3.2/yacore.egg-info/PKG-INFO` & `yacore-0.4.0/yacore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yacore
-Version: 0.3.2
+Version: 0.4.0
 Summary: yet another core library
 Home-page: https://github.com/pohmelie/yacore
 Author: pohmelie
 Author-email: multisosnooley@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yacore-0.3.2/yacore.egg-info/SOURCES.txt` & `yacore-0.4.0/yacore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

