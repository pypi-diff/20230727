# Comparing `tmp/py_astrolab-0.5.0.tar.gz` & `tmp/py_astrolab-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.5.0.tar", max compression
+gzip compressed data, was "py_astrolab-0.5.1.tar", max compression
```

## Comparing `py_astrolab-0.5.0.tar` & `py_astrolab-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.5.0/README.md
--rwxr-xr-x   0        0        0     4901 2023-07-25 18:22:38.205897 py_astrolab-0.5.0/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    16852 2023-07-25 18:52:05.362319 py_astrolab-0.5.0/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.5.0/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    80941 2023-07-21 16:15:50.088586 py_astrolab-0.5.0/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.5.0/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.5.0/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.5.0/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    71736 2023-07-25 15:24:19.500166 py_astrolab-0.5.0/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.5.0/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12401 2023-07-25 15:23:51.791751 py_astrolab-0.5.0/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    26834 2023-07-26 15:09:24.526544 py_astrolab-0.5.0/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.5.0/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7566 2023-07-25 15:24:01.061996 py_astrolab-0.5.0/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.5.0/py_astrolab/report.py
--rwxr-xr-x   0        0        0     1828 2023-07-26 15:25:43.091683 py_astrolab-0.5.0/py_astrolab/transits.py
--rwxr-xr-x   0        0        0     5038 2023-07-25 18:48:54.917170 py_astrolab-0.5.0/py_astrolab/types.py
--rwxr-xr-x   0        0        0     9741 2023-07-26 15:25:12.372813 py_astrolab-0.5.0/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      664 2023-07-26 15:45:44.850034 py_astrolab-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0       89 2023-07-25 15:23:36.907730 py_astrolab-0.5.1/README.md
+-rwxr-xr-x   0        0        0     4901 2023-07-27 15:11:41.462674 py_astrolab-0.5.1/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    16852 2023-07-27 16:04:29.967031 py_astrolab-0.5.1/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.5.1/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    80941 2023-07-21 16:15:50.088586 py_astrolab-0.5.1/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    60114 2023-07-25 15:24:23.074123 py_astrolab-0.5.1/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    60384 2023-07-25 15:24:37.291242 py_astrolab-0.5.1/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    64742 2023-07-25 15:24:40.068434 py_astrolab-0.5.1/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    71736 2023-07-25 15:24:19.500166 py_astrolab-0.5.1/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     4922 2023-07-25 15:23:48.436964 py_astrolab-0.5.1/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12401 2023-07-25 15:23:51.791751 py_astrolab-0.5.1/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    27221 2023-07-27 15:55:55.273274 py_astrolab-0.5.1/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3105 2023-07-25 15:23:58.111196 py_astrolab-0.5.1/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7566 2023-07-25 15:24:01.061996 py_astrolab-0.5.1/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2279 2023-07-25 15:24:03.920702 py_astrolab-0.5.1/py_astrolab/report.py
+-rwxr-xr-x   0        0        0     3247 2023-07-27 20:12:31.604054 py_astrolab-0.5.1/py_astrolab/transits.py
+-rwxr-xr-x   0        0        0     5235 2023-07-27 20:11:43.719226 py_astrolab-0.5.1/py_astrolab/types.py
+-rwxr-xr-x   0        0        0     9741 2023-07-26 15:25:12.372813 py_astrolab-0.5.1/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      664 2023-07-27 20:13:38.665107 py_astrolab-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.5.1/PKG-INFO
```

### Comparing `py_astrolab-0.5.0/py_astrolab/__init__.py` & `py_astrolab-0.5.1/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/aspects.py` & `py_astrolab-0.5.1/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.5.1/py_astrolab/charts/charts_svg.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.5.1/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.5.1/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.5.1/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.5.1/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/fetch_geonames.py` & `py_astrolab-0.5.1/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/kr.config.json` & `py_astrolab-0.5.1/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/main.py` & `py_astrolab-0.5.1/py_astrolab/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -615,41 +615,49 @@
             if x == 27:
                 high = 360
             else:
                 high = sunstep[x+1]
             if degrees_between >= low and degrees_between < high:
                 sun_phase = x + 1
 
