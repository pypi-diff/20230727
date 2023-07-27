# Comparing `tmp/avnet-scotty-2023.6.tar.gz` & `tmp/avnet-scotty-2023.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avnet-scotty-2023.6.tar", last modified: Fri Jul  7 06:38:04 2023, max compression
+gzip compressed data, was "avnet-scotty-2023.7.tar", last modified: Thu Jul 27 09:08:48 2023, max compression
```

## Comparing `avnet-scotty-2023.6.tar` & `avnet-scotty-2023.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:38:04.233218 avnet-scotty-2023.6/
--rw-r--r--   0 root         (0) root         (0)    32879 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)    20288 2023-07-07 06:38:04.233218 avnet-scotty-2023.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19990 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:38:04.229218 avnet-scotty-2023.6/avnet_scotty.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20288 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      380 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-07 06:38:04.000000 avnet-scotty-2023.6/avnet_scotty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:38:04.229218 avnet-scotty-2023.6/bumper/
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/bumper/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4006 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/bumper/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     6719 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/scotty
--rwxr-xr-x   0 root         (0) root         (0)     1637 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/scotty-runqemu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:38:04.229218 avnet-scotty-2023.6/scotty_test/
--rw-r--r--   0 root         (0) root         (0)     4424 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/scotty_test/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 06:38:04.233218 avnet-scotty-2023.6/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      811 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/scripts/vm_bundle.sh
--rw-r--r--   0 root         (0) root         (0)     1137 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/scripts/vm_create.sh.template
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 06:38:04.233218 avnet-scotty-2023.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1153 2023-07-07 06:37:53.000000 avnet-scotty-2023.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:08:48.148742 avnet-scotty-2023.7/
+-rw-r--r--   0 root         (0) root         (0)    32879 2023-07-27 09:08:39.000000 avnet-scotty-2023.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20288 2023-07-27 09:08:48.148742 avnet-scotty-2023.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19990 2023-07-27 09:08:39.000000 avnet-scotty-2023.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:08:48.148742 avnet-scotty-2023.7/avnet_scotty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20288 2023-07-27 09:08:48.000000 avnet-scotty-2023.7/avnet_scotty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      380 2023-07-27 09:08:48.000000 avnet-scotty-2023.7/avnet_scotty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 09:08:48.000000 avnet-scotty-2023.7/avnet_scotty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-27 09:08:48.000000 avnet-scotty-2023.7/avnet_scotty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-27 09:08:48.000000 avnet-scotty-2023.7/avnet_scotty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-27 09:08:48.000000 avnet-scotty-2023.7/avnet_scotty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:08:48.148742 avnet-scotty-2023.7/bumper/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-27 09:08:39.000000 avnet-scotty-2023.7/bumper/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4006 2023-07-27 09:08:39.000000 avnet-scotty-2023.7/bumper/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6719 2023-07-27 09:08:40.000000 avnet-scotty-2023.7/scotty
+-rwxr-xr-x   0 root         (0) root         (0)     1637 2023-07-27 09:08:39.000000 avnet-scotty-2023.7/scotty-runqemu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:08:48.148742 avnet-scotty-2023.7/scotty_test/
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-27 09:08:39.000000 avnet-scotty-2023.7/scotty_test/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 09:08:48.148742 avnet-scotty-2023.7/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      811 2023-07-27 09:08:39.000000 avnet-scotty-2023.7/scripts/vm_bundle.sh
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-07-27 09:08:39.000000 avnet-scotty-2023.7/scripts/vm_create.sh.template
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 09:08:48.148742 avnet-scotty-2023.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-07-27 09:08:39.000000 avnet-scotty-2023.7/setup.py
```

### Comparing `avnet-scotty-2023.6/LICENSE` & `avnet-scotty-2023.7/LICENSE`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.6/PKG-INFO` & `avnet-scotty-2023.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2023.6
+Version: 2023.7
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Home-page: https://github.com/avnet-embedded/simplecore-tools
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `avnet-scotty-2023.6/README.rst` & `avnet-scotty-2023.7/README.rst`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.6/avnet_scotty.egg-info/PKG-INFO` & `avnet-scotty-2023.7/avnet_scotty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2023.6
+Version: 2023.7
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Home-page: https://github.com/avnet-embedded/simplecore-tools
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `avnet-scotty-2023.6/bumper/__main__.py` & `avnet-scotty-2023.7/bumper/__main__.py`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.6/scotty` & `avnet-scotty-2023.7/scotty`

 * *Files 0% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 	TERM \
 	UBOOT_ENV_VARS \
 	"
 # SCOTTY_FEATURES_LAYERS REPO_URL SCOTTY_MACHINE_DIR BUILDDIR
 declare -r scotty_whitelist=${SCOTTY_WHITELIST:-${scotty_whitelist_default}}
 
 if [ "${SCOTTY_DOCKER_IMAGE:-1}" == "1" ]; then
-    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:2023.6"
+    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:2023.7"
 else
     declare -r docker_default_image="${SCOTTY_DOCKER_IMAGE}"
 fi
 
-export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2023.6"
+export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2023.7"
 export SCOTTY_DEFAULT_MANIFEST_NAME="default-release.xml"
 
 debug() {
 	if [ "${SCOTTY_DEBUG:-0}" == "1" ]; then
 		echo -e "\033[1;38m${*}\033[0m"
 	fi
 }
```

### Comparing `avnet-scotty-2023.6/scotty-runqemu` & `avnet-scotty-2023.7/scotty-runqemu`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.6/scotty_test/__main__.py` & `avnet-scotty-2023.7/scotty_test/__main__.py`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.6/scripts/vm_bundle.sh` & `avnet-scotty-2023.7/scripts/vm_bundle.sh`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.6/scripts/vm_create.sh.template` & `avnet-scotty-2023.7/scripts/vm_create.sh.template`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.6/setup.py` & `avnet-scotty-2023.7/setup.py`

 * *Files identical despite different names*

