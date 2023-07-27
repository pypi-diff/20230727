# Comparing `tmp/apkinjector-1.0.4.tar.gz` & `tmp/apkinjector-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkinjector-1.0.4.tar", last modified: Tue Jul 25 21:40:39 2023, max compression
+gzip compressed data, was "apkinjector-1.1.0.tar", last modified: Thu Jul 27 17:55:35 2023, max compression
```

## Comparing `apkinjector-1.0.4.tar` & `apkinjector-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:40:39.084815 apkinjector-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 21:40:28.000000 apkinjector-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-25 21:40:39.084815 apkinjector-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-25 21:40:28.000000 apkinjector-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:40:39.084815 apkinjector-1.0.4/apkinjector/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/adb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/apktool.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/frida.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/gadget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/uber_apk_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-25 21:40:28.000000 apkinjector-1.0.4/apkinjector/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:40:39.084815 apkinjector-1.0.4/apkinjector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 21:40:39.000000 apkinjector-1.0.4/apkinjector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:40:39.084815 apkinjector-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-25 21:40:28.000000 apkinjector-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:55:35.157077 apkinjector-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 17:55:24.000000 apkinjector-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-27 17:55:35.157077 apkinjector-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-27 17:55:24.000000 apkinjector-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:55:35.153077 apkinjector-1.1.0/apkinjector/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/adb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/apktool.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/frida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/gadget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/uber_apk_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-27 17:55:24.000000 apkinjector-1.1.0/apkinjector/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:55:35.153077 apkinjector-1.1.0/apkinjector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-27 17:55:35.000000 apkinjector-1.1.0/apkinjector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-27 17:55:35.000000 apkinjector-1.1.0/apkinjector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:55:35.000000 apkinjector-1.1.0/apkinjector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-27 17:55:35.000000 apkinjector-1.1.0/apkinjector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 17:55:35.000000 apkinjector-1.1.0/apkinjector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 17:55:35.000000 apkinjector-1.1.0/apkinjector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:55:35.157077 apkinjector-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-27 17:55:24.000000 apkinjector-1.1.0/setup.py
```

### Comparing `apkinjector-1.0.4/LICENSE` & `apkinjector-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.4/PKG-INFO` & `apkinjector-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkinjector
-Version: 1.0.4
+Version: 1.1.0
 Summary: Utilities to help injecting libraries and frida in apks.
 Home-page: https://nitanmarcel.github.io/apkinjector
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK,INJECTION,INJECT
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkinjector-1.0.4/README.md` & `apkinjector-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.4/apkinjector/__init__.py` & `apkinjector-1.1.0/apkinjector/__init__.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.4/apkinjector/__main__.py` & `apkinjector-1.1.0/apkinjector/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import os
 import sys
 import time
+import zipfile
 
 import click
 import json
 import shutil
 import requests
 import tempfile
 from colorama import Fore
-from pyaxmlparser import APK
 
 from . import LOG, USER_DIRECTORIES, __PLUGIN_DATA__
 from .adb import Adb
 from .apktool import Apktool
 from .java import Java
 from .arch import ARCH
 from .download import ProgressCompleted, ProgressDownloading, ProgressFailed, ProgressUnknown
 from .frida import Frida
 from .gadget import Gadget
 from .injector import Injector
 from .plugins import _PluginLoader, main
 from .uber_apk_signer import UberApkSigner
-from .bundle import Bundle
+from .bundle import Bundle, ConfigArch, ConfigDpi, ConfigLocale
 from .download import download_file
+from .manifest import Manifest
+
+def _clear_cache(func):
+    def inner(*args, **kwargs):
+        func(*args, **kwargs)
+        shutil.rmtree(USER_DIRECTORIES.user_cache_dir)
+        os.makedirs(USER_DIRECTORIES.user_cache_dir)
+    return inner
+
 
 def _install_callback(progress):
     if isinstance(progress, ProgressDownloading):
         sys.stdout.write(
             Fore.GREEN + f'\r[+] Downloading {progress.filename} - {progress.progress:03d}%')
         sys.stdout.flush()
     if isinstance(progress, ProgressFailed):
