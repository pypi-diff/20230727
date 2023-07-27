# Comparing `tmp/abpandas-0.0.2.tar.gz` & `tmp/abpandas-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abpandas-0.0.2.tar", last modified: Thu Jul 27 08:10:34 2023, max compression
+gzip compressed data, was "abpandas-0.0.3.tar", last modified: Thu Jul 27 12:45:10 2023, max compression
```

## Comparing `abpandas-0.0.2.tar` & `abpandas-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 08:10:34.915096 abpandas-0.0.2/
--rw-rw-rw-   0        0        0      894 2023-07-27 08:10:34.899091 abpandas-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 08:10:34.787092 abpandas-0.0.2/abpandas/
--rw-rw-rw-   0        0        0       85 2023-07-26 18:33:02.000000 abpandas-0.0.2/abpandas/__init__.py
--rw-rw-rw-   0        0        0      739 2023-07-26 16:13:24.000000 abpandas-0.0.2/abpandas/agent.py
--rw-rw-rw-   0        0        0     6698 2023-07-26 18:33:17.000000 abpandas-0.0.2/abpandas/model.py
--rw-rw-rw-   0        0        0     1178 2023-07-26 15:50:02.000000 abpandas-0.0.2/abpandas/space.py
-drwxrwxrwx   0        0        0        0 2023-07-27 08:10:34.892095 abpandas-0.0.2/abpandas.egg-info/
--rw-rw-rw-   0        0        0      894 2023-07-27 08:10:31.000000 abpandas-0.0.2/abpandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-07-27 08:10:34.000000 abpandas-0.0.2/abpandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 08:10:31.000000 abpandas-0.0.2/abpandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-27 08:10:32.000000 abpandas-0.0.2/abpandas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-27 08:10:33.000000 abpandas-0.0.2/abpandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 08:10:34.916094 abpandas-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-07-27 08:09:34.000000 abpandas-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:45:10.870087 abpandas-0.0.3/
+-rw-rw-rw-   0        0        0      894 2023-07-27 12:45:10.865563 abpandas-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 12:45:10.838743 abpandas-0.0.3/abpandas/
+-rw-rw-rw-   0        0        0       85 2023-07-26 18:33:02.000000 abpandas-0.0.3/abpandas/__init__.py
+-rw-rw-rw-   0        0        0      739 2023-07-27 10:03:57.000000 abpandas-0.0.3/abpandas/agent.py
+-rw-rw-rw-   0        0        0     6911 2023-07-27 10:03:45.000000 abpandas-0.0.3/abpandas/model.py
+-rw-rw-rw-   0        0        0     1347 2023-07-27 12:36:56.000000 abpandas-0.0.3/abpandas/space.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:45:10.862565 abpandas-0.0.3/abpandas.egg-info/
+-rw-rw-rw-   0        0        0      894 2023-07-27 12:45:10.000000 abpandas-0.0.3/abpandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-07-27 12:45:10.000000 abpandas-0.0.3/abpandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 12:45:10.000000 abpandas-0.0.3/abpandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-27 12:45:10.000000 abpandas-0.0.3/abpandas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 12:45:10.000000 abpandas-0.0.3/abpandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 12:45:10.870541 abpandas-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1466 2023-07-27 12:45:05.000000 abpandas-0.0.3/setup.py
```

### Comparing `abpandas-0.0.2/PKG-INFO` & `abpandas-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abpandas
-Version: 0.0.2
+Version: 0.0.3
 Summary: Agent Based Pandas tool (ABPandas)
 Author: Yahya Gamal
 Author-email: <abpandas.yg@outlook.com>
 Keywords: python,Agent Based Model,Spatial,Pandas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
```

### Comparing `abpandas-0.0.2/abpandas/agent.py` & `abpandas-0.0.3/abpandas/agent.py`

 * *Files identical despite different names*

### Comparing `abpandas-0.0.2/abpandas/model.py` & `abpandas-0.0.3/abpandas/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .agent import Agent
 import geopandas as gpd
 import pandas as pd
 import fiona
 import copy
 
 class Model:
-    def __init__ (self, space, agents= []):
+    def __init__ (self, space: gpd.GeoDataFrame, agents= []):
         """
         A class containing the GIS map and all the agents
 
         Attributes
         ----------
         space: geopandas object
             a spatial map with polygons read as a geopandas object
@@ -58,15 +58,15 @@
         """
         a_temp = Agent(properties)
         a_temp.id = self.__id_counter
         self.__id_counter += 1
         self.agents.append(a_temp)
         return(a_temp)
     
