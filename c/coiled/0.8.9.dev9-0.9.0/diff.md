# Comparing `tmp/coiled-0.8.9.dev9.tar.gz` & `tmp/coiled-0.9.0.tar.gz`

## Comparing `coiled-0.8.9.dev9.tar` & `coiled-0.9.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/_version.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/analytics.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/auth.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/compatibility.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/context.py
--rw-r--r--   0        0        0   102271 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/exceptions.py
--rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/magic.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/run.py
--rw-r--r--   0        0        0    20044 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/scan.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/shutdown.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/software.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/types.py
--rw-r--r--   0        0        0    55355 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/config.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/env.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/login.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/prefect.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/run.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    46135 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/cli/setup/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/extensions/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/extensions/prefect/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/extensions/prefect/runners.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/extensions/prefect/workers.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/__init__.py
--rw-r--r--   0        0        0    94043 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/cluster.py
--rw-r--r--   0        0        0    59085 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/cwi_log_link.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/states.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/coiled/v2/widgets/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.8.9.dev9/PKG-INFO
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/_version.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/analytics.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/auth.py
+-rw-r--r--   0        0        0    25197 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/capture_environment.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/compatibility.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/context.py
+-rw-r--r--   0        0        0   102304 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/exceptions.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/run.py
+-rw-r--r--   0        0        0    20053 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/scan.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/shutdown.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/software.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/types.py
+-rw-r--r--   0        0        0    56396 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/utils.py
+-rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/config.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/core.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/env.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/login.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/prefect.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/run.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/utils.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    48728 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26906 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/extensions/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/extensions/prefect/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/extensions/prefect/runners.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/extensions/prefect/workers.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/__init__.py
+-rw-r--r--   0        0        0    97921 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/cluster.py
+-rw-r--r--   0        0        0    59205 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/cwi_log_link.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/states.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/widgets/__init__.py
+-rw-r--r--   0        0        0    16304 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.9.0/coiled/v2/widgets/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.9.0/.gitignore
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 coiled-0.9.0/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.9.0/README.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 coiled-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 coiled-0.9.0/PKG-INFO
```

### Comparing `coiled-0.8.9.dev9/coiled/__init__.py` & `coiled-0.9.0/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/analytics.py` & `coiled-0.9.0/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/auth.py` & `coiled-0.9.0/coiled/auth.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cluster.py` & `coiled-0.9.0/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/coiled.yaml` & `coiled-0.9.0/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/context.py` & `coiled-0.9.0/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/core.py` & `coiled-0.9.0/coiled/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 
 
 class AWSSessionCredentials(TypedDict):
     AccessKeyId: str
     SecretAccessKey: str
     SessionToken: Optional[str]
     Expiration: Optional[datetime.datetime]
+    DefaultRegion: Optional[str]
 
 
 def delete_docstring(func):
     delete_doc = """ Delete a {kind}
 
 Parameters
 ---------
```

### Comparing `coiled-0.8.9.dev9/coiled/exceptions.py` & `coiled-0.9.0/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/magic.py` & `coiled-0.9.0/coiled/capture_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         outdir = Path(tmpdir.name) / Path(pkg_name)
         if outdir.exists():
             logger.debug(f"Checking for existing wheel for {pkg_name} @ {outdir}")
             wheel_fn = next((file for file in outdir.iterdir() if file.suffix == ".whl"), None)
         else:
             wheel_fn = None
         if not wheel_fn:
-            logger.info(f"No existing wheel, creating a wheel for {pkg_name} @ {src}")
+            logger.debug(f"No existing wheel, creating a wheel for {pkg_name} @ {src}")
             # must use executable to avoid using some other random python
             p = await create_subprocess_shell(
                 cmd=f"{executable} -m pip wheel --wheel-dir {outdir} --no-deps --use-pep517 --no-cache-dir {src}",
                 stderr=subprocess.STDOUT,
                 stdout=subprocess.PIPE,
             )
             if p.returncode:
@@ -132,15 +132,15 @@
                         " package, will not be included in environment, check stdout for the build log"
                     ),
                     "note": None,
                     "sdist": None,
                     "md5": None,
                 }
             wheel_fn = next(file for file in outdir.iterdir() if file.suffix == ".whl")
-        logger.info(f"Using wheel @ {wheel_fn}")
+        logger.debug(f"Using wheel @ {wheel_fn}")
         _, build_version, _, _ = parse_wheel_filename(str(wheel_fn.name))
         has_python, md5, missing_py_files = await validate_wheel(wheel_fn, src)
     return {
         "name": pkg_name,
         "source": "pip",
         "channel": None,
         "conda_name": None,
@@ -158,15 +158,15 @@
 
 
 @track_context
 async def create_wheel_from_egg(pkg_name: str, version: str, src: str) -> ResolvedPackageInfo:
     tmpdir = TemporaryDirectory()
     outdir = Path(tmpdir.name) / Path(pkg_name)
     outdir.mkdir(parents=True)
-    logger.info(f"Attempting to create a wheel for {pkg_name} in directory {src}")
+    logger.debug(f"Attempting to create a wheel for {pkg_name} in directory {src}")
     # must use executable to avoid using some other random python
     p = await create_subprocess_shell(
         cmd=f"{executable} -m wheel convert --dest-dir {outdir} {src}",
         stderr=subprocess.STDOUT,
         stdout=subprocess.PIPE,
     )
     if p.returncode:
@@ -226,15 +226,15 @@
         outdir = Path(tmpdir.name) / Path(pkg_name)
         if outdir.exists():
             logger.debug(f"Checking for existing source archive for {pkg_name} @ {outdir}")
             wheel_fn = next((file for file in outdir.iterdir() if file.suffix == ".whl"), None)
         else:
             wheel_fn = None
         if not wheel_fn:
-            logger.info(f"No existing source archive, creating an archive for {pkg_name} @ {src}")
+            logger.debug(f"No existing source archive, creating an archive for {pkg_name} @ {src}")
             try:
                 unpacked_dir = outdir / f"{pkg_name}-{version}"
                 # Create fake metadata to make wheel work
                 dist_info_dir = unpacked_dir / f"{unpacked_dir.name}.dist-info"
                 dist_info_dir.mkdir(parents=True)
                 with open(dist_info_dir / "METADATA", "w") as f:
                     f.write(f"Metadata-Version: 2.1\nName: {pkg_name}\nVersion: {version}\n")
@@ -283,15 +283,15 @@
                     "include": False,
                     "error": f"Failed to build a package of your local python files. Exception: {e}",
                     "note": None,
                     "sdist": None,
                     "md5": None,
                 }
             wheel_fn = next(file for file in outdir.iterdir() if file.suffix == ".whl")
-        logger.info(f"Using wheel @ {wheel_fn}")
+        logger.debug(f"Using wheel @ {wheel_fn}")
         _, build_version, _, _ = parse_wheel_filename(str(wheel_fn.name))
         has_python, md5, missing_py_files = await validate_wheel(wheel_fn, src)
     return {
         "name": pkg_name,
         "source": "pip",
         "channel": None,
         "conda_name": None,
```

### Comparing `coiled-0.8.9.dev9/coiled/scan.py` & `coiled-0.9.0/coiled/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import hashlib
 import json
 import os
 import platform
+import re
 import sys
 import typing
 from base64 import urlsafe_b64encode
 from collections import defaultdict
 from logging import getLogger
 from pathlib import Path
 from typing import Dict, List, Optional, Union, cast
@@ -449,15 +450,15 @@
     extra_paths = {p.resolve() for p in locations if prefix not in p.parents} - pkg_paths
     for extra_path in extra_paths:
         if not extra_path.is_dir():
             continue
         if any(recurse_importable_python_files(extra_path)):
             results.append(
                 {
-                    "name": f"{COILED_LOCAL_PACKAGE_PREFIX}{extra_path.name.replace('-', '_')}",
+                    "name": COILED_LOCAL_PACKAGE_PREFIX + re.sub(r"\W+", "_", extra_path.name),
                     "path": extra_path,
                     "source": "pip",
                     "version": "0.0.0",
                     "channel_url": None,
                     "channel": None,
                     "subdir": None,
                     "conda_name": None,
```

### Comparing `coiled-0.8.9.dev9/coiled/shutdown.py` & `coiled-0.9.0/coiled/shutdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import logging
 import time
 
 from dask.utils import parse_timedelta
 from distributed import SchedulerPlugin
-from distributed.compatibility import PeriodicCallback  # pyright: reportPrivateImportUsage=false
+
+try:
+    from distributed.compatibility import PeriodicCallback  # pyright: reportPrivateImportUsage=false
+except ImportError:
+    # For `distributed<2022.10.1` (xref https://github.com/dask/distributed/pull/7165)
+    from tornado.ioloop import PeriodicCallback
 
 logger = logging.getLogger("distributed.scheduler")
 
 
 class NoClientShutdown(SchedulerPlugin):
     """Shut down a scheduler if all of the clients have gone"""
```

### Comparing `coiled-0.8.9.dev9/coiled/software.py` & `coiled-0.9.0/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/types.py` & `coiled-0.9.0/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/utils.py` & `coiled-0.9.0/coiled/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1378,36 +1378,61 @@
     if http:
         ports.append(80)
     if https:
         ports.append(443)
     return {"ingress": [{"ports": ports, "cidr": cidr}]}
 
 
-def is_legal_module_file(fpath: Path):
-    return not any([part for part in fpath.parts if contains_invalid_import_characters(part)])
-
-
-def contains_invalid_import_characters(s: str):
-    return any(char in s for char in [".", "-", " "])
-
-
 def is_legal_python_filename(filename: str):
-    return filename.endswith(".py") and not contains_invalid_import_characters(filename[:-3])
+    return filename.endswith(".py") and filename[:-3].isidentifier()
 
 
 def recurse_importable_python_files(src: Path):
+    skip_dirs = set()
+    if platform.system() == "Darwin":
+        skip_dirs = {
+            (Path.home() / "Applications").resolve(),
+            (Path.home() / "Desktop").resolve(),
+            (Path.home() / "Documents").resolve(),
+            (Path.home() / "Downloads").resolve(),
+            (Path.home() / "Library").resolve(),
+            (Path.home() / "Movies").resolve(),
+            (Path.home() / "Music").resolve(),
+            (Path.home() / "Pictures").resolve(),
+            (Path.home() / "Public").resolve(),
+        }
+    dir_has_py = {}
+    dot_path = Path(".")
     for root, dirs, files in os.walk(src, topdown=True):
         root_path = Path(root)
-        for d in [d for d in dirs if not is_legal_module_file((root_path / d).relative_to(src))]:
-            # pruning inplace like this works as long as topdown=True
-            dirs.remove(d)
-        for file in [f for f in files if is_legal_python_filename(f)]:
-            fpath = root_path / file
-            rel_file = fpath.relative_to(src)
-            yield rel_file
+        rel_root = root_path.relative_to(src)
+        has_py = False
+        # Don't need .get because we always iterate through parents before
+        # children, and the only case where there isn't a parent is when
+        # rel_root == dot_path.
+        parent_has_py = rel_root == dot_path or dir_has_py[rel_root.parent]
+
+        for file in files:
+            if is_legal_python_filename(file):
+                has_py = True
+                yield rel_root / file
+
+        dir_has_py[rel_root] = has_py
+        for d in dirs[:]:
+            if (
+                not d.isidentifier()
+                or (root_path / d).resolve() in skip_dirs
+                # Let's assume we can stop looking if there are no Python files
+                # three levels deep.
+                # For example, ./a/b/c/module.py would only be yielded if
+                # there's a .py file in ./a/ or ./a/b/.
+                or (not has_py and not parent_has_py and rel_root.parent != dot_path)
+            ):
+                # pruning inplace like this works as long as topdown=True
+                dirs.remove(d)
 
 
 async def validate_wheel(wheel: Path, src: str) -> Tuple[bool, str, Set[str]]:
     """
     Validate a wheel contains some python files and return the md5
 
     Also, warn if there are Python files in src directory that are not
```

### Comparing `coiled-0.8.9.dev9/coiled/websockets.py` & `coiled-0.9.0/coiled/websockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     async def on_message(self, message_data: Dict) -> None:
         # This could be there as a None value
         data = message_data.get("data") or {}
         # Ignore notifications that are unrelated to this context
         if not data.get("coiled-operation-id", "") == COILED_OP_CONTEXT.get(""):
             return
         message_data = message_data["message"]