@@ -34,111 +43,163 @@
             Fore.RED + f'[*] Download failed with status: {progress.status_code}')
     if isinstance(progress, ProgressCompleted):
         sys.stdout.write('\n')
     if isinstance(progress, ProgressUnknown):
         LOG.info('Downloading {} this might take a while...', progress.filename)
 
 
+@_clear_cache
 def _inject(apk, libraries, include, activity, output, override, use_aapt):
     if not os.path.isfile(apk):
         LOG.error('{} - not such file.', apk)
     for lib in libraries:
         if not os.path.isfile(lib):
             LOG.error('{} - not such file.', lib)
     
     if include:
         for i in include:
             if not os.path.isfile(i):
-                LOG.error('Include {} is not a valid file', include)
+                LOG.error('Include {} is not a valid file.', include)
 
-    apk_name, ext = os.path.basename(apk).rsplit('.', 1)
+    apk_name, ext =  os.path.splitext(apk)
     workdir = os.path.join(USER_DIRECTORIES.user_cache_dir, apk_name)
-    target = apk
-    bundle_path = None
+    entry_lib = libraries[0]
 
-    if override:
-        output = apk
-    else:
+    _, _ext = os.path.splitext(output)
+    if not _ext:
+        # is file
+        tmp_output = output
         if os.path.isdir(output):
-            tmp_output = os.path.join(output, f'{apk_name}_patched.{ext}')
+            tmp_output = os.path.join(output, f'{apk_name}_patched{ext}' if not override else apk)
+        else:
+            if tmp_output.endswith(os.sep):
+                tmp_output = tmp_output.rsplit(os.sep, 1)[0]
         if os.path.exists(tmp_output):
-            timestamp = str(time.time()).split('.')[0]
-            tmp_output = os.path.join(output, f'{apk_name}_patched_{timestamp}.{ext}')
+            timestamp = int(time.time())
+            tmp_output = os.path.join(output, f'{apk_name}_patched_{timestamp}{ext}')
         output = tmp_output
-    
+    else:
+        if os.path.exists(output) and not override:
+            LOG.error('{} already exists.', output)
+
     is_bundle = Bundle.is_bundle(apk)
+
+    output_bundle = None
+    bundle_info = None
+
     if is_bundle:
         LOG.info('Extracting split apks...')
         output_bundle = f'{workdir}_bundle'
         if os.path.exists(output_bundle):
             shutil.rmtree(output_bundle)
-            bundle_path, target = Bundle.extract(apk, output_bundle)
-            LOG.info('Found base apk: {}', target)
-    
-    manifest = APK(target)
+        bundle_info = Bundle.extract(apk, output_bundle)
 
-    target_activity = None
+    targets = []
+
+    if bundle_info and bundle_info.configs:
+        for config in bundle_info.configs:
+            if isinstance(config, ConfigArch):
+                for lib in libraries.copy():
+                    lib_arch = Injector.guess_arch_from_lib(lib)
+                    if lib_arch == config.arch:
+                        target_split = os.path.join(output_bundle, config.file_name)
+                        targets.append([target_split, lib])
+                        libraries.remove(lib)
+    for lib in libraries:
+        if is_bundle:
+            target_split = os.path.join(output_bundle, bundle_info.base_apk)
+            targets.append([target_split, lib])
+        else:
+            targets.append([output, lib])
+
+    Apktool.install(progress_callback=_install_callback)
+    LOG.info('Using apktool: {}', Apktool.version())
 
+    base = os.path.join(output_bundle, bundle_info.base_apk) if is_bundle else apk
+    # extract base
+    LOG.info('Extracting {}', base)
+    Apktool.decode(base, force=True, output=workdir, framework_path=f'{workdir}_framework')
+
+    manifest_path = os.path.join(workdir, 'AndroidManifest.xml')
+    target_activity = None
     if activity:
