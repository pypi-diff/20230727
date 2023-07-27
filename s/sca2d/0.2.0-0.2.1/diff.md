# Comparing `tmp/sca2d-0.2.0.tar.gz` & `tmp/sca2d-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sca2d-0.2.0.tar", last modified: Fri May 27 10:47:58 2022, max compression
+gzip compressed data, was "sca2d-0.2.1.tar", last modified: Thu Jul 27 18:11:25 2023, max compression
```

## Comparing `sca2d-0.2.0.tar` & `sca2d-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,33 @@
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2022-05-27 10:47:58.000000 sca2d-0.2.0/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3267 2022-05-27 10:47:58.000000 sca2d-0.2.0/PKG-INFO
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2083 2021-04-01 15:29:06.000000 sca2d-0.2.0/README.md
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2022-05-27 10:47:58.000000 sca2d-0.2.0/sca2d/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       41 2020-11-17 19:56:19.000000 sca2d-0.2.0/sca2d/__init__.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3648 2021-04-01 16:24:43.000000 sca2d-0.2.0/sca2d/__main__.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3940 2022-05-27 10:17:20.000000 sca2d-0.2.0/sca2d/definitions.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2022-05-27 10:47:58.000000 sca2d-0.2.0/sca2d/lark/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     6293 2021-12-10 10:50:01.000000 sca2d-0.2.0/sca2d/lark/scad.lark
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     9202 2022-05-27 08:56:13.000000 sca2d-0.2.0/sca2d/messages.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    18218 2021-12-13 00:14:44.000000 sca2d-0.2.0/sca2d/outerscope.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       41 2021-04-07 13:32:24.000000 sca2d-0.2.0/sca2d/patterns.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     5641 2022-05-27 09:48:43.000000 sca2d-0.2.0/sca2d/sca2d.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     9927 2022-05-27 10:34:19.000000 sca2d-0.2.0/sca2d/scadclasses.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    34944 2022-05-27 10:00:13.000000 sca2d-0.2.0/sca2d/scope.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    12266 2022-05-27 10:01:09.000000 sca2d-0.2.0/sca2d/utilities.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2022-05-27 10:47:58.000000 sca2d-0.2.0/sca2d.egg-info/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3267 2022-05-27 10:47:58.000000 sca2d-0.2.0/sca2d.egg-info/PKG-INFO
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      426 2022-05-27 10:47:58.000000 sca2d-0.2.0/sca2d.egg-info/SOURCES.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2022-05-27 10:47:58.000000 sca2d-0.2.0/sca2d.egg-info/dependency_links.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       47 2022-05-27 10:47:58.000000 sca2d-0.2.0/sca2d.egg-info/entry_points.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2020-11-15 18:17:42.000000 sca2d-0.2.0/sca2d.egg-info/not-zip-safe
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       21 2022-05-27 10:47:58.000000 sca2d-0.2.0/sca2d.egg-info/requires.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        6 2022-05-27 10:47:58.000000 sca2d-0.2.0/sca2d.egg-info/top_level.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       38 2022-05-27 10:47:58.000000 sca2d-0.2.0/setup.cfg
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1887 2022-05-27 10:47:26.000000 sca2d-0.2.0/setup.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-07-27 18:11:25.391683 sca2d-0.2.1/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    35147 2019-06-18 15:37:09.000000 sca2d-0.2.1/LICENSE
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2830 2023-07-27 18:11:25.391683 sca2d-0.2.1/PKG-INFO
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2083 2021-04-01 15:29:06.000000 sca2d-0.2.1/README.md
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-07-27 18:11:25.387683 sca2d-0.2.1/sca2d/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       41 2020-11-17 19:56:19.000000 sca2d-0.2.1/sca2d/__init__.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     4529 2023-07-20 10:15:30.000000 sca2d-0.2.1/sca2d/__main__.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3940 2022-05-27 10:17:20.000000 sca2d-0.2.1/sca2d/definitions.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-07-27 18:11:25.387683 sca2d-0.2.1/sca2d/lark/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     6293 2021-12-10 10:50:01.000000 sca2d-0.2.1/sca2d/lark/scad.lark
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     9202 2022-05-27 08:56:13.000000 sca2d-0.2.1/sca2d/messages.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    18218 2021-12-13 00:14:44.000000 sca2d-0.2.1/sca2d/outerscope.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       41 2021-04-07 13:32:24.000000 sca2d-0.2.1/sca2d/patterns.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     5641 2022-05-27 09:48:43.000000 sca2d-0.2.1/sca2d/sca2d.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     9927 2022-05-27 10:34:19.000000 sca2d-0.2.1/sca2d/scadclasses.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    34944 2022-05-27 10:00:13.000000 sca2d-0.2.1/sca2d/scope.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    12266 2022-05-27 10:01:09.000000 sca2d-0.2.1/sca2d/utilities.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-07-27 18:11:25.387683 sca2d-0.2.1/sca2d.egg-info/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2830 2023-07-27 18:11:25.000000 sca2d-0.2.1/sca2d.egg-info/PKG-INFO
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      547 2023-07-27 18:11:25.000000 sca2d-0.2.1/sca2d.egg-info/SOURCES.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-07-27 18:11:25.000000 sca2d-0.2.1/sca2d.egg-info/dependency_links.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       46 2023-07-27 18:11:25.000000 sca2d-0.2.1/sca2d.egg-info/entry_points.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2020-11-15 18:17:42.000000 sca2d-0.2.1/sca2d.egg-info/not-zip-safe
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       41 2023-07-27 18:11:25.000000 sca2d-0.2.1/sca2d.egg-info/requires.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        6 2023-07-27 18:11:25.000000 sca2d-0.2.1/sca2d.egg-info/top_level.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       38 2023-07-27 18:11:25.391683 sca2d-0.2.1/setup.cfg
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1976 2023-07-20 11:10:53.000000 sca2d-0.2.1/setup.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-07-27 18:11:25.391683 sca2d-0.2.1/tests/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    14339 2022-05-27 09:47:41.000000 sca2d-0.2.1/tests/test_analyser.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2698 2023-07-20 11:08:10.000000 sca2d-0.2.1/tests/test_cli.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1450 2021-12-13 23:33:54.000000 sca2d-0.2.1/tests/test_file_analysis.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2578 2022-05-27 09:49:35.000000 sca2d-0.2.1/tests/test_messages.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1353 2021-12-10 10:48:09.000000 sca2d-0.2.1/tests/test_parser.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sca2d-0.2.0/PKG-INFO` & `sca2d-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 Metadata-Version: 2.1
 Name: sca2d
