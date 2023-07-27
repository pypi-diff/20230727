# Comparing `tmp/redfish_utilities-3.1.5.tar.gz` & `tmp/redfish_utilities-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_utilities-3.1.5.tar", last modified: Fri Jul  7 20:05:04 2023, max compression
+gzip compressed data, was "redfish_utilities-3.1.6.tar", last modified: Thu Jul 27 18:12:12 2023, max compression
```

## Comparing `redfish_utilities-3.1.5.tar` & `redfish_utilities-3.1.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    41821 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    41277 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/redfish_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22420 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/resets.py
--rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25527 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/redfish_utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/redfish_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41821 2023-07-07 20:05:03.000000 redfish_utilities-3.1.5/redfish_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 20:05:03.000000 redfish_utilities-3.1.5/redfish_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:05:03.000000 redfish_utilities-3.1.5/redfish_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 20:05:03.000000 redfish_utilities-3.1.5/redfish_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 20:05:03.000000 redfish_utilities-3.1.5/redfish_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_bios_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_boot_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_diagnostic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_event_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_power_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_sensor_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_sys_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/scripts/rf_virtual_media.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 20:05:04.359438 redfish_utilities-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-07 20:04:48.000000 redfish_utilities-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:12:12.240746 redfish_utilities-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-07-27 18:12:12.240746 redfish_utilities-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42354 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:12:12.236746 redfish_utilities-3.1.6/redfish_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23508 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/resets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25527 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/redfish_utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:12:12.240746 redfish_utilities-3.1.6/redfish_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-07-27 18:12:11.000000 redfish_utilities-3.1.6/redfish_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-27 18:12:11.000000 redfish_utilities-3.1.6/redfish_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:12:11.000000 redfish_utilities-3.1.6/redfish_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 18:12:11.000000 redfish_utilities-3.1.6/redfish_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 18:12:11.000000 redfish_utilities-3.1.6/redfish_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:12:12.240746 redfish_utilities-3.1.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_bios_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_boot_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_diagnostic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_event_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_power_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_sensor_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_sys_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/scripts/rf_virtual_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 18:12:12.240746 redfish_utilities-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-27 18:12:00.000000 redfish_utilities-3.1.6/setup.py
```

### Comparing `redfish_utilities-3.1.5/LICENSE.md` & `redfish_utilities-3.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/PKG-INFO` & `redfish_utilities-3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_utilities
-Version: 3.1.5
+Version: 3.1.6
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -259,25 +259,27 @@
 
 
 ### Manager Configuration
 
 ```
 usage: rf_manager_config.py [-h] --user USER --password PASSWORD --rhost RHOST
                             [--manager MANAGER]
-                            {info,reset,getnet,setnet} ...
+                            {info,reset,getnet,setnet,resettodefaults,settime}
+                            ...
 
 A tool to manage managers in a service
 
 positional arguments:
-  {info,reset,getnet,setnet,resettodefaults}
+  {info,reset,getnet,setnet,resettodefaults,settime}
     info                Displays information about a manager
     reset               Resets a manager
     getnet              Displays information about an Ethernet interface
     setnet              Configures an Ethernet interface
-    resettodefaults     Resets a manager to default setting
+    resettodefaults     Resets a manager to default settings
+    settime             Sets the date-time on a manager
 
 required arguments:
   --user USER, -u USER  The user name for authentication
   --password PASSWORD, -p PASSWORD
                         The password for authentication
   --rhost RHOST, -r RHOST
                         The address of the Redfish service (with scheme)
@@ -319,20 +321,42 @@
                         The type of power/reset operation to perform
   --info, -info         Indicates if reset information should be reported
 ```
 
 Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 reset -t GracefulRestart`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
-It then traverses the manager collection for the service to find the matching system specified by the *manager* argument.
+It then traverses the manager collection for the service to find the matching manager specified by the *manager* argument.
 It will perform the `Reset` action with the specified reset type from the *type* argument.
 * If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
 * If *type* is not specified, it will attempt a `GracefulRestart`.
 
 
+#### Set Time
+
+```
+usage: rf_manager_config.py settime [-h] [--datetime DATETIME] [--offset OFFSET]
+
+options:
+  -h, --help            show this help message and exit
+  --datetime DATETIME, -dt DATETIME
+                        The date-time value to set
+  --offset OFFSET, -o OFFSET
+                        The date-time offset value to set
+```
+
+Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 settime -dt 2023-07-27T12:00:00-05:00`
+
+Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 settime -o=-05:00`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the manager specified by the *manager* argument, and applies the *datetime* and *offset* values to the manager instance.
+* If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
+
+
 #### Get Network Interface
 
 ```
 usage: rf_manager_config.py getnet [-h] [--id ID]
 
 optional arguments:
   -h, --help      show this help message and exit