-        for activities in manifest.get_activities():
+        for activities in Manifest.get_activities(manifest_path):
             for i in activities:
                 if activity in i:
                     target_activity = i
                     break
     else:
-        target_activity = manifest.get_main_activity()
+        target_activity = Manifest.get_main_activity(manifest_path)
     if not target_activity:
         LOG.error('{} did not match any activities', activity)
     
     LOG.info('Found target activity {}', target_activity)
 
-    LOG.info('Extracting {}', target)
-
-    Apktool.install(progress_callback=_install_callback)
-    LOG.info('Using apktool {}', Apktool.version())
-
-    Apktool.decode(target, force=True, output=workdir, framework_path=f'{workdir}_framework', no_res=True)
-
     entrypoint = None
     for file in os.listdir(workdir):
         if file.startswith('smali'):
             entrypoint_tmp = os.path.join(
             workdir, file, target_activity.replace('.', '/') + '.smali')
             if os.path.isfile(entrypoint_tmp):
                 entrypoint = entrypoint_tmp
-                break           
-
+                break  
     if not entrypoint:
         LOG.error('Failed to find smali file for activity {}', target_activity)
-    LOG.info('Injecting {} into {}', libraries[0], target_activity)
-    injected = Injector.inject_library(libraries[0], workdir, entrypoint, include)
+        
+    LOG.info('Injecting smali loader into {}.', target_activity)
+    injected = Injector.inject_library(entry_lib, workdir, entrypoint, include, skip_copy=True) # Copying will be done for each target bellow
     if not injected:
-        LOG.warning('Something wen\'t wrong when injecting {}', library)
-    if len(libraries) > 0:
-        for library in libraries[1:]:
-            LOG.info('Copying {} into apk.', library)
-            injected = Injector.inject_library(library, workdir, None, include)
-            if not injected:
-                LOG.warning('Something wen\'t wrong when injecting {}', library)
+        LOG.error('Something wen\'t wrong when injecting into target..')
+    LOG.info('Repacking {} -> {}', base if is_bundle else apk, base if is_bundle else output)
+    Apktool.build(workdir, output=base if is_bundle else output, framework_path=f'{workdir}_framework', use_aapt2=use_aapt)
+
+    for target in targets:
+        apk_target = target[0]
+        lib_target = target[1]
+        if os.path.exists(workdir):
+            shutil.rmtree(workdir)
+        os.makedirs(workdir)
+        LOG.info('Extracting {}', apk_target)
+        with zipfile.ZipFile(apk_target, 'r') as ref:
+            ref.extractall(workdir)
+        LOG.info('Injecting {} in {}', lib_target, apk_target)
+        injected = Injector.inject_library(lib_target, workdir, smali_path=None, extra_files=include)
+        if not injected:
+            LOG.error('Something wen\'t wrong when injecting into target..')
+        LOG.info('Repacking {} -> {}', apk_target, apk_target if is_bundle else output)
+        with zipfile.ZipFile(apk_target if is_bundle else output, 'w') as ref:
+            for root, dirs, files in os.walk(workdir):
+                for file in files:
+                    ref.write(os.path.join(root, file), 
+                        os.path.relpath(os.path.join(root, file), 
+                                        workdir))
     
-    LOG.info('Repacking target')
+    apks = []
+    if is_bundle:
+        apks = [os.path.join(output_bundle, apk) for apk in os.listdir(output_bundle) if apk.endswith('.apk')]
+    else:
+        apks = [output,]
+    
+    LOG.info('Signing {}', ' '.join([os.path.basename(apk) for apk in apks]))
+    UberApkSigner.install(progress_callback=_install_callback)
+
+    LOG.info('Using uber-apk-signer {}', UberApkSigner.version().split()[-1])
+
+    UberApkSigner.sign(apks, allow_resign=True, overwrite=True)
+
     if is_bundle:
