# Comparing `tmp/SocksDriver-1.0.tar.gz` & `tmp/SocksDriver-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SocksDriver-1.0.tar", last modified: Wed Jul 26 00:43:55 2023, max compression
+gzip compressed data, was "SocksDriver-1.1.tar", last modified: Thu Jul 27 06:35:01 2023, max compression
```

## Comparing `SocksDriver-1.0.tar` & `SocksDriver-1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-26 00:43:55.960780 SocksDriver-1.0/
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1068 2023-07-25 21:34:45.000000 SocksDriver-1.0/LICENSE
--rw-r--r--   0 dsw       (1000) dsw       (1000)      418 2023-07-26 00:43:55.959783 SocksDriver-1.0/PKG-INFO
--rw-r--r--   0 dsw       (1000) dsw       (1000)       59 2023-07-25 22:54:56.000000 SocksDriver-1.0/README.md
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-26 00:43:55.935853 SocksDriver-1.0/SocksDriver/
--rw-r--r--   0 dsw       (1000) dsw       (1000)       43 2023-07-23 10:49:49.000000 SocksDriver-1.0/SocksDriver/__init__.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     7703 2023-07-25 07:33:41.000000 SocksDriver-1.0/SocksDriver/client.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      483 2023-07-24 10:07:13.000000 SocksDriver-1.0/SocksDriver/complex_types.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      249 2023-07-24 07:59:31.000000 SocksDriver-1.0/SocksDriver/errors.py
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-26 00:43:55.945825 SocksDriver-1.0/SocksDriver.egg-info/
--rw-r--r--   0 dsw       (1000) dsw       (1000)      418 2023-07-26 00:43:55.000000 SocksDriver-1.0/SocksDriver.egg-info/PKG-INFO
--rw-r--r--   0 dsw       (1000) dsw       (1000)      529 2023-07-26 00:43:55.000000 SocksDriver-1.0/SocksDriver.egg-info/SOURCES.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)        1 2023-07-26 00:43:55.000000 SocksDriver-1.0/SocksDriver.egg-info/dependency_links.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)       12 2023-07-26 00:43:55.000000 SocksDriver-1.0/SocksDriver.egg-info/top_level.txt
--rw-r--r--   0 dsw       (1000) dsw       (1000)      425 2023-07-25 22:54:56.000000 SocksDriver-1.0/pyproject.toml
--rw-r--r--   0 dsw       (1000) dsw       (1000)       38 2023-07-26 00:43:55.960780 SocksDriver-1.0/setup.cfg
-drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-26 00:43:55.958430 SocksDriver-1.0/tests/
--rw-r--r--   0 dsw       (1000) dsw       (1000)     2090 2023-07-24 09:58:57.000000 SocksDriver-1.0/tests/test_command_blockdev.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      699 2023-07-24 08:21:34.000000 SocksDriver-1.0/tests/test_command_help.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      329 2023-07-25 07:34:53.000000 SocksDriver-1.0/tests/test_command_meminfo.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      290 2023-07-24 09:12:37.000000 SocksDriver-1.0/tests/test_command_sleep.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      469 2023-07-24 09:12:17.000000 SocksDriver-1.0/tests/test_command_sysinfo.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      564 2023-07-24 09:11:50.000000 SocksDriver-1.0/tests/test_command_uptime.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)      514 2023-07-25 06:00:12.000000 SocksDriver-1.0/tests/test_connect_disconnect.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     1381 2023-07-25 04:53:01.000000 SocksDriver-1.0/tests/test_error_handling.py
--rw-r--r--   0 dsw       (1000) dsw       (1000)     2732 2023-07-23 12:30:43.000000 SocksDriver-1.0/tests/test_protocol.py
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-27 06:35:01.061635 SocksDriver-1.1/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1068 2023-07-25 21:34:45.000000 SocksDriver-1.1/LICENSE
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      419 2023-07-27 06:35:01.060637 SocksDriver-1.1/PKG-INFO
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       60 2023-07-27 06:33:28.000000 SocksDriver-1.1/README.md
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-27 06:35:01.036701 SocksDriver-1.1/SocksDriver/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       43 2023-07-23 10:49:49.000000 SocksDriver-1.1/SocksDriver/__init__.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     8403 2023-07-27 06:33:28.000000 SocksDriver-1.1/SocksDriver/client.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      483 2023-07-24 10:07:13.000000 SocksDriver-1.1/SocksDriver/complex_types.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      249 2023-07-24 07:59:31.000000 SocksDriver-1.1/SocksDriver/errors.py
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-27 06:35:01.044680 SocksDriver-1.1/SocksDriver.egg-info/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      419 2023-07-27 06:35:01.000000 SocksDriver-1.1/SocksDriver.egg-info/PKG-INFO
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      559 2023-07-27 06:35:01.000000 SocksDriver-1.1/SocksDriver.egg-info/SOURCES.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)        1 2023-07-27 06:35:01.000000 SocksDriver-1.1/SocksDriver.egg-info/dependency_links.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       12 2023-07-27 06:35:01.000000 SocksDriver-1.1/SocksDriver.egg-info/top_level.txt
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      425 2023-07-27 06:33:28.000000 SocksDriver-1.1/pyproject.toml
+-rw-r--r--   0 dsw       (1000) dsw       (1000)       38 2023-07-27 06:35:01.061635 SocksDriver-1.1/setup.cfg
+drwxr-xr-x   0 dsw       (1000) dsw       (1000)        0 2023-07-27 06:35:01.059639 SocksDriver-1.1/tests/
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     2090 2023-07-24 09:58:57.000000 SocksDriver-1.1/tests/test_command_blockdev.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      703 2023-07-27 06:33:28.000000 SocksDriver-1.1/tests/test_command_help.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      329 2023-07-25 07:34:53.000000 SocksDriver-1.1/tests/test_command_meminfo.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      290 2023-07-24 09:12:37.000000 SocksDriver-1.1/tests/test_command_sleep.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      469 2023-07-24 09:12:17.000000 SocksDriver-1.1/tests/test_command_sysinfo.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      564 2023-07-24 09:11:50.000000 SocksDriver-1.1/tests/test_command_uptime.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      231 2023-07-27 06:33:28.000000 SocksDriver-1.1/tests/test_command_version.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)      514 2023-07-25 06:00:12.000000 SocksDriver-1.1/tests/test_connect_disconnect.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     1381 2023-07-25 04:53:01.000000 SocksDriver-1.1/tests/test_error_handling.py
+-rw-r--r--   0 dsw       (1000) dsw       (1000)     2732 2023-07-23 12:30:43.000000 SocksDriver-1.1/tests/test_protocol.py
```

### Comparing `SocksDriver-1.0/LICENSE` & `SocksDriver-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.0/SocksDriver/client.py` & `SocksDriver-1.1/SocksDriver/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,7 +233,30 @@
         if results['status'] != 'Success':
             raise SocksInternalServerError(results['status'])
 
         del results['status']
 
         results['totalram'] = int(results['totalram'])
         return results