```

### Comparing `redfish_utilities-3.1.5/README.md` & `redfish_utilities-3.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -243,25 +243,27 @@
 
 
 ### Manager Configuration
 
 ```
 usage: rf_manager_config.py [-h] --user USER --password PASSWORD --rhost RHOST
                             [--manager MANAGER]
-                            {info,reset,getnet,setnet} ...
+                            {info,reset,getnet,setnet,resettodefaults,settime}
+                            ...
 
 A tool to manage managers in a service
 
 positional arguments:
-  {info,reset,getnet,setnet,resettodefaults}
+  {info,reset,getnet,setnet,resettodefaults,settime}
     info                Displays information about a manager
     reset               Resets a manager
     getnet              Displays information about an Ethernet interface
     setnet              Configures an Ethernet interface
-    resettodefaults     Resets a manager to default setting
+    resettodefaults     Resets a manager to default settings
+    settime             Sets the date-time on a manager
 
 required arguments:
   --user USER, -u USER  The user name for authentication
   --password PASSWORD, -p PASSWORD
                         The password for authentication
   --rhost RHOST, -r RHOST
                         The address of the Redfish service (with scheme)
@@ -303,20 +305,42 @@
                         The type of power/reset operation to perform
   --info, -info         Indicates if reset information should be reported
 ```
 
 Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 reset -t GracefulRestart`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
-It then traverses the manager collection for the service to find the matching system specified by the *manager* argument.
+It then traverses the manager collection for the service to find the matching manager specified by the *manager* argument.
 It will perform the `Reset` action with the specified reset type from the *type* argument.
 * If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
 * If *type* is not specified, it will attempt a `GracefulRestart`.
 
 
+#### Set Time
+
+```
+usage: rf_manager_config.py settime [-h] [--datetime DATETIME] [--offset OFFSET]
+
+options:
+  -h, --help            show this help message and exit
+  --datetime DATETIME, -dt DATETIME
+                        The date-time value to set
+  --offset OFFSET, -o OFFSET
+                        The date-time offset value to set
+```
+
+Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 settime -dt 2023-07-27T12:00:00-05:00`
+
+Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 settime -o=-05:00`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the manager specified by the *manager* argument, and applies the *datetime* and *offset* values to the manager instance.
+* If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
+
+
 #### Get Network Interface
 
 ```
 usage: rf_manager_config.py getnet [-h] [--id ID]
 
 optional arguments:
   -h, --help      show this help message and exit
```

### Comparing `redfish_utilities-3.1.5/redfish_utilities/__init__.py` & `redfish_utilities-3.1.6/redfish_utilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from .logs import get_log_entries
 from .logs import print_log_entries
 from .logs import clear_log_entries
 from .logs import collect_diagnostic_data
 from .logs import download_diagnostic_data
 from .managers import get_manager_ids
 from .managers import get_manager
+from .managers import set_manager
 from .managers import print_manager
 from .managers import get_manager_reset_info
 from .managers import manager_reset
 from .managers import get_manager_reset_to_defaults_info
 from .managers import manager_reset_to_defaults
 from .managers import get_manager_ethernet_interface_ids
 from .managers import get_manager_ethernet_interface