-Version: 0.2.0
+Version: 0.2.1
 Summary: An experimental static code analyser for OpenSCAD.
 Home-page: https://gitlab.com/bath_open_instrumentation_group/sca2d
 Author: Julian Stirling
 Author-email: julian@julianstirling.co.uk
 License: GPLv3
 Project-URL: Bug Tracker, https://gitlab.com/bath_open_instrumentation_group/sca2d/issues
 Project-URL: Source Code, https://gitlab.com/bath_open_instrumentation_group/sca2d
-Description: # SCA2D - Static Code Analysis for SCAD
-        
-        ![](identity/SCA2D.png)
-        
-        This is an experimental linter for OpenSCAD. The focus is to properly lex the `.scad` files so that we can test for dangerous code like redefining variable from other scopes. SCA2D is in a very early stage of development.
-        
-        ## How to install
-        
-        If you have Python 3.6 or later installed on your machine (and on the PATH) you can install SCA2D from PyPi by running the following command from a terminal
-        
-            pip install sca2d
-        
-        to upgrade your current versions of SCA2D run:
-        
-            pip install sca2d --upgrade
-        
-        You can check that SCA2D is installed by running the following:
-        
-            sca2d -h
-        
-        you should see a help screen.
-        
-        ### Install issues
-        
-        If you have problems with installation possible problems include:
-        
-        * You may need to run `pip3` instead of `pip`
-        * Python may not be on the PATH, this often happens in Windows depending on how python was installed
-        * Python and PIP are on the path but SCA2D isn't. This normally happens if Python is installed through the Windows store. It is best to install Python from [python.org](https://www.python.org/downloads/)
-        
-        ## How to run
-        
-        To analyse a `.scad` file run:
-        
-            sca2d filename.scad
-        This will print any code messages to the screen.
-        
-        To analyse all `.scad` files in a directory run:
-        
-            sca2d directory_path
-        This will also print any code messages to the screen.
-        
-        If you wish to inspect the parse tree that SCA2D generates and then uses you can instead run:
-        
-            sca2d --output-tree filename.scad
-        the tree will be printed into a file called `filename.sca2d`.
-        
-        ## What works
-        
-        * Parsing most `.scad` files. We don't yet to extensive testing. Please raise an issue if you find a parsing error in SCA2D.
-        * Parsing included and used `.scad` files and checking variable, function, and module usage in different scopes.
-        * Checking for a minimal number of code errors
-        
-        ## How to get involved
-        
-        The best way to get involved is to find bugs and then [open an issue](https://gitlab.com/bath_open_instrumentation_group/sca2d/-/issues). You could also make changes and open a merge request.
-        
 Keywords: OpenSCAD,Linting
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# SCA2D - Static Code Analysis for SCAD
+
+![](identity/SCA2D.png)
+
+This is an experimental linter for OpenSCAD. The focus is to properly lex the `.scad` files so that we can test for dangerous code like redefining variable from other scopes. SCA2D is in a very early stage of development.
+
+## How to install
+
+If you have Python 3.6 or later installed on your machine (and on the PATH) you can install SCA2D from PyPi by running the following command from a terminal
+
+    pip install sca2d
+
+to upgrade your current versions of SCA2D run:
+
+    pip install sca2d --upgrade
+
+You can check that SCA2D is installed by running the following:
+
+    sca2d -h
+
+you should see a help screen.
+
+### Install issues
+
+If you have problems with installation possible problems include:
+
+* You may need to run `pip3` instead of `pip`
+* Python may not be on the PATH, this often happens in Windows depending on how python was installed
+* Python and PIP are on the path but SCA2D isn't. This normally happens if Python is installed through the Windows store. It is best to install Python from [python.org](https://www.python.org/downloads/)
+
+## How to run
+
+To analyse a `.scad` file run:
+
+    sca2d filename.scad
+This will print any code messages to the screen.
+
+To analyse all `.scad` files in a directory run:
+
+    sca2d directory_path
+This will also print any code messages to the screen.
+
+If you wish to inspect the parse tree that SCA2D generates and then uses you can instead run:
+
+    sca2d --output-tree filename.scad
+the tree will be printed into a file called `filename.sca2d`.
+
+## What works
+
+* Parsing most `.scad` files. We don't yet to extensive testing. Please raise an issue if you find a parsing error in SCA2D.
+* Parsing included and used `.scad` files and checking variable, function, and module usage in different scopes.
+* Checking for a minimal number of code errors
+
+## How to get involved
+
+The best way to get involved is to find bugs and then [open an issue](https://gitlab.com/bath_open_instrumentation_group/sca2d/-/issues). You could also make changes and open a merge request.
```

### Comparing `sca2d-0.2.0/README.md` & `sca2d-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sca2d-0.2.0/sca2d/__main__.py` & `sca2d-0.2.1/sca2d/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 '''The entry point for SCA2D. This file runs when you run `sca2d` in terminal'''
 
 import os
 import sys
 import argparse
 import json
 from sca2d import Analyser
-from sca2d.messages import print_messages, count_messages, gitlab_summary
+from sca2d.messages import print_messages, count_messages, gitlab_summary, MESSAGES
 
-def parse_args():
+
+def _parse_ignore_arg(ignore_str):
+    to_ignore = set(filter(None, ignore_str.split(",")))
+    assert to_ignore.issubset(MESSAGES), ("'--ignore' contains unknown message "
+                                          f"codes: {to_ignore - set(MESSAGES)}")
+    return sorted(to_ignore)
+
+
+def parse_args(cli_arguments=None):
     """
     This sets up the argumant parsing using the argparse module. It will automatically
     create a help message describing all options. Run `sca2d -h` in your terminal to see
     this description.
     """
     parser = argparse.ArgumentParser(description="SCA2D - A static code analyser for OpenSCAD.")
     parser.add_argument("file_or_dir_name",
@@ -30,20 +38,27 @@
                         action="store_true")
     parser.add_argument("--debug",
                         help=("Also print SCA2D debug messages"),
                         action="store_true")
     parser.add_argument("--gitlab-report",
                         help=("Output a gitlab code quality report"),
                         action="store_true")
-    return parser.parse_args()
+    parser.add_argument("--ignore",
+                        type=_parse_ignore_arg,
+                        help=("Comma-seperated list of message codes to ignore. "
+                              "Note that some messages cannot be ignored, for instance "
+                              "fatal syntax errors.  example: --ignore=W2010,W1003"),
+                        default="")
+    return parser.parse_args(cli_arguments)
 
 
 def _run_on_file(args, analyser):
     [parsed, all_messages] = analyser.analyse_file(args.file_or_dir_name,
-                                                   output_tree=args.output_tree)
+                                                   output_tree=args.output_tree,
+                                                   ignore_list=args.ignore)
     print_messages(all_messages, args.file_or_dir_name, args.colour, args.debug)
     return [parsed, all_messages]
 
 def _get_all_scad_files(dir_name):
     scad_files = []
     for root, _, files in os.walk(dir_name):
         for name in files:
@@ -55,26 +70,27 @@
 
 def _run_on_dir(args, analyser):
     parsed = True
     all_messages = []
     scad_files = _get_all_scad_files(args.file_or_dir_name)
     for scad_filename in scad_files:
         [file_parsed, file_messages] = analyser.analyse_file(scad_filename,
-                                                             output_tree=args.output_tree)
+                                                             output_tree=args.output_tree,
+                                                             ignore_list=args.ignore)
         print_messages(file_messages, scad_filename, args.colour, args.debug)
         parsed = parsed and file_parsed
         all_messages += file_messages
     return [parsed, all_messages]
 
