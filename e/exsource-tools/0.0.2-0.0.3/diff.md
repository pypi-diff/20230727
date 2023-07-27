# Comparing `tmp/exsource_tools-0.0.2.tar.gz` & `tmp/exsource_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exsource_tools-0.0.2.tar", last modified: Fri May  5 19:48:33 2023, max compression
+gzip compressed data, was "dist/exsource_tools-0.0.3.tar", last modified: Thu Jul 27 12:13:44 2023, max compression
```

## Comparing `exsource_tools-0.0.2.tar` & `exsource_tools-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1352 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/PKG-INFO
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      546 2023-04-17 21:16:27.000000 exsource_tools-0.0.2/README.md
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      132 2023-04-21 09:46:07.000000 exsource_tools-0.0.2/exsource_tools/__init__.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools/schemas/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     5044 2023-05-03 14:26:55.000000 exsource_tools-0.0.2/exsource_tools/schemas/exsource.schema.json
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    25420 2023-05-05 17:35:45.000000 exsource_tools-0.0.2/exsource_tools/tools.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3393 2023-05-03 13:22:06.000000 exsource_tools-0.0.2/exsource_tools/utils.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1352 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/PKG-INFO
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      442 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       61 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/entry_points.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-04-17 12:35:00.000000 exsource_tools-0.0.2/exsource_tools.egg-info/not-zip-safe
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       52 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/requires.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       21 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/top_level.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       38 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/setup.cfg
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2082 2023-04-20 13:26:16.000000 exsource_tools-0.0.2/setup.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/tests/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2023-04-21 09:39:47.000000 exsource_tools-0.0.2/tests/__init__.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2330 2023-04-26 14:40:54.000000 exsource_tools-0.0.2/tests/test_tools.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1352 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/PKG-INFO
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      546 2023-04-17 21:16:27.000000 exsource_tools-0.0.3/README.md
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/exsource_tools/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      132 2023-04-21 09:46:07.000000 exsource_tools-0.0.3/exsource_tools/__init__.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/exsource_tools/schemas/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     5044 2023-05-03 14:26:55.000000 exsource_tools-0.0.3/exsource_tools/schemas/exsource.schema.json
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    26452 2023-07-27 10:27:54.000000 exsource_tools-0.0.3/exsource_tools/tools.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3575 2023-07-27 10:25:57.000000 exsource_tools-0.0.3/exsource_tools/utils.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/exsource_tools.egg-info/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1352 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/exsource_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      442 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/exsource_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/exsource_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       61 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/exsource_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-04-17 12:35:00.000000 exsource_tools-0.0.3/exsource_tools.egg-info/not-zip-safe
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       52 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/exsource_tools.egg-info/requires.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       21 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/exsource_tools.egg-info/top_level.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       38 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/setup.cfg
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2082 2023-07-27 12:12:10.000000 exsource_tools-0.0.3/setup.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-07-27 12:13:43.000000 exsource_tools-0.0.3/tests/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2023-04-21 09:39:47.000000 exsource_tools-0.0.3/tests/__init__.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2330 2023-04-26 14:40:54.000000 exsource_tools-0.0.3/tests/test_tools.py
```

### Comparing `exsource_tools-0.0.2/PKG-INFO` & `exsource_tools-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exsource_tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python tools for using Exsource files
 Home-page: https://gitlab.com/gitbuilding/exsource-tools
 Author: Julian Stirling
 Author-email: julian@julianstirling.co.uk
 License: LGPLv3
 Project-URL: Bug Tracker, https://gitlab.com/gitbuilding/exsource-tools/issues
 Project-URL: Source Code, https://gitlab.com/gitbuilding/exsource-tools
```

### Comparing `exsource_tools-0.0.2/README.md` & `exsource_tools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `exsource_tools-0.0.2/exsource_tools/schemas/exsource.schema.json` & `exsource_tools-0.0.3/exsource_tools/schemas/exsource.schema.json`

 * *Files identical despite different names*

### Comparing `exsource_tools-0.0.2/exsource_tools/tools.py` & `exsource_tools-0.0.3/exsource_tools/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,32 +310,34 @@
         return self._name
 
     @name.setter
     def name(self, value):
         """
         Set the export name. This is the human freindly name.
         """
-        if not isinstance(value, str):
-            raise TypeError("Name must be a string")
+        if value is not None:
+            if not isinstance(value, str):
+                raise TypeError("Name must be a string")
         self._name = value
 
     @property
     def description(self):
         """
         Return the description of the export
         """
         return self._description
 
     @description.setter
     def description(self, value):
         """
         Set the export description. This is the human freindly description.
         """
-        if not isinstance(value, str):
-            raise TypeError("Description must be a string")
+        if value is not None:
+            if not isinstance(value, str):
+                raise TypeError("Description must be a string")
         self._description = value
 
     @property
     def parameters(self):
         """
         Return the parameters to be used for export
         """