```

### Comparing `redfish_utilities-3.1.5/redfish_utilities/accounts.py` & `redfish_utilities-3.1.6/redfish_utilities/accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/collections.py` & `redfish_utilities-3.1.6/redfish_utilities/collections.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/config.py` & `redfish_utilities-3.1.6/redfish_utilities/config.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/event_service.py` & `redfish_utilities-3.1.6/redfish_utilities/event_service.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/inventory.py` & `redfish_utilities-3.1.6/redfish_utilities/inventory.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/licenses.py` & `redfish_utilities-3.1.6/redfish_utilities/licenses.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/logs.py` & `redfish_utilities-3.1.6/redfish_utilities/logs.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/managers.py` & `redfish_utilities-3.1.6/redfish_utilities/managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,14 +92,47 @@
     if manager.status == 404:
         if avail_managers is None:
             avail_managers = get_manager_ids( context )
         raise RedfishManagerNotFoundError( "The service does not contain a manager called {}; valid managers: {}".format( manager_id, ", ".join( avail_managers ) ) )
     verify_response( manager )
     return manager
 
+def set_manager( context, manager_id = None, date_time = None, date_time_offset = None ):
+    """
+    Finds a manager matching the given identifier and sets one or more properties
+
+    Args:
+        context: The Redfish client object with an open session
+        manager_id: The manager to locate; if None, perform on the only manager
+        date_time: The date-time value to set
+        date_time_offset: The date-time offset value to set
+
+    Returns:
+        The response of the PATCH
+    """
+
+    # Locate the manager
+    manager = get_manager( context, manager_id )
+
+    # Build the payload
+    payload = {}
+    if date_time is not None:
+        payload["DateTime"] = date_time
+    if date_time_offset is not None:
+        payload["DateTimeOffset"] = date_time_offset
+
+    # Update the manager
+    headers = None
+    etag = manager.getheader( "ETag" )
+    if etag is not None:
+        headers = { "If-Match": etag }
+    response = context.patch( manager.dict["@odata.id"], body = payload, headers = headers )
+    verify_response( response )
+    return response
+
 def print_manager( manager ):
     """
     Prints the manager info
 
     Args:
         manager: The manager info to print
     """
@@ -133,17 +166,17 @@
     """
 
     if manager is None:
         manager = get_manager( context, manager_id )
 
     # Check that there is a Reset action
     if "Actions" not in manager.dict:
-        raise RedfishManagerResetNotFoundError( "Manager {} does not support the Reset action".format( manager["Id"] ) )
+        raise RedfishManagerResetNotFoundError( "Manager {} does not support the Reset action".format( manager.dict["Id"] ) )
     if "#Manager.Reset" not in manager.dict["Actions"]:
-        raise RedfishManagerResetNotFoundError( "Manager {} does not support the Reset action".format( manager["Id"] ) )
+        raise RedfishManagerResetNotFoundError( "Manager {} does not support the Reset action".format( manager.dict["Id"] ) )
 
     # Extract the info about the Reset action
     reset_action = manager.dict["Actions"]["#Manager.Reset"]
     reset_uri = reset_action["target"]
 
     if "@Redfish.ActionInfo" not in reset_action:
         # No action info; need to build this manually based on other annotations
@@ -236,17 +269,17 @@
     """
 
     if manager is None:
         manager = get_manager( context, manager_id )
 
     # Check that there is a Reset action
     if "Actions" not in manager.dict:
-        raise RedfishManagerResetToDefaultsNotFoundError( "Manager {} does not support the ResetToDefaults action".format( manager["Id"] ) )
+        raise RedfishManagerResetToDefaultsNotFoundError( "Manager {} does not support the ResetToDefaults action".format( manager.dict["Id"] ) )
     if "#Manager.ResetToDefaults" not in manager.dict["Actions"]:
-        raise RedfishManagerResetToDefaultsNotFoundError( "Manager {} does not support the ResetToDefaults action".format( manager["Id"] ) )
+        raise RedfishManagerResetToDefaultsNotFoundError( "Manager {} does not support the ResetToDefaults action".format( manager.dict["Id"] ) )
 
     # Extract the info about the ResetToDefaults action
     reset_action = manager.dict["Actions"]["#Manager.ResetToDefaults"]
     reset_uri = reset_action["target"]
 
     if "@Redfish.ActionInfo" not in reset_action:
         # No action info; need to build this manually based on other annotations