-        Apktool.build(workdir, output=os.path.join(bundle_path, target), framework_path=f'{workdir}_framework', use_aapt2=use_aapt)
+        LOG.info('Repacking bundle')
         cache_bundle = os.path.join(USER_DIRECTORIES.user_cache_dir, f'cached.{ext}')
         Bundle.repack(f'{workdir}_bundle', cache_bundle)
         if os.path.isfile(output):
             os.remove(output)
         shutil.copyfile(cache_bundle, output)
-    else:
-        Apktool.build(workdir, output=output, framework_path=f'{workdir}_framework', use_aapt2=use_aapt)
-    LOG.info('Signing {}', output)
-    UberApkSigner.install(progress_callback=_install_callback)
-    LOG.info('Using uber-apk-signer {}', UberApkSigner.version().split()[-1])
-    UberApkSigner.sign(output, allow_resign=True, overwrite=True)
     LOG.info('DONE! {}', output)
+
+    ### Clear cache
   
 @main.command(help='Inject a shared library (*.so) in a target apk.')
 @click.argument('apk')
 @click.option('--library', required=True, multiple=True, help='Shared library (*.so) to inject. If multiple are given, only the first one will be automatically loaded.')
 @click.option('--include', multiple=True, required=False, help='Extra files to include in the lib folder. Can be used multiple times to include more files.')
 @click.option('--activity', required=False, help='Name of the activity to inject into. If unspecified, the main activity will be injected.')
 @click.option('--output', required=False, default=os.getcwd(), help='Custom path where the patched apk should be saved.')
@@ -226,26 +287,32 @@
 @click.argument('apk')
 @click.option('--activities', is_flag=True, help='Gets all activities')
 @click.option('--permissions', is_flag=True, help='Gets all permissions')
 @click.option('--libraries', is_flag=True, help='Gets all libraries')
 @click.option('--recievers', is_flag=True, help='Gets all receivers')
 def apk(apk, activities, permissions, libraries, recievers):
     def _parse_apk():
-        manifest = APK(apk)
+        Java.install(progress_callback=_install_callback)
+        Apktool.install(progress_callback=_install_callback)
+
+        decoded_dir = os.path.join(USER_DIRECTORIES.user_cache_dir, 'decoded_tmp')
+
+        Apktool.decode(apk, output=decoded_dir, framework_path=f'{decoded_dir}_framework', no_res=True, no_src=True, force_manifest=True)
+        manifest_path = os.path.join(decoded_dir, 'AndroidManifest.xml')
         if activities:
-            for activity in manifest.get_activities():
+            for activity in Manifest.get_activities(manifest_path):
                 LOG.info(activity)
         if permissions:
-            for permission in manifest.get_permissions():
+            for permission in Manifest.get_permissions(manifest_path):
                 LOG.info(permission)
         if libraries:
-            for library in manifest.get_libraries():
+            for library in Manifest.get_libraries(manifest_path):
                 LOG.info(library)
         if recievers:
-            for reciever in manifest.get_receivers():
+            for reciever in Manifest.get_receivers(manifest_path):
                 LOG.info('{}', reciever)
     if not os.path.isfile(apk):
         LOG.error('{} - not such file.', apk)
     if Bundle.is_bundle(apk):
         with tempfile.TemporaryDirectory() as tmp:
             apk, base = Bundle.extract(apk, tmp)
             apk = os.path.join(apk, base)
```

### Comparing `apkinjector-1.0.4/apkinjector/adb.py` & `apkinjector-1.1.0/apkinjector/adb.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.4/apkinjector/apktool.py` & `apkinjector-1.1.0/apkinjector/apktool.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         if framework_path:
             command += f' --frame-path {framework_path}'
         if tag:
             command += f' --tag {tag}'
         return Java.run_jar(DEPENDENCIES.apktool, command)
 
     @staticmethod