+
+    def version(self) -> dict[str, str]:
+
+        """Ask peer to return the ChristmasSocks server version.
+
+        :return dict[str, str]
+        :raise: SocksTransmissionError if round-trip transmission failed.
+        :raise: SocksInternalServerError if server returns an error.
+        """
+
+        results_s = self.send('version')
+
+        try:
+            results = loads(results_s)
+        except JSONDecodeError as exc:
+            raise SocksTransmissionError('Could not decode data. Buffer size is possibly too small') from exc
+
+        if results['status'] != 'Success':
+            raise SocksInternalServerError(results['status'])
+
+        del results['status']
+
+        return results
```

### Comparing `SocksDriver-1.0/SocksDriver.egg-info/SOURCES.txt` & `SocksDriver-1.1/SocksDriver.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 SocksDriver.egg-info/top_level.txt
 tests/test_command_blockdev.py
 tests/test_command_help.py
 tests/test_command_meminfo.py
 tests/test_command_sleep.py
 tests/test_command_sysinfo.py
 tests/test_command_uptime.py
+tests/test_command_version.py
 tests/test_connect_disconnect.py
 tests/test_error_handling.py
 tests/test_protocol.py
```

### Comparing `SocksDriver-1.0/tests/test_command_blockdev.py` & `SocksDriver-1.1/tests/test_command_blockdev.py`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.0/tests/test_command_help.py` & `SocksDriver-1.1/tests/test_command_help.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def test_command_help(client: SocksClient) -> None:
 
     results = client.help()
 
     assert len(results) == 8
 
-    assert results['host'] == gethostname()
     assert results['blockdev'] == 'Return information about block devices on host'
-    assert results['exit'] == 'Shut down the server'
     assert results['help'] == 'Get a list of commands'
+    assert results['host'] == gethostname()
     assert results['meminfo'] == 'Return host memory statistics'
     assert results['sleep'] == 'Sleep for a short delay'
     assert results['sysinfo'] == 'Return information about the host operating system'
     assert results['uptime'] == 'Return time since boot in HH:MM:SS format'
+    assert results['version'] == 'Return binary version'
```

### Comparing `SocksDriver-1.0/tests/test_command_uptime.py` & `SocksDriver-1.1/tests/test_command_uptime.py`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.0/tests/test_connect_disconnect.py` & `SocksDriver-1.1/tests/test_connect_disconnect.py`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.0/tests/test_error_handling.py` & `SocksDriver-1.1/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `SocksDriver-1.0/tests/test_protocol.py` & `SocksDriver-1.1/tests/test_protocol.py`

 * *Files identical despite different names*