```

### Comparing `redfish_utilities-3.1.5/redfish_utilities/messages.py` & `redfish_utilities-3.1.6/redfish_utilities/messages.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/resets.py` & `redfish_utilities-3.1.6/redfish_utilities/resets.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/sensors.py` & `redfish_utilities-3.1.6/redfish_utilities/sensors.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/systems.py` & `redfish_utilities-3.1.6/redfish_utilities/systems.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/tasks.py` & `redfish_utilities-3.1.6/redfish_utilities/tasks.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities/update.py` & `redfish_utilities-3.1.6/redfish_utilities/update.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/redfish_utilities.egg-info/PKG-INFO` & `redfish_utilities-3.1.6/redfish_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish-utilities
-Version: 3.1.5
+Version: 3.1.6
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -259,25 +259,27 @@
 
 
 ### Manager Configuration
 
 ```
 usage: rf_manager_config.py [-h] --user USER --password PASSWORD --rhost RHOST
                             [--manager MANAGER]
-                            {info,reset,getnet,setnet} ...
+                            {info,reset,getnet,setnet,resettodefaults,settime}
+                            ...
 
 A tool to manage managers in a service
 
 positional arguments:
-  {info,reset,getnet,setnet,resettodefaults}
+  {info,reset,getnet,setnet,resettodefaults,settime}
     info                Displays information about a manager
     reset               Resets a manager
     getnet              Displays information about an Ethernet interface
     setnet              Configures an Ethernet interface
-    resettodefaults     Resets a manager to default setting
+    resettodefaults     Resets a manager to default settings
+    settime             Sets the date-time on a manager
 
 required arguments:
   --user USER, -u USER  The user name for authentication
   --password PASSWORD, -p PASSWORD
                         The password for authentication
   --rhost RHOST, -r RHOST
                         The address of the Redfish service (with scheme)
@@ -319,20 +321,42 @@
                         The type of power/reset operation to perform
   --info, -info         Indicates if reset information should be reported
 ```
 
 Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 reset -t GracefulRestart`
 
 The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
-It then traverses the manager collection for the service to find the matching system specified by the *manager* argument.
+It then traverses the manager collection for the service to find the matching manager specified by the *manager* argument.
 It will perform the `Reset` action with the specified reset type from the *type* argument.
 * If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
 * If *type* is not specified, it will attempt a `GracefulRestart`.
 
 
+#### Set Time
+
+```
+usage: rf_manager_config.py settime [-h] [--datetime DATETIME] [--offset OFFSET]
+
+options:
+  -h, --help            show this help message and exit
+  --datetime DATETIME, -dt DATETIME
+                        The date-time value to set
+  --offset OFFSET, -o OFFSET
+                        The date-time offset value to set
+```
+
+Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 settime -dt 2023-07-27T12:00:00-05:00`
+
+Example: `rf_manager_config.py -u root -p root -r https://192.168.1.100 settime -o=-05:00`
+
+The tool will log into the service specified by the *rhost* argument using the credentials provided by the *user* and *password* arguments.
+It will then locate the manager specified by the *manager* argument, and applies the *datetime* and *offset* values to the manager instance.
+* If *manager* is not specified, and if the service has exactly one manager, it will perform the operation on the one manager.
+
+
 #### Get Network Interface
 
 ```
 usage: rf_manager_config.py getnet [-h] [--id ID]
 
 optional arguments:
   -h, --help      show this help message and exit
```

