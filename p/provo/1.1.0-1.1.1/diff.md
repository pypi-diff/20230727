# Comparing `tmp/provo-1.1.0.tar.gz` & `tmp/provo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "provo-1.1.0.tar", last modified: Mon Jun 26 15:30:59 2023, max compression
+gzip compressed data, was "provo-1.1.1.tar", last modified: Thu Jul 27 12:44:34 2023, max compression
```

## Comparing `provo-1.1.0.tar` & `provo-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-26 15:30:59.951288 provo-1.1.0/
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1070 2023-06-23 06:54:13.000000 provo-1.1.0/LICENSE
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      515 2023-06-26 15:30:59.951288 provo-1.1.0/PKG-INFO
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    25679 2023-06-26 14:25:22.000000 provo-1.1.0/README.md
-drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-26 15:30:59.947288 provo-1.1.0/provo/
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       54 2023-06-23 06:54:13.000000 provo-1.1.0/provo/__init__.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     3627 2023-06-26 15:24:38.000000 provo-1.1.0/provo/idvault.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    25046 2023-06-26 14:28:15.000000 provo-1.1.0/provo/provontologygraph.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    10519 2023-06-26 14:19:28.000000 provo-1.1.0/provo/startingpointclasses.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      442 2023-06-23 06:54:13.000000 provo-1.1.0/provo/staticfunctions.py
-drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-26 15:30:59.951288 provo-1.1.0/provo/tests/
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-23 06:54:13.000000 provo-1.1.0/provo/tests/__init__.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1363 2023-06-23 06:54:13.000000 provo-1.1.0/provo/tests/test_provenance_graph.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     4777 2023-06-26 15:25:26.000000 provo-1.1.0/provo/tests/test_rdf_output.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     3332 2023-06-23 06:54:13.000000 provo-1.1.0/provo/tests/test_starting_point_classes.py
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1423 2023-06-26 15:28:25.000000 provo-1.1.0/provo/tests/test_vault.py
-drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-26 15:30:59.951288 provo-1.1.0/provo.egg-info/
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      515 2023-06-26 15:30:59.000000 provo-1.1.0/provo.egg-info/PKG-INFO
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      448 2023-06-26 15:30:59.000000 provo-1.1.0/provo.egg-info/SOURCES.txt
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        1 2023-06-26 15:30:59.000000 provo-1.1.0/provo.egg-info/dependency_links.txt
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       23 2023-06-26 15:30:59.000000 provo-1.1.0/provo.egg-info/requires.txt
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        6 2023-06-26 15:30:59.000000 provo-1.1.0/provo.egg-info/top_level.txt
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       38 2023-06-26 15:30:59.951288 provo-1.1.0/setup.cfg
--rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      862 2023-06-26 14:25:41.000000 provo-1.1.0/setup.py
+drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-07-27 12:44:34.989484 provo-1.1.1/
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1070 2023-06-23 06:54:13.000000 provo-1.1.1/LICENSE
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      515 2023-07-27 12:44:34.989484 provo-1.1.1/PKG-INFO
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    25859 2023-07-27 11:28:09.000000 provo-1.1.1/README.md
+drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-07-27 12:44:34.985484 provo-1.1.1/provo/
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       54 2023-06-23 06:54:13.000000 provo-1.1.1/provo/__init__.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     3627 2023-06-26 15:24:38.000000 provo-1.1.1/provo/idvault.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    23251 2023-07-27 12:39:44.000000 provo-1.1.1/provo/provontologygraph.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    10519 2023-06-26 14:19:28.000000 provo-1.1.1/provo/startingpointclasses.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      572 2023-07-27 12:01:09.000000 provo-1.1.1/provo/staticfunctions.py
+drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-07-27 12:44:34.989484 provo-1.1.1/provo/tests/
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-23 06:54:13.000000 provo-1.1.1/provo/tests/__init__.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1363 2023-06-23 06:54:13.000000 provo-1.1.1/provo/tests/test_provenance_graph.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     4777 2023-06-26 15:25:26.000000 provo-1.1.1/provo/tests/test_rdf_output.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     3332 2023-06-23 06:54:13.000000 provo-1.1.1/provo/tests/test_starting_point_classes.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1423 2023-06-26 15:28:25.000000 provo-1.1.1/provo/tests/test_vault.py
+drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-07-27 12:44:34.985484 provo-1.1.1/provo.egg-info/
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      515 2023-07-27 12:44:34.000000 provo-1.1.1/provo.egg-info/PKG-INFO
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      448 2023-07-27 12:44:34.000000 provo-1.1.1/provo.egg-info/SOURCES.txt
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        1 2023-07-27 12:44:34.000000 provo-1.1.1/provo.egg-info/dependency_links.txt
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       23 2023-07-27 12:44:34.000000 provo-1.1.1/provo.egg-info/requires.txt
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        6 2023-07-27 12:44:34.000000 provo-1.1.1/provo.egg-info/top_level.txt
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       38 2023-07-27 12:44:34.989484 provo-1.1.1/setup.cfg
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      862 2023-07-27 12:44:22.000000 provo-1.1.1/setup.py
```

### Comparing `provo-1.1.0/LICENSE` & `provo-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `provo-1.1.0/PKG-INFO` & `provo-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: provo
-Version: 1.1.0
+Version: 1.1.1
 Summary: Construct  PROV-O compliant provenance graphs.
 Home-page: https://github.com/rue-a/provo
 Author: Arne Rümmler
 Author-email: arne.ruemmler@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `provo-1.1.0/README.md` & `provo-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,18 @@
 If the markdown interpreter supports mermaid, this results in:
 
 ```mermaid
 flowchart LR
     entity_id[Entity] -- was generated by --> activity_id[Activity]
 ```
 
