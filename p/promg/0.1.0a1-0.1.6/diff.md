# Comparing `tmp/promg-0.1.0a1.tar.gz` & `tmp/promg-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promg-0.1.0a1.tar", last modified: Tue Jul 25 10:00:35 2023, max compression
+gzip compressed data, was "promg-0.1.6.tar", last modified: Thu Jul 27 11:39:08 2023, max compression
```

## Comparing `promg-0.1.0a1.tar` & `promg-0.1.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 10:00:35.592193 promg-0.1.0a1/
--rw-rw-rw-   0        0        0     7817 2023-04-24 11:35:40.000000 promg-0.1.0a1/LICENSE
--rw-rw-rw-   0        0        0     5808 2023-07-25 10:00:35.592193 promg-0.1.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     5558 2023-07-24 14:46:25.000000 promg-0.1.0a1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 10:00:35.592193 promg-0.1.0a1/setup.cfg
--rw-rw-rw-   0        0        0      706 2023-07-25 09:48:06.000000 promg-0.1.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:00:35.380858 promg-0.1.0a1/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 10:00:35.390865 promg-0.1.0a1/src/promg/
--rw-rw-rw-   0        0        0      516 2023-07-25 09:31:05.000000 promg-0.1.0a1/src/promg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:00:35.462155 promg-0.1.0a1/src/promg/cypher_queries/
--rw-rw-rw-   0        0        0        0 2023-07-25 08:31:19.000000 promg-0.1.0a1/src/promg/cypher_queries/__init__.py
--rw-rw-rw-   0        0        0     4739 2023-07-25 09:38:34.000000 promg-0.1.0a1/src/promg/cypher_queries/analysis_ql.py
--rw-rw-rw-   0        0        0     6392 2023-07-25 09:38:34.000000 promg-0.1.0a1/src/promg/cypher_queries/data_importer_ql.py
--rw-rw-rw-   0        0        0     5152 2023-07-25 09:38:34.000000 promg-0.1.0a1/src/promg/cypher_queries/db_managment_ql.py
--rw-rw-rw-   0        0        0     5867 2023-07-25 09:38:34.000000 promg-0.1.0a1/src/promg/cypher_queries/inference_engine_ql.py
--rw-rw-rw-   0        0        0    17793 2023-07-25 09:38:34.000000 promg-0.1.0a1/src/promg/cypher_queries/semantic_header_ql.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:00:35.483719 promg-0.1.0a1/src/promg/data_managers/
--rw-rw-rw-   0        0        0        0 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/data_managers/__init__.py
--rw-rw-rw-   0        0        0    22666 2023-07-25 09:38:34.000000 promg-0.1.0a1/src/promg/data_managers/datastructures.py
--rw-rw-rw-   0        0        0    31897 2023-07-25 09:38:34.000000 promg-0.1.0a1/src/promg/data_managers/semantic_header.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:00:35.518059 promg-0.1.0a1/src/promg/database_managers/
--rw-rw-rw-   0        0        0    15976 2023-07-25 09:38:34.000000 promg-0.1.0a1/src/promg/database_managers/EventKnowledgeGraph.py
--rw-rw-rw-   0        0        0        0 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/database_managers/__init__.py
--rw-rw-rw-   0        0        0      588 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/database_managers/authentication.py
--rw-rw-rw-   0        0        0     3157 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/database_managers/db_connection.py
--rw-rw-rw-   0        0        0      235 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/database_managers/remote_authentication.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:00:35.563058 promg-0.1.0a1/src/promg/ekg_modules/
--rw-rw-rw-   0        0        0        0 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/ekg_modules/__init__.py
--rw-rw-rw-   0        0        0     6236 2023-07-24 15:50:53.000000 promg-0.1.0a1/src/promg/ekg_modules/data_importer.py
--rw-rw-rw-   0        0        0     3867 2023-07-24 15:51:03.000000 promg-0.1.0a1/src/promg/ekg_modules/db_management.py
--rw-rw-rw-   0        0        0      755 2023-07-24 15:51:20.000000 promg-0.1.0a1/src/promg/ekg_modules/ekg_analysis.py
--rw-rw-rw-   0        0        0     7510 2023-07-24 15:51:15.000000 promg-0.1.0a1/src/promg/ekg_modules/ekg_builder_semantic_header.py
--rw-rw-rw-   0        0        0     1644 2023-07-24 15:51:19.000000 promg-0.1.0a1/src/promg/ekg_modules/inference_engine.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:00:35.590193 promg-0.1.0a1/src/promg/utilities/
--rw-rw-rw-   0        0        0        0 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/utilities/__init__.py
--rw-rw-rw-   0        0        0     1048 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/utilities/auxiliary_functions.py
--rw-rw-rw-   0        0        0     1072 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/utilities/context_manager_tqdm.py
--rw-rw-rw-   0        0        0     1876 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/utilities/get_db_size.py
--rw-rw-rw-   0        0        0     2134 2023-07-24 15:37:27.000000 promg-0.1.0a1/src/promg/utilities/performance_handling.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:00:35.410432 promg-0.1.0a1/src/promg.egg-info/
--rw-rw-rw-   0        0        0     5808 2023-07-25 10:00:35.000000 promg-0.1.0a1/src/promg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1272 2023-07-25 10:00:35.000000 promg-0.1.0a1/src/promg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 10:00:35.000000 promg-0.1.0a1/src/promg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-25 10:00:35.000000 promg-0.1.0a1/src/promg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-25 10:00:35.000000 promg-0.1.0a1/src/promg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.763670 promg-0.1.6/
+-rw-rw-rw-   0        0        0     7817 2023-04-24 11:35:40.000000 promg-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     5806 2023-07-27 11:39:08.762644 promg-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5558 2023-07-25 13:07:47.000000 promg-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:39:08.763670 promg-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      704 2023-07-27 11:31:54.000000 promg-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.622630 promg-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.636717 promg-0.1.6/src/promg/
+-rw-rw-rw-   0        0        0      516 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.690322 promg-0.1.6/src/promg/cypher_queries/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/cypher_queries/__init__.py
+-rw-rw-rw-   0        0        0     4275 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/cypher_queries/analysis_ql.py
+-rw-rw-rw-   0        0        0     8514 2023-07-26 12:17:37.000000 promg-0.1.6/src/promg/cypher_queries/data_importer_ql.py
+-rw-rw-rw-   0        0        0     5207 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/cypher_queries/db_managment_ql.py
+-rw-rw-rw-   0        0        0     5867 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/cypher_queries/inference_engine_ql.py
+-rw-rw-rw-   0        0        0    21132 2023-07-27 09:29:36.000000 promg-0.1.6/src/promg/cypher_queries/semantic_header_ql.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.707503 promg-0.1.6/src/promg/data_managers/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/data_managers/__init__.py
+-rw-rw-rw-   0        0        0    22701 2023-07-26 12:08:52.000000 promg-0.1.6/src/promg/data_managers/datastructures.py
+-rw-rw-rw-   0        0        0    37835 2023-07-27 09:48:28.000000 promg-0.1.6/src/promg/data_managers/semantic_header.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.722050 promg-0.1.6/src/promg/database_managers/
+-rw-rw-rw-   0        0        0    16050 2023-07-26 12:18:33.000000 promg-0.1.6/src/promg/database_managers/EventKnowledgeGraph.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/database_managers/__init__.py
+-rw-rw-rw-   0        0        0      588 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/database_managers/authentication.py
+-rw-rw-rw-   0        0        0     3157 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/database_managers/db_connection.py
+-rw-rw-rw-   0        0        0      235 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/database_managers/remote_authentication.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.750120 promg-0.1.6/src/promg/ekg_modules/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/ekg_modules/__init__.py
+-rw-rw-rw-   0        0        0     6923 2023-07-26 12:20:16.000000 promg-0.1.6/src/promg/ekg_modules/data_importer.py
+-rw-rw-rw-   0        0        0     3867 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/ekg_modules/db_management.py
+-rw-rw-rw-   0        0        0      755 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/ekg_modules/ekg_analysis.py
+-rw-rw-rw-   0        0        0     8562 2023-07-26 13:30:57.000000 promg-0.1.6/src/promg/ekg_modules/ekg_builder_semantic_header.py
+-rw-rw-rw-   0        0        0     1644 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/ekg_modules/inference_engine.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.760626 promg-0.1.6/src/promg/utilities/
+-rw-rw-rw-   0        0        0        0 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1048 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/utilities/auxiliary_functions.py
+-rw-rw-rw-   0        0        0     1072 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/utilities/context_manager_tqdm.py
+-rw-rw-rw-   0        0        0     1876 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/utilities/get_db_size.py
+-rw-rw-rw-   0        0        0     2134 2023-07-25 13:07:47.000000 promg-0.1.6/src/promg/utilities/performance_handling.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:39:08.650242 promg-0.1.6/src/promg.egg-info/
+-rw-rw-rw-   0        0        0     5806 2023-07-27 11:39:08.000000 promg-0.1.6/src/promg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1272 2023-07-27 11:39:08.000000 promg-0.1.6/src/promg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:39:08.000000 promg-0.1.6/src/promg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-27 11:39:08.000000 promg-0.1.6/src/promg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 11:39:08.000000 promg-0.1.6/src/promg.egg-info/top_level.txt
```

### Comparing `promg-0.1.0a1/LICENSE` & `promg-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/PKG-INFO` & `promg-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promg
-Version: 0.1.0a1
+Version: 0.1.6
 Summary: Pyhton library to build Event Knowledge Graphs
 Author: A. Swevels, D.Fahland
 License: GPL 3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `promg-0.1.0a1/README.md` & `promg-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/setup.py` & `promg-0.1.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='promg',
-    version='0.1.0a1',
+    version='0.1.6',
     description='Pyhton library to build Event Knowledge Graphs',
     author='A. Swevels, D.Fahland',
     python_requires='>=3.7',
     install_requires=['neo4j', 'numpy', 'pandas', 'tabulate', 'tqdm'],
     license='GPL 3.0',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `promg-0.1.0a1/src/promg/__init__.py` & `promg-0.1.6/src/promg/__init__.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg/cypher_queries/analysis_ql.py` & `promg-0.1.6/src/promg/cypher_queries/analysis_ql.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,63 +22,58 @@
         if df_threshold == 0 and relative_df_threshold == 0:
             # corresponds to aggregate_df_relations &  aggregate_df_relations_for_entities in graphdb-event-logs
             # aggregate only for a specific entity type and event classifier
 
             # language=sql
             query_str = '''
                                 MATCH 
-                                (c1:Class) <-[:OBSERVED]-(e1:Event) 
+                                (c1:Activity) -[:OBSERVED]-> (e1:Event) 
                                     -[df:$df_label {entityType: '$entity_type'}]-> 
-                                (e2:Event) -[:OBSERVED]-> (c2:Class)
-                                MATCH (e1) -[:CORR] -> (n) <-[:CORR]- (e2)
-                                WHERE n.entityType = df.entityType AND 
-                                    c1.classType = c2.classType $classifier_condition $classifier_self_loops
-                                WITH n.entityType as EType,c1,count(df) AS df_freq,c2
+                                (e2:Event) <-  [:OBSERVED] - (c2:Activity)
+                                $classifier_self_loops
+                                WITH c1, count(df) AS df_freq,c2
                                 MERGE 
                                 (c1) 
-                                    -[rel2:$dfc_label {entityType: '$entity_type', type:'DF_C', classType: 
-                                    c1.classType}]-> 
+                                    -[rel2:$dfc_label {entityType: '$entity_type', type:'DF_C'}]-> 
                                 (c2) 
                                 ON CREATE SET rel2.count=df_freq'''
         else:
             # aggregate only for a specific entity type and event classifier
             # include only edges with a minimum threshold, drop weak edges (similar to heuristics miner)
 
             # language=sql
             query_str = '''
                                 MATCH 
-                                (c1:Class) 
-                                    <-[:OBSERVED]-
+                                (c1:Activity) 
+                                    -[:OBSERVED]->
                                 (e1:Event) 
                                     -[df:$df_label {entityType: '$entity_type'}]-> 
-                                (e2:Event) -[:OBSERVED]-> (c2:Class)
+                                (e2:Event) <-[:OBSERVED]- (c2:Activity)
                                 MATCH (e1) -[:CORR] -> (n) <-[:CORR]- (e2)
-                                WHERE n.entityType = df.entityType 
-                                    AND c1.classType = c2.classType $classifier_condition $classifier_self_loops
-                                WITH n.entityType as entityType,c1,count(df) AS df_freq,c2
+                                $classifier_self_loops
+                                WITH c1,count(df) AS df_freq,c2
                                 WHERE df_freq > $df_threshold
-                                OPTIONAL MATCH (c2:Class) <-[:OBSERVED]- (e2b:Event) -[df2:DF]-> 
-                                    (e1b:Event) -[:OBSERVED]-> (c1:Class)
-                                WITH entityType as EType,c1,df_freq,count(df2) AS df_freq2,c2
+                                OPTIONAL MATCH (c2:Activity) -[:OBSERVED]-> (e2b:Event) -[df2:$df_label {entityType: '$entity_type'}]-> 
+                                    (e1b:Event) <-[:OBSERVED]- (c2:Activity)
+                                WITH c1,df_freq,count(df2) AS df_freq2,c2
                                 WHERE (df_freq*$relative_df_threshold > df_freq2)
                                 MERGE 
                                 (c1) 
-                                    -[rel2:$dfc_label {entityType: '$entity_type', type:'DF_C', classType: 
-                                    c1.classType}]-> 
+                                    -[rel2:$dfc_label {entityType: '$entity_type', type:'DF_C'}]-> 
                                 (c2) 
                                 ON CREATE SET rel2.count=df_freq'''
 
         classifier_condition = ""
         if classifiers is not None:
             classifier_string = "_".join(classifiers)
             classifier_condition = f"AND c1.classType = '{classifier_string}'"
 
         return Query(query_str=query_str,
                      template_string_parameters={
                          "df_label": entity.get_df_label(),
                          "entity_type": entity.node_type,
                          "classifier_condition": classifier_condition,
-                         "classifier_self_loops": "AND c1 <> c2" if exclude_self_loops else "",
+                         "classifier_self_loops": "WHERE c1 <> c2" if exclude_self_loops else "",
                          "dfc_label": AnalysisQueryLibrary.get_dfc_label(entity.node_type, include_label_in_c_df),
                          "df_threshold": df_threshold,
                          "relative_df_threshold": relative_df_threshold
                      })