-        print(message_data, file=self.log_output)
+        print("   ", message_data, file=self.log_output)
 
     async def on_error(self, error: WSMessage) -> None:
         print(
             f"Error with connection to notifications endpoint: {error}",
             file=self.log_output,
         )
 
@@ -218,8 +218,8 @@
             await self.close()
             return
         elif message in ["CONFIGURING_BACKEND", "NOT_CONFIGURING_BACKEND"]:
             # These are messages used by the web UI, we can ignore
             # them here.
             return
 
-        print(message, file=self.log_output)
+        print("  ", message, file=self.log_output)
```

### Comparing `coiled-0.8.9.dev9/coiled/cli/config.py` & `coiled-0.9.0/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/core.py` & `coiled-0.9.0/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/curl.py` & `coiled-0.9.0/coiled/cli/curl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from json import loads as json_loads
+
 import click
 from rich import print
 
 import coiled
 
 from .utils import CONTEXT_SETTINGS
 
@@ -10,35 +12,37 @@
     context_settings=CONTEXT_SETTINGS,
     help="CLI to hit endpoints using Coiled account authentication (mostly for internal use)",
 )
 @click.argument("url")
 @click.option("-X", "--request", default="GET")
 @click.option("-d", "--data", multiple=True)
 @click.option("--json", is_flag=True, default=False)
-def curl(url: str, request, data, json):
+@click.option("--json-output", is_flag=True, default=False, help="Set to pretty print JSON responses")
+def curl(url: str, request, data, json, json_output):
     all_data = "&".join(data) if data else None
     with coiled.Cloud() as cloud:
         if "http" not in url:
             url = f"{cloud.server}{url}"
 
-        response = sync_request(cloud, url, method=request, data=all_data, json=json)
+        response = sync_request(cloud, url, method=request, data=all_data, json=json, json_output=json_output)
 
     print(response)
 
 
-def sync_request(cloud, url, method, data, json: bool = False):
-    response = cloud._sync(
-        cloud._do_request,
-        method=method,
-        url=url,
-        data=data,
-    )
+def sync_request(cloud, url, method, data, json: bool = False, json_output: bool = False):
+    kwargs = {"method": method, "url": url}
+
+    if json:
+        kwargs["json"] = json_loads(data)
+    else:
+        kwargs["data"] = data
+    response = cloud._sync(cloud._do_request, **kwargs)
     if response.status >= 400:
         print(f"{url} returned {response.status}")
 
     async def get_result(r):
-        return await (r.json() if json else r.text())
+        return await (r.json() if json_output else r.text())
 
     return cloud._sync(
         get_result,
         response,
     )
```

### Comparing `coiled-0.8.9.dev9/coiled/cli/env.py` & `coiled-0.9.0/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/login.py` & `coiled-0.9.0/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/package_sync.py` & `coiled-0.9.0/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/prefect.py` & `coiled-0.9.0/coiled/cli/prefect.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/utils.py` & `coiled-0.9.0/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/cluster/__init__.py` & `coiled-0.9.0/coiled/cli/cluster/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 
 from ..utils import CONTEXT_SETTINGS
-from .better_logs import better_logs
+from .better_logs import better_logs_cli as better_logs
 from .logs import logs
 from .ssh import ssh
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 def cluster():
     """Commands for managing Coiled clusters"""
```

### Comparing `coiled-0.8.9.dev9/coiled/cli/cluster/better_logs.py` & `coiled-0.9.0/coiled/cli/cluster/better_logs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import time
 from datetime import datetime, timedelta, timezone
-from typing import Optional
+from typing import List, Optional, Tuple
 
 import click
 from rich.console import Console
 
 import coiled
 
 from ..utils import CONTEXT_SETTINGS
@@ -101,15 +101,15 @@
     help="Prepend datetime to all log messages",
 )
 @click.option(
     "--interval",
     default=3,
     help="Tail polling interval",
 )
