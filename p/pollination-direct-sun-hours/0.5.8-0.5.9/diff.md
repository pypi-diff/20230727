# Comparing `tmp/pollination-direct-sun-hours-0.5.8.tar.gz` & `tmp/pollination-direct-sun-hours-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-direct-sun-hours-0.5.8.tar", last modified: Tue Oct 25 22:07:23 2022, max compression
+gzip compressed data, was "dist/pollination-direct-sun-hours-0.5.9.tar", last modified: Wed Nov 30 10:14:44 2022, max compression
```

## Comparing `pollination-direct-sun-hours-0.5.8.tar` & `pollination-direct-sun-hours-0.5.9.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     5103 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/pollination/direct_sun_hours/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/pollination/direct_sun_hours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3066 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/pollination/direct_sun_hours/_direct_sunlight_calc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9295 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/pollination/direct_sun_hours/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/pollination_direct_sun_hours.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/pollination_direct_sun_hours.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/pollination_direct_sun_hours.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/pollination_direct_sun_hours.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 22:06:41.000000 pollination-direct-sun-hours-0.5.8/pollination_direct_sun_hours.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/pollination_direct_sun_hours.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/pollination_direct_sun_hours.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:07:23.000000 pollination-direct-sun-hours-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-10-25 22:06:18.000000 pollination-direct-sun-hours-0.5.8/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/pollination/direct_sun_hours/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/pollination/direct_sun_hours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/pollination/direct_sun_hours/_direct_sunlight_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/pollination/direct_sun_hours/_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/pollination/direct_sun_hours/_prepare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/pollination/direct_sun_hours/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/pollination_direct_sun_hours.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/pollination_direct_sun_hours.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/pollination_direct_sun_hours.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/pollination_direct_sun_hours.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-30 10:14:05.000000 pollination-direct-sun-hours-0.5.9/pollination_direct_sun_hours.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/pollination_direct_sun_hours.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/pollination_direct_sun_hours.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 10:14:44.000000 pollination-direct-sun-hours-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2022-11-30 10:13:40.000000 pollination-direct-sun-hours-0.5.9/tests/validation_test.py
```

### Comparing `pollination-direct-sun-hours-0.5.8/.github/workflows/ci.yaml` & `pollination-direct-sun-hours-0.5.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours-0.5.8/.github/workflows/tests.yaml` & `pollination-direct-sun-hours-0.5.9/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours-0.5.8/LICENSE` & `pollination-direct-sun-hours-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours-0.5.8/PKG-INFO` & `pollination-direct-sun-hours-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-direct-sun-hours
-Version: 0.5.8
+Version: 0.5.9
 Summary: Direct sun hours recipe for Pollination.
 Home-page: https://github.com/pollination/direct-sun-hours
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-direct-sun-hours-0.5.8/README.md` & `pollination-direct-sun-hours-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours-0.5.8/pollination/direct_sun_hours/_direct_sunlight_calc.py` & `pollination-direct-sun-hours-0.5.9/pollination/direct_sun_hours/_direct_sunlight_calc.py`

 * *Files identical despite different names*

### Comparing `pollination-direct-sun-hours-0.5.8/pollination/direct_sun_hours/entry.py` & `pollination-direct-sun-hours-0.5.9/pollination/direct_sun_hours/_prepare_folder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-from pollination_dsl.dag import Inputs, DAG, task, Outputs
+from pollination_dsl.dag import Inputs, GroupedDAG, task, Outputs
 from dataclasses import dataclass
 from pollination.ladybug.translate import WeaToConstant
 from pollination.honeybee_radiance.sun import CreateSunMatrix, ParseSunUpHours
 from pollination.honeybee_radiance.translate import CreateRadianceFolderGrid
 from pollination.honeybee_radiance.octree import CreateOctreeWithSky
-from pollination.honeybee_radiance.grid import SplitGridFolder, MergeFolderData
-from pollination.path.copy import Copy
+from pollination.honeybee_radiance.grid import SplitGridFolder
+from pollination.path.copy import CopyFile
 from pollination.path.write import WriteInt
 
 # input/output alias
 from pollination.alias.inputs.model import hbjson_model_grid_input
 from pollination.alias.inputs.wea import wea_input
 from pollination.alias.inputs.north import north_input
 from pollination.alias.inputs.grid import grid_filter_input, \
     min_sensor_count_input, cpu_count
