# Comparing `tmp/modflow-devtools-0.1.8.tar.gz` & `tmp/modflow-devtools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modflow-devtools-0.1.8.tar", last modified: Fri Apr 21 19:45:24 2023, max compression
+gzip compressed data, was "modflow-devtools-0.2.0.tar", last modified: Wed Jul 26 22:03:12 2023, max compression
```

## Comparing `modflow-devtools-0.1.8.tar` & `modflow-devtools-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-04-21 19:45:24.210920 modflow-devtools-0.1.8/
--rwxr-xr-x   0 wes        (501) staff       (20)     1627 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/LICENSE.md
--rw-r--r--   0 wes        (501) staff       (20)      163 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/MANIFEST.in
--rw-r--r--   0 wes        (501) staff       (20)     5069 2023-04-21 19:45:24.210424 modflow-devtools-0.1.8/PKG-INFO
--rw-r--r--   0 wes        (501) staff       (20)     3856 2023-04-18 20:59:23.000000 modflow-devtools-0.1.8/README.md
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-04-21 19:45:24.165680 modflow-devtools-0.1.8/modflow_devtools/
--rw-r--r--   0 wes        (501) staff       (20)      248 2023-04-21 13:48:06.000000 modflow-devtools-0.1.8/modflow_devtools/__init__.py
--rw-r--r--   0 wes        (501) staff       (20)      984 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/build.py
--rw-r--r--   0 wes        (501) staff       (20)     1029 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/case.py
--rw-r--r--   0 wes        (501) staff       (20)     7352 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/context.py
--rw-r--r--   0 wes        (501) staff       (20)    17531 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/download.py
--rw-r--r--   0 wes        (501) staff       (20)     2487 2023-04-18 20:59:23.000000 modflow-devtools-0.1.8/modflow_devtools/executables.py
--rw-r--r--   0 wes        (501) staff       (20)    11854 2023-04-21 19:36:54.000000 modflow-devtools-0.1.8/modflow_devtools/fixtures.py
--rw-r--r--   0 wes        (501) staff       (20)     1732 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/markers.py
--rw-r--r--   0 wes        (501) staff       (20)    10007 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/misc.py
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-04-21 19:45:24.207602 modflow-devtools-0.1.8/modflow_devtools/test/
--rw-r--r--   0 wes        (501) staff       (20)        0 2022-11-03 17:55:40.000000 modflow-devtools-0.1.8/modflow_devtools/test/__init__.py
--rw-r--r--   0 wes        (501) staff       (20)     1163 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_build.py
--rw-r--r--   0 wes        (501) staff       (20)     1788 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_case.py
--rw-r--r--   0 wes        (501) staff       (20)     3606 2023-04-21 19:36:54.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_download.py
--rw-r--r--   0 wes        (501) staff       (20)     1148 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_executables.py
--rw-r--r--   0 wes        (501) staff       (20)     8043 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_fixtures.py
--rw-r--r--   0 wes        (501) staff       (20)      904 2022-11-03 18:33:54.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_markers.py
--rw-r--r--   0 wes        (501) staff       (20)     8053 2023-04-21 16:21:19.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_misc.py
--rw-r--r--   0 wes        (501) staff       (20)     2663 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_zip.py
--rw-r--r--   0 wes        (501) staff       (20)     5708 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/zip.py
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-04-21 19:45:24.171718 modflow-devtools-0.1.8/modflow_devtools.egg-info/
--rw-r--r--   0 wes        (501) staff       (20)     5069 2023-04-21 19:45:24.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/PKG-INFO
--rw-r--r--   0 wes        (501) staff       (20)      913 2023-04-21 19:45:24.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/SOURCES.txt
--rw-r--r--   0 wes        (501) staff       (20)        1 2023-04-21 19:45:24.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/dependency_links.txt
--rw-r--r--   0 wes        (501) staff       (20)        1 2022-07-22 15:19:26.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/not-zip-safe
--rw-r--r--   0 wes        (501) staff       (20)      235 2023-04-21 19:45:24.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/requires.txt
--rw-r--r--   0 wes        (501) staff       (20)       17 2023-04-21 19:45:24.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/top_level.txt
--rw-r--r--   0 wes        (501) staff       (20)     2182 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/pyproject.toml
--rw-r--r--   0 wes        (501) staff       (20)       38 2023-04-21 19:45:24.211042 modflow-devtools-0.1.8/setup.cfg
--rwxr-xr-x   0 wes        (501) staff       (20)       61 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/setup.py
--rw-r--r--   0 wes        (501) staff       (20)        5 2023-04-21 13:48:06.000000 modflow-devtools-0.1.8/version.txt
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-07-26 22:03:12.090946 modflow-devtools-0.2.0/
+-rwxr-xr-x   0 wes        (501) staff       (20)     1627 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/LICENSE.md
+-rw-r--r--   0 wes        (501) staff       (20)      163 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/MANIFEST.in
+-rw-r--r--   0 wes        (501) staff       (20)     5069 2023-07-26 22:03:12.089895 modflow-devtools-0.2.0/PKG-INFO
+-rw-r--r--   0 wes        (501) staff       (20)     3856 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/README.md
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-07-26 22:03:12.074693 modflow-devtools-0.2.0/modflow_devtools/
+-rw-r--r--   0 wes        (501) staff       (20)      248 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/__init__.py
+-rw-r--r--   0 wes        (501) staff       (20)      984 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/build.py
+-rw-r--r--   0 wes        (501) staff       (20)     1029 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/case.py
+-rw-r--r--   0 wes        (501) staff       (20)     7352 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/context.py
+-rw-r--r--   0 wes        (501) staff       (20)    17531 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/download.py
+-rw-r--r--   0 wes        (501) staff       (20)     2487 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/executables.py
+-rw-r--r--   0 wes        (501) staff       (20)    11854 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/fixtures.py
+-rw-r--r--   0 wes        (501) staff       (20)     1732 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/markers.py
+-rw-r--r--   0 wes        (501) staff       (20)    11069 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/misc.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-07-26 22:03:12.089158 modflow-devtools-0.2.0/modflow_devtools/test/
+-rw-r--r--   0 wes        (501) staff       (20)        0 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/test/__init__.py
+-rw-r--r--   0 wes        (501) staff       (20)     1163 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_build.py
+-rw-r--r--   0 wes        (501) staff       (20)     1788 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_case.py
+-rw-r--r--   0 wes        (501) staff       (20)     3606 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_download.py
+-rw-r--r--   0 wes        (501) staff       (20)     1148 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_executables.py
+-rw-r--r--   0 wes        (501) staff       (20)     8043 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_fixtures.py
+-rw-r--r--   0 wes        (501) staff       (20)      904 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_markers.py
+-rw-r--r--   0 wes        (501) staff       (20)     8476 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_misc.py
+-rw-r--r--   0 wes        (501) staff       (20)     2663 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_zip.py
+-rw-r--r--   0 wes        (501) staff       (20)     5708 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/zip.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-07-26 22:03:12.079378 modflow-devtools-0.2.0/modflow_devtools.egg-info/
+-rw-r--r--   0 wes        (501) staff       (20)     5069 2023-07-26 22:03:12.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/PKG-INFO
+-rw-r--r--   0 wes        (501) staff       (20)      913 2023-07-26 22:03:12.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/SOURCES.txt
+-rw-r--r--   0 wes        (501) staff       (20)        1 2023-07-26 22:03:12.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/dependency_links.txt
+-rw-r--r--   0 wes        (501) staff       (20)        1 2022-07-22 15:19:26.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/not-zip-safe
+-rw-r--r--   0 wes        (501) staff       (20)      235 2023-07-26 22:03:12.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/requires.txt
+-rw-r--r--   0 wes        (501) staff       (20)       17 2023-07-26 22:03:12.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/top_level.txt
+-rw-r--r--   0 wes        (501) staff       (20)     2182 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/pyproject.toml
+-rw-r--r--   0 wes        (501) staff       (20)       38 2023-07-26 22:03:12.091570 modflow-devtools-0.2.0/setup.cfg
+-rwxr-xr-x   0 wes        (501) staff       (20)       61 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/setup.py
+-rw-r--r--   0 wes        (501) staff       (20)        5 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/version.txt
```

### Comparing `modflow-devtools-0.1.8/LICENSE.md` & `modflow-devtools-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/PKG-INFO` & `modflow-devtools-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 0.1.8
+Version: 0.2.0
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
```

### Comparing `modflow-devtools-0.1.8/README.md` & `modflow-devtools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/build.py` & `modflow-devtools-0.2.0/modflow_devtools/build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/case.py` & `modflow-devtools-0.2.0/modflow_devtools/case.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/context.py` & `modflow-devtools-0.2.0/modflow_devtools/context.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/download.py` & `modflow-devtools-0.2.0/modflow_devtools/download.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/executables.py` & `modflow-devtools-0.2.0/modflow_devtools/executables.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/fixtures.py` & `modflow-devtools-0.2.0/modflow_devtools/fixtures.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/markers.py` & `modflow-devtools-0.2.0/modflow_devtools/markers.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/misc.py` & `modflow-devtools-0.2.0/modflow_devtools/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,47 @@
         print(f"Changed to working directory: {wrkdir} (previously: {origin})")
         yield
     finally:
         chdir(origin)
         print(f"Returned to previous directory: {origin}")
 
 
