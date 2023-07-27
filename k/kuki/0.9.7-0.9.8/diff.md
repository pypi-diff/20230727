# Comparing `tmp/kuki-0.9.7.tar.gz` & `tmp/kuki-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuki-0.9.7.tar", last modified: Tue Jul 25 13:38:34 2023, max compression
+gzip compressed data, was "kuki-0.9.8.tar", last modified: Thu Jul 27 15:27:28 2023, max compression
```

## Comparing `kuki-0.9.7.tar` & `kuki-0.9.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-25 13:38:34.471388 kuki-0.9.7/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.9.7/LICENSE
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-25 13:38:34.471388 kuki-0.9.7/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      459 2023-07-20 14:47:33.000000 kuki-0.9.7/README.md
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-25 13:38:34.469388 kuki-0.9.7/kuki/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.9.7/kuki/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1176 2023-05-20 06:39:32.000000 kuki-0.9.7/kuki/config_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1375 2023-07-23 05:45:31.000000 kuki-0.9.7/kuki/kest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1994 2023-07-19 16:18:20.000000 kuki-0.9.7/kuki/ktrl.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4652 2023-07-22 06:51:24.000000 kuki-0.9.7/kuki/ktrl_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4577 2023-07-22 07:28:15.000000 kuki-0.9.7/kuki/kuki.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4087 2023-07-23 15:13:37.000000 kuki-0.9.7/kuki/package_util.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-25 13:38:34.471388 kuki-0.9.7/kuki/q/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.9.7/kuki/q/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-03 16:51:49.000000 kuki-0.9.7/kuki/q/cli.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     7819 2023-07-15 09:03:13.000000 kuki-0.9.7/kuki/q/kest.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      219 2023-07-19 16:35:57.000000 kuki-0.9.7/kuki/q/ktrl.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1913 2023-07-22 16:08:18.000000 kuki-0.9.7/kuki/q/kuki.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2187 2023-07-20 15:49:50.000000 kuki-0.9.7/kuki/q/log.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1435 2023-07-15 14:20:22.000000 kuki-0.9.7/kuki/q/path.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    18554 2023-07-25 13:34:57.000000 kuki-0.9.7/kuki/registry_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3704 2023-07-19 16:32:47.000000 kuki-0.9.7/kuki/util.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-25 13:38:34.470388 kuki-0.9.7/kuki.egg-info/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      554 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/SOURCES.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/dependency_links.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/entry_points.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/not-zip-safe
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       15 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/requires.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/top_level.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      468 2023-07-25 13:38:34.472388 kuki-0.9.7/setup.cfg
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.9.7/setup.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-25 13:38:34.471388 kuki-0.9.7/test/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.7/test/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.7/test/conftest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1423 2023-07-19 15:39:03.000000 kuki-0.9.7/test/test_kest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    15810 2023-07-21 15:26:05.000000 kuki-0.9.7/test/test_kuki.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-27 15:27:28.953883 kuki-0.9.8/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.9.8/LICENSE
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12048 2023-07-27 15:27:28.953883 kuki-0.9.8/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      463 2023-07-25 13:52:37.000000 kuki-0.9.8/README.md
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-27 15:27:28.951882 kuki-0.9.8/kuki/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.9.8/kuki/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1176 2023-05-20 06:39:32.000000 kuki-0.9.8/kuki/config_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1375 2023-07-23 05:45:31.000000 kuki-0.9.8/kuki/kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1994 2023-07-19 16:18:20.000000 kuki-0.9.8/kuki/ktrl.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4652 2023-07-22 06:51:24.000000 kuki-0.9.8/kuki/ktrl_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4768 2023-07-27 15:23:50.000000 kuki-0.9.8/kuki/kuki.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4087 2023-07-23 15:13:37.000000 kuki-0.9.8/kuki/package_util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-27 15:27:28.952883 kuki-0.9.8/kuki/q/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.9.8/kuki/q/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-26 16:08:04.000000 kuki-0.9.8/kuki/q/cli.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     7819 2023-07-27 06:39:46.000000 kuki-0.9.8/kuki/q/kest.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      219 2023-07-19 16:35:57.000000 kuki-0.9.8/kuki/q/ktrl.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1918 2023-07-27 07:07:32.000000 kuki-0.9.8/kuki/q/kuki.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2187 2023-07-20 15:49:50.000000 kuki-0.9.8/kuki/q/log.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1435 2023-07-15 14:20:22.000000 kuki-0.9.8/kuki/q/path.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    20344 2023-07-27 15:26:18.000000 kuki-0.9.8/kuki/registry_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3704 2023-07-19 16:32:47.000000 kuki-0.9.8/kuki/util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-27 15:27:28.952883 kuki-0.9.8/kuki.egg-info/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12048 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      554 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/SOURCES.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/dependency_links.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/entry_points.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/not-zip-safe
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       15 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/requires.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/top_level.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      468 2023-07-27 15:27:28.953883 kuki-0.9.8/setup.cfg
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.9.8/setup.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-27 15:27:28.953883 kuki-0.9.8/test/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.8/test/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.8/test/conftest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1423 2023-07-19 15:39:03.000000 kuki-0.9.8/test/test_kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    15975 2023-07-27 15:05:32.000000 kuki-0.9.8/test/test_kuki.py
```

### Comparing `kuki-0.9.7/LICENSE` & `kuki-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/PKG-INFO` & `kuki-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.9.7
+Version: 0.9.8
 Summary: K Ultimate pacKage Installer
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: q,k
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,15 @@
 
 Refer to [wiki](https://github.com/jshinonome/kuki/wiki) for documentations.
 
 ### Commands
 
 `kuki` includes a set of 3 commands
 
-- kuki: _K Ultimate pacKage Installer_, manage q/k packages
+- kuki: _K Ultimate pacKage Installer cli_, manage q/k packages
 - kest: _K tEST cli_, test q/k codes
 - ktrl: _K conTRoL cli_,control
 
 ### Registry Site
 
 `kuki` can publish and install packages from central registry site [kuki.ninja](https://kuki.ninja/), thanks to [verdaccio](https://verdaccio.org/)
```

### Comparing `kuki-0.9.7/kuki/config_util.py` & `kuki-0.9.8/kuki/config_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/kuki/kest.py` & `kuki-0.9.8/kuki/kest.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/kuki/ktrl.py` & `kuki-0.9.8/kuki/ktrl.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/kuki/ktrl_util.py` & `kuki-0.9.8/kuki/ktrl_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/kuki/kuki.py` & `kuki-0.9.8/kuki/kuki.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,20 @@
     elif args.download:
         registry_util.download_entry(args.download)
     elif args.unpublish:
         registry_util.unpublish_package(args.unpublish)
     else:
         if args.globalMode:
             if isinstance(args.install, list):
-                registry_util.install_packages(args.install, False, True)
-                registry_util.dump_global_index()
+                for pkg in args.install:
+                    if pkg.startswith("."):
+                        registry_util.install_local_package(pkg, False, True)
+                    else:
+                        registry_util.install_package(pkg, False, True)
+                    registry_util.dump_global_index()
         elif not package_util.exits():
             logger.error("kuki.json not found, use 'kuki --init' to init the package first")
             return
         elif args.version:
             package_util.roll_up_version(args.version)
         elif args.publish:
             registry_util.publish_entry()
```

### Comparing `kuki-0.9.7/kuki/package_util.py` & `kuki-0.9.8/kuki/package_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/kuki/q/cli.q` & `kuki-0.9.8/kuki/q/cli.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/kuki/q/kest.q` & `kuki-0.9.8/kuki/q/kest.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/kuki/q/kuki.q` & `kuki-0.9.8/kuki/q/kuki.q`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 .kuki.index:.j.k (,/) @[read0;`:kuki_index.json;{"{}"}];
 
 .kuki.importGlobal:{[module]
   subPaths: "/" vs module;
   moduleName: `$first subPaths;
   if[not moduleName in key .kuki.index; '"No module named - ", string moduleName];
-  path: .kuki.joinPath[.kuki.rootDir;(first subPaths;.kuki.index[`file;`version];"src"),(-1_ 1_subPaths), enlist .kuki.appendDotQ last subPaths];
+  path: .kuki.joinPath[.kuki.rootDir;(first subPaths;.kuki.index[moduleName;`version];"src"),(-1_ 1_subPaths), enlist .kuki.appendDotQ last subPaths];
   .kuki.importModule path
  };
 
 // global import - import {"moduleName/[folder/]/module"}
 // local import - import {"./[folder/]/module"}
 // module doesn't include .q
 import:{[moduleFunc]
```

### Comparing `kuki-0.9.7/kuki/q/log.q` & `kuki-0.9.8/kuki/q/log.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/kuki/q/path.q` & `kuki-0.9.8/kuki/q/path.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/kuki/registry_util.py` & `kuki-0.9.8/kuki/registry_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -407,88 +407,133 @@
         else:
             raise Exception("empty tar file - " + tar_name)
     return cached_filepath
 
 
 def install_entry(pkgs: List[str]):
     try:
-        install_packages(pkgs, False)
+        for pkg in pkgs:
+            if pkg.startswith("."):
+                install_local_package(pkg)
+            else:
+                install_package(pkg, False)
         install_dependencies()
         package_util.dump_kuki(kuki_json)
         package_util.dump_pkg_index(package_index)
         dump_global_index()
     except Exception as e:
         logger.error("failed to install packages with error: {}".format(e))
 
 
-def install_packages(pkgs: List[str], skip_updating_pkg_index=True, globalMode=False):
+def install_package(pkg: str, skip_updating_pkg_index=True, globalMode=False):
     package_type = kuki_json.get("type", "q")
 
     if package_type == "k":
         allow_package_types = ["k"]
     elif package_type == "k9":
         allow_package_types = ["k9"]
     else:
         allow_package_types = ["q", "k"]
 
-    for pkg in pkgs:
-        if skip_updating_pkg_index:
-            logger.info("install dependency package '{}'".format(pkg))
-        else:
-            logger.info("install package '{}'".format(pkg))
-        metadata = get_metadata(pkg)
+    if skip_updating_pkg_index:
+        logger.info("installing dependency package '{}'".format(pkg))
+    else:
+        logger.info("installing package '{}'".format(pkg))
+    metadata = get_metadata(pkg)
 
-        if not metadata.get("type") in allow_package_types and not globalMode:
-            logger.error("")
+    if not metadata.get("type", "q") in allow_package_types and not globalMode:
+        logger.error(
+            "Only allows to install package type '{}', Got package type '{}'".format(
+                allow_package_types, metadata.get("type", "q")
+            )
+        )
+        return
+    name = metadata["name"]
+    if not globalMode and name == kuki_json["name"]:
+        logger.warning("shouldn't install itself, skip...")
+        return
 
-        name = metadata["name"]
-        if not globalMode and name == kuki_json["name"]:
-            logger.warning("shouldn't install itself, skip...")
-            return
-
-        version = metadata["version"]
-        pkg_id = get_pkg_id(metadata)
-
-        if not skip_updating_pkg_index and not globalMode:
-            kuki_json["dependencies"][name] = version
-
-        if not globalMode:
-            if name in package_index and version != package_index[name]["version"]:
-                logger.info("current '{}@{}' exists".format(name, package_index[name]["version"]))
-                if name in kuki_json["dependencies"]:
-                    version = kuki_json["dependencies"][name]
-                    logger.warning(
-                        "{} is a dependency package, force to use version {}".format(name, version)
-                    )
-                elif newer_than(version, package_index[name]["version"]):
-                    logger.warning("use newer '{}@{}'".format(name, version))
-                else:
-                    logger.warning("skip outdated '{}@{}'".format(name, version))
-                    continue
+    version = metadata["version"]
+    pkg_id = get_pkg_id(metadata)
 
-            package_index[name] = metadata
+    if not skip_updating_pkg_index and not globalMode:
+        kuki_json["dependencies"][name] = version
 
-        if pkg_id in global_index and name in package_index:
-            logger.warning("{} is already installed, skip...".format(pkg_id))
-            continue
-        if pkg_id not in global_index:
-            # global index uses package id as keys, package index uses package name as keys
-            global_index[pkg_id] = metadata
-            install_packages(
-                [k + "@" + v for k, v in metadata["dependencies"].items()], True, globalMode
-            )
-            install_package(metadata)
+    if not globalMode:
+        if name in package_index and version != package_index[name]["version"]:
+            logger.info("current '{}@{}' exists".format(name, package_index[name]["version"]))
+            if name in kuki_json["dependencies"]:
+                version = kuki_json["dependencies"][name]
+                logger.warning(
+                    "{} is a dependency package, force to use version {}".format(name, version)
+                )
+            elif newer_than(version, package_index[name]["version"]):
+                logger.warning("use newer '{}@{}'".format(name, version))
+            else:
+                logger.warning("skip outdated '{}@{}'".format(name, version))
+                return
 
+        package_index[name] = metadata
 
-def install_package(metadata: Metadata):
+    if pkg_id in global_index and name in package_index:
+        logger.warning("{} is already installed in kuki root, skip...".format(pkg_id))
+        return
+    if pkg_id not in global_index:
+        # global index uses package id as keys, package index uses package name as keys
+        global_index[pkg_id] = metadata
+        for dep in [k + "@" + v for k, v in metadata["dependencies"].items()]:
+            install_package(dep, True, globalMode)
+        extract_package(metadata)
+
+
+def install_local_package(
+    local_pkg_tar: str,
+    skip_updating_pkg_index=True,
+    globalMode=False,
+):
+    logger.info("installing local package '{}'".format(local_pkg_tar))
+    local_pkg_tar_path = Path(local_pkg_tar)
+    if local_pkg_tar_path.exists():
+        tar = tarfile.open(local_pkg_tar_path)
+        file = tar.extractfile("kuki.json")
+        pkg_kuki_json: package_util.Kuki = json.load(file)
+    name = pkg_kuki_json["name"]
+    version = pkg_kuki_json["version"]
+    install_pkg_path = get_pkg_path(name, version)
+    if not install_pkg_path.exists():
+        install_pkg_path.mkdir(parents=True, exist_ok=True)
+    tar.extractall(install_pkg_path)
+    tar.close()
+
+    if not skip_updating_pkg_index and not globalMode:
+        kuki_json["dependencies"][name] = version
+
+    if not globalMode:
+        if name in package_index and version != package_index[name]["version"]:
+            logger.info("current '{}@{}' exists".format(name, package_index[name]["version"]))
+            if name in kuki_json["dependencies"]:
+                version = kuki_json["dependencies"][name]
+                logger.warning(
+                    "{} is a dependency package, force to use version {}".format(name, version)
+                )
+            elif newer_than(version, package_index[name]["version"]):
+                logger.warning("use newer '{}@{}'".format(name, version))
+            else:
+                logger.warning("skip outdated '{}@{}'".format(name, version))
+                return
+
+        package_index[name] = pkg_kuki_json
+    else:
+        global_index[get_pkg_id(pkg_kuki_json)] = pkg_kuki_json
+    logger.info("installed local package '{}'".format(local_pkg_tar))
+
+
+def extract_package(metadata: Metadata):
     pkg_filepath = download_package(metadata)
     pkg_path = get_pkg_path(metadata["name"], metadata["version"])
-    # already exists
-    if pkg_path.exists() and pkg_path.is_dir():
-        return
     if not pkg_path.exists():
         pkg_path.mkdir(parents=True, exist_ok=True)
     tar = tarfile.open(pkg_filepath, "r:gz")
     tar.extractall(pkg_path)
     tar.close()
 
 
@@ -548,8 +593,9 @@
     pending = []
     for name, version in deps.items():
         if name in package_index and version == package_index[name]["version"]:
             continue
         pkg_id = get_pkg_id({"name": name, "version": version})
         logger.warning("missing '{}'".format(pkg_id))
         pending.append(pkg_id)
-    install_packages(pending)
+    for pkg in pending:
+        install_package(pkg)
```

### Comparing `kuki-0.9.7/kuki/util.py` & `kuki-0.9.8/kuki/util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/kuki.egg-info/PKG-INFO` & `kuki-0.9.8/kuki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.9.7
+Version: 0.9.8
 Summary: K Ultimate pacKage Installer
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: q,k
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,15 @@
 
 Refer to [wiki](https://github.com/jshinonome/kuki/wiki) for documentations.
 
 ### Commands
 
 `kuki` includes a set of 3 commands
 
-- kuki: _K Ultimate pacKage Installer_, manage q/k packages
+- kuki: _K Ultimate pacKage Installer cli_, manage q/k packages
 - kest: _K tEST cli_, test q/k codes
 - ktrl: _K conTRoL cli_,control
 
 ### Registry Site
 
 `kuki` can publish and install packages from central registry site [kuki.ninja](https://kuki.ninja/), thanks to [verdaccio](https://verdaccio.org/)
```

### Comparing `kuki-0.9.7/kuki.egg-info/SOURCES.txt` & `kuki-0.9.8/kuki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/test/test_kest.py` & `kuki-0.9.8/test/test_kest.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.7/test/test_kuki.py` & `kuki-0.9.8/test/test_kuki.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,20 @@
     package_name = "dummy"
     responses.add(
         responses.PUT,
         registry_util.registry + package_name,
         status=201,
     )
 
+    responses.add(
+        responses.GET,
+        registry_util.registry + package_name,
+        status=404,
+    )
+
     monkeypatch.setattr("builtins.input", lambda _: "yes")
     package_util.generate_json(
         package_name, "a dummy package", "Saitama", "https://github.com/saitama/dummy"
     )
 
     source_files = [
         "src/dummy.q",
@@ -286,14 +292,15 @@
     tar = tarfile.open(str(tar_path), "r:gz")
     tar_files = tar.getnames()
 
     source_files.remove("conf/exchange.csv")
     source_files.append("src/lib")
     source_files.append("README.md")
     source_files.append(package_util.config_file)
+    source_files.append(package_util.index_file)
 
     assert len(source_files) == len(tar_files)
 
     sorted_source_files = sorted(source_files)
     sorted_tar_files = sorted(tar_files)
     for i, file in enumerate(sorted_tar_files):
         assert file == sorted_source_files[i]
```