-from pollination.alias.outputs.daylight import direct_sun_hours_results, \
-    cumulative_sun_hour_results
-
-from ._direct_sunlight_calc import DirectSunHoursCalculation
 
 
 @dataclass
-class DirectSunHoursEntryPoint(DAG):
-    """Direct sun hours entry point."""
+class DirectSunHoursPrepareFolder(GroupedDAG):
+    """Prepare folder for direct sun hours."""
 
     # inputs
     timestep = Inputs.int(
         description='Input wea timestep. This value will be used to divide the '
         'cumulative results to ensure the units of the output are in hours.', default=1,
         spec={'type': 'integer', 'minimum': 1, 'maximum': 60}
     )
@@ -91,67 +87,57 @@
     @task(template=CreateSunMatrix, needs=[convert_wea_to_constant])
     def generate_sunpath(
         self, wea=convert_wea_to_constant._outputs.constant_wea,
         north=north, output_type=1
     ):
         """Create sunpath for sun-up-hours."""
         return [
-            {'from': CreateSunMatrix()._outputs.sunpath, 'to': 'resources/sunpath.mtx'},
+            {
+                'from': CreateSunMatrix()._outputs.sunpath,
+                'to': 'resources/sunpath.mtx'
+            },
             {
                 'from': CreateSunMatrix()._outputs.sun_modifiers,
                 'to': 'resources/suns.mod'
             }
         ]
 
     @task(template=ParseSunUpHours, needs=[generate_sunpath])
     def parse_sun_up_hours(self, sun_modifiers=generate_sunpath._outputs.sun_modifiers):
         return [
             {
                 'from': ParseSunUpHours()._outputs.sun_up_hours,
-                'to': 'results/direct_sun_hours/sun-up-hours.txt'
+                'to': 'resources/sun-up-hours.txt'
             }
         ]
 
     @task(template=WriteInt)
     def write_timestep(self, src=timestep):
         return [
             {
                 'from': WriteInt()._outputs.dst,
-                'to': 'results/direct_sun_hours/timestep.txt'
+                'to': 'resources/timestep.txt'
             }
         ]
 
-    @task(template=CreateRadianceFolderGrid)
+    @task(template=CreateRadianceFolderGrid, annotations={'main_task': True})
     def create_rad_folder(self, input_model=model, grid_filter=grid_filter):
         """Translate the input model to a radiance folder."""
         return [
             {
                 'from': CreateRadianceFolderGrid()._outputs.model_folder,
                 'to': 'model'
             },
             {
                 'from': CreateRadianceFolderGrid()._outputs.bsdf_folder,
                 'to': 'model/bsdf'
             },
             {
                 'from': CreateRadianceFolderGrid()._outputs.sensor_grids_file,
-                'to': 'results/direct_sun_hours/grids_info.json'
-            },
-            {
-                'from': CreateRadianceFolderGrid()._outputs.sensor_grids,
-                'description': 'Sensor grids information.'
-            }
-        ]
-
-    @task(template=Copy, needs=[create_rad_folder])
-    def copy_grid_info(self, src=create_rad_folder._outputs.sensor_grids_file):
-        return [
-            {
-                'from': Copy()._outputs.dst,
-                'to': 'results/cumulative/grids_info.json'
+                'to': 'resources/grids_info.json'
             }
         ]
 
     @task(
         template=CreateOctreeWithSky, needs=[generate_sunpath, create_rad_folder]
     )
     def create_octree(
@@ -179,84 +165,32 @@
             {
                 'from': SplitGridFolder()._outputs.output_folder,
                 'to': 'resources/grid'
             },
             {
                 'from': SplitGridFolder()._outputs.dist_info,
                 'to': 'initial_results/direct_sun_hours/_redist_info.json'
-            },
-            {
-                'from': SplitGridFolder()._outputs.sensor_grids,
-                'description': 'Sensor grids information.'
             }
         ]
 
