# Comparing `tmp/flaggie-0.99.5.tar.gz` & `tmp/flaggie-0.99.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaggie-0.99.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flaggie-0.99.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flaggie-0.99.5.tar` & `flaggie-0.99.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1058 2023-01-15 07:39:45.197204 flaggie-0.99.5/COPYING
--rw-r--r--   0        0        0       84 2023-07-17 09:37:59.888358 flaggie-0.99.5/flaggie/__init__.py
--rw-r--r--   0        0        0    13202 2023-07-17 09:37:20.610998 flaggie-0.99.5/flaggie/__main__.py
--rw-r--r--   0        0        0     6739 2023-01-15 07:39:45.200537 flaggie-0.99.5/flaggie/config.py
--rw-r--r--   0        0        0    14319 2023-01-20 19:03:37.545724 flaggie-0.99.5/flaggie/mangle.py
--rw-r--r--   0        0        0     7288 2023-02-15 16:46:20.320855 flaggie-0.99.5/flaggie/pm.py
--rw-r--r--   0        0        0     1118 2023-04-26 13:10:43.742172 flaggie-0.99.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-15 07:39:45.200537 flaggie-0.99.5/test/__init__.py
--rw-r--r--   0        0        0     4723 2023-01-15 07:39:45.200537 flaggie-0.99.5/test/test_config.py
--rw-r--r--   0        0        0     1845 2023-01-15 16:47:15.640493 flaggie-0.99.5/test/test_main.py
--rw-r--r--   0        0        0    16203 2023-01-20 19:03:53.062748 flaggie-0.99.5/test/test_mangle.py
--rw-r--r--   0        0        0     7205 2023-02-15 16:46:20.320855 flaggie-0.99.5/test/test_pm.py
--rw-r--r--   0        0        0      464 2023-01-15 07:39:45.200537 flaggie-0.99.5/tox.ini
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 flaggie-0.99.5/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-01-15 07:39:45.197204 flaggie-0.99.6/COPYING
+-rw-r--r--   0        0        0       84 2023-07-27 14:14:58.894412 flaggie-0.99.6/flaggie/__init__.py
+-rw-r--r--   0        0        0    13280 2023-07-27 12:40:47.009200 flaggie-0.99.6/flaggie/__main__.py
+-rw-r--r--   0        0        0     6739 2023-01-15 07:39:45.200537 flaggie-0.99.6/flaggie/config.py
+-rw-r--r--   0        0        0    14319 2023-01-20 19:03:37.545724 flaggie-0.99.6/flaggie/mangle.py
+-rw-r--r--   0        0        0     7288 2023-02-15 16:46:20.320855 flaggie-0.99.6/flaggie/pm.py
+-rw-r--r--   0        0        0     1118 2023-04-26 13:10:43.742172 flaggie-0.99.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-15 07:39:45.200537 flaggie-0.99.6/test/__init__.py
+-rw-r--r--   0        0        0     4723 2023-01-15 07:39:45.200537 flaggie-0.99.6/test/test_config.py
+-rw-r--r--   0        0        0     1845 2023-01-15 16:47:15.640493 flaggie-0.99.6/test/test_main.py
+-rw-r--r--   0        0        0    16203 2023-01-20 19:03:53.062748 flaggie-0.99.6/test/test_mangle.py
+-rw-r--r--   0        0        0     7205 2023-02-15 16:46:20.320855 flaggie-0.99.6/test/test_pm.py
+-rw-r--r--   0        0        0      464 2023-01-15 07:39:45.200537 flaggie-0.99.6/tox.ini
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 flaggie-0.99.6/PKG-INFO
```

### Comparing `flaggie-0.99.5/COPYING` & `flaggie-0.99.6/COPYING`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.5/flaggie/__main__.py` & `flaggie-0.99.6/flaggie/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,20 +164,21 @@
                                f"for {package}")
                 if flag in values:
                     yield (ns, token_type)
 
     matched_types = set(get_matching_types())
     if not matched_types:
         argp.error(f"{op}: Argument not recognized as any type, pass "
-                   f"e.g. use::{flag} to force one")
+                   f"e.g. use::{flag} to force one (for packages: "
+                   f"{packages})")
     elif len(matched_types) > 1:
         names = sorted(x[0] for x in matched_types)
         argp.error(f"{op}: Argument matches multiple token types: "
                    f"{', '.join(names)}; pass e.g. {names[0]}::{flag} to "
-                   "disambiguate")
+                   f"disambiguate (for packages: {packages})")
     return next(iter(matched_types))[0]
 
 
 def main(prog_name: str, *argv: str) -> int:
     # same as argparse default, enforce for consistency
     help_width = shutil.get_terminal_size().columns - 2
     if help_width > 10:
```

### Comparing `flaggie-0.99.5/flaggie/config.py` & `flaggie-0.99.6/flaggie/config.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.5/flaggie/mangle.py` & `flaggie-0.99.6/flaggie/mangle.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.5/flaggie/pm.py` & `flaggie-0.99.6/flaggie/pm.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.5/pyproject.toml` & `flaggie-0.99.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.5/test/test_config.py` & `flaggie-0.99.6/test/test_config.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.5/test/test_main.py` & `flaggie-0.99.6/test/test_main.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.5/test/test_mangle.py` & `flaggie-0.99.6/test/test_mangle.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.5/test/test_pm.py` & `flaggie-0.99.6/test/test_pm.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.5/PKG-INFO` & `flaggie-0.99.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaggie
-Version: 0.99.5
+Version: 0.99.6
 Summary: CLI mangler for Portage package.* configuration files
 Author-email: Michał Górny <mgorny@gentoo.org>
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: more-itertools
 Requires-Dist: gentoopm >= 0.5 ; extra == "package-manager"
 Requires-Dist: rich ; extra == "pretty-log"
```