+> **Note**
+> To convert Mermaid charts into other formats the software [`mermaid-cli`](https://github.com/mermaid-js/mermaid-cli) is recommended.
+> You can also use the [Mermaid Live Editor](https://mermaid.live/) to edit (and convert) the document.
+
 To export the provenance graph as mermaid chart call the according export method:
 
 ```python
 # ex5
 
 prov_ontology_graph.export_as_mermaid_flowchart(file_name="examples/manual_examples_flowchart_default.md")
 ```
@@ -251,15 +255,15 @@
 The style of the resulting graph is defined by a dictionary that holds the default style values. To change the styling, a dictionary can be passed to the method by using the `user_options` argument. If this is done, the configurations that are defined in the user options overwrite the according default configurations. A reference and some more details concerning the options dictionary can be found below.
 
 ```python
 # ex6
 
 options = {
     "orientation": "LR",
-    "revert-relations": True,
+    "invert-relations": True,
     "activity": {
         "fill": "#89e6dc",
         "shape": "{{:}}"
     }
 }
 
 prov_ontology_graph.export_as_mermaid_flowchart(
@@ -290,15 +294,15 @@
 
 #### User Options Reference
 
 The default styling configuration mimics the graph styling from the PROV-O reference page and is defined as follows:
 
 ```python
 options = {
-    "revert-relations": False,
+    "invert-relations": False,
     "orientation": "TD",            
     "included-relations": [
         "was_generated_by",
         "was_attributed_to",
         "used",
         "was_associated_with",
         "acted_on_behalf_of"
@@ -332,28 +336,28 @@
         "stroke-width": None
     }
 }
 ```
 
 __Reference Table__
 
-| keyword            | options                                     | explanation                                                                                                                                                                                                                                                          |
-|--------------------|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| revert-relations   | True \| False                               | Reverts the arrows and changes the labels accordingly. The reverted labels are not defined by PROV, and thus they are not compliant to the PROV model.                                                                                                               |
-| orientation        | "TD" \| "LR"                                | Top-down or left-right orientation of the graph (mermaid syntax).                                                                                                                                                                                                    |
-| included-relations | list of displayed relations                 | Defines which relations should be displayed. Per default "was_derived_by" and "was_informed_by" are excluded. Possible values are: "was_generated_by", was_derived_by", "was_attributed_to", "used", "was_informed_by", "was_associated_with", "acted_on_behalf_of". |
+| keyword            | options                               | explanation                                                                                                                                                                                                                                                          |
+| ------------------ | ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| invert-relations   | True \| False                         | Reverts the arrows and changes the labels accordingly. The reverted labels are not defined by PROV, and thus they are not compliant to the PROV model.                                                                                                               |
+| orientation        | "TD" \| "LR"                          | Top-down or left-right orientation of the graph (mermaid syntax).                                                                                                                                                                                                    |
+| included-relations | list of displayed relations           | Defines which relations should be displayed. Per default "was_derived_by" and "was_informed_by" are excluded. Possible values are: "was_generated_by", was_derived_by", "was_attributed_to", "used", "was_informed_by", "was_associated_with", "acted_on_behalf_of". |
 | fill               | "\<#color-hex-code\>", e.g. "#fffedf" | Defines the color of the nodes.                                                                                                                                                                                                                                      |
-| shape              | "\<shape identifier\>", e.g. "[:]"            | Uses [mermaid shape syntax](https://mermaid-js.github.io/mermaid/#/flowchart?id=node-shapes). The colon separates the opening symbols from the closing symbols.                                                                                                      |
-| color              |  "\<#color-hex-code\>"                |  Defines the color of the nodes' texts.                                                                                                                                                                                                                              |
-|  stroke            |  "\<#color-hex-code\>"                |  Defines the color of the nodes' borders                                                                                                                                                                                                                             |
-|  stroke-width      |  "\<border width in px\>", e.g. "1px"         |  Defines the width of the nodes' borders.                                                                                                                                                                                                                            |
-| relation-style     | "-" (solid) \| "." (dashed)                 | Defines the style of the relations. Only two options are available.                                                                                                                                                                                                  |
-| entity             | dict                                        | Specify fill, shape, color, stroke, stroke-with and relation-style for entities. If any value is `None`, it falls back to the op level definitions                                                                                                                    |
-| activity           | dict                                        | see entity                                                                                                                                                                                                                                                           |
-| agent              | dict                                        | see entity                                                                                                                                                                                                                                                           |
+| shape              | "\<shape identifier\>", e.g. "[:]"    | Uses [mermaid shape syntax](https://mermaid-js.github.io/mermaid/#/flowchart?id=node-shapes). The colon separates the opening symbols from the closing symbols.                                                                                                      |
+| color              | "\<#color-hex-code\>"                 | Defines the color of the nodes' texts.                                                                                                                                                                                                                               |
+| stroke             | "\<#color-hex-code\>"                 | Defines the color of the nodes' borders                                                                                                                                                                                                                              |
+| stroke-width       | "\<border width in px\>", e.g. "1px"  | Defines the width of the nodes' borders.                                                                                                                                                                                                                             |
+| relation-style     | "-" (solid) \| "." (dashed)           | Defines the style of the relations. Only two options are available.                                                                                                                                                                                                  |
+| entity             | dict                                  | Specify fill, shape, color, stroke, stroke-with and relation-style for entities. If any value is `None`, it falls back to the op level definitions                                                                                                                   |
+| activity           | dict                                  | see entity                                                                                                                                                                                                                                                           |
+| agent              | dict                                  | see entity                                                                                                                                                                                                                                                           |
 
 If further styling configuration is required, users have to interact directly with the resulting mermaid-md.
 
 
 ## Comprehensive Examples
 
 Code to create the PROV-O [example 1](https://www.w3.org/TR/prov-o/#narrative-example-simple-1)
@@ -545,15 +549,15 @@
 http://example.org#derek-. acted on behalf of .->http://example.org#national_newspaper_inc
 ```
 
 __User defined mermaid graph:__
 
 ```python
 options = {
-    "revert-relations": True,
+    "invert-relations": True,
     "entity": {
         "shape": "[:]",
         "fill": "#FC766AFF",
         "stroke": "#FC766AFF",
         "color": "333"
     },
     "agent": {
```

### Comparing `provo-1.1.0/provo/idvault.py` & `provo-1.1.1/provo/idvault.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.0/provo/provontologygraph.py` & `provo-1.1.1/provo/provontologygraph.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Namespace,
     URIRef,
 )
 from validators import url
 
 from provo.idvault import IdVault
 from provo.startingpointclasses import Activity, Agent, Entity
-from provo.staticfunctions import update_dict
+from provo.staticfunctions import update_dict, get_option
 
 
 @dataclass(frozen=True)
 class NamespaceMalformed(Exception):
     """Raised when the namespace is not a valid URL."""
 
     message: str
@@ -354,16 +354,16 @@
 
     def export_as_mermaid_flowchart(
         self, file_name: str, user_options: dict = {}
     ) -> None:
         """exports the contents of the graph as mermaid-md flowchart"""
 
         # if possible the options use the mermaid terminology
-        options = {
-            "revert-relations": False,
+        default_options = {
+            "invert-relations": False,
             "orientation": "TD",
             "included-relations": [
                 "was_generated_by",
                 "was_attributed_to",
                 "used",
                 "was_associated_with",
                 "acted_on_behalf_of",
@@ -394,177 +394,173 @@
                 "relation-style": ".",
                 "color": None,
                 "stroke": None,
                 "stroke-width": None,
             },
         }
 
-        options = update_dict(options, user_options)
+         # Update default options with user options
+        options = update_dict(default_options, user_options)
 
+        # Unpack commonly used option values
         text_color = options["color"]
         stroke_color = options["stroke"]
         stroke_width = options["stroke-width"]
         stroke_style = options["relation-style"]
 
-        entity_text_color = options["entity"]["color"]
-        entity_stroke_color = options["entity"]["stroke"]
-        entity_stroke_width = options["entity"]["stroke-width"]
-        entity_stroke_style = options["entity"]["relation-style"]
-
-        activity_text_color = options["activity"]["color"]
-        activity_stroke_color = options["activity"]["stroke"]
-        activity_stroke_width = options["activity"]["stroke-width"]
-        activity_stroke_style = options["activity"]["relation-style"]
-
-        agent_text_color = options["agent"]["color"]
-        agent_stroke_color = options["agent"]["stroke"]
-        agent_stroke_width = options["agent"]["stroke-width"]
-        agent_stroke_style = options["agent"]["relation-style"]
+        # Unpack entity options
+        entity_opts = options["entity"]
+        entity_fill_color = entity_opts["fill"]
+        entity_text_color = entity_opts["color"] or text_color
+        entity_stroke_color = entity_opts["stroke"] or stroke_color
+        entity_stroke_width = entity_opts["stroke-width"] or stroke_width
+        entity_stroke_style = entity_opts["relation-style"] or stroke_style
+
+        # Unpack activity options
+        activity_opts = options["activity"]
+        activity_fill_color = activity_opts["fill"]
+        activity_text_color = activity_opts["color"] or text_color
+        activity_stroke_color = activity_opts["stroke"] or stroke_color
+        activity_stroke_width = activity_opts["stroke-width"] or stroke_width
+        activity_stroke_style = activity_opts["relation-style"] or stroke_style
+
+        # Unpack agent options
+        agent_opts = options["agent"]
+        agent_fill_color = agent_opts["fill"]
+        agent_text_color = agent_opts["color"] or text_color
+        agent_stroke_color = agent_opts["stroke"] or stroke_color
+        agent_stroke_width = agent_opts["stroke-width"] or stroke_width
+        agent_stroke_style = agent_opts["relation-style"] or stroke_style
+
+
 
         lines = []
         lines.append("```mermaid")
         lines.append(f"flowchart {options['orientation']}")
 
-        lines.append(f"classDef entity fill:{options['entity']['fill']}")
+        # Class definitions for entities
+        lines.append(f"classDef entity fill:{entity_fill_color}")
         if entity_text_color:
-            lines.append(f"classDef entity color:{options['entity']['color']}")
-        elif text_color:
-            lines.append(f"classDef entity color:{options['color']}")
+            lines.append(f"classDef entity color:{entity_text_color}")
         if entity_stroke_color:
-            lines.append(
-                f"classDef entity stroke:{options['entity']['stroke']}")
-        elif stroke_color:
-            lines.append(f"classDef entity stroke:{options['stroke']}")
+            lines.append(f"classDef entity stroke:{entity_stroke_color}")
         if entity_stroke_width:
-            lines.append(
-                f"classDef entity stroke-width:{options['entity']['stroke-width']}"
-            )
-        elif stroke_width:
-            lines.append(
-                f"classDef entity stroke-width:{options['stroke-width']}")
+            lines.append(f"classDef entity stroke-width:{entity_stroke_width}")
 
-        lines.append(f"classDef activity fill:{options['activity']['fill']}")
+        # Class definitions for activities
+        lines.append(f"classDef activity fill:{activity_fill_color}")
         if activity_text_color:
-            lines.append(
-                f"classDef activity color:{options['activity']['color']}")
-        elif text_color:
-            lines.append(f"classDef activity color:{options['color']}")
+            lines.append(f"classDef activity color:{activity_text_color}")
         if activity_stroke_color:
-            lines.append(
-                f"classDef activity stroke:{options['activity']['stroke']}")
-        elif stroke_color:
-            lines.append(f"classDef activity stroke:{options['stroke']}")
+            lines.append(f"classDef activity stroke:{activity_stroke_color}")
         if activity_stroke_width:
-            lines.append(
-                f"classDef activity stroke-width:{options['activity']['stroke-width']}"
-            )
-        elif stroke_width:
-            lines.append(
-                f"classDef activity stroke-width:{options['stroke-width']}")
+            lines.append(f"classDef activity stroke-width:{activity_stroke_width}")
 
-        lines.append(f"classDef agent fill:{options['agent']['fill']}")
+        # Class definitions for agents
+        lines.append(f"classDef agent fill:{agent_fill_color}")
         if agent_text_color:
-            lines.append(f"classDef agent color:{options['agent']['color']}")
-        elif text_color:
-            lines.append(f"classDef agent color:{options['color']}")
+            lines.append(f"classDef agent color:{agent_text_color}")
         if agent_stroke_color:
-            lines.append(f"classDef agent stroke:{options['agent']['stroke']}")
-        elif stroke_color:
-            lines.append(f"classDef agent stroke:{options['stroke']}")
+            lines.append(f"classDef agent stroke:{agent_stroke_color}")
         if agent_stroke_width:
-            lines.append(
-                f"classDef agent stroke-width:{options['agent']['stroke-width']}"
-            )
-        elif stroke_width:
-            lines.append(
-                f"classDef agent stroke-width:{options['stroke-width']}")
+            lines.append(f"classDef agent stroke-width:{agent_stroke_width}")
 
         for entity in self._entities:
             lines.append(
-                f'{entity.node_id}{options["entity"]["shape"].split(":")[0]}<a style=color:inherit href={entity.node_id}>{entity.label if entity.label else entity.node_id}</a>{options["entity"]["shape"].split(":")[1]}:::entity'
+                f'{entity.node_id}{options["entity"]["shape"].split(":")[0]}<a style=color:inherit href={entity.node_id}>{entity.label or entity.node_id}</a>{options["entity"]["shape"].split(":")[1]}:::entity'
             )
             if "was_derived_by" in options["included-relations"]:
-                for item in entity._was_derived_from_entities:
-                    if not options["revert-relations"]:
+                attrs = "style=color:inherit href=https://www.w3.org/TR/prov-o/#wasDerivedFrom"
+                for item in entity._was_derived_from_entities:                    
+                    if not options["invert-relations"]:
                         lines.append(
-                            f"{entity.node_id}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasDerivedFrom>was derived from</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{item.node_id}"
+                            f"{entity.node_id}-{entity_stroke_style} <a {attrs}>was derived from</a> {entity_stroke_style}->{item.node_id}"
                         )
                     else:
                         lines.append(
-                            f"{item.node_id}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasDerivedFrom>originated from</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{entity.node_id}"
+                            f"{item.node_id}-{entity_stroke_style} <a {attrs}>originated from</a> {entity_stroke_style}->{entity.node_id}"
                         )
             if "was_generated_by" in options["included-relations"]:
+                attrs ="style=color:inherit href=https://www.w3.org/TR/prov-o/#wasGeneratedBy"
                 for item in entity._was_generated_by_activities:
-                    if not options["revert-relations"]:
+                    
+                    if not options["invert-relations"]:
                         lines.append(
-                            f"{entity.node_id}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasGeneratedBy>was generated by</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{item.node_id}"
+                            f"{entity.node_id}-{activity_stroke_style} <a {attrs}>was generated by</a> {activity_stroke_style}->{item.node_id}"
                         )
                     else:
                         lines.append(
-                            f"{item.node_id}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasGeneratedBy>generated</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{entity.node_id}"
+                            f"{item.node_id}-{activity_stroke_style} <a {attrs}>generated</a> {activity_stroke_style}->{entity.node_id}"
                         )
             if "was_attributed_to" in options["included-relations"]:
+                attrs = "style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAttributedTo"
                 for item in entity._was_attributed_to_agents:
-                    if not options["revert-relations"]:
+                    
+                    if not options["invert-relations"]:
                         lines.append(
-                            f"{entity.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAttributedTo>was attributed to</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{item.node_id}"
+                            f"{entity.node_id}-{agent_stroke_style} <a {attrs}>was attributed to</a> {agent_stroke_style}->{item.node_id}"
                         )
                     else:
                         lines.append(
-                            f"{item.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAttributedTo>produced</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{entity.node_id}"
+                            f"{item.node_id}-{agent_stroke_style} <a {attrs}>produced</a> {agent_stroke_style}->{entity.node_id}"
                         )
 
         for activity in self._activities:
             lines.append(
-                f"{activity.node_id}{options['activity']['shape'].split(':')[0]}<a style=color:inherit href={activity.node_id}>{activity.label if activity.label else activity.node_id}</a>{options['activity']['shape'].split(':')[1]}:::activity"
+                f"{activity.node_id}{options['activity']['shape'].split(':')[0]}<a style=color:inherit href={activity.node_id}>{activity.label or activity.node_id}</a>{options['activity']['shape'].split(':')[1]}:::activity"
             )
             if "was_informed_by" in options["included-relations"]:
+                attrs = "style=color:inherit href=https://www.w3.org/TR/prov-o/#wasInformedBy"
                 for item in activity._was_informed_by_activities:
-                    if not options["revert-relations"]:
+                    
+                    if not options["invert-relations"]:
                         lines.append(
-                            f"{activity.node_id}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasInformedBy>was informed by</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{item.node_id}"
+                            f"{activity.node_id}-{entity_stroke_style} <a {attrs}>was informed by</a> {entity_stroke_style}->{item.node_id}"
                         )
                     else:
                         lines.append(
-                            f"{item.node_id}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasInformedBy>informed</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{activity.node_id}"
+                            f"{item.node_id}-{entity_stroke_style} <a {attrs}>informed</a> {entity_stroke_style}->{activity.node_id}"
                         )
             if "used" in options["included-relations"]:
-                for item in activity._used_entities:
-                    if not options["revert-relations"]:
+                attrs="style=color:inherit href=https://www.w3.org/TR/prov-o/#used"
+                for item in activity._used_entities:                    
+                    if not options["invert-relations"]:
                         lines.append(
-                            f"{activity.node_id}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#used>used</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{item.node_id}"
+                            f"{activity.node_id}-{activity_stroke_style} <a {attrs}>used</a> {activity_stroke_style}->{item.node_id}"
                         )
                     else:
                         lines.append(
-                            f"{item.node_id}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#used>was used by</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{activity.node_id}"
+                            f"{item.node_id}-{activity_stroke_style} <a {attrs}>was used by</a> {activity_stroke_style}->{activity.node_id}"
                         )
             if "was_associated_with" in options["included-relations"]:
+                attrs = "style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAssociatedWith"
                 for item in activity._was_associated_with_agents:
-                    if not options["revert-relations"]:
+                    if not options["invert-relations"]:
                         lines.append(
-                            f"{activity.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAssociatedWith>was associated with</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{item.node_id}"
+                            f"{activity.node_id}-{agent_stroke_style} <a {attrs}>was associated with</a> {agent_stroke_style}->{item.node_id}"
                         )
                     else:
                         lines.append(
-                            f"{item.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAssociatedWith>initiated</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{activity.node_id}"
+                            f"{item.node_id}-{agent_stroke_style} <a {attrs}>initiated</a> {agent_stroke_style}->{activity.node_id}"
                         )
 
         for agent in self._agents:
             lines.append(
-                f"{agent.node_id}{options['agent']['shape'].split(':')[0]}<a style=color:inherit href={agent.node_id}>{agent.label if agent.label else agent.node_id}</a>{options['agent']['shape'].split(':')[1]}:::agent"
+                f"{agent.node_id}{options['agent']['shape'].split(':')[0]}<a style=color:inherit href={agent.node_id}>{agent.label or agent.node_id}</a>{options['agent']['shape'].split(':')[1]}:::agent"
             )
             if "acted_on_behalf_of" in options["included-relations"]:
+                attrs = "style=color:inherit href=https://www.w3.org/TR/prov-o/#actedOnBehalfOf"
                 for item in agent._acted_on_behalf_of_agents:
-                    if not options["revert-relations"]:
+                    if not options["invert-relations"]:
                         lines.append(
-                            f"{agent.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#actedOnBehalfOf>acted on behalf of</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{item.node_id}"
+                            f"{agent.node_id}-{agent_stroke_style} <a {attrs}>acted on behalf of</a> {agent_stroke_style}->{item.node_id}"
                         )
                     else:
                         lines.append(
-                            f"{item.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#actedOnBehalfOf>instructed</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{agent.node_id}"
+                            f"{item.node_id}-{agent_stroke_style} <a {attrs}>instructed</a> {agent_stroke_style}->{agent.node_id}"
                         )
 
         lines.append("```")
         lines = "\n".join(lines)
 
         with open(file_name, "w") as f:
             f.write(lines)
```

### Comparing `provo-1.1.0/provo/startingpointclasses.py` & `provo-1.1.1/provo/startingpointclasses.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.0/provo/tests/test_provenance_graph.py` & `provo-1.1.1/provo/tests/test_provenance_graph.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.0/provo/tests/test_rdf_output.py` & `provo-1.1.1/provo/tests/test_rdf_output.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.0/provo/tests/test_starting_point_classes.py` & `provo-1.1.1/provo/tests/test_starting_point_classes.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.0/provo/tests/test_vault.py` & `provo-1.1.1/provo/tests/test_vault.py`

 * *Files identical despite different names*

### Comparing `provo-1.1.0/provo.egg-info/PKG-INFO` & `provo-1.1.1/provo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: provo
-Version: 1.1.0
+Version: 1.1.1
 Summary: Construct  PROV-O compliant provenance graphs.
 Home-page: https://github.com/rue-a/provo
 Author: Arne Rümmler
 Author-email: arne.ruemmler@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `provo-1.1.0/setup.py` & `provo-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 this_directory = Path(__file__).parent
 
 setup(
     name="provo",
     author="Arne Rümmler",
     author_email="arne.ruemmler@gmail.com",
-    version="1.1.0",
+    version="1.1.1",
     description="Construct  PROV-O compliant provenance graphs.",
     url="https://github.com/rue-a/provo",
     packages=find_packages(".", exclude=["tests", "tests.*"]),
     install_requires=["rdflib", "validators", "uuid"],
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

