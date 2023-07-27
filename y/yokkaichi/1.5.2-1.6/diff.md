# Comparing `tmp/yokkaichi-1.5.2.tar.gz` & `tmp/yokkaichi-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yokkaichi-1.5.2.tar", last modified: Mon Jul 10 11:40:11 2023, max compression
+gzip compressed data, was "yokkaichi-1.6.tar", last modified: Thu Jul 27 00:28:08 2023, max compression
```

## Comparing `yokkaichi-1.5.2.tar` & `yokkaichi-1.6.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-10 11:40:11.371308 yokkaichi-1.5.2/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.5.2/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2949 2023-07-10 11:40:11.371308 yokkaichi-1.5.2/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2205 2023-05-24 18:11:37.000000 yokkaichi-1.5.2/README.md
--rw-r--r--   0 krystian  (1000) krystian  (1000)       57 2023-05-24 14:00:39.000000 yokkaichi-1.5.2/pyproject.toml
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-10 11:40:11.371308 yokkaichi-1.5.2/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1577 2023-07-09 21:03:26.000000 yokkaichi-1.5.2/setup.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-10 11:40:11.357974 yokkaichi-1.5.2/yokkaichi/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2923 2023-05-24 14:00:39.000000 yokkaichi-1.5.2/yokkaichi/MasscanScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     6014 2023-07-10 11:38:02.000000 yokkaichi-1.5.2/yokkaichi/ServerScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-07-10 11:39:03.000000 yokkaichi-1.5.2/yokkaichi/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     9059 2023-07-10 11:30:15.000000 yokkaichi-1.5.2/yokkaichi/__main__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1609 2023-07-09 20:54:16.000000 yokkaichi-1.5.2/yokkaichi/args_to_cfg.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     4364 2023-07-09 20:54:16.000000 yokkaichi-1.5.2/yokkaichi/config_loader.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-10 11:40:11.364641 yokkaichi-1.5.2/yokkaichi/constants/
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.5.2/yokkaichi/constants/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-05-14 19:38:14.000000 yokkaichi-1.5.2/yokkaichi/constants/rich_console.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-10 11:40:11.367974 yokkaichi-1.5.2/yokkaichi/enums/
--rw-r--r--   0 krystian  (1000) krystian  (1000)       98 2023-07-09 20:54:16.000000 yokkaichi-1.5.2/yokkaichi/enums/MasscanMethods.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       89 2023-07-09 20:54:16.000000 yokkaichi-1.5.2/yokkaichi/enums/Platforms.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:54:16.000000 yokkaichi-1.5.2/yokkaichi/enums/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1168 2023-05-24 14:00:39.000000 yokkaichi-1.5.2/yokkaichi/port_parser.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-10 11:40:11.367974 yokkaichi-1.5.2/yokkaichi/structs/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1015 2023-07-09 20:54:16.000000 yokkaichi-1.5.2/yokkaichi/structs/CFG.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.5.2/yokkaichi/structs/__init__.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-10 11:40:11.361307 yokkaichi-1.5.2/yokkaichi.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2949 2023-07-10 11:40:11.000000 yokkaichi-1.5.2/yokkaichi.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      593 2023-07-10 11:40:11.000000 yokkaichi-1.5.2/yokkaichi.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-07-10 11:40:11.000000 yokkaichi-1.5.2/yokkaichi.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       81 2023-07-10 11:40:11.000000 yokkaichi-1.5.2/yokkaichi.egg-info/requires.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-07-10 11:40:11.000000 yokkaichi-1.5.2/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.093362 yokkaichi-1.6/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.6/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3890 2023-07-27 00:28:08.093362 yokkaichi-1.6/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3148 2023-07-21 15:44:18.000000 yokkaichi-1.6/README.md
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       57 2023-05-24 14:00:39.000000 yokkaichi-1.6/pyproject.toml
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-27 00:28:08.093362 yokkaichi-1.6/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1665 2023-07-21 15:44:18.000000 yokkaichi-1.6/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.090029 yokkaichi-1.6/yokkaichi/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     4709 2023-07-27 00:25:15.000000 yokkaichi-1.6/yokkaichi/Checker.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     7361 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/IP2L_Manager.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      685 2023-07-27 00:25:15.000000 yokkaichi-1.6/yokkaichi/Results.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3226 2023-07-27 00:25:15.000000 yokkaichi-1.6/yokkaichi/ServerScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       20 2023-07-27 00:26:33.000000 yokkaichi-1.6/yokkaichi/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     4408 2023-07-27 00:25:15.000000 yokkaichi-1.6/yokkaichi/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     4749 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/config_loader.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.093362 yokkaichi-1.6/yokkaichi/constants/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       30 2023-07-15 21:48:34.000000 yokkaichi-1.6/yokkaichi/constants/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-07-15 21:48:34.000000 yokkaichi-1.6/yokkaichi/constants/_console.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.093362 yokkaichi-1.6/yokkaichi/enums/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      178 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/enums/_IP2LocDBStatus.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      151 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/enums/_IP2LocManagerUserAnswers.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      146 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/enums/_OfflinePrintingModes.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       89 2023-07-15 21:48:34.000000 yokkaichi-1.6/yokkaichi/enums/_Platforms.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      198 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/enums/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      224 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/env_loader.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1155 2023-07-20 01:23:02.000000 yokkaichi-1.6/yokkaichi/port_parser.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.093362 yokkaichi-1.6/yokkaichi/structs/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1243 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/structs/_CFG.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      135 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/structs/_EnvVariables.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      275 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/structs/_MinecraftServer.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      108 2023-07-21 15:44:18.000000 yokkaichi-1.6/yokkaichi/structs/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-27 00:28:08.093362 yokkaichi-1.6/yokkaichi.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3890 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      829 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       54 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/entry_points.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      105 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/requires.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-07-27 00:28:08.000000 yokkaichi-1.6/yokkaichi.egg-info/top_level.txt
```

### Comparing `yokkaichi-1.5.2/LICENSE.txt` & `yokkaichi-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.5.2/setup.py` & `yokkaichi-1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     description="Shodan-like server scanner for Minecraft (formely mcserverscanner)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Oreeeee",
     license="MIT",
     url="https://github.com/Oreeeee/yokkaichi",
     install_requires=[
-        "rich",
-        "mcstatus",
-        "ip2location",
-        "python-masscan",
-        "requests",
-        "tomli >= 1.1.0",
+        "rich==13.4.2",
+        "mcstatus==11.0.0",
+        "IP2Location==8.10.0",
+        "tomli==2.0.1",
+        "pyScannerWrapper==0.2.0",
     ],
     extras_require={"testing": ["pytest"]},