-    def decode(file_apk, force=False, output=None, framework_path=None, no_res=False, no_src=False, tag=None):
+    def decode(file_apk, force=False, output=None, framework_path=None, no_res=False, no_src=False, tag=None, force_manifest=False):
         """
         Decode an APK file with provided options.
 
         :param file_apk: The APK file to be decoded.
         :type file_apk: str
         :param force: Whether to force delete the destination directory, defaults to False.
         :type force: bool, optional
@@ -77,14 +77,16 @@
         :type framework_path: str, optional
         :param no_res: Whether to not decode resources, defaults to False.
         :type no_res: bool, optional
         :param no_src: Whether to not decode sources, defaults to False.
         :type no_src: bool, optional
         :param tag: A tag for the framework file, defaults to None.
         :type tag: str, optional
+        :param force_manifest: Forces decode of AndroidManifest.xml regardless of decoding of resources parameter.
+        :type force_manifest: str, optional
         :return: The stdout from the command execution.
         :rtype: str
         """
         command = f'd {file_apk}'
         if force:
             command += ' --force'
         if output:
@@ -93,14 +95,16 @@
             command += f' --frame-path {framework_path}'
         if no_res:
             command += ' --no-res'
         if no_src:
             command += ' --no-src'
         if tag:
             command += f' --frame-tag {tag}'
+        if force_manifest:
+            command += f' --force-manifest'
         return Java.run_jar(DEPENDENCIES.apktool, command)
 
     @staticmethod
     def build(app_path, force_all=False, output=None, framework_path=None, use_aapt2=False):
         """
         Build the unpacked apk from the given path with the provided options.
 
@@ -109,15 +113,15 @@
         :param force_all: Whether to skip changes detection and build all files, defaults to False.
         :type force_all: bool, optional
         :param output: The name of the output APK file, defaults to None.
         :type output: str, optional
         :param framework_path: The directory containing framework files, defaults to None.
         :type framework_path: str, optional
         :param use_aapt2: Whether to use aapt 2 or no, defaults to False.
-        :type use_aapt2: bool, optional
+        :type use_aapt2: bool, optional.
         :return: The stdout from the command execution.
         :rtype: str
         """
         command = f'b {app_path}'
         if force_all:
             command += ' --force-all'
         if output:
```

### Comparing `apkinjector-1.0.4/apkinjector/dependencies.py` & `apkinjector-1.1.0/apkinjector/dependencies.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.4/apkinjector/download.py` & `apkinjector-1.1.0/apkinjector/download.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.4/apkinjector/frida.py` & `apkinjector-1.1.0/apkinjector/frida.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.4/apkinjector/gadget.py` & `apkinjector-1.1.0/apkinjector/gadget.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.4/apkinjector/injector.py` & `apkinjector-1.1.0/apkinjector/injector.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,57 +6,56 @@
 
 from .arch import ARCH
 from .utils import arch_to_abi
 
 
 class Injector:
     @staticmethod
-    def inject_library(source: str, unpack_path: str, smali_path: str = None, extra_files: List[str] = None) -> None:
-        """Inject library into unpacked apk
+    def inject_library(source: str, unpack_path: str, smali_path: str = None, extra_files: List[str] = None, skip_copy=False) -> None:
+        """
+        Injects a library into an unpacked apk.
 
-        Args:
-            source (str): Path to shared library to inject.
-            unpack_path (str): Path to apktool unpacked apk.
-            smali_path (str, optional): _description_. Path to smali file to inject into. Leave empty to skip this step
-            extra_files (List[str], optional): _description_. Extra files to copy over the the apk lib/ folder
+        :param source: The path to the shared library to inject.
+        :type source: str
+        :param unpack_path: The path to the apktool unpacked apk.
+        :type unpack_path: str
+        :param smali_path: The path to the smali file to inject into. Leave empty to skip this step. Defaults to None.
+        :type smali_path: str, optional
+        :param extra_files: Extra files to copy over the to the apk lib/ folder. Defaults to None.
+        :type extra_files: list of str, optional
+        :param skip_copy: Whatever to copy the library into target, or skip and just edit the smali. Defaults to False.
+        :type skip_copy: bool, optional
 