### Comparing `redfish_utilities-3.1.5/redfish_utilities.egg-info/SOURCES.txt` & `redfish_utilities-3.1.6/redfish_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_accounts.py` & `redfish_utilities-3.1.6/scripts/rf_accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_bios_settings.py` & `redfish_utilities-3.1.6/scripts/rf_bios_settings.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_boot_override.py` & `redfish_utilities-3.1.6/scripts/rf_boot_override.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_diagnostic_data.py` & `redfish_utilities-3.1.6/scripts/rf_diagnostic_data.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_discover.py` & `redfish_utilities-3.1.6/scripts/rf_discover.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_event_service.py` & `redfish_utilities-3.1.6/scripts/rf_event_service.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_licenses.py` & `redfish_utilities-3.1.6/scripts/rf_licenses.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_logs.py` & `redfish_utilities-3.1.6/scripts/rf_logs.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_manager_config.py` & `redfish_utilities-3.1.6/scripts/rf_manager_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 setnet_argget.add_argument( "--dhcpv6", "-dhcpv6", type = str, help = "The DHCPv6 configuration to set", choices = [ "Stateful", "Stateless", "Disabled", "Enabled" ] )
 setnet_argget.add_argument( "--vlan", "-vlan", type = str, help = "The VLAN enabled configuration to set", choices = [ "On", "Off" ] )
 setnet_argget.add_argument( "--vlanid", "-vlanid", type = int, help = "The VLAN ID to set" )
 setnet_argget.add_argument( "--vlanpriority", "-vlanpriority", type = int, help = "The VLAN priority to set" )
 reset_to_defaults_argget = subparsers.add_parser( "resettodefaults", help = "Resets a manager to default settings" )
 reset_to_defaults_argget.add_argument( "--type", "-t", type = str, help = "The type of reset-to-defaults operation to perform", choices = redfish_utilities.reset_to_defaults_types )
 reset_to_defaults_argget.add_argument( "--info", "-info", action = "store_true", help = "Indicates if reset-to-defaults information should be reported" )
+set_time_argget = subparsers.add_parser( "settime", help = "Sets the date-time on a manager" )
+set_time_argget.add_argument( "--datetime", "-dt", type = str, help = "The date-time value to set" )
+set_time_argget.add_argument( "--offset", "-o", type = str, help = "The date-time offset value to set" )
 args = argget.parse_args()
 
 if args.debug:
     log_file = "rf_manager_config-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
     logger.info( "rf_manager_config Trace" )
@@ -87,14 +90,16 @@
             if not printed_reset_types:
                 print( "No reset information found" )
         else:
             print( "Resetting the manager to defaults..." )
             response = redfish_utilities.manager_reset_to_defaults( redfish_obj, args.manager, args.type )
             response = redfish_utilities.poll_task_monitor( redfish_obj, response )
             redfish_utilities.verify_response( response )
+    elif args.command == "settime":
+        redfish_utilities.set_manager( redfish_obj, args.manager, args.datetime, args.offset )
     elif args.command == "getnet":
         interface = redfish_utilities.get_manager_ethernet_interface( redfish_obj, args.manager, args.id )
         redfish_utilities.print_manager_ethernet_interface( interface )
     elif args.command == "setnet":
         vlan = {}
         if args.vlan == "On":
             vlan["VLANEnable"] = True
```

### Comparing `redfish_utilities-3.1.5/scripts/rf_power_reset.py` & `redfish_utilities-3.1.6/scripts/rf_power_reset.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_raw_request.py` & `redfish_utilities-3.1.6/scripts/rf_raw_request.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_sensor_list.py` & `redfish_utilities-3.1.6/scripts/rf_sensor_list.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_sys_inventory.py` & `redfish_utilities-3.1.6/scripts/rf_sys_inventory.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_update.py` & `redfish_utilities-3.1.6/scripts/rf_update.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/scripts/rf_virtual_media.py` & `redfish_utilities-3.1.6/scripts/rf_virtual_media.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.1.5/setup.py` & `redfish_utilities-3.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open( "README.md", "r", "utf-8" ) as f:
     long_description = f.read()
 
 setup(
     name = "redfish_utilities",
-    version = "3.1.5",
+    version = "3.1.6",
     description = "Redfish Utilities",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     author = "DMTF, https://www.dmtf.org/standards/feedback",
     license = "BSD 3-clause \"New\" or \"Revised License\"",
     classifiers = [
         "Development Status :: 5 - Production/Stable",
```