-    @task(template=Copy, needs=[split_grid_folder])
+    @task(template=CopyFile, needs=[split_grid_folder])
     def copy_redist_info(self, src=split_grid_folder._outputs.dist_info):
         return [
             {
-                'from': Copy()._outputs.dst,
+                'from': CopyFile()._outputs.dst,
                 'to': 'initial_results/cumulative/_redist_info.json'
             }
         ]
 
-    @task(
-        template=DirectSunHoursCalculation,
-        needs=[create_octree, generate_sunpath, create_rad_folder, split_grid_folder],
-        loop=split_grid_folder._outputs.sensor_grids,
-        sub_folder='initial_results/{{item.full_id}}',  # subfolder for each grid
-        sub_paths={'sensor_grid': '{{item.full_id}}.pts'}  # sensor_grid sub_path
-    )
-    def direct_sun_hours_raytracing(
-        self,
-        timestep=timestep,
-        sensor_count='{{item.count}}',
-        octree_file=create_octree._outputs.scene_file,
-        grid_name='{{item.full_id}}',
-        sensor_grid=split_grid_folder._outputs.output_folder,
-        sunpath=generate_sunpath._outputs.sunpath,
-        sun_modifiers=generate_sunpath._outputs.sun_modifiers,
-        bsdfs=create_rad_folder._outputs.bsdf_folder
-    ):
-        pass
-
-    @task(
-        template=MergeFolderData,
-        needs=[direct_sun_hours_raytracing]
+    model_folder = Outputs.folder(
+        source='model', description='input model folder folder.'
     )
-    def restructure_timestep_results(
-        self, input_folder='initial_results/direct_sun_hours',
-        extension='ill'
-    ):
-        return [
-            {
-                'from': MergeFolderData()._outputs.output_folder,
-                'to': 'results/direct_sun_hours'
-            }
-        ]
 
-    @task(
-        template=MergeFolderData,
-        needs=[direct_sun_hours_raytracing]
+    resources = Outputs.folder(
+        source='resources', description='resources folder.'
     )
-    def restructure_cumulative_results(
-        self, input_folder='initial_results/cumulative',
-        extension='res'
-    ):
-        return [
-            {
-                'from': MergeFolderData()._outputs.output_folder,
-                'to': 'results/cumulative'
-            }
-        ]
 
-    direct_sun_hours = Outputs.folder(
-        source='results/direct_sun_hours',
-        description='Hourly results for direct sun hours.',
-        alias=direct_sun_hours_results
+    initial_results = Outputs.folder(
+        source='initial_results', description='initial results folder.'
     )
 
-    cumulative_sun_hours = Outputs.folder(
-        source='results/cumulative',
-        description='Cumulative direct sun hours for all the input hours.',
-        alias=cumulative_sun_hour_results
-    )
+    sensor_grids = Outputs.list(source='resources/grid/_info.json')
```

### Comparing `pollination-direct-sun-hours-0.5.8/pollination_direct_sun_hours.egg-info/PKG-INFO` & `pollination-direct-sun-hours-0.5.9/pollination_direct_sun_hours.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-direct-sun-hours
-Version: 0.5.8
+Version: 0.5.9
 Summary: Direct sun hours recipe for Pollination.
 Home-page: https://github.com/pollination/direct-sun-hours
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-direct-sun-hours-0.5.8/pollination_direct_sun_hours.egg-info/SOURCES.txt` & `pollination-direct-sun-hours-0.5.9/pollination_direct_sun_hours.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 setup.cfg
 setup.py
 .github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/tests.yaml
 pollination/direct_sun_hours/__init__.py
 pollination/direct_sun_hours/_direct_sunlight_calc.py
+pollination/direct_sun_hours/_postprocess.py
+pollination/direct_sun_hours/_prepare_folder.py
 pollination/direct_sun_hours/entry.py
 pollination_direct_sun_hours.egg-info/PKG-INFO
 pollination_direct_sun_hours.egg-info/SOURCES.txt
 pollination_direct_sun_hours.egg-info/dependency_links.txt
 pollination_direct_sun_hours.egg-info/not-zip-safe
 pollination_direct_sun_hours.egg-info/requires.txt
 pollination_direct_sun_hours.egg-info/top_level.txt
```

### Comparing `pollination-direct-sun-hours-0.5.8/setup.py` & `pollination-direct-sun-hours-0.5.9/setup.py`

 * *Files identical despite different names*