+    entry_points={"console_scripts": ["yokkaichi=yokkaichi.__main__:main"]},
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `yokkaichi-1.5.2/yokkaichi/config_loader.py` & `yokkaichi-1.6/yokkaichi/config_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 import tomli
 
-from .constants.rich_console import console
-from .enums.MasscanMethods import MasscanMethods
-from .enums.Platforms import Platforms
+from .constants import console
+from .enums import Platforms
 from .port_parser import parse_port_range
-from .structs.CFG import CFG
+from .structs import CFG
 
-CONFIG_VERSION = "1"
+CONFIG_VERSION = "2"
 # TODO: Bring this back to a separate file
 SAMPLE_CFG = """
 # This is an example configuration file for Yokkaichi.
 # Configure this for your preferences.
 # Pass the location to this config file with -c as an argument.
 # Example: python -m yokkaichi -c sample.toml
 # You can pass this without the file location and it will look for yokkaichi.toml in your current location.
 # Do not comment any of the config's options, it will currently cause a crash
 
-version = "1" # Changed for every change breaking config compatibility
+version = "2" # Changed for every change breaking config compatibility
 
 [platforms]
 java = true
 bedrock = false
 
 [platforms.additional]
 java_query = false # Use the Query protocol (more info, but a little bit broken and slow right now)
 
 [type]
 masscan = true # Recommended, fast
 ip_list = false # Not recommended, slow, outdated
 
 [type.options_masscan]
-ip_source = "countries" # Availible types: "countries", "list"
 args = "" # Additional arguments for masscan
-output = false
-output_location = "masscan_out.json" # Where to output masscan's results (not required)
 
 [type.options_masscan.countries]
+enabled = true
 countries = ["US", "DE"] # Standard TOML array, use ISO 3166-1 alpha-2 codes (the 2 letter ones)
 
 [type.options_masscan.list]
+enabled = false
 list = "masscan_ips.txt" # Location to the list of IPs to scan with masscan, separated by newlines
 
 [type.options_ip_list]
 list = "ips.txt" # Location to the list of IPs to scan, separated by newlines
 
 [scanner]
 ports = "25564-25566,25569" # Port list (not TOML's format! Similarly to nmap and masscan splits ports by commas and sets ranges with hyphens)
-threads = 100 # Leave this at default unless you have a lot of servers
+threads = 100 # Setting this to a higher value will make the scanning faster, but too much can crash the system or the network
+timeout = 3.0 # Timeout in seconds before assuming the server is offline
+offline_printing = "disabled" # Should the script output offline servers. "disabled" will print nothing, "offline" will print offline servers and "full_traceback" will print entire traceback
 output = "out.json" # IMPORTANT! That's where the servers go!
 
 [ip2location]
 enabled = false # Enable getting the location of the server
-db = "IP2LOCATION-LITE-DB11.BIN" # IP2Location .BIN database (get from lite.ip2location.com)
+databases_location = "ip2location_dbs/" # Where are the databases stored
+bin_filename = "IP2LOCATION-LITE-DB11.BIN"
+csv_filename = "IP2LOCATION-LITE-DB1.CSV"
+bin_code = "DB11LITEBIN" # Avoid changing this
+csv_code = "DB1LITECSV" # Avoid changing this
 cache = true # Enable for faster speed at the cost of RAM
 """.strip()
 
 
 def load_cfg(cfg_location):
     with open(cfg_location, "rb") as f:
         cfg_file = tomli.load(f)
@@ -84,40 +88,40 @@
         cfg.platforms.append(Platforms.BEDROCK)
 
     cfg.query_java = cfg_file["platforms"]["additional"]["java_query"]
 
     cfg.masscan_scan = cfg_file["type"]["masscan"]
     cfg.ip_list_scan = cfg_file["type"]["ip_list"]
 
-    if (
-        cfg_file["type"]["options_masscan"]["ip_source"]
-        == MasscanMethods.COUNTRIES.value
-    ):
-        cfg.masscan_ip_source = MasscanMethods.COUNTRIES
-    elif cfg_file["type"]["options_masscan"]["ip_source"] == MasscanMethods.LIST.value:
-        cfg.masscan_ip_source = MasscanMethods.LIST
-
     cfg.masscan_args = cfg_file["type"]["options_masscan"]["args"]
-    cfg.masscan_output = cfg_file["type"]["options_masscan"]["output"]
-    cfg.masscan_output_location = cfg_file["type"]["options_masscan"]["output_location"]
 
+    cfg.masscan_country_scan = cfg_file["type"]["options_masscan"]["countries"][
+        "enabled"
+    ]
     cfg.masscan_country_list = cfg_file["type"]["options_masscan"]["countries"][
         "countries"
     ]
 
+    cfg.masscan_ip_scan = cfg_file["type"]["options_masscan"]["list"]["enabled"]
     cfg.masscan_ip_list = cfg_file["type"]["options_masscan"]["list"]["list"]
 
     cfg.ip_list = cfg_file["type"]["options_ip_list"]["list"]
 
     cfg.ports = parse_port_range(cfg_file["scanner"]["ports"])
     cfg.threads = cfg_file["scanner"]["threads"]
+    cfg.timeout = cfg_file["scanner"]["timeout"]
+    cfg.offline_printing = cfg_file["scanner"]["offline_printing"]
     cfg.output = cfg_file["scanner"]["output"]
 
     cfg.use_ip2location = cfg_file["ip2location"]["enabled"]
-    cfg.ip2location_db = cfg_file["ip2location"]["db"]
+    cfg.ip2location_dbs = cfg_file["ip2location"]["databases_location"]
+    cfg.ip2location_db_bin = cfg_file["ip2location"]["bin_filename"]
+    cfg.ip2location_db_csv = cfg_file["ip2location"]["csv_filename"]
+    cfg.ip2location_bin_code = cfg_file["ip2location"]["bin_code"]
+    cfg.ip2location_csv_code = cfg_file["ip2location"]["csv_code"]
     cfg.ip2location_cache = cfg_file["ip2location"]["cache"]
 
     return cfg
 
 
 def write_cfg(cfg_location):
     # Write the sample config
```