-def better_logs(
+def better_logs_cli(
     account: Optional[str],
     cluster: Optional[str],
     no_scheduler: bool,
     workers: str,
     label: str,
     system: bool,
     combined: bool,
@@ -117,39 +117,73 @@
     interval: int,
     since: Optional[str],
     until: Optional[str],
     color: bool,
     filter: Optional[str],
     show_all_timestamps: bool,
 ):
-    console = Console(force_terminal=color)
-
     dask = not system or combined
     system = system or combined
     label = label.lower()
 
     if tail and until:
         raise click.ClickException("You can't use --until when tailing logs.")
 
     with coiled.Cloud(account=account) as cloud:
         cluster_info = find_cluster(cloud, cluster or "")
 
+    instance_labels_dict = make_instance_labels(
+        label=label,
+        no_scheduler=no_scheduler,
+        scheduler_id=cluster_info.get("scheduler", {}).get("instance", {}).get("id"),
+        workers=workers,
+        workers_info=cluster_info["workers"],
+    )
+
+    console = Console(force_terminal=color)
+
     cluster_id = cluster_info["id"]
+    cluster_name = cluster_info["name"]
+    cluster_state = cluster_info["current_state"]["state"]
 
-    if tail and cluster_info["current_state"]["state"] in (
+    if tail and cluster_state in (
         "stopped",
         "error",
     ):
         tail = False
-        console.print(f"[red]Cluster state is {cluster_info['current_state']['state']} so not tailing.[/red]")
+        console.print(f"[red]Cluster state is {cluster_state} so not tailing.[/red]")
+
+    if workers and not no_scheduler and not instance_labels_dict:
+        # exit here if there are no instances, otherwise passing empty list to
+        # coiled.better_cluster_logs will result in pulling logs for all instances
+        console.print("no instances match specified filters")
+        return
+
+    console.print(f"=== Logs for {cluster_name} ({cluster_id}) ===\n")
+    better_logs(
+        cluster_id=cluster_id,
+        instance_labels_dict=instance_labels_dict,
+        show_label=label == "none",
+        show_all_instances=workers == "all" and not no_scheduler,
+        console=console,
+        dask=dask,
+        system=system,
+        tail=tail,
+        interval=interval,
+        since=since,
+        until=until,
+        filter=filter,
+        show_all_timestamps=show_all_timestamps,
+    )
 
+
+def make_instance_labels(label, no_scheduler, scheduler_id, workers, workers_info):
     # instance ID's for which to show logs, key maps to label to use
     instances = {}
-    if not no_scheduler and cluster_info.get("scheduler", {}).get("instance"):
-        scheduler_id = cluster_info["scheduler"]["instance"]["id"]
+    if not no_scheduler and scheduler_id:
         instances[scheduler_id] = {
             "label": "scheduler" if label != "none" else "",
             "color": COLORS[-1],
         }
 
     def worker_label(worker: dict):
         if label == "none":
@@ -184,89 +218,185 @@
                 return True
 
             return False
 
         instances.update(
             {
                 worker["instance"]["id"]: dict(label=worker_label(worker), color=COLORS[idx % len(COLORS)])
-                for idx, worker in enumerate(cluster_info["workers"])
+                for idx, worker in enumerate(workers_info)
                 if worker.get("instance") and (workers == "all" or filter_worker(worker))
             }
         )
 
-    show_all_instances = workers == "all" and not no_scheduler
+    return instances
 
-    console.print(f"=== Logs for {cluster_info['name']} ({cluster_id}) ===\n")
 
-    if not instances:
-        # exit here if there are no instances, otherwise passing empty list to
-        # coiled.better_cluster_logs will result in pulling logs for all instances
-        console.print("no instances match specified filters")
-        return
+def better_logs(
+    *,
+    cluster_id: int,
+    instance_labels_dict: dict,
+    show_label: bool,
+    show_all_instances: bool,
+    console=None,
+    color: bool = True,
+    dask: bool = True,
+    system: bool = False,
+    tail: bool = False,
+    tail_max_times: Optional[int] = None,
+    interval: int = 3,
+    since: Optional[str] = None,
+    until: Optional[str] = None,
+    filter: Optional[str] = None,
+    show_timestamp: bool = True,
+    show_all_timestamps: bool = False,
+    start_sentinel: str = "",
+    stop_sentinel: str = "",
+):
+    console = console or Console(force_terminal=color)
 
     from_timestamp = ts_ms_from_string(since)
     until_timestamp = ts_ms_from_string(until)
     last_events = set()
 
     if tail and not from_timestamp:
         # for tail, start with logs from 30s ago if start isn't specified
         current_ms = int(time.time_ns() // 1e6)
         from_timestamp = current_ms - (30 * 1000)
 
+    waiting_for_start_sentinel = bool(start_sentinel)
+
     while True:
         events = coiled.better_cluster_logs(
             cluster_id=cluster_id,
             # function returns all instances if none specified, we'll use that
             # in order to not exclude instances that show up while tailing
-            instance_ids=None if show_all_instances else list(instances.keys()),
+            instance_ids=None if show_all_instances else list(instance_labels_dict.keys()),
             dask=dask,
             system=system,
             since_ms=from_timestamp,
             until_ms=until_timestamp,
             filter=filter,
         )
 
         if last_events:
             events = [e for e in events if e["timestamp"] != from_timestamp or event_dedupe_key(e) not in last_events]
 
         if events:
-            print_events(console, events, instances, show_all_timestamps=show_all_timestamps)
-
             from_timestamp = events[-1]["timestamp"]
             last_events = {event_dedupe_key(e) for e in events if e["timestamp"] == from_timestamp}
 
-        if tail:
+            # filter using sentinels
+            events, waiting_for_start_sentinel, found_stop_sentinel = filter_events(
+                events, start_sentinel, stop_sentinel, waiting_for_start_sentinel
+            )
+
+            print_events(
+                console,
+                events,
+                instance_labels_dict,
+                show_label=show_label,
+                show_timestamp=show_timestamp,
+                show_all_timestamps=show_all_timestamps,
+            )
+
+            if found_stop_sentinel:
+                break
+
+        if tail and (tail_max_times is None or tail_max_times > 0):
             # TODO stop tailing once cluster is stopped/errored (future MR)
+            if tail_max_times:
+                tail_max_times -= 1
             time.sleep(interval)
         else:
             break
 
 
+def filter_events(events, start_sentinel, stop_sentinel, waiting_for_start_sentinel) -> Tuple[list, bool, bool]:
+    found_stop_sentinel = False
+
+    if start_sentinel or stop_sentinel:
+        show_from = 0
+        show_to = -1
+        for i, event in enumerate(events):
+            if waiting_for_start_sentinel and start_sentinel in event["message"]:
+                waiting_for_start_sentinel = False
+                # remove everything before (first) start sentinel
+                # handle sentinel inside longer message
+                pos = event["message"].find(start_sentinel)
+                event["message"] = event["message"][pos + len(start_sentinel) :].strip()
+                # if there's text after start sentinel, include event with sentinel, otherwise start at next
+                # this is especially important because multiple lines can be joined into one event
+                show_from = i if event["message"] else i + 1
+
+            if show_to == -1 and stop_sentinel in event["message"]:
+                found_stop_sentinel = True
+                # remove everything after (first) stop sentinel
+                # handle sentinel inside longer message
+                pos = event["message"].find(stop_sentinel)
+                event["message"] = event["message"][:pos].strip()
+                # if there's text before stop sentinel, include event with sentinel, otherwise stop at previous
+                show_to = i + 1 if event["message"] else i
+
+            if not waiting_for_start_sentinel and show_to > -1:
+                # minor optimization
+                break
+        if waiting_for_start_sentinel:
+            events = []
+        elif show_from or show_to > -1:
+            events = events[show_from:show_to]
+
+    return events, waiting_for_start_sentinel, found_stop_sentinel
+
+
 def event_dedupe_key(event):
     return f'{event["timestamp"]}#{event["instance_id"]}#{event["message"]}'
 
 
-def print_events(console, events, instances: dict, pretty=True, show_all_timestamps=False):
+def print_events(
+    console,
+    events: List[dict],
+    instances: dict,
+    pretty=True,
+    show_label=True,
+    show_timestamp=True,
+    show_all_timestamps=False,
+):
     for e in events:
-        console.print(format_log_event(e, instances, pretty=pretty, show_all_timestamps=show_all_timestamps))
+        console.print(
+            format_log_event(
+                e,
+                instances,
+                pretty=pretty,
+                show_label=show_label,
+                show_timestamp=show_timestamp,
+                show_all_timestamps=show_all_timestamps,
+            )
+        )
 
 
-def format_log_event(event: dict, instances: dict, pretty: bool, show_all_timestamps: bool) -> str:
+def format_log_event(
+    event: dict, instances: dict, pretty: bool, show_label: bool, show_timestamp: bool, show_all_timestamps: bool
+) -> str:
     message = event["message"]
-    if event["instance_id"] in instances:
-        label = instances[event["instance_id"]]["label"]
-        color = instances[event["instance_id"]]["color"]
+
+    if show_label:
+        if event["instance_id"] in instances:
+            label = instances[event["instance_id"]]["label"]
+            color = instances[event["instance_id"]]["color"]
+        else:
+            # we might not know about instance if it showed up while we're tailing all worker logs
+            label = event["instance_id"]
+            color = COLORS[0]
     else:
-        # we might not know about instance if it showed up while we're tailing all worker logs
-        label = event["instance_id"]
-        color = COLORS[0]
+        label = ""
+        color = ""
 
     time_string = ""
 
-    if event.get("timestamp"):
+    if show_timestamp and event.get("timestamp"):
         time_format = "%Y-%m-%d %H:%M:%S.%f"
         t = datetime.utcfromtimestamp(event["timestamp"] / 1000)
 
         if show_all_timestamps or not message_has_timestamp(message, t):
             time_string = f"{t.strftime(time_format)} "
 
     # indent multiline log messages
```

### Comparing `coiled-0.8.9.dev9/coiled/cli/cluster/logs.py` & `coiled-0.9.0/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/cluster/metrics.py` & `coiled-0.9.0/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/cluster/ssh.py` & `coiled-0.9.0/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/cluster/utils.py` & `coiled-0.9.0/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/notebook/__init__.py` & `coiled-0.9.0/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/notebook/notebook.py` & `coiled-0.9.0/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/setup/__init__.py` & `coiled-0.9.0/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/setup/amp.py` & `coiled-0.9.0/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/setup/aws.py` & `coiled-0.9.0/coiled/cli/setup/aws.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,41 @@
 
 import coiled
 
 from ...auth import get_local_user
 from ..utils import CONTEXT_SETTINGS
 from .util import setup_failure
 
+WIDTH = 90
+
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.option(
+    "--region",
+    default=None,
+    help=(
+        "AWS region to use for Coiled. By default, this will use the "
+        "default region configured in your AWS profile if one is configured."
+    ),
+)
+@click.option(
+    "--profile",
+    default=None,
+    envvar="AWS_PROFILE",
+    help=(
+        "AWS profile to use from your local AWS credentials file. "
+        "By default, uses your `[default]` profile if one is configured."
+    ),
+)
+@click.option(
+    "--account",
+    default=None,
+    help="Coiled account that will be configured to use the AWS account. By default, uses your default Coiled account.",
+)
+@click.option(
     "--iam-user",
     default="coiled",
     help="IAM User to create in your AWS account",
 )
 @click.option(
     "--setup-policy",
     default=None,
@@ -32,20 +56,14 @@
 )
 @click.option(
     "--ongoing-policy",
     default=None,
     help="Non-default name for the ongoing IAM Policy, default `{iam-user}-ongoing`",
 )
 @click.option(
-    "--profile",
-    default=None,
-    envvar="AWS_PROFILE",
-    help="AWS profile to use from your local AWS credentials file",
-)
-@click.option(
     "--update-policies",
     default=False,
     is_flag=True,
     help="Only update existing IAM Policies",
 )
 @click.option(
     "--update-instance-policy",
@@ -55,20 +73,19 @@
 )
 @click.option(
     "--cloudshell-link",
     default=None,
     is_flag=True,
     help="Don't do setup, give instructions for setup using CloudShell",
 )
-@click.option("--region", default=None, help="AWS region to use when setting up your VPC/subnets")
 @click.option(
     "--manual-final-setup",
     default=False,
     is_flag=True,
-    help="Don't automatically send credentials to Coiled, " "finish setup manually in the web UI",
+    help="Don't automatically send credentials to Coiled, finish setup manually in the web UI",
 )
 @click.option(
     "--quotas",
     default=False,
     is_flag=True,
     help="Check and potentially request AWS quota increases for common instance types",
 )
@@ -90,22 +107,23 @@
     "--use-shim",
     default=False,
     is_flag=True,
     hidden=True,
     help="Use new setup backend",
 )
 def aws_setup(
+    region: Optional[str],
+    profile: Optional[str],
+    account: Optional[str],
     iam_user: str,
     setup_policy: Optional[str],
     ongoing_policy: Optional[str],
-    profile: Optional[str],
     update_policies: bool,
     update_instance_policy: bool,
     cloudshell_link: Optional[bool],
-    region: Optional[str],
     manual_final_setup: bool,
     quotas: bool,
     yes: bool,
     accept_delete: bool,
     use_shim: bool,
 ):
     accept_delete = yes and accept_delete  # (only accept_delete if --yes is also specified)
@@ -119,30 +137,30 @@
         cloudshell_link=cloudshell_link,
         region=region,
         manual_final_setup=manual_final_setup,
         quotas=quotas,
         yes=yes,
         accept_delete=accept_delete,
         use_shim=use_shim,
+        coiled_account=account,
     ):
         pass
         # print("[red]The setup process didn't finish.[/red]")
 
 
 DEFAULT_REGION = "us-east-1"
 
 TAGS = [{"Key": "owner", "Value": "coiled"}]
 
 PROMPTS = {
-    "initial": "Proceed with IAM setup for Coiled?",
+    "initial": "Proceed with IAM setup?",
     "replace_access_key": (
         "Too many access keys already exist for user "
         "[green]{user_name}[/green]. "
-        "Unable to retrieve secret for an existing key. "
-        "Delete key [green]{key_id}[/green] and create a new key?"
+        "\nDelete key [green]{key_id}[/green] and create a new key?"
     ),
     "request_quotas": "Would you like to make any AWS quota increase requests?",
 }
 
 SCRIPT_REQUIRED_IAM = [
     "iam:GetPolicy",
     "iam:ListAccessKeys",
@@ -279,30 +297,30 @@
         arn = r["User"]["Arn"]
         coiled.add_interaction(action="CreateUser", success=True, arn=arn)
     except iam.exceptions.EntityAlreadyExistsException:
         print(f"user [green]{name}[/green] already exists")
     return arn
 
 
-def create_or_update_policy(iam, account, name, doc):
+def create_or_update_policy(iam, aws_account, name, doc):
     try:
         r = iam.create_policy(PolicyName=name, PolicyDocument=doc)
         arn = r["Policy"]["Arn"]
         coiled.add_interaction(action="CreatePolicy", success=True, arn=arn)
     except iam.exceptions.EntityAlreadyExistsException:
-        arn = f"arn:aws:iam::{account}:policy/{name}"
-        update_policy(iam, account, name, doc)
+        arn = f"arn:aws:iam::{aws_account}:policy/{name}"
+        update_policy(iam, aws_account, name, doc)
 
     return arn
 
 
-def get_policy_diff(iam, account, name, doc):
+def get_policy_diff(iam, aws_account, name, doc):
     existing_arn, changes = None, None
 
-    arn = f"arn:aws:iam::{account}:policy/{name}"
+    arn = f"arn:aws:iam::{aws_account}:policy/{name}"
 
     try:
         policy = iam.get_policy(PolicyArn=arn)
         existing_arn = arn
     except iam.exceptions.ClientError as e:
         error_code = e.response["Error"].get("Code")
 
@@ -345,31 +363,31 @@
 
         # if we couldn't print the short version, just print the raw diff object
         return f"{doc_diff}"
     else:
         return ""
 
 
-def update_policy(iam, account, name, doc):
-    policy_arn = f"arn:aws:iam::{account}:policy/{name}"
+def update_policy(iam, aws_account, name, doc):
+    policy_arn = f"arn:aws:iam::{aws_account}:policy/{name}"
     try:
         r = iam.create_policy_version(PolicyArn=policy_arn, PolicyDocument=doc, SetAsDefault=True)
         coiled.add_interaction(action="CreatePolicyVersion", success=True, arn=policy_arn)
         new_version = r["PolicyVersion"]["VersionId"]
         print(f"Updated Policy [green]{policy_arn}[/green] is [bold]{new_version}[/bold]")
         print()
     except iam.exceptions.LimitExceededException:
         # this is Coiled-specific policy so should be fine to delete old version
         existing_policies = iam.list_policy_versions(PolicyArn=policy_arn)
         to_delete = [
             version["VersionId"] for version in existing_policies["Versions"] if not version["IsDefaultVersion"]
         ][-1]
         print(f"Policy {name} has too many existing versions, deleting {to_delete}")
         iam.delete_policy_version(PolicyArn=policy_arn, VersionId=to_delete)
-        update_policy(iam, account, name, doc)
+        update_policy(iam, aws_account, name, doc)
     except Exception as e:
         coiled.add_interaction(
             action="CreatePolicyVersion",
             success=False,
             arn=policy_arn,
             error_message=str(e),
         )
@@ -434,31 +452,32 @@
 
 
 def delete_access_key(iam, user, accept_delete: bool = False):
     r = iam.list_access_keys(UserName=user)
     key_id = r["AccessKeyMetadata"][0]["AccessKeyId"]
 
     # NOTE: --yes doesn't apply to this since currently
+    print()
     if accept_delete or Confirm.ask(
         PROMPTS["replace_access_key"].format(user_name=user, key_id=key_id),
         default=True,
     ):
         coiled.add_interaction(action="prompt:DeleteAccessKey", success=True, user=user)
         iam.delete_access_key(UserName=user, AccessKeyId=key_id)
         coiled.add_interaction(action="DeleteAccessKey", success=True, user=user, key_id=key_id)
-        print(f"    Deleted access key [green]{key_id}[/green]")
-        print()
+        print(f"Deleted access key [green]{key_id}[/green]")
         return True
     else:
         coiled.add_interaction(action="prompt:DeleteAccessKey", success=False, user=user)
 
     return False
 
 
 def wait_till_key_works(iam, key, secret):
+    print("")
     print("Waiting until access key is ready", end="")
     t0 = time.time()
 
     while t0 + 10 > time.time():
         try:
             coiled.utils.verify_aws_credentials(key, secret)
             # a little extra wait here also seems to help, otherwise we *still* yet error sometimes when trying to use
@@ -474,62 +493,73 @@
                 time.sleep(1)
                 continue
 
     print("\nAccess key is still not ready. Please manually set up your Coiled account with AWS.")
     return False
 
 
-def do_intro(sts, iam, region):
-    print("This uses your AWS credentials to setup Coiled.\n")
+def do_intro(sts, iam, region, coiled_account):
+    introduction = """
+[bold]Introduction[/bold]
+
+This uses your AWS credentials to set up Coiled.
+
+This will do the following ...
+1. Create limited IAM roles and grant them to Coiled
+2. Check and expand your AWS quota if needed
+3. Create initial resources to deploy clusters
+
+This will [bold]not[/bold] ...
+1. Create resources that cost money
+2. Grant Coiled access to your data
+""".strip()
+    print(Panel(introduction, width=WIDTH))
 
     try:
         # get_caller_identity doesn't require any specific IAM rights
         identity = sts.get_caller_identity()
-        account = identity.get("Account")
+        aws_account = identity.get("Account")
         identity_as = identity.get("Arn").split(":")[-1]
 
         coiled.add_interaction(
             action="GetCallerIdentity",
             success=True,
-            account=account,
+            account=aws_account,
             identity_as=identity_as,
         )
 
         try:
             r = iam.list_account_aliases()
             account_alias = r.get("AccountAliases", [])[0]
-            alias_string = f" ([green]{account_alias}[/green])"
+            alias_string = f" ({account_alias})"
             coiled.add_interaction(
                 action="ListAccountAliases",
                 success=True,
-                account=account,
+                account=aws_account,
                 alias=alias_string,
             )
         except Exception:
             # doesn't matter much if we can't get account alias
             alias_string = ""
 
-        account_desc = (
-            f"Current local AWS credentials:\t[green]{identity_as}[/green]"
-            "\n"
-            f"Proposed region for Coiled:\t[green]{region}[/green]"
-            "\t(use [green]coiled setup aws --region[/green] to change)"
-            "\n"
-            f"Proposed account for Coiled:\t[green]{account}[/green]{alias_string}"
-            "\n"
-            "\n"
-            "If this is not correct then please stop and select a different profile "
-            "from your AWS credentials file using the "
-            "[green]coiled setup aws [bold]--profile[/bold][/green] argument."
-        )
+        account_desc = f"""
+[bold]Target AWS Account[/bold]
 
-        print(Panel(account_desc))
-        print()
+Current credentials:\t[green]{identity_as}[/green]
+Proposed region :\t[green]{region}[/green]
+Proposed account:\t[green]{aws_account}[/green]{alias_string}
+
+If this is incorrect then stop and select a different ...
+  profile using the [green]coiled setup aws [bold]--profile[/bold][/green] argument
+  region using the [green]coiled setup aws [bold]--region[/bold][/green] argument
+""".strip()
+
+        print(Panel(account_desc, width=WIDTH))
 
-        return account
+        return aws_account
     except botocore.exceptions.NoCredentialsError:
         coiled.add_interaction(
             action="GetCallerIdentity",
             success=False,
             error_message="NoCredentialsError",
         )
 
@@ -539,42 +569,42 @@
         )
         setup_failure("Getting local aws credentials failed", backend="aws")
         print()
         # is aws cli installed?
         # get_aws_cli_version = subprocess.run(["aws", "--version"], capture_output=True)
         # has_aws_cli = get_aws_cli_version.returncode == 0
 
-        show_cloudshell_instructions(region)
+        show_cloudshell_instructions(region, coiled_account=coiled_account)
 
     except Exception as e:
         coiled.add_interaction(action="GetCallerIdentity", success=False, error_message=str(e))
         setup_failure(f"Getting local aws credentials failed {str(e)}", backend="aws")
         print("Error determining your AWS account:")
         print(f"    [red]{e}[/red]")
         print()
 
-        show_cloudshell_instructions(region)
+        show_cloudshell_instructions(region, coiled_account=coiled_account)
 
     return None
 
 
-def show_cloudshell_instructions(region):
+def show_cloudshell_instructions(region, coiled_account):
     # explain cloudshell
     server_arg = (
         f"--server {dask.config.get('coiled.server', coiled.utils.COILED_SERVER)} \\ "
         if dask.config.get("coiled.server", coiled.utils.COILED_SERVER) != coiled.utils.COILED_SERVER
         else ""
     )
     token_arg = f"--token {dask.config.get('coiled.token')} && \\"
-
     region_arg = f" --region {region}" if region else ""
+    account_arg = f"--account {coiled_account} " if coiled_account else ""
 
     cli_lines = [
         "pip3 install coiled && \\ ",
-        "coiled login \\ ",
+        f"coiled login {account_arg}\\ ",
     ]
     if server_arg:
         cli_lines.append(server_arg)
     cli_lines.extend(
         [
             token_arg,
             f"coiled setup aws{region_arg}",
@@ -591,102 +621,119 @@
         f"  [green]{cli_command}[/green]\n"
     )
 
     # box might be nice but would make copying the command much worse
     print(instruction_text)
 
 
-def do_coiled_setup(iam, key, secret, region, yes, use_shim) -> bool:
+def do_coiled_setup(iam, key, secret, region, coiled_account, yes, use_shim) -> bool:
     success = False
     backend_failure = False
 
     if key and secret:
-        print("[bold]You can setup Coiled to use the AWS credentials you just created.")
-        print(
-            "This AWS access key will go to Coiled, where it will be stored securely and "
-            "used to create clusters in your AWS account on your behalf."
-        )
-        print(
-            "This will also create infrastructure in your account like a VPC and subnets "
-            "none of which has a standing cost."
-        )
-        print()
-        if yes or Confirm.ask(
-            "Setup your Coiled account to use the AWS credentials you just created?",
-            default=True,
-        ):
-            coiled.add_interaction(action="prompt:CoiledSetup", success=True)
-            # wait on this for a bit till we don't get InvalidClientTokenId error
-            if wait_till_key_works(iam, key, secret):
-                print("Setting up Coiled to use your AWS account...")
-                try:
-                    coiled.set_backend_options(
-                        backend="aws",
-                        aws_access_key_id=key,
-                        aws_secret_access_key=secret,
-                        aws_region=region,
-                        use_shim=use_shim,
-                    )
-                    success = True
-                    coiled.add_interaction(action="CoiledSetup", success=True)
-                except Exception as e:
-                    backend_failure = True
-                    error_message = str(e)
-                    coiled.add_interaction(action="CoiledSetup", success=False, error_message=error_message)
-                    print()
-                    print("[red]There was an error setting up Coiled to use your AWS account:\n")
-                    print(error_message)
-            else:
-                coiled.add_interaction(action="CoiledSetup", success=False)
-                print("[red]Access key is still not ready. You need to complete Coiled setup manually.")
+        coiled.add_interaction(action="prompt:CoiledSetup", success=True)
+        # wait on this for a bit till we don't get InvalidClientTokenId error
+        if wait_till_key_works(iam, key, secret):
+            print("Setting up Coiled to use your AWS account...")
+            try:
+                coiled.set_backend_options(
+                    account=coiled_account,
+                    backend="aws",
+                    aws_access_key_id=key,
+                    aws_secret_access_key=secret,
+                    aws_region=region,
+                    use_shim=use_shim,
+                )
+                success = True
+                coiled.add_interaction(action="CoiledSetup", success=True)
+            except Exception as e:
+                backend_failure = True
+                error_message = str(e)
+                coiled.add_interaction(action="CoiledSetup", success=False, error_message=error_message)
                 print()
+                print("[red]There was an error setting up Coiled to use your AWS account:\n")
+                print(error_message)
         else:
             coiled.add_interaction(action="prompt:CoiledSetup", success=False)
 
+        message = """
+[bold]Setup complete 🎉[/bold]
+
+What's next?
+
+  Run a command line application in the cloud with:
+
+    $ [bold]coiled run echo 'Hello, world'[/bold]
+
+  Or create a Dask cluster with:
+
+    $ ipython
+
+    [bold]import coiled
+    cluster = coiled.Cluster(
+        n_workers=10,
+    )
+    client = cluster.get_client()[/bold]
+
+  For more examples see [link]https://docs.coiled.io/user_guide/examples/index.html[/link]
+""".strip()
+
+        print()
+        print()
+        print(message)
+
         if not success and not backend_failure:
-            show_manual_setup(key, secret)
+            show_manual_setup(key, secret, coiled_account=coiled_account)
 
     return success
 
 
 def do_full_setup(
-    session, iam, user_name, account, region, setup_name, ongoing_name, manual_final_setup, yes, accept_delete, use_shim
+    session,
+    iam,
+    user_name,
+    aws_account,
+    region,
+    setup_name,
+    ongoing_name,
+    *,
+    coiled_account,
+    manual_final_setup,
+    yes,
+    accept_delete,
+    use_shim,
 ) -> bool:
     # Check for existing user
     user_exists, user_keys = get_user_access_keys(iam, user_name)
 
     # Check for existing policies
-    setup_arn, setup_diff = get_policy_diff(iam, account, setup_name, setup_doc)
-    ongoing_arn, ongoing_diff = get_policy_diff(iam, account, ongoing_name, ongoing_doc)
+    setup_arn, setup_diff = get_policy_diff(iam, aws_account, setup_name, setup_doc)
+    ongoing_arn, ongoing_diff = get_policy_diff(iam, aws_account, ongoing_name, ongoing_doc)
 
-    print("Attempting to create/update the following resources in your AWS account:")
-
-    resource_strings = []
+    resource_strings = ["[bold]Proposed AWS Account Changes[/bold]\n"]
 
     if not user_exists:
         resource_strings.append(f"Create IAM User:\t[green]{user_name}[/green]")
         resource_strings.append("  and create Access Key for this new IAM User")
     else:
         resource_strings.append(f"Create Access Key for [bold]existing[/bold] IAM User:\t[green]{user_name}[/green]")
 
         existing_key_message = f"  This IAM User already has {len(user_keys)} access keys."
         if len(user_keys) > 1:
             existing_key_message = (
                 f"  This IAM User already has {len(user_keys)} access keys. \n"
-                "  We'll need to [bold]delete[/bold] an existing access key in order to create a new access key "
-                "for Coiled to use."
+                "  We'll need to [bold]delete[/bold] an existing access key to create a new access key."
             )
         resource_strings.append(existing_key_message)
         resource_strings.append("")
         resource_strings.append(
             "If you didn't want to configure Coiled with this existing IAM User, "
             "stop now and specify a different IAM User name with the "
             "[green]coiled setup aws [bold]--iam-user[/bold][/green] argument."
         )
-        resource_strings.append("")
 
     if not setup_arn:
         resource_strings.append("")
         resource_strings.append(f"Create IAM Policy:\t[green]{setup_name}[/green]")
         resource_strings.append(f"  and attach to IAM User [green]{user_name}[/green]")
     if setup_diff:
         resource_strings.append(f"Update IAM Policy:\t[green]{setup_name}[/green]")
@@ -704,23 +751,22 @@
         resource_strings.append(show_policy_diff(setup_diff))
 
     if ongoing_diff:
         resource_strings.append("")
         resource_strings.append(f"Proposed changes to the existing [green]{ongoing_name}[/green] IAM Policy:")
         resource_strings.append(show_policy_diff(ongoing_diff))
 
-    resource_desc = "\n".join(resource_strings)
-    print(Panel(resource_desc))
-
     if not setup_arn or not ongoing_arn:
-        print(
-            "Documentation for IAM Policies at "
+        resource_strings.append(
+            "\nDocumentation for IAM Policies at "
             "[link]https://docs.coiled.io/user_guide/aws_configure.html#create-iam-policies[/link]"
         )
-        print()
+
+    resource_desc = "\n".join(resource_strings)
+    print(Panel(resource_desc, width=WIDTH))
 
     if not yes and not Confirm.ask(PROMPTS["initial"], default=True):
         coiled.add_interaction(action="prompt:Setup_AWS", success=False)
         return False
 
     coiled.add_interaction(action="prompt:Setup_AWS", success=True)
 
@@ -728,24 +774,24 @@
 
     if not user_exists:
         user_arn = create_user(iam, user_name)
         if user_arn:
             create_arns.append(user_arn)
 
     if not setup_arn:
-        setup_arn = create_or_update_policy(iam, account, setup_name, setup_doc)
+        setup_arn = create_or_update_policy(iam, aws_account, setup_name, setup_doc)
         create_arns.append(setup_arn)
     elif setup_diff:
-        setup_arn = create_or_update_policy(iam, account, setup_name, setup_doc)
+        setup_arn = create_or_update_policy(iam, aws_account, setup_name, setup_doc)
 
     if not ongoing_arn:
-        ongoing_arn = create_or_update_policy(iam, account, ongoing_name, ongoing_doc)
+        ongoing_arn = create_or_update_policy(iam, aws_account, ongoing_name, ongoing_doc)
         create_arns.append(ongoing_arn)
     elif ongoing_diff:
-        ongoing_arn = create_or_update_policy(iam, account, ongoing_name, ongoing_doc)
+        ongoing_arn = create_or_update_policy(iam, aws_account, ongoing_name, ongoing_doc)
 
     attach_policy(iam, user_name, setup_arn)
     attach_policy(iam, user_name, ongoing_arn)
 
     print()
     if create_arns:
         print("The following resources were created in your AWS account:")
@@ -755,22 +801,25 @@
     print()
 
     check_quotas(session, region=region)
 
     key, secret = make_access_key(iam, user_name, accept_delete=accept_delete)
 
     if manual_final_setup:
-        return show_manual_setup(key, secret)
+        return show_manual_setup(key, secret, coiled_account)
     else:
-        return do_coiled_setup(iam, key, secret, region, yes, use_shim)
+        return do_coiled_setup(
+            iam=iam, key=key, secret=secret, region=region, coiled_account=coiled_account, yes=yes, use_shim=use_shim
+        )
 
 
-def show_manual_setup(key, secret):
-    with coiled.Cloud() as cloud:
-        coiled_account = cloud.default_account
+def show_manual_setup(key, secret, coiled_account):
+    if not coiled_account:
+        with coiled.Cloud() as cloud:
+            coiled_account = cloud.default_account
 
     setup_url = (
         f"{dask.config.get('coiled.server', coiled.utils.COILED_SERVER)}/"
         f"{coiled_account}/settings/setup/update-backend-options"
     )
 
     print(
@@ -788,25 +837,26 @@
             "\n"
             "3. Select your desired default AWS region and enter these values where prompted:\n"
             "\n"
             f"\tAWS Access Key ID:\t[green]{key}[/green]\n"
             f"\tAWS Secret Access Key:\t[green]{secret}[/green]\n"
             "\n"
             "4. Continue with the other account setup steps; you'll be able to "
-            "choose non-default network or container registry settings as desired."
+            "choose non-default network or container registry settings as desired.",
+            width=WIDTH,
         )
     )
 
     return True
 
 
-def do_just_update_policies(iam, account, setup_name, ongoing_name, yes) -> bool:
+def do_just_update_policies(iam, aws_account, setup_name, ongoing_name, yes) -> bool:
     # Check for existing policies
-    setup_arn, setup_diff = get_policy_diff(iam, account, setup_name, setup_doc)
-    ongoing_arn, ongoing_diff = get_policy_diff(iam, account, ongoing_name, ongoing_doc)
+    setup_arn, setup_diff = get_policy_diff(iam, aws_account, setup_name, setup_doc)
+    ongoing_arn, ongoing_diff = get_policy_diff(iam, aws_account, ongoing_name, ongoing_doc)
 
     if not setup_arn:
         print(f"[red]WARNING[/red]: No IAM Policy named [green]{setup_name}[/green] found.")
         print("Use `--setup-policy` to specify a different name for the existing setup policy.")
         print()
         return False
 
@@ -835,45 +885,46 @@
         print("Your [bold]ongoing[/bold] IAM Policy is up-to-date")
         print("You may need to update your [bold]setup[/bold] IAM Policy.")
 
     elif not yes and not Confirm.ask(PROMPTS["initial"], default=True):
         return False
 
     if setup_diff:
-        update_policy(iam, account, setup_name, setup_doc)
+        update_policy(iam, aws_account, setup_name, setup_doc)
 
     if ongoing_diff:
-        update_policy(iam, account, ongoing_name, ongoing_doc)
+        update_policy(iam, aws_account, ongoing_name, ongoing_doc)
 
     return True
 
 
-def get_session(aws_profile: Optional[str], region_name: Optional[str]):
+def get_session(aws_profile: Optional[str], region_name: Optional[str], skip_telemetry: bool = False):
     try:
         session = boto3.Session(profile_name=aws_profile, region_name=region_name)
-        coiled.add_interaction(
-            action="BotoSession",
-            success=True,
-            profile=aws_profile,
-            region_name=session.region_name,
-        )
+        if not skip_telemetry:
+            coiled.add_interaction(
+                action="BotoSession",
+                success=True,
+                profile=aws_profile,
+                region_name=session.region_name,
+            )
         return session
     except botocore.exceptions.ProfileNotFound:
         coiled.add_interaction(
             action="BotoSession",
             success=False,
             profile=aws_profile,
             error_message="ProfileNotFound",
         )
         print()
         print(f"[red]The profile `{aws_profile}` is not configured in your local AWS credentials.")
         print(
             "If this isn't the correct AWS identity or account, you can specify a different profile "
             "from your AWS credentials file using the "
-            "[green]coiled setup aws [bold]--profile[/bold][/green] argument."
+            "[green]coiled setup aws [bold]--profile[/bold][/green] argument"
         )
         setup_failure("Requested AWS profile not found", backend="aws")
         return None
 
 
 def do_setup(
     slug,
@@ -885,88 +936,114 @@
     region=None,
     cloudshell_link=None,
     manual_final_setup=None,
     quotas=None,
     yes=False,
     accept_delete=False,
     use_shim=False,
+    coiled_account=None,
 ) -> bool:
     local_user = get_local_user()
 
-    # TODO check for Coiled login, explain that we need this to automatically do Coiled setup, but they can do manually
-    # call coiled.Cloud() here if we want to ensure/force log in -- is there way to just check?
-    coiled.add_interaction(
-        action="CliSetupAws",
-        success=True,
-        local_user=local_user,
-        # use keys that match the cli args
-        profile=aws_profile,
-        iam_user=slug,
-        setup_policy=setup_name,
-        ongoing_policy=ongoing_name,
-        update_policies=just_update_policies,
-        update_instance_policy=just_update_instance_policy,
-        region=region,
-        cloudshell_link=cloudshell_link,
-        manual_final_setup=manual_final_setup,
-        yes=yes,
-        accept_delete=accept_delete,
-    )
+    # this isn't perfect since we aren't checking if token is valid, but it's better than nothing
+    is_logged_in = bool(dask.config.get("coiled.token", None))
+
+    # We don't want to require Coiled account if just using `coiled setup aws --quotas`, thus
+    # skipping telemetry for `--quotas` if user doesn't already have local Coiled token.
+    skip_telemetry = bool(quotas and not is_logged_in)
+
+    if not is_logged_in and not quotas:
+        print("To set up your Coiled account, you'll need to authorize this computer to access your Coiled account.")
+
+    if not skip_telemetry:
+        # This will trigger auth flow if necessary.
+        try:
+            coiled.add_interaction(
+                action="CliSetupAws",
+                success=True,
+                local_user=local_user,
+                # use keys that match the cli args
+                profile=aws_profile,
+                iam_user=slug,
+                setup_policy=setup_name,
+                ongoing_policy=ongoing_name,
+                update_policies=just_update_policies,
+                update_instance_policy=just_update_instance_policy,
+                region=region,
+                cloudshell_link=cloudshell_link,
+                manual_final_setup=manual_final_setup,
+                yes=yes,
+                accept_delete=accept_delete,
+                coiled_account=coiled_account,
+            )
+        except KeyboardInterrupt:
+            if not bool(dask.config.get("coiled.token", None)):
+                print("[red]This computer doesn't have access to your Coiled account so setup cannot continue.")
+                print("Try running [green]coiled login[/green] to authorize access to your Coiled account.")
+                return False
+        except ValueError as e:
+            if "Authorization failed" in str(e):
+                print("[red]This computer doesn't have access to your Coiled account so setup cannot continue.")
+                print("Try running [green]coiled login[/green] to authorize access to your Coiled account.")
+                return False
+            else:
+                raise
 
     if cloudshell_link:
-        show_cloudshell_instructions(region)
+        show_cloudshell_instructions(region, coiled_account=coiled_account)
         return False
 
     try:
-        session = get_session(aws_profile, region_name=region)
+        session = get_session(aws_profile, region_name=region, skip_telemetry=skip_telemetry)
         if session is None:
             return False
 
         region = region or session.region_name or DEFAULT_REGION
 
         if quotas:
             # check quotas and give option to request increases
-            check_quotas(session, region=region, request_quotas=True)
+            check_quotas(session, region=region, just_quota_flow=True)
             return False
 
         try:
             iam = session.client("iam")
         except Exception as e:
             print()
             print("Something went wrong when trying to use your local AWS credentials.")
             print()
             print(f"[red][bold]{type(e).__name__}[/bold]: {e}[/red]")
             print()
-            show_cloudshell_instructions(region)
+            show_cloudshell_instructions(region, coiled_account=coiled_account)
             return False
 
         sts = session.client("sts")
 
         user_name = slug
         setup_name = setup_name or f"{slug}-setup"
         ongoing_name = ongoing_name or f"{slug}-ongoing"
 
         try:
-            account = do_intro(sts, iam, region=region)
-            if not account:
+            aws_account = do_intro(sts, iam, region=region, coiled_account=coiled_account)
+            if not aws_account:
                 return False
 
             if just_update_instance_policy:
-                return update_instance_profile_policy(iam, account, yes=yes)
+                return update_instance_profile_policy(iam, aws_account, yes=yes)
             elif just_update_policies:
-                return do_just_update_policies(iam, account, setup_name, ongoing_name, yes=yes)
+                return do_just_update_policies(iam, aws_account, setup_name, ongoing_name, yes=yes)
             else:
                 return do_full_setup(
                     session,
                     iam,
                     user_name,
-                    account,
+                    aws_account,
                     region,
                     setup_name,
                     ongoing_name,
+                    coiled_account=coiled_account,
                     manual_final_setup=manual_final_setup,
                     yes=yes,
                     accept_delete=accept_delete,
                     use_shim=use_shim,
                 )
 
         except iam.exceptions.ClientError as e:
@@ -981,15 +1058,15 @@
                 print("It appears that you're trying to set up Coiled from inside Amazon SageMaker.")
                 print(
                     "SageMaker has restricted permissions on your AWS account. Although you [bold]can use[/bold] "
                     "Coiled from a SageMaker notebook, you [bold]cannot set up[/bold] Coiled from SageMaker."
                 )
                 print()
                 setup_failure("Inside sagemaker", backend="aws")
-                show_cloudshell_instructions(region)
+                show_cloudshell_instructions(region, coiled_account=coiled_account)
                 return False
 
             elif "AccessDenied" in str(e):
                 print()
                 print(f"Insufficient permissions to [green]{error_op}[/green] using current AWS profile/user.")
                 print("You may want to try with a different AWS profile that has different permissions.")
                 print()
@@ -1017,46 +1094,47 @@
                 print()
                 setup_failure(
                     f"Error trying {error_op}. {error_msg}",
                     backend="aws",
                 )
                 return False
 
-    # catch all so we make sure all errors are tracked
     except KeyboardInterrupt as e:
         tb = "\n".join(traceback.format_tb(e.__traceback__))
         coiled.add_interaction(action="KeyboardInterrupt", success=False, error_message=tb)
         raise
 
-    # except Exception as e:
-    #     msg = traceback.format_exc()
-    #     coiled.add_interaction(action="Unknown", success=False, error_message=msg)
-    #     # TODO
-    #     print()
-    #     print("[red]An unhandled exception happened!")
-    #     print(e)
-    #     setup_failure(
-    #         f"Unhandled exception {msg}",
-    #         backend="aws",
-    #     )
-    #     return False
+    # catch all so we make sure all errors are tracked
+    except Exception as e:
+        msg = traceback.format_exc()
+        coiled.add_interaction(action="Unknown", success=False, error_message=msg)
+        # TODO better generic error handling
+        print()
+        print("[red][bold]ERROR[/bold][/red] Something unexpected happened:")
+        print(f"    [red]{e}")
+        print("Please reach out to Coiled Support at support@coiled.io if you need help with this issue.")
+        setup_failure(
+            f"Unhandled exception {msg}",
+            backend="aws",
+        )
+        return False
 
 
 def check_local_aws_creds():
     session = boto3.Session()
     sts = session.client("sts")
     try:
         # good call to try, since this doesn't require any IAM permissions
         sts.get_caller_identity()
         return True
     except botocore.exceptions.NoCredentialsError:
         return False
 
 
-def update_instance_profile_policy(iam, account, yes):
+def update_instance_profile_policy(iam, aws_account, yes):
     policy_name = "CoiledInstancePolicy"
     policy_doc = """{
     "Version": "2012-10-17",
     "Statement": [
         {
             "Sid": "CoiledEC2Policy",
             "Effect": "Allow",
@@ -1069,15 +1147,15 @@
             ],
             "Resource": "*"
         }
     ]
 }"""
 
     # Check for existing policy
-    policy_arn, policy_diff = get_policy_diff(iam, account, policy_name, policy_doc)
+    policy_arn, policy_diff = get_policy_diff(iam, aws_account, policy_name, policy_doc)
 
     if not policy_arn:
         print(f"[red]WARNING[/red]: No IAM Policy named [green]{policy_name}[/green] found.")
         print()
 
     if policy_diff:
         print(f"Proposed changes to the existing [green]{policy_name}[/green] IAM Policy:")
@@ -1087,20 +1165,20 @@
     if policy_arn and not policy_diff:
         print(f"Your AWS policy document for {policy_name} is up-to-date")
 
     elif not yes and not Confirm.ask(f"Update {policy_name} policy document?", default=True):
         return False
 
     if policy_diff:
-        update_policy(iam, account, policy_name, policy_doc)
+        update_policy(iam, aws_account, policy_name, policy_doc)
 
     return True
 
 
-def check_quotas(session, region: str, request_quotas: bool = False):
+def check_quotas(session, region: str, just_quota_flow: bool = False):
     quota_client = session.client("service-quotas", region_name=region)
 
     quotas = [
         {
             "class": "Standard On-Demand",
             "name": "Running On-Demand Standard (A, C, D, H, I, M, R, T, Z) instances",
             "code": "L-1216C47A",
@@ -1175,38 +1253,42 @@
             quota_value_text = f"[link]{quota['link']}[/link]"
 
         quota_lines.append(f"{quota_label:<36}{quota_value_text}")
 
     quota_text = "\n".join(quota_lines)
 
     quota_text = (
-        "Coiled runs in your AWS account, so your cluster sizes will be constrained by your AWS quotas:\n\n"
+        "[bold]Current AWS Quotas[/bold]\n\n"
         f"{quota_text}\n\n"
-        "[bold]Standard[/bold] includes "
-        "general purpose [bold]M[/bold] and [bold]T[/bold] families (e.g., M6i, T3), "
-        "compute optimized [bold]C[/bold] families (e.g., C6i), "
-        "and memory optimized [bold]R[/bold] families (e.g., R6i)."
-        "\n\n[bold]GPU[/bold] instances require a separate quota. "
-        "[bold]G4dn[/bold] is our default GPU instance type on AWS, these have an NVIDIA T4 GPU."
+        "[bold]Standard[/bold] includes:\n"
+        "    general purpose [bold]M[/bold] and [bold]T[/bold] families (e.g., M6i, T3),\n"
+        "    compute optimized [bold]C[/bold] families (e.g., C6i),\n"
+        "    memory optimized [bold]R[/bold] families (e.g., R6i).\n"
+        "\n[bold]GPU[/bold] instances have a separate quotas based on GPU type."
     )
 
-    if got_quotas:
+    if got_quotas and not just_quota_flow:
+        example_cost = "2.46" if region == "us-west-1" else "2.11"
+        example_region = region if region in ("us-east-1", "us-east-2", "us-west-1", "us-west-2") else "us-east-1"
+
         quota_text = (
             f"{quota_text}\n\n"
-            "The default Coiled instance type ([bold]t3.xlarge[/bold]) has [bold]4 vCPUs[/bold], "
-            "so a 10 worker cluster (plus scheduler) would have [bold]44 vCPUs[/bold]."
+            "[bold]Example Usage:[/bold]\n"
+            "10 VM cluster with m6i.xlarge instances would have 40 vCPUs.\n"
+            f"AWS compute cost would be ${example_cost}/hr "
+            f"for on-demand instances in {example_region}."
         )
 
     if error_message:
         quota_text = f"{error_message}\n\n{quota_text}"
 
-    print(Panel(quota_text))
+    print(Panel(quota_text, width=WIDTH))
 
     if got_quotas:
-        if request_quotas:
+        if just_quota_flow:
             # when running explicit quota check (`--quotas`), prompt about each quota
             do_quota_increases(quota_client, region, quotas)
         elif low_quotas:
             print(
                 "Some of your quotas are low. If you'd like to request any increases for these quotas, "
                 "we can prompt you for the desired quota value and attempt to submit this request to AWS.\n"
             )
@@ -1223,16 +1305,16 @@
     )
     return int(quota["Quota"]["Value"])
 
 
 def do_quota_increases(quota_client, region: str, quotas: list):
     for quota in quotas:
         prompt = (
-            f"Your current quota for [bold]{quota['class']}[/bold] ({region}) is [bold]{quota['value']}[/bold]. "
-            "If you'd like to request an increase from AWS, enter the new number (or hit return to skip):"
+            f"[bold]{quota['class']}[/bold] ({region}) current quota: [bold]{quota['value']}[/bold]\n"
+            "Request new quota value? (return to skip):"
         )
         desired_value = IntPrompt.ask(prompt, default=quota["value"])
         if desired_value and desired_value != quota["value"]:
             if not request_quota_increase(quota_client, region, quota, desired_value=desired_value):
                 # something failed so stop
                 return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `coiled-0.8.9.dev9/coiled/cli/setup/entry.py` & `coiled-0.9.0/coiled/cli/setup/entry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import traceback
 
 import click
 from rich import print
+from rich.panel import Panel
 from rich.prompt import Prompt
 
 import coiled
 
 from ..utils import CONTEXT_SETTINGS
 from .util import setup_failure
 
@@ -21,21 +22,29 @@
 
     coiled.add_interaction(
         action="cli-setup-wizard:start",
         success=True,
     )
 
     print(
-        "Welcome to Coiled!\n\n"
-        "To begin you need to connect Coiled to your cloud account.\n"
-        "Select one of the following options:\n\n"
-        "  1. Amazon Web Service (AWS)\n"
-        "  2. Google Cloud Platform (GCP)\n"
-        "  3. I don't have a cloud account, set me up with a free trial?\n"
-        "  [red]x[/red]. Exit setup\n"
+        Panel(
+            """
+[bold]Welcome to Coiled![/bold]
+
+To begin you need to connect Coiled to your cloud account.
+Select one of the following options:
+
+  1. Amazon Web Service ([green]AWS[/green])
+  2. Google Cloud Platform ([green]GCP[/green])
+  3. I don't have a cloud account, set me up with a free trial?
+  [red]x[/red]. Exit setup
+
+""".strip(),
+            width=90,
+        )
     )
 
     try:
         choice = Prompt.ask(
             "Choice",
             choices=["1", "2", "3", "x"],
             show_choices=False,
@@ -43,15 +52,14 @@
     except KeyboardInterrupt:
         coiled.add_interaction(action="cli-setup-wizard:KeyboardInterrupt", success=False)
         return False
 
     coiled.add_interaction(action="cli-setup-wizard:prompt", success=True, choice=choice)
 
     if choice == "1":  # AWS
-        print("\nRunning [green]coiled setup aws[/green]\n")
         from .aws import do_setup
 
         try:
             return do_setup(slug="coiled")
         except Exception:
             setup_failure(f"Exception raised {traceback.format_exc()}", backend="aws")
             raise
```

### Comparing `coiled-0.8.9.dev9/coiled/cli/setup/gcp.py` & `coiled-0.9.0/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/cli/setup/prometheus.py` & `coiled-0.9.0/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/extensions/prefect/runners.py` & `coiled-0.9.0/coiled/extensions/prefect/runners.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/extensions/prefect/workers.py` & `coiled-0.9.0/coiled/extensions/prefect/workers.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/v2/__init__.py` & `coiled-0.9.0/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/v2/cluster.py` & `coiled-0.9.0/coiled/v2/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 from packaging.version import Version
 from rich.live import Live
 from rich.panel import Panel
 from rich.progress import BarColumn, Progress, TextColumn, TimeElapsedColumn
 from typing_extensions import Literal, TypeAlias
 from urllib3.util import parse_url
 
-from coiled import magic
+from coiled.capture_environment import ResolvedPackageInfo, create_environment_approximation
 from coiled.cluster import CoiledAdaptive, CredentialsPreferred
 from coiled.compatibility import DISTRIBUTED_VERSION
 from coiled.context import track_context
 from coiled.core import IsAsynchronous
 from coiled.errors import ClusterCreationError, DoesNotExist
 from coiled.exceptions import ArgumentCombinationError, InstanceTypeError
 from coiled.types import ArchitectureTypesEnum, AWSOptions, GCPOptions, PackageLevel, PackageLevelEnum
@@ -134,15 +134,15 @@
     worker_class
         Worker class to use. Defaults to :class:`distributed.nanny.Nanny`.
     worker_options
         Mapping with keyword arguments to pass to ``worker_class``. Defaults
         to ``{}``.
     worker_vm_types
         List of instance types that you would like workers to use, default instance type
-        selected contains 2 cores. You can use the command ``coiled.list_instance_types()``
+        selected contains 4 cores. You can use the command ``coiled.list_instance_types()``
         to see a list of allowed types.
     worker_cpu
         Number, or range, of CPUs requested for each worker. Specify a range by
         using a list of two elements, for example: ``worker_cpu=[2, 8]``.
     worker_memory
         Amount of memory to request for each worker, Coiled will use a +/- 10% buffer
         from the memory that you specify. You may specify a range of memory by using a
@@ -167,15 +167,15 @@
     scheduler_class
         Scheduler class to use. Defaults to :class:`distributed.scheduler.Scheduler`.
     scheduler_options
         Mapping with keyword arguments to pass to ``scheduler_class``. Defaults
         to ``{}``.
     scheduler_vm_types
         List of instance types that you would like the scheduler to use, default instances
-        type selected contains 2 cores. You can use the command
+        type selected contains 4 cores. You can use the command
         ``coiled.list_instance_types()`` to se a list of allowed types.
     scheduler_cpu
         Number, or range, of CPUs requested for the scheduler. Specify a range by
         using a list of two elements, for example: ``scheduler_cpu=[2, 8]``.
     scheduler_memory
         Amount of memory to request for the scheduler, Coiled will use a +/-10%
         buffer from the memory what you specify. You may specify a range of memory by using a
@@ -349,14 +349,15 @@
         package_sync_strict: bool = False,
         package_sync_ignore: Optional[List[str]] = None,
         package_sync_fail_on: Literal["critical-only", "warning-or-higher", "any"] = "critical-only",
         private_to_creator: Optional[bool] = None,
         use_best_zone: bool = True,
         compute_purchase_option: Optional[Literal["on-demand", "spot", "spot_with_fallback"]] = None,
         extra_worker_on_scheduler: Optional[bool] = None,
+        _n_worker_specs_per_host: Optional[int] = None,
         # easier network config
         scheduler_port: Optional[int] = None,
         allow_ingress_from: Optional[str] = None,
         allow_ssh: Optional[bool] = None,
         jupyter: Optional[bool] = None,
         region: Optional[str] = None,
         arm: Optional[bool] = None,
@@ -469,14 +470,16 @@
         # Set cluster attributes from kwargs (first choice) or dask config
 
         self.private_to_creator = (
             dask.config.get("coiled.private-to-creator") if private_to_creator is None else private_to_creator
         )
 
         self.extra_worker_on_scheduler = extra_worker_on_scheduler
+        self._worker_on_scheduler_name = None
+        self.n_worker_specs_per_host = _n_worker_specs_per_host
 
         # FIXME what happens when no kwargs passed but coiled.software is set in dask config?
         self.software_environment = software or dask.config.get("coiled.software")
         self.software_container = container
         if not container and not software and not package_sync:
             self.package_sync = True
 
@@ -558,15 +561,14 @@
         #
         # Some good places to learn about adaptive:
         # https://github.com/dask/distributed/blob/39024291e429d983d7b73064c209701b68f41f71/distributed/deploy/adaptive_core.py#L31-L43
         # https://github.com/dask/distributed/issues/5080
         self._requested: Set[str] = set()
         self._plan: Set[str] = set()
 
-        self._adaptive_options: Dict[str, Union[str, int]] = {}
         self.cluster_id: Optional[int] = None
         self.use_scheduler_public_ip: bool = (
             dask.config.get("coiled.use_scheduler_public_ip", True)
             if use_scheduler_public_ip is None
             else use_scheduler_public_ip
         )
         self.use_dashboard_https: bool = (
@@ -831,27 +833,27 @@
                 package_level_lookup = {
                     (pkg["name"], pkg["source"]): PackageLevelEnum(pkg["level"]) for pkg in package_levels
                 }
                 if self.package_sync_ignore:
                     for package in self.package_sync_ignore:
                         package_level_lookup[(package, "conda")] = PackageLevelEnum.IGNORE
                         package_level_lookup[(package, "pip")] = PackageLevelEnum.IGNORE
-                approximation = await magic.create_environment_approximation(
+                approximation = await create_environment_approximation(
                     cloud=self.cloud,
                     only=self.package_sync_only,
                     priorities=package_level_lookup,
                     strict=self.package_sync_strict,
                     progress=progress,
                     architecture=architecture,
                 )
 
                 if not self.package_sync_only:
                     # if we're not operating on a subset, check
                     # all the coiled defined critical packages are present
-                    packages_by_name: Dict[str, magic.ResolvedPackageInfo] = {p["name"]: p for p in approximation}
+                    packages_by_name: Dict[str, ResolvedPackageInfo] = {p["name"]: p for p in approximation}
                     self._check_halting_issues(package_levels, packages_by_name)
                 packages_with_errors = [
                     (
                         pkg,
                         package_level_lookup.get(
                             (
                                 (cast(str, pkg["conda_name"]) if pkg["source"] == "conda" else pkg["name"]),
@@ -883,46 +885,46 @@
                                 PackageLevelEnum.WARN,
                             )
                             > PackageLevelEnum.IGNORE
                         )
                     )
                 ]
                 for pkg_with_note in packages_with_notes:
-                    logger.info(f"Package - {pkg_with_note['name']}, {pkg_with_note['note']}")
+                    logger.debug(f"Package - {pkg_with_note['name']}, {pkg_with_note['note']}")
 
                 package_sync_env_alias = await self.cloud._create_package_sync_env(
                     packages=approximation,
                     account=self.account,
                     progress=progress,
                     gpu_enabled=gpu_enabled,
                     architecture=architecture,
                 )
                 package_sync_env = package_sync_env_alias["id"]
             if use_rich_widget() and self.show_widget:
                 from .widgets.rich import print_rich_package_table
 
                 print_rich_package_table(packages_with_notes, packages_with_errors)
 
-            logger.debug(f"Environment magic complete, {package_sync_env}")
+            logger.debug(f"Environment capture complete, {package_sync_env}")
         else:
             package_sync_env = None
 
         return package_sync_env
 
     @track_context
     def _check_halting_issues(
         self,
         package_levels: List[PackageLevel],
-        packages_by_name: Dict[str, magic.ResolvedPackageInfo],
+        packages_by_name: Dict[str, ResolvedPackageInfo],
     ):
         critical_packages = [pkg["name"] for pkg in package_levels if pkg["level"] == PackageLevelEnum.CRITICAL]
         halting_failures = []
         for critical_package in critical_packages:
             if critical_package not in packages_by_name:
-                problem: magic.ResolvedPackageInfo = {
+                problem: ResolvedPackageInfo = {
                     "name": critical_package,
                     "sdist": None,
                     "source": "pip",
                     "channel": None,
                     "conda_name": critical_package,
                     "client_version": "n/a",
                     "specifier": "n/a",
@@ -1176,14 +1178,15 @@
                     worker_vm_types=worker_vm_types_to_use,
                     backend_options=self.backend_options,
                     use_scheduler_public_ip=self.use_scheduler_public_ip,
                     use_dashboard_https=self.use_dashboard_https,
                     senv_v2_id=senv_v2_id,
                     private_to_creator=self.private_to_creator,
                     extra_worker_on_scheduler=self.extra_worker_on_scheduler,
+                    n_worker_specs_per_host=self.n_worker_specs_per_host,
                 )
                 cluster_created = not cluster_existed
 
             if not self.cluster_id:
                 raise RuntimeError(f"Failed to find/create cluster {self.name}")
 
             if cluster_created:
@@ -1193,15 +1196,14 @@
             else:
                 logger.info(f"Attaching to existing cluster (name: {self.name}, {self.details_url} )")
 
             await self._attach_to_cluster(is_new_cluster=cluster_created)
             await super()._start()
 
             # Set adaptive maximum value based on available config and user quota
-            self._set_adaptive_options()
         except Exception as e:
             if self._asynchronous:
                 did_error = True
                 asyncio.create_task(
                     self.cloud.add_interaction(
                         "cluster-create",
                         success=False,
@@ -1353,45 +1355,56 @@
                 self.errored_worker_count = sum(
                     [
                         1
                         for current in worker_current_states
                         if ProcessStateEnum(current["state"]) == ProcessStateEnum.error
                     ]
                 )
+                starting_workers = sum(
+                    [
+                        1
+                        for current in worker_current_states
+                        if ProcessStateEnum(current["state"])
+                        in [
+                            ProcessStateEnum.starting,
+                            ProcessStateEnum.pending,
+                        ]
+                    ]
+                )
 
                 if scheduler_state == ProcessStateEnum.started and scheduler_instance_state in [
                     InstanceStateEnum.ready,
                     InstanceStateEnum.started,
                 ]:
                     scheduler_ready = True
                     scheduler_reason_not_ready = ""
                 else:
                     scheduler_ready = False
                     scheduler_reason_not_ready = "Scheduler not ready."
 
                 n_workers_ready = len(ready_worker_current)
+
                 final_update = None
                 if n_workers_ready >= num_workers_to_wait_for:
                     if n_workers_ready == self._start_n_workers:
                         final_update = "All workers ready."
                     else:
                         final_update = "Most of your workers have arrived. Cluster ready for use."
 
-                    workers_ready = True
+                    enough_workers_ready = True
                     workers_reason_not_ready = ""
-
                 else:
-                    workers_ready = False
+                    enough_workers_ready = False
                     workers_reason_not_ready = (
                         f"Only {len(ready_worker_current)} workers ready "
                         f"(was waiting for at least {num_workers_to_wait_for}). "
                     )
-                # TODO -- if all workers are ready *or error* then give final update
 
-                if scheduler_ready and workers_ready:
+                # Check if cluster is ready to return to user in a good state
+                if scheduler_ready and enough_workers_ready:
                     assert final_update is not None
                     if widget:
                         widget.update(
                             cluster_details,
                             self._cluster_status_logs,
                             final_update=final_update,
                         )
@@ -1414,39 +1427,52 @@
                         logger.debug(summarize_status(cluster_details))
                         raise ClusterCreationError(
                             error,
                             cluster_id=self.cluster_id,
                         )
                     elif cluster_state == ClusterStateEnum.ready:
                         # (cluster state "ready" means all worked either started or errored, so
-                        # this cluster will ever have all the workers we want)
+                        # this cluster will never have all the workers we want)
                         if widget:
                             widget.update(
                                 cluster_details,
                                 self._cluster_status_logs,
                                 final_update=reason_not_ready,
                             )
                         logger.debug(summarize_status(cluster_details))
                         raise ClusterCreationError(
                             reason_not_ready,
                             cluster_id=self.cluster_id,
                         )
+                    elif (starting_workers + n_workers_ready) < num_workers_to_wait_for:
+                        # including workers that are starting, cluster cannot get to the number
+                        # of desired ready workers (because some workers have already errored),
+                        logger.debug(summarize_status(cluster_details))
+                        raise ClusterCreationError(
+                            f"The Cluster was waiting for {num_workers_to_wait_for} workers."
+                            f"Because {self.errored_worker_count} workers have already failed, "
+                            "this cluster cannot get to the desired number of workers. "
+                            f"({n_workers_ready} are ready and {starting_workers} are still starting). "
+                            "Try adjusting the wait_for_workers argument if fewer workers is acceptable.",
+                            cluster_id=self.cluster_id,
+                        )
                     elif timeout_at is not None and datetime.datetime.now() > timeout_at:
                         error = "User-specified timeout expired: " + reason_not_ready
                         if widget:
                             widget.update(
                                 cluster_details,
                                 self._cluster_status_logs,
                                 final_update=error,
                             )
                         logger.debug(summarize_status(cluster_details))
                         raise ClusterCreationError(
                             error,
                             cluster_id=self.cluster_id,
                         )
+
                     else:
                         await asyncio.sleep(1.0)
 
     async def _update_cluster_status_logs(self):
         cluster_id = self._assert_cluster_id()
         states_by_type = await self.cloud._get_cluster_states_declarative(
             cluster_id, self.account, start_time=self._latest_dt_seen
@@ -1490,32 +1516,46 @@
         assert self.account
         assert self.cluster_id
         eventually_maybe_good_workers = await self.cloud._get_worker_names(
             account=self.account,
             cluster_id=self.cluster_id,
             statuses=eventually_maybe_good_statuses,
         )
+
+        # scale (including adaptive) relies on `plan` and `requested` and these (on Coiled)
+        # are set based on the control-plane's view of what workers there are, so if we have
+        # extra worker on the scheduler (which isn't tracked separately by control-plane)
+        # we need to include that here.
+        if self.extra_worker_on_scheduler:
+            # get the actual name of worker on scheduler if we haven't gotten it yet
+            if not self._worker_on_scheduler_name:
+                worker_on_scheduler = [worker for worker in self.observed if "scheduler" in worker]
+                if worker_on_scheduler:
+                    self._worker_on_scheduler_name = worker_on_scheduler[0]
+            # if we have actual name, use it, otherwise use fake name for now
+            if self._worker_on_scheduler_name:
+                eventually_maybe_good_workers.add(self._worker_on_scheduler_name)
+            else:
+                eventually_maybe_good_workers.add("extra-worker-on-scheduler")
+
         self._plan = eventually_maybe_good_workers
         self._requested = eventually_maybe_good_workers
 
     @track_context
     async def _scale(self, n: int) -> None:
-        await self._set_plan_requested()  # need to update our understanding of current workers before scaling
-        logger.debug(f"current _plan: {self._plan}")
         if not self.cluster_id:
             raise ValueError("No cluster available to scale!")
+
+        await self._set_plan_requested()  # need to update our understanding of current workers before scaling
+        logger.debug(f"current _plan: {self._plan}")
+
         recommendations = await self.recommendations(n)
-        logger.debug(f"scale recommmendations: {recommendations}")
-        status = recommendations.pop("status")
-        if status == "same":
-            return
-        if status == "up":
-            return await self.scale_up(**recommendations)
-        if status == "down":
-            return await self.scale_down(**recommendations)
+        logger.debug(f"scale recommendations: {recommendations}")
+
+        return await self._apply_scaling_recommendations(recommendations)
 
     @track_context
     async def scale_up(self, n: int, reason: Optional[str] = None) -> None:
         """
         Scales up *to* a target number of ``n`` workers
 
         It's documented that scale_up should scale up to a certain target, not scale up BY a certain amount:
@@ -1531,27 +1571,14 @@
             n=target,
             reason=reason,
         )
         if response:
             self._plan.update(set(response.get("workers", [])))
             self._requested.update(set(response.get("workers", [])))
 
-    def _set_adaptive_options(self, **kwargs):
-        # legacy version got dict with data about account limit and worker size
-        # and then used that to determine maximum size for adaptive scaling
-        self._adaptive_options = {
-            "interval": "5s",
-            "wait_count": 12,
-            "target_duration": "5m",
-            "minimum": 1,
-            # TODO: want a more sensible limit; see _set_adaptive_options in coiled.Cluster
-            # for inspiration from the logic there
-            "maximum": 200,
-        }
-
     @track_context
     async def _close(self, force_shutdown: bool = False) -> None:
         # My small changes to _close probably make sense for legacy Cluster too, but I don't want to carefully
         # test them, so copying this method over.
 
         with suppress(AttributeError):
             self._adaptive.stop()  # type: ignore
@@ -1650,30 +1677,38 @@
                 raise TimeoutError(err_msg)
             await asyncio.sleep(1)
 
     @staticmethod
     def _sync_get_aws_local_session_token(
         duration_seconds: Optional[int] = None,
     ) -> AWSSessionCredentials:
-        token_creds = AWSSessionCredentials(AccessKeyId="", SecretAccessKey="", SessionToken=None, Expiration=None)
+        token_creds = AWSSessionCredentials(
+            AccessKeyId="",
+            SecretAccessKey="",
+            SessionToken=None,
+            Expiration=None,
+            DefaultRegion=None,
+        )
         try:
             from boto3.session import Session
 
             session = Session()
+
             sts = session.client("sts")
             try:
                 kwargs = {"DurationSeconds": duration_seconds} if duration_seconds else {}
                 credentials = sts.get_session_token(**kwargs)
 
                 credentials = credentials["Credentials"]
                 token_creds = AWSSessionCredentials(
                     AccessKeyId=credentials.get("AccessKeyId", ""),
                     SecretAccessKey=credentials.get("SecretAccessKey", ""),
                     SessionToken=credentials.get("SessionToken"),
                     Expiration=credentials.get("Expiration"),
+                    DefaultRegion=session.region_name,
                 )
             except botocore.errorfactory.ClientError as e:
                 if "session credentials" in str(e):
                     # Credentials are already an STS token, which gives us this error:
                     # > Cannot call GetSessionToken with session credentials
                     # In this case we'll just use the existing STS token for the active, local session.
                     # Note that in some cases this will have a shorter TTL than the default 12 hour tokens.
@@ -1688,14 +1723,15 @@
                     )
 
                     token_creds = AWSSessionCredentials(
                         AccessKeyId=frozen_creds.access_key,
                         SecretAccessKey=frozen_creds.secret_key,
                         SessionToken=frozen_creds.token,
                         Expiration=expiration,
+                        DefaultRegion=session.region_name,
                     )
 
         except (
             botocore.exceptions.ProfileNotFound,
             botocore.exceptions.NoCredentialsError,
         ):
             # no AWS credentials (maybe not running against AWS?), fail gracefully
@@ -1725,15 +1761,15 @@
         Manually trigger sending STS token to cluster.
 
         Usually STS token is automatically sent and refreshed by default, this allows
         you to manually force a refresh in case that's needed for any reason.
         """
         return self.sync(self._send_credentials, schedule_callback=automatic_refresh)
 
-    async def _send_credentials(self, schedule_callback: bool = True):
+    async def _send_credentials(self, schedule_callback: bool = True, retries=5):
         """
         Get credentials and pass them to the scheduler.
         """
         if self.credentials is not CredentialsPreferred.NONE:
             try:
                 if self.credentials is CredentialsPreferred.ACCOUNT:
                     # cloud.get_aws_credentials doesn't return credentials for currently implemented backends
@@ -1752,14 +1788,15 @@
                     await scheduler_comm.aws_update_credentials(
                         credentials={
                             k: token_creds.get(k)
                             for k in [
                                 "AccessKeyId",
                                 "SecretAccessKey",
                                 "SessionToken",
+                                "DefaultRegion",
                             ]
                         }
                     )
 
                     if schedule_callback:
                         # schedule callback for updating creds before they expire
 
@@ -1804,16 +1841,22 @@
                 terminating_states = (
                     Status.closing,
                     Status.closed,
                     Status.closing_gracefully,
                     Status.failed,
                 )
                 if self.status not in terminating_states:
-                    # warn, but don't crash
-                    logger.warning(f"error sending AWS credentials to cluster: {e}")
+                    # sending credentials sometimes fails on a poor internet connection
+                    # so try a few times before giving up and showing warning
+                    if retries > 0:
+                        await self._send_credentials(schedule_callback, retries=retries - 1)
+                    else:
+                        # no more retries!
+                        # warn, but don't crash
+                        logger.warning(f"error sending AWS credentials to cluster: {e}")
 
     def __await__(self: Cluster[Async]):
         async def _():
             if self._lock is None:
                 self._lock = asyncio.Lock()
             async with self._lock:
                 if self.status == Status.created:
@@ -1891,36 +1934,58 @@
             reason=reason,
         )
         self._plan.difference_update(workers)
         self._requested.difference_update(workers)
 
     async def recommendations(self, target: int) -> dict:
         """
-        Make scale up/down recommendations based on current state and target
+        Make scale up/down recommendations based on current state and target.
+
+        Return a recommendation of the form
+        - {"status": "same"}
+        - {"status": "up", "n": <desired number of total workers>}
+        - {"status": "down", "workers": <list of workers to close>}
         """
+        # note that `Adaptive` has a `recommendations()` method, but (as far as I can tell) it doesn't
+        # appear that adaptive every calls `cluster.recommendations()`, so this appears to only be used
+        # from `cluster.scale()`
         plan = self.plan
         requested = self.requested
         observed = self.observed
 
-        if target == len(plan):
+        n_current_or_expected = len(plan)
+
+        if target == n_current_or_expected:
             return {"status": "same"}
 
-        if target > len(plan):
+        if target > n_current_or_expected:
             return {"status": "up", "n": target}
 
+        # when scaling down, prefer workers that haven't yet connected to scheduler
+        # for this to work, the worker name known by scheduler needs to match worker name in database
         not_yet_arrived = requested - observed
         to_close = set()
         if not_yet_arrived:
-            to_close.update(islice(not_yet_arrived, len(plan) - target))
+            to_close.update(islice(not_yet_arrived, n_current_or_expected - target))
 
-        if target < len(plan) - len(to_close):
+        if target < n_current_or_expected - len(to_close):
             L = await self.workers_to_close(target=target)
             to_close.update(L)
         return {"status": "down", "workers": list(to_close)}
 
+    async def _apply_scaling_recommendations(self, recommendations: dict):
+        # structure of `recommendations` matches output of `self.recommendations()`
+        status = recommendations.pop("status")
+        if status == "same":
+            return
+        if status == "up":
+            return await self.scale_up(**recommendations)
+        if status == "down":
+            return await self.scale_down(**recommendations)
+
     async def workers_to_close(self, target: int) -> List[str]:
         """
         Determine which, if any, workers should potentially be removed from
         the cluster.
 
         Notes
         -----
@@ -1955,40 +2020,55 @@
             # worker-on-scheduler was in the list), we need only return the desired number (in case
             # extra worker-on-scheduler was *not* in the list of workers to kill).
             desired_workers = len(workers) - target_offset
             return list(filter(lambda name: "scheduler" not in name, workers))[:desired_workers]
 
         return workers  # type: ignore
 
-    def adapt(self, Adaptive=CoiledAdaptive, **kwargs) -> Adaptive:
+    def adapt(
+        self,
+        Adaptive=CoiledAdaptive,
+        *,
+        minimum=1,
+        maximum=200,
+        target_duration="5m",
+        wait_count=24,
+        interval="5s",
+        **kwargs,
+    ) -> Adaptive:
         """Dynamically scale the number of workers in the cluster
         based on scaling heuristics.
 
         Parameters
         ----------
         minimum : int
             Minimum number of workers that the cluster should have while
             on low load, defaults to 1.
         maximum : int
             Maximum numbers of workers that the cluster should have while
             on high load.
         wait_count : int
             Number of consecutive times that a worker should be suggested
-            for removal before the cluster removes it, defaults to 60.
+            for removal before the cluster removes it.
         interval : timedelta or str
             Milliseconds between checks, defaults to 5000 ms.
         target_duration : timedelta or str
             Amount of time we want a computation to take. This affects how
-            aggressively the cluster scales up, defaults to 5s.
+            aggressively the cluster scales up.
 
         """
-        maximum = kwargs.pop("maximum", None)
-        if maximum is not None:
-            kwargs["maximum"] = maximum
-        return super().adapt(Adaptive=Adaptive, **kwargs)
+        return super().adapt(
+            Adaptive=Adaptive,
+            minimum=minimum,
+            maximum=maximum,
+            target_duration=target_duration,
+            wait_count=wait_count,
+            interval=interval,
+            **kwargs,
+        )
 
     def __enter__(self: Cluster[Sync]) -> Cluster[Sync]:
         return self.sync(self.__aenter__)
 
     def __exit__(self: Cluster[Sync], *args, **kwargs) -> None:
         return self.sync(self.__aexit__, *args, **kwargs)
```

### Comparing `coiled-0.8.9.dev9/coiled/v2/core.py` & `coiled-0.9.0/coiled/v2/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,15 +552,15 @@
         return result
 
     @track_context
     async def _create_senv_package(
         self, package_file: BinaryIO, contents_md5: str, account: Optional[str] = None
     ) -> int:
         package_name = Path(package_file.name).name
-        logger.info(f"Starting upload for {package_name}")
+        logger.debug(f"Starting upload for {package_name}")
         package_data = package_file.read()
         # s3 expects the md5 to be base64 encoded
         wheel_md5 = base64.b64encode(md5(package_data).digest()).decode("utf-8")
         account = account or self.default_account
 
         response = await self._do_request(
             "POST",
@@ -621,14 +621,15 @@
         worker_disk_size: Optional[int] = None,
         worker_disk_throughput: Optional[int] = None,
         backend_options: Optional[Union[AWSOptions, GCPOptions, dict]] = None,
         use_scheduler_public_ip: Optional[bool] = None,
         use_dashboard_https: Optional[bool] = None,
         private_to_creator: Optional[bool] = None,
         extra_worker_on_scheduler: Optional[bool] = None,
+        n_worker_specs_per_host: Optional[int] = None,
     ) -> Tuple[int, bool]:
         # TODO (Declarative): support these args, or decide not to
         # https://gitlab.com/coiled/cloud/-/issues/4305
 
         if scheduler_class is not None:
             raise ValueError("scheduler_class is not supported in beta/new Coiled yet")
 
@@ -654,14 +655,15 @@
             "environ": environ,
             "tags": tags,
             "dask_config": dask_config,
             "private_to_creator": private_to_creator,
             "env_id": senv_v2_id,
             "env_name": software_environment,
             "extra_worker_on_scheduler": extra_worker_on_scheduler,
+            "n_worker_specs_per_host": n_worker_specs_per_host,
             # "jupyter_on_scheduler": True,
         }
 
         backend_options = backend_options if backend_options else {}
 
         if gcp_worker_gpu_type is not None:
             # for backwards compatibility with v1 options
```

### Comparing `coiled-0.8.9.dev9/coiled/v2/cwi_log_link.py` & `coiled-0.9.0/coiled/v2/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/v2/states.py` & `coiled-0.9.0/coiled/v2/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/v2/widgets/__init__.py` & `coiled-0.9.0/coiled/v2/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/coiled/v2/widgets/rich.py` & `coiled-0.9.0/coiled/v2/widgets/rich.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 import rich.live
 import rich.panel
 import rich.progress
 import rich.table
 
 from coiled.types import PackageLevelEnum
 
+from ...capture_environment import ResolvedPackageInfo
 from ...errors import ClusterCreationError
-from ...magic import ResolvedPackageInfo
 from ...utils import get_details_url
 from ..states import CombinedProcessStateEnum, ProcessStateEnum
 from . import EXECUTION_CONTEXT
 from .util import get_instance_types, get_worker_statuses
 
 LOCAL_TIMEZONE = datetime.datetime.now(datetime.timezone.utc).astimezone().tzinfo
```

### Comparing `coiled-0.8.9.dev9/coiled/v2/widgets/util.py` & `coiled-0.9.0/coiled/v2/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/README.md` & `coiled-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.8.9.dev9/pyproject.toml` & `coiled-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     "aiohttp",
     "backoff",
     "boto3",
     "click>=7.1",
     "dask>=2.23.0",
     "distributed>=2.23.0",
     "filelock",
+    "gilknocker>=0.4.1",
     "importlib-metadata",
     "ipywidgets",
     "jmespath",
     "jsondiff",
     "packaging",
     "pip",
     "pip>=19.3",
```

### Comparing `coiled-0.8.9.dev9/PKG-INFO` & `coiled-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.8.9.dev9
+Version: 0.9.0
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
 Requires-Dist: click>=7.1
 Requires-Dist: dask>=2.23.0
 Requires-Dist: distributed>=2.23.0
 Requires-Dist: filelock
+Requires-Dist: gilknocker>=0.4.1
 Requires-Dist: importlib-metadata
 Requires-Dist: ipywidgets
 Requires-Dist: jmespath
 Requires-Dist: jsondiff
 Requires-Dist: packaging
 Requires-Dist: pip
 Requires-Dist: pip>=19.3
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.8.9.dev9 Project-URL: Homepage,
-https://coiled.io Maintainer-email: Coiled
+Metadata-Version: 2.1 Name: coiled Version: 0.9.0 Project-URL: Homepage, https:
+//coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
-Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
-jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
-Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
-rich>=11.2.0 Requires-Dist: setuptools>=49.3.0 Requires-Dist: typing-extensions
-Requires-Dist: wheel Description-Content-Type: text/markdown
+Requires-Dist: gilknocker>=0.4.1 Requires-Dist: importlib-metadata Requires-
+Dist: ipywidgets Requires-Dist: jmespath Requires-Dist: jsondiff Requires-Dist:
+packaging Requires-Dist: pip Requires-Dist: pip>=19.3 Requires-Dist:
+prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist: setuptools>=49.3.0
+Requires-Dist: typing-extensions Requires-Dist: wheel Description-Content-Type:
+text/markdown
                                    [Coiled]
              Coiled.io â¢ Documentation â¢ Community â¢ Support
 Coiled is a deployment-as-a-service library for scaling Python with Dask, a
 popular open source library for parallel analytics. Coiled manages cloud
 resources, networking, software environments, and everything you need to scale
 Python in the cloud robustly and easily. Go to https://cloud.coiled.io to get
 started with Coiled.
```