-        def moon_emoji(phase):
+        def moon_phase_interpreter(phase):
             if phase == 1:
-                result = "🌑"
+                name = 'New'
+                emoji = "🌑"
             elif phase < 7:
-                result = "🌒"
+                name = 'Waxing Crescent'
+                emoji = "🌒"
             elif 7 <= phase <= 9:
-                result = "🌓"
+                name = 'First Quarter'
+                emoji = "🌓"
             elif phase < 14:
-                result = "🌔"
+                name = 'Waxing Gibbous'
+                emoji = "🌔"
             elif phase == 14:
-                result = "🌕"
+                name = 'Full'
+                emoji = "🌕"
             elif phase < 20:
-                result = "🌖"
+                name = 'Waning Gibbous'
+                emoji = "🌖"
             elif 20 <= phase <= 22:
-                result = "🌗"
+                name = 'Last Quarter'
+                emoji = "🌗"
             elif phase <= 28:
-                result = "🌘"
-            else:
-                result = phase
-
-            return result
+                name = 'Waning Crescent'
+                emoji = "🌘"
+            return name, emoji
+        
+        moon_phase_name, moon_phase_emoji = moon_phase_interpreter(moon_phase)
 
         lunar_phase_dictionary = {
             "degrees_between_s_m": degrees_between,
             "moon_phase": moon_phase,
+            "moon_phase_name": moon_phase_name,
             "sun_phase": sun_phase,
-            "moon_emoji": moon_emoji(moon_phase)
+            "moon_emoji": moon_phase_emoji
         }
 
         self.lunar_phase = LunarPhaseObject(**lunar_phase_dictionary)
 
     def __make_lists(self):
         """ Internal function to generate the lists"""
         self.planets_list = [self.sun, self.moon, self.mercury, self.venus,
```

### Comparing `py_astrolab-0.5.0/py_astrolab/print_all_data.py` & `py_astrolab-0.5.1/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/relationship_score.py` & `py_astrolab-0.5.1/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/report.py` & `py_astrolab-0.5.1/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/py_astrolab/types.py` & `py_astrolab-0.5.1/py_astrolab/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     '🌗',
     '🌘'
 ]
 
 class LunarPhaseObject(BaseModel):
     degrees_between_s_m: Union[int, float]
     moon_phase: int
+    moon_phase_name: str
     sun_phase: int
     moon_emoji: LunarPhaseEmoji
 
     def __str__(self):
         return super().dict(exclude_none=True, exclude_unset=True, exclude_defaults=True, by_alias=False).__str__()
 
     def __repr__(self):
@@ -170,15 +171,14 @@
 
     def __delitem__(self, key):
         delattr(self, key)
     
     def get(self, key, default):
         return getattr(self, key, default)
 
-
 class KerykeionSubject(BaseModel):
     # Data
     name: str
     year: int
     month: int
     day: int
     hour: int
@@ -233,22 +233,29 @@
     # Lilith
     mean_apog: KerykeionPoint
     oscu_apog: KerykeionPoint
 
     # Lunar Phase
     lunar_phase: LunarPhaseObject
 
+class Transit(BaseModel):
+    transit_aspects: list
+    natal_aspects: list
+    points_in_houses: list
+    phase: Union[LunarPhaseObject, None]
+    new_moon: KerykeionPoint
+
 if __name__ == "__main__":
     sun = KerykeionPoint(
         name='Sun',
         element='Air',
         quality='Fixed',
         sign='Aqu',
         sign_num=1,
         position=0,
         abs_pos=12.123123,
         emoji='♈',
         point_type='Planet'
     )
 
     print(sun.json())
-    print(sun)
+    print(sun)
```

### Comparing `py_astrolab-0.5.0/py_astrolab/utilities.py` & `py_astrolab-0.5.1/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.5.0/pyproject.toml` & `py_astrolab-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.5.0"
+version = "0.5.1"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.5.0/PKG-INFO` & `py_astrolab-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

