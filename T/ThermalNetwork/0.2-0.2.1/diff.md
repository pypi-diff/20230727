# Comparing `tmp/ThermalNetwork-0.2.tar.gz` & `tmp/ThermalNetwork-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ThermalNetwork-0.2.tar", last modified: Wed Jul 26 17:02:45 2023, max compression
+gzip compressed data, was "ThermalNetwork-0.2.1.tar", last modified: Thu Jul 27 18:24:56 2023, max compression
```

## Comparing `ThermalNetwork-0.2.tar` & `ThermalNetwork-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 17:02:45.646352 ThermalNetwork-0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-26 17:02:45.646352 ThermalNetwork-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 17:02:45.642352 ThermalNetwork-0.2/ThermalNetwork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-26 17:02:45.000000 ThermalNetwork-0.2/ThermalNetwork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-26 17:02:45.646352 ThermalNetwork-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 17:02:45.646352 ThermalNetwork-0.2/thermalnetwork/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/base_component.py
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/energy_transfer_station.py
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/fan.py
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/ground_heat_exchanger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/heat_pump.py
--rw-r--r--   0 runner    (1001) docker     (122)    24151 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/network.py
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-26 17:02:41.000000 ThermalNetwork-0.2/thermalnetwork/pump.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 18:24:56.838893 ThermalNetwork-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-27 18:24:56.838893 ThermalNetwork-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 18:24:56.838893 ThermalNetwork-0.2.1/ThermalNetwork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-27 18:24:56.000000 ThermalNetwork-0.2.1/ThermalNetwork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-27 18:24:56.000000 ThermalNetwork-0.2.1/ThermalNetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 18:24:56.000000 ThermalNetwork-0.2.1/ThermalNetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-27 18:24:56.000000 ThermalNetwork-0.2.1/ThermalNetwork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-27 18:24:56.000000 ThermalNetwork-0.2.1/ThermalNetwork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-27 18:24:56.000000 ThermalNetwork-0.2.1/ThermalNetwork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-27 18:24:56.838893 ThermalNetwork-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 18:24:56.838893 ThermalNetwork-0.2.1/thermalnetwork/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/thermalnetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/thermalnetwork/base_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/thermalnetwork/energy_transfer_station.py
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/thermalnetwork/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/thermalnetwork/fan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/thermalnetwork/ground_heat_exchanger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/thermalnetwork/heat_pump.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24034 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/thermalnetwork/network.py
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-27 18:24:54.000000 ThermalNetwork-0.2.1/thermalnetwork/pump.py
```

### Comparing `ThermalNetwork-0.2/LICENSE` & `ThermalNetwork-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.2/PKG-INFO` & `ThermalNetwork-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ThermalNetwork
-Version: 0.2
+Version: 0.2.1
 Summary: A thermal network solver for GHE sizing.
 Home-page: https://github.com/mitchute/ThermalNetwork
 Author: Matt Mitchell
 Author-email: mitchute@gmail.com
 License: BSD-3
 Description: # ThermalNetwork
```

### Comparing `ThermalNetwork-0.2/ThermalNetwork.egg-info/PKG-INFO` & `ThermalNetwork-0.2.1/ThermalNetwork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ThermalNetwork
-Version: 0.2
+Version: 0.2.1
 Summary: A thermal network solver for GHE sizing.
 Home-page: https://github.com/mitchute/ThermalNetwork
 Author: Matt Mitchell
 Author-email: mitchute@gmail.com
 License: BSD-3
 Description: # ThermalNetwork
```

### Comparing `ThermalNetwork-0.2/ThermalNetwork.egg-info/SOURCES.txt` & `ThermalNetwork-0.2.1/ThermalNetwork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.2/setup.py` & `ThermalNetwork-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.2/thermalnetwork/energy_transfer_station.py` & `ThermalNetwork-0.2.1/thermalnetwork/energy_transfer_station.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.2/thermalnetwork/fan.py` & `ThermalNetwork-0.2.1/thermalnetwork/fan.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.2/thermalnetwork/ground_heat_exchanger.py` & `ThermalNetwork-0.2.1/thermalnetwork/ground_heat_exchanger.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.2/thermalnetwork/heat_pump.py` & `ThermalNetwork-0.2.1/thermalnetwork/heat_pump.py`

 * *Files identical despite different names*

### Comparing `ThermalNetwork-0.2/thermalnetwork/network.py` & `ThermalNetwork-0.2.1/thermalnetwork/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,16 @@
                     'district_system_type': feature['properties'].get('district_system_type', ''),
                     'properties': {k: v for k, v in feature['properties'].items() if k not in [':type', ':name']},
                     'start_loop': 'true' if feature_id == startloop_feature_id else None
                 })
 
         return connected_objects
 
-    def reorder_connected_features(self, features):
+    @staticmethod
+    def reorder_connected_features(features):
         """
         Reorders a list of connected features so that the feature with 'startloop' set to 'true' is at the beginning.
 
         :param features: List of connected features.
         :return: Reordered list of connected features.
         """
         while features[0].get('start_loop') != 'true':
@@ -116,15 +117,16 @@
         converted_features.append(obj)
 
         # Convert the features from geojson list
         for feature in json_data:
             feature_type = feature['type']
             if feature_type == 'Building':
                 feature_type = 'ENERGYTRANSFERSTATION'