+@contextmanager
+def set_env(*remove, **update):
+    """
+    Temporarily updates the ``os.environ`` dictionary in-place.
+
+    Referenced from https://stackoverflow.com/a/34333710/6514033.
+
+    The ``os.environ`` dictionary is updated in-place so that the modification
+    is sure to work in all situations.
+
+    :param remove: Environment variables to remove.
+    :param update: Dictionary of environment variables and values to add/update.
+    """
+    env = environ
+    update = update or {}
+    remove = remove or []
+
+    # List of environment variables being updated or removed.
+    stomped = (set(update.keys()) | set(remove)) & set(env.keys())
+    # Environment variables and values to restore on exit.
+    update_after = {k: env[k] for k in stomped}
+    # Environment variables and values to remove on exit.
+    remove_after = frozenset(k for k in update if k not in env)
+
+    try:
+        env.update(update)
+        [env.pop(k, None) for k in remove]
+        yield
+    finally:
+        env.update(update_after)
+        [env.pop(k) for k in remove_after]
+
+
 class add_sys_path:
     """
     Context manager for temporarily editing the system path
     (https://stackoverflow.com/a/39855753/6514033)
     """
 
     def __init__(self, path):
```

### Comparing `modflow-devtools-0.1.8/modflow_devtools/test/test_build.py` & `modflow-devtools-0.2.0/modflow_devtools/test/test_build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/test/test_case.py` & `modflow-devtools-0.2.0/modflow_devtools/test/test_case.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/test/test_download.py` & `modflow-devtools-0.2.0/modflow_devtools/test/test_download.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/test/test_executables.py` & `modflow-devtools-0.2.0/modflow_devtools/test/test_executables.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/test/test_fixtures.py` & `modflow-devtools-0.2.0/modflow_devtools/test/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/test/test_markers.py` & `modflow-devtools-0.2.0/modflow_devtools/test/test_markers.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/test/test_misc.py` & `modflow-devtools-0.2.0/modflow_devtools/test/test_misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,41 @@
 import pytest
 from modflow_devtools.misc import (
     get_model_paths,
     get_namefile_paths,
     get_packages,
     has_package,
     set_dir,
+    set_env,
 )
 
 
 def test_set_dir(tmp_path):
     assert Path(os.getcwd()) != tmp_path
     with set_dir(tmp_path):
         assert Path(os.getcwd()) == tmp_path
     assert Path(os.getcwd()) != tmp_path
 
 
