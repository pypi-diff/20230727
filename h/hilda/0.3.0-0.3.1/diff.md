# Comparing `tmp/hilda-0.3.0.tar.gz` & `tmp/hilda-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilda-0.3.0.tar", last modified: Wed Jul 26 14:52:45 2023, max compression
+gzip compressed data, was "hilda-0.3.1.tar", last modified: Thu Jul 27 16:12:16 2023, max compression
```

## Comparing `hilda-0.3.0.tar` & `hilda-0.3.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-26 14:52:25.000000 hilda-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-07-26 14:52:45.284183 hilda-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-07-26 14:52:25.000000 hilda-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.280183 hilda-0.3.0/hilda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/from_ns_to_json.m
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/get_objectivec_class_description.m
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/get_objectivec_symbol_data.m
--rw-r--r--   0 runner    (1001) docker     (123)   120119 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/hilda_ascii_art.html
--rw-r--r--   0 runner    (1001) docker     (123)    42180 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/hilda_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/launch_lldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/lldb_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/lsof.m
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/hilda/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/boringssl.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/dyld.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/fs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/hilda/snippets/mach/
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/mach/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/hilda/snippets/macho/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/all_image_infos.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/apple_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/image_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/macho.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/macho/macho_load_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/remotepairingd.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/snippets/xpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/to_ns_from_json.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/hilda/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/ui/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/ui/ui_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-26 14:52:25.000000 hilda-0.3.0/hilda/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:52:45.284183 hilda-0.3.0/hilda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 14:52:45.000000 hilda-0.3.0/hilda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-26 14:52:25.000000 hilda-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-26 14:52:25.000000 hilda-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:52:45.284183 hilda-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:16.234191 hilda-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-27 16:11:56.000000 hilda-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-07-27 16:12:16.234191 hilda-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-07-27 16:11:56.000000 hilda-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:16.226190 hilda-0.3.1/hilda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/from_ns_to_json.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/get_objectivec_class_description.m
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/get_objectivec_symbol_data.m
+-rw-r--r--   0 runner    (1001) docker     (123)   120119 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/hilda_ascii_art.html
+-rw-r--r--   0 runner    (1001) docker     (123)    42522 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/hilda_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/launch_lldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/lldb_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/lsof.m
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:16.230191 hilda-0.3.1/hilda/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/boringssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/dyld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/fs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:16.230191 hilda-0.3.1/hilda/snippets/mach/
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/mach/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:16.234191 hilda-0.3.1/hilda/snippets/macho/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/macho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/macho/all_image_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/macho/apple_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/macho/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/macho/macho.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/macho/macho_load_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/remotepairingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/snippets/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/to_ns_from_json.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:16.234191 hilda-0.3.1/hilda/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/ui/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/ui/ui_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-27 16:11:57.000000 hilda-0.3.1/hilda/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:16.230191 hilda-0.3.1/hilda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-07-27 16:12:16.000000 hilda-0.3.1/hilda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-27 16:12:16.000000 hilda-0.3.1/hilda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:12:16.000000 hilda-0.3.1/hilda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 16:12:16.000000 hilda-0.3.1/hilda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 16:12:16.000000 hilda-0.3.1/hilda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 16:12:16.000000 hilda-0.3.1/hilda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-27 16:11:57.000000 hilda-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 16:11:57.000000 hilda-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:12:16.234191 hilda-0.3.1/setup.cfg
```

### Comparing `hilda-0.3.0/LICENSE` & `hilda-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/PKG-INFO` & `hilda-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 0.3.0
+Version: 0.3.1
 Summary: LLDB wrapped and empowered by iPython's features
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `hilda-0.3.0/README.md` & `hilda-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/command.py` & `hilda-0.3.1/hilda/command.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/exceptions.py` & `hilda-0.3.1/hilda/exceptions.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/from_ns_to_json.m` & `hilda-0.3.1/hilda/from_ns_to_json.m`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/get_objectivec_class_description.m` & `hilda-0.3.1/hilda/get_objectivec_class_description.m`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/get_objectivec_symbol_data.m` & `hilda-0.3.1/hilda/get_objectivec_symbol_data.m`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/hilda_ascii_art.html` & `hilda-0.3.1/hilda/hilda_ascii_art.html`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/hilda_client.py` & `hilda-0.3.1/hilda/hilda_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 import docstring_parser
 import hexdump
 import IPython
 import lldb
 from humanfriendly import prompts
 from humanfriendly.terminal.html import html_to_ansi
-from keystone import KS_ARCH_ARM64, KS_ARCH_X86, KS_MODE_64, KS_MODE_LITTLE_ENDIAN, Ks
 from pygments import highlight
 from pygments.formatters import TerminalTrueColorFormatter
 from pygments.lexers import XmlLexer
 from tqdm import tqdm
 from traitlets.config import Config
 
 from hilda import objective_c_class
@@ -39,14 +38,21 @@
 from hilda.objective_c_symbol import ObjectiveCSymbol
 from hilda.registers import Registers
 from hilda.snippets.mach import CFRunLoopServiceMachPort_hooks
 from hilda.symbol import Symbol
 from hilda.symbols_jar import SymbolsJar
 from hilda.ui.ui_manager import UiManager
 
+lldb.KEYSTONE_SUPPORT = True
+try:
+    from keystone import KS_ARCH_ARM64, KS_ARCH_X86, KS_MODE_64, KS_MODE_LITTLE_ENDIAN, Ks
+except ImportError:
+    lldb.KEYSTONE_SUPPORT = False
+    print('failed to import keystone. disabling some features')
+
 IsaMagic = namedtuple('IsaMagic', 'mask value')
 ISA_MAGICS = [
     # ARM64
     IsaMagic(mask=0x000003f000000001, value=0x000001a000000001),
     # X86_64
     IsaMagic(mask=0x001f800000000001, value=0x001d800000000001),
 ]
@@ -253,14 +259,16 @@
     @command()
     def poke_text(self, address: int, code: str) -> int:
         """
         Write instructions to address.
         :param address:
         :param code:
         """
+        if not lldb.KEYSTONE_SUPPORT:
+            raise NotImplementedError('Not supported without keystone')
         bytecode, count = self._ks.asm(code, as_bytes=True)
         return self.poke(address, bytecode)
 
     @command()
     def peek(self, address, size: int) -> bytes:
         """
         Read data at given address
@@ -1189,12 +1197,14 @@
         }
         if fmt in formatters:
             return formatters[fmt](value)
         else:
             return f'{value:x} (unsupported format)'
 
     @cached_property
-    def _ks(self) -> Ks:
+    def _ks(self) -> Optional['Ks']:
+        if not lldb.KEYSTONE_SUPPORT:
+            return False
         platforms = {'arm64': Ks(KS_ARCH_ARM64, KS_MODE_LITTLE_ENDIAN),
                      'arm64e': Ks(KS_ARCH_ARM64, KS_MODE_LITTLE_ENDIAN),
                      'x86_64h': Ks(KS_ARCH_X86, KS_MODE_64)}
         return platforms.get(self.arch)
```

