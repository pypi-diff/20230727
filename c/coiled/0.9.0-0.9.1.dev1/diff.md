# Comparing `tmp/coiled-0.9.0.tar.gz` & `tmp/coiled-0.9.1.dev1.tar.gz`

## Comparing `coiled-0.9.0.tar` & `coiled-0.9.1.dev1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/analytics.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/auth.py
--rw-r--r--   0        0        0    25197 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/capture_environment.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/context.py
--rw-r--r--   0        0        0   102304 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/exceptions.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/run.py
--rw-r--r--   0        0        0    20053 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/scan.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/shutdown.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/types.py
--rw-r--r--   0        0        0    56396 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/utils.py
--rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/core.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/env.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/prefect.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/utils.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    48728 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/__init__.py
--rw-r--r--   0        0        0    97921 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/cluster.py
--rw-r--r--   0        0        0    59205 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.9.0/.gitignore
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-0.9.0/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.9.0/README.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coiled-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 coiled-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/analytics.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/auth.py
+-rw-r--r--   0        0        0    25197 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/capture_environment.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/context.py
+-rw-r--r--   0        0        0   102304 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/exceptions.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/run.py
+-rw-r--r--   0        0        0    20053 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/scan.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/shutdown.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/types.py
+-rw-r--r--   0        0        0    56396 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/utils.py
+-rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/core.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/utils.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    48728 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    98650 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    59205 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/.gitignore
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/README.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 coiled-0.9.1.dev1/PKG-INFO
```

### Comparing `coiled-0.9.0/coiled/__init__.py` & `coiled-0.9.1.dev1/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/analytics.py` & `coiled-0.9.1.dev1/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/auth.py` & `coiled-0.9.1.dev1/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/capture_environment.py` & `coiled-0.9.1.dev1/coiled/capture_environment.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cluster.py` & `coiled-0.9.1.dev1/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/coiled.yaml` & `coiled-0.9.1.dev1/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/context.py` & `coiled-0.9.1.dev1/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/core.py` & `coiled-0.9.1.dev1/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/exceptions.py` & `coiled-0.9.1.dev1/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/run.py` & `coiled-0.9.1.dev1/coiled/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/scan.py` & `coiled-0.9.1.dev1/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/shutdown.py` & `coiled-0.9.1.dev1/coiled/shutdown.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/software.py` & `coiled-0.9.1.dev1/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/types.py` & `coiled-0.9.1.dev1/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/utils.py` & `coiled-0.9.1.dev1/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/websockets.py` & `coiled-0.9.1.dev1/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/config.py` & `coiled-0.9.1.dev1/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/core.py` & `coiled-0.9.1.dev1/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/curl.py` & `coiled-0.9.1.dev1/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/env.py` & `coiled-0.9.1.dev1/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/login.py` & `coiled-0.9.1.dev1/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/package_sync.py` & `coiled-0.9.1.dev1/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/prefect.py` & `coiled-0.9.1.dev1/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/run.py` & `coiled-0.9.1.dev1/coiled/cli/run.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/utils.py` & `coiled-0.9.1.dev1/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/cluster/__init__.py` & `coiled-0.9.1.dev1/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/cluster/better_logs.py` & `coiled-0.9.1.dev1/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/cluster/logs.py` & `coiled-0.9.1.dev1/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/cluster/metrics.py` & `coiled-0.9.1.dev1/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/cluster/ssh.py` & `coiled-0.9.1.dev1/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/cluster/utils.py` & `coiled-0.9.1.dev1/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/notebook/__init__.py` & `coiled-0.9.1.dev1/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/notebook/notebook.py` & `coiled-0.9.1.dev1/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/setup/__init__.py` & `coiled-0.9.1.dev1/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/setup/amp.py` & `coiled-0.9.1.dev1/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/setup/aws.py` & `coiled-0.9.1.dev1/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/setup/entry.py` & `coiled-0.9.1.dev1/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/setup/gcp.py` & `coiled-0.9.1.dev1/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/cli/setup/prometheus.py` & `coiled-0.9.1.dev1/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/extensions/prefect/runners.py` & `coiled-0.9.1.dev1/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/extensions/prefect/workers.py` & `coiled-0.9.1.dev1/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/v2/__init__.py` & `coiled-0.9.1.dev1/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/v2/cluster.py` & `coiled-0.9.1.dev1/coiled/v2/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 )
 from .cwi_log_link import cloudwatch_url
 from .states import (
     ClusterStateEnum,
     InstanceStateEnum,
     ProcessStateEnum,
     flatten_log_states,
+    group_worker_errors,
     log_states,
     summarize_status,
 )
 from .widgets import EXECUTION_CONTEXT, HAS_RICH
 from .widgets.rich import CONSOLE_WIDTH
 from .widgets.util import simple_progress
 