+def test_set_env(tmp_path):
+    # test adding a variable
+    key = "TEST_ENV"
+    val = "test"
+    assert environ.get(key) is None
+    with set_env(**{key: val}):
+        assert environ.get(key) == val
+    with set_env(TEST_ENV=val):
+        assert environ.get(key) == val
+
+    # test removing a variable
+    with set_env(**{key: val}):
+        with set_env(key):
+            assert environ.get(key) is None
+
+
 _repos_path = environ.get("REPOS_PATH")
 if _repos_path is None:
     _repos_path = Path(__file__).parent.parent.parent.parent
 _repos_path = Path(_repos_path).expanduser().absolute()
 _testmodels_repo_path = _repos_path / "modflow6-testmodels"
 _testmodels_repo_paths_mf6 = sorted(
     list((_testmodels_repo_path / "mf6").glob("test*"))
@@ -163,15 +180,15 @@
 )
 @pytest.mark.parametrize(
     "models", [(_examples_path, 63), (_largetestmodels_repo_path, 16)]
 )
 def test_get_model_paths_exclude_patterns(models):
     path, expected_count = models
     paths = get_model_paths(path, excluded=["gwt"])
-    assert len(paths) == expected_count
+    assert len(paths) >= expected_count
 
 
 @pytest.mark.skipif(
     not any(_example_paths), reason="modflow6-examples repo not found"
 )
 def test_get_namefile_paths_examples():
     expected_paths = get_expected_namefiles(_examples_path)
@@ -206,29 +223,29 @@
 )
 @pytest.mark.parametrize(
     "models", [(_examples_path, 43), (_largetestmodels_repo_path, 19)]
 )
 def test_get_namefile_paths_exclude_patterns(models):
     path, expected_count = models
     paths = get_namefile_paths(path, excluded=["gwf"])
-    assert len(paths) == expected_count
+    assert len(paths) >= expected_count
 
 
 @pytest.mark.skipif(not any(_example_paths), reason="examples not found")
 def test_get_namefile_paths_select_prefix():
     paths = get_namefile_paths(_examples_path, prefix="ex2")
     assert not any(paths)
 
     paths = get_namefile_paths(_examples_path, prefix="ex")
     assert any(paths)
 
 
 @pytest.mark.skipif(not any(_example_paths), reason="examples not found")
 def test_get_namefile_paths_select_patterns():
     paths = get_namefile_paths(_examples_path, selected=["gwf"])
-    assert len(paths) == 70
+    assert len(paths) >= 70
 
 
 @pytest.mark.skipif(not any(_example_paths), reason="examples not found")
 def test_get_namefile_paths_select_packages():
     paths = get_namefile_paths(_examples_path, packages=["wel"])
-    assert len(paths) == 43
+    assert len(paths) >= 43
```

### Comparing `modflow-devtools-0.1.8/modflow_devtools/test/test_zip.py` & `modflow-devtools-0.2.0/modflow_devtools/test/test_zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools/zip.py` & `modflow-devtools-0.2.0/modflow_devtools/zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/modflow_devtools.egg-info/PKG-INFO` & `modflow-devtools-0.2.0/modflow_devtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 0.1.8
+Version: 0.2.0
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
```

### Comparing `modflow-devtools-0.1.8/modflow_devtools.egg-info/SOURCES.txt` & `modflow-devtools-0.2.0/modflow_devtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.8/pyproject.toml` & `modflow-devtools-0.2.0/pyproject.toml`

 * *Files identical despite different names*