### Comparing `yokkaichi-1.5.2/yokkaichi/port_parser.py` & `yokkaichi-1.6/yokkaichi/port_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .constants.rich_console import console
+from .constants import console
 
 
 def parse_port_range(unparsed_args: str) -> list:
     def verify_ints(port: any) -> None:
         try:
             int(port)
         except TypeError:
```

### Comparing `yokkaichi-1.5.2/yokkaichi/structs/CFG.py` & `yokkaichi-1.6/yokkaichi/structs/_CFG.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 
 @dataclass
 class CFG:
     platforms: list = field(default_factory=list)
     query_java: bool = field(default_factory=bool)
     masscan_scan: bool = field(default_factory=bool)
     ip_list_scan: bool = field(default_factory=bool)
-    masscan_ip_source: str = field(
-        default_factory=str
-    )  # Possible values: "countries", "list"
     masscan_args: str = field(default_factory=str)
-    masscan_output: bool = field(default_factory=bool)
-    masscan_output_location: str = field(default_factory=str)
     masscan_country_list: list = field(default_factory=list)
+    masscan_country_scan: bool = field(default_factory=bool)
     masscan_ip_list: str = field(default_factory=str)
+    masscan_ip_scan: bool = field(default_factory=bool)
     ip_list: str = field(default_factory=str)
     ports: list = field(default_factory=list)
     threads: int = field(default_factory=int)
+    timeout: float = field(default_factory=float)
+    offline_printing: str = field(default_factory=str)
     output: str = field(default_factory=str)
     use_ip2location: bool = field(default_factory=bool)
-    ip2location_db: str = field(default_factory=str)
+    ip2location_dbs: str = field(default_factory=str)
+    ip2location_db_bin: str = field(default_factory=str)
+    ip2location_db_csv: str = field(default_factory=str)
+    ip2location_bin_code: str = field(default_factory=str)
+    ip2location_csv_code: str = field(default_factory=str)
     ip2location_cache: bool = field(default_factory=bool)
```