@@ -491,16 +493,19 @@
     Create the argument parser for the exsource-make command
     """
     description = "Process exsource file to create inputs."
     parser = argparse.ArgumentParser(description=description,
                                      formatter_class=argparse.RawTextHelpFormatter)
     def_help = "Path to ExSource definition file. Default is exsource-def.yml or exsource-def.json"
     parser.add_argument("-d", "--exsource-def", help=def_help)
-    def_help = "Path to ExSource output file. Default is exsource-out.yml or exsource-out.json"
-    parser.add_argument("-o", "--exsource-out", help=def_help)
+    out_help = "Path to ExSource output file. Default is exsource-out.yml or exsource-out.json"
+    parser.add_argument("-o", "--exsource-out", help=out_help)
+    headless_help = ("Set this flag on machines without an X server running. Commands "
+                     "requring X will be run with xvfb. Ensure xvfb is installed.")
+    parser.add_argument("-H", "--headless", action='store_true', help=headless_help)
     return parser
 
 def find_def_file():
     """
     Find the exsource definition file in the current directory.
     """
     default_names = ["exsource-def.yml", "exsource-def.yaml", "exsource-def.json"]
@@ -538,24 +543,30 @@
     if out_filepath is None:
         out_filepath = find_out_file()
 
     out_file = None
     if out_filepath is not None and path.exists(out_filepath):
         out_file = load_exsource_file(out_filepath)
 
-    processor = ExSourceProcessor(def_file, out_file, out_filepath)
+    processor = ExSourceProcessor(def_file, out_file, out_filepath, args.headless)
     processor.make()
 
 class ExSourceProcessor:
     """
     This class processes the data in the exsource file to create all the ouputs.
     Currently it only works for certain OpenSCAD and FreeCAD exports
     """
 
-    def __init__(self, exsource_def, previous_exsource=None, exsource_out_path=None):
+    def __init__(self,
+                 exsource_def,
+                 previous_exsource=None,
+                 exsource_out_path=None,
+                 headless=False):
+
+        self.headless = headless
         self._exsource = deepcopy(exsource_def)
         self._exsource_prev = previous_exsource
         self._exsource_out_path = exsource_out_path
         self._all_output_files = {output.filepath: UNSTAGED for output in self._exsource.all_output_files}
 
     def make(self):
         """
@@ -589,16 +600,16 @@
             if dep_action == CONTINUE:
                 if app.lower() == "openscad":
                     self._process_openscad(export)
                 elif app.lower() == "freecad":
                     self._process_freecad(export)
                 else:
                     LOGGER.warning("Skipping %s as no methods available process files with %s",
-                                export_id,
-                                app)
+                                   export_id,
+                                   app)
                     for output in export.output_files:
                         self._all_output_files[output.filepath] = SKIPPED
             elif dep_action == SKIP:
                 for output in export.output_files:
                     self._all_output_files[output.filepath] = SKIPPED
                 LOGGER.warning("Skipping %s it has skipped dependencies", export_id)
             elif dep_action == DELAY:
@@ -638,19 +649,22 @@
                     action = DELAY
                     #No return here as another dependency might require it be skipped
 
         return action
 
     def _process_openscad(self, export):
         #TODO: Tidy up
-        assert len(export.output_files)==1, "OpenSCAD expects only one output"
+        assert len(export.output_files) == 1, "OpenSCAD expects only one output"
         output = export.output_files[0]
-        assert len(export.source_files)==1, "Openscad expects only one source file"
+        assert len(export.source_files) == 1, "Openscad expects only one source file"
         source = export.source_files[0]
 
+        require_x = True if output.filepath.lower().endswith('.png') else False
+
+
         params = []
         for parameter in export.parameters:
             if isinstance(export.parameters[parameter], (float, int)):
                 par = str(export.parameters[parameter])
             elif isinstance(export.parameters[parameter], bool):
                 #ensure lowercase for booleans
                 par = str(export.parameters[parameter]).lower()
@@ -662,51 +676,61 @@
                 continue
             params.append("-D")
             params.append(f"{parameter}={par}")
 
         executable = "openscad"
 
         depfilename = output.filepath + ".d"
+        utils.add_directory_if_needed(output.filepath)
         openscad_file_args = ["-d", depfilename, "-o", output.filepath, source.filepath]
         openscad_args = export.app_options + params + openscad_file_args
         try:
-            ret = subprocess.run([executable] + openscad_args, check=True, capture_output=True)
+            if self.headless and require_x:
+                xrvb_args = ['xvfb-run',
+                             '--auto-servernum',
+                             '--server-args',
+                             '-screen 0 1024x768x24']
+                args = xrvb_args + [executable] + openscad_args
+            else:
+                args = [executable] + openscad_args
+            ret = subprocess.run(args, check=True, capture_output=True)
             #print std_err as OpenSCAD uses it to print rather than std_out
             std_err = ret.stderr.decode('UTF-8')
             print(std_err)
         except subprocess.CalledProcessError as error:
             std_err = error.stderr.decode('UTF-8')
             raise RuntimeError(f"\n\nOpenSCAD failed create file: {output} with error:\n\n"
                                f"{std_err}") from error
         output.store_hash()
         depsfile = utils.Depsfile(depfilename)