-        Returns:
-            bool: If the injection was succesful or not.
+        :return: If the injection was successful or not.
+        :rtype: bool
         """
-        lib, ext = os.path.basename(source).rsplit('.', 1)
+        lib, _ = os.path.splitext(os.path.basename(source))
         lib = lib.split('lib', 1)[-1]
         lines = []
         injected = False
         if smali_path and not os.path.isfile(smali_path):
             return injected
 
-        abi = None
-
-        with open(source, 'rb') as libfile:
-            elffile = ELFFile(libfile)
-            arch = elffile.get_machine_arch()
-            if arch.lower() in ['aarch64', 'arm64']:
-                arch = ARCH.ARM64
-            if arch.lower() in ['x64']:
-                return ARCH.X64
-            abi = arch_to_abi(arch.lower())
+        arch = Injector.guess_arch_from_lib(source)
+        abi = arch_to_abi(arch.lower())
 
-        path = os.path.join(unpack_path, 'lib', abi)
-        if not os.path.isdir(path):
-            os.makedirs(path)
-        paths = []
-        paths.append(source)
-        if extra_files:
-            paths.extend(extra_files)
-        for file in paths:
-            name = os.path.basename(file)
-            dest = os.path.join(path, name)
-            if os.path.isfile(dest):
-                os.remove(dest)
-            shutil.copyfile(file, dest)
+        if not skip_copy:
+            path = os.path.join(unpack_path, 'lib', abi)
+            if not os.path.isdir(path):
+                os.makedirs(path)
+            paths = []
+            paths.append(source)
+            if extra_files:
+                paths.extend(extra_files)
+            for file in paths:
+                name = os.path.basename(file)
+                dest = os.path.join(path, name)
+                if os.path.isfile(dest):
+                    os.remove(dest)
+                shutil.copyfile(file, dest)
 
         injected = not bool(smali_path)
         if smali_path:
             with open(smali_path, 'r') as smali:
                 lines = smali.readlines()
             matches = []
             for line in lines:
@@ -82,7 +81,19 @@
                         lines.insert(
                             index + 2, '    invoke-static {v0}, Ljava/lang/System;->loadLibrary(Ljava/lang/String;)V\n')
                         injected = True
                         break
             with open(smali_path, 'w') as smali:
                 smali.writelines(lines)
         return injected
+    
+    @staticmethod
+    def guess_arch_from_lib(lib_path: str) -> ARCH:
+        with open(lib_path, 'rb') as libfile:
+            elffile = ELFFile(libfile)
+            arch = elffile.get_machine_arch()
+            if arch.lower() in ['aarch64', 'arm64']:
+                arch = ARCH.ARM64
+            if arch.lower() in ['x64']:
+                arch = ARCH.X64
+        return arch
+
```

### Comparing `apkinjector-1.0.4/apkinjector/java.py` & `apkinjector-1.1.0/apkinjector/java.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,18 @@
         """
         process = subprocess.run(
             f'{DEPENDENCIES.java} -jar {jar_file} {command}', shell=True, capture_output=True, text=True)
         return process.stdout
     
     @staticmethod
     def install(path: str = None, progress_callback: Callable = None) -> None:
-        """Installs java
+        """
+        Installs java
 
-        :param path: Path to existing java if not found will use the system installed one or download it., defaults to None
+        :param path: Path to existing java if not found will use the system installed one or download it. Defaults to None.
         :type path: str, optional
-        :param progress_callback:Callback to be called when install progress changes, defaults to None.
-        :type progress_callback: Callable, optional
-        
+        :param progress_callback: Callback to be called when install progress changes. Defaults to None.
+        :type progress_callback: Callable, optional.
+
         """
         DEPENDENCIES.add_dependency(
             'java', path=path, fallback=_download_java, fallback_args=(progress_callback,))
```

### Comparing `apkinjector-1.0.4/apkinjector/logger.py` & `apkinjector-1.1.0/apkinjector/logger.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.4/apkinjector/plugins.py` & `apkinjector-1.1.0/apkinjector/plugins.py`

 * *Files identical despite different names*

### Comparing `apkinjector-1.0.4/apkinjector/uber_apk_signer.py` & `apkinjector-1.1.0/apkinjector/uber_apk_signer.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,28 +26,28 @@
 
         :return: The stdout from the command execution.
         :rtype: str
         """
         return Java.run_jar(DEPENDENCIES.uber_apk_signer, '--version')
 
     @staticmethod
