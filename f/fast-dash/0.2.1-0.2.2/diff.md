# Comparing `tmp/fast_dash-0.2.1.tar.gz` & `tmp/fast_dash-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dash-0.2.1.tar", max compression
+gzip compressed data, was "fast_dash-0.2.2.tar", max compression
```

## Comparing `fast_dash-0.2.1.tar` & `fast_dash-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-07-24 00:13:17.063369 fast_dash-0.2.1/LICENSE
--rw-r--r--   0        0        0     3824 2023-07-24 00:13:17.063369 fast_dash-0.2.1/README.md
--rw-r--r--   0        0        0    34285 2023-07-24 00:13:17.191369 fast_dash-0.2.1/fast_dash/Components.py
--rw-r--r--   0        0        0      635 2023-07-24 00:13:17.191369 fast_dash-0.2.1/fast_dash/__init__.py
--rw-r--r--   0        0        0    24457 2023-07-24 00:13:17.191369 fast_dash-0.2.1/fast_dash/assets/favicon.ico
--rw-r--r--   0        0        0    17290 2023-07-24 00:13:17.191369 fast_dash-0.2.1/fast_dash/fast_dash.py
--rw-r--r--   0        0        0     7667 2023-07-24 00:13:17.191369 fast_dash-0.2.1/fast_dash/utils.py
--rw-r--r--   0        0        0     2325 2023-07-24 00:13:17.195369 fast_dash-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       39 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      314 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     3538 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/examples.py
--rw-r--r--   0        0        0     2709 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/test_examples.py
--rw-r--r--   0        0        0     6261 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/test_fast_dash.py
--rw-r--r--   0        0        0    21632 2023-07-24 00:13:17.195369 fast_dash-0.2.1/tests/test_fast_dash_autodetect.py
--rw-r--r--   0        0        0     5081 1970-01-01 00:00:00.000000 fast_dash-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-26 23:53:13.759936 fast_dash-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3824 2023-07-26 23:53:13.759936 fast_dash-0.2.2/README.md
+-rw-r--r--   0        0        0    34285 2023-07-26 23:53:13.803936 fast_dash-0.2.2/fast_dash/Components.py
+-rw-r--r--   0        0        0      655 2023-07-26 23:53:13.803936 fast_dash-0.2.2/fast_dash/__init__.py
+-rw-r--r--   0        0        0    24457 2023-07-26 23:53:13.807936 fast_dash-0.2.2/fast_dash/assets/favicon.ico
+-rw-r--r--   0        0        0    17282 2023-07-26 23:53:13.807936 fast_dash-0.2.2/fast_dash/fast_dash.py
+-rw-r--r--   0        0        0     7667 2023-07-26 23:53:13.807936 fast_dash-0.2.2/fast_dash/utils.py
+-rw-r--r--   0        0        0     2325 2023-07-26 23:53:13.807936 fast_dash-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      314 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     3538 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/examples.py
+-rw-r--r--   0        0        0     2709 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/test_examples.py
+-rw-r--r--   0        0        0     6261 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/test_fast_dash.py
+-rw-r--r--   0        0        0    21632 2023-07-26 23:53:13.807936 fast_dash-0.2.2/tests/test_fast_dash_autodetect.py
+-rw-r--r--   0        0        0     5081 1970-01-01 00:00:00.000000 fast_dash-0.2.2/PKG-INFO
```

### Comparing `fast_dash-0.2.1/LICENSE` & `fast_dash-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.1/README.md` & `fast_dash-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.1/fast_dash/Components.py` & `fast_dash-0.2.2/fast_dash/Components.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.1/fast_dash/__init__.py` & `fast_dash-0.2.2/fast_dash/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Top-level package for Fast Dash."""
 
 __author__ = """Kedar Dabhadkar"""
 __email__ = "kedar@fastdash.app"
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 from fast_dash.Components import (
     Graph,
     Image,
     Slider,
     Text,
     TextArea,
     Upload,
     UploadImage,
     acknowledge_image_component,
     dbc,
     dcc,
+    dmc,
     html,
 )
 from fast_dash.fast_dash import FastDash, fastdash
 from fast_dash.utils import Fastify
 
 __all__ = [
     "FastDash",
@@ -30,9 +31,10 @@
     "Upload",
     "acknowledge_image_component",
     "UploadImage",
     "Image",
     "Graph",
     "dcc",
     "dbc",
+    "dmc",
     "html",
 ]
```

### Comparing `fast_dash-0.2.1/fast_dash/assets/favicon.ico` & `fast_dash-0.2.2/fast_dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.1/fast_dash/fast_dash.py` & `fast_dash-0.2.2/fast_dash/fast_dash.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import logging
 import re
 import warnings
 
 import dash
 import dash_bootstrap_components as dbc
 import flask
-from dash import Input, Output
+from dash import Input, Output, ctx
+from dash.exceptions import PreventUpdate
 
 from .Components import (
     BaseLayout,
     SidebarLayout,
     Text,
     _infer_input_components,
     _infer_output_components,
@@ -293,41 +294,40 @@
             + [
                 Input(component_id="reset_inputs", component_property="n_clicks"),
                 Input(component_id="submit_inputs", component_property="n_clicks"),
             ],
             prevent_initial_callback=True,
         )
         def process_input(*args):
-            reset_button = args[-2]
-            submit_button = args[-1]
+            # if ctx.triggered_id not in ["submit_inputs", "reset_inputs"]:
+            #     raise PreventUpdate
+
             ack_components = [
                 ack if mask is True else None
                 for mask, ack in zip(self.ack_mask, list(args[:-2]))
             ]
 
-            if submit_button > self.submit_clicks or (
+            if ctx.triggered_id == "submit_inputs" or (
                 self.update_live is True and None not in args
             ):
                 self.app_initialized = True
-                self.submit_clicks = submit_button
                 output_state = self.callback_fn(*args[:-2])
 
                 if isinstance(output_state, tuple):
                     self.output_state = list(output_state)
 
                 else:
                     self.output_state = [output_state]
 
                 # Transform outputs to fit in the desired components
                 self.output_state = _transform_outputs(self.output_state)
 
                 return self.output_state + ack_components
 
-            elif reset_button > self.reset_clicks:
-                self.reset_clicks = reset_button
+            elif ctx.triggered_id == "reset_inputs":
                 self.output_state = self.output_state_default
                 return self.output_state + ack_components
 
             elif self.app_initialized:
                 return self.output_state + ack_components
 
             else:
```

### Comparing `fast_dash-0.2.1/fast_dash/utils.py` & `fast_dash-0.2.2/fast_dash/utils.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.1/pyproject.toml` & `fast_dash-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "fast_dash"
-version = "0.2.1"
+version = "0.2.2"
 homepage = "https://github.com/dkedar7/fast_dash"
 description = "Build Machine Learning prototypes web applications lightning fast."
 authors = ["Kedar Dabhadkar <kedar@fastdash.app>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 4 - Beta',
```

### Comparing `fast_dash-0.2.1/tests/examples.py` & `fast_dash-0.2.2/tests/examples.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.1/tests/test_examples.py` & `fast_dash-0.2.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.1/tests/test_fast_dash.py` & `fast_dash-0.2.2/tests/test_fast_dash.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.1/tests/test_fast_dash_autodetect.py` & `fast_dash-0.2.2/tests/test_fast_dash_autodetect.py`

 * *Files identical despite different names*

### Comparing `fast_dash-0.2.1/PKG-INFO` & `fast_dash-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-dash
-Version: 0.2.1
+Version: 0.2.2
 Summary: Build Machine Learning prototypes web applications lightning fast.
 Home-page: https://github.com/dkedar7/fast_dash
 License: MIT
 Author: Kedar Dabhadkar
 Author-email: kedar@fastdash.app
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

