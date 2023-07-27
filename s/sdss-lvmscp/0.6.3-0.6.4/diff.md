# Comparing `tmp/sdss_lvmscp-0.6.3.tar.gz` & `tmp/sdss_lvmscp-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmscp-0.6.3.tar", max compression
+gzip compressed data, was "sdss_lvmscp-0.6.4.tar", max compression
```

## Comparing `sdss_lvmscp-0.6.3.tar` & `sdss_lvmscp-0.6.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1504 2023-07-26 19:25:37.157604 sdss_lvmscp-0.6.3/LICENSE.md
--rw-r--r--   0        0        0     1578 2023-07-26 19:25:37.157880 sdss_lvmscp-0.6.3/README.md
--rw-r--r--   0        0        0     2673 2023-07-26 19:25:37.202549 sdss_lvmscp-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      369 2023-07-26 19:25:37.203053 sdss_lvmscp-0.6.3/python/lvmscp/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-26 19:25:37.203359 sdss_lvmscp-0.6.3/python/lvmscp/__main__.py
--rw-r--r--   0        0        0      258 2023-07-26 19:25:37.203767 sdss_lvmscp-0.6.3/python/lvmscp/actor/__init__.py
--rw-r--r--   0        0        0     3455 2023-07-26 19:25:37.204035 sdss_lvmscp-0.6.3/python/lvmscp/actor/actor.py
--rw-r--r--   0        0        0      859 2023-07-26 19:25:37.204392 sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/__init__.py
--rw-r--r--   0        0        0     3827 2023-07-26 19:25:37.204684 sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/focus.py
--rw-r--r--   0        0        0     1272 2023-07-26 19:25:37.204961 sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/hardware_status.py
--rw-r--r--   0        0        0      758 2023-07-26 19:25:37.205411 sdss_lvmscp-0.6.3/python/lvmscp/controller.py
--rw-r--r--   0        0        0    14890 2023-07-26 19:25:37.205762 sdss_lvmscp-0.6.3/python/lvmscp/delegate.py
--rw-r--r--   0        0        0    40889 2023-07-26 19:25:37.206165 sdss_lvmscp-0.6.3/python/lvmscp/etc/LVM_100kHz.acf
--rw-r--r--   0        0        0     5502 2023-07-26 19:25:37.206522 sdss_lvmscp-0.6.3/python/lvmscp/etc/lvmscp.yml
--rw-r--r--   0        0        0      161 2023-07-26 19:25:37.206710 sdss_lvmscp-0.6.3/python/lvmscp/etc/schema.json
--rw-r--r--   0        0        0    18807 2023-07-26 19:25:37.207019 sdss_lvmscp-0.6.3/python/lvmscp/ln2.py
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 sdss_lvmscp-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-27 16:07:36.532274 sdss_lvmscp-0.6.4/LICENSE.md
+-rw-r--r--   0        0        0     1578 2023-07-27 16:07:36.532512 sdss_lvmscp-0.6.4/README.md
+-rw-r--r--   0        0        0     2693 2023-07-27 16:07:36.581964 sdss_lvmscp-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-07-27 16:07:36.582374 sdss_lvmscp-0.6.4/python/lvmscp/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-27 16:07:36.582642 sdss_lvmscp-0.6.4/python/lvmscp/__main__.py
+-rw-r--r--   0        0        0      258 2023-07-27 16:07:36.582939 sdss_lvmscp-0.6.4/python/lvmscp/actor/__init__.py
+-rw-r--r--   0        0        0     3522 2023-07-27 16:07:36.583166 sdss_lvmscp-0.6.4/python/lvmscp/actor/actor.py
+-rw-r--r--   0        0        0      859 2023-07-27 16:07:36.583455 sdss_lvmscp-0.6.4/python/lvmscp/actor/commands/__init__.py
+-rw-r--r--   0        0        0     3827 2023-07-27 16:07:36.583731 sdss_lvmscp-0.6.4/python/lvmscp/actor/commands/focus.py
+-rw-r--r--   0        0        0     1272 2023-07-27 16:07:36.583953 sdss_lvmscp-0.6.4/python/lvmscp/actor/commands/hardware_status.py
+-rw-r--r--   0        0        0      758 2023-07-27 16:07:36.584169 sdss_lvmscp-0.6.4/python/lvmscp/controller.py
+-rw-r--r--   0        0        0    14890 2023-07-27 16:07:36.584442 sdss_lvmscp-0.6.4/python/lvmscp/delegate.py
+-rw-r--r--   0        0        0    40889 2023-07-27 16:07:36.584854 sdss_lvmscp-0.6.4/python/lvmscp/etc/LVM_100kHz.acf
+-rw-r--r--   0        0        0     5502 2023-07-27 16:07:36.585150 sdss_lvmscp-0.6.4/python/lvmscp/etc/lvmscp.yml
+-rw-r--r--   0        0        0      161 2023-07-27 16:07:36.585354 sdss_lvmscp-0.6.4/python/lvmscp/etc/schema.json
+-rw-r--r--   0        0        0    18807 2023-07-27 16:07:36.585654 sdss_lvmscp-0.6.4/python/lvmscp/ln2.py
+-rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 sdss_lvmscp-0.6.4/PKG-INFO
```

### Comparing `sdss_lvmscp-0.6.3/LICENSE.md` & `sdss_lvmscp-0.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/README.md` & `sdss_lvmscp-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/pyproject.toml` & `sdss_lvmscp-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmscp"
-version = "0.6.3"
+version = "0.6.4"
 description = "LVM spectrograph control package."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Changgon Kim <changgonkim@khu.ac.kr>"]
 maintainers = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmscp"
 repository = "https://github.com/sdss/lvmscp"