@@ -1443,20 +1444,34 @@
                             reason_not_ready,
                             cluster_id=self.cluster_id,
                         )
                     elif (starting_workers + n_workers_ready) < num_workers_to_wait_for:
                         # including workers that are starting, cluster cannot get to the number
                         # of desired ready workers (because some workers have already errored),
                         logger.debug(summarize_status(cluster_details))
+
+                        message = (
+                            f"Cluster was waiting for {num_workers_to_wait_for} workers but "
+                            f"{self.errored_worker_count} (of {self._start_n_workers}) workers have already failed. "
+                            "You could try requesting fewer workers or adjust `wait_for_workers` if fewer workers "
+                            "would be acceptable."
+                        )
+                        errors = group_worker_errors(cluster_details)
+                        if errors:
+                            header = "Failure Reasons\n" "---------------"
+                            message = f"{message}\n\n{header}"
+                            # show error that affected the most workers first
+                            for error in sorted(errors, key=lambda k: -errors[k]):
+                                n_affected = errors[error]
+                                plural = "" if n_affected == 1 else "s"
+                                error_message = f"{error}\n\t(error affected {n_affected} worker{plural})"
+                                message = f"{message}\n\n{error_message}"
+
                         raise ClusterCreationError(
-                            f"The Cluster was waiting for {num_workers_to_wait_for} workers."
-                            f"Because {self.errored_worker_count} workers have already failed, "
-                            "this cluster cannot get to the desired number of workers. "
-                            f"({n_workers_ready} are ready and {starting_workers} are still starting). "
-                            "Try adjusting the wait_for_workers argument if fewer workers is acceptable.",
+                            message,
                             cluster_id=self.cluster_id,
                         )
                     elif timeout_at is not None and datetime.datetime.now() > timeout_at:
                         error = "User-specified timeout expired: " + reason_not_ready
                         if widget:
                             widget.update(
                                 cluster_details,
```

### Comparing `coiled-0.9.0/coiled/v2/core.py` & `coiled-0.9.1.dev1/coiled/v2/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/v2/cwi_log_link.py` & `coiled-0.9.1.dev1/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/v2/states.py` & `coiled-0.9.1.dev1/coiled/v2/states.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from collections import Counter
 from datetime import datetime
 from enum import Enum
-from typing import List, NamedTuple, Optional, Tuple
+from typing import Dict, List, NamedTuple, Optional, Tuple
 
 from coiled.utils import COILED_LOGGER_NAME
 
 logger = logging.getLogger(COILED_LOGGER_NAME)
 
 DISPLAY_DATETIME_FORMAT = "%H:%M:%S (%Z)"
 
@@ -235,7 +235,20 @@
         worker_statuses_to_show = (
             f"Workers: {', '.join(worker_status_descriptions)} " f"(of {sum(worker_state_counts.values())})"
         )
         return (
             f"{scheduler_status_to_show:{max_description_length + len('Scheduler: ') + 3}} "
             f"{worker_statuses_to_show}"
         )
+
+
+def group_worker_errors(details: dict) -> Dict[str, int]:
+    reasons = {}
+    for worker in details.get("workers", []):
+        state = worker.get("current_state", {}).get("state")
+        reason = worker.get("current_state", {}).get("reason")
+        if state == "error" and reason:
+            if reason not in reasons:
+                reasons[reason] = 1
+            else:
+                reasons[reason] += 1
+    return reasons
```

### Comparing `coiled-0.9.0/coiled/v2/widgets/__init__.py` & `coiled-0.9.1.dev1/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/v2/widgets/rich.py` & `coiled-0.9.1.dev1/coiled/v2/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/coiled/v2/widgets/util.py` & `coiled-0.9.1.dev1/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/README.md` & `coiled-0.9.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/pyproject.toml` & `coiled-0.9.1.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.9.0/PKG-INFO` & `coiled-0.9.1.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.9.0
+Version: 0.9.1.dev1
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.9.0 Project-URL: Homepage, https:
-//coiled.io Maintainer-email: Coiled
+Metadata-Version: 2.1 Name: coiled Version: 0.9.1.dev1 Project-URL: Homepage,
+https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: gilknocker>=0.4.1 Requires-Dist: importlib-metadata Requires-
 Dist: ipywidgets Requires-Dist: jmespath Requires-Dist: jsondiff Requires-Dist:
 packaging Requires-Dist: pip Requires-Dist: pip>=19.3 Requires-Dist:
 prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist: setuptools>=49.3.0
```