```

### Comparing `promg-0.1.0a1/src/promg/cypher_queries/db_managment_ql.py` & `promg-0.1.6/src/promg/cypher_queries/db_managment_ql.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,20 +125,20 @@
                 WITH Type(r) as type, count(r) as numberOfRelations, sortOrder
                 RETURN type, numberOfRelations ORDER BY sortOrder
             '''
 
         return Query(query_str=query_str)
 
     @staticmethod
-    def get_event_log_query(node: ConstructedNodes, additional_event_attributes) -> Query:
+    def get_event_log_query(entity: ConstructedNodes, additional_event_attributes) -> Query:
         query_str = '''
                 MATCH (e:Event) - [:CORR] -> (n:$node_label)
-                RETURN n.ID as caseId, e.activity as activity, e.timestamp as timestamp $extra_attributes
+                RETURN n.sysId as caseId, e.activity as activity, e.timestamp as timestamp $extra_attributes
                 ORDER BY n.ID, e.timestamp
             '''
 
         attributes_query = ",".join(f"e.{attribute} as {attribute}" for attribute in additional_event_attributes)
         return Query(query_str=query_str,
                      template_string_parameters={
-                         "node_label": node.get_label_string(),
-                         "extra_attributes": f", {attributes_query}"
+                         "node_label": entity.get_label_string(),
+                         "extra_attributes": f", {attributes_query}" if len(additional_event_attributes) > 0 else ""
                      })
```

### Comparing `promg-0.1.0a1/src/promg/cypher_queries/inference_engine_ql.py` & `promg-0.1.6/src/promg/cypher_queries/inference_engine_ql.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg/cypher_queries/semantic_header_ql.py` & `promg-0.1.6/src/promg/cypher_queries/semantic_header_ql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from string import Template
 
 from ..data_managers.semantic_header import ConstructedNodes, NodeConstructor, Node, \
-    RelationConstructor
+    RelationConstructor, RecordConstructor
 from ..database_managers.db_connection import Query
 
 
 class SemanticHeaderQueryLibrary:
     @staticmethod
     def get_create_node_by_record_constructor_query(node_constructor: NodeConstructor, batch_size: int = 5000,
                                                     merge=False) -> Query:
@@ -17,54 +17,55 @@
         set_property_str = ""
         infer_corr_str = ""
         infer_observed_str = ""
 
         if node_constructor.set_labels is not None:
             set_label_str = f'SET $set_labels'''
 