-def main():
+def main(cli_arguments=None):
     '''
     creates a sca2d analyser and then analyses the input file. Printing
     analysis to the screen
     '''
-    args = parse_args()
+    args = parse_args(cli_arguments)
     analyser = Analyser(verbose=args.verbose)
     if os.path.isfile(args.file_or_dir_name):
         [_, all_messages] = _run_on_file(args, analyser)
 
     elif os.path.isdir(args.file_or_dir_name):
         [_, all_messages] = _run_on_dir(args, analyser)
     else:
@@ -86,11 +102,10 @@
 
     if args.gitlab_report:
         with open("gl-code-quality-report.json", "w") as json_file:
             json.dump(gitlab_summary(all_messages), json_file)
 
     if (message_summary.fatal + message_summary.error) > 0:
         sys.exit(1)
-    sys.exit(0)
 
 if __name__ == "__main__":
     main()
```

### Comparing `sca2d-0.2.0/sca2d/definitions.py` & `sca2d-0.2.1/sca2d/definitions.py`

 * *Files identical despite different names*

### Comparing `sca2d-0.2.0/sca2d/lark/scad.lark` & `sca2d-0.2.1/sca2d/lark/scad.lark`

 * *Files identical despite different names*

### Comparing `sca2d-0.2.0/sca2d/messages.py` & `sca2d-0.2.1/sca2d/messages.py`

 * *Files identical despite different names*

### Comparing `sca2d-0.2.0/sca2d/outerscope.py` & `sca2d-0.2.1/sca2d/outerscope.py`

 * *Files identical despite different names*

### Comparing `sca2d-0.2.0/sca2d/sca2d.py` & `sca2d-0.2.1/sca2d/sca2d.py`

 * *Files identical despite different names*

### Comparing `sca2d-0.2.0/sca2d/scadclasses.py` & `sca2d-0.2.1/sca2d/scadclasses.py`

 * *Files identical despite different names*

### Comparing `sca2d-0.2.0/sca2d/scope.py` & `sca2d-0.2.1/sca2d/scope.py`

 * *Files identical despite different names*

### Comparing `sca2d-0.2.0/sca2d/utilities.py` & `sca2d-0.2.1/sca2d/utilities.py`

 * *Files identical despite different names*

### Comparing `sca2d-0.2.0/sca2d.egg-info/PKG-INFO` & `sca2d-0.2.1/sca2d.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 Metadata-Version: 2.1
 Name: sca2d