### Comparing `hilda-0.3.0/hilda/launch_lldb.py` & `hilda-0.3.1/hilda/launch_lldb.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/lldb_entrypoint.py` & `hilda-0.3.1/hilda/lldb_entrypoint.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/lsof.m` & `hilda-0.3.1/hilda/lsof.m`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/objective_c_class.py` & `hilda-0.3.1/hilda/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/objective_c_symbol.py` & `hilda-0.3.1/hilda/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/registers.py` & `hilda-0.3.1/hilda/registers.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/snippets/boringssl.py` & `hilda-0.3.1/hilda/snippets/boringssl.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/snippets/dyld.py` & `hilda-0.3.1/hilda/snippets/dyld.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py` & `hilda-0.3.1/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,17 @@
         CoreFoundation:__text:0000000186E50140                 STP             X20, X19, [SP,#0x60+var_10]
         CoreFoundation:__text:0000000186E50144                 STP             X29, X30, [SP,#0x60+var_s0]
         CoreFoundation:__text:0000000186E50148                 ADD             X29, SP, #0x60
         CoreFoundation:__text:0000000186E5014C                 MOV             X21, X5
         CoreFoundation:__text:0000000186E50150                 MOV             X22, X4
         CoreFoundation:__text:0000000186E50154                 MOV             X23, X3       <-------- Timeout parameter
     """
+    if not lldb.KEYSTONE_SUPPORT:
+        return
+
     hilda = lldb.hilda_client
     if hilda.arch == 'x86_64h':
         return
 
     with hilda.stopped():
         for inst in hilda.symbols.__CFRunLoopServiceMachPort.disass(200, should_print=False):
             mnemonic = inst.GetMnemonic(hilda.target)
```

### Comparing `hilda-0.3.0/hilda/snippets/macho/all_image_infos.py` & `hilda-0.3.1/hilda/snippets/macho/all_image_infos.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/snippets/macho/image_info.py` & `hilda-0.3.1/hilda/snippets/macho/image_info.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/snippets/macho/macho.py` & `hilda-0.3.1/hilda/snippets/macho/macho.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/snippets/macho/macho_load_commands.py` & `hilda-0.3.1/hilda/snippets/macho/macho_load_commands.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/snippets/remotepairingd.py` & `hilda-0.3.1/hilda/snippets/remotepairingd.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/snippets/xpc.py` & `hilda-0.3.1/hilda/snippets/xpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,21 +50,21 @@
     """
     Convert XPC object to python object.
     :param address: Address of XPC object.
     """
     return lldb.hilda_client.from_ns(f'_CFXPCCreateCFObjectFromXPCObject({address})')
 
 
-def disable_transaction_exit():
+def disable_transaction_exit() -> None:
     """
     xpc_transaction_exit_clean will kill the process when transaction is done.
     By patching this function the process will stay alive.
     """
     hilda = lldb.hilda_client
-    hilda.symbols.xpc_transaction_exit_clean.poke_text('ret')
+    hilda.symbols.xpc_transaction_exit_clean.poke(b'\xc0\x03\x5f\xd6')  # ret
 
 
 def to_xpc_object(obj: object):
     """
     Convert python object to XPC object.
     :param obj: Native python object
     """
```

### Comparing `hilda-0.3.0/hilda/symbol.py` & `hilda-0.3.1/hilda/symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/symbols_jar.py` & `hilda-0.3.1/hilda/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/to_ns_from_json.m` & `hilda-0.3.1/hilda/to_ns_from_json.m`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/ui/ui_manager.py` & `hilda-0.3.1/hilda/ui/ui_manager.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda/ui/views.py` & `hilda-0.3.1/hilda/ui/views.py`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/hilda.egg-info/PKG-INFO` & `hilda-0.3.1/hilda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 0.3.0
+Version: 0.3.1
 Summary: LLDB wrapped and empowered by iPython's features
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `hilda-0.3.0/hilda.egg-info/SOURCES.txt` & `hilda-0.3.1/hilda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hilda-0.3.0/pyproject.toml` & `hilda-0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hilda"
-version = "0.3.0"
+version = "0.3.1"
 description = "LLDB wrapped and empowered by iPython's features"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["python", "debugger", "lldb", "ipython", "ios", "debug"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" },
```