-                # add building directory ID to scenario path; look for dir named '_export_modelica_loads' for the building_loads.csv
+                # add building directory ID to scenario path; look for dir named
+                # '_export_modelica_loads' for the building_loads.csv
                 new_path = self.scenario_directory_path / feature['properties']['id']
                 for directory in new_path.iterdir():
                     if directory.is_dir() and "_export_modelica_loads" in directory.name:
                         new_path = new_path / directory.name / 'building_loads.csv'
                         print(f"building_loads.csv path: {new_path}\n")
                         break
                 if not Path.is_file(new_path):
@@ -169,15 +171,16 @@
         return converted_features
 
     def set_design(self, des_method_str: str, throw: bool = True) -> int:
         """
         Sets up the design method.
 
         :param des_method_str: design method string
-        :param throw: by default, function will raise an exception on error, override to false to not raise exception
+        :param throw: by default, function will raise an exception on error.
+                      override to "False" to not raise exception
         :returns: zero if successful, nonzero if failure
         :rtype: int
         """
 
         des_method_str = des_method_str.strip().upper()
 
         if des_method_str == DesignType.AREAPROPORTIONAL.name:
@@ -460,16 +463,15 @@
 
     system_parameters_data = json.loads(system_parameter_path.read_text())
     # print(f"system_parameters_data: {system_parameters_data}")
 
     # load all input data
     version: int = system_parameters_data["district_system"]["fifth_generation"]["ghe_parameters"]["version"]
     if version != VERSION:
-        print("Mismatched versions, could be a problem", file=stderr)
-        return 1
+        print("Mismatched ThermalNetwork versions. Could be a problem.", file=stderr)
 
     design_data: dict = system_parameters_data["district_system"]["fifth_generation"]["ghe_parameters"]["design"]
     print(f"design_data: {design_data}\n")
     # instantiate a new Network object
     network = Network()
     network.geojson_data = geojson_data
     network.ghe_parameters = system_parameters_data["district_system"]["fifth_generation"]["ghe_parameters"]
@@ -478,15 +480,16 @@
     # get network list from geojson
     connected_features = network.get_connected_features(geojson_data)
     print(f"Features in district loop: {connected_features}\n")
 
     reordered_features = network.reorder_connected_features(connected_features)
     print(f"Features in loop order: {reordered_features}\n")
 
-    # convert geojson type "Building","District System" to "ENERGYTRANSFERSTATION","GROUNDHEATEXCHANGER" and add properties
+    # convert geojson type "Building","District System" to "ENERGYTRANSFERSTATION",
+    # "GROUNDHEATEXCHANGER" and add properties
     network_data: list[dict] = network.convert_features(reordered_features)
     # print(f"Network data: {network_data}\n")
     # network_data: list[dict] = data["network"]
     # component_data: list[dict] = data["components"]
 
     # begin populating structures in preparation for sizing
     errors = 0
@@ -516,35 +519,31 @@
     network.size(output_directory_path)
     # network.write_outputs(output_path)
 
     return 0
 
 
 @click.command(name="ThermalNetworkCommandLine")
-@click.option("-y", "--sys_param_file", type=click.Path(exists=True), metavar="SYS_PARAM_PATH", help="Path to System Parameter file")
-@click.option("-s", "--scenario_directory", type=click.Path(exists=True), metavar="SCENARIO_DIRECTORY",
+@click.option("-y", "--system-parameter-file", type=click.Path(exists=True),
+              help="Path to System Parameter file")
+@click.option("-s", "--scenario-directory", type=click.Path(exists=True),
               help="Path to scenario directory")
-@click.option("-f", "--geojson_file", type=click.Path(exists=True), metavar="GEOJSON_FILE", help="Path to GeoJSON file")
-@click.option("-o", "--output_directory", type=click.Path(), metavar="OUTPUT_DIRECTORY",
+@click.option("-f", "--geojson-file", type=click.Path(exists=True),
+              help="Path to GeoJSON file")
+@click.option("-o", "--output-directory", type=click.Path(),
               help="Path to output directory")
 @click.version_option(VERSION)
-# @click.option(
-#     "--validate",
-#     default=False,
-#     is_flag=True,
-#     show_default=False,
-#     help="Validate input and exit."
-# )
 def run_sizer_from_cli(system_parameter_file, scenario_directory, geojson_file, output_directory):
     """
     CLI entrypoint for sizing runner.
 
     :param system_parameter_file: path to system parameter file
+    :param scenario_directory: path to scenario directory
     :param geojson_file: path to GeoJSON file
-    :param output_directory: path to output directory    :param validate: flag for input schema validation
+    :param output_directory: path to output directory
     """
 
     print("System Parameter File:", system_parameter_file)
     print("Scenario directory:", scenario_directory)
     print("GeoJSON file:", geojson_file)
     print("Output directory:", output_directory)
 
@@ -573,12 +572,13 @@
         print("Output path does not exist. attempting to create")  # Add this line
         try:
             output_directory_path.mkdir(parents=True, exist_ok=True)
         except Exception as e:
             print(f"Failed to create directory: {e}")
 
     output_directory_path = output_directory_path.resolve()
-    return run_sizer_from_cli_worker(system_parameter_path, scenario_directory_path, geojson_file_path, output_directory_path)
+    return run_sizer_from_cli_worker(system_parameter_path, scenario_directory_path,
+                                     geojson_file_path, output_directory_path)
 
 
 if __name__ == "__main__":
     exit(run_sizer_from_cli())
```

### Comparing `ThermalNetwork-0.2/thermalnetwork/pump.py` & `ThermalNetwork-0.2.1/thermalnetwork/pump.py`

 * *Files identical despite different names*