-    def agents_with_id(self, id):
+    def agents_with_id(self, id: int):
         """
         Search for agents by id
 
         Parameters
         ----------
         id: int or list
             the id(s) of the agent to search for
@@ -89,15 +89,15 @@
                     if a.id == id_temp:
                         list_temp.append(a)
             return list_temp
         
         else:
             print("Invalid ID")
 
-    def agents_with_props(self, condition):
+    def agents_with_props(self, condition: str):
         """
         Search for agents based on its properties
 
         Parameters
         ----------
         condition: str
             a string representing a condition to be evaluated across all agents in the model
@@ -109,15 +109,15 @@
         """
         list_temp = []
         for agent in self.agents:
             if eval(condition):
                 list_temp.append(agent)
         return list_temp
     
-    def agents_at(self, loc_index):
+    def agents_at(self, loc_index: str):
         """
         Find all the agents based on their location index
 
         Parameters
         ----------
         loc_index: int
             the index of the polygon in the space
@@ -125,15 +125,15 @@
         Returns
         -------
         list of Agent objects
             list of Agent objects located in input index
         """
         return(self.space.at[loc_index, 'agents'])
 
-    def move_agents(self, agents, new_loc_index):
+    def move_agents(self, agents: list or Agent, new_loc_index: int):
         """
         Move an agent to a new location
 
         Parameters
         ----------
         agents: list of Agent objects or an Agent object
             the agents to move to a new location
@@ -154,15 +154,15 @@
         else:
             if agents.location_index is not None:
                 self.space.at[agents.location_index, "agents"].remove(agents)
             agents.location_index = new_loc_index
             self.space.at[new_loc_index, "agents"].append(agents)
             self.space.at[new_loc_index, "n_agents"] += 1
 
-    def remove_agents(self, agents):
+    def remove_agents(self, agents: list or Agent):
         """
         Removes agents from the model
 
         Parameters
         ----------
         agents: list of Agent objects or an Agent object
             the agents to remove from the model
@@ -173,20 +173,23 @@
         """
         if type(agents) is list:
             for a in agents:
                 self.space.at[a.location_index, 'agents'].remove(a)
                 self.space.at[a.location_index, "n_agents"] -= 1
                 self.agents.remove(a)
         
-        else:
+        elif type(agents) is Agent:
             self.space.at[agents.location_index, 'agents'].remove(agents)
             self.space.at[agents.location_index, "n_agents"] -= 1
             self.agents.remove(agents)
+        
+        else:
+            print('Error: agents are not of type Agent or a list of objects of type Agent')
 
-    def save_space(self, file_directory):
+    def save_space(self, file_directory: str):
         """
         Saves the space to a shape file name
 
         Parameters
         ----------
         file_directory: str
             the full directory of the file to be saved (should end in .shp or .pkl)
```

### Comparing `abpandas-0.0.2/abpandas/space.py` & `abpandas-0.0.3/abpandas/space.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,28 +18,37 @@
     -------
     geopandas object
         the geopandas objec read from the saved shapefile
     """
     w = shp.Writer(rf'{file_directory}')
     w.autoBalance = 1
     w.field('id')
+    w.field('x')
+    w.field('y')
     id = 0
+    x = 0
+    y = 0
     dist = 0
 
     for j in range(n_y):
+        x = 0
+        y += 1
         for i in range(n_x):
             id += 1
+            x += 1
             vertices = []
             parts = []
             vertices.append([i + dist, j + dist])
             vertices.append([i + dist + 1, j + dist])
             vertices.append([i + dist + 1, j + dist + 1])
             vertices.append([i + dist, j + dist + 1])
             parts.append(vertices)
             w.poly(parts)
-            w.record(id)
+            w.record(id= id)
+            w.record(x= x)
+            w.record(y= y)
     
     w.close()
     temp = gpd.read_file(rf'{file_directory}')
     return(temp)
```

### Comparing `abpandas-0.0.2/abpandas.egg-info/PKG-INFO` & `abpandas-0.0.3/abpandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abpandas
-Version: 0.0.2
+Version: 0.0.3
 Summary: Agent Based Pandas tool (ABPandas)
 Author: Yahya Gamal
 Author-email: <abpandas.yg@outlook.com>
 Keywords: python,Agent Based Model,Spatial,Pandas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
```

### Comparing `abpandas-0.0.2/setup.py` & `abpandas-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Agent Based Pandas tool (ABPandas)'
 LONG_DESCRIPTION = 'An Agent Based Modelling (ABM) package that can generate grid spatial shape files or work with predefined shape files.\nThe package focuses on simplicity by assigning Agents to spatial Polygons instead of assigning x and y locations for each agents.\nThis makes it useful in situations where granual movement of agents in space is not necessary (e.g. residentail location models)'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="abpandas",
```