-Version: 0.2.0
+Version: 0.2.1
 Summary: An experimental static code analyser for OpenSCAD.
 Home-page: https://gitlab.com/bath_open_instrumentation_group/sca2d
 Author: Julian Stirling
 Author-email: julian@julianstirling.co.uk
 License: GPLv3
 Project-URL: Bug Tracker, https://gitlab.com/bath_open_instrumentation_group/sca2d/issues
 Project-URL: Source Code, https://gitlab.com/bath_open_instrumentation_group/sca2d
-Description: # SCA2D - Static Code Analysis for SCAD
-        
-        ![](identity/SCA2D.png)
-        
-        This is an experimental linter for OpenSCAD. The focus is to properly lex the `.scad` files so that we can test for dangerous code like redefining variable from other scopes. SCA2D is in a very early stage of development.
-        
-        ## How to install
-        
-        If you have Python 3.6 or later installed on your machine (and on the PATH) you can install SCA2D from PyPi by running the following command from a terminal
-        
-            pip install sca2d
-        
-        to upgrade your current versions of SCA2D run:
-        
-            pip install sca2d --upgrade
-        
-        You can check that SCA2D is installed by running the following:
-        
-            sca2d -h
-        
-        you should see a help screen.
-        
-        ### Install issues
-        
-        If you have problems with installation possible problems include:
-        
-        * You may need to run `pip3` instead of `pip`
-        * Python may not be on the PATH, this often happens in Windows depending on how python was installed
-        * Python and PIP are on the path but SCA2D isn't. This normally happens if Python is installed through the Windows store. It is best to install Python from [python.org](https://www.python.org/downloads/)
-        
-        ## How to run
-        
-        To analyse a `.scad` file run:
-        
-            sca2d filename.scad
-        This will print any code messages to the screen.
-        
-        To analyse all `.scad` files in a directory run:
-        
-            sca2d directory_path
-        This will also print any code messages to the screen.
-        
-        If you wish to inspect the parse tree that SCA2D generates and then uses you can instead run:
-        
-            sca2d --output-tree filename.scad
-        the tree will be printed into a file called `filename.sca2d`.
-        
-        ## What works
-        
-        * Parsing most `.scad` files. We don't yet to extensive testing. Please raise an issue if you find a parsing error in SCA2D.
-        * Parsing included and used `.scad` files and checking variable, function, and module usage in different scopes.
-        * Checking for a minimal number of code errors
-        
-        ## How to get involved
-        
-        The best way to get involved is to find bugs and then [open an issue](https://gitlab.com/bath_open_instrumentation_group/sca2d/-/issues). You could also make changes and open a merge request.
-        
 Keywords: OpenSCAD,Linting
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# SCA2D - Static Code Analysis for SCAD
+
+![](identity/SCA2D.png)
+
+This is an experimental linter for OpenSCAD. The focus is to properly lex the `.scad` files so that we can test for dangerous code like redefining variable from other scopes. SCA2D is in a very early stage of development.
+
+## How to install
+
+If you have Python 3.6 or later installed on your machine (and on the PATH) you can install SCA2D from PyPi by running the following command from a terminal
+
+    pip install sca2d
+
+to upgrade your current versions of SCA2D run:
+
+    pip install sca2d --upgrade
+
+You can check that SCA2D is installed by running the following:
+
+    sca2d -h
+
+you should see a help screen.
+
+### Install issues
+
+If you have problems with installation possible problems include:
+
+* You may need to run `pip3` instead of `pip`
+* Python may not be on the PATH, this often happens in Windows depending on how python was installed
+* Python and PIP are on the path but SCA2D isn't. This normally happens if Python is installed through the Windows store. It is best to install Python from [python.org](https://www.python.org/downloads/)
+
+## How to run
+
+To analyse a `.scad` file run:
+
+    sca2d filename.scad
+This will print any code messages to the screen.
+
+To analyse all `.scad` files in a directory run:
+
+    sca2d directory_path
+This will also print any code messages to the screen.
+
+If you wish to inspect the parse tree that SCA2D generates and then uses you can instead run:
+
+    sca2d --output-tree filename.scad
+the tree will be printed into a file called `filename.sca2d`.
+
+## What works
+
+* Parsing most `.scad` files. We don't yet to extensive testing. Please raise an issue if you find a parsing error in SCA2D.
+* Parsing included and used `.scad` files and checking variable, function, and module usage in different scopes.
+* Checking for a minimal number of code errors
+
+## How to get involved
+
+The best way to get involved is to find bugs and then [open an issue](https://gitlab.com/bath_open_instrumentation_group/sca2d/-/issues). You could also make changes and open a merge request.
```

### Comparing `sca2d-0.2.0/setup.py` & `sca2d-0.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''Setup for the module'''
 
 __author__ = 'Julian Stirling'
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 import sys
 from os import path
 import glob
 from setuptools import setup, find_packages
 
 def install():
@@ -37,12 +37,14 @@
           url='https://gitlab.com/bath_open_instrumentation_group/sca2d',
           project_urls={"Bug Tracker": "https://gitlab.com/bath_open_instrumentation_group/sca2d/issues",
                         "Source Code": "https://gitlab.com/bath_open_instrumentation_group/sca2d"},
           classifiers=['Development Status :: 5 - Production/Stable',
                        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
                        'Programming Language :: Python :: 3.6'],
           install_requires=['lark-parser', 'colorama'],
+          extras_require={'dev': ['pylint',
+                                  'twine']},
           python_requires=">=3.6",
           entry_points={'console_scripts': ['sca2d = sca2d.__main__:main']})
 
 if __name__ == "__main__":
     install()
```