-        if node_constructor.set_properties is not None:
+        if len(node_constructor.result.optional_properties) > 0:
             set_property_str = 'SET $set_result_properties'
 
         if node_constructor.infer_corr_from_event_record:
             # language=SQL
             infer_corr_str = '''
             WITH record, $result_node_name
-                                MATCH (event:$event_label) - [:PREVALENCE] -> (record) <- [:PREVALENCE] - ($result_node_name)
+                                MATCH (event:$event_label) - [:PREVALENCE] -> (record) <- [:PREVALENCE] - (
+                                $result_node_name)
                                 MERGE (event) - [:$corr_type] -> ($result_node_name)'''
         elif node_constructor.infer_corr_from_entity_record:  # TODO update such that only correct events are considered
             # language=SQL
             infer_corr_str = '''
                         WITH record, $result_node_name
                                 MATCH (event:$event_label) - [:PREVALENCE] -> (record) <- [:PREVALENCE] - (
                                 $result_node_name)
                                 MERGE (event) - [:$corr_type] -> ($result_node_name)'''
         elif node_constructor.infer_observed:
             # language=SQL
             infer_observed_str = '''
             WITH record, $result_node_name
-                                MATCH (event:$event_label) - [:PREVALENCE] -> (record) <- [:PREVALENCE] - ($result_node_name)
+                                MATCH (event:$event_label) - [:PREVALENCE] -> (record) <- [:PREVALENCE] - (
+                                $result_node_name)
                                 CREATE (event) <- [:OBSERVED] - ($result_node_name)
                                 '''
 
         # language=SQL
         query_str = '''
                     CALL apoc.periodic.commit(
                         'MATCH ($record) 
                             WHERE record.created IS NULL
-                            $conditions 
-                            WITH record limit $limit
+                            WITH $record_name limit $limit
                             $merge_or_create ($result_node)
                             SET record.created = True
                             $set_label_str
                             $set_property_str
                             MERGE (record) <- [:PREVALENCE] - ($result_node_name)
                             $infer_corr_str
                             $infer_observed_str
                             RETURN count(*)',
-                            {limit: $limit})
+                            {limit: $limit*10})
                     '''
 
         query_str = Template(query_str).safe_substitute({
             "set_label_str": set_label_str,
             "set_property_str": set_property_str,
             "infer_corr_str": infer_corr_str,
             "infer_observed_str": infer_observed_str,
@@ -110,15 +111,15 @@
         if use_record:
             query_str = '''MATCH ($record) 
                            RETURN count(DISTINCT record.$attribute) as num_ids'''
 
         return Query(query_str=query_str,
                      template_string_parameters={
                          "labels": node_constructor.get_label_string(),
-                         "attribute": node_constructor.result.properties[0].ref_attribute,
+                         "attribute": node_constructor.result.required_properties[0].ref_attribute,
                          "record": node_constructor.get_prevalent_record_pattern(node_name="record")
                      })
 
     @staticmethod
     def get_merge_nodes_with_same_id_query(node_constructor: NodeConstructor, batch_size: int):
         if "Event" in node_constructor.get_labels():
             return None
@@ -142,48 +143,58 @@
                      template_string_parameters={
                          "labels": node_constructor.get_label_string(),
                          "idt_properties": node_constructor.get_idt_properties_query()
                      },
                      parameters={"limit": batch_size})
 
     @staticmethod
-    def get_create_nodes_by_relations_query(node_constructor: NodeConstructor) -> Query:
+    def get_create_nodes_by_relations_query(node_constructor: NodeConstructor, batch_size: int) -> Query:
         if node_constructor.infer_reified_relation:
             # language=sql
-            query_str = '''
-                                   MATCH ($from_node) - [r:$rel_type] -> ($to_node)
-                                   MERGE ($from_node_name) <- [:REIFIED] - ($result_node) - [:REIFIED] -> (
-                                   $to_node_name)
-                               '''
+            apoc_str = '''apoc.refactor.extractNode(rel, $result_labels, "TO", "FROM")'''
         else:
             # language=sql
-            query_str = '''
-                                   MATCH ($from_node) - [r:$rel_type] -> ($to_node)
-                                   MERGE ($result_node)
-                               '''
+            apoc_str = '''apoc.refactor.extractNode(rel, $result_labels)'''
         if node_constructor.infer_corr_from_reified_parents:
             # language=sql
-            query_str += '''WITH $from_node_name, $to_node_name, $result_node_name
-                                   MATCH ($from_node_name) <- [:CORR] - (e:Event)
-                                   MATCH ($to_node_name) <- [:CORR] - (f:Event)
-                                   MERGE ($result_node_name) <- [:CORR] - (e)
-                                   MERGE ($result_node_name) <- [:CORR] - (f)
+            add_str = '''WITH $from_node_name, $to_node_name, output
+                                MATCH ($from_node_name) <- [:CORR] - (e:Event)
+                                MATCH ($to_node_name) <- [:CORR] - (f:Event)
+                                MERGE (output) <- [:CORR] - (e)
+                                MERGE (output) <- [:CORR] - (f)
                    '''
 
+        query_str = '''
+            CALL apoc.periodic.commit(
+                'MATCH ($from_node) - [rel:$rel_type] -> ($to_node)
+                WITH $from_node_name, $to_node_name, rel limit $limit
+                CALL $apoc_str
+                YIELD input, output
+                $add_str
+                RETURN count(*)',
+                {limit: $limit}
+            )
+        '''
+
+        query_str = Template(query_str).safe_substitute({
+            "apoc_str": apoc_str,
+            "add_str": add_str
+        })
+
         # TODO from node
         return Query(query_str=query_str,
                      template_string_parameters={
                          "from_node": node_constructor.relation.from_node.get_pattern(),
                          "to_node": node_constructor.relation.to_node.get_pattern(),
                          "from_node_name": node_constructor.relation.from_node.get_name(),
                          "to_node_name": node_constructor.relation.to_node.get_name(),
-                         "rel_type": node_constructor.relation.relation_type,
-                         "result_node": node_constructor.result.get_pattern(),
-                         "result_node_name": node_constructor.result.get_name()
-                     })
+                         "rel_type": node_constructor.relation.get_relation_type(),
+                         "result_labels": node_constructor.result.get_label_str(as_list=True)
+                     },
+                     parameters={"limit": batch_size})
 
     @staticmethod
     def get_create_relation_by_relations_query(relation_constructor: RelationConstructor, batch_size: int) -> Query:
         # language=SQL
         query_str = '''
                 CALL apoc.periodic.iterate(
                 '$relation_queries                        
@@ -198,33 +209,94 @@
                          "from_node_name": relation_constructor.from_node.get_name(),
                          "to_node_name": relation_constructor.to_node.get_name(),
                          "rel_pattern": relation_constructor.result.get_pattern(),
                          "batch_size": batch_size
                      })
 
     @staticmethod
-    def get_create_relation_using_record_query(relation_constructor: RelationConstructor) -> Query:
+    def get_create_relation_using_record_query(relation_constructor: RelationConstructor, batch_size: int) -> Query:
         # find events that are related to different entities of which one event also has a reference to the other entity
         # create a relation between these two entities
+        add_str = ""
+        if relation_constructor.model_as_node:
+            # language=sql
+            merge_str = '''
+                            MERGE ($from_node_name) -[:FROM] -> (relation:$relation_label_str) - [:TO] -> ($to_node_name)
+                            MERGE (relation)  - [:PREVALENCE] -> (record)
+                            '''
+            if relation_constructor.infer_corr_from_reified_parents:
+                # language=sql
+                add_str = '''
+                            WITH $from_node_name, $to_node_name, relation
+                            CALL {WITH $from_node_name, relation
+                                    MATCH ($from_node_name) <- [:CORR] - (e:Event)
+                                    MERGE (relation) <- [:CORR] - (e)}
+                            CALL {WITH $to_node_name, relation
+                                    MATCH ($to_node_name) <- [:CORR] - (f:Event)
+                                    MERGE (relation) <- [:CORR] - (f)
+                             }                                
+                                    
+                       '''
+        else:
+            merge_str = "MERGE ($from_node_name) -[$rel_pattern] -> ($to_node_name)"
 
