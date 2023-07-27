# Comparing `tmp/idem-posix-4.0.0.tar.gz` & `tmp/idem-posix-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-posix-4.0.0.tar", last modified: Mon Jul  3 10:50:38 2023, max compression
+gzip compressed data, was "idem-posix-5.0.0.tar", last modified: Thu Jul 27 20:12:03 2023, max compression
```

## Comparing `idem-posix-4.0.0.tar` & `idem-posix-5.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-07-03 10:50:21.000000 idem-posix-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3734 2023-07-03 10:50:38.447766 idem-posix-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2895 2023-07-03 10:50:21.000000 idem-posix-4.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/
--rw-r--r--   0 root         (0) root         (0)      282 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/exec/
--rw-r--r--   0 root         (0) root         (0)     5553 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/exec/cmdmod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/exec/contracts/
--rw-r--r--   0 root         (0) root         (0)     3403 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/exec/contracts/cmdmod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/exec/posix/
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/exec/posix/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/posix/
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/posix/net/
--rw-r--r--   0 root         (0) root         (0)     3866 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/net/dns.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/net/fqdn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/posix/os/
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/os/uname.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/posix/proc/
--rw-r--r--   0 root         (0) root         (0)      246 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/proc/group.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/proc/pid.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/proc/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/grains/posix/system/
--rw-r--r--   0 root         (0) root         (0)      810 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/system/console.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/system/init_system.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/system/locale.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/system/machine_id.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/grains/posix/system/shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/states/
--rw-r--r--   0 root         (0) root         (0)     4938 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/states/cmdmod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix/states/posix/
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-03 10:50:21.000000 idem-posix-4.0.0/idem_posix/states/posix/init.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 10:50:37.000000 idem-posix-4.0.0/idem_posix/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:50:38.447766 idem-posix-4.0.0/idem_posix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3734 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-03 10:50:38.000000 idem-posix-4.0.0/idem_posix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-03 10:50:38.447766 idem-posix-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2712 2023-07-03 10:50:21.000000 idem-posix-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.492761 idem-posix-5.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-07-27 20:11:49.000000 idem-posix-5.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3735 2023-07-27 20:12:03.492761 idem-posix-5.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-07-27 20:11:49.000000 idem-posix-5.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.488761 idem-posix-5.0.0/idem_posix/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.488761 idem-posix-5.0.0/idem_posix/exec/
+-rw-r--r--   0 root         (0) root         (0)     5553 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/exec/cmdmod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.492761 idem-posix-5.0.0/idem_posix/exec/contracts/
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/exec/contracts/cmdmod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.492761 idem-posix-5.0.0/idem_posix/exec/posix/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/exec/posix/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.488761 idem-posix-5.0.0/idem_posix/grains/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.492761 idem-posix-5.0.0/idem_posix/grains/posix/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.492761 idem-posix-5.0.0/idem_posix/grains/posix/net/
+-rw-r--r--   0 root         (0) root         (0)     3866 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/net/dns.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/net/fqdn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.492761 idem-posix-5.0.0/idem_posix/grains/posix/os/
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/os/uname.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.492761 idem-posix-5.0.0/idem_posix/grains/posix/proc/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/proc/group.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/proc/pid.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/proc/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.492761 idem-posix-5.0.0/idem_posix/grains/posix/system/
+-rw-r--r--   0 root         (0) root         (0)      810 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/system/console.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/system/init_system.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/system/locale.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/system/machine_id.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/grains/posix/system/shell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.492761 idem-posix-5.0.0/idem_posix/states/
+-rw-r--r--   0 root         (0) root         (0)     4954 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/states/cmdmod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.492761 idem-posix-5.0.0/idem_posix/states/posix/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-27 20:11:49.000000 idem-posix-5.0.0/idem_posix/states/posix/init.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-27 20:12:02.000000 idem-posix-5.0.0/idem_posix/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:12:03.488761 idem-posix-5.0.0/idem_posix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3735 2023-07-27 20:12:03.000000 idem-posix-5.0.0/idem_posix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-07-27 20:12:03.000000 idem-posix-5.0.0/idem_posix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 20:12:03.000000 idem-posix-5.0.0/idem_posix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-27 20:12:03.000000 idem-posix-5.0.0/idem_posix.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-27 20:12:03.000000 idem-posix-5.0.0/idem_posix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-27 20:12:03.000000 idem-posix-5.0.0/idem_posix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 20:12:03.492761 idem-posix-5.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-07-27 20:11:49.000000 idem-posix-5.0.0/setup.py
```

### Comparing `idem-posix-4.0.0/LICENSE` & `idem-posix-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-posix-4.0.0/PKG-INFO` & `idem-posix-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-posix
-Version: 4.0.0
+Version: 5.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
 Provides-Extra: grains
 License-File: LICENSE
 
 **********
 idem-posix