@@ -29,14 +29,15 @@
 lvmscp = "lvmscp.__main__:main"
 ln2fill = "lvmscp.ln2:ln2fill"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 click-default-group = "^1.2.2"
 sdss-archon = "^0.11.0"
+sdss-clu = "^2.1.3"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=7.11.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 isort = ">=4.3.21"
 ipdb = ">=0.12.3"
```

### Comparing `sdss_lvmscp-0.6.3/python/lvmscp/__main__.py` & `sdss_lvmscp-0.6.4/python/lvmscp/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/python/lvmscp/actor/actor.py` & `sdss_lvmscp-0.6.4/python/lvmscp/actor/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         await asyncio.sleep(5)
 
         while True:
             await Command(
                 "status",
                 actor=self,
                 commander_id=f".{self.name}",
+                internal=True,
+                write_to_log=False,
             ).parse()
 
             await asyncio.sleep(delay)
 
     def merge_schemas(self, scp_schema_path: str | None = None):
         """Merge default schema with SCP one."""
```

### Comparing `sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/__init__.py` & `sdss_lvmscp-0.6.4/python/lvmscp/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/focus.py` & `sdss_lvmscp-0.6.4/python/lvmscp/actor/commands/focus.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/hardware_status.py` & `sdss_lvmscp-0.6.4/python/lvmscp/actor/commands/hardware_status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/python/lvmscp/controller.py` & `sdss_lvmscp-0.6.4/python/lvmscp/controller.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/python/lvmscp/delegate.py` & `sdss_lvmscp-0.6.4/python/lvmscp/delegate.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/python/lvmscp/etc/LVM_100kHz.acf` & `sdss_lvmscp-0.6.4/python/lvmscp/etc/LVM_100kHz.acf`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/python/lvmscp/etc/lvmscp.yml` & `sdss_lvmscp-0.6.4/python/lvmscp/etc/lvmscp.yml`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/python/lvmscp/ln2.py` & `sdss_lvmscp-0.6.4/python/lvmscp/ln2.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.3/PKG-INFO` & `sdss_lvmscp-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmscp
-Version: 0.6.3
+Version: 0.6.4
 Summary: LVM spectrograph control package.
 Home-page: https://github.com/sdss/lvmscp
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Maintainer: José Sánchez-Gallego
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: sdss-archon (>=0.11.0,<0.12.0)
+Requires-Dist: sdss-clu (>=2.1.3,<3.0.0)
 Project-URL: Documentation, https://sdss-lvmscp.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/lvmscp
 Description-Content-Type: text/markdown
 
 # lvmscp
 
 ![Versions](https://img.shields.io/badge/python->3.8-blue)
```