-        query_str = '''
+
+
+        query_str = '''     CALL apoc.periodic.commit('
+                            MATCH (record:$record_labels)
+                            WHERE record.rel_created IS NULL
+                            WITH  record limit $limit
                             MATCH ($from_node) - [:PREVALENCE] -> (record)
                             MATCH ($to_node) - [:PREVALENCE] -> (record)
-                            MATCH ($record_node)
-                            MERGE ($from_node_name) -[$rel_pattern] -> ($to_node_name)
+                            $merge_str
+                            SET record.rel_created = True
+                            $add_str
+                            RETURN COUNT(*)',
+                            {limit:$limit})
                         '''
 
+        query_str = Template(query_str).safe_substitute({
+            "merge_str": merge_str,
+            "add_str": add_str
+        })
+
         return Query(query_str=query_str,
                      template_string_parameters={
                          "from_node": relation_constructor.from_node.get_pattern(),
                          "from_node_name": relation_constructor.from_node.get_name(),
                          "to_node": relation_constructor.to_node.get_pattern(),
                          "to_node_name": relation_constructor.to_node.get_name(),
-                         "record_node": relation_constructor.prevalent_record.get_pattern(name="record"),
-                         "rel_pattern": relation_constructor.result.get_pattern()
+                         "record_labels": relation_constructor.prevalent_record.get_label_str(
+                             include_first_colon=False),
+                         "rel_pattern": relation_constructor.result.get_pattern("r"),
+                         "relation_labels": relation_constructor.result.get_relation_types_str(as_list=True),
+                         "relation_label_str": relation_constructor.result.get_relation_types_str()
+                     },
+                     parameters={
+                         "limit": batch_size * 10})
+
+    @staticmethod
+    def get_reset_created_relation_query(relation_constructor: RelationConstructor, batch_size: int) -> Query:
+        # find events that are related to different entities of which one event also has a reference to the other entity
+        # create a relation between these two entities
+
+        query_str = '''     CALL apoc.periodic.commit('
+                              MATCH (record:$record_labels)
+                              WHERE record.rel_created = True
+                              WITH record limit $limit
+                              SET record.rel_created = Null
+                              RETURN COUNT(*)',
+                              {limit:$limit})
+                          '''
+
+        return Query(query_str=query_str,
+                     template_string_parameters={
+                         "record_labels": relation_constructor.prevalent_record.get_label_str(
+                             include_first_colon=False),
+                         "limit": batch_size * 10
                      })
 
     @staticmethod
     def get_create_directly_follows_query(entity: ConstructedNodes, batch_size, event_label) -> Query:
         # find the specific entities and events with a certain label correlated to that entity
         # order all events by time, order_nr and id grouped by a node n
         # collect the sorted nodes as a list
```

### Comparing `promg-0.1.0a1/src/promg/data_managers/datastructures.py` & `promg-0.1.6/src/promg/data_managers/datastructures.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import List, Dict, Any, Optional
 from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame
 
+from .semantic_header import Node
 from ..utilities.auxiliary_functions import replace_undefined_value, create_list
 
 
 @dataclass
 class DatetimeObject:
     format: str
     timezone_offset: str
@@ -40,39 +41,39 @@
 
 
 @dataclass
 class Column:
     name: str
     dtype: str
     nan_values: List[str]
-    mandatory: bool
+    optional: bool
     range_start: int
     range_end: int
 
     @staticmethod
     def from_dict(obj: Any) -> Optional['Column']:
         if obj is None:
             return None
         _name = obj.get("name")
         _dtype = obj.get("dtype")
         _nan_values = replace_undefined_value(obj.get("nan_values"), [])
-        _mandatory = replace_undefined_value(obj.get("mandatory"), True)
+        _optional = replace_undefined_value(obj.get("optional"), False)
         _range_start = obj.get("range_start")
         _range_end = obj.get("range_end")
-        return Column(_name, _dtype, _nan_values, _mandatory, _range_start, _range_end)
+        return Column(_name, _dtype, _nan_values, _optional, _range_start, _range_end)
 
 
 @dataclass
 class Attribute:
     name: str
     columns: List[Column]
     separator: str
     is_datetime: bool
     is_compound: bool
-    mandatory: bool
+    optional: bool
     datetime_object: DatetimeObject
     na_rep_value: Any
     na_rep_columns: List[Column]
     filter_exclude_values: List[str]
     filter_include_values: List[str]
     use_filter: bool
     is_primary_key: bool
@@ -81,27 +82,27 @@
     @staticmethod
     def from_dict(obj: Any) -> Optional['Attribute']:
         if obj is None:
             return None
         _name = obj.get("name")
         _columns = create_list(Column, obj.get("columns"))
         _is_compound = len(_columns) > 1
-        _mandatory = bool(obj.get("mandatory"))
+        _optional = bool(obj.get("optional"))
         _datetime_object = DatetimeObject.from_dict(obj.get("datetime_object"))
         _is_datetime = _datetime_object is not None
         _na_rep_value = obj.get("na_rep_value")
         _na_rep_columns = create_list(Column, obj.get("na_rep_columns"))
         _separator = obj.get("separator")
         _filter_exclude_values = obj.get("filter_exclude_values")
         _filter_include_values = obj.get("filter_include_values")
         _use_filter = _filter_include_values is not None or _filter_exclude_values is not None  # default value
         _use_filter = replace_undefined_value(obj.get("use_filter"), _use_filter)
         _is_primary_key = replace_undefined_value(obj.get("is_primary_key"), False)
         _is_foreign_key = replace_undefined_value(obj.get("is_foreign_key"), False)
-        return Attribute(name=_name, mandatory=_mandatory, columns=_columns, separator=_separator,
+        return Attribute(name=_name, optional=_optional, columns=_columns, separator=_separator,
                          is_compound=_is_compound,
                          is_datetime=_is_datetime, datetime_object=_datetime_object,
                          na_rep_value=_na_rep_value, na_rep_columns=_na_rep_columns,
                          filter_exclude_values=_filter_exclude_values, filter_include_values=_filter_include_values,
                          use_filter=_use_filter, is_primary_key=_is_primary_key, is_foreign_key=_is_foreign_key)
 
 
@@ -193,14 +194,15 @@
         else:
             _samples = create_list(Sample, _samples_obj)
 
         _samples = {sample.file_name: sample for sample in _samples}
         _attributes = create_list(Attribute, obj.get("attributes"))
         _attributes = {attribute.name: attribute for attribute in _attributes}
         _split_combined_events = replace_undefined_value(obj.get("split_combined_events"), False)
+
         return DataStructure(_include, _name, _file_directory, _file_names, _encoding, _seperator, _decimal,
                              _labels, _true_values, _false_values, _add_log, _add_index,
                              _samples, _attributes, _split_combined_events)
 
     def get_primary_keys(self):
         return [attribute_name for attribute_name, attribute in self.attributes.items() if attribute.is_primary_key]
 
@@ -282,15 +284,15 @@
         return df_log
 
     @staticmethod
     def replace_nan_values_with_unknown(df_log, attribute):
         column: Column
         for i, column in zip(range(len(attribute.columns)), attribute.columns):
             attribute_name = f"{attribute.name}_{i}"
-            if column.mandatory:
+            if not column.optional:
                 try:
                     df_log[attribute_name].fillna("Unknown", inplace=True)
                 except:
                     df_log[attribute_name].fillna(-1, inplace=True)
         return df_log
 
     @staticmethod
@@ -335,15 +337,15 @@
         for attribute in self.attributes.values():
             df_log = DataStructure.create_attribute_columns(df_log, attribute)
             df_log = DataStructure.replace_with_nan(df_log, attribute)
             if len(attribute.na_rep_columns) > 0:  # impute values in case of missing values
                 df_log = DataStructure.replace_nan_values_based_on_na_rep_columns(df_log, attribute)
             if attribute.na_rep_value is not None:
                 df_log = DataStructure.replace_nan_values_based_on_na_rep_value(df_log, attribute)
-            if attribute.mandatory:
+            if not attribute.optional:
                 df_log = DataStructure.replace_nan_values_with_unknown(df_log, attribute)
 
             df_log = DataStructure.combine_attribute_columns(df_log, attribute)
 
         return df_log
 
     def split_df_log_into_combined_events(self, df_log: DataFrame):
```

### Comparing `promg-0.1.0a1/src/promg/data_managers/semantic_header.py` & `promg-0.1.6/src/promg/data_managers/semantic_header.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,77 +43,97 @@
             components = attribute.split(".")
             node_name = components[0]
             node_attribute = components[1]
 
         return Property(attribute=attribute, value=value, node_name=node_name,
                         node_attribute=node_attribute, ref_node=ref_node, ref_attribute=ref_attribute)
 
-    def get_pattern(self, is_set=False):
+    def get_pattern(self, is_set=False, node_name=None):
         if not is_set:
             return f"{self.attribute}: {self.value}"
         else:
-            return f"{self.attribute} = {self.value}"
+            if node_name is None:
+                return f"{self.attribute} = {self.value}"
+            else:
+                return f"{node_name}.{self.attribute} = {self.value}"
+
+    def __repr__(self):
+        return self.get_pattern()
 
 
 @dataclass()
 class Node:
-    def __init__(self, name: str, labels: List[str], properties: List[Property], where_condition: str):
+    def __init__(self, name: str, labels: List[str], required_properties: List[Property],
+                 optional_properties: List[Property], where_condition: str):
         self.name = name
         self.labels = labels
-        self.properties = properties
+        self.required_properties = required_properties
+        self.optional_properties = optional_properties
         self.where_condition = where_condition
 
     @staticmethod
     def from_string(node_description: str) -> Optional["Node"]:
         if node_description is None:
             return None
         # we expect a node to be described in (node_name:Node_label)
         node_description = re.sub(r"[()]", "", node_description)
         node_components = node_description.split(":", 1)
         name = node_components[0]
         labels = ""
         where_condition = ""
-        properties = []
+        required_properties = []
+        optional_properties = []
         if len(node_components) > 1:
             node_labels_prop_where = node_components[1]
             node_labels_prop_where = node_labels_prop_where.replace("'", "\"")
             if "WHERE" in node_labels_prop_where:
                 labels = node_labels_prop_where.split(" WHERE ")[0]
                 where_condition = node_labels_prop_where.split(" WHERE ")[1]
             elif "{" in node_labels_prop_where:
                 labels = node_labels_prop_where.split(" {")[0]
                 properties = node_labels_prop_where.split(" {")[1]
                 properties = properties.replace("}", "")
                 properties = properties.split(",")
-                properties = [Property.from_string(prop) for prop in properties]
+
+                required_properties = [prop for prop in properties if "OPTIONAL" not in prop]
+                optional_properties = [prop.replace("OPTIONAL", "") for prop in properties if "OPTIONAL" in prop]
+
+                required_properties = [Property.from_string(prop) for prop in required_properties]
+                optional_properties = [Property.from_string(prop) for prop in optional_properties]
             else:
                 labels = node_labels_prop_where
 
         labels = labels.strip()
         labels = labels.split(":")
 
-        return Node(name=name, labels=labels, properties=properties,
+        return Node(name=name, labels=labels, required_properties=required_properties,
+                    optional_properties=optional_properties,
                     where_condition=where_condition)
 
     def get_name(self, with_brackets=False):
         if with_brackets:
             return f"({self.name})"
         else:
             return self.name
 
-    def get_condition_string(self, with_brackets=False, with_where=False):
-        if len(self.properties) > 0:
-            return self._get_property_string(with_brackets)
+    def get_condition_string(self, with_brackets=False, with_where=False, with_optional=False):
+        properties = self.required_properties + self.optional_properties if with_optional else self.required_properties
+        if len(properties) > 0:
+            return self._get_property_string(with_brackets, with_optional)
         elif self.where_condition != "":
             return self._get_where_condition_string(with_where)
         else:
             return ""
 
-    def _get_property_string(self, with_brackets=False):
-        properties = ",".join([prop.get_pattern() for prop in self.properties])
+    def _get_property_string(self, with_brackets=False, with_optional=False):
+        properties = [req_prop.get_pattern() for req_prop in self.required_properties]
+        if with_optional:
+            properties += [f"OPTIONAL {prop.get_pattern()}" for prop in self.optional_properties]
+
+        properties = ", ".join(properties)
         if with_brackets:
             property_string = "{$properties}"
             properties = Template(property_string).substitute(properties=properties)
         return properties
 
     def _get_where_condition_string(self, with_where=False):
         condition = self.where_condition
@@ -141,38 +161,53 @@
                                                                      with_brackets=True, with_where=True))
         if with_brackets:
             node_pattern_str = "($node_pattern)"
             node_pattern = Template(node_pattern_str).substitute(node_pattern=node_pattern)
 
         return node_pattern
 
-    def get_label_str(self, include_first_colon=False):
+    def get_label_str(self, include_first_colon=False, as_list=False):
+        if as_list:
+            str = ",".join([f'"{label}"' for label in self.labels])
+            return f'[{str}]'
+
         if len(self.labels) > 0:
             return ":" * include_first_colon + ":".join(self.labels)
         return ""
 
     def __repr__(self):
         return self.get_pattern(with_brackets=True)
 
     @staticmethod
     def from_dict(obj: Any) -> Optional["Node"]:
         return Node.from_string(obj)
 
 
 class Relationship:
-    def __init__(self, relation_name: str, relation_type: str, from_node: Node, to_node: Node,
+    def __init__(self, relation_name: str, relation_types: List[str], from_node: Node, to_node: Node,
                  properties: List[Property], where_condition: str, has_direction: bool):
         self.relation_name = relation_name
-        self.relation_type = relation_type
+        self.relation_types = relation_types
         self.from_node = from_node
         self.to_node = to_node
         self.properties = properties
         self.where_condition = where_condition
         self.has_direction = has_direction
 
+    def get_relation_type(self):
+        return self.relation_types[0]
+
+    def get_relation_types_str(self, include_first_colon = False, as_list=False):
+        if as_list:
+            str = ",".join([f'"{label}"' for label in self.relation_types])
+            return f'[{str}]'
+        if len(self.relation_types) > 0:
+            return ":" * include_first_colon + ":".join(self.relation_types)
+        return ""
+
     @staticmethod
     def from_string(relation_description: str) -> Optional["Relationship"]:
         if relation_description is None:
             return None
 
         # we expect a node to be described in (node_name:Node_label)
         relation_directions = {
@@ -180,47 +215,48 @@
             "right-to-left": {"has_direction": True, "from_node": 1, "to_node": 0},
             "undefined": {"has_direction": False, "from_node": 0, "to_node": 1}
         }
 
         nodes = re.findall(r'\([^<>]*\)', relation_description)
         _relation_string = re.findall(r'\[[^<>]*]', relation_description)[0]
         _relation_string = re.sub(r"[\[\]]", "", _relation_string)
-        _relation_components = _relation_string.split(":")
+        _relation_components = _relation_string.split(":", maxsplit=1)
         _relation_name = _relation_components[0]
-        _relation_type = _relation_components[1]
+        _relation_types = _relation_components[1]
+        _relation_types = _relation_types.split(":")
 
         if ">" in relation_description:
             direction = "left-to-right"
         elif "<" in relation_description:
             direction = "right-to-left"
         else:
             direction = "undefined"
 
         # TODO, implement properties and where condition
 
         _has_direction = relation_directions[direction]["has_direction"]
         _from_node = Node.from_string(nodes[relation_directions[direction]["from_node"]])
         _to_node = Node.from_string(nodes[relation_directions[direction]["to_node"]])
 
-        return Relationship(relation_name=_relation_name, relation_type=_relation_type,
+        return Relationship(relation_name=_relation_name, relation_types=_relation_types,
                             from_node=_from_node, to_node=_to_node, properties=[], where_condition="",
                             has_direction=_has_direction)
 
     @staticmethod
     def from_dict(obj: Any) -> Optional["Relationship"]:
         return Relationship.from_string(obj)
 
     def get_pattern(self, name: Optional[str] = None, exclude_nodes=True, with_brackets=False):
         rel_pattern_str = "$rel_name"
-        if self.relation_type != "":
+        if self.get_relation_type() != "":
             rel_pattern_str = "$rel_name:$rel_type"
 
         name = name if name is not None else self.relation_name
         rel_pattern = Template(rel_pattern_str).substitute(rel_name=name,
-                                                           rel_type=self.relation_type)
+                                                           rel_type=self.get_relation_type())
 
         if len(self.properties) > 0:
             properties_string = ",".join([prop.get_pattern() for prop in self.properties])
             rel_pattern_str = "$rel_pattern {$properties}"
             rel_pattern = Template(rel_pattern_str).substitute(rel_pattern=rel_pattern,
                                                                properties=properties_string)
         elif self.where_condition != "":
@@ -355,28 +391,26 @@
 
 
 class NodeConstructor:
     def __init__(self, prevalent_record: Optional[Union["Relationship", "Node"]],
                  node: Optional["Node"],
                  relation: Optional["Relationship"],
                  result: "Node",
-                 set_properties: List[Property],
                  set_labels: str,
                  infer_observed: bool = False,
                  infer_corr_from_event_record: bool = False,
                  infer_corr_from_entity_record: bool = False,
                  infer_corr_from_reified_parents: bool = False,
                  event_label: str = "Event",
                  corr_type: str = "CORR",
                  infer_reified_relation: bool = False):
         self.prevalent_record = prevalent_record
         self.relation = relation
         self.node = node
         self.result = result
-        self.set_properties = set_properties
         self.set_labels = set_labels
         self.infer_prevalence_record = prevalent_record is not None
         self.infer_observed = infer_observed
         self.infer_corr_from_event_record = infer_corr_from_event_record
         self.infer_corr_from_entity_record = infer_corr_from_entity_record
         self.infer_corr_from_reified_parents = infer_corr_from_reified_parents
         self.event_label = event_label
@@ -385,18 +419,14 @@
 
     @staticmethod
     def from_dict(obj: Any) -> "NodeConstructor":
         _prevalent_record = RelationshipOrNode.from_string(obj.get("prevalent_record"))
         _node = Relationship.from_string(obj.get("node"))
         _relation = Relationship.from_string(obj.get("relation"))
         _result = Node.from_string(obj.get("result"))
-        _set_properties = obj.get("set_properties")
-        if _set_properties is not None:
-            _set_properties = _set_properties.split(",")
-            _set_properties = [Property.from_string(prop) for prop in _set_properties]
         _set_labels = obj.get("set_labels")
         _infer_observed = replace_undefined_value(obj.get("infer_observed"), False)
         _infer_corr_from_event_record = replace_undefined_value(obj.get("infer_corr_from_event_record"), False)
         _infer_corr_from_entity_record = replace_undefined_value(obj.get("infer_corr_from_entity_record"), False)
         _infer_corr_from_reified_parents = replace_undefined_value(obj.get("infer_corr_from_reified_parents"), False)
         _corr_type = replace_undefined_value(obj.get("corr_type"), "CORR")
         _event_label = replace_undefined_value(obj.get("event_label"), "Event")
@@ -409,15 +439,14 @@
                                infer_observed=_infer_observed,
                                infer_corr_from_event_record=_infer_corr_from_event_record,
                                infer_corr_from_entity_record=_infer_corr_from_entity_record,
                                infer_corr_from_reified_parents=_infer_corr_from_reified_parents,
                                corr_type=_corr_type,
                                event_label=_event_label,
                                infer_reified_relation=_infer_reified_relation,
-                               set_properties=_set_properties,
                                set_labels=_set_labels)
 
     def __name__(self):
         if self.prevalent_record is not None:
             return "constructed_by_record"
         elif self.node is not None:
             return "constructed_by_node"
@@ -433,15 +462,15 @@
         return self.result.labels
 
     def get_prevalent_record_pattern(self, node_name: str = "record"):
         return self.prevalent_record.get_pattern(node_name)
 
     def get_keys(self):
         keys = []
-        for prop in self.result.properties:
+        for prop in self.result.required_properties:
             # only check whether the ref attribute exists, if it should exist in the ref node
             if prop.ref_node is not None:
                 key = prop.ref_attribute
                 keys.append(key)
         return keys
 
     def get_where_condition(self, node_name: str = "record", include_start_and: bool = False):
@@ -467,22 +496,24 @@
     def constructed_by_node(self):
         return self.node is not None
 
     def constructed_by_relation(self):
         return self.relation is not None
 
     def get_set_result_properties_query(self):
-        if self.set_properties is None:
+        if len(self.result.optional_properties) == 0:
             return None
-        return ",".join([prop.get_pattern(is_set=True) for prop in self.set_properties])
+        return ",".join(
+            [prop.get_pattern(is_set=True, node_name=self.result.name) for prop in self.result.optional_properties])
 
     def get_idt_properties_query(self, node_name="n"):
-        if self.result.properties is None:
+        if self.result.required_properties is None:
             return None
-        return ",".join([f"{node_name}.{prop.attribute} as {prop.attribute}" for prop in self.result.properties])
+        return ",".join(
+            [f"{node_name}.{prop.attribute} as {prop.attribute}" for prop in self.result.required_properties])
 
     def get_set_result_labels_query(self):
         if self.set_labels is None:
             return None
         return f"{self.result.get_name()}:{self.set_labels}"
 
 
@@ -526,17 +557,21 @@
                                             merge_duplicate_df=_merge_duplicate_df,
                                             delete_parallel_df=_delete_parallel_df)
 
         # TODO check whether names match
         return constructed_node
 
     def get_label_string(self):
+        if len(self.node_constructors) == 0:
+            return self.node_type
         return self.node_constructors[0].get_label_string()
 
     def get_labels(self):
+        if len(self.node_constructors) == 0:
+            return self.node_type
         return self.node_constructors[0].get_labels()
 
     def get_corr_type_strings(self):
         corr_types = list(set([node_constructor.corr_type for node_constructor in self.node_constructors]))
         return "|".join(corr_types)
 
     def get_df_label(self):
@@ -549,54 +584,63 @@
 class RelationConstructor:
     def __init__(self, prevalent_record: Optional[Union["Relationship", "Node"]],
                  nodes: List["Node"],
                  relations: List["Relationship"],
                  from_node: "Node",
                  to_node: "Node",
                  result: "Relationship",
-                 set_properties: List[Property]):
+                 optional_properties: List[Property],
+                 model_as_node: bool,
+                 infer_corr_from_reified_parents: bool):
         self.prevalent_record = prevalent_record
         self.from_node = from_node
         self.to_node = to_node
         self.relations = relations
         self.nodes = nodes
         self.result = result
-        self.set_properties = set_properties
+        self.optional_properties = optional_properties
+        self.model_as_node = model_as_node
+        self.infer_corr_from_reified_parents = infer_corr_from_reified_parents
 
     @staticmethod
     def from_dict(obj: Any) -> "RelationConstructor":
         _prevalent_record = RelationshipOrNode.from_string(obj.get("prevalent_record"))
         _nodes = create_list(Node, obj.get("nodes"))
         _relations = create_list(Relationship, obj.get("relations"))
         _from_node = Node.from_string(obj.get("from_node"))
         _to_node = Node.from_string(obj.get("to_node"))
         _result = Relationship.from_string(obj.get("result"))
-        _set_properties = obj.get("set_properties")
-        if _set_properties is not None:
-            _set_properties = _set_properties.split(",")
-            _set_properties = [Property.from_string(prop) for prop in _set_properties]
+        _optional_properties = obj.get("set_optional_properties")
+        if _optional_properties is not None:
+            _optional_properties = _optional_properties.split(",")
+            _optional_properties = [Property.from_string(prop) for prop in _optional_properties]
+
+        _model_as_node = replace_undefined_value(obj.get("model_as_node"), False)
+        _infer_corr_from_reified_parents = replace_undefined_value(obj.get("infer_corr_from_reified_parents"), False)
 
         return RelationConstructor(prevalent_record=_prevalent_record,
                                    relations=_relations,
                                    nodes=_nodes,
                                    from_node=_from_node,
                                    to_node=_to_node,
                                    result=_result,
-                                   set_properties=_set_properties, )
+                                   optional_properties=_optional_properties,
+                                   model_as_node=_model_as_node,
+                                   infer_corr_from_reified_parents=_infer_corr_from_reified_parents)
 
     def __name__(self):
         if self.prevalent_record is not None:
             return "constructed_by_record"
         elif self.nodes is not None:
             return "constructed_by_nodes"
         elif self.relations is not None:
             return "constructed_by_relations"
 
     def get_type(self):
-        return self.result.relation_type
+        return self.result.get_relation_type()
 
     def get_prevalent_record_pattern(self, node_name: str):
         return self.prevalent_record.get_pattern(node_name)
 
     def get_keys(self):
         keys = []
         for prop in self.result.properties:
@@ -621,17 +665,17 @@
     def constructed_by_nodes(self):
         return len(self.nodes) > 0
 
     def constructed_by_relations(self):
         return len(self.relations) > 0
 
     def get_set_result_properties_query(self):
-        if self.set_properties is None:
+        if self.optional_properties is None:
             return None
-        return ",".join([prop.get_pattern(is_set=True) for prop in self.set_properties])
+        return ",".join([prop.get_pattern(is_set=True) for prop in self.optional_properties])
 
     def get_relations_query(self):
         relation_queries = [f"MATCH {relation.get_pattern(exclude_nodes=False, with_brackets=True)}" for relation in
                             self.relations]
         relation_query = "\n".join(relation_queries)
         return relation_query
 
@@ -654,19 +698,86 @@
         _relation_constructors = create_list(RelationConstructor, obj.get("constructor"))
         return ConstructedRelation(_include, _type, relation_constructors=_relation_constructors)
 
     def __repr__(self):
         return f"[:{self.type}]"
 
 
+class RecordConstructor:
+    def __init__(self, record_labels: List[str],
+                 required_attributes: List[str], optional_attributes: List[str], node_name: str = "record",
+                 prevalent_record: Optional["Node"] = Node.from_string("(record:Record)")):
+        self.node_name = node_name
+        self.prevalent_record = prevalent_record
+        self.record_labels = record_labels
+        self.required_attributes = required_attributes
+        self.optional_attributes = optional_attributes
+
+    @staticmethod
+    def from_dict(obj: Any) -> "RecordConstructor":
+        if isinstance(obj, str):
+            return RecordConstructor.from_str(obj)
+        _prevalent_record = Node.from_string(obj.get("prevalent_record"))
+        _record_labels = obj.get("record_labels").split(":")
+        _required_attributes = obj.get("required_attributes")
+        _optional_attributes = obj.get("optional_attributes")
+
+        return RecordConstructor(prevalent_record=_prevalent_record, record_labels=_record_labels,
+                                 required_attributes=_required_attributes,
+                                 optional_attributes=_optional_attributes)
+
+    @staticmethod
+    def from_str(obj: str) -> "RecordConstructor":
+        obj = re.sub("[\(\)]", "", obj)
+        _node_name = obj.split(":", maxsplit=1)[0].strip()
+        if _node_name == "":
+            _node_name = "record"
+        record_description = obj.split(":", maxsplit=1)[1].strip()
+        if "WHERE" in record_description.upper():
+            labels = record_description.split("WHERE")[0].replace(" ", "")
+            condition_and_properties = record_description.split("WHERE")[1].strip()
+            condition = condition_and_properties.split("{")[0].strip()
+            properties = condition_and_properties.split("{")[1].replace("}", "").strip()
+        else:
+            labels = record_description.split("{")[0].replace(" ", "")
+            condition = None
+            properties = record_description.split("{")[1].replace("}", "").strip()
+
+        _record_labels = labels.split(":")
+        prevalent_record_str = f"({_node_name}:Record)"
+        if condition is not None:
+            prevalent_record_str = f"({_node_name}:Record WHERE {condition})"
+        _prevalent_record = Node.from_string(prevalent_record_str)
+        properties = properties.split(",")
+        _required_attributes = [prop.strip() for prop in properties if "OPTIONAL" not in prop.upper()]
+        _optional_attributes = [prop.replace("OPTIONAL", "").strip() for prop in properties if
+                                "OPTIONAL" in prop.upper()]
+
+        return RecordConstructor(node_name=_node_name, record_labels=_record_labels, prevalent_record=_prevalent_record,
+                                 required_attributes=_required_attributes, optional_attributes=_optional_attributes)
+
+    def get_prevalent_record_pattern(self, record_name: str = "record"):
+        return self.prevalent_record.get_pattern(record_name)
+
+    def get_required_attributes_is_not_null_pattern(self, record_name: str = "record"):
+        return " AND ".join(
+            [f'''{record_name}.{attribute} IS NOT NULL''' for attribute in self.required_attributes])
+
+    def get_record_labels_pattern(self):
+        return ":".join(self.record_labels)
+
+
 class SemanticHeader:
     def __init__(self, name: str, version: str,
-                 nodes: List[ConstructedNodes], relations: List[ConstructedRelation]):
+                 records: List["RecordConstructor"],
+                 nodes: List[ConstructedNodes],
+                 relations: List[ConstructedRelation]):
         self.name = name
         self.version = version
+        self.records = records
         self.nodes = nodes
         self.relations = relations
 
     def get_entity(self, entity_type) -> Optional[ConstructedNodes]:
         for entity in self.nodes:
             if entity_type == entity.node_type:
                 return entity
@@ -676,15 +787,16 @@
     def from_dict(obj: Any) -> Optional["SemanticHeader"]:
         if obj is None:
             return None
         _name = obj.get("name")
         _version = obj.get("version")
         _nodes = create_list(ConstructedNodes, obj.get("nodes"))
         _relations = create_list(ConstructedRelation, obj.get("relations"))
-        return SemanticHeader(_name, _version, _nodes, _relations)
+        _records = create_list(RecordConstructor, obj.get("records"))
+        return SemanticHeader(name=_name, version=_version, records=_records, nodes=_nodes, relations=_relations)
 
     @staticmethod
     def create_semantic_header(path: Path):
         with open(path) as f:
             json_semantic_header = json.load(f)
 
         semantic_header = SemanticHeader.from_dict(json_semantic_header)
```

### Comparing `promg-0.1.0a1/src/promg/database_managers/EventKnowledgeGraph.py` & `promg-0.1.6/src/promg/database_managers/EventKnowledgeGraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                  specification_of_data_structures: ImportedDataStructures,
                  batch_size: int = 5000, use_sample: bool = False, use_preprocessed_files: bool = False,
                  semantic_header: SemanticHeader = None,
                  perf: Performance = None, custom_module_name=None):
         # classes responsible for executing queries
         self.ekg_management = DBManagement(db_connection=db_connection, db_name=db_name, perf=perf)
         self.data_importer = Importer(db_connection, data_structures=specification_of_data_structures,
+                                      records=semantic_header.records,
                                       batch_size=batch_size,
                                       use_sample=use_sample, use_preprocessed_files=use_preprocessed_files, perf=perf)
         self.ekg_builder = EKGUsingSemanticHeaderBuilder(db_connection=db_connection, semantic_header=semantic_header,
                                                          batch_size=batch_size, perf=perf)
         self.inference_engine = InferenceEngine(db_connection=db_connection, perf=perf)
         self.ekg_analysis = EKGAnalysis(db_connection=db_connection, perf=perf)
 
@@ -167,28 +168,27 @@
 
         """
         self.data_importer.import_data()
 
     # endregion
 
     # region EKG builder using semantic header
-
-    def create_nodes_by_records(self, node_type: Optional[List[str]] = None) -> None:
+    def create_nodes_by_records(self, node_types: Optional[List[str]] = None) -> None:
         """
         Pass on method to ekg_builder to create relations between entities based on nodes as specified in the
         semantic header
 
-        :param node_type: list of entity types that should be created based on nodes. In case of None,
+        :param node_types: list of entity types that should be created based on nodes. In case of None,
         all entities based on nodes are created as specified in the semantic header
-        :type node_type: List[str], optional
+        :type node_types: List[str], optional
         :return: None
 
         """
 
-        self.ekg_builder.create_nodes_by_records(node_type)
+        self.ekg_builder.create_nodes_by_records(node_types)
 
     def create_relations_using_record(self, relation_types: Optional[List[str]] = None) -> None:
         """
         Pass on method to ekg_builder to create relations between entities based on nodes as specified in the
         semantic header
 
         :param relation_types: list of relation types for which the relations should be created. In case of None,
```

### Comparing `promg-0.1.0a1/src/promg/database_managers/authentication.py` & `promg-0.1.6/src/promg/database_managers/authentication.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg/database_managers/db_connection.py` & `promg-0.1.6/src/promg/database_managers/db_connection.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg/ekg_modules/data_importer.py` & `promg-0.1.6/src/promg/ekg_modules/data_importer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import math
+from typing import List
 
 import numpy as np
 from tqdm import tqdm
 
+from ..data_managers.semantic_header import RecordConstructor
 from ..database_managers.db_connection import DatabaseConnection
 from ..data_managers.datastructures import ImportedDataStructures
 from ..utilities.performance_handling import Performance
 from ..cypher_queries.data_importer_ql import DataImporterQueryLibrary as di_ql
 import pandas as pd
 
 
 class Importer:
-    def __init__(self, db_connection: DatabaseConnection, data_structures: ImportedDataStructures, batch_size: int,
+    def __init__(self, db_connection: DatabaseConnection, data_structures: ImportedDataStructures,
+                 records: List["RecordConstructor"], batch_size: int,
                  use_sample: bool = False, use_preprocessed_files: bool = False,
                  perf: Performance = None):
         self.connection = db_connection
         self.structures = data_structures.structures
+        self.records = records
 
         self.batch_size = batch_size
         self.use_sample = use_sample
         self.use_preprocessed_files = use_preprocessed_files
         self.perf = perf
 
     def _write_message_to_performance(self, message: str):
@@ -33,26 +37,22 @@
             # read in all file names that match this structure
             for file_name in structure.file_names:
                 # read and import the nodes
                 df_log = structure.read_data_set(file_directory, file_name, use_sample=self.use_sample,
                                                  use_preprocessed_file=self.use_preprocessed_files)
                 df_log["justImported"] = True
                 self._import_nodes_from_data(labels, df_log, file_name)
+
                 self._write_message_to_performance(f"Imported data from table {structure.name}: {file_name}")
 
             if structure.has_datetime_attribute():
                 # once all events are imported, we convert the string timestamp to the timestamp as used in Cypher
                 self._reformat_timestamps(structure)
                 self._write_message_to_performance(
                     f"Reformatted timestamps from events from event table {structure.name}: {file_name}")
-            else:
-                # non event nodes may need to get merged depending on their primary key
-                self._merge_nodes(structure)
-                self._write_message_to_performance(
-                    f"Similar nodes from table {structure.name}: {file_name} are merged")
 
             self._filter_nodes(structure=structure)  # filter nodes according to the structure
             self._write_message_to_performance(
                 f"Filtered the nodes from table {structure.name}: {file_name}")
 
             self._finalize_import(labels=labels)  # removes temporary properties
 
@@ -74,18 +74,14 @@
             self.connection.exec_query(di_ql.get_make_timestamp_date_query,
                                        **{
                                            "label": structure.get_label_string(),
                                            "attribute": attribute, "datetime_object": datetime_format,
                                            "batch_size": self.batch_size
                                        })
 
-    def _merge_nodes(self, structure):
-        self.connection.exec_query(di_ql.get_merge_same_nodes_query,
-                                   **{"data_structure": structure})
-
     def _filter_nodes(self, structure):
         for boolean in (True, False):
             attribute_values_pairs_filtered = structure.get_attribute_value_pairs_filtered(exclude=boolean)
             for name, values in attribute_values_pairs_filtered.items():
                 self.connection.exec_query(di_ql.get_filter_events_by_property_query,
                                            **{"prop": name, "values": values, "exclude": boolean})
 
@@ -109,11 +105,29 @@
             batch_without_nans = [{k: int(v) if isinstance(v, np.integer) else v for k, v in m.items()
                                    if (isinstance(v, list) and len(v) > 0) or (not pd.isna(v) and v is not None)}
                                   for m in
                                   df_log[batch * self.batch_size:(batch + 1) * self.batch_size].to_dict(
                                       orient='records')]
             self.connection.exec_query(di_ql.get_create_nodes_by_importing_batch_query,
                                        **{"batch": batch_without_nans, "labels": labels})
+            self._create_records()
 
             pbar.update(1)
             batch += 1
         pbar.close()
+
+    def _create_records(self) -> None:
+        for record_constructor in self.records:
+            self.connection.exec_query(di_ql.get_create_record_query,
+                                       **{
+                                           "record_constructor": record_constructor,
+                                           "batch_size": self.batch_size
+                                       })
+            self.connection.exec_query(di_ql.get_reset_added_label_query,
+                                       **{
+                                           "record_constructor": record_constructor,
+                                           "batch_size": self.batch_size
+                                       })
+        self.connection.exec_query(di_ql.get_mark_records_as_done_query,
+                                   **{
+                                       "batch_size": self.batch_size
+                                   })
```

### Comparing `promg-0.1.0a1/src/promg/ekg_modules/db_management.py` & `promg-0.1.6/src/promg/ekg_modules/db_management.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg/ekg_modules/ekg_analysis.py` & `promg-0.1.6/src/promg/ekg_modules/ekg_analysis.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg/ekg_modules/ekg_builder_semantic_header.py` & `promg-0.1.6/src/promg/ekg_modules/ekg_builder_semantic_header.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     def _write_message_to_performance(self, message: str):
         if self.perf is not None:
             self.perf.finished_step(activity=message)
 
     def create_nodes_by_records(self, node_types: Optional[List[str]]) -> None:
         for node_constructor in self.semantic_header.get_node_by_record_constructors(node_types):
             num_ids = self.connection.exec_query(sh_ql.get_number_of_ids_query,
-                                                   **{"node_constructor": node_constructor,
-                                                      "use_record": True})
+                                                 **{
+                                                     "node_constructor": node_constructor,
+                                                     "use_record": True
+                                                 })
             merge_first = num_ids[0]['num_ids'] < 1000
 
             self.connection.exec_query(sh_ql.get_create_node_by_record_constructor_query,
                                        **{
                                            "node_constructor": node_constructor,
                                            "batch_size": self.batch_size,
                                            "merge": merge_first
@@ -38,43 +40,58 @@
                     f"using ({node_constructor.get_prevalent_record_pattern()} merged")
             else:
                 self._write_message_to_performance(f"Node ({node_constructor.get_pattern(with_properties=False)}) "
                                                    f"using ({node_constructor.get_prevalent_record_pattern()}) "
                                                    f"created")
 
             self.connection.exec_query(sh_ql.get_reset_created_record_query,
-                                       **{"node_constructor": node_constructor,
-                                          "batch_size": self.batch_size}
+                                       **{
+                                           "node_constructor": node_constructor,
+                                           "batch_size": self.batch_size
+                                       }
                                        )
             if not merge_first:
                 max_limit = self.connection.exec_query(sh_ql.get_number_of_ids_query,
                                                        **{"node_constructor": node_constructor})
                 self.connection.exec_query(sh_ql.get_merge_nodes_with_same_id_query,
-                                           **{"node_constructor": node_constructor,
-                                              "batch_size": max(self.batch_size*10, max_limit[0]['num_ids']*2)}
+                                           **{
+                                               "node_constructor": node_constructor,
+                                               "batch_size": max(self.batch_size * 10, max_limit[0]['num_ids'] * 2)
+                                           }
                                            )
 
             self._write_message_to_performance(f"Node ({node_constructor.get_pattern(with_properties=False)}) merged")
 
     def create_nodes_by_relations(self, node_types: Optional[List[str]]) -> None:
         for node_constructors in self.semantic_header.get_nodes_constructed_by_relations(node_types).values():
             for node_constructor in node_constructors:
                 self.connection.exec_query(sh_ql.get_create_nodes_by_relations_query,
-                                           **{"node_constructor": node_constructor})
+                                           **{
+                                               "node_constructor": node_constructor,
+                                               "batch_size": self.batch_size
+                                           })
                 self._write_message_to_performance(
                     message=f"Relation [{node_constructor.relation.get_pattern()}] reified as "
                             f"({node_constructor.get_pattern(with_properties=False)}) node")
 
     def create_relations_using_record(self, relation_types: Optional[List[str]]) -> None:
         # find events that are related to different entities of which one event also has a reference to the other entity
         # create a relation between these two entities
         relation: ConstructedRelation
         for relation_constructor in self.semantic_header.get_relations_constructed_by_record(relation_types):
             self.connection.exec_query(sh_ql.get_create_relation_using_record_query,
-                                       **{"relation_constructor": relation_constructor})
+                                       **{
+                                           "relation_constructor": relation_constructor,
+                                           "batch_size": self.batch_size
+                                       })
+            self.connection.exec_query(sh_ql.get_reset_created_relation_query,
+                                       **{
+                                           "relation_constructor": relation_constructor,
+                                           "batch_size": self.batch_size
+                                       })
             self._write_message_to_performance(
                 message=f"Relation {relation_constructor.get_pattern()} done")
 
     def create_relations_using_relations(self, relation_types: Optional[List[str]]) -> None:
         relation: ConstructedRelation
         for relation_constructor in self.semantic_header.get_relations_constructed_by_relations(relation_types):
             self.connection.exec_query(sh_ql.get_create_relation_by_relations_query,
@@ -88,16 +105,18 @@
 
         if entity_types is None:
             entity_types = [entity.node_type for entity in self.semantic_header.nodes]
 
         for entity in self.semantic_header.nodes:
             if entity.infer_df and entity.node_type in entity_types:
                 self.connection.exec_query(sh_ql.get_create_directly_follows_query,
-                                           **{"entity": entity, "batch_size": self.batch_size,
-                                           "event_label": event_label})
+                                           **{
+                                               "entity": entity, "batch_size": self.batch_size,
+                                               "event_label": event_label
+                                           })
                 self._write_message_to_performance(f"Created [:DF] edge for (:{entity.get_label_string()})")
 
     def merge_duplicate_df(self):
         node: ConstructedNodes
         for node in self.semantic_header.nodes:
             if node.merge_duplicate_df:
                 self.connection.exec_query(sh_ql.get_merge_duplicate_df_entity_query, **{"node": node})
```

### Comparing `promg-0.1.0a1/src/promg/ekg_modules/inference_engine.py` & `promg-0.1.6/src/promg/ekg_modules/inference_engine.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg/utilities/auxiliary_functions.py` & `promg-0.1.6/src/promg/utilities/auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg/utilities/context_manager_tqdm.py` & `promg-0.1.6/src/promg/utilities/context_manager_tqdm.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg/utilities/get_db_size.py` & `promg-0.1.6/src/promg/utilities/get_db_size.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg/utilities/performance_handling.py` & `promg-0.1.6/src/promg/utilities/performance_handling.py`

 * *Files identical despite different names*

### Comparing `promg-0.1.0a1/src/promg.egg-info/PKG-INFO` & `promg-0.1.6/src/promg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promg
-Version: 0.1.0a1
+Version: 0.1.6
 Summary: Pyhton library to build Event Knowledge Graphs
 Author: A. Swevels, D.Fahland
 License: GPL 3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `promg-0.1.0a1/src/promg.egg-info/SOURCES.txt` & `promg-0.1.6/src/promg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