-        assert len(depsfile.rules)==1, "Expecting only one rule in and openscad deps file"
-        assert len(depsfile.rules[0].outputs)==1, "Expecting only one output to be specified in the openscad depsile"
-        assert depsfile.rules[0].outputs[0]==output, "depsfile output doens't match expected file"
+        assert len(depsfile.rules) == 1, "Expecting only one rule in and openscad deps file"
+        assert len(depsfile.rules[0].outputs) == 1, "Expecting only one output to be specified in the openscad depsile"
+        assert depsfile.rules[0].outputs[0] == output, "depsfile output doens't match expected file"
         for dep in depsfile.rules[0].dependencies:
             if dep not in export.source_files+export.dependencies:
                 export.add_dependency(dep, store_hash=True)
         export.mark_dependencies_exhaustive()
         self._all_output_files[output.filepath] = PROCESSED
 
     def _process_freecad(self, export):
         #TODO: Tidy up
 
         outputs = export.output_files
         sources = export.source_files
-        assert len(sources)==1, "FreeCAD expects only one source file"
+        assert len(sources) == 1, "FreeCAD expects only one source file"
         sourcefile = sources[0].filepath
-        assert len(export.app_options)==0, "Cannot apply options to FreeCAD"
+        assert len(export.app_options) == 0, "Cannot apply options to FreeCAD"
         for parameter in export.parameters:
             LOGGER.info("Cannot process parameters for FreeCAD skipping parameter %s",
                         parameter)
             continue
 
         for outfile_obj in outputs:
             outfile = outfile_obj.filepath
+            utils.add_directory_if_needed(outfile_obj.filepath)
             if outfile.lower().endswith('.stp') or outfile.lower().endswith('.step'):
                 macro = (f"doc = FreeCAD.openDocument('{sourcefile}')\n"
                          "body = doc.getObject('Body')\n"
                          f"body.Shape.exportStep('{outfile}')\n")
             elif outfile.lower().endswith('.stl'):
                 macro = ("from FreeCAD import Mesh\n"
                          f"doc = FreeCAD.openDocument('{sourcefile}')\n"
@@ -715,7 +739,8 @@
             tmpdir = gettempdir()
             macropath = path.join(tmpdir, "export.FCMacro")
             with open(macropath, 'w', encoding="utf-8") as file_obj:
                 file_obj.write(macro)
             subprocess.run(["freecadcmd", macropath], check=True)
             outfile_obj.store_hash()
             self._all_output_files[outfile] = PROCESSED
+
```

### Comparing `exsource_tools-0.0.2/exsource_tools/utils.py` & `exsource_tools-0.0.3/exsource_tools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 This file contains misc utilities
 """
 
 import re
-from os import path
+import os
 
 class DependencyRule:
     """
     Class to store a single dependency rule
     """
 
     def __init__(self, outputs, dependencies):
 
-        self._outputs = [path.relpath(output) for output in outputs]
-        self._dependencies = [path.relpath(dep) for dep in dependencies]
+        self._outputs = [os.path.relpath(output) for output in outputs]
+        self._dependencies = [os.path.relpath(dep) for dep in dependencies]
 
     @property
     def outputs(self):
         """
         Returns the list of the outputs specified in the dependency rule
         """
         return self._outputs
@@ -101,7 +101,13 @@
             else:
                 if item.endswith(":"):
                     colon_delimeter_found = True
                     outputs.append(item[:-1])
                 else:
                     outputs.append(item)
         self._rules.append(DependencyRule(outputs, deps))
+
+def add_directory_if_needed(filepath):
+    directory = os.path.dirname(filepath)
+    if not directory == "":
+        if not os.path.exists(directory):
+            os.makedirs(directory)
```

### Comparing `exsource_tools-0.0.2/exsource_tools.egg-info/PKG-INFO` & `exsource_tools-0.0.3/exsource_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exsource-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python tools for using Exsource files
 Home-page: https://gitlab.com/gitbuilding/exsource-tools
 Author: Julian Stirling
 Author-email: julian@julianstirling.co.uk
 License: LGPLv3
 Project-URL: Bug Tracker, https://gitlab.com/gitbuilding/exsource-tools/issues
 Project-URL: Source Code, https://gitlab.com/gitbuilding/exsource-tools
```

### Comparing `exsource_tools-0.0.2/setup.py` & `exsource_tools-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''Setup for the module'''
 
 __author__ = 'Julian Stirling'
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 import sys
 from os import path
 import glob
 from setuptools import setup, find_packages
 
 def install():
```

### Comparing `exsource_tools-0.0.2/tests/test_tools.py` & `exsource_tools-0.0.3/tests/test_tools.py`

 * *Files identical despite different names*