-    def sign(apks: str, allow_resign: Optional[bool] = False, debug: Optional[bool] = False,
+    def sign(apks: List[str], allow_resign: Optional[bool] = False, debug: Optional[bool] = False,
              dry_run: Optional[bool] = False, ks: Optional[str] = None, ks_alias: Optional[str] = None,
              ks_debug: Optional[str] = None, ks_key_pass: Optional[str] = None, ks_pass: Optional[str] = None,
              lineage: Optional[str] = None, out: Optional[str] = None, overwrite: Optional[bool] = False,
              skip_zip_align: Optional[bool] = False, only_verify: Optional[bool] = False,
              zip_align_path: Optional[str] = None, verify_sha256: Optional[str] = None) -> str:
         """
         Sign an APK or a set of APKs.
 
         :return: The stdout from the command execution.
         :rtype: str
         """
 
-        command = f'-a {apks}'
+        command = '-a {}'.format(' '.join(apks))
 
         if allow_resign:
             command += " --allowResign"
 
         if debug:
             command += " --debug"
```

### Comparing `apkinjector-1.0.4/apkinjector/utils.py` & `apkinjector-1.1.0/apkinjector/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         abi (str): Abi string
 
     Returns:
         Union[ARCH, None]: Converted abi to apkinjector.arch.Arch or None if the abi is not recognized.
     """
     mappings = {
         'armeabi-v7a': ARCH.ARM,
-        'arm64-v8a': ARCH.ARM64,
+        'arm64_v8a': ARCH.ARM64,
         'x86': ARCH.X86,
         'x86_64': ARCH.X64
     }
     if abi in mappings.keys():
         return mappings[abi]
     return None
```

### Comparing `apkinjector-1.0.4/apkinjector.egg-info/PKG-INFO` & `apkinjector-1.1.0/apkinjector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkinjector
-Version: 1.0.4
+Version: 1.1.0
 Summary: Utilities to help injecting libraries and frida in apks.
 Home-page: https://nitanmarcel.github.io/apkinjector
 Author: Marcel Alexandru Nitan
 Author-email: nitan.marcel@gmail.com
 Keywords: FRIDA,APK,INJECTION,INJECT
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `apkinjector-1.0.4/apkinjector.egg-info/SOURCES.txt` & `apkinjector-1.1.0/apkinjector.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 apkinjector/dependencies.py
 apkinjector/download.py
 apkinjector/frida.py
 apkinjector/gadget.py
 apkinjector/injector.py
 apkinjector/java.py
 apkinjector/logger.py
+apkinjector/manifest.py
 apkinjector/plugins.py
 apkinjector/uber_apk_signer.py
 apkinjector/utils.py
 apkinjector.egg-info/PKG-INFO
 apkinjector.egg-info/SOURCES.txt
 apkinjector.egg-info/dependency_links.txt
 apkinjector.egg-info/entry_points.txt
```

### Comparing `apkinjector-1.0.4/setup.py` & `apkinjector-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='apkinjector',
-    version='1.0.4',
+    version='1.1.0',
     description='Utilities to help injecting libraries and frida in apks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Marcel Alexandru Nitan',
     author_email='nitan.marcel@gmail.com',
     url='https://nitanmarcel.github.io/apkinjector',
     keywords=['FRIDA', 'APK', 'INJECTION', 'INJECT'],
@@ -21,15 +21,14 @@
         ]
     },
     install_requires=[
         'requests',
         'appdirs',
         'install-jdk',
         'click',
-        'pyaxmlparser',
         'pyelftools',
         'colorama'
     ],
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