```

### Comparing `idem-posix-4.0.0/README.rst` & `idem-posix-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem-posix-4.0.0/idem_posix/exec/cmdmod.py` & `idem-posix-5.0.0/idem_posix/exec/cmdmod.py`

 * *Files identical despite different names*

### Comparing `idem-posix-4.0.0/idem_posix/exec/contracts/cmdmod.py` & `idem-posix-5.0.0/idem_posix/exec/contracts/cmdmod.py`

 * *Files identical despite different names*

### Comparing `idem-posix-4.0.0/idem_posix/grains/posix/net/dns.py` & `idem-posix-5.0.0/idem_posix/grains/posix/net/dns.py`

 * *Files identical despite different names*

### Comparing `idem-posix-4.0.0/idem_posix/grains/posix/net/fqdn.py` & `idem-posix-5.0.0/idem_posix/grains/posix/net/fqdn.py`

 * *Files identical despite different names*

### Comparing `idem-posix-4.0.0/idem_posix/grains/posix/system/console.py` & `idem-posix-5.0.0/idem_posix/grains/posix/system/console.py`

 * *Files identical despite different names*

### Comparing `idem-posix-4.0.0/idem_posix/grains/posix/system/init_system.py` & `idem-posix-5.0.0/idem_posix/grains/posix/system/init_system.py`

 * *Files identical despite different names*

### Comparing `idem-posix-4.0.0/idem_posix/grains/posix/system/locale.py` & `idem-posix-5.0.0/idem_posix/grains/posix/system/locale.py`

 * *Files identical despite different names*

### Comparing `idem-posix-4.0.0/idem_posix/states/cmdmod.py` & `idem-posix-5.0.0/idem_posix/states/cmdmod.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,23 +79,23 @@
 
     Example:
         .. code-block:: sls
 
           # Execute "ls -l" command
           my_state_name:
             cmd.run:
-              cmd: ls -l
-              cwd: /
-              shell: False
-              env:
-                ENV_VAR_1: ENV_VAL_1
-                ENV_VAR_2: ENV_VAL_2
-              timeout: 100
-              render_pipe:
-              kwargs:
+              - cmd: ls -l
+              - cwd: /
+              - shell: False
+              - env:
+                 ENV_VAR_1: ENV_VAL_1
+                 ENV_VAR_2: ENV_VAL_2
+              - timeout: 100
+              - render_pipe:
+              - kwargs:
 
         The "new_state" will have the following keys:
 
             "stdout": The plaintext output of the command
 
             "stderr": The plaintext error/logging output of the command
```

### Comparing `idem-posix-4.0.0/idem_posix.egg-info/PKG-INFO` & `idem-posix-5.0.0/idem_posix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-posix
-Version: 4.0.0
+Version: 5.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
 Provides-Extra: grains
 License-File: LICENSE
 
 **********
 idem-posix
```

### Comparing `idem-posix-4.0.0/idem_posix.egg-info/SOURCES.txt` & `idem-posix-5.0.0/idem_posix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-posix-4.0.0/setup.py` & `idem-posix-5.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,25 +70,25 @@
     url="",
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: POSIX",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     entry_points={"console_scripts": [""]},
     cmdclass={"clean": Clean},
 )
```

