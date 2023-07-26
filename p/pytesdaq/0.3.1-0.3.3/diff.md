# Comparing `tmp/pytesdaq-0.3.1.tar.gz` & `tmp/pytesdaq-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytesdaq-0.3.1.tar", last modified: Wed May 17 00:28:41 2023, max compression
+gzip compressed data, was "pytesdaq-0.3.3.tar", last modified: Wed Jul 26 22:35:29 2023, max compression
```

## Comparing `pytesdaq-0.3.1.tar` & `pytesdaq-0.3.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.359462 pytesdaq-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-17 00:28:41.359462 pytesdaq-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.343462 pytesdaq-0.3.1/pytesdaq/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.343462 pytesdaq-0.3.1/pytesdaq/analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27099 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/analyzer/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.343462 pytesdaq-0.3.1/pytesdaq/config/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27188 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.347462 pytesdaq-0.3.1/pytesdaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/daq/daq.py
--rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/daq/nidaqtask.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/daq/polaris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.347462 pytesdaq-0.3.1/pytesdaq/display/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/display/series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.347462 pytesdaq-0.3.1/pytesdaq/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)    78506 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.347462 pytesdaq-0.3.1/pytesdaq/instruments/feb/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/feb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/feb/feb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.351462 pytesdaq-0.3.1/pytesdaq/instruments/imacrt/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/imacrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/imacrt/imacrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/imacrt/macrtmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.351462 pytesdaq-0.3.1/pytesdaq/instruments/keysight/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/keysight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/keysight/keysight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.351462 pytesdaq-0.3.1/pytesdaq/instruments/lakeshore/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/lakeshore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61202 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/lakeshore/lakeshore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.351462 pytesdaq-0.3.1/pytesdaq/instruments/magnicon/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/magnicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/magnicon/magnicon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.355462 pytesdaq-0.3.1/pytesdaq/instruments/niadc/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/niadc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/instruments/niadc/nidevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.355462 pytesdaq-0.3.1/pytesdaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23183 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/io/filter_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    65885 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/io/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.359462 pytesdaq-0.3.1/pytesdaq/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63818 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/processing/_iv_didv_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    24567 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/processing/_iv_didv_tools_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/processing/_process_iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    65026 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/processing/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.359462 pytesdaq-0.3.1/pytesdaq/scope/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38417 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/scope/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    67331 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/scope/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.359462 pytesdaq-0.3.1/pytesdaq/sequencer/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/sequencer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45457 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/sequencer/iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/sequencer/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/sequencer/tc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.359462 pytesdaq-0.3.1/pytesdaq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/utils/arg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/utils/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/pytesdaq/utils/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 00:28:41.343462 pytesdaq-0.3.1/pytesdaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-17 00:28:41.000000 pytesdaq-0.3.1/pytesdaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-17 00:28:41.000000 pytesdaq-0.3.1/pytesdaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:28:41.000000 pytesdaq-0.3.1/pytesdaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 00:28:41.000000 pytesdaq-0.3.1/pytesdaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 00:28:41.000000 pytesdaq-0.3.1/pytesdaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 00:28:41.000000 pytesdaq-0.3.1/pytesdaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 00:28:41.359462 pytesdaq-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-17 00:28:30.000000 pytesdaq-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:29.003694 pytesdaq-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-26 22:35:29.003694 pytesdaq-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27099 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/analyzer/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27052 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/daq/daq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/daq/nidaqtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/daq/polaris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/display/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/display/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78796 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/instruments/feb/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/feb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/feb/feb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/instruments/imacrt/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/imacrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/imacrt/imacrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/imacrt/macrtmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/instruments/keysight/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/keysight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/keysight/keysight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/instruments/lakeshore/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/lakeshore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61202 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/lakeshore/lakeshore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/instruments/magnicon/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/magnicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/magnicon/magnicon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/instruments/niadc/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/niadc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/niadc/nidevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/io/filter_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70229 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/io/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63818 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/processing/_iv_didv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24567 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/processing/_iv_didv_tools_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/processing/_process_iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65026 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/processing/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/scope/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38417 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/scope/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67331 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/scope/scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/sequencer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45457 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/sequencer/iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/sequencer/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/sequencer/tc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/utils/arg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/utils/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/utils/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:35:29.003694 pytesdaq-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/setup.py
```

### Comparing `pytesdaq-0.3.1/PKG-INFO` & `pytesdaq-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.3.1
+Version: 0.3.3
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 
 # `pytesdaq`
```

### Comparing `pytesdaq-0.3.1/README.md` & `pytesdaq-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/analyzer/analyzer.py` & `pytesdaq-0.3.3/pytesdaq/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/config/settings.py` & `pytesdaq-0.3.3/pytesdaq/config/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,16 +499,15 @@
 
 
             
         # loop channel list
         for adc_chan in adc_channel_list:
             item = 'detector_config' + str(adc_chan)
             if not self._has_setting(adc_id, item):
-                raise ValueError('ERROR in get_detector_config: No detector settings found for channel '
-                                 + str(adc_chan) + '!')
+                continue
 
             settings = self._get_comma_separated_setting(adc_id, item)
             for param in settings:
                 param_split = param.split(':')
                 param_name = param_split[0]
                 param_val = float(param_split[1])
```

### Comparing `pytesdaq-0.3.1/pytesdaq/daq/daq.py` & `pytesdaq-0.3.3/pytesdaq/daq/daq.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         if self._driver_name=='polaris':
             self._driver.set_detector_config(config_dict)
         
 
 
     def run(self, run_time=60, run_type=1, run_comment='No comment',
             group_name='None', group_comment='No comment',
-            data_prefix='raw', data_path=None,
+            group_time=None, data_prefix='raw', data_path=None,
             write_config=True, debug=False):
         
         success = False
 
         # run purpose (using "run type" -> "run pupose" table)
         run_purpose = 'Test'
         if run_type in self._run_purpose_dict:
@@ -177,30 +177,37 @@
         fridge_run = self._config.get_fridge_run()
         fridge_run_start = self._config.get_fridge_run_start()
           
         # data path
         if data_path is None:
             data_path = self._config.get_data_path()
 
-            
 
+        # series start time
+        time_now = int(round(time.time()))
+      
         # run polaris
         if self._driver_name=='polaris':
 
             # polaris config
             polaris_config = self._config.get_polaris_info()
             if polaris_config:
                 self._driver.set_polaris_config(polaris_config)
 
             # run config
             run_config = dict()
             run_config['facility'] = facility_num
             run_config['fridge_run'] = fridge_run
             run_config['fridge_run_start'] = fridge_run_start
+            run_config['series_start'] = time_now
+            if group_time is not None:
+                run_config['group_start'] = group_time 
             run_config['comment'] = '"' + run_comment + '"'
+            run_config['data_purpose'] = run_purpose
+            run_config['data_type'] = run_type
             run_config['run_purpose'] = run_purpose
             run_config['run_type'] = run_type
             run_config['group_name'] = group_name
             run_config['group_comment'] = '"' + group_comment + '"'
             
             prefix = data_path + '/'
             if data_prefix:
```

### Comparing `pytesdaq-0.3.1/pytesdaq/daq/nidaqtask.py` & `pytesdaq-0.3.3/pytesdaq/daq/nidaqtask.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/daq/polaris.py` & `pytesdaq-0.3.3/pytesdaq/daq/polaris.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/display/series.py` & `pytesdaq-0.3.3/pytesdaq/display/series.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/instruments/communication.py` & `pytesdaq-0.3.3/pytesdaq/instruments/communication.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/instruments/control.py` & `pytesdaq-0.3.3/pytesdaq/instruments/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1600,33 +1600,37 @@
                                                  adc_id=adc_id,
                                                  adc_channel=adc_channel)
         )
 
         param_val = nan
         if not self._read_from_redis:
           
-            if self._squid_controller_name == 'feb':
+            if ('feb' in controller_id
+                and self._squid_controller_name=='feb'):
+
                 # CDMS FEB device
-                
                 feb_info = self._config.get_feb_subrack_slot(controller_id)
               
                 subrack = int(feb_info[0])
                 slot = int(feb_info[1])
             
                 if self._debug:
-                    print('INFO: Getting setting "' + param_name + '" from FEB')
-                    print('(subrack = ' + str(subrack) + ', slot = ' + str(slot) + 
+                    print('INFO: Getting setting "'
+                          + param_name + '" from FEB')
+                    print('(subrack = ' + str(subrack)
+                          + ', slot = ' + str(slot) + 
                           ', channel = ' + str(controller_channel) + ')')
                         
                 if self._dummy_mode:
                     param_val= 1
                 else:
 
                     if param_name == 'tes_bias':
-                        param_val = self._readout_inst.get_phonon_qet_bias(subrack, slot, controller_channel)
+                        param_val = self._readout_inst.get_phonon_qet_bias(
+                            subrack, slot, controller_channel)
 
                     elif param_name == 'squid_bias':
                         param_val = self._readout_inst.get_phonon_squid_bias(
                             subrack, slot, controller_channel
                         )
 
                     elif param_name == 'lock_point_voltage':
@@ -1685,34 +1689,39 @@
                         param_val = self._readout_inst.is_signal_generator_tes_connected(
                             subrack, slot,controller_channel
                         )
 
                     else:
                         pass
                 
-            elif self._squid_controller_name == 'magnicon':
-
+            elif ('magnicon' in controller_id
+                  and self._squid_controller_name=='magnicon'):
+                
                 if self._verbose:
                     print('INFO: Getting "' + param_name + ' for channel ' 
                           + str(controller_channel) + ' (Magnicon)')
 
 
                 if not self._dummy_mode:
                     
                     if param_name == 'tes_bias':
-                        param_val = self._readout_inst.get_tes_current_bias(controller_channel)
+                        param_val = self._readout_inst.get_tes_current_bias(
+                            controller_channel)
 
                     elif param_name == 'squid_bias':
-                        param_val = self._readout_inst.get_squid_bias(controller_channel,'I')
+                        param_val = self._readout_inst.get_squid_bias(
+                            controller_channel,'I')
 
                     elif param_name == 'lock_point_voltage':
-                        param_val = self._readout_inst.get_squid_bias(controller_channel,'V')
+                        param_val = self._readout_inst.get_squid_bias(
+                            controller_channel,'V')
 
                     elif param_name == 'feedback_gain':
-                        param_val = self._readout_inst.get_GBP(controller_channel)
+                        param_val = self._readout_inst.get_GBP(
+                            controller_channel)
 
                     elif param_name == 'output_offset':
                         # No offset setting magnicon
                         param_val = 0
                         
                     elif param_name == 'output_gain':
                         # No output gain magnicon
@@ -1752,28 +1761,27 @@
 
                     else:
                         pass
                 else:
                     param_val= 1
 
             else:
-                print('ERROR: Unknown SQUID controller "' + 
-                      self._squid_controller_name + '"!')
+                param_val= 1
 
         else:
             print('ERROR: Reading from redis N/A')
 
             
             
         return param_val
 
 
         
         
-    def _set_sensor_val(self,param_name,value, 
+    def _set_sensor_val(self,param_name, value, 
                         tes_channel=None,
                         detector_channel= None,
                         adc_id=None,adc_channel=None):
 
         
         
         """
@@ -1799,15 +1807,16 @@
               
         # ================
         # Set value
         # ================
         
         readback_val = None
 
-        if self._squid_controller_name == 'feb':
+        if ('feb' in controller_id and
+            self._squid_controller_name == 'feb'):
             # CDMS FEB device
             
             feb_info = self._config.get_feb_subrack_slot(controller_id)
             subrack = int(feb_info[0])
             slot = int(feb_info[1])
             
             if self._verbose or self._debug:
@@ -1865,15 +1874,16 @@
                         subrack, slot, controller_channel, value
                     )
                 
                 elif param_name == 'signal_gen_tes_connection':
                     self._readout_inst.connect_signal_generator_tes(subrack, slot, controller_channel, value)
                            
 
-        elif self._squid_controller_name == 'magnicon':
+        elif ('magnicon' in controller_id and
+              self._squid_controller_name == 'magnicon'):
             
             if self._verbose or self._debug:
                 print('INFO: Setting "' + param_name + '" to ' + str(value) + ' for channel ' 
                       + str(controller_channel) + ' (Magnicon)!')
 
             if not self._dummy_mode:
```

### Comparing `pytesdaq-0.3.1/pytesdaq/instruments/feb/feb.py` & `pytesdaq-0.3.3/pytesdaq/instruments/feb/feb.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/instruments/imacrt/imacrt.py` & `pytesdaq-0.3.3/pytesdaq/instruments/imacrt/imacrt.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/instruments/imacrt/macrtmodule.py` & `pytesdaq-0.3.3/pytesdaq/instruments/imacrt/macrtmodule.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/instruments/keysight/keysight.py` & `pytesdaq-0.3.3/pytesdaq/instruments/keysight/keysight.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/instruments/lakeshore/lakeshore.py` & `pytesdaq-0.3.3/pytesdaq/instruments/lakeshore/lakeshore.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/instruments/magnicon/magnicon.py` & `pytesdaq-0.3.3/pytesdaq/instruments/magnicon/magnicon.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/instruments/niadc/nidevice.py` & `pytesdaq-0.3.3/pytesdaq/instruments/niadc/nidevice.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/io/filter_hdf5.py` & `pytesdaq-0.3.3/pytesdaq/io/filter_hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -599,31 +599,44 @@
         Return:
         ------
 
         None
 
 
         """
-
+        
         # loop filter data and save data
         for chan_name, chan_dict in filter_dict.items():
-            for param_name, val in chan_dict.items():
 
-                # metadata
-                param_metadata_name = param_name + '_metadata'
-                if param_name==param_metadata_name:
+
+            # first get list of parameters
+            param_name_list = list()
+            for param_name in chan_dict.keys():
+                if '_metadata' in param_name:
                     continue
+                else:
+                    param_name_list.append(param_name)
+
+
+            # loop parameters and get value and metadata
+            for param_name in param_name_list:
                 
+                # parameter value
+                val = chan_dict[param_name]
+
+                # parameter metadata
                 metadata = None
-                if param_metadata_name in chan_dict:
-                    metadata = chan_dict[param_metadata_name]   
+                param_name_metadata = param_name + '_metadata'
+                if param_name_metadata in chan_dict.keys():
+                    metadata = chan_dict[param_name_metadata]
 
                 # save
                 self.save_param(chan_name, param_name, val,
-                                attributes=metadata, overwrite=overwrite)
+                                attributes=metadata,
+                                overwrite=overwrite)
                 
                     
 
         
     def load(self):
         """
         Load filter file into dictionary
@@ -793,15 +806,15 @@
             
         if '|' in key:
             key = key.replace('|','__')
             
             
         # check if key exist already
         file_keys = filter_file.keys()
-        if key in file_keys and not overwrite:
+        if (key in file_keys and not overwrite):
             raise ValueError('Key ' + key + ' already stored in '
                              + self._filter_file + '. Use "overwrite=True"'
                              + ' to overwrite or change file name')
 
         # save
         filter_file.put(key, value, format='fixed')
```

### Comparing `pytesdaq-0.3.1/pytesdaq/io/hdf5.py` & `pytesdaq-0.3.3/pytesdaq/io/hdf5.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,86 +3,86 @@
 00000020: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
 00000030: 6e70 0a69 6d70 6f72 7420 7061 6e64 6173  np.import pandas
 00000040: 2061 7320 7064 0a66 726f 6d20 676c 6f62   as pd.from glob
 00000050: 2069 6d70 6f72 7420 676c 6f62 0a69 6d70   import glob.imp
 00000060: 6f72 7420 7374 6174 0a69 6d70 6f72 7420  ort stat.import 
 00000070: 6d61 7470 6c6f 746c 6962 2e70 7970 6c6f  matplotlib.pyplo
 00000080: 7420 6173 2070 6c74 0a69 6d70 6f72 7420  t as plt.import 
-00000090: 7761 726e 696e 6773 0a0a 6672 6f6d 2070  warnings..from p
-000000a0: 7974 6573 6461 712e 7574 696c 7320 696d  ytesdaq.utils im
-000000b0: 706f 7274 2063 6f6e 6e65 6374 696f 6e5f  port connection_
-000000c0: 7574 696c 730a 0a5f 5f61 6c6c 5f5f 203d  utils..__all__ =
-000000d0: 205b 2748 3552 6561 6465 7227 2c20 2748   ['H5Reader', 'H
-000000e0: 3557 7269 7465 7227 2c0a 2020 2020 2020  5Writer',.      
-000000f0: 2020 2020 2027 6578 7472 6163 745f 7365       'extract_se
-00000100: 7269 6573 5f6e 756d 272c 2027 6578 7472  ries_num', 'extr
-00000110: 6163 745f 7365 7269 6573 5f6e 616d 6527  act_series_name'
-00000120: 2c0a 2020 2020 2020 2020 2020 2027 6578  ,.           'ex
-00000130: 7472 6163 745f 6475 6d70 5f6e 756d 275d  tract_dump_num']
-00000140: 0a0a 0a0a 6465 6620 6578 7472 6163 745f  ....def extract_
-00000150: 7365 7269 6573 5f6e 756d 2873 6572 6965  series_num(serie
-00000160: 735f 6e61 6d65 293a 0a20 2020 2022 2222  s_name):.    """
-00000170: 0a20 2020 2045 7874 7261 6374 2073 6572  .    Extract ser
-00000180: 6965 7320 6e75 6d62 6572 2066 726f 6d20  ies number from 
-00000190: 6669 6c65 206e 616d 6520 6f72 2073 6572  file name or ser
-000001a0: 6965 7320 6e61 6d65 0a20 2020 2041 7373  ies name.    Ass
-000001b0: 756d 6520 7365 7269 6573 206e 616d 6520  ume series name 
-000001c0: 6861 7320 7468 6520 666f 6c6c 6f77 696e  has the followin
-000001d0: 672e 2054 6869 7320 6675 6e63 7469 6f6e  g. This function
-000001e0: 0a20 2020 2073 686f 756c 6420 6f6e 6c79  .    should only
-000001f0: 2062 6520 7573 6564 2069 6620 2273 6572   be used if "ser
-00000200: 6965 735f 6e75 6d22 2069 7320 6e6f 7420  ies_num" is not 
-00000210: 7374 6f72 6564 2069 6e20 7261 7720 0a20  stored in raw . 
-00000220: 2020 2064 6174 612e 0a0a 2020 2020 4e61     data...    Na
-00000230: 6d69 6e67 2063 6f6e 7665 6e74 696f 6e3a  ming convention:
-00000240: 2020 4978 5f44 7979 7979 6d6d 6464 5f54    Ix_Dyyyymmdd_T
-00000250: 6868 6d6d 7373 0a20 2020 2020 2020 200a  hhmmss.        .
-00000260: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00000270: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000280: 2020 7365 7269 6573 5f6e 616d 6520 3a20    series_name : 
-00000290: 7374 720a 2020 2020 2020 6e61 6d65 206f  str.      name o
-000002a0: 6620 7468 6520 7365 7269 6573 2077 6974  f the series wit
-000002b0: 6820 666f 726d 6174 2028 666f 726d 6174  h format (format
-000002c0: 2049 785f 4479 7979 796d 6d64 645f 5468   Ix_Dyyyymmdd_Th
-000002d0: 686d 6d73 7329 0a0a 2020 2020 5265 7475  hmmss)..    Retu
-000002e0: 726e 0a20 2020 202d 2d2d 2d2d 2d0a 2020  rn.    ------.  
-000002f0: 2020 7365 7269 655f 6e75 6d20 3a20 6e70    serie_num : np
-00000300: 2e75 696e 7436 340a 2020 2020 2020 7365  .uint64.      se
-00000310: 7269 6573 206e 756d 6265 7220 2866 6f72  ries number (for
-00000320: 6d61 7420 7879 7979 796d 6d64 6468 686d  mat xyyyymmddhhm
-00000330: 6d73 7329 0a0a 2020 2020 2222 220a 0a20  mss)..    """.. 
-00000340: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-00000350: 616e 6365 2873 6572 6965 735f 6e61 6d65  ance(series_name
-00000360: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-00000370: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00000380: 2827 4552 524f 5220 696e 2065 7874 7261  ('ERROR in extra
-00000390: 6374 5f73 6572 6965 735f 6e75 6d3a 2073  ct_series_num: s
-000003a0: 6572 6965 7320 6e61 6d65 2073 686f 756c  eries name shoul
-000003b0: 6420 6265 2061 2073 7472 696e 6727 290a  d be a string').
-000003c0: 0a20 2020 2023 2063 6865 636b 2069 6620  .    # check if 
-000003d0: 6675 6c6c 2070 6174 680a 2020 2020 6966  full path.    if
-000003e0: 2073 6572 6965 735f 6e61 6d65 2e66 696e   series_name.fin
-000003f0: 6428 272f 2729 213d 2d31 3a0a 2020 2020  d('/')!=-1:.    
-00000400: 2020 2020 7365 7269 6573 5f6e 616d 6520      series_name 
-00000410: 3d20 7365 7269 6573 5f6e 616d 652e 7370  = series_name.sp
-00000420: 6c69 7428 272f 2729 5b2d 315d 0a20 2020  lit('/')[-1].   
-00000430: 2020 2020 200a 0a20 2020 2023 2073 706c       ..    # spl
-00000440: 6974 2073 6572 6965 7320 6e61 6d65 200a  it series name .
-00000450: 2020 2020 7365 7269 6573 5f73 706c 6974      series_split
-00000460: 203d 2073 6572 6965 735f 6e61 6d65 2e73   = series_name.s
-00000470: 706c 6974 2827 5f27 290a 0a20 2020 2023  plit('_')..    #
-00000480: 2069 6e64 6578 2066 6163 696c 6974 7920   index facility 
-00000490: 2864 6966 6665 7265 6e74 2069 6620 6669  (different if fi
-000004a0: 6c65 206f 7220 7365 7269 6573 206e 616d  le or series nam
-000004b0: 6529 0a20 2020 2069 6e64 6578 5f66 6163  e).    index_fac
-000004c0: 696c 6974 7920 3d20 300a 2020 2020 6966  ility = 0.    if
-000004d0: 2073 6572 6965 735f 7370 6c69 745b 315d   series_split[1]
-000004e0: 5b30 5d20 3d3d 2027 4927 3a0a 2020 2020  [0] == 'I':.    
-000004f0: 2020 2020 696e 6465 785f 6661 6369 6c69      index_facili
-00000500: 7479 203d 2031 0a0a 0a20 2020 2023 2063  ty = 1...    # c
+00000090: 7761 726e 696e 6773 0a69 6d70 6f72 7420  warnings.import 
+000000a0: 636f 7079 0a0a 6672 6f6d 2070 7974 6573  copy..from pytes
+000000b0: 6461 712e 7574 696c 7320 696d 706f 7274  daq.utils import
+000000c0: 2063 6f6e 6e65 6374 696f 6e5f 7574 696c   connection_util
+000000d0: 730a 0a5f 5f61 6c6c 5f5f 203d 205b 2748  s..__all__ = ['H
+000000e0: 3552 6561 6465 7227 2c20 2748 3557 7269  5Reader', 'H5Wri
+000000f0: 7465 7227 2c0a 2020 2020 2020 2020 2020  ter',.          
+00000100: 2027 6578 7472 6163 745f 7365 7269 6573   'extract_series
+00000110: 5f6e 756d 272c 2027 6578 7472 6163 745f  _num', 'extract_
+00000120: 7365 7269 6573 5f6e 616d 6527 2c0a 2020  series_name',.  
+00000130: 2020 2020 2020 2020 2027 6578 7472 6163           'extrac
+00000140: 745f 6475 6d70 5f6e 756d 275d 0a0a 6465  t_dump_num']..de
+00000150: 6620 6578 7472 6163 745f 7365 7269 6573  f extract_series
+00000160: 5f6e 756d 2873 6572 6965 735f 6e61 6d65  _num(series_name
+00000170: 293a 0a20 2020 2022 2222 0a20 2020 2045  ):.    """.    E
+00000180: 7874 7261 6374 2073 6572 6965 7320 6e75  xtract series nu
+00000190: 6d62 6572 2066 726f 6d20 6669 6c65 206e  mber from file n
+000001a0: 616d 6520 6f72 2073 6572 6965 7320 6e61  ame or series na
+000001b0: 6d65 0a20 2020 2041 7373 756d 6520 7365  me.    Assume se
+000001c0: 7269 6573 206e 616d 6520 6861 7320 7468  ries name has th
+000001d0: 6520 666f 6c6c 6f77 696e 672e 2054 6869  e following. Thi
+000001e0: 7320 6675 6e63 7469 6f6e 0a20 2020 2073  s function.    s
+000001f0: 686f 756c 6420 6f6e 6c79 2062 6520 7573  hould only be us
+00000200: 6564 2069 6620 2273 6572 6965 735f 6e75  ed if "series_nu
+00000210: 6d22 2069 7320 6e6f 7420 7374 6f72 6564  m" is not stored
+00000220: 2069 6e20 7261 7720 0a20 2020 2064 6174   in raw .    dat
+00000230: 612e 0a0a 2020 2020 4e61 6d69 6e67 2063  a...    Naming c
+00000240: 6f6e 7665 6e74 696f 6e3a 2020 4978 5f44  onvention:  Ix_D
+00000250: 7979 7979 6d6d 6464 5f54 6868 6d6d 7373  yyyymmdd_Thhmmss
+00000260: 0a20 2020 2020 2020 200a 2020 2020 5061  .        .    Pa
+00000270: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00000280: 2d2d 2d2d 2d2d 2d0a 2020 2020 7365 7269  -------.    seri
+00000290: 6573 5f6e 616d 6520 3a20 7374 720a 2020  es_name : str.  
+000002a0: 2020 2020 6e61 6d65 206f 6620 7468 6520      name of the 
+000002b0: 7365 7269 6573 2077 6974 6820 666f 726d  series with form
+000002c0: 6174 2028 666f 726d 6174 2049 785f 4479  at (format Ix_Dy
+000002d0: 7979 796d 6d64 645f 5468 686d 6d73 7329  yyymmdd_Thhmmss)
+000002e0: 0a0a 2020 2020 5265 7475 726e 0a20 2020  ..    Return.   
+000002f0: 202d 2d2d 2d2d 2d0a 2020 2020 7365 7269   ------.    seri
+00000300: 655f 6e75 6d20 3a20 6e70 2e75 696e 7436  e_num : np.uint6
+00000310: 340a 2020 2020 2020 7365 7269 6573 206e  4.      series n
+00000320: 756d 6265 7220 2866 6f72 6d61 7420 7879  umber (format xy
+00000330: 7979 796d 6d64 6468 686d 6d73 7329 0a20  yyymmddhhmmss). 
+00000340: 2020 2022 2222 0a0a 2020 2020 6966 206e     """..    if n
+00000350: 6f74 2069 7369 6e73 7461 6e63 6528 7365  ot isinstance(se
+00000360: 7269 6573 5f6e 616d 652c 2073 7472 293a  ries_name, str):
+00000370: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00000380: 616c 7565 4572 726f 7228 2745 5252 4f52  alueError('ERROR
+00000390: 2069 6e20 6578 7472 6163 745f 7365 7269   in extract_seri
+000003a0: 6573 5f6e 756d 3a20 7365 7269 6573 206e  es_num: series n
+000003b0: 616d 6520 7368 6f75 6c64 2062 6520 6120  ame should be a 
+000003c0: 7374 7269 6e67 2729 0a0a 2020 2020 2320  string')..    # 
+000003d0: 6368 6563 6b20 6966 2066 756c 6c20 7061  check if full pa
+000003e0: 7468 0a20 2020 2069 6620 7365 7269 6573  th.    if series
+000003f0: 5f6e 616d 652e 6669 6e64 2827 2f27 2921  _name.find('/')!
+00000400: 3d2d 313a 0a20 2020 2020 2020 2073 6572  =-1:.        ser
+00000410: 6965 735f 6e61 6d65 203d 2073 6572 6965  ies_name = serie
+00000420: 735f 6e61 6d65 2e73 706c 6974 2827 2f27  s_name.split('/'
+00000430: 295b 2d31 5d0a 200a 2020 2020 2320 7370  )[-1]. .    # sp
+00000440: 6c69 7420 7365 7269 6573 206e 616d 6520  lit series name 
+00000450: 0a20 2020 2073 6572 6965 735f 7370 6c69  .    series_spli
+00000460: 7420 3d20 7365 7269 6573 5f6e 616d 652e  t = series_name.
+00000470: 7370 6c69 7428 275f 2729 0a0a 2020 2020  split('_')..    
+00000480: 2320 696e 6465 7820 6661 6369 6c69 7479  # index facility
+00000490: 2028 6469 6666 6572 656e 7420 6966 2066   (different if f
+000004a0: 696c 6520 6f72 2073 6572 6965 7320 6e61  ile or series na
+000004b0: 6d65 290a 2020 2020 696e 6465 785f 6661  me).    index_fa
+000004c0: 6369 6c69 7479 203d 2030 0a20 2020 2069  cility = 0.    i
+000004d0: 6620 7365 7269 6573 5f73 706c 6974 5b31  f series_split[1
+000004e0: 5d5b 305d 203d 3d20 2749 273a 0a20 2020  ][0] == 'I':.   
+000004f0: 2020 2020 2069 6e64 6578 5f66 6163 696c       index_facil
+00000500: 6974 7920 3d20 310a 0a20 2020 2023 2063  ity = 1..    # c
 00000510: 6865 636b 2066 6f72 6d61 740a 2020 2020  heck format.    
 00000520: 6966 2028 6c65 6e28 7365 7269 6573 5f73  if (len(series_s
 00000530: 706c 6974 293c 2033 2020 6f72 0a20 2020  plit)< 3  or.   
 00000540: 2020 2020 2073 6572 6965 735f 7370 6c69       series_spli
 00000550: 745b 696e 6465 785f 6661 6369 6c69 7479  t[index_facility
 00000560: 5d5b 305d 213d 2027 4927 206f 720a 2020  ][0]!= 'I' or.  
 00000570: 2020 2020 2020 7365 7269 6573 5f73 706c        series_spl
@@ -92,4027 +92,4299 @@
 000005b0: 7370 6c69 745b 696e 6465 785f 6661 6369  split[index_faci
 000005c0: 6c69 7479 2b32 5d5b 305d 213d 2027 5427  lity+2][0]!= 'T'
 000005d0: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
 000005e0: 2056 616c 7565 4572 726f 7228 2745 5252   ValueError('ERR
 000005f0: 4f52 2069 6e20 6578 7472 6163 745f 7365  OR in extract_se
 00000600: 7269 6573 5f6e 756d 3a20 756e 6b6e 6f77  ries_num: unknow
 00000610: 6e20 7365 7269 6573 206e 616d 6520 666f  n series name fo
-00000620: 726d 6174 2127 290a 0a20 200a 2020 2020  rmat!')..  .    
-00000630: 0a20 2020 2023 2065 7874 7261 6374 2073  .    # extract s
-00000640: 6572 6965 7320 6e75 6d0a 2020 2020 7365  eries num.    se
-00000650: 7269 6573 5f6e 756d 203d 2073 6572 6965  ries_num = serie
-00000660: 735f 7370 6c69 745b 696e 6465 785f 6661  s_split[index_fa
-00000670: 6369 6c69 7479 5d5b 313a 5d20 2b20 7365  cility][1:] + se
-00000680: 7269 6573 5f73 706c 6974 5b69 6e64 6578  ries_split[index
-00000690: 5f66 6163 696c 6974 792b 315d 5b31 3a5d  _facility+1][1:]
-000006a0: 0a20 2020 2073 6572 6965 735f 6e75 6d20  .    series_num 
-000006b0: 2b3d 2073 6572 6965 735f 7370 6c69 745b  += series_split[
-000006c0: 696e 6465 785f 6661 6369 6c69 7479 2b32  index_facility+2
-000006d0: 5d5b 313a 5d0a 2020 2020 7365 7269 6573  ][1:].    series
-000006e0: 5f6e 756d 203d 206e 702e 7569 6e74 3634  _num = np.uint64
-000006f0: 2866 6c6f 6174 2873 6572 6965 735f 6e75  (float(series_nu
-00000700: 6d29 290a 0a20 2020 2072 6574 7572 6e20  m))..    return 
-00000710: 7365 7269 6573 5f6e 756d 0a0a 0a64 6566  series_num...def
-00000720: 2065 7874 7261 6374 5f73 6572 6965 735f   extract_series_
-00000730: 6e61 6d65 2873 6572 6965 735f 6e75 6d29  name(series_num)
-00000740: 3a0a 2020 2020 2222 220a 2020 2020 4578  :.    """.    Ex
-00000750: 7472 6163 7420 7365 7269 6573 206e 616d  tract series nam
-00000760: 6520 6672 6f6d 2073 6572 6965 7320 6e75  e from series nu
-00000770: 6d62 6572 0a0a 2020 2020 466f 726d 6174  mber..    Format
-00000780: 3a0a 2020 2020 5365 7269 6573 206e 616d  :.    Series nam
-00000790: 653a 2020 4978 5f44 7979 7979 6d6d 6464  e:  Ix_Dyyyymmdd
-000007a0: 5f54 6868 6d6d 7373 0a20 2020 2053 6572  _Thhmmss.    Ser
-000007b0: 6965 7320 6e75 6d3a 2078 7979 7979 6d6d  ies num: xyyyymm
-000007c0: 6464 6868 6d6d 7373 200a 2020 0a20 2020  ddhhmmss .  .   
-000007d0: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
-000007e0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-000007f0: 7365 7269 6573 5f6e 756d 3a20 696e 740a  series_num: int.
-00000800: 2020 2020 2073 6572 6965 7320 6e75 6d62       series numb
-00000810: 6572 0a0a 2020 2020 5265 7475 726e 0a20  er..    Return. 
-00000820: 2020 202d 2d2d 2d2d 2d0a 2020 2020 7365     ------.    se
-00000830: 7269 6573 5f6e 616d 6520 3a20 7374 720a  ries_name : str.
-00000840: 0a20 2020 2022 2222 0a0a 2020 2020 7365  .    """..    se
-00000850: 7269 6573 5f6e 756d 5f73 7472 203d 2073  ries_num_str = s
-00000860: 7472 2873 6572 6965 735f 6e75 6d29 0a20  tr(series_num). 
-00000870: 2020 2073 6572 6965 735f 7469 6d65 203d     series_time =
-00000880: 2027 5427 202b 2073 6572 6965 735f 6e75   'T' + series_nu
-00000890: 6d5f 7374 725b 2d36 3a5d 0a20 2020 2073  m_str[-6:].    s
-000008a0: 6572 6965 735f 6461 7920 3d20 2744 2720  eries_day = 'D' 
-000008b0: 2b20 7365 7269 6573 5f6e 756d 5f73 7472  + series_num_str
-000008c0: 5b2d 3134 3a2d 365d 0a20 2020 2073 6572  [-14:-6].    ser
-000008d0: 6965 735f 696e 7374 203d 2027 4927 202b  ies_inst = 'I' +
-000008e0: 2073 6572 6965 735f 6e75 6d5f 7374 725b   series_num_str[
-000008f0: 3a2d 3134 5d0a 2020 2020 7365 7269 6573  :-14].    series
-00000900: 5f6e 616d 6520 3d20 7365 7269 6573 5f69  _name = series_i
-00000910: 6e73 7420 2b20 275f 2720 2b20 2073 6572  nst + '_' +  ser
-00000920: 6965 735f 6461 7920 2b20 275f 2720 2b20  ies_day + '_' + 
-00000930: 7365 7269 6573 5f74 696d 650a 0a20 2020  series_time..   
-00000940: 2072 6574 7572 6e20 7365 7269 6573 5f6e   return series_n
-00000950: 616d 650a 2020 2020 0a20 2020 200a 2020  ame.    .    .  
-00000960: 2020 0a20 2020 200a 2020 2020 2020 200a    .    .       .
-00000970: 0a64 6566 2065 7874 7261 6374 5f64 756d  .def extract_dum
-00000980: 705f 6e75 6d28 6669 6c65 5f6e 616d 6529  p_num(file_name)
-00000990: 3a0a 2020 2020 2222 220a 2020 2020 4578  :.    """.    Ex
-000009a0: 7472 6163 7420 6475 6d70 206e 756d 6265  tract dump numbe
-000009b0: 7220 666f 7220 6669 6c65 206e 616d 652e  r for file name.
-000009c0: 2054 6869 7320 6675 6e63 7469 6f6e 0a20   This function. 
-000009d0: 2020 2073 686f 756c 6420 6f6e 6c79 2062     should only b
-000009e0: 6520 7573 6564 2069 6620 2264 756d 705f  e used if "dump_
-000009f0: 6e75 6d22 2069 7320 6e6f 7420 7374 6f72  num" is not stor
-00000a00: 6564 2069 6e20 7261 7720 0a20 2020 2064  ed in raw .    d
-00000a10: 6174 612e 0a0a 2020 2020 4669 6c65 206e  ata...    File n
-00000a20: 616d 6520 666f 726d 6174 3a20 7365 7269  ame format: seri
-00000a30: 6573 5f6e 616d 655f 4678 7878 782e 6864  es_name_Fxxxx.hd
-00000a40: 6635 0a20 2020 2020 2020 200a 2020 2020  f5.        .    
-00000a50: 5265 7475 726e 3a0a 0a20 2020 2064 756d  Return:..    dum
-00000a60: 705f 6e75 6d3a 2069 6e74 200a 2020 2020  p_num: int .    
-00000a70: 2872 6574 7572 6e20 4e6f 6e65 2069 6620  (return None if 
-00000a80: 6e6f 7420 6475 6d70 206e 756d 6265 7220  not dump number 
-00000a90: 666f 756e 6429 0a20 2020 2022 2222 0a0a  found).    """..
-00000aa0: 2020 2020 2320 7265 6d6f 7665 2070 6f74      # remove pot
-00000ab0: 680a 2020 2020 6966 2066 696c 655f 6e61  h.    if file_na
-00000ac0: 6d65 2e66 696e 6428 272f 2729 213d 2d31  me.find('/')!=-1
-00000ad0: 3a0a 2020 2020 2020 2020 6669 6c65 5f6e  :.        file_n
-00000ae0: 616d 6520 3d20 6669 6c65 5f6e 616d 652e  ame = file_name.
-00000af0: 7370 6c69 7428 272f 2729 5b2d 315d 0a0a  split('/')[-1]..
-00000b00: 0a20 2020 2023 2066 696e 6420 2064 756d  .    # find  dum
-00000b10: 7020 7374 7269 6e67 0a20 2020 2064 756d  p string.    dum
-00000b20: 705f 6e75 6d20 3d20 4e6f 6e65 0a20 2020  p_num = None.   
-00000b30: 2070 6f73 203d 2066 696c 655f 6e61 6d65   pos = file_name
-00000b40: 2e66 696e 6428 275f 4627 290a 2020 2020  .find('_F').    
-00000b50: 6966 2070 6f73 3e30 3a0a 2020 2020 2020  if pos>0:.      
-00000b60: 2020 6475 6d70 5f6e 756d 203d 2069 6e74    dump_num = int
-00000b70: 2866 696c 655f 6e61 6d65 5b70 6f73 2b32  (file_name[pos+2
-00000b80: 3a70 6f73 2b36 5d29 0a20 2020 2020 2020  :pos+6]).       
-00000b90: 2020 200a 2020 2020 7265 7475 726e 2064     .    return d
-00000ba0: 756d 705f 6e75 6d0a 2020 2020 0a0a 0a0a  ump_num.    ....
-00000bb0: 0a0a 0a0a 636c 6173 7320 4835 5265 6164  ....class H5Read
-00000bc0: 6572 3a0a 2020 2020 2222 220a 2020 2020  er:.    """.    
-00000bd0: 436c 6173 7320 746f 2072 6561 6420 7261  Class to read ra
-00000be0: 7720 6461 7461 2068 6466 3520 6669 6c65  w data hdf5 file
-00000bf0: 7320 7461 6b65 6e20 6279 2070 7974 6573  s taken by pytes
-00000c00: 6461 710a 2020 2020 2222 220a 2020 2020  daq.    """.    
-00000c10: 0a20 2020 200a 2020 2020 6465 6620 5f5f  .    .    def __
-00000c20: 696e 6974 5f5f 2873 656c 662c 2072 6169  init__(self, rai
-00000c30: 7365 5f65 7272 6f72 733d 5472 7565 2c20  se_errors=True, 
-00000c40: 7665 7262 6f73 653d 5472 7565 293a 0a20  verbose=True):. 
-00000c50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00000c60: 2020 2049 6e69 7469 616c 697a 6520 4835     Initialize H5
-00000c70: 5265 6164 6572 0a0a 2020 2020 2020 2020  Reader..        
-00000c80: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00000c90: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000ca0: 2020 2020 2020 7261 6973 655f 6572 726f        raise_erro
-00000cb0: 7273 203a 2062 6f6f 6c65 616e 2c20 6f70  rs : boolean, op
-00000cc0: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00000cd0: 2069 6620 5472 7565 2072 6169 7365 2056   if True raise V
-00000ce0: 616c 7565 4572 726f 7220 2864 6566 6175  alueError (defau
-00000cf0: 6c74 290a 2020 2020 2020 2020 2020 6966  lt).          if
-00000d00: 2046 616c 7365 2c20 6469 7370 6c61 7920   False, display 
-00000d10: 6572 726f 7220 616e 6420 7265 7475 726e  error and return
-00000d20: 2065 6d70 7479 2063 6f6e 7461 696e 6572   empty container
-00000d30: 730a 0a20 2020 2020 2020 2076 6572 626f  s..        verbo
-00000d40: 7365 203a 2062 6f6f 6c65 616e 2c20 6f70  se : boolean, op
-00000d50: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00000d60: 2069 6620 5472 7565 2c20 6469 7370 6c61   if True, displa
-00000d70: 7920 6d65 7373 6167 6573 2028 6465 6661  y messages (defa
-00000d80: 756c 7429 0a20 2020 2020 2020 200a 2020  ult).        .  
-00000d90: 2020 2020 2020 0a20 2020 2020 2020 2052        .        R
-00000da0: 6574 7572 6e0a 2020 2020 2020 2020 2d2d  eturn.        --
-00000db0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-00000dc0: 650a 0a20 2020 2020 2020 2022 2222 0a20  e..        """. 
-00000dd0: 2020 2020 2020 200a 0a0a 2020 2020 2020         ...      
-00000de0: 2020 7365 6c66 2e5f 7261 6973 655f 6572    self._raise_er
-00000df0: 726f 7273 203d 2072 6169 7365 5f65 7272  rors = raise_err
-00000e00: 6f72 730a 2020 2020 2020 2020 7365 6c66  ors.        self
-00000e10: 2e5f 7665 7262 6f73 6520 3d20 7665 7262  ._verbose = verb
-00000e20: 6f73 650a 2020 2020 2020 2020 0a20 2020  ose.        .   
-00000e30: 2020 2020 2023 206c 6973 7420 6f66 2066       # list of f
-00000e40: 696c 6573 0a20 2020 2020 2020 2073 656c  iles.        sel
-00000e50: 662e 5f66 696c 655f 6c69 7374 203d 206c  f._file_list = l
-00000e60: 6973 7428 290a 2020 2020 2020 2020 0a0a  ist().        ..
-00000e70: 2020 2020 2020 2020 2320 6375 7272 656e          # curren
-00000e80: 7420 6669 6c65 2069 6e66 6f0a 2020 2020  t file info.    
-00000e90: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
-00000ea0: 745f 6669 6c65 203d 204e 6f6e 650a 2020  t_file = None.  
-00000eb0: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
-00000ec0: 656e 745f 6669 6c65 5f6e 616d 6520 3d20  ent_file_name = 
-00000ed0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-00000ee0: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
-00000ef0: 6d65 7461 6461 7461 203d 204e 6f6e 650a  metadata = None.
-00000f00: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-00000f10: 7272 656e 745f 6669 6c65 5f6e 625f 6576  rrent_file_nb_ev
-00000f20: 656e 7473 203d 2030 0a20 2020 2020 2020  ents = 0.       
-00000f30: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-00000f40: 696c 655f 6576 656e 745f 636f 756e 7465  ile_event_counte
-00000f50: 7220 3d20 300a 2020 2020 2020 200a 2020  r = 0.       .  
-00000f60: 2020 2020 2020 2320 6576 656e 7420 636f        # event co
-00000f70: 756e 7465 720a 2020 2020 2020 2020 7365  unter.        se
-00000f80: 6c66 2e5f 676c 6f62 616c 5f65 7665 6e74  lf._global_event
-00000f90: 5f63 6f75 6e74 6572 203d 2030 0a20 2020  _counter = 0.   
-00000fa0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00000fb0: 2066 696c 6520 636f 756e 7465 720a 2020   file counter.  
-00000fc0: 2020 2020 2020 7365 6c66 2e5f 6669 6c65        self._file
-00000fd0: 5f63 6f75 6e74 6572 203d 2030 0a20 2020  _counter = 0.   
-00000fe0: 2020 2020 200a 2020 2020 0a20 2020 2064       .    .    d
-00000ff0: 6566 2073 6574 5f66 696c 6573 2873 656c  ef set_files(sel
-00001000: 662c 2066 696c 6570 6174 6873 293a 0a20  f, filepaths):. 
-00001010: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00001020: 2020 2043 7265 6174 6520 6120 6c69 7374     Create a list
-00001030: 206f 6620 6669 6c65 7320 2866 756c 6c20   of files (full 
-00001040: 7061 7468 2920 616e 6420 7361 7665 200a  path) and save .
-00001050: 2020 2020 2020 2020 696e 2069 6e74 6572          in inter
-00001060: 6e61 6c20 6174 7472 6962 7574 650a 0a20  nal attribute.. 
-00001070: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00001080: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00001090: 2d2d 2d2d 0a20 2020 2020 2020 2066 696c  ----.        fil
-000010a0: 6570 6174 6873 203a 2073 7472 206f 7220  epaths : str or 
-000010b0: 6c69 7374 0a20 2020 2020 2020 2020 6669  list.         fi
-000010c0: 6c65 2f64 6972 6563 746f 7279 2061 6e64  le/directory and
-000010d0: 2f6f 7220 6c69 7374 206f 6620 6669 6c65  /or list of file
-000010e0: 732f 6469 7265 6374 6f72 6965 730a 0a20  s/directories.. 
-000010f0: 2020 2020 2020 2052 6574 7572 6e0a 2020         Return.  
-00001100: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
-00001110: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
-00001120: 2020 2022 2222 0a20 2020 2020 2020 200a     """.        .
-00001130: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
-00001140: 6172 2829 0a20 2020 2020 2020 2073 656c  ar().        sel
-00001150: 662e 5f66 696c 655f 6c69 7374 203d 206c  f._file_list = l
-00001160: 6973 7428 290a 2020 2020 2020 2020 0a20  ist().        . 
-00001170: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00001180: 616e 6365 2866 696c 6570 6174 6873 2c20  ance(filepaths, 
-00001190: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-000011a0: 2020 6669 6c65 7061 7468 7320 3d20 5b66    filepaths = [f
-000011b0: 696c 6570 6174 6873 5d0a 0a20 2020 2020  ilepaths]..     
-000011c0: 2020 2023 206c 6f6f 7020 6669 6c65 2f70     # loop file/p
-000011d0: 6174 6820 6c69 7374 2074 6f20 6765 7420  ath list to get 
-000011e0: 6c69 7374 206f 6620 6669 6c65 730a 2020  list of files.  
-000011f0: 2020 2020 2020 6669 6c65 5f6c 6973 745f        file_list_
-00001200: 7465 6d70 2020 3d20 6c69 7374 2829 0a20  temp  = list(). 
-00001210: 2020 2020 2020 2066 6f72 2066 696c 6570         for filep
-00001220: 6174 6820 696e 2066 696c 6570 6174 6873  ath in filepaths
-00001230: 3a0a 2020 2020 2020 2020 2020 2020 0a20  :.            . 
-00001240: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
-00001250: 2e70 6174 682e 6973 6469 7228 6669 6c65  .path.isdir(file
-00001260: 7061 7468 293a 0a20 2020 2020 2020 2020  path):.         
-00001270: 2020 2020 2020 2066 696c 655f 6c69 7374         file_list
-00001280: 5f74 656d 702e 6578 7465 6e64 2867 6c6f  _temp.extend(glo
-00001290: 6228 6669 6c65 7061 7468 2b27 2f2a 2e68  b(filepath+'/*.h
-000012a0: 6466 3527 2929 0a20 2020 2020 2020 2020  df5')).         
-000012b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000012c0: 2020 2020 2020 2020 2069 6620 6669 6c65           if file
-000012d0: 7061 7468 5b2d 343a 5d21 3d27 6864 6635  path[-4:]!='hdf5
-000012e0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-000012f0: 2020 2020 2020 2066 696c 6570 6174 6820         filepath 
-00001300: 2b3d 2027 2e68 6466 3527 0a20 2020 2020  += '.hdf5'.     
-00001310: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
-00001320: 2e70 6174 682e 6973 6669 6c65 2866 696c  .path.isfile(fil
-00001330: 6570 6174 6829 3a0a 2020 2020 2020 2020  epath):.        
-00001340: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00001350: 5f6c 6973 745f 7465 6d70 2e61 7070 656e  _list_temp.appen
-00001360: 6428 6669 6c65 7061 7468 290a 2020 2020  d(filepath).    
-00001370: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001380: 2069 6620 6e6f 7420 6669 6c65 5f6c 6973   if not file_lis
-00001390: 745f 7465 6d70 3a0a 2020 2020 2020 2020  t_temp:.        
-000013a0: 2020 2020 6966 2073 656c 662e 5f72 6169      if self._rai
-000013b0: 7365 5f65 7272 6f72 733a 0a20 2020 2020  se_errors:.     
-000013c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000013d0: 2056 616c 7565 4572 726f 7228 274e 6f20   ValueError('No 
-000013e0: 6669 6c65 7320 666f 756e 6421 2729 0a20  files found!'). 
-000013f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00001400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001410: 2070 7269 6e74 2827 4552 524f 523a 204e   print('ERROR: N
-00001420: 6f20 6669 6c65 7320 666f 756e 6421 2729  o files found!')
-00001430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001440: 2072 6574 7572 6e0a 0a0a 2020 2020 2020   return...      
-00001450: 2020 2320 6c6f 6f70 2061 6761 696e 2074    # loop again t
-00001460: 6f20 6368 6563 6b20 666f 7220 6475 706c  o check for dupl
-00001470: 6963 6174 650a 2020 2020 2020 2020 7365  icate.        se
-00001480: 6c66 2e5f 6669 6c65 5f6c 6973 7420 3d20  lf._file_list = 
-00001490: 6c69 7374 2829 0a20 2020 2020 2020 2066  list().        f
-000014a0: 696c 655f 6e61 6d65 5f6c 6973 7420 3d20  ile_name_list = 
-000014b0: 6c69 7374 2829 0a20 2020 2020 2020 2066  list().        f
-000014c0: 6f72 2066 696c 655f 6e61 6d65 2069 6e20  or file_name in 
-000014d0: 6669 6c65 5f6c 6973 745f 7465 6d70 3a0a  file_list_temp:.
-000014e0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-000014f0: 5f6e 616d 655f 7370 6c69 7420 3d20 6669  _name_split = fi
-00001500: 6c65 5f6e 616d 650a 2020 2020 2020 2020  le_name.        
-00001510: 2020 2020 6966 2066 696c 655f 6e61 6d65      if file_name
-00001520: 2e66 696e 6428 272f 2729 213d 2d31 3a0a  .find('/')!=-1:.
-00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 6669 6c65 5f6e 616d 655f 7370 6c69 7420  file_name_split 
-00001550: 3d20 6669 6c65 5f6e 616d 652e 7370 6c69  = file_name.spli
-00001560: 7428 272f 2729 5b2d 315d 0a20 2020 2020  t('/')[-1].     
-00001570: 2020 2020 2020 2069 6620 6669 6c65 5f6e         if file_n
-00001580: 616d 655f 7370 6c69 7420 6e6f 7420 696e  ame_split not in
-00001590: 2066 696c 655f 6e61 6d65 5f6c 6973 743a   file_name_list:
-000015a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000015b0: 2066 696c 655f 6e61 6d65 5f6c 6973 742e   file_name_list.
-000015c0: 6170 7065 6e64 2866 696c 655f 6e61 6d65  append(file_name
-000015d0: 5f73 706c 6974 290a 2020 2020 2020 2020  _split).        
-000015e0: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
-000015f0: 6c65 5f6c 6973 742e 6170 7065 6e64 2866  le_list.append(f
-00001600: 696c 655f 6e61 6d65 290a 2020 2020 2020  ile_name).      
-00001610: 2020 2320 736f 7274 0a20 2020 2020 2020    # sort.       
-00001620: 2073 656c 662e 5f66 696c 655f 6c69 7374   self._file_list
-00001630: 203d 2073 6f72 7465 6428 7365 6c66 2e5f   = sorted(self._
-00001640: 6669 6c65 5f6c 6973 7429 0a20 2020 2020  file_list).     
-00001650: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00001660: 0a20 200a 2020 2020 6465 6620 636c 6f73  .  .    def clos
-00001670: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00001680: 2022 2222 0a20 2020 2020 2020 2043 6c6f   """.        Clo
-00001690: 7365 2063 7572 7265 6e74 2066 696c 6520  se current file 
-000016a0: 616e 6420 696e 6974 6961 6c69 7a65 200a  and initialize .
-000016b0: 2020 2020 2020 2020 6669 6c65 206e 616d          file nam
-000016c0: 6520 7061 7261 6d74 6572 730a 0a20 2020  e paramters..   
-000016d0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-000016e0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-000016f0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-00001700: 0a20 2020 2020 2020 2052 6574 7572 6e0a  .        Return.
-00001710: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0a20          ------. 
-00001720: 2020 2020 2020 204e 6f6e 650a 2020 2020         None.    
-00001730: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00001740: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
-00001750: 6c6f 7365 5f66 696c 6528 290a 0a20 2020  lose_file()..   
-00001760: 2020 2020 200a 2020 2020 6465 6620 636c       .    def cl
-00001770: 6561 7228 7365 6c66 293a 0a20 2020 2020  ear(self):.     
-00001780: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00001790: 6c6f 7365 2063 7572 7265 6e74 2066 696c  lose current fil
-000017a0: 6520 616e 6420 696e 6974 6961 6c69 7a65  e and initialize
-000017b0: 200a 2020 2020 2020 2020 6669 6c65 206e   .        file n
-000017c0: 616d 6520 7061 7261 6d65 7465 7273 2061  ame parameters a
-000017d0: 6e64 2063 6f75 6e74 6572 730a 0a20 2020  nd counters..   
-000017e0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-000017f0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00001800: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-00001810: 0a20 2020 2020 2020 2052 6574 7572 6e0a  .        Return.
-00001820: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0a20          ------. 
-00001830: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
-00001840: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00001850: 200a 2020 2020 2020 2020 7365 6c66 2e5f   .        self._
-00001860: 636c 6f73 655f 6669 6c65 2829 0a20 2020  close_file().   
-00001870: 2020 2020 2073 656c 662e 5f66 696c 655f       self._file_
-00001880: 636f 756e 7465 7220 3d20 300a 2020 2020  counter = 0.    
-00001890: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
-000018a0: 745f 6669 6c65 203d 204e 6f6e 650a 2020  t_file = None.  
-000018b0: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
-000018c0: 656e 745f 6669 6c65 5f6e 616d 6520 3d20  ent_file_name = 
-000018d0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-000018e0: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
-000018f0: 6d65 7461 6461 7461 203d 204e 6f6e 650a  metadata = None.
-00001900: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-00001910: 7272 656e 745f 6669 6c65 5f65 7665 6e74  rrent_file_event
-00001920: 5f63 6f75 6e74 6572 3d20 300a 2020 2020  _counter= 0.    
-00001930: 2020 2020 7365 6c66 2e5f 676c 6f62 616c      self._global
-00001940: 5f65 7665 6e74 5f63 6f75 6e74 6572 203d  _event_counter =
-00001950: 2030 0a0a 0a20 2020 2064 6566 2072 6577   0...    def rew
-00001960: 696e 6428 7365 6c66 293a 0a20 2020 2020  ind(self):.     
-00001970: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00001980: 6577 696e 6420 746f 2062 6567 696e 6e69  ewind to beginni
-00001990: 6e67 206f 6620 6669 6c65 2873 290a 2020  ng of file(s).  
-000019a0: 2020 2020 2020 7265 6f70 656e 2e2e 2e2e        reopen....
-000019b0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-000019c0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-000019d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-000019e0: 4e6f 6e65 0a0a 2020 2020 2020 2020 5265  None..        Re
-000019f0: 7475 726e 0a20 2020 2020 2020 202d 2d2d  turn.        ---
-00001a00: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-00001a10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00001a20: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-00001a30: 2020 2020 2020 2320 6966 206d 756c 7469        # if multi
-00001a40: 706c 6520 6669 6c65 7320 2d3e 2063 6c6f  ple files -> clo
-00001a50: 7365 2063 7572 7265 6e74 2066 696c 6520  se current file 
-00001a60: 7468 656e 2072 656f 7065 6e20 6669 7273  then reopen firs
-00001a70: 7420 6669 6c65 0a20 2020 2020 2020 2069  t file.        i
-00001a80: 6620 6c65 6e28 7365 6c66 2e5f 6669 6c65  f len(self._file
-00001a90: 5f6c 6973 7429 3e31 3a0a 2020 2020 2020  _list)>1:.      
-00001aa0: 2020 2020 2020 7365 6c66 2e5f 636c 6f73        self._clos
-00001ab0: 655f 6669 6c65 2829 0a20 2020 2020 2020  e_file().       
-00001ac0: 2020 2020 2073 656c 662e 5f6f 7065 6e5f       self._open_
-00001ad0: 6669 6c65 2873 656c 662e 5f66 696c 655f  file(self._file_
-00001ae0: 6c69 7374 5b30 5d29 0a20 2020 200a 2020  list[0]).    .  
-00001af0: 2020 2020 2020 2320 696e 6974 6961 6c69        # initiali
-00001b00: 7a65 0a20 2020 2020 2020 2073 656c 662e  ze.        self.
-00001b10: 5f66 696c 655f 636f 756e 7465 7220 3d20  _file_counter = 
-00001b20: 300a 2020 2020 2020 2020 7365 6c66 2e5f  0.        self._
-00001b30: 6375 7272 656e 745f 6669 6c65 5f65 7665  current_file_eve
-00001b40: 6e74 5f63 6f75 6e74 6572 203d 2030 0a20  nt_counter = 0. 
-00001b50: 2020 2020 2020 2073 656c 662e 5f67 6c6f         self._glo
-00001b60: 6261 6c5f 6576 656e 745f 636f 756e 7465  bal_event_counte
-00001b70: 7220 3d20 300a 0a0a 0a0a 2020 2020 6465  r = 0.....    de
-00001b80: 6620 7265 6164 5f6e 6578 745f 6576 656e  f read_next_even
-00001b90: 7428 7365 6c66 2c20 6465 7465 6374 6f72  t(self, detector
-00001ba0: 5f63 6861 6e73 3d4e 6f6e 652c 0a20 2020  _chans=None,.   
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bc0: 2020 2020 2061 6463 746f 766f 6c74 3d46       adctovolt=F
-00001bd0: 616c 7365 2c20 6164 6374 6f61 6d70 3d46  alse, adctoamp=F
-00001be0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00001c00: 7365 6c69 6e65 7375 623d 4661 6c73 652c  selinesub=False,
-00001c10: 2062 6173 656c 696e 6569 6e64 733d 4e6f   baselineinds=No
-00001c20: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00001c30: 2020 2020 2020 2020 2020 2020 696e 636c              incl
-00001c40: 7564 655f 6d65 7461 6461 7461 3d46 616c  ude_metadata=Fal
-00001c50: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00001c60: 2020 2020 2020 2020 2020 2020 6164 635f              adc_
-00001c70: 6e61 6d65 3d27 6164 6331 2729 3a0a 2020  name='adc1'):.  
-00001c80: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00001c90: 2020 4675 6e63 7469 6f6e 2074 6f20 7265    Function to re
-00001ca0: 6164 206e 6578 7420 6576 656e 7420 616e  ad next event an
-00001cb0: 6420 696e 6372 656d 656e 7420 6576 656e  d increment even
-00001cc0: 740a 2020 2020 2020 2020 6e75 6d62 6572  t.        number
-00001cd0: 2063 6f75 6e74 6572 2e20 5265 7175 6972   counter. Requir
-00001ce0: 6520 6669 7273 7420 746f 2073 6574 2066  e first to set f
-00001cf0: 696c 6520 6c69 7374 0a20 2020 2020 2020  ile list.       
-00001d00: 2028 7365 6520 2273 6574 5f66 696c 6573   (see "set_files
-00001d10: 2220 6675 6e63 7469 6f6e 290a 0a20 2020  " function)..   
-00001d20: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00001d30: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00001d40: 2d2d 0a20 2020 2020 2020 200a 2020 2020  --.        .    
-00001d50: 2020 2020 6465 7465 6374 6f72 5f63 6861      detector_cha
-00001d60: 6e73 203a 2073 7472 206f 7220 6c69 7374  ns : str or list
-00001d70: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00001d80: 2020 2020 2064 6574 6563 746f 722f 6368       detector/ch
-00001d90: 616e 6e65 6c20 6e61 6d65 206f 7220 6c69  annel name or li
-00001da0: 7374 206f 6620 6465 7465 6374 6f72 732f  st of detectors/
-00001db0: 6368 616e 6e65 6c73 0a20 2020 2020 2020  channels.       
-00001dc0: 2020 2069 6620 4e6f 6e65 2c20 6765 7420     if None, get 
-00001dd0: 616c 6c20 6368 616e 6e65 6c73 2028 6465  all channels (de
-00001de0: 6661 756c 7429 0a0a 2020 2020 2020 2020  fault)..        
-00001df0: 6164 6374 6f76 6f6c 7420 3a20 626f 6f6c  adctovolt : bool
-00001e00: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00001e10: 2020 2020 2063 6f6e 7665 7274 2066 726f       convert fro
-00001e20: 6d20 4144 4320 746f 2076 6f6c 7473 0a20  m ADC to volts. 
-00001e30: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-00001e40: 3a20 4661 6c73 650a 0a20 2020 2020 2020  : False..       
-00001e50: 2061 6463 746f 616d 7020 3a20 626f 6f6c   adctoamp : bool
-00001e60: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00001e70: 2020 2020 2063 6f6e 7665 7274 2066 726f       convert fro
-00001e80: 6d20 4144 4320 746f 2063 7572 7265 6e74  m ADC to current
-00001e90: 2061 6d70 730a 2020 2020 2020 2020 2020   amps.          
-00001ea0: 6465 6661 756c 743a 2046 616c 7365 0a20  default: False. 
-00001eb0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001ec0: 2020 2020 2020 0a20 2020 2020 2020 2062        .        b
-00001ed0: 6173 656c 696e 6573 7562 3a20 626f 6f6c  aselinesub: bool
-00001ee0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00001ef0: 2020 2020 2069 6620 5472 7565 2c20 7375       if True, su
-00001f00: 6274 7261 6374 2070 7265 2d70 756c 7365  btract pre-pulse
-00001f10: 2062 6173 656c 696e 650a 2020 2020 2020   baseline.      
-00001f20: 2020 2020 6465 6661 756c 743a 2046 616c      default: Fal
-00001f30: 7365 0a0a 2020 2020 2020 2020 6261 7365  se..        base
-00001f40: 6c69 6e65 696e 6473 3a20 7475 706c 6520  lineinds: tuple 
-00001f50: 2869 6e74 2c20 696e 7429 206f 7220 6c69  (int, int) or li
-00001f60: 7374 205b 696e 742c 2069 6e74 5d0a 2020  st [int, int].  
-00001f70: 2020 2020 2020 2020 6d69 6e2f 6d61 7820          min/max 
-00001f80: 696e 6465 7820 666f 7220 2062 6173 656c  index for  basel
-00001f90: 696e 6520 6361 6c63 756c 6174 696f 6e20  ine calculation 
-00001fa0: 0a20 2020 2020 2020 2020 2064 6566 6175  .          defau
-00001fb0: 6c74 3a20 2831 302c 2030 2e38 2a70 7265  lt: (10, 0.8*pre
-00001fc0: 7472 6967 6765 7220 6c65 6e67 7468 2929  trigger length))
-00001fd0: 0a20 2020 2020 2020 2020 200a 2020 2020  .          .    
-00001fe0: 2020 2020 696e 636c 7564 655f 6d65 7461      include_meta
-00001ff0: 6461 7461 203a 2062 6f6f 6c2c 206f 7074  data : bool, opt
-00002000: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-00002010: 7265 7475 726e 2066 696c 652f 6576 656e  return file/even
-00002020: 742f 6465 7465 6374 6f72 206d 6574 6164  t/detector metad
-00002030: 6174 610a 2020 2020 2020 2020 2020 6465  ata.          de
-00002040: 6661 756c 743a 2046 616c 7365 0a0a 2020  fault: False..  
-00002050: 2020 2020 2020 6164 635f 6e61 6d65 203a        adc_name :
-00002060: 2073 7472 2c20 6f70 7469 6f6e 616c 0a20   str, optional. 
-00002070: 2020 2020 2020 2020 206e 616d 652f 4944           name/ID
-00002080: 206f 6620 7468 6520 6164 630a 2020 2020   of the adc.    
-00002090: 2020 2020 2020 6465 6661 756c 743a 2022        default: "
-000020a0: 6164 6331 220a 0a20 2020 2020 2020 2052  adc1"..        R
-000020b0: 6574 7572 6e0a 2020 2020 2020 2020 2d2d  eturn.        --
-000020c0: 2d2d 2d2d 0a20 2020 2020 2020 200a 2020  ----.        .  
-000020d0: 2020 2020 2020 6172 7261 7920 3a20 3244        array : 2D
-000020e0: 206e 756d 7079 2061 7272 6179 0a20 2020   numpy array.   
-000020f0: 2020 2020 2020 2020 7472 6163 6573 2066          traces f
-00002100: 6f72 2065 6163 6820 6368 616e 6e65 6c20  or each channel 
-00002110: 5b6e 6220 6368 616e 6e65 6c2c 206e 6220  [nb channel, nb 
-00002120: 7361 6d70 6c65 735d 0a0a 2020 2020 2020  samples]..      
-00002130: 2020 696e 666f 203a 2064 6963 740a 2020    info : dict.  
-00002140: 2020 2020 2020 2020 2066 696c 652f 6576           file/ev
-00002150: 656e 742f 6465 7465 6374 6f72 206d 6574  ent/detector met
-00002160: 6164 6174 6120 2869 6620 2269 6e63 6c75  adata (if "inclu
-00002170: 6465 5f6d 6574 6164 6174 6122 203d 2054  de_metadata" = T
-00002180: 7275 6529 0a20 2020 2020 2020 2022 2222  rue).        """
-00002190: 0a0a 2020 2020 2020 2020 696e 666f 203d  ..        info =
-000021a0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000021b0: 6172 7261 7920 3d20 6e70 2e61 7272 6179  array = np.array
-000021c0: 285b 5d29 0a20 2020 2020 2020 200a 2020  ([]).        .  
-000021d0: 2020 2020 2020 2320 6368 6563 6b20 6966        # check if
-000021e0: 2066 696c 6573 2061 7661 696c 6162 6c65   files available
-000021f0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00002200: 7365 6c66 2e5f 6669 6c65 5f6c 6973 7420  self._file_list 
-00002210: 6f72 206c 656e 2873 656c 662e 5f66 696c  or len(self._fil
-00002220: 655f 6c69 7374 293d 3d30 3a0a 2020 2020  e_list)==0:.    
-00002230: 2020 2020 2020 2020 696e 666f 5b27 7265          info['re
-00002240: 6164 5f73 7461 7475 7327 5d20 3d20 310a  ad_status'] = 1.
-00002250: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00002260: 5b27 6572 726f 725f 6d73 6727 5d20 3d20  ['error_msg'] = 
-00002270: 274e 6f20 6669 6c65 2061 7661 696c 6162  'No file availab
-00002280: 6c65 2127 0a20 2020 2020 2020 2020 2020  le!'.           
-00002290: 2072 6574 7572 6e20 6172 7261 792c 2069   return array, i
-000022a0: 6e66 6f0a 2020 2020 2020 2020 2020 0a20  nfo.          . 
-000022b0: 2020 2020 2020 2023 206f 7065 6e20 6669         # open fi
-000022c0: 6c65 2069 6620 6e65 6564 6564 0a20 2020  le if needed.   
-000022d0: 2020 2020 2069 6620 7365 6c66 2e5f 6375       if self._cu
-000022e0: 7272 656e 745f 6669 6c65 2069 7320 4e6f  rrent_file is No
-000022f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002300: 7365 6c66 2e5f 6f70 656e 5f66 696c 6528  self._open_file(
-00002310: 7365 6c66 2e5f 6669 6c65 5f6c 6973 745b  self._file_list[
-00002320: 7365 6c66 2e5f 6669 6c65 5f63 6f75 6e74  self._file_count
-00002330: 6572 5d29 0a0a 2020 2020 2020 2020 2020  er])..          
-00002340: 2020 0a20 2020 2020 2020 2023 2063 6865    .        # che
-00002350: 636b 2069 6620 7468 6572 6520 6172 6520  ck if there are 
-00002360: 6d6f 7265 2065 7665 6e74 730a 2020 2020  more events.    
-00002370: 2020 2020 6966 2073 656c 662e 5f63 7572      if self._cur
-00002380: 7265 6e74 5f66 696c 655f 6576 656e 745f  rent_file_event_
-00002390: 636f 756e 7465 723e 3d73 656c 662e 5f63  counter>=self._c
-000023a0: 7572 7265 6e74 5f66 696c 655f 6e62 5f65  urrent_file_nb_e
-000023b0: 7665 6e74 733a 0a0a 2020 2020 2020 2020  vents:..        
-000023c0: 2020 2020 2320 636c 6f73 6520 0a20 2020      # close .   
-000023d0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-000023e0: 6c6f 7365 5f66 696c 6528 290a 2020 2020  lose_file().    
-000023f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002400: 2020 2020 2023 2063 6865 636b 2069 6620       # check if 
-00002410: 7468 6572 6520 6172 6520 6d6f 7265 2066  there are more f
-00002420: 696c 6573 0a20 2020 2020 2020 2020 2020  iles.           
-00002430: 2069 6620 2073 656c 662e 5f66 696c 655f   if  self._file_
-00002440: 636f 756e 7465 723e 3d6c 656e 2873 656c  counter>=len(sel
-00002450: 662e 5f66 696c 655f 6c69 7374 293a 0a20  f._file_list):. 
-00002460: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002470: 6e66 6f5b 2772 6561 645f 7374 6174 7573  nfo['read_status
-00002480: 275d 203d 2031 0a20 2020 2020 2020 2020  '] = 1.         
-00002490: 2020 2020 2020 2069 6e66 6f5b 2765 7272         info['err
-000024a0: 6f72 5f6d 7367 275d 203d 2027 4e6f 206d  or_msg'] = 'No m
-000024b0: 6f72 6520 6669 6c65 7320 6176 6169 6c61  ore files availa
-000024c0: 626c 6527 0a20 2020 2020 2020 2020 2020  ble'.           
-000024d0: 2020 2020 2072 6574 7572 6e20 6172 7261       return arra
-000024e0: 792c 2069 6e66 6f0a 2020 2020 2020 2020  y, info.        
-000024f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00002500: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00002510: 6f70 656e 5f66 696c 6528 7365 6c66 2e5f  open_file(self._
-00002520: 6669 6c65 5f6c 6973 745b 7365 6c66 2e5f  file_list[self._
-00002530: 6669 6c65 5f63 6f75 6e74 6572 5d29 0a0a  file_counter])..
-00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 0a20 2020 2020 2020 2020 2020 200a 0a20  .            .. 
-00002560: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
-00002570: 6620 6669 6c65 206e 6f74 2079 6574 206f  f file not yet o
-00002580: 7065 6e20 2873 686f 756c 646e 2774 2068  pen (shouldn't h
-00002590: 6170 7065 6e29 0a20 2020 2020 2020 2069  appen).        i
-000025a0: 6620 7365 6c66 2e5f 6375 7272 656e 745f  f self._current_
-000025b0: 6669 6c65 2069 7320 4e6f 6e65 3a0a 2020  file is None:.  
-000025c0: 2020 2020 2020 2020 2020 696e 666f 5b27            info['
-000025d0: 7265 6164 5f73 7461 7475 7327 5d20 3d20  read_status'] = 
-000025e0: 310a 2020 2020 2020 2020 2020 2020 696e  1.            in
-000025f0: 666f 5b27 6572 726f 725f 6d73 6727 5d20  fo['error_msg'] 
-00002600: 3d20 2750 726f 626c 656d 2072 6561 6469  = 'Problem readi
-00002610: 6e67 206e 6578 7420 6576 656e 742e 2046  ng next event. F
-00002620: 696c 6520 636c 6f73 6564 2127 0a20 2020  ile closed!'.   
-00002630: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002640: 6172 7261 792c 2069 6e66 6f0a 2020 2020  array, info.    
-00002650: 2020 2020 200a 0a20 2020 2020 2020 2023       ..        #
-00002660: 206c 6f61 6420 6461 7461 0a20 2020 2020   load data.     
-00002670: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-00002680: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
-00002690: 7465 722b 3d31 0a20 2020 2020 2020 2061  ter+=1.        a
-000026a0: 7272 6179 2c20 696e 666f 203d 2073 656c  rray, info = sel
-000026b0: 662e 5f6c 6f61 645f 6576 656e 7428 7365  f._load_event(se
-000026c0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-000026d0: 5f65 7665 6e74 5f63 6f75 6e74 6572 2c0a  _event_counter,.
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002700: 2020 2020 2020 2061 6463 5f6e 616d 653d         adc_name=
-00002710: 6164 635f 6e61 6d65 2c0a 2020 2020 2020  adc_name,.      
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 2064 6574 6563 746f 725f 6368 616e 733d   detector_chans=
-00002750: 6465 7465 6374 6f72 5f63 6861 6e73 2c0a  detector_chans,.
-00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000620: 726d 6174 2127 290a 2020 2020 0a20 2020  rmat!').    .   
+00000630: 2023 2065 7874 7261 6374 2073 6572 6965   # extract serie
+00000640: 7320 6e75 6d0a 2020 2020 7365 7269 6573  s num.    series
+00000650: 5f6e 756d 203d 2073 6572 6965 735f 7370  _num = series_sp
+00000660: 6c69 745b 696e 6465 785f 6661 6369 6c69  lit[index_facili
+00000670: 7479 5d5b 313a 5d20 2b20 7365 7269 6573  ty][1:] + series
+00000680: 5f73 706c 6974 5b69 6e64 6578 5f66 6163  _split[index_fac
+00000690: 696c 6974 792b 315d 5b31 3a5d 0a20 2020  ility+1][1:].   
+000006a0: 2073 6572 6965 735f 6e75 6d20 2b3d 2073   series_num += s
+000006b0: 6572 6965 735f 7370 6c69 745b 696e 6465  eries_split[inde
+000006c0: 785f 6661 6369 6c69 7479 2b32 5d5b 313a  x_facility+2][1:
+000006d0: 5d0a 2020 2020 7365 7269 6573 5f6e 756d  ].    series_num
+000006e0: 203d 206e 702e 7569 6e74 3634 2866 6c6f   = np.uint64(flo
+000006f0: 6174 2873 6572 6965 735f 6e75 6d29 290a  at(series_num)).
+00000700: 0a20 2020 2072 6574 7572 6e20 7365 7269  .    return seri
+00000710: 6573 5f6e 756d 0a0a 0a64 6566 2065 7874  es_num...def ext
+00000720: 7261 6374 5f73 6572 6965 735f 6e61 6d65  ract_series_name
+00000730: 2873 6572 6965 735f 6e75 6d29 3a0a 2020  (series_num):.  
+00000740: 2020 2222 220a 2020 2020 4578 7472 6163    """.    Extrac
+00000750: 7420 7365 7269 6573 206e 616d 6520 6672  t series name fr
+00000760: 6f6d 2073 6572 6965 7320 6e75 6d62 6572  om series number
+00000770: 0a0a 2020 2020 466f 726d 6174 3a0a 2020  ..    Format:.  
+00000780: 2020 5365 7269 6573 206e 616d 653a 2020    Series name:  
+00000790: 4978 5f44 7979 7979 6d6d 6464 5f54 6868  Ix_Dyyyymmdd_Thh
+000007a0: 6d6d 7373 0a20 2020 2053 6572 6965 7320  mmss.    Series 
+000007b0: 6e75 6d3a 2078 7979 7979 6d6d 6464 6868  num: xyyyymmddhh
+000007c0: 6d6d 7373 200a 2020 0a20 2020 2050 6172  mmss .  .    Par
+000007d0: 616d 6574 6572 733a 0a20 2020 202d 2d2d  ameters:.    ---
+000007e0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7365 7269  -------.    seri
+000007f0: 6573 5f6e 756d 3a20 696e 740a 2020 2020  es_num: int.    
+00000800: 2073 6572 6965 7320 6e75 6d62 6572 0a0a   series number..
+00000810: 2020 2020 5265 7475 726e 0a20 2020 202d      Return.    -
+00000820: 2d2d 2d2d 2d0a 2020 2020 7365 7269 6573  -----.    series
+00000830: 5f6e 616d 6520 3a20 7374 720a 0a20 2020  _name : str..   
+00000840: 2022 2222 0a0a 2020 2020 7365 7269 6573   """..    series
+00000850: 5f6e 756d 5f73 7472 203d 2073 7472 2873  _num_str = str(s
+00000860: 6572 6965 735f 6e75 6d29 0a20 2020 2073  eries_num).    s
+00000870: 6572 6965 735f 7469 6d65 203d 2027 5427  eries_time = 'T'
+00000880: 202b 2073 6572 6965 735f 6e75 6d5f 7374   + series_num_st
+00000890: 725b 2d36 3a5d 0a20 2020 2073 6572 6965  r[-6:].    serie
+000008a0: 735f 6461 7920 3d20 2744 2720 2b20 7365  s_day = 'D' + se
+000008b0: 7269 6573 5f6e 756d 5f73 7472 5b2d 3134  ries_num_str[-14
+000008c0: 3a2d 365d 0a20 2020 2073 6572 6965 735f  :-6].    series_
+000008d0: 696e 7374 203d 2027 4927 202b 2073 6572  inst = 'I' + ser
+000008e0: 6965 735f 6e75 6d5f 7374 725b 3a2d 3134  ies_num_str[:-14
+000008f0: 5d0a 2020 2020 7365 7269 6573 5f6e 616d  ].    series_nam
+00000900: 6520 3d20 7365 7269 6573 5f69 6e73 7420  e = series_inst 
+00000910: 2b20 275f 2720 2b20 2073 6572 6965 735f  + '_' +  series_
+00000920: 6461 7920 2b20 275f 2720 2b20 7365 7269  day + '_' + seri
+00000930: 6573 5f74 696d 650a 0a20 2020 2072 6574  es_time..    ret
+00000940: 7572 6e20 7365 7269 6573 5f6e 616d 650a  urn series_name.
+00000950: 2020 2020 0a20 2020 200a 6465 6620 6578      .    .def ex
+00000960: 7472 6163 745f 6475 6d70 5f6e 756d 2866  tract_dump_num(f
+00000970: 696c 655f 6e61 6d65 293a 0a20 2020 2022  ile_name):.    "
+00000980: 2222 0a20 2020 2045 7874 7261 6374 2064  "".    Extract d
+00000990: 756d 7020 6e75 6d62 6572 2066 6f72 2066  ump number for f
+000009a0: 696c 6520 6e61 6d65 2e20 5468 6973 2066  ile name. This f
+000009b0: 756e 6374 696f 6e0a 2020 2020 7368 6f75  unction.    shou
+000009c0: 6c64 206f 6e6c 7920 6265 2075 7365 6420  ld only be used 
+000009d0: 6966 2022 6475 6d70 5f6e 756d 2220 6973  if "dump_num" is
+000009e0: 206e 6f74 2073 746f 7265 6420 696e 2072   not stored in r
+000009f0: 6177 200a 2020 2020 6461 7461 2e0a 0a20  aw .    data... 
+00000a00: 2020 2046 696c 6520 6e61 6d65 2066 6f72     File name for
+00000a10: 6d61 743a 2073 6572 6965 735f 6e61 6d65  mat: series_name
+00000a20: 5f46 7878 7878 2e68 6466 350a 2020 2020  _Fxxxx.hdf5.    
+00000a30: 2020 2020 0a20 2020 2052 6574 7572 6e3a      .    Return:
+00000a40: 0a0a 2020 2020 6475 6d70 5f6e 756d 3a20  ..    dump_num: 
+00000a50: 696e 7420 0a20 2020 2028 7265 7475 726e  int .    (return
+00000a60: 204e 6f6e 6520 6966 206e 6f74 2064 756d   None if not dum
+00000a70: 7020 6e75 6d62 6572 2066 6f75 6e64 290a  p number found).
+00000a80: 2020 2020 2222 220a 0a20 2020 2023 2072      """..    # r
+00000a90: 656d 6f76 6520 7061 7468 0a20 2020 2069  emove path.    i
+00000aa0: 6620 6669 6c65 5f6e 616d 652e 6669 6e64  f file_name.find
+00000ab0: 2827 2f27 2921 3d2d 313a 0a20 2020 2020  ('/')!=-1:.     
+00000ac0: 2020 2066 696c 655f 6e61 6d65 203d 2066     file_name = f
+00000ad0: 696c 655f 6e61 6d65 2e73 706c 6974 2827  ile_name.split('
+00000ae0: 2f27 295b 2d31 5d0a 0a0a 2020 2020 2320  /')[-1]...    # 
+00000af0: 6669 6e64 2020 6475 6d70 2073 7472 696e  find  dump strin
+00000b00: 670a 2020 2020 6475 6d70 5f6e 756d 203d  g.    dump_num =
+00000b10: 204e 6f6e 650a 2020 2020 706f 7320 3d20   None.    pos = 
+00000b20: 6669 6c65 5f6e 616d 652e 6669 6e64 2827  file_name.find('
+00000b30: 5f46 2729 0a20 2020 2069 6620 706f 733e  _F').    if pos>
+00000b40: 303a 0a20 2020 2020 2020 2064 756d 705f  0:.        dump_
+00000b50: 6e75 6d20 3d20 696e 7428 6669 6c65 5f6e  num = int(file_n
+00000b60: 616d 655b 706f 732b 323a 706f 732b 365d  ame[pos+2:pos+6]
+00000b70: 290a 2020 2020 2020 2020 2020 0a20 2020  ).          .   
+00000b80: 2072 6574 7572 6e20 6475 6d70 5f6e 756d   return dump_num
+00000b90: 0a0a 0a0a 0a63 6c61 7373 2048 3552 6561  .....class H5Rea
+00000ba0: 6465 723a 0a20 2020 2022 2222 0a20 2020  der:.    """.   
+00000bb0: 2043 6c61 7373 2074 6f20 7265 6164 2072   Class to read r
+00000bc0: 6177 2064 6174 6120 6864 6635 2066 696c  aw data hdf5 fil
+00000bd0: 6573 2074 616b 656e 2062 7920 7079 7465  es taken by pyte
+00000be0: 7364 6171 0a20 2020 2022 2222 0a20 2020  sdaq.    """.   
+00000bf0: 200a 2020 2020 0a20 2020 2064 6566 205f   .    .    def _
+00000c00: 5f69 6e69 745f 5f28 7365 6c66 2c20 7261  _init__(self, ra
+00000c10: 6973 655f 6572 726f 7273 3d54 7275 652c  ise_errors=True,
+00000c20: 2076 6572 626f 7365 3d54 7275 6529 3a0a   verbose=True):.
+00000c30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00000c40: 2020 2020 496e 6974 6961 6c69 7a65 2048      Initialize H
+00000c50: 3552 6561 6465 720a 0a20 2020 2020 2020  5Reader..       
+00000c60: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00000c70: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00000c80: 2020 2020 2020 2072 6169 7365 5f65 7272         raise_err
+00000c90: 6f72 7320 3a20 626f 6f6c 6561 6e2c 206f  ors : boolean, o
+00000ca0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00000cb0: 2020 6966 2054 7275 6520 7261 6973 6520    if True raise 
+00000cc0: 5661 6c75 6545 7272 6f72 2028 6465 6661  ValueError (defa
+00000cd0: 756c 7429 0a20 2020 2020 2020 2020 2069  ult).          i
+00000ce0: 6620 4661 6c73 652c 2064 6973 706c 6179  f False, display
+00000cf0: 2065 7272 6f72 2061 6e64 2072 6574 7572   error and retur
+00000d00: 6e20 656d 7074 7920 636f 6e74 6169 6e65  n empty containe
+00000d10: 7273 0a0a 2020 2020 2020 2020 7665 7262  rs..        verb
+00000d20: 6f73 6520 3a20 626f 6f6c 6561 6e2c 206f  ose : boolean, o
+00000d30: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00000d40: 2020 6966 2054 7275 652c 2064 6973 706c    if True, displ
+00000d50: 6179 206d 6573 7361 6765 7320 2864 6566  ay messages (def
+00000d60: 6175 6c74 290a 2020 2020 2020 2020 0a20  ault).        . 
+00000d70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000d80: 5265 7475 726e 0a20 2020 2020 2020 202d  Return.        -
+00000d90: 2d2d 2d2d 2d0a 2020 2020 2020 2020 4e6f  -----.        No
+00000da0: 6e65 0a0a 2020 2020 2020 2020 2222 220a  ne..        """.
+00000db0: 0a20 2020 2020 2020 2073 656c 662e 5f72  .        self._r
+00000dc0: 6169 7365 5f65 7272 6f72 7320 3d20 7261  aise_errors = ra
+00000dd0: 6973 655f 6572 726f 7273 0a20 2020 2020  ise_errors.     
+00000de0: 2020 2073 656c 662e 5f76 6572 626f 7365     self._verbose
+00000df0: 203d 2076 6572 626f 7365 0a20 2020 2020   = verbose.     
+00000e00: 2020 200a 2020 2020 2020 2020 2320 6669     .        # fi
+00000e10: 6c65 2064 6963 7469 6f6e 6172 7920 7b66  le dictionary {f
+00000e20: 696c 653a 206c 6973 7420 6f66 2065 7665  ile: list of eve
+00000e30: 6e74 2064 6963 747d 0a20 2020 2020 2020  nt dict}.       
+00000e40: 2073 656c 662e 5f66 696c 655f 6469 6374   self._file_dict
+00000e50: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00000e60: 200a 2020 2020 2020 2020 2320 6375 7272   .        # curr
+00000e70: 656e 7420 6669 6c65 2064 6174 610a 2020  ent file data.  
+00000e80: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
+00000e90: 656e 745f 6669 6c65 203d 204e 6f6e 650a  ent_file = None.
+00000ea0: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
+00000eb0: 7272 656e 745f 6669 6c65 5f6e 616d 6520  rrent_file_name 
+00000ec0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00000ed0: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+00000ee0: 655f 6d65 7461 6461 7461 203d 204e 6f6e  e_metadata = Non
+00000ef0: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00000f00: 6375 7272 656e 745f 6669 6c65 5f6e 625f  current_file_nb_
+00000f10: 6576 656e 7473 203d 2030 0a20 2020 2020  events = 0.     
+00000f20: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
+00000f30: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
+00000f40: 7465 7220 3d20 300a 2020 2020 2020 2020  ter = 0.        
+00000f50: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+00000f60: 6c65 5f65 7665 6e74 5f6c 6973 7420 3d20  le_event_list = 
+00000f70: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00000f80: 2020 0a20 2020 2020 2020 2023 2067 6c6f    .        # glo
+00000f90: 6261 6c20 7472 6967 6765 7220 636f 756e  bal trigger coun
+00000fa0: 7465 7220 2873 616d 6520 6173 2022 6576  ter (same as "ev
+00000fb0: 656e 7422 0a20 2020 2020 2020 2023 2077  ent".        # w
+00000fc0: 6865 6e20 656e 7469 7265 2074 7261 6365  hen entire trace
+00000fd0: 2075 7365 6429 0a20 2020 2020 2020 2073   used).        s
+00000fe0: 656c 662e 5f67 6c6f 6261 6c5f 6576 656e  elf._global_even
+00000ff0: 7473 5f63 6f75 6e74 6572 203d 2030 0a20  ts_counter = 0. 
+00001000: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001010: 2023 2067 6c6f 6261 6c20 6669 6c65 2063   # global file c
+00001020: 6f75 6e74 6572 0a20 2020 2020 2020 2073  ounter.        s
+00001030: 656c 662e 5f66 696c 655f 636f 756e 7465  elf._file_counte
+00001040: 7220 3d20 300a 0a20 2020 2020 2020 200a  r = 0..        .
+00001050: 2020 2020 6465 6620 7365 745f 6669 6c65      def set_file
+00001060: 7328 7365 6c66 2c20 6669 6c65 7061 7468  s(self, filepath
+00001070: 732c 2073 6572 6965 733d 4e6f 6e65 2c20  s, series=None, 
+00001080: 6576 656e 745f 6c69 7374 3d4e 6f6e 6529  event_list=None)
+00001090: 3a0a 2020 2020 2020 2020 2222 220a 0a20  :.        """.. 
+000010a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000010b0: 2020 2023 2063 6c65 6172 0a20 2020 2020     # clear.     
+000010c0: 2020 2073 656c 662e 636c 6561 7228 290a     self.clear().
+000010d0: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
+000010e0: 6c65 5f64 6963 7420 3d20 6469 6374 2829  le_dict = dict()
+000010f0: 0a20 2020 2020 200a 2020 2020 2020 2020  .      .        
+00001100: 2320 6669 6e64 2066 696c 6573 0a20 2020  # find files.   
+00001110: 2020 2020 2073 656c 662e 5f66 696c 655f       self._file_
+00001120: 6469 6374 203d 2073 656c 662e 5f67 6574  dict = self._get
+00001130: 5f66 696c 655f 6469 6374 280a 2020 2020  _file_dict(.    
+00001140: 2020 2020 2020 2020 6669 6c65 7061 7468          filepath
+00001150: 732c 2073 6572 6965 733d 7365 7269 6573  s, series=series
+00001160: 2c0a 2020 2020 2020 2020 2020 2020 6576  ,.            ev
+00001170: 656e 745f 6c69 7374 3d65 7665 6e74 5f6c  ent_list=event_l
+00001180: 6973 740a 2020 2020 2020 2020 290a 2020  ist.        ).  
+00001190: 2020 2020 2020 2020 2020 200a 2020 0a20             .  . 
+000011a0: 2020 2064 6566 2063 6c6f 7365 2873 656c     def close(sel
+000011b0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+000011c0: 2020 2020 2020 2020 436c 6f73 6520 6375          Close cu
+000011d0: 7272 656e 7420 6669 6c65 2061 6e64 2069  rrent file and i
+000011e0: 6e69 7469 616c 697a 6520 0a20 2020 2020  nitialize .     
+000011f0: 2020 2066 696c 6520 6e61 6d65 2070 6172     file name par
+00001200: 616d 7465 7273 0a0a 2020 2020 2020 2020  amters..        
+00001210: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00001220: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00001230: 2020 2020 2020 4e6f 6e65 0a0a 2020 2020        None..    
+00001240: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
+00001250: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
+00001260: 2020 4e6f 6e65 0a20 2020 2020 2020 2022    None.        "
+00001270: 2222 0a20 2020 2020 2020 200a 2020 2020  "".        .    
+00001280: 2020 2020 7365 6c66 2e5f 636c 6f73 655f      self._close_
+00001290: 6669 6c65 2829 0a0a 0a20 2020 2020 2020  file()...       
+000012a0: 200a 2020 2020 6465 6620 636c 6561 7228   .    def clear(
+000012b0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000012c0: 2222 0a20 2020 2020 2020 2043 6c6f 7365  "".        Close
+000012d0: 2063 7572 7265 6e74 2066 696c 6520 616e   current file an
+000012e0: 6420 696e 6974 6961 6c69 7a65 200a 2020  d initialize .  
+000012f0: 2020 2020 2020 6669 6c65 206e 616d 6520        file name 
+00001300: 7061 7261 6d65 7465 7273 2061 6e64 2063  parameters and c
+00001310: 6f75 6e74 6572 730a 0a20 2020 2020 2020  ounters..       
+00001320: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00001330: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00001340: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
+00001350: 2020 2020 2052 6574 7572 6e0a 2020 2020       Return.    
+00001360: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2020      ------.     
+00001370: 2020 204e 6f6e 650a 0a20 2020 2020 2020     None..       
+00001380: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
+00001390: 636c 6f73 6520 6375 7272 656e 7420 6669  close current fi
+000013a0: 6c65 0a20 2020 2020 2020 2073 656c 662e  le.        self.
+000013b0: 5f63 6c6f 7365 5f66 696c 6528 290a 0a20  _close_file().. 
+000013c0: 2020 2020 2020 2023 2069 6e69 7469 616c         # initial
+000013d0: 697a 6520 0a20 2020 2020 2020 2073 656c  ize .        sel
+000013e0: 662e 5f63 7572 7265 6e74 5f66 696c 6520  f._current_file 
+000013f0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00001400: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+00001410: 655f 6e61 6d65 203d 204e 6f6e 650a 2020  e_name = None.  
+00001420: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
+00001430: 656e 745f 6669 6c65 5f6d 6574 6164 6174  ent_file_metadat
+00001440: 6120 3d20 4e6f 6e65 0a20 2020 2020 2020  a = None.       
+00001450: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
+00001460: 696c 655f 6e62 5f65 7665 6e74 7320 3d20  ile_nb_events = 
+00001470: 300a 2020 2020 2020 2020 7365 6c66 2e5f  0.        self._
+00001480: 6375 7272 656e 745f 6669 6c65 5f65 7665  current_file_eve
+00001490: 6e74 5f63 6f75 6e74 6572 203d 2030 0a20  nt_counter = 0. 
+000014a0: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
+000014b0: 7265 6e74 5f66 696c 655f 6576 656e 745f  rent_file_event_
+000014c0: 6c69 7374 203d 204e 6f6e 650a 2020 2020  list = None.    
+000014d0: 2020 2020 7365 6c66 2e5f 6669 6c65 5f63      self._file_c
+000014e0: 6f75 6e74 6572 203d 2030 0a20 2020 2020  ounter = 0.     
+000014f0: 2020 2073 656c 662e 5f67 6c6f 6261 6c5f     self._global_
+00001500: 6576 656e 7473 5f63 6f75 6e74 6572 203d  events_counter =
+00001510: 2030 0a0a 0a0a 2020 2020 6465 6620 7265   0....    def re
+00001520: 7769 6e64 2873 656c 6629 3a0a 2020 2020  wind(self):.    
+00001530: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00001540: 5265 7769 6e64 2074 6f20 6265 6769 6e6e  Rewind to beginn
+00001550: 696e 6720 6f66 2066 696c 6528 7329 0a20  ing of file(s). 
+00001560: 2020 2020 2020 2072 656f 7065 6e2e 2e2e         reopen...
+00001570: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00001580: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00001590: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+000015a0: 204e 6f6e 650a 0a20 2020 2020 2020 2052   None..        R
+000015b0: 6574 7572 6e0a 2020 2020 2020 2020 2d2d  eturn.        --
+000015c0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+000015d0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+000015e0: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
+000015f0: 2020 2020 2020 2023 2069 6620 6d75 6c74         # if mult
+00001600: 6970 6c65 2066 696c 6573 202d 3e20 636c  iple files -> cl
+00001610: 6f73 6520 6375 7272 656e 7420 6669 6c65  ose current file
+00001620: 2074 6865 6e20 7265 6f70 656e 2066 6972   then reopen fir
+00001630: 7374 2066 696c 650a 2020 2020 2020 2020  st file.        
+00001640: 6966 206c 656e 2873 656c 662e 5f66 696c  if len(self._fil
+00001650: 655f 6469 6374 293e 313a 0a20 2020 2020  e_dict)>1:.     
+00001660: 2020 2020 2020 2073 656c 662e 5f63 6c6f         self._clo
+00001670: 7365 5f66 696c 6528 290a 2020 2020 2020  se_file().      
+00001680: 2020 2020 2020 6669 6c65 5f6c 6973 7420        file_list 
+00001690: 3d20 6c69 7374 2873 656c 662e 5f66 696c  = list(self._fil
+000016a0: 655f 6469 6374 2e6b 6579 7328 2929 0a20  e_dict.keys()). 
+000016b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000016c0: 5f6f 7065 6e5f 6669 6c65 2866 696c 655f  _open_file(file_
+000016d0: 6c69 7374 5b30 5d29 0a20 2020 200a 2020  list[0]).    .  
+000016e0: 2020 2020 2020 2320 696e 6974 6961 6c69        # initiali
+000016f0: 7a65 2063 6f75 6e74 6572 730a 2020 2020  ze counters.    
+00001700: 2020 2020 7365 6c66 2e5f 6669 6c65 5f63      self._file_c
+00001710: 6f75 6e74 6572 203d 2030 0a20 2020 2020  ounter = 0.     
+00001720: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
+00001730: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
+00001740: 7465 7220 3d20 300a 2020 2020 2020 2020  ter = 0.        
+00001750: 7365 6c66 2e5f 676c 6f62 616c 5f65 7665  self._global_eve
+00001760: 6e74 735f 636f 756e 7465 7220 3d20 300a  nts_counter = 0.
+00001770: 2020 2020 200a 0a0a 0a20 2020 2064 6566       ....    def
+00001780: 2072 6561 645f 6e65 7874 5f65 7665 6e74   read_next_event
+00001790: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000017b0: 7261 6365 5f6c 656e 6774 685f 6d73 6563  race_length_msec
+000017c0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+000017d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000017e0: 7261 6365 5f6c 656e 6774 685f 7361 6d70  race_length_samp
+000017f0: 6c65 733d 4e6f 6e65 2c0a 2020 2020 2020  les=None,.      
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 2020 7072 6574 7269 6767 6572 5f6c 656e    pretrigger_len
+00001820: 6774 685f 6d73 6563 3d4e 6f6e 652c 0a20  gth_msec=None,. 
+00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001840: 2020 2020 2020 2070 7265 7472 6967 6765         pretrigge
+00001850: 725f 6c65 6e67 7468 5f73 616d 706c 6573  r_length_samples
+00001860: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+00001870: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00001880: 6574 6563 746f 725f 6368 616e 733d 4e6f  etector_chans=No
+00001890: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+000018a0: 2020 2020 2020 2020 2020 2020 6164 6374              adct
+000018b0: 6f76 6f6c 743d 4661 6c73 652c 2061 6463  ovolt=False, adc
+000018c0: 746f 616d 703d 4661 6c73 652c 0a20 2020  toamp=False,.   
+000018d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018e0: 2020 2020 2062 6173 656c 696e 6573 7562       baselinesub
+000018f0: 3d46 616c 7365 2c20 6261 7365 6c69 6e65  =False, baseline
+00001900: 696e 6473 3d4e 6f6e 652c 0a20 2020 2020  inds=None,.     
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 2069 6e63 6c75 6465 5f6d 6574 6164     include_metad
+00001930: 6174 613d 4661 6c73 652c 0a20 2020 2020  ata=False,.     
+00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001950: 2020 2061 6463 5f6e 616d 653d 2761 6463     adc_name='adc
+00001960: 3127 293a 0a20 2020 2020 2020 2022 2222  1'):.        """
+00001970: 0a20 2020 2020 2020 2046 756e 6374 696f  .        Functio
+00001980: 6e20 746f 2072 6561 6420 6e65 7874 2065  n to read next e
+00001990: 7665 6e74 2061 6e64 2069 6e63 7265 6d65  vent and increme
+000019a0: 6e74 2065 7665 6e74 0a20 2020 2020 2020  nt event.       
+000019b0: 206e 756d 6265 7220 636f 756e 7465 722e   number counter.
+000019c0: 2052 6571 7569 7265 2066 6972 7374 2074   Require first t
+000019d0: 6f20 7365 7420 6669 6c65 206c 6973 740a  o set file list.
+000019e0: 2020 2020 2020 2020 2873 6565 2022 7365          (see "se
+000019f0: 745f 6669 6c65 7322 2066 756e 6374 696f  t_files" functio
+00001a00: 6e29 0a0a 2020 2020 2020 2020 5061 7261  n)..        Para
+00001a10: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00001a20: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00001a30: 2020 0a20 2020 2020 2020 2064 6574 6563    .        detec
+00001a40: 746f 725f 6368 616e 7320 3a20 7374 7220  tor_chans : str 
+00001a50: 6f72 206c 6973 742c 206f 7074 696f 6e61  or list, optiona
+00001a60: 6c0a 2020 2020 2020 2020 2020 6465 7465  l.          dete
+00001a70: 6374 6f72 2f63 6861 6e6e 656c 206e 616d  ctor/channel nam
+00001a80: 6520 6f72 206c 6973 7420 6f66 2064 6574  e or list of det
+00001a90: 6563 746f 7273 2f63 6861 6e6e 656c 730a  ectors/channels.
+00001aa0: 2020 2020 2020 2020 2020 6966 204e 6f6e            if Non
+00001ab0: 652c 2067 6574 2061 6c6c 2063 6861 6e6e  e, get all chann
+00001ac0: 656c 7320 2864 6566 6175 6c74 290a 0a20  els (default).. 
+00001ad0: 2020 2020 2020 2061 6463 746f 766f 6c74         adctovolt
+00001ae0: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+00001af0: 6c0a 2020 2020 2020 2020 2020 636f 6e76  l.          conv
+00001b00: 6572 7420 6672 6f6d 2041 4443 2074 6f20  ert from ADC to 
+00001b10: 766f 6c74 730a 2020 2020 2020 2020 2020  volts.          
+00001b20: 6465 6661 756c 743a 2046 616c 7365 0a0a  default: False..
+00001b30: 2020 2020 2020 2020 6164 6374 6f61 6d70          adctoamp
+00001b40: 203a 2062 6f6f 6c2c 206f 7074 696f 6e61   : bool, optiona
+00001b50: 6c0a 2020 2020 2020 2020 2020 636f 6e76  l.          conv
+00001b60: 6572 7420 6672 6f6d 2041 4443 2074 6f20  ert from ADC to 
+00001b70: 6375 7272 656e 7420 616d 7073 0a20 2020  current amps.   
+00001b80: 2020 2020 2020 2064 6566 6175 6c74 3a20         default: 
+00001b90: 4661 6c73 650a 2020 2020 2020 2020 0a20  False.        . 
+00001ba0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00001bb0: 2020 2020 2020 6261 7365 6c69 6e65 7375        baselinesu
+00001bc0: 623a 2062 6f6f 6c2c 206f 7074 696f 6e61  b: bool, optiona
+00001bd0: 6c0a 2020 2020 2020 2020 2020 6966 2054  l.          if T
+00001be0: 7275 652c 2073 7562 7472 6163 7420 7072  rue, subtract pr
+00001bf0: 652d 7075 6c73 6520 6261 7365 6c69 6e65  e-pulse baseline
+00001c00: 0a20 2020 2020 2020 2020 2064 6566 6175  .          defau
+00001c10: 6c74 3a20 4661 6c73 650a 0a20 2020 2020  lt: False..     
+00001c20: 2020 2062 6173 656c 696e 6569 6e64 733a     baselineinds:
+00001c30: 2074 7570 6c65 2028 696e 742c 2069 6e74   tuple (int, int
+00001c40: 2920 6f72 206c 6973 7420 5b69 6e74 2c20  ) or list [int, 
+00001c50: 696e 745d 0a20 2020 2020 2020 2020 206d  int].          m
+00001c60: 696e 2f6d 6178 2069 6e64 6578 2066 6f72  in/max index for
+00001c70: 2020 6261 7365 6c69 6e65 2063 616c 6375    baseline calcu
+00001c80: 6c61 7469 6f6e 200a 2020 2020 2020 2020  lation .        
+00001c90: 2020 6465 6661 756c 743a 2028 3130 2c20    default: (10, 
+00001ca0: 302e 382a 7072 6574 7269 6767 6572 206c  0.8*pretrigger l
+00001cb0: 656e 6774 6829 290a 2020 2020 2020 2020  ength)).        
+00001cc0: 2020 0a20 2020 2020 2020 2069 6e63 6c75    .        inclu
+00001cd0: 6465 5f6d 6574 6164 6174 6120 3a20 626f  de_metadata : bo
+00001ce0: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
+00001cf0: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
+00001d00: 6c65 2f65 7665 6e74 2f64 6574 6563 746f  le/event/detecto
+00001d10: 7220 6d65 7461 6461 7461 0a20 2020 2020  r metadata.     
+00001d20: 2020 2020 2064 6566 6175 6c74 3a20 4661       default: Fa
+00001d30: 6c73 650a 0a20 2020 2020 2020 2061 6463  lse..        adc
+00001d40: 5f6e 616d 6520 3a20 7374 722c 206f 7074  _name : str, opt
+00001d50: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00001d60: 6e61 6d65 2f49 4420 6f66 2074 6865 2061  name/ID of the a
+00001d70: 6463 0a20 2020 2020 2020 2020 2064 6566  dc.          def
+00001d80: 6175 6c74 3a20 2261 6463 3122 0a0a 2020  ault: "adc1"..  
+00001d90: 2020 2020 2020 5265 7475 726e 0a20 2020        Return.   
+00001da0: 2020 2020 202d 2d2d 2d2d 2d0a 2020 2020       ------.    
+00001db0: 2020 2020 0a20 2020 2020 2020 2061 7272      .        arr
+00001dc0: 6179 203a 2032 4420 6e75 6d70 7920 6172  ay : 2D numpy ar
+00001dd0: 7261 790a 2020 2020 2020 2020 2020 2074  ray.           t
+00001de0: 7261 6365 7320 666f 7220 6561 6368 2063  races for each c
+00001df0: 6861 6e6e 656c 205b 6e62 2063 6861 6e6e  hannel [nb chann
+00001e00: 656c 2c20 6e62 2073 616d 706c 6573 5d0a  el, nb samples].
+00001e10: 0a20 2020 2020 2020 2069 6e66 6f20 3a20  .        info : 
+00001e20: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
+00001e30: 6669 6c65 2f65 7665 6e74 2f64 6574 6563  file/event/detec
+00001e40: 746f 7220 6d65 7461 6461 7461 2028 6966  tor metadata (if
+00001e50: 2022 696e 636c 7564 655f 6d65 7461 6461   "include_metada
+00001e60: 7461 2220 3d20 5472 7565 290a 2020 2020  ta" = True).    
+00001e70: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00001e80: 200a 2020 2020 2020 2020 696e 666f 203d   .        info =
+00001e90: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00001ea0: 6172 7261 7920 3d20 6e70 2e61 7272 6179  array = np.array
+00001eb0: 285b 5d29 0a20 2020 2020 2020 200a 2020  ([]).        .  
+00001ec0: 2020 2020 2020 2320 6368 6563 6b20 6966        # check if
+00001ed0: 2066 696c 6573 2061 7661 696c 6162 6c65   files available
+00001ee0: 0a20 2020 2020 2020 2066 696c 655f 6c69  .        file_li
+00001ef0: 7374 203d 206c 6973 7428 7365 6c66 2e5f  st = list(self._
+00001f00: 6669 6c65 5f64 6963 742e 6b65 7973 2829  file_dict.keys()
+00001f10: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00001f20: 2066 696c 655f 6c69 7374 206f 7220 6c65   file_list or le
+00001f30: 6e28 6669 6c65 5f6c 6973 7429 3d3d 303a  n(file_list)==0:
+00001f40: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
+00001f50: 6f5b 2772 6561 645f 7374 6174 7573 275d  o['read_status']
+00001f60: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+00001f70: 2069 6e66 6f5b 2765 7272 6f72 5f6d 7367   info['error_msg
+00001f80: 275d 203d 2027 4e6f 2066 696c 6520 6176  '] = 'No file av
+00001f90: 6169 6c61 626c 6521 270a 2020 2020 2020  ailable!'.      
+00001fa0: 2020 2020 2020 7265 7475 726e 2061 7272        return arr
+00001fb0: 6179 2c20 696e 666f 0a20 2020 2020 2020  ay, info.       
+00001fc0: 2020 200a 2020 2020 2020 2020 2320 6f70     .        # op
+00001fd0: 656e 2066 696c 6520 6966 206e 6f20 6669  en file if no fi
+00001fe0: 6c65 2063 7572 7265 6e74 6c79 206f 7065  le currently ope
+00001ff0: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
+00002000: 662e 5f63 7572 7265 6e74 5f66 696c 6520  f._current_file 
+00002010: 6973 204e 6f6e 653a 0a0a 2020 2020 2020  is None:..      
+00002020: 2020 2020 2020 2320 646f 7562 6c65 2063        # double c
+00002030: 6865 636b 2077 6520 6361 6e20 6f70 656e  heck we can open
+00002040: 2066 696c 650a 2020 2020 2020 2020 2020   file.          
+00002050: 2020 6966 2073 656c 662e 5f66 696c 655f    if self._file_
+00002060: 636f 756e 7465 723e 3d6c 656e 2866 696c  counter>=len(fil
+00002070: 655f 6c69 7374 293a 0a20 2020 2020 2020  e_list):.       
+00002080: 2020 2020 2020 2020 2069 6e66 6f5b 2772           info['r
+00002090: 6561 645f 7374 6174 7573 275d 203d 2031  ead_status'] = 1
+000020a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000020b0: 2069 6e66 6f5b 2765 7272 6f72 5f6d 7367   info['error_msg
+000020c0: 275d 203d 2027 4e6f 206d 6f72 6520 6669  '] = 'No more fi
+000020d0: 6c65 7320 6176 6169 6c61 626c 6527 0a20  les available'. 
+000020e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000020f0: 6574 7572 6e20 6172 7261 792c 2069 6e66  eturn array, inf
+00002100: 6f0a 0a20 2020 2020 2020 2020 2020 2066  o..            f
+00002110: 696c 655f 6e61 6d65 203d 2066 696c 655f  ile_name = file_
+00002120: 6c69 7374 5b73 656c 662e 5f66 696c 655f  list[self._file_
+00002130: 636f 756e 7465 725d 0a20 2020 2020 2020  counter].       
+00002140: 2020 2020 2065 7665 6e74 5f6c 6973 7420       event_list 
+00002150: 3d20 7365 6c66 2e5f 6669 6c65 5f64 6963  = self._file_dic
+00002160: 745b 6669 6c65 5f6e 616d 655d 0a20 2020  t[file_name].   
+00002170: 2020 2020 2020 2020 2073 656c 662e 5f6f           self._o
+00002180: 7065 6e5f 6669 6c65 2866 696c 655f 6e61  pen_file(file_na
+00002190: 6d65 2c20 6576 656e 745f 6c69 7374 3d65  me, event_list=e
+000021a0: 7665 6e74 5f6c 6973 7429 0a0a 2020 2020  vent_list)..    
+000021b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000021c0: 2023 2043 6865 636b 2069 6620 7468 6572   # Check if ther
+000021d0: 6520 6172 6520 6d6f 7265 2065 7665 6e74  e are more event
+000021e0: 730a 2020 2020 2020 2020 2320 6966 206e  s.        # if n
+000021f0: 6f74 2c20 6f70 656e 206e 6577 2066 696c  ot, open new fil
+00002200: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00002210: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
+00002220: 6576 656e 745f 636f 756e 7465 723e 3d73  event_counter>=s
+00002230: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+00002240: 655f 6e62 5f65 7665 6e74 733a 0a0a 2020  e_nb_events:..  
+00002250: 2020 2020 2020 2020 2020 2320 636c 6f73            # clos
+00002260: 6520 0a20 2020 2020 2020 2020 2020 2073  e .            s
+00002270: 656c 662e 5f63 6c6f 7365 5f66 696c 6528  elf._close_file(
+00002280: 290a 2020 2020 2020 2020 2020 2020 0a20  ).            . 
+00002290: 2020 2020 2020 2020 2020 2023 2063 6865             # che
+000022a0: 636b 2069 6620 7468 6572 6520 6172 6520  ck if there are 
+000022b0: 6d6f 7265 2066 696c 6573 0a20 2020 2020  more files.     
+000022c0: 2020 2020 2020 2069 6620 2073 656c 662e         if  self.
+000022d0: 5f66 696c 655f 636f 756e 7465 723e 3d6c  _file_counter>=l
+000022e0: 656e 2866 696c 655f 6c69 7374 293a 0a20  en(file_list):. 
+000022f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002300: 6e66 6f5b 2772 6561 645f 7374 6174 7573  nfo['read_status
+00002310: 275d 203d 2031 0a20 2020 2020 2020 2020  '] = 1.         
+00002320: 2020 2020 2020 2069 6e66 6f5b 2765 7272         info['err
+00002330: 6f72 5f6d 7367 275d 203d 2027 4e6f 206d  or_msg'] = 'No m
+00002340: 6f72 6520 6669 6c65 7320 6176 6169 6c61  ore files availa
+00002350: 626c 6527 0a20 2020 2020 2020 2020 2020  ble'.           
+00002360: 2020 2020 2072 6574 7572 6e20 6172 7261       return arra
+00002370: 792c 2069 6e66 6f0a 2020 2020 2020 2020  y, info.        
+00002380: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00002390: 2020 2020 2020 2020 2020 6669 6c65 5f6e            file_n
+000023a0: 616d 6520 3d20 6669 6c65 5f6c 6973 745b  ame = file_list[
+000023b0: 7365 6c66 2e5f 6669 6c65 5f63 6f75 6e74  self._file_count
+000023c0: 6572 5d0a 2020 2020 2020 2020 2020 2020  er].            
+000023d0: 2020 2020 6576 656e 745f 6c69 7374 203d      event_list =
+000023e0: 2073 656c 662e 5f66 696c 655f 6469 6374   self._file_dict
+000023f0: 5b66 696c 655f 6e61 6d65 5d0a 2020 2020  [file_name].    
+00002400: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002410: 2e5f 6f70 656e 5f66 696c 6528 6669 6c65  ._open_file(file
+00002420: 5f6e 616d 652c 2065 7665 6e74 5f6c 6973  _name, event_lis
+00002430: 743d 6576 656e 745f 6c69 7374 290a 2020  t=event_list).  
+00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002450: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00002460: 6368 6563 6b20 6966 2066 696c 6520 6e6f  check if file no
+00002470: 7420 7965 7420 6f70 656e 2028 7368 6f75  t yet open (shou
+00002480: 6c64 6e27 7420 6861 7070 656e 290a 2020  ldn't happen).  
+00002490: 2020 2020 2020 6966 2073 656c 662e 5f63        if self._c
+000024a0: 7572 7265 6e74 5f66 696c 6520 6973 204e  urrent_file is N
+000024b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000024c0: 2069 6e66 6f5b 2772 6561 645f 7374 6174   info['read_stat
+000024d0: 7573 275d 203d 2031 0a20 2020 2020 2020  us'] = 1.       
+000024e0: 2020 2020 2069 6e66 6f5b 2765 7272 6f72       info['error
+000024f0: 5f6d 7367 275d 203d 2027 5072 6f62 6c65  _msg'] = 'Proble
+00002500: 6d20 7265 6164 696e 6720 6e65 7874 2065  m reading next e
+00002510: 7665 6e74 2e20 4669 6c65 2063 6c6f 7365  vent. File close
+00002520: 6421 270a 2020 2020 2020 2020 2020 2020  d!'.            
+00002530: 7265 7475 726e 2061 7272 6179 2c20 696e  return array, in
+00002540: 666f 0a20 2020 2020 2020 2020 0a20 2020  fo.         .   
+00002550: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00002560: 6765 7420 6576 656e 7420 696e 6465 7820  get event index 
+00002570: 616e 6420 7472 6967 6765 7220 696e 6465  and trigger inde
+00002580: 7820 2865 7665 6e74 5f69 6e64 6578 2073  x (event_index s
+00002590: 7461 7274 2066 726f 6d20 3129 0a20 2020  tart from 1).   
+000025a0: 2020 2020 2065 7665 6e74 5f69 6e64 6578       event_index
+000025b0: 203d 2073 656c 662e 5f63 7572 7265 6e74   = self._current
+000025c0: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
+000025d0: 7465 722b 310a 2020 2020 2020 2020 7472  ter+1.        tr
+000025e0: 6967 6765 725f 696e 6465 7820 3d20 4e6f  igger_index = No
+000025f0: 6e65 0a20 2020 2020 2020 2069 6620 7365  ne.        if se
+00002600: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+00002610: 5f65 7665 6e74 5f6c 6973 7420 6973 206e  _event_list is n
+00002620: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00002630: 2020 2020 2065 7665 6e74 5f64 6963 7420       event_dict 
+00002640: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00002650: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
+00002660: 745f 6669 6c65 5f65 7665 6e74 5f6c 6973  t_file_event_lis
+00002670: 745b 7365 6c66 2e5f 6375 7272 656e 745f  t[self._current_
+00002680: 6669 6c65 5f65 7665 6e74 5f63 6f75 6e74  file_event_count
+00002690: 6572 5d0a 2020 2020 2020 2020 2020 2020  er].            
+000026a0: 290a 2020 2020 2020 2020 2020 2020 0a20  ).            . 
+000026b0: 2020 2020 2020 2020 2020 2065 7665 6e74             event
+000026c0: 5f69 6e64 6578 203d 2069 6e74 2865 7665  _index = int(eve
+000026d0: 6e74 5f64 6963 745b 2765 7665 6e74 5f6e  nt_dict['event_n
+000026e0: 756d 6265 7227 5d25 3130 3030 3030 290a  umber']%100000).
+000026f0: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+00002700: 7472 6967 6765 725f 696e 6465 7827 2069  trigger_index' i
+00002710: 6e20 6576 656e 745f 6469 6374 2e6b 6579  n event_dict.key
+00002720: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00002730: 2020 2020 2074 7269 6767 6572 5f69 6e64       trigger_ind
+00002740: 6578 203d 2065 7665 6e74 5f64 6963 745b  ex = event_dict[
+00002750: 2774 7269 6767 6572 5f69 6e64 6578 275d  'trigger_index']
+00002760: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
 00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002780: 2020 2020 2020 2061 6463 746f 766f 6c74         adctovolt
-00002790: 3d61 6463 746f 766f 6c74 2c20 6164 6374  =adctovolt, adct
-000027a0: 6f61 6d70 3d61 6463 746f 616d 702c 0a20  oamp=adctoamp,. 
-000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 2020 2020 2020 6261 7365 6c69 6e65 7375        baselinesu
-000027e0: 623d 6261 7365 6c69 6e65 7375 622c 0a20  b=baselinesub,. 
-000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 2020 2020 2020 6261 7365 6c69 6e65 696e        baselinein
-00002820: 6473 3d62 6173 656c 696e 6569 6e64 7329  ds=baselineinds)
-00002830: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002840: 2020 2320 7265 7475 726e 0a20 2020 2020    # return.     
-00002850: 2020 2069 6620 696e 636c 7564 655f 6d65     if include_me
-00002860: 7461 6461 7461 3a0a 2020 2020 2020 2020  tadata:.        
-00002870: 2020 2020 7265 7475 726e 2061 7272 6179      return array
-00002880: 2c69 6e66 6f0a 2020 2020 2020 2020 656c  ,info.        el
-00002890: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000028a0: 7265 7475 726e 2061 7272 6179 0a20 2020  return array.   
-000028b0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-000028c0: 2020 2020 0a0a 0a20 2020 2064 6566 2072      ...    def r
-000028d0: 6561 645f 7369 6e67 6c65 5f65 7665 6e74  ead_single_event
-000028e0: 2873 656c 662c 2065 7665 6e74 5f69 6e64  (self, event_ind
-000028f0: 6578 2c20 6669 6c65 5f6e 616d 653d 4e6f  ex, file_name=No
-00002900: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00002910: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00002920: 7465 6374 6f72 5f63 6861 6e73 3d4e 6f6e  tector_chans=Non
-00002930: 652c 2061 6463 746f 766f 6c74 3d46 616c  e, adctovolt=Fal
-00002940: 7365 2c20 6164 6374 6f61 6d70 3d46 616c  se, adctoamp=Fal
-00002950: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00002960: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00002970: 7365 6c69 6e65 7375 623d 4661 6c73 652c  selinesub=False,
-00002980: 2062 6173 656c 696e 6569 6e64 733d 4e6f   baselineinds=No
-00002990: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-000029a0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-000029b0: 636c 7564 655f 6d65 7461 6461 7461 3d46  clude_metadata=F
-000029c0: 616c 7365 2c20 6164 635f 6e61 6d65 3d27  alse, adc_name='
-000029d0: 6164 6331 2729 3a0a 2020 2020 2020 2020  adc1'):.        
-000029e0: 2222 220a 2020 2020 2020 2020 5265 6164  """.        Read
-000029f0: 2061 2073 696e 676c 6520 6576 656e 7420   a single event 
-00002a00: 6672 6f6d 2061 2066 696c 6520 6261 7365  from a file base
-00002a10: 6420 0a20 2020 2020 2020 206f 6e20 696e  d .        on in
-00002a20: 6465 7820 2822 6461 7461 7365 7422 206e  dex ("dataset" n
-00002a30: 756d 6265 7229 0a0a 2020 2020 2020 2020  umber)..        
-00002a40: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00002a50: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00002a60: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2065  ------.        e
-00002a70: 7665 6e74 5f69 6e64 6578 203a 2069 6e74  vent_index : int
-00002a80: 0a20 2020 2020 2020 2020 2065 7665 6e74  .          event
-00002a90: 2028 6864 6635 2022 6461 7461 7365 7422   (hdf5 "dataset"
-00002aa0: 2920 206e 756d 6265 7220 0a20 2020 2020  )  number .     
-00002ab0: 2020 200a 2020 2020 2020 2020 6669 6c65     .        file
-00002ac0: 5f6e 616d 6520 3a20 7374 722c 206f 7074  _name : str, opt
-00002ad0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-00002ae0: 6e61 6d65 206f 6620 7468 6520 6669 6c65  name of the file
-00002af0: 0a20 2020 2020 2020 2020 2069 6620 4e6f  .          if No
-00002b00: 6e65 3a20 7573 6520 6375 7272 656e 7420  ne: use current 
-00002b10: 6669 6c65 0a20 2020 2020 2020 200a 0a20  file.        .. 
-00002b20: 2020 2020 2020 2064 6574 6563 746f 725f         detector_
-00002b30: 6368 616e 7320 3a20 7374 7220 6f72 206c  chans : str or l
-00002b40: 6973 742c 206f 7074 696f 6e61 6c0a 2020  ist, optional.  
-00002b50: 2020 2020 2020 2020 6465 7465 6374 6f72          detector
-00002b60: 2f63 6861 6e6e 656c 206e 616d 6520 6f72  /channel name or
-00002b70: 206c 6973 7420 6f66 2064 6574 6563 746f   list of detecto
-00002b80: 7273 2f63 6861 6e6e 656c 730a 2020 2020  rs/channels.    
-00002b90: 2020 2020 2020 6966 204e 6f6e 652c 2067        if None, g
-00002ba0: 6574 2061 6c6c 2063 6861 6e6e 656c 7320  et all channels 
-00002bb0: 2864 6566 6175 6c74 290a 0a20 2020 2020  (default)..     
-00002bc0: 2020 2061 6463 746f 766f 6c74 203a 2062     adctovolt : b
-00002bd0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
-00002be0: 2020 2020 2020 2020 636f 6e76 6572 7420          convert 
-00002bf0: 6672 6f6d 2041 4443 2074 6f20 766f 6c74  from ADC to volt
-00002c00: 730a 2020 2020 2020 2020 2020 6465 6661  s.          defa
-00002c10: 756c 743a 2046 616c 7365 0a0a 2020 2020  ult: False..    
-00002c20: 2020 2020 6164 6374 6f61 6d70 203a 2062      adctoamp : b
-00002c30: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
-00002c40: 2020 2020 2020 2020 636f 6e76 6572 7420          convert 
-00002c50: 6672 6f6d 2041 4443 2074 6f20 6375 7272  from ADC to curr
-00002c60: 656e 7420 616d 7073 0a20 2020 2020 2020  ent amps.       
-00002c70: 2020 2064 6566 6175 6c74 3a20 4661 6c73     default: Fals
-00002c80: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
-00002c90: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00002ca0: 2020 6261 7365 6c69 6e65 7375 623a 2062    baselinesub: b
-00002cb0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
-00002cc0: 2020 2020 2020 2020 6966 2054 7275 652c          if True,
-00002cd0: 2073 7562 7472 6163 7420 7072 652d 7075   subtract pre-pu
-00002ce0: 6c73 6520 6261 7365 6c69 6e65 0a20 2020  lse baseline.   
-00002cf0: 2020 2020 2020 2064 6566 6175 6c74 3a20         default: 
-00002d00: 4661 6c73 650a 0a20 2020 2020 2020 2062  False..        b
-00002d10: 6173 656c 696e 6569 6e64 733a 2074 7570  aselineinds: tup
-00002d20: 6c65 2028 696e 742c 2069 6e74 2920 6f72  le (int, int) or
-00002d30: 206c 6973 7420 5b69 6e74 2c20 696e 745d   list [int, int]
-00002d40: 0a20 2020 2020 2020 2020 206d 696e 2f6d  .          min/m
-00002d50: 6178 2069 6e64 6578 2066 6f72 2020 6261  ax index for  ba
-00002d60: 7365 6c69 6e65 2063 616c 6375 6c61 7469  seline calculati
-00002d70: 6f6e 200a 2020 2020 2020 2020 2020 6465  on .          de
-00002d80: 6661 756c 743a 2028 3130 2c20 302e 382a  fault: (10, 0.8*
-00002d90: 7072 6574 7269 6767 6572 206c 656e 6774  pretrigger lengt
-00002da0: 6829 290a 2020 2020 2020 2020 2020 0a20  h)).          . 
-00002db0: 2020 2020 2020 2069 6e63 6c75 6465 5f6d         include_m
-00002dc0: 6574 6164 6174 6120 3a20 626f 6f6c 2c20  etadata : bool, 
-00002dd0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-00002de0: 2020 2072 6574 7572 6e20 6669 6c65 2f65     return file/e
-00002df0: 7665 6e74 2f64 6574 6563 746f 7220 6d65  vent/detector me
-00002e00: 7461 6461 7461 0a20 2020 2020 2020 2020  tadata.         
-00002e10: 2064 6566 6175 6c74 3a20 4661 6c73 650a   default: False.
-00002e20: 0a20 2020 2020 2020 2061 6463 5f6e 616d  .        adc_nam
-00002e30: 6520 3a20 7374 722c 206f 7074 696f 6e61  e : str, optiona
-00002e40: 6c0a 2020 2020 2020 2020 2020 6e61 6d65  l.          name
-00002e50: 2f49 4420 6f66 2074 6865 2061 6463 0a20  /ID of the adc. 
-00002e60: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-00002e70: 3a20 2261 6463 3122 0a0a 2020 2020 2020  : "adc1"..      
-00002e80: 2020 5265 7475 726e 0a20 2020 2020 2020    Return.       
-00002e90: 202d 2d2d 2d2d 2d0a 2020 2020 2020 2020   ------.        
-00002ea0: 0a20 2020 2020 2020 2061 7272 6179 203a  .        array :
-00002eb0: 2032 4420 6e75 6d70 7920 6172 7261 790a   2D numpy array.
-00002ec0: 2020 2020 2020 2020 2020 2074 7261 6365             trace
-00002ed0: 7320 666f 7220 6561 6368 2063 6861 6e6e  s for each chann
-00002ee0: 656c 205b 6e62 2063 6861 6e6e 656c 2c20  el [nb channel, 
-00002ef0: 6e62 2073 616d 706c 6573 5d0a 0a20 2020  nb samples]..   
-00002f00: 2020 2020 2069 6e66 6f20 3a20 6469 6374       info : dict
-00002f10: 0a20 2020 2020 2020 2020 2020 6669 6c65  .           file
-00002f20: 2f65 7665 6e74 2f64 6574 6563 746f 7220  /event/detector 
-00002f30: 6d65 7461 6461 7461 2028 6966 2022 696e  metadata (if "in
-00002f40: 636c 7564 655f 6d65 7461 6461 7461 2220  clude_metadata" 
-00002f50: 3d20 5472 7565 290a 0a20 2020 2020 2020  = True)..       
-00002f60: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
-00002f70: 2073 6574 2066 696c 6520 6c69 7374 0a20   set file list. 
-00002f80: 2020 2020 2020 2069 6620 6669 6c65 5f6e         if file_n
-00002f90: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-00002fa0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002fb0: 662e 7365 745f 6669 6c65 7328 6669 6c65  f.set_files(file
-00002fc0: 5f6e 616d 6529 0a20 2020 2020 2020 2020  _name).         
-00002fd0: 2020 200a 2020 2020 2020 2020 2320 6f70     .        # op
-00002fe0: 656e 2066 696c 6520 6966 206e 6565 6465  en file if neede
-00002ff0: 6420 0a20 2020 2020 2020 2069 6620 7365  d .        if se
-00003000: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-00003010: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00003020: 2020 2020 2020 7365 6c66 2e5f 6f70 656e        self._open
-00003030: 5f66 696c 6528 7365 6c66 2e5f 6669 6c65  _file(self._file
-00003040: 5f6c 6973 745b 305d 290a 0a20 2020 2020  _list[0])..     
-00003050: 2020 200a 2020 2020 2020 2020 2320 6c6f     .        # lo
-00003060: 6164 2065 7665 6e74 0a20 2020 2020 2020  ad event.       
-00003070: 2061 7272 6179 2c20 696e 666f 203d 2073   array, info = s
-00003080: 656c 662e 5f6c 6f61 645f 6576 656e 7428  elf._load_event(
-00003090: 6576 656e 745f 696e 6465 782c 0a20 2020  event_index,.   
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030c0: 2020 2020 6164 635f 6e61 6d65 3d61 6463      adc_name=adc
-000030d0: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
-000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030f0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00003100: 7465 6374 6f72 5f63 6861 6e73 3d64 6574  tector_chans=det
-00003110: 6563 746f 725f 6368 616e 732c 0a20 2020  ector_chans,.   
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 2020 6164 6374 6f76 6f6c 743d 6164      adctovolt=ad
-00003150: 6374 6f76 6f6c 742c 2061 6463 746f 616d  ctovolt, adctoam
-00003160: 703d 6164 6374 6f61 6d70 2c0a 2020 2020  p=adctoamp,.    
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003190: 2020 2062 6173 656c 696e 6573 7562 3d62     baselinesub=b
-000031a0: 6173 656c 696e 6573 7562 2c0a 2020 2020  aselinesub,.    
-000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031d0: 2020 2062 6173 656c 696e 6569 6e64 733d     baselineinds=
-000031e0: 6261 7365 6c69 6e65 696e 6473 290a 2020  baselineinds).  
-000031f0: 2020 2020 2020 0a20 2020 2020 2020 2069        .        i
-00003200: 6620 696e 636c 7564 655f 6d65 7461 6461  f include_metada
-00003210: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00003220: 7265 7475 726e 2061 7272 6179 2c20 696e  return array, in
-00003230: 666f 0a20 2020 2020 2020 2065 6c73 653a  fo.        else:
-00003240: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00003250: 7572 6e20 6172 7261 790a 2020 2020 2020  urn array.      
-00003260: 2020 0a0a 2020 2020 0a20 2020 2064 6566    ..    .    def
-00003270: 2072 6561 645f 6d61 6e79 5f65 7665 6e74   read_many_event
-00003280: 7328 7365 6c66 2c20 6669 6c65 7061 7468  s(self, filepath
-00003290: 3d4e 6f6e 652c 206e 6576 656e 7473 3d30  =None, nevents=0
-000032a0: 2c20 6f75 7470 7574 5f66 6f72 6d61 743d  , output_format=
-000032b0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-000032c0: 2020 2020 2020 2020 2020 2020 6465 7465              dete
-000032d0: 6374 6f72 5f63 6861 6e73 3d4e 6f6e 652c  ctor_chans=None,
-000032e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000032f0: 2020 2020 2020 2020 2020 6576 656e 745f            event_
-00003300: 6e75 6d73 3d4e 6f6e 652c 2073 6572 6965  nums=None, serie
-00003310: 735f 6e75 6d73 3d4e 6f6e 652c 0a20 2020  s_nums=None,.   
-00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003330: 2020 2020 2020 696e 636c 7564 655f 6d65        include_me
-00003340: 7461 6461 7461 3d46 616c 7365 2c0a 2020  tadata=False,.  
-00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003360: 2020 2020 2020 2061 6463 746f 766f 6c74         adctovolt
-00003370: 3d46 616c 7365 2c20 6164 6374 6f61 6d70  =False, adctoamp
-00003380: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033a0: 2062 6173 656c 696e 6573 7562 3d46 616c   baselinesub=Fal
-000033b0: 7365 2c20 6261 7365 6c69 6e65 696e 6473  se, baselineinds
-000033c0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033e0: 6d65 6d6f 7279 5f6c 696d 6974 3d32 2c20  memory_limit=2, 
-000033f0: 6164 635f 6e61 6d65 3d27 6164 6331 2729  adc_name='adc1')
-00003400: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00003410: 2020 2020 2020 5265 6164 206d 756c 7469        Read multi
-00003420: 706c 6520 6576 656e 7473 2028 6465 6661  ple events (defa
-00003430: 756c 7420 7265 6164 2061 6c6c 2065 7665  ult read all eve
-00003440: 6e74 7329 0a20 2020 2020 2020 200a 2020  nts).        .  
-00003450: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00003460: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00003470: 2d2d 0a20 2020 2020 2020 2066 696c 6570  --.        filep
-00003480: 6174 683a 2073 7472 696e 6720 6f72 206c  ath: string or l
-00003490: 6973 7420 206f 6620 7374 7269 6e67 730a  ist  of strings.
-000034a0: 2020 2020 2020 2020 2020 2066 696c 652f             file/
-000034b0: 7061 7468 206f 7220 6c69 7374 206f 6620  path or list of 
-000034c0: 6669 6c65 732f 7061 7468 7320 2864 6566  files/paths (def
-000034d0: 6175 6c74 3a20 7573 6520 6375 7272 656e  ault: use curren
-000034e0: 7420 6669 6c65 290a 2020 2020 2020 2020  t file).        
-000034f0: 2020 0a20 2020 2020 2020 206e 6576 656e    .        neven
-00003500: 7473 3a20 696e 7465 6765 720a 2020 2020  ts: integer.    
-00003510: 2020 2020 2020 206e 756d 6265 7220 6f66         number of
-00003520: 2065 7665 6e74 7320 746f 2072 6561 6420   events to read 
-00003530: 2028 6465 6661 756c 7420 6e62 5f65 7665   (default nb_eve
-00003540: 6e74 733d 3020 2d3e 2061 6c6c 2065 7665  nts=0 -> all eve
-00003550: 6e74 7320 696e 2064 756d 7073 290a 0a20  nts in dumps).. 
-00003560: 2020 2020 2020 206f 7574 7075 745f 666f         output_fo
-00003570: 726d 6174 3a20 696e 7465 6765 720a 2020  rmat: integer.  
-00003580: 2020 2020 2020 2020 2020 313a 206c 6973            1: lis
-00003590: 7420 6f66 2032 4420 6e64 6172 7261 795b  t of 2D ndarray[
-000035a0: 6368 616e 2c20 7361 6d70 6c65 735d 0a20  chan, samples]. 
-000035b0: 2020 2020 2020 2020 2020 2032 3a20 3344             2: 3D
-000035c0: 206e 6461 7272 6179 5b65 7665 6e74 2c20   ndarray[event, 
-000035d0: 6368 616e 2c20 7361 6d70 6c65 735d 0a20  chan, samples]. 
-000035e0: 0a20 2020 2020 2020 2064 6574 6563 746f  .        detecto
-000035f0: 725f 6368 616e 733a 2073 7472 696e 672f  r_chans: string/
-00003600: 696e 7420 6f72 206c 6973 7420 6f66 2073  int or list of s
-00003610: 7472 696e 672f 696e 740a 2020 2020 2020  tring/int.      
-00003620: 2020 2020 2020 6465 7465 6374 6f72 2063        detector c
-00003630: 6861 6e6e 656c 206e 616d 6529 2873 2920  hannel name)(s) 
-00003640: 2865 7861 6d70 6c65 2027 5a31 5041 5331  (example 'Z1PAS1
-00003650: 272c 2027 5044 3227 2c20 6f72 2031 290a  ', 'PD2', or 1).
-00003660: 2020 2020 2020 2020 2020 2020 666f 6c6c              foll
-00003670: 6f77 696e 6720 666f 726d 6174 2069 6e20  owing format in 
-00003680: 7365 7475 702e 696e 6920 6669 6c65 0a20  setup.ini file. 
-00003690: 2020 2020 2020 2020 2020 2049 6620 4e6f             If No
-000036a0: 6e65 2c20 7265 6164 2061 6c6c 2063 6861  ne, read all cha
-000036b0: 6e6e 656c 7320 6176 6169 6c61 626c 6520  nnels available 
-000036c0: 0a0a 2020 2020 2020 2020 6576 656e 745f  ..        event_
-000036d0: 6e75 6d73 3a20 6c69 7374 206f 7220 6e75  nums: list or nu
-000036e0: 6d70 7920 6172 7261 790a 2020 2020 2020  mpy array.      
-000036f0: 2020 2020 2020 4576 656e 7420 6e75 6d62        Event numb
-00003700: 6572 7320 2866 6f72 6d61 743a 2064 756d  ers (format: dum
-00003710: 705f 6e75 6d20 2a20 3130 3030 3030 202b  p_num * 100000 +
-00003720: 2065 7665 6e74 5f69 6e64 6578 290a 2020   event_index).  
-00003730: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00003740: 2020 2020 2073 6572 6965 735f 6e75 6d73       series_nums
-00003750: 3a20 6c69 7374 206f 7220 6e75 6d70 7920  : list or numpy 
-00003760: 6172 7261 790a 2020 2020 2020 2020 2020  array.          
-00003770: 2020 5365 7269 6573 206e 756d 6265 7273    Series numbers
-00003780: 2028 666f 726d 6174 3a20 7879 7979 796d   (format: xyyyym
-00003790: 6d64 6468 686d 6d73 7329 0a20 2020 2020  mddhhmmss).     
-000037a0: 2020 2020 2020 2069 6620 6576 656e 745f         if event_
-000037b0: 6e75 6d73 2061 7267 756d 656e 7420 7072  nums argument pr
-000037c0: 6f76 6964 6564 2c20 7365 7269 6573 5f6e  ovided, series_n
-000037d0: 756d 7320 7368 6f75 6c64 2068 6176 6520  ums should have 
-000037e0: 7361 6d65 206c 656e 6774 6821 290a 0a20  same length!).. 
-000037f0: 2020 2020 2020 2069 6e63 6c75 6465 5f6d         include_m
-00003800: 6574 6164 6174 613a 2062 6f6f 6c20 0a20  etadata: bool . 
-00003810: 2020 2020 2020 2020 2020 2069 6e63 6c75             inclu
-00003820: 6465 2066 696c 652f 6772 6f75 702f 6461  de file/group/da
-00003830: 7461 7365 7420 6d65 7461 6461 7461 2028  taset metadata (
-00003840: 6465 6661 756c 7420 3d20 4661 6c73 6529  default = False)
-00003850: 0a0a 2020 2020 2020 2020 6164 6374 6f76  ..        adctov
-00003860: 6f6c 743a 2042 6f6f 6c0a 2020 2020 2020  olt: Bool.      
-00003870: 2020 2020 2020 436f 6e76 6572 7420 2066        Convert  f
-00003880: 726f 6d20 4144 4320 746f 2076 6f6c 7420  rom ADC to volt 
-00003890: 2844 6566 6175 6c74 3d46 616c 7365 2920  (Default=False) 
-000038a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000038b0: 2020 6164 6374 6f61 6d70 3a20 426f 6f6c    adctoamp: Bool
-000038c0: 0a20 2020 2020 2020 2020 2020 2043 6f6e  .            Con
-000038d0: 7665 7274 2020 6672 6f6d 2041 4443 2074  vert  from ADC t
-000038e0: 6f20 636c 6f73 6520 6c6f 6f70 2f46 4c4c  o close loop/FLL
-000038f0: 2061 6d70 7320 2844 6566 6175 6c74 3d46   amps (Default=F
-00003900: 616c 7365 2920 0a0a 2020 2020 2020 2020  alse) ..        
-00003910: 6261 7365 6c69 6e65 7375 623a 2042 6f6f  baselinesub: Boo
-00003920: 6c0a 2020 2020 2020 2020 2020 2020 4170  l.            Ap
-00003930: 706c 7920 6261 7365 6c69 6e65 2073 7562  ply baseline sub
-00003940: 7472 6163 7469 6f6e 0a0a 2020 2020 2020  traction..      
-00003950: 2020 6261 7365 6c69 6e65 696e 6473 3a20    baselineinds: 
-00003960: 7475 706c 6520 2869 6e74 2c20 696e 7429  tuple (int, int)
-00003970: 206f 7220 6c69 7374 205b 696e 742c 2069   or list [int, i
-00003980: 6e74 5d0a 2020 2020 2020 2020 2020 2020  nt].            
-00003990: 7374 6172 742f 7374 6f70 2062 6173 656c  start/stop basel
-000039a0: 696e 6520 6361 6c63 756c 6174 696f 6e20  ine calculation 
-000039b0: 2864 6566 6175 6c74 3a20 2831 302c 2030  (default: (10, 0
-000039c0: 2e38 2a70 7265 7472 6967 6765 7220 6c65  .8*pretrigger le
-000039d0: 6e67 7468 2929 0a20 2020 2020 2020 2020  ngth)).         
-000039e0: 200a 2020 2020 2020 2020 6d65 6d6f 7279   .        memory
-000039f0: 5f6c 696d 6974 3a20 466c 6f61 740a 2020  _limit: Float.  
-00003a00: 2020 2020 2020 2020 2020 5075 6c73 6520            Pulse 
-00003a10: 6461 7461 206d 656d 6f72 7920 6c69 6d69  data memory limi
-00003a20: 7420 696e 2047 4220 5b64 6566 6175 6c74  t in GB [default
-00003a30: 3a20 3247 425d 0a0a 2020 2020 2020 2020  : 2GB]..        
-00003a40: 6164 635f 6e61 6d65 3a20 7374 7269 6e67  adc_name: string
-00003a50: 0a20 2020 2020 2020 2020 2020 2020 2041  .              A
-00003a60: 4443 2069 6420 2864 6566 6175 6c74 3a20  DC id (default: 
-00003a70: 2761 6463 3127 290a 2020 2020 2020 2020  'adc1').        
-00003a80: 2020 0a0a 2020 2020 2020 2020 5265 7475    ..        Retu
-00003a90: 726e 0a20 2020 2020 2020 202d 2d2d 2d2d  rn.        -----
-00003aa0: 2d0a 200a 2020 2020 2020 2020 6f75 7470  -. .        outp
-00003ab0: 7574 5f64 6174 6120 3a20 6c69 7374 206f  ut_data : list o
-00003ac0: 7220 7061 6e64 6173 2064 6174 6166 7261  r pandas datafra
-00003ad0: 6d65 0a20 2020 2020 2020 2020 2020 7472  me.           tr
-00003ae0: 6163 6573 2066 6f72 2065 6163 6820 6368  aces for each ch
-00003af0: 616e 6e65 6c73 2061 6e64 2065 7665 6e74  annels and event
-00003b00: 730a 0a20 2020 2020 2020 2069 6e66 6f20  s..        info 
-00003b10: 3a20 6c69 7374 0a20 2020 2020 2020 2020  : list.         
-00003b20: 2020 6669 6c65 2f65 7665 6e74 2f64 6574    file/event/det
-00003b30: 6563 746f 7220 6d65 7461 6461 7461 200a  ector metadata .
-00003b40: 2020 2020 2020 2020 2020 2028 6966 2022             (if "
-00003b50: 696e 636c 7564 655f 6d65 7461 6461 7461  include_metadata
-00003b60: 2220 3d20 5472 7565 290a 0a0a 2020 2020  " = True)...    
-00003b70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003b80: 0a20 2020 2020 2020 2023 203d 3d3d 3d3d  .        # =====
-00003b90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003ba0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2020  ==========.     
-00003bb0: 2020 2023 2043 6865 636b 2061 7267 756d     # Check argum
-00003bc0: 656e 7473 0a20 2020 2020 2020 2023 203d  ents.        # =
-00003bd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003be0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
-00003bf0: 0a20 2020 2020 2020 2023 2073 6574 2066  .        # set f
-00003c00: 696c 6520 7061 7468 2069 6620 7072 6f76  ile path if prov
-00003c10: 6964 6564 0a20 2020 2020 2020 2069 6620  ided.        if 
-00003c20: 6669 6c65 7061 7468 2069 7320 6e6f 7420  filepath is not 
-00003c30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003c40: 2020 7365 6c66 2e73 6574 5f66 696c 6573    self.set_files
-00003c50: 2866 696c 6570 6174 6829 0a0a 2020 2020  (filepath)..    
-00003c60: 2020 2020 2320 6368 6563 6b20 0a20 2020      # check .   
-00003c70: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00003c80: 2e5f 6669 6c65 5f6c 6973 743a 0a20 2020  ._file_list:.   
-00003c90: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00003ca0: 616c 7565 4572 726f 7228 2745 5252 4f52  alueError('ERROR
-00003cb0: 3a20 4e6f 2066 696c 6573 2073 656c 6563  : No files selec
-00003cc0: 7465 6421 2729 0a0a 2020 2020 2020 2020  ted!')..        
-00003cd0: 2320 6c65 7427 7320 6b65 6570 2061 2063  # let's keep a c
-00003ce0: 6f70 7920 6f66 2063 7572 7265 6e74 2066  opy of current f
-00003cf0: 696c 6520 6c69 7374 0a20 2020 2020 2020  ile list.       
-00003d00: 2063 7572 7265 6e74 5f66 696c 655f 6c69   current_file_li
-00003d10: 7374 203d 204e 6f6e 650a 2020 2020 2020  st = None.      
-00003d20: 2020 6966 2073 656c 662e 5f66 696c 655f    if self._file_
-00003d30: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
-00003d40: 2020 6375 7272 656e 745f 6669 6c65 5f6c    current_file_l
-00003d50: 6973 7420 3d20 7365 6c66 2e5f 6669 6c65  ist = self._file
-00003d60: 5f6c 6973 742e 636f 7079 2829 0a0a 0a20  _list.copy()... 
-00003d70: 2020 2020 2020 2023 2064 6574 6563 746f         # detecto
-00003d80: 722f 6368 616e 6e65 6c0a 2020 2020 2020  r/channel.      
-00003d90: 2020 6966 2028 6465 7465 6374 6f72 5f63    if (detector_c
-00003da0: 6861 6e73 2069 7320 6e6f 7420 4e6f 6e65  hans is not None
-00003db0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00003dc0: 206e 6f74 2028 6973 696e 7374 616e 6365   not (isinstance
-00003dd0: 2864 6574 6563 746f 725f 6368 616e 732c  (detector_chans,
-00003de0: 206c 6973 7429 0a20 2020 2020 2020 2020   list).         
-00003df0: 2020 2020 2020 2020 2020 2020 6f72 2069              or i
-00003e00: 7369 6e73 7461 6e63 6528 6465 7465 6374  sinstance(detect
-00003e10: 6f72 5f63 6861 6e73 2c20 6e70 2e6e 6461  or_chans, np.nda
-00003e20: 7272 6179 2929 293a 0a20 2020 2020 2020  rray))):.       
-00003e30: 2020 2020 2064 6574 6563 746f 725f 6368       detector_ch
-00003e40: 616e 7320 3d20 5b64 6574 6563 746f 725f  ans = [detector_
-00003e50: 6368 616e 735d 0a20 2020 200a 0a20 2020  chans].    ..   
-00003e60: 2020 2020 2023 206c 6574 2773 2066 696c       # let's fil
-00003e70: 7465 7220 6669 6c65 7320 6261 7365 6420  ter files based 
-00003e80: 0a20 2020 2020 2020 2023 2073 6572 6965  .        # serie
-00003e90: 735f 6e75 6d73 2061 6e64 2065 7665 6e74  s_nums and event
-00003ea0: 5f6e 756d 7320 696e 7075 740a 2020 2020  _nums input.    
-00003eb0: 2020 2020 6669 6c74 6572 6564 5f66 696c      filtered_fil
-00003ec0: 655f 6c69 7374 203d 206c 6973 7428 290a  e_list = list().
-00003ed0: 2020 2020 2020 2020 6966 2073 6572 6965          if serie
-00003ee0: 735f 6e75 6d73 2069 7320 6e6f 7420 4e6f  s_nums is not No
-00003ef0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00003f00: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003f10: 2020 2020 2023 2063 6f6e 7665 7274 2074       # convert t
-00003f20: 6f20 6172 7261 790a 2020 2020 2020 2020  o array.        
-00003f30: 2020 2020 6966 2028 6e6f 7420 6973 696e      if (not isin
-00003f40: 7374 616e 6365 2873 6572 6965 735f 6e75  stance(series_nu
-00003f50: 6d73 2c20 6c69 7374 290a 2020 2020 2020  ms, list).      
-00003f60: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
-00003f70: 7420 6973 696e 7374 616e 6365 2873 6572  t isinstance(ser
-00003f80: 6965 735f 6e75 6d73 2c20 6e70 2e6e 6461  ies_nums, np.nda
-00003f90: 7272 6179 2929 3a0a 2020 2020 2020 2020  rray)):.        
-00003fa0: 2020 2020 2020 2020 7365 7269 6573 5f6e          series_n
-00003fb0: 756d 7320 3d20 5b73 6572 6965 735f 6e75  ums = [series_nu
-00003fc0: 6d73 5d0a 2020 2020 2020 2020 2020 2020  ms].            
-00003fd0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00003fe0: 2023 206c 6f6f 7020 7365 7269 6573 2061   # loop series a
-00003ff0: 6e64 2063 6f6e 7665 7274 2074 6f20 7365  nd convert to se
-00004000: 7269 6573 206e 616d 650a 2020 2020 2020  ries name.      
-00004010: 2020 2020 2020 2320 2861 6e64 2063 6865        # (and che
-00004020: 636b 2069 6e74 6567 6572 290a 2020 2020  ck integer).    
-00004030: 2020 2020 2020 2020 7365 7269 6573 5f6e          series_n
-00004040: 616d 6573 203d 206c 6973 7428 290a 2020  ames = list().  
-00004050: 2020 2020 2020 2020 2020 666f 7220 6973            for is
-00004060: 6572 6965 7320 696e 2072 616e 6765 286c  eries in range(l
-00004070: 656e 2873 6572 6965 735f 6e75 6d73 2929  en(series_nums))
-00004080: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004090: 2020 7365 7269 6573 203d 2069 6e74 2873    series = int(s
-000040a0: 6572 6965 735f 6e75 6d73 5b69 7365 7269  eries_nums[iseri
-000040b0: 6573 5d29 0a20 2020 2020 2020 2020 2020  es]).           
-000040c0: 2020 2020 2073 6572 6965 735f 6e61 6d65       series_name
-000040d0: 732e 6170 7065 6e64 2865 7874 7261 6374  s.append(extract
-000040e0: 5f73 6572 6965 735f 6e61 6d65 2873 6572  _series_name(ser
-000040f0: 6965 7329 290a 2020 2020 2020 2020 2020  ies)).          
-00004100: 2020 2020 2020 7365 7269 6573 5f6e 756d        series_num
-00004110: 735b 6973 6572 6965 735d 203d 2073 6572  s[iseries] = ser
-00004120: 6965 730a 0a20 2020 2020 2020 2020 2020  ies..           
-00004130: 2023 206c 6f6f 7020 6669 6c65 7320 616e   # loop files an
-00004140: 6420 6368 6563 6b20 6966 2070 6172 7420  d check if part 
-00004150: 6f66 2073 656c 6563 7465 6420 7365 7269  of selected seri
-00004160: 6573 0a20 2020 2020 2020 2020 2020 2066  es.            f
-00004170: 6f72 2066 696c 655f 6e61 6d65 2069 6e20  or file_name in 
-00004180: 7365 6c66 2e5f 6669 6c65 5f6c 6973 743a  self._file_list:
-00004190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000041a0: 2066 6f72 2073 6572 6965 7320 696e 2073   for series in s
-000041b0: 6572 6965 735f 6e61 6d65 733a 0a20 2020  eries_names:.   
-000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041d0: 2069 6620 7365 7269 6573 2069 6e20 6669   if series in fi
-000041e0: 6c65 5f6e 616d 653a 0a20 2020 2020 2020  le_name:.       
-000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004200: 2066 696c 7465 7265 645f 6669 6c65 5f6c   filtered_file_l
-00004210: 6973 742e 6170 7065 6e64 2866 696c 655f  ist.append(file_
-00004220: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
-00004230: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00004240: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
-00004250: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004260: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00004270: 6669 6c74 6572 2062 6173 6564 206f 6e20  filter based on 
-00004280: 6576 656e 7420 6e75 6d73 0a20 2020 2020  event nums.     
-00004290: 2020 2023 2028 7365 7269 6573 206e 616d     # (series nam
-000042a0: 6573 2073 686f 756c 6420 6265 2073 616d  es should be sam
-000042b0: 6520 6c65 6e67 7468 290a 0a20 2020 2020  e length)..     
-000042c0: 2020 2064 756d 705f 6e75 6d73 203d 206c     dump_nums = l
-000042d0: 6973 7428 290a 2020 2020 2020 2020 6576  ist().        ev
-000042e0: 656e 745f 696e 6469 6365 7320 3d20 6c69  ent_indices = li
-000042f0: 7374 2829 0a20 2020 2020 2020 2069 6620  st().        if 
-00004300: 6576 656e 745f 6e75 6d73 2069 7320 6e6f  event_nums is no
-00004310: 7420 4e6f 6e65 3a0a 0a20 2020 2020 2020  t None:..       
-00004320: 2020 2020 2073 6572 6965 735f 6475 6d70       series_dump
-00004330: 5f6e 616d 6573 203d 206c 6973 7428 290a  _names = list().
-00004340: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00004350: 2020 2020 2020 2020 2023 2063 6f6e 7665           # conve
-00004360: 7274 2074 6f20 6c69 7374 2069 6620 6e6f  rt to list if no
-00004370: 7420 6172 7261 792f 6c69 7374 0a20 2020  t array/list.   
-00004380: 2020 2020 2020 2020 2069 6620 286e 6f74           if (not
-00004390: 2069 7369 6e73 7461 6e63 6528 6576 656e   isinstance(even
-000043a0: 745f 6e75 6d73 2c20 6c69 7374 290a 2020  t_nums, list).  
-000043b0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-000043c0: 6420 6e6f 7420 6973 696e 7374 616e 6365  d not isinstance
-000043d0: 2865 7665 6e74 5f6e 756d 732c 6e70 2e6e  (event_nums,np.n
-000043e0: 6461 7272 6179 2929 3a0a 2020 2020 2020  darray)):.      
-000043f0: 2020 2020 2020 2020 2020 6576 656e 745f            event_
-00004400: 6e75 6d73 203d 205b 6576 656e 745f 6e75  nums = [event_nu
-00004410: 6d73 5d0a 2020 2020 2020 2020 2020 2020  ms].            
-00004420: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00004430: 2069 6620 2873 6572 6965 735f 6e75 6d73   if (series_nums
-00004440: 2069 7320 4e6f 6e65 0a20 2020 2020 2020   is None.       
-00004450: 2020 2020 2020 2020 206f 7220 6c65 6e28           or len(
-00004460: 6576 656e 745f 6e75 6d73 2921 3d6c 656e  event_nums)!=len
-00004470: 2873 6572 6965 735f 6e75 6d73 2929 3a0a  (series_nums)):.
-00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004490: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-000044a0: 2827 4552 524f 523a 2073 6572 6965 735f  ('ERROR: series_
-000044b0: 6e75 6d73 2061 6e64 2065 7665 6e74 5f6e  nums and event_n
-000044c0: 756d 7320 270a 2020 2020 2020 2020 2020  ums '.          
-000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044e0: 2020 2020 2020 202b 2027 6e65 6564 2074         + 'need t
-000044f0: 6f20 6265 2073 616d 6520 6c65 6e67 7468  o be same length
-00004500: 2127 290a 0a20 2020 2020 2020 2020 2020  !')..           
-00004510: 2073 6572 6965 735f 6475 6d70 5f6e 616d   series_dump_nam
-00004520: 6573 203d 206c 6973 7428 290a 2020 2020  es = list().    
-00004530: 2020 2020 2020 2020 666f 7220 6965 7665          for ieve
-00004540: 6e74 2069 6e20 7261 6e67 6528 6c65 6e28  nt in range(len(
-00004550: 6576 656e 745f 6e75 6d73 2929 3a0a 2020  event_nums)):.  
-00004560: 2020 2020 2020 2020 2020 2020 2020 6576                ev
-00004570: 656e 745f 6e75 6d73 5b69 6576 656e 745d  ent_nums[ievent]
-00004580: 203d 2069 6e74 2865 7665 6e74 5f6e 756d   = int(event_num
-00004590: 735b 6965 7665 6e74 5d29 0a20 2020 2020  s[ievent]).     
-000045a0: 2020 2020 2020 2020 2020 2064 756d 705f             dump_
-000045b0: 6e75 6d20 3d20 696e 7428 6576 656e 745f  num = int(event_
-000045c0: 6e75 6d73 5b69 6576 656e 745d 2f31 3030  nums[ievent]/100
-000045d0: 3030 3029 0a20 2020 2020 2020 2020 2020  000).           
-000045e0: 2020 2020 2065 7665 6e74 5f69 6e64 6578       event_index
-000045f0: 203d 2069 6e74 2865 7665 6e74 5f6e 756d   = int(event_num
-00004600: 735b 6965 7665 6e74 5d25 3130 3030 3030  s[ievent]%100000
-00004610: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004620: 2020 6966 2064 756d 705f 6e75 6d20 3d3d    if dump_num ==
-00004630: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00004640: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00004650: 6c75 6545 7272 6f72 2827 4552 524f 523a  lueError('ERROR:
-00004660: 2055 6e65 7870 6563 7465 6420 6576 656e   Unexpected even
-00004670: 7420 6e75 6d62 6572 2066 6f72 6d61 7421  t number format!
-00004680: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046a0: 2020 2020 2020 202b 2027 2052 6571 7569         + ' Requi
-000046b0: 7265 6420 666f 726d 6174 203d 2027 0a20  red format = '. 
-000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046e0: 2020 2020 2b20 2722 6475 6d70 5f6e 756d      + '"dump_num
-000046f0: 2a31 3030 3030 302b 6576 656e 745f 696e  *100000+event_in
-00004700: 6465 7822 2729 0a20 2020 2020 2020 2020  dex"').         
-00004710: 2020 2020 2020 2064 756d 705f 6e75 6d73         dump_nums
-00004720: 2e61 7070 656e 6428 6475 6d70 5f6e 756d  .append(dump_num
-00004730: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004740: 2020 6576 656e 745f 696e 6469 6365 732e    event_indices.
-00004750: 6170 7065 6e64 2865 7665 6e74 5f69 6e64  append(event_ind
-00004760: 6578 290a 2020 2020 2020 2020 2020 2020  ex).            
-00004770: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00004780: 2020 2020 2023 2064 756d 7020 7374 720a       # dump str.
+00002780: 2020 200a 2020 2020 2020 2020 6172 7261     .        arra
+00002790: 792c 2069 6e66 6f20 3d20 7365 6c66 2e5f  y, info = self._
+000027a0: 6c6f 6164 5f65 7665 6e74 280a 2020 2020  load_event(.    
+000027b0: 2020 2020 2020 2020 6576 656e 745f 696e          event_in
+000027c0: 6465 782c 0a20 2020 2020 2020 2020 2020  dex,.           
+000027d0: 2074 7269 6767 6572 5f69 6e64 6578 3d74   trigger_index=t
+000027e0: 7269 6767 6572 5f69 6e64 6578 2c0a 2020  rigger_index,.  
+000027f0: 2020 2020 2020 2020 2020 7472 6163 655f            trace_
+00002800: 6c65 6e67 7468 5f6d 7365 633d 7472 6163  length_msec=trac
+00002810: 655f 6c65 6e67 7468 5f6d 7365 632c 0a20  e_length_msec,. 
+00002820: 2020 2020 2020 2020 2020 2074 7261 6365             trace
+00002830: 5f6c 656e 6774 685f 7361 6d70 6c65 733d  _length_samples=
+00002840: 7472 6163 655f 6c65 6e67 7468 5f73 616d  trace_length_sam
+00002850: 706c 6573 2c0a 2020 2020 2020 2020 2020  ples,.          
+00002860: 2020 7072 6574 7269 6767 6572 5f6c 656e    pretrigger_len
+00002870: 6774 685f 6d73 6563 3d70 7265 7472 6967  gth_msec=pretrig
+00002880: 6765 725f 6c65 6e67 7468 5f6d 7365 632c  ger_length_msec,
+00002890: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
+000028a0: 7472 6967 6765 725f 6c65 6e67 7468 5f73  trigger_length_s
+000028b0: 616d 706c 6573 3d70 7265 7472 6967 6765  amples=pretrigge
+000028c0: 725f 6c65 6e67 7468 5f73 616d 706c 6573  r_length_samples
+000028d0: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
+000028e0: 7465 6374 6f72 5f63 6861 6e73 3d64 6574  tector_chans=det
+000028f0: 6563 746f 725f 6368 616e 732c 0a20 2020  ector_chans,.   
+00002900: 2020 2020 2020 2020 2061 6463 746f 766f           adctovo
+00002910: 6c74 3d61 6463 746f 766f 6c74 2c20 6164  lt=adctovolt, ad
+00002920: 6374 6f61 6d70 3d61 6463 746f 616d 702c  ctoamp=adctoamp,
+00002930: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+00002940: 656c 696e 6573 7562 3d62 6173 656c 696e  elinesub=baselin
+00002950: 6573 7562 2c0a 2020 2020 2020 2020 2020  esub,.          
+00002960: 2020 6261 7365 6c69 6e65 696e 6473 3d62    baselineinds=b
+00002970: 6173 656c 696e 6569 6e64 732c 0a20 2020  aselineinds,.   
+00002980: 2020 2020 2020 2020 2061 6463 5f6e 616d           adc_nam
+00002990: 653d 6164 635f 6e61 6d65 290a 0a0a 2020  e=adc_name)...  
+000029a0: 2020 2020 2020 2320 696e 6372 656d 656e        # incremen
+000029b0: 7420 746f 206e 6578 7420 6576 656e 740a  t to next event.
+000029c0: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
+000029d0: 7272 656e 745f 6669 6c65 5f65 7665 6e74  rrent_file_event
+000029e0: 5f63 6f75 6e74 6572 202b 3d20 310a 2020  _counter += 1.  
+000029f0: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
+00002a00: 2020 2020 2020 2020 2320 7265 7475 726e          # return
+00002a10: 0a20 2020 2020 2020 2069 6620 696e 636c  .        if incl
+00002a20: 7564 655f 6d65 7461 6461 7461 3a0a 2020  ude_metadata:.  
+00002a30: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002a40: 2061 7272 6179 2c69 6e66 6f0a 2020 2020   array,info.    
+00002a50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00002a60: 2020 2020 2020 7265 7475 726e 2061 7272        return arr
+00002a70: 6179 0a20 2020 2020 2020 200a 2020 2020  ay.        .    
+00002a80: 2020 2020 2020 2020 2020 0a0a 0a20 2020            ...   
+00002a90: 2064 6566 2072 6561 645f 7369 6e67 6c65   def read_single
+00002aa0: 5f65 7665 6e74 2873 656c 662c 2065 7665  _event(self, eve
+00002ab0: 6e74 5f69 6e64 6578 2c0a 2020 2020 2020  nt_index,.      
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2020 2020 6669 6c65 5f6e 616d 653d 4e6f      file_name=No
+00002ae0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00002af0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00002b00: 6967 6765 725f 696e 6465 783d 4e6f 6e65  igger_index=None
+00002b10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002b20: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00002b30: 655f 6c65 6e67 7468 5f6d 7365 633d 4e6f  e_length_msec=No
+00002b40: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00002b50: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00002b60: 6163 655f 6c65 6e67 7468 5f73 616d 706c  ace_length_sampl
+00002b70: 6573 3d4e 6f6e 652c 0a20 2020 2020 2020  es=None,.       
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2020 2070 7265 7472 6967 6765 725f 6c65     pretrigger_le
+00002ba0: 6e67 7468 5f6d 7365 633d 4e6f 6e65 2c0a  ngth_msec=None,.
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bc0: 2020 2020 2020 2020 2020 7072 6574 7269            pretri
+00002bd0: 6767 6572 5f6c 656e 6774 685f 7361 6d70  gger_length_samp
+00002be0: 6c65 733d 4e6f 6e65 2c0a 2020 2020 2020  les=None,.      
+00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c00: 2020 2020 6465 7465 6374 6f72 5f63 6861      detector_cha
+00002c10: 6e73 3d4e 6f6e 652c 0a20 2020 2020 2020  ns=None,.       
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 2061 6463 746f 766f 6c74 3d46 616c     adctovolt=Fal
+00002c40: 7365 2c20 6164 6374 6f61 6d70 3d46 616c  se, adctoamp=Fal
+00002c50: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00002c60: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+00002c70: 7365 6c69 6e65 7375 623d 4661 6c73 652c  selinesub=False,
+00002c80: 2062 6173 656c 696e 6569 6e64 733d 4e6f   baselineinds=No
+00002c90: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00002ca0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00002cb0: 636c 7564 655f 6d65 7461 6461 7461 3d46  clude_metadata=F
+00002cc0: 616c 7365 2c20 6164 635f 6e61 6d65 3d27  alse, adc_name='
+00002cd0: 6164 6331 2729 3a0a 2020 2020 2020 2020  adc1'):.        
+00002ce0: 2222 220a 2020 2020 2020 2020 5265 6164  """.        Read
+00002cf0: 2061 2073 696e 676c 6520 6576 656e 7420   a single event 
+00002d00: 6672 6f6d 2061 2066 696c 6520 6261 7365  from a file base
+00002d10: 6420 0a20 2020 2020 2020 206f 6e20 696e  d .        on in
+00002d20: 6465 7820 2822 6461 7461 7365 7422 206e  dex ("dataset" n
+00002d30: 756d 6265 7229 0a0a 2020 2020 2020 2020  umber)..        
+00002d40: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00002d50: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00002d60: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2065  ------.        e
+00002d70: 7665 6e74 5f69 6e64 6578 203a 2069 6e74  vent_index : int
+00002d80: 0a20 2020 2020 2020 2020 2065 7665 6e74  .          event
+00002d90: 2028 6864 6635 2022 6461 7461 7365 7422   (hdf5 "dataset"
+00002da0: 2920 206e 756d 6265 7220 0a20 2020 2020  )  number .     
+00002db0: 2020 200a 2020 2020 2020 2020 6669 6c65     .        file
+00002dc0: 5f6e 616d 6520 3a20 7374 722c 206f 7074  _name : str, opt
+00002dd0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00002de0: 6e61 6d65 206f 6620 7468 6520 6669 6c65  name of the file
+00002df0: 0a20 2020 2020 2020 2020 2069 6620 4e6f  .          if No
+00002e00: 6e65 3a20 7573 6520 6375 7272 656e 7420  ne: use current 
+00002e10: 6669 6c65 0a20 2020 2020 2020 200a 0a20  file.        .. 
+00002e20: 2020 2020 2020 2064 6574 6563 746f 725f         detector_
+00002e30: 6368 616e 7320 3a20 7374 7220 6f72 206c  chans : str or l
+00002e40: 6973 742c 206f 7074 696f 6e61 6c0a 2020  ist, optional.  
+00002e50: 2020 2020 2020 2020 6465 7465 6374 6f72          detector
+00002e60: 2f63 6861 6e6e 656c 206e 616d 6520 6f72  /channel name or
+00002e70: 206c 6973 7420 6f66 2064 6574 6563 746f   list of detecto
+00002e80: 7273 2f63 6861 6e6e 656c 730a 2020 2020  rs/channels.    
+00002e90: 2020 2020 2020 6966 204e 6f6e 652c 2067        if None, g
+00002ea0: 6574 2061 6c6c 2063 6861 6e6e 656c 7320  et all channels 
+00002eb0: 2864 6566 6175 6c74 290a 0a20 2020 2020  (default)..     
+00002ec0: 2020 2061 6463 746f 766f 6c74 203a 2062     adctovolt : b
+00002ed0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+00002ee0: 2020 2020 2020 2020 636f 6e76 6572 7420          convert 
+00002ef0: 6672 6f6d 2041 4443 2074 6f20 766f 6c74  from ADC to volt
+00002f00: 730a 2020 2020 2020 2020 2020 6465 6661  s.          defa
+00002f10: 756c 743a 2046 616c 7365 0a0a 2020 2020  ult: False..    
+00002f20: 2020 2020 6164 6374 6f61 6d70 203a 2062      adctoamp : b
+00002f30: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+00002f40: 2020 2020 2020 2020 636f 6e76 6572 7420          convert 
+00002f50: 6672 6f6d 2041 4443 2074 6f20 6375 7272  from ADC to curr
+00002f60: 656e 7420 616d 7073 0a20 2020 2020 2020  ent amps.       
+00002f70: 2020 2064 6566 6175 6c74 3a20 4661 6c73     default: Fals
+00002f80: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
+00002f90: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00002fa0: 2020 6261 7365 6c69 6e65 7375 623a 2062    baselinesub: b
+00002fb0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+00002fc0: 2020 2020 2020 2020 6966 2054 7275 652c          if True,
+00002fd0: 2073 7562 7472 6163 7420 7072 652d 7075   subtract pre-pu
+00002fe0: 6c73 6520 6261 7365 6c69 6e65 0a20 2020  lse baseline.   
+00002ff0: 2020 2020 2020 2064 6566 6175 6c74 3a20         default: 
+00003000: 4661 6c73 650a 0a20 2020 2020 2020 2062  False..        b
+00003010: 6173 656c 696e 6569 6e64 733a 2074 7570  aselineinds: tup
+00003020: 6c65 2028 696e 742c 2069 6e74 2920 6f72  le (int, int) or
+00003030: 206c 6973 7420 5b69 6e74 2c20 696e 745d   list [int, int]
+00003040: 0a20 2020 2020 2020 2020 206d 696e 2f6d  .          min/m
+00003050: 6178 2069 6e64 6578 2066 6f72 2020 6261  ax index for  ba
+00003060: 7365 6c69 6e65 2063 616c 6375 6c61 7469  seline calculati
+00003070: 6f6e 200a 2020 2020 2020 2020 2020 6465  on .          de
+00003080: 6661 756c 743a 2028 3130 2c20 302e 382a  fault: (10, 0.8*
+00003090: 7072 6574 7269 6767 6572 206c 656e 6774  pretrigger lengt
+000030a0: 6829 290a 2020 2020 2020 2020 2020 0a20  h)).          . 
+000030b0: 2020 2020 2020 2069 6e63 6c75 6465 5f6d         include_m
+000030c0: 6574 6164 6174 6120 3a20 626f 6f6c 2c20  etadata : bool, 
+000030d0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+000030e0: 2020 2072 6574 7572 6e20 6669 6c65 2f65     return file/e
+000030f0: 7665 6e74 2f64 6574 6563 746f 7220 6d65  vent/detector me
+00003100: 7461 6461 7461 0a20 2020 2020 2020 2020  tadata.         
+00003110: 2064 6566 6175 6c74 3a20 4661 6c73 650a   default: False.
+00003120: 0a20 2020 2020 2020 2061 6463 5f6e 616d  .        adc_nam
+00003130: 6520 3a20 7374 722c 206f 7074 696f 6e61  e : str, optiona
+00003140: 6c0a 2020 2020 2020 2020 2020 6e61 6d65  l.          name
+00003150: 2f49 4420 6f66 2074 6865 2061 6463 0a20  /ID of the adc. 
+00003160: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+00003170: 3a20 2261 6463 3122 0a0a 2020 2020 2020  : "adc1"..      
+00003180: 2020 5265 7475 726e 0a20 2020 2020 2020    Return.       
+00003190: 202d 2d2d 2d2d 2d0a 2020 2020 2020 2020   ------.        
+000031a0: 0a20 2020 2020 2020 2061 7272 6179 203a  .        array :
+000031b0: 2032 4420 6e75 6d70 7920 6172 7261 790a   2D numpy array.
+000031c0: 2020 2020 2020 2020 2020 2074 7261 6365             trace
+000031d0: 7320 666f 7220 6561 6368 2063 6861 6e6e  s for each chann
+000031e0: 656c 205b 6e62 2063 6861 6e6e 656c 2c20  el [nb channel, 
+000031f0: 6e62 2073 616d 706c 6573 5d0a 0a20 2020  nb samples]..   
+00003200: 2020 2020 2069 6e66 6f20 3a20 6469 6374       info : dict
+00003210: 0a20 2020 2020 2020 2020 2020 6669 6c65  .           file
+00003220: 2f65 7665 6e74 2f64 6574 6563 746f 7220  /event/detector 
+00003230: 6d65 7461 6461 7461 2028 6966 2022 696e  metadata (if "in
+00003240: 636c 7564 655f 6d65 7461 6461 7461 2220  clude_metadata" 
+00003250: 3d20 5472 7565 290a 0a20 2020 2020 2020  = True)..       
+00003260: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
+00003270: 6368 6563 6b20 6966 2066 696c 6520 6e65  check if file ne
+00003280: 6564 6564 0a20 2020 2020 2020 2069 6620  eded.        if 
+00003290: 286e 6f74 2073 656c 662e 5f66 696c 655f  (not self._file_
+000032a0: 6469 6374 2061 6e64 2066 696c 655f 6e61  dict and file_na
+000032b0: 6d65 2069 7320 4e6f 6e65 293a 0a20 2020  me is None):.   
+000032c0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000032d0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+000032e0: 2020 2020 2020 2020 2020 2027 4552 524f             'ERRO
+000032f0: 523a 204e 6f20 6669 6c65 2061 7661 696c  R: No file avail
+00003300: 6162 6c65 2e20 270a 2020 2020 2020 2020  able. '.        
+00003310: 2020 2020 2020 2020 2b20 2755 7365 2022          + 'Use "
+00003320: 6669 6c65 5f6e 616d 6522 2061 7267 756d  file_name" argum
+00003330: 656e 7421 2729 200a 0a0a 2020 2020 2020  ent!') ...      
+00003340: 2020 0a20 2020 2020 2020 2023 2063 7572    .        # cur
+00003350: 7265 6e74 2066 696c 6520 6469 6374 0a20  rent file dict. 
+00003360: 2020 2020 2020 2063 7572 7265 6e74 5f66         current_f
+00003370: 696c 655f 6469 6374 203d 2063 6f70 792e  ile_dict = copy.
+00003380: 6465 6570 636f 7079 2873 656c 662e 5f66  deepcopy(self._f
+00003390: 696c 655f 6469 6374 290a 2020 2020 2020  ile_dict).      
+000033a0: 2020 0a20 2020 2020 2020 2023 2020 7365    .        #  se
+000033b0: 7420 6669 6c65 206c 6973 7420 2863 6c65  t file list (cle
+000033c0: 6172 2069 6e74 6572 6e61 6c20 6461 7461  ar internal data
+000033d0: 290a 2020 2020 2020 2020 6966 2066 696c  ).        if fil
+000033e0: 655f 6e61 6d65 2069 7320 6e6f 7420 4e6f  e_name is not No
+000033f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00003400: 7365 6c66 2e73 6574 5f66 696c 6573 2866  self.set_files(f
+00003410: 696c 655f 6e61 6d65 290a 0a20 2020 2020  ile_name)..     
+00003420: 2020 2023 206c 6973 7420 6f66 2066 696c     # list of fil
+00003430: 6573 0a20 2020 2020 2020 2066 696c 655f  es.        file_
+00003440: 6c69 7374 203d 206c 6973 7428 7365 6c66  list = list(self
+00003450: 2e5f 6669 6c65 5f64 6963 742e 6b65 7973  ._file_dict.keys
+00003460: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+00003470: 0a20 2020 2020 2020 2023 206f 7065 6e20  .        # open 
+00003480: 6669 6c65 2069 6620 6e65 6564 6564 200a  file if needed .
+00003490: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000034a0: 5f63 7572 7265 6e74 5f66 696c 6520 6973  _current_file is
+000034b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000034c0: 2020 2073 656c 662e 5f6f 7065 6e5f 6669     self._open_fi
+000034d0: 6c65 2866 696c 655f 6c69 7374 5b30 5d2c  le(file_list[0],
+000034e0: 2065 7665 6e74 5f6c 6973 743d 4e6f 6e65   event_list=None
+000034f0: 290a 0a20 2020 2020 2020 200a 2020 2020  )..        .    
+00003500: 2020 2020 2320 6c6f 6164 2065 7665 6e74      # load event
+00003510: 0a20 2020 2020 2020 2061 7272 6179 2c20  .        array, 
+00003520: 696e 666f 203d 2073 656c 662e 5f6c 6f61  info = self._loa
+00003530: 645f 6576 656e 7428 0a20 2020 2020 2020  d_event(.       
+00003540: 2020 2020 2065 7665 6e74 5f69 6e64 6578       event_index
+00003550: 2c0a 2020 2020 2020 2020 2020 2020 7472  ,.            tr
+00003560: 6967 6765 725f 696e 6465 783d 7472 6967  igger_index=trig
+00003570: 6765 725f 696e 6465 782c 0a20 2020 2020  ger_index,.     
+00003580: 2020 2020 2020 2074 7261 6365 5f6c 656e         trace_len
+00003590: 6774 685f 6d73 6563 3d74 7261 6365 5f6c  gth_msec=trace_l
+000035a0: 656e 6774 685f 6d73 6563 2c0a 2020 2020  ength_msec,.    
+000035b0: 2020 2020 2020 2020 7472 6163 655f 6c65          trace_le
+000035c0: 6e67 7468 5f73 616d 706c 6573 3d74 7261  ngth_samples=tra
+000035d0: 6365 5f6c 656e 6774 685f 7361 6d70 6c65  ce_length_sample
+000035e0: 732c 0a20 2020 2020 2020 2020 2020 2070  s,.            p
+000035f0: 7265 7472 6967 6765 725f 6c65 6e67 7468  retrigger_length
+00003600: 5f6d 7365 633d 7072 6574 7269 6767 6572  _msec=pretrigger
+00003610: 5f6c 656e 6774 685f 6d73 6563 2c0a 2020  _length_msec,.  
+00003620: 2020 2020 2020 2020 2020 7072 6574 7269            pretri
+00003630: 6767 6572 5f6c 656e 6774 685f 7361 6d70  gger_length_samp
+00003640: 6c65 733d 7072 6574 7269 6767 6572 5f6c  les=pretrigger_l
+00003650: 656e 6774 685f 7361 6d70 6c65 732c 0a20  ength_samples,. 
+00003660: 2020 2020 2020 2020 2020 2064 6574 6563             detec
+00003670: 746f 725f 6368 616e 733d 6465 7465 6374  tor_chans=detect
+00003680: 6f72 5f63 6861 6e73 2c0a 2020 2020 2020  or_chans,.      
+00003690: 2020 2020 2020 6164 6374 6f76 6f6c 743d        adctovolt=
+000036a0: 6164 6374 6f76 6f6c 742c 2061 6463 746f  adctovolt, adcto
+000036b0: 616d 703d 6164 6374 6f61 6d70 2c0a 2020  amp=adctoamp,.  
+000036c0: 2020 2020 2020 2020 2020 6261 7365 6c69            baseli
+000036d0: 6e65 7375 623d 6261 7365 6c69 6e65 7375  nesub=baselinesu
+000036e0: 622c 0a20 2020 2020 2020 2020 2020 2062  b,.            b
+000036f0: 6173 656c 696e 6569 6e64 733d 6261 7365  aselineinds=base
+00003700: 6c69 6e65 696e 6473 2c0a 2020 2020 2020  lineinds,.      
+00003710: 2020 2020 2020 6164 635f 6e61 6d65 3d61        adc_name=a
+00003720: 6463 5f6e 616d 6529 0a0a 0a0a 2020 2020  dc_name)....    
+00003730: 2020 2020 2320 7365 7420 6261 636b 2066      # set back f
+00003740: 696c 6520 6469 6374 0a20 2020 2020 2020  ile dict.       
+00003750: 2073 656c 662e 636c 6561 7228 290a 2020   self.clear().  
+00003760: 2020 2020 2020 7365 6c66 2e5f 6669 6c65        self._file
+00003770: 5f64 6963 7420 3d20 6375 7272 656e 745f  _dict = current_
+00003780: 6669 6c65 5f64 6963 740a 0a20 2020 2020  file_dict..     
+00003790: 2020 2023 2072 6574 7572 6e0a 2020 2020     # return.    
+000037a0: 2020 2020 6966 2069 6e63 6c75 6465 5f6d      if include_m
+000037b0: 6574 6164 6174 613a 0a20 2020 2020 2020  etadata:.       
+000037c0: 2020 2020 2072 6574 7572 6e20 6172 7261       return arra
+000037d0: 792c 2069 6e66 6f0a 2020 2020 2020 2020  y, info.        
+000037e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000037f0: 2020 7265 7475 726e 2061 7272 6179 0a20    return array. 
+00003800: 2020 2020 2020 200a 0a20 2020 200a 2020         ..    .  
+00003810: 2020 6465 6620 7265 6164 5f6d 616e 795f    def read_many_
+00003820: 6576 656e 7473 2873 656c 662c 2066 696c  events(self, fil
+00003830: 6570 6174 683d 4e6f 6e65 2c0a 2020 2020  epath=None,.    
+00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003850: 2020 2020 206e 6576 656e 7473 3d30 2c0a       nevents=0,.
+00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003870: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+00003880: 666f 726d 6174 3d31 2c0a 2020 2020 2020  format=1,.      
+00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038a0: 2020 2064 6574 6563 746f 725f 6368 616e     detector_chan
+000038b0: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038d0: 2065 7665 6e74 5f6e 756d 733d 4e6f 6e65   event_nums=None
+000038e0: 2c20 7365 7269 6573 5f6e 756d 733d 4e6f  , series_nums=No
+000038f0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00003900: 2020 2020 2020 2020 2020 2020 2074 7269               tri
+00003910: 6767 6572 5f69 6e64 6963 6573 3d4e 6f6e  gger_indices=Non
+00003920: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00003930: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00003940: 745f 6c69 7374 3d4e 6f6e 652c 0a20 2020  t_list=None,.   
+00003950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003960: 2020 2020 2020 7472 6163 655f 6c65 6e67        trace_leng
+00003970: 7468 5f6d 7365 633d 4e6f 6e65 2c0a 2020  th_msec=None,.  
+00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003990: 2020 2020 2020 2074 7261 6365 5f6c 656e         trace_len
+000039a0: 6774 685f 7361 6d70 6c65 733d 4e6f 6e65  gth_samples=None
+000039b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000039c0: 2020 2020 2020 2020 2020 2070 7265 7472             pretr
+000039d0: 6967 6765 725f 6c65 6e67 7468 5f6d 7365  igger_length_mse
+000039e0: 633d 4e6f 6e65 2c0a 2020 2020 2020 2020  c=None,.        
+000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a00: 2070 7265 7472 6967 6765 725f 6c65 6e67   pretrigger_leng
+00003a10: 7468 5f73 616d 706c 6573 3d4e 6f6e 652c  th_samples=None,
+00003a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003a30: 2020 2020 2020 2020 2020 696e 636c 7564            includ
+00003a40: 655f 6d65 7461 6461 7461 3d46 616c 7365  e_metadata=False
+00003a50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003a60: 2020 2020 2020 2020 2020 2061 6463 746f             adcto
+00003a70: 766f 6c74 3d46 616c 7365 2c20 6164 6374  volt=False, adct
+00003a80: 6f61 6d70 3d46 616c 7365 2c0a 2020 2020  oamp=False,.    
+00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003aa0: 2020 2020 2062 6173 656c 696e 6573 7562       baselinesub
+00003ab0: 3d46 616c 7365 2c20 6261 7365 6c69 6e65  =False, baseline
+00003ac0: 696e 6473 3d4e 6f6e 652c 0a20 2020 2020  inds=None,.     
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ae0: 2020 2020 6d65 6d6f 7279 5f6c 696d 6974      memory_limit
+00003af0: 3d34 2c20 6164 635f 6e61 6d65 3d27 6164  =4, adc_name='ad
+00003b00: 6331 2729 3a0a 2020 2020 2020 2020 2222  c1'):.        ""
+00003b10: 220a 2020 2020 2020 2020 5265 6164 206d  ".        Read m
+00003b20: 756c 7469 706c 6520 6576 656e 7473 2028  ultiple events (
+00003b30: 6465 6661 756c 7420 7265 6164 2061 6c6c  default read all
+00003b40: 2065 7665 6e74 7329 0a20 2020 2020 2020   events).       
+00003b50: 200a 2020 2020 2020 2020 5061 7261 6d65   .        Parame
+00003b60: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00003b70: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2066  ------.        f
+00003b80: 696c 6570 6174 683a 2073 7472 696e 6720  ilepath: string 
+00003b90: 6f72 206c 6973 7420 206f 6620 7374 7269  or list  of stri
+00003ba0: 6e67 730a 2020 2020 2020 2020 2020 2066  ngs.           f
+00003bb0: 696c 652f 7061 7468 206f 7220 6c69 7374  ile/path or list
+00003bc0: 206f 6620 6669 6c65 732f 7061 7468 7320   of files/paths 
+00003bd0: 2864 6566 6175 6c74 3a20 7573 6520 6375  (default: use cu
+00003be0: 7272 656e 7420 6669 6c65 290a 2020 2020  rrent file).    
+00003bf0: 2020 2020 2020 0a20 2020 2020 2020 206e        .        n
+00003c00: 6576 656e 7473 3a20 696e 7465 6765 720a  events: integer.
+00003c10: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
+00003c20: 7220 6f66 2065 7665 6e74 7320 746f 2072  r of events to r
+00003c30: 6561 6420 2028 6465 6661 756c 7420 6e62  ead  (default nb
+00003c40: 5f65 7665 6e74 733d 3020 2d3e 2061 6c6c  _events=0 -> all
+00003c50: 2065 7665 6e74 7320 696e 2064 756d 7073   events in dumps
+00003c60: 290a 0a20 2020 2020 2020 206f 7574 7075  )..        outpu
+00003c70: 745f 666f 726d 6174 3a20 696e 7465 6765  t_format: intege
+00003c80: 720a 2020 2020 2020 2020 2020 2020 313a  r.            1:
+00003c90: 206c 6973 7420 6f66 2032 4420 6e64 6172   list of 2D ndar
+00003ca0: 7261 795b 6368 616e 2c20 7361 6d70 6c65  ray[chan, sample
+00003cb0: 735d 0a20 2020 2020 2020 2020 2020 2032  s].            2
+00003cc0: 3a20 3344 206e 6461 7272 6179 5b65 7665  : 3D ndarray[eve
+00003cd0: 6e74 2c20 6368 616e 2c20 7361 6d70 6c65  nt, chan, sample
+00003ce0: 735d 0a20 0a20 2020 2020 2020 2064 6574  s]. .        det
+00003cf0: 6563 746f 725f 6368 616e 733a 2073 7472  ector_chans: str
+00003d00: 696e 672f 696e 7420 6f72 206c 6973 7420  ing/int or list 
+00003d10: 6f66 2073 7472 696e 672f 696e 740a 2020  of string/int.  
+00003d20: 2020 2020 2020 2020 2020 6465 7465 6374            detect
+00003d30: 6f72 2063 6861 6e6e 656c 206e 616d 6529  or channel name)
+00003d40: 2873 2920 2865 7861 6d70 6c65 2027 5a31  (s) (example 'Z1
+00003d50: 5041 5331 272c 2027 5044 3227 2c20 6f72  PAS1', 'PD2', or
+00003d60: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+00003d70: 666f 6c6c 6f77 696e 6720 666f 726d 6174  following format
+00003d80: 2069 6e20 7365 7475 702e 696e 6920 6669   in setup.ini fi
+00003d90: 6c65 0a20 2020 2020 2020 2020 2020 2049  le.            I
+00003da0: 6620 4e6f 6e65 2c20 7265 6164 2061 6c6c  f None, read all
+00003db0: 2063 6861 6e6e 656c 7320 6176 6169 6c61   channels availa
+00003dc0: 626c 6520 0a0a 2020 2020 2020 2020 6576  ble ..        ev
+00003dd0: 656e 745f 6e75 6d73 3a20 6c69 7374 206f  ent_nums: list o
+00003de0: 7220 6e75 6d70 7920 6172 7261 790a 2020  r numpy array.  
+00003df0: 2020 2020 2020 2020 2020 4576 656e 7420            Event 
+00003e00: 6e75 6d62 6572 7320 2866 6f72 6d61 743a  numbers (format:
+00003e10: 2064 756d 705f 6e75 6d20 2a20 3130 3030   dump_num * 1000
+00003e20: 3030 202b 2065 7665 6e74 5f69 6e64 6578  00 + event_index
+00003e30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003e40: 0a20 2020 2020 2020 2073 6572 6965 735f  .        series_
+00003e50: 6e75 6d73 3a20 6c69 7374 206f 7220 6e75  nums: list or nu
+00003e60: 6d70 7920 6172 7261 790a 2020 2020 2020  mpy array.      
+00003e70: 2020 2020 2020 5365 7269 6573 206e 756d        Series num
+00003e80: 6265 7273 2028 666f 726d 6174 3a20 7879  bers (format: xy
+00003e90: 7979 796d 6d64 6468 686d 6d73 7329 0a20  yyymmddhhmmss). 
+00003ea0: 2020 2020 2020 2020 2020 2069 6620 6576             if ev
+00003eb0: 656e 745f 6e75 6d73 2061 7267 756d 656e  ent_nums argumen
+00003ec0: 7420 7072 6f76 6964 6564 2c20 7365 7269  t provided, seri
+00003ed0: 6573 5f6e 756d 7320 7368 6f75 6c64 2068  es_nums should h
+00003ee0: 6176 6520 7361 6d65 206c 656e 6774 6821  ave same length!
+00003ef0: 290a 0a20 2020 2020 2020 2069 6e63 6c75  )..        inclu
+00003f00: 6465 5f6d 6574 6164 6174 613a 2062 6f6f  de_metadata: boo
+00003f10: 6c20 0a20 2020 2020 2020 2020 2020 2069  l .            i
+00003f20: 6e63 6c75 6465 2066 696c 652f 6772 6f75  nclude file/grou
+00003f30: 702f 6461 7461 7365 7420 6d65 7461 6461  p/dataset metada
+00003f40: 7461 2028 6465 6661 756c 7420 3d20 4661  ta (default = Fa
+00003f50: 6c73 6529 0a0a 2020 2020 2020 2020 6164  lse)..        ad
+00003f60: 6374 6f76 6f6c 743a 2042 6f6f 6c0a 2020  ctovolt: Bool.  
+00003f70: 2020 2020 2020 2020 2020 436f 6e76 6572            Conver
+00003f80: 7420 2066 726f 6d20 4144 4320 746f 2076  t  from ADC to v
+00003f90: 6f6c 7420 2844 6566 6175 6c74 3d46 616c  olt (Default=Fal
+00003fa0: 7365 2920 0a20 2020 2020 2020 200a 2020  se) .        .  
+00003fb0: 2020 2020 2020 6164 6374 6f61 6d70 3a20        adctoamp: 
+00003fc0: 426f 6f6c 0a20 2020 2020 2020 2020 2020  Bool.           
+00003fd0: 2043 6f6e 7665 7274 2020 6672 6f6d 2041   Convert  from A
+00003fe0: 4443 2074 6f20 636c 6f73 6520 6c6f 6f70  DC to close loop
+00003ff0: 2f46 4c4c 2061 6d70 7320 2844 6566 6175  /FLL amps (Defau
+00004000: 6c74 3d46 616c 7365 2920 0a0a 2020 2020  lt=False) ..    
+00004010: 2020 2020 6261 7365 6c69 6e65 7375 623a      baselinesub:
+00004020: 2042 6f6f 6c0a 2020 2020 2020 2020 2020   Bool.          
+00004030: 2020 4170 706c 7920 6261 7365 6c69 6e65    Apply baseline
+00004040: 2073 7562 7472 6163 7469 6f6e 0a0a 2020   subtraction..  
+00004050: 2020 2020 2020 6261 7365 6c69 6e65 696e        baselinein
+00004060: 6473 3a20 7475 706c 6520 2869 6e74 2c20  ds: tuple (int, 
+00004070: 696e 7429 206f 7220 6c69 7374 205b 696e  int) or list [in
+00004080: 742c 2069 6e74 5d0a 2020 2020 2020 2020  t, int].        
+00004090: 2020 2020 7374 6172 742f 7374 6f70 2062      start/stop b
+000040a0: 6173 656c 696e 6520 6361 6c63 756c 6174  aseline calculat
+000040b0: 696f 6e20 2864 6566 6175 6c74 3a20 2831  ion (default: (1
+000040c0: 302c 2030 2e38 2a70 7265 7472 6967 6765  0, 0.8*pretrigge
+000040d0: 7220 6c65 6e67 7468 2929 0a20 2020 2020  r length)).     
+000040e0: 2020 2020 200a 2020 2020 2020 2020 6d65       .        me
+000040f0: 6d6f 7279 5f6c 696d 6974 3a20 466c 6f61  mory_limit: Floa
+00004100: 740a 2020 2020 2020 2020 2020 2020 5075  t.            Pu
+00004110: 6c73 6520 6461 7461 206d 656d 6f72 7920  lse data memory 
+00004120: 6c69 6d69 7420 696e 2047 4220 5b64 6566  limit in GB [def
+00004130: 6175 6c74 3a20 3247 425d 0a0a 2020 2020  ault: 2GB]..    
+00004140: 2020 2020 6164 635f 6e61 6d65 3a20 7374      adc_name: st
+00004150: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
+00004160: 2020 2041 4443 2069 6420 2864 6566 6175     ADC id (defau
+00004170: 6c74 3a20 2761 6463 3127 290a 2020 2020  lt: 'adc1').    
+00004180: 2020 2020 2020 0a0a 2020 2020 2020 2020        ..        
+00004190: 5265 7475 726e 0a20 2020 2020 2020 202d  Return.        -
+000041a0: 2d2d 2d2d 2d0a 200a 2020 2020 2020 2020  -----. .        
+000041b0: 6f75 7470 7574 5f64 6174 6120 3a20 6c69  output_data : li
+000041c0: 7374 206f 7220 7061 6e64 6173 2064 6174  st or pandas dat
+000041d0: 6166 7261 6d65 0a20 2020 2020 2020 2020  aframe.         
+000041e0: 2020 7472 6163 6573 2066 6f72 2065 6163    traces for eac
+000041f0: 6820 6368 616e 6e65 6c73 2061 6e64 2065  h channels and e
+00004200: 7665 6e74 730a 0a20 2020 2020 2020 2069  vents..        i
+00004210: 6e66 6f20 3a20 6c69 7374 0a20 2020 2020  nfo : list.     
+00004220: 2020 2020 2020 6669 6c65 2f65 7665 6e74        file/event
+00004230: 2f64 6574 6563 746f 7220 6d65 7461 6461  /detector metada
+00004240: 7461 200a 2020 2020 2020 2020 2020 2028  ta .           (
+00004250: 6966 2022 696e 636c 7564 655f 6d65 7461  if "include_meta
+00004260: 6461 7461 2220 3d20 5472 7565 290a 0a0a  data" = True)...
+00004270: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00004280: 2020 2020 2023 203d 3d3d 3d3d 3d3d 3d3d       # =========
+00004290: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000042a0: 3d3d 3d3d 3d3d 0a20 2020 2020 2020 2023  ======.        #
+000042b0: 2043 6865 636b 2061 7267 756d 656e 7473   Check arguments
+000042c0: 0a20 2020 2020 2020 2023 203d 3d3d 3d3d  .        # =====
+000042d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000042e0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 200a 2020  ==========.. .  
+000042f0: 2020 2020 2020 2320 6368 6563 6b20 6966        # check if
+00004300: 2066 696c 6520 6e65 6564 6564 0a20 2020   file needed.   
+00004310: 2020 2020 2069 6620 286e 6f74 2073 656c       if (not sel
+00004320: 662e 5f66 696c 655f 6469 6374 2061 6e64  f._file_dict and
+00004330: 2066 696c 6570 6174 6820 6973 204e 6f6e   filepath is Non
+00004340: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00004350: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00004360: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004370: 2020 2745 5252 4f52 3a20 4e6f 2066 696c    'ERROR: No fil
+00004380: 6520 6176 6169 6c61 626c 652e 2027 0a20  e available. '. 
+00004390: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+000043a0: 2027 5573 6520 2266 696c 655f 6e61 6d65   'Use "file_name
+000043b0: 2220 6172 6775 6d65 6e74 2127 2920 0a0a  " argument!') ..
+000043c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000043d0: 2020 2320 6465 7465 6374 6f72 2f63 6861    # detector/cha
+000043e0: 6e6e 656c 0a20 2020 2020 2020 2069 6620  nnel.        if 
+000043f0: 2864 6574 6563 746f 725f 6368 616e 7320  (detector_chans 
+00004400: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+00004410: 2020 2020 2020 2020 616e 6420 6e6f 7420          and not 
+00004420: 2869 7369 6e73 7461 6e63 6528 6465 7465  (isinstance(dete
+00004430: 6374 6f72 5f63 6861 6e73 2c20 6c69 7374  ctor_chans, list
+00004440: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004450: 2020 2020 2020 206f 7220 6973 696e 7374         or isinst
+00004460: 616e 6365 2864 6574 6563 746f 725f 6368  ance(detector_ch
+00004470: 616e 732c 206e 702e 6e64 6172 7261 7929  ans, np.ndarray)
+00004480: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00004490: 6465 7465 6374 6f72 5f63 6861 6e73 203d  detector_chans =
+000044a0: 205b 6465 7465 6374 6f72 5f63 6861 6e73   [detector_chans
+000044b0: 5d0a 2020 2020 0a0a 2020 2020 2020 2020  ].    ..        
+000044c0: 2320 6576 656e 7420 6c69 7374 0a20 2020  # event list.   
+000044d0: 2020 2020 2069 6620 2865 7665 6e74 5f6c       if (event_l
+000044e0: 6973 7420 6973 206e 6f74 204e 6f6e 650a  ist is not None.
+000044f0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00004500: 2865 7665 6e74 5f6e 756d 7320 6973 206e  (event_nums is n
+00004510: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+00004520: 2020 2020 2020 2020 206f 7220 7365 7269           or seri
+00004530: 6573 5f6e 756d 7320 6973 206e 6f74 204e  es_nums is not N
+00004540: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00004550: 2020 2020 206f 7220 7472 6967 6765 725f       or trigger_
+00004560: 696e 6469 6365 7320 6973 206e 6f74 204e  indices is not N
+00004570: 6f6e 6529 293a 0a20 2020 2020 2020 2020  one)):.         
+00004580: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00004590: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+000045a0: 2020 2020 2027 4552 524f 523a 2043 686f       'ERROR: Cho
+000045b0: 6f73 6520 2265 7665 6e74 5f6c 6973 7422  ose "event_list"
+000045c0: 2061 7267 756d 656e 7420 270a 2020 2020   argument '.    
+000045d0: 2020 2020 2020 2020 2020 2020 2b20 274f              + 'O
+000045e0: 5220 2265 7665 6e74 5f6e 756d 7322 2f22  R "event_nums"/"
+000045f0: 7365 7269 6573 5f6e 756d 7322 2f22 7472  series_nums"/"tr
+00004600: 6967 6765 725f 696e 6469 6365 7327 290a  igger_indices').
+00004610: 0a0a 2020 2020 2020 2020 2320 7072 656c  ..        # prel
+00004620: 696d 696e 6172 7920 6368 6563 6b73 206f  iminary checks o
+00004630: 6620 6576 656e 742f 7365 7269 6573 2f74  f event/series/t
+00004640: 7269 6767 6572 206e 756d 730a 2020 2020  rigger nums.    
+00004650: 2020 2020 6966 2074 7269 6767 6572 5f69      if trigger_i
+00004660: 6e64 6963 6573 2069 7320 6e6f 7420 4e6f  ndices is not No
+00004670: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00004680: 6966 2065 7665 6e74 5f6e 756d 7320 6973  if event_nums is
+00004690: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000046a0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+000046b0: 7565 4572 726f 7228 2745 5252 4f52 3a20  ueError('ERROR: 
+000046c0: 2265 7665 6e5f 6e75 6d73 2220 7265 7175  "even_nums" requ
+000046d0: 6972 6564 2069 6620 270a 2020 2020 2020  ired if '.      
+000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046f0: 2020 2020 2020 2020 2020 202b 2027 6576             + 'ev
+00004700: 656e 7420 7365 6c65 6374 6564 2077 6974  ent selected wit
+00004710: 6820 2274 7269 6767 6572 2069 6e64 6963  h "trigger indic
+00004720: 6573 2227 290a 2020 2020 2020 2020 2020  es"').          
+00004730: 2020 0a20 2020 2020 2020 2020 2020 2069    .            i
+00004740: 6620 2874 7261 6365 5f6c 656e 6774 685f  f (trace_length_
+00004750: 6d73 6563 2069 7320 4e6f 6e65 0a20 2020  msec is None.   
+00004760: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00004770: 2074 7261 6365 5f6c 656e 6774 685f 7361   trace_length_sa
+00004780: 6d70 6c65 7320 6973 204e 6f6e 6529 3a0a  mples is None):.
 00004790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047a0: 6475 6d70 5f6e 616d 6520 3d20 7374 7228  dump_name = str(
-000047b0: 6475 6d70 5f6e 756d 290a 2020 2020 2020  dump_num).      
-000047c0: 2020 2020 2020 2020 2020 666f 7220 7820            for x 
-000047d0: 696e 2072 616e 6765 2831 2c35 2d6c 656e  in range(1,5-len
-000047e0: 2864 756d 705f 6e61 6d65 2929 3a0a 2020  (dump_name)):.  
-000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 2020 6475 6d70 5f6e 616d 6520 3d20 2730    dump_name = '0
-00004810: 272b 6475 6d70 5f6e 616d 650a 2020 2020  '+dump_name.    
-00004820: 2020 2020 2020 2020 2020 2020 7365 7269              seri
-00004830: 6573 5f64 756d 705f 6e61 6d65 732e 6170  es_dump_names.ap
-00004840: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
-00004850: 2020 2020 2020 2020 2020 7365 7269 6573            series
-00004860: 5f6e 616d 6573 5b69 6576 656e 745d 202b  _names[ievent] +
-00004870: 2027 5f46 2720 2b20 6475 6d70 5f6e 616d   '_F' + dump_nam
-00004880: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00004890: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000048a0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-000048b0: 2023 2066 696c 7465 7220 6669 6c65 730a   # filter files.
-000048c0: 2020 2020 2020 2020 2020 2020 6576 656e              even
-000048d0: 745f 6669 6c74 6572 6564 5f66 696c 6573  t_filtered_files
-000048e0: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
-000048f0: 2020 2020 2020 666f 7220 6669 6c65 5f6e        for file_n
-00004900: 616d 6520 696e 2066 696c 7465 7265 645f  ame in filtered_
-00004910: 6669 6c65 5f6c 6973 743a 0a20 2020 2020  file_list:.     
-00004920: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-00004930: 6572 6965 735f 6475 6d70 2069 6e20 7365  eries_dump in se
-00004940: 7269 6573 5f64 756d 705f 6e61 6d65 733a  ries_dump_names:
-00004950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004960: 2020 2020 2069 6620 7365 7269 6573 5f64       if series_d
-00004970: 756d 7020 696e 2066 696c 655f 6e61 6d65  ump in file_name
-00004980: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004990: 2020 2020 2020 2020 2020 6576 656e 745f            event_
-000049a0: 6669 6c74 6572 6564 5f66 696c 6573 2e61  filtered_files.a
-000049b0: 7070 656e 6428 6669 6c65 5f6e 616d 6529  ppend(file_name)
-000049c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000049d0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-000049e0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-000049f0: 2020 2020 2020 2020 6669 6c74 6572 6564          filtered
-00004a00: 5f66 696c 655f 6c69 7374 203d 2065 7665  _file_list = eve
-00004a10: 6e74 5f66 696c 7465 7265 645f 6669 6c65  nt_filtered_file
-00004a20: 730a 2020 2020 0a20 2020 2020 2020 2020  s.    .         
-00004a30: 2020 200a 2020 2020 2020 2020 2320 7265     .        # re
-00004a40: 706c 6163 6520 6669 6c65 206c 6973 740a  place file list.
-00004a50: 2020 2020 2020 2020 6966 2066 696c 7465          if filte
-00004a60: 7265 645f 6669 6c65 5f6c 6973 743a 0a20  red_file_list:. 
-00004a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004a80: 7365 745f 6669 6c65 7328 6669 6c74 6572  set_files(filter
-00004a90: 6564 5f66 696c 655f 6c69 7374 290a 2020  ed_file_list).  
-00004aa0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00004ab0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00004ac0: 2020 2020 2023 203d 3d3d 3d3d 3d3d 3d3d       # =========
-00004ad0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004ae0: 3d3d 3d3d 3d3d 0a20 2020 2020 2020 2023  ======.        #
-00004af0: 2043 6865 636b 2072 6177 2064 6174 610a   Check raw data.
-00004b00: 2020 2020 2020 2020 2320 3d3d 3d3d 3d3d          # ======
-00004b10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004b20: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 2020  =========.      
-00004b30: 2020 0a20 2020 2020 2020 2023 2069 6e69    .        # ini
-00004b40: 7469 616c 697a 6520 7573 6566 756c 2070  tialize useful p
-00004b50: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00004b60: 2020 6e62 5f65 7665 6e74 735f 746f 7420    nb_events_tot 
-00004b70: 3d20 300a 2020 2020 2020 2020 6e62 5f63  = 0.        nb_c
-00004b80: 6861 6e6e 656c 7320 3d20 300a 2020 2020  hannels = 0.    
-00004b90: 2020 2020 6e62 5f73 616d 706c 6573 203d      nb_samples =
-00004ba0: 2030 0a20 2020 2020 2020 0a20 2020 2020   0.       .     
-00004bb0: 2020 2023 2073 656c 6563 7465 6420 6669     # selected fi
-00004bc0: 6c65 7320 2863 6173 6520 7365 7269 6573  les (case series
-00004bd0: 206e 756d 6265 7220 6f6e 6c79 2070 726f   number only pro
-00004be0: 7669 6465 6429 0a20 2020 2020 2020 2023  vided).        #
-00004bf0: 2020 2020 7475 706c 6520 2865 7665 6e74      tuple (event
-00004c00: 2069 6e64 6578 2c20 6669 6c65 2920 6966   index, file) if
-00004c10: 2065 7665 6e74 2070 726f 7669 6465 640a   event provided.
-00004c20: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
-00004c30: 5f65 7665 6e74 5f66 696c 6573 203d 206c  _event_files = l
-00004c40: 6973 7428 290a 2020 2020 0a20 2020 2020  ist().    .     
-00004c50: 2020 200a 2020 2020 2020 2020 2320 6c6f     .        # lo
-00004c60: 6f70 2066 696c 6573 2074 6f20 6765 7420  op files to get 
-00004c70: 6e75 6d62 6572 206f 6620 6576 656e 7473  number of events
-00004c80: 0a20 2020 2020 2020 2066 6f72 2066 696c  .        for fil
-00004c90: 655f 6e61 6d65 2069 6e20 7365 6c66 2e5f  e_name in self._
-00004ca0: 6669 6c65 5f6c 6973 743a 0a0a 2020 2020  file_list:..    
-00004cb0: 2020 2020 2020 2020 2320 6765 7420 6d65          # get me
-00004cc0: 7461 6461 7461 0a20 2020 2020 2020 2020  tadata.         
-00004cd0: 2020 206d 6574 6164 6174 6120 3d20 7365     metadata = se
-00004ce0: 6c66 2e67 6574 5f6d 6574 6164 6174 6128  lf.get_metadata(
-00004cf0: 6669 6c65 5f6e 616d 6529 0a20 2020 2020  file_name).     
-00004d00: 2020 2020 2020 2061 6463 5f6d 6574 6164         adc_metad
-00004d10: 6174 6120 3d20 6d65 7461 6461 7461 5b27  ata = metadata['
-00004d20: 6772 6f75 7073 275d 5b61 6463 5f6e 616d  groups'][adc_nam
-00004d30: 655d 0a0a 0a20 2020 2020 2020 2020 2020  e]...           
-00004d40: 2023 2065 7874 7261 6374 2064 756d 7020   # extract dump 
-00004d50: 616e 6420 7365 7269 6573 2062 6173 6564  and series based
-00004d60: 206f 6e20 6d65 7461 6461 7461 0a20 2020   on metadata.   
-00004d70: 2020 2020 2020 2020 2066 696c 655f 7365           file_se
-00004d80: 7269 6573 5f6e 756d 203d 204e 6f6e 650a  ries_num = None.
-00004d90: 2020 2020 2020 2020 2020 2020 6966 2027              if '
-00004da0: 7365 7269 6573 5f6e 756d 2720 696e 206d  series_num' in m
-00004db0: 6574 6164 6174 613a 0a20 2020 2020 2020  etadata:.       
-00004dc0: 2020 2020 2020 2020 2066 696c 655f 7365           file_se
-00004dd0: 7269 6573 5f6e 756d 203d 2069 6e74 286d  ries_num = int(m
-00004de0: 6574 6164 6174 615b 2773 6572 6965 735f  etadata['series_
-00004df0: 6e75 6d27 5d29 0a20 2020 2020 2020 2020  num']).         
-00004e00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00004e10: 2020 2020 2020 2020 2066 696c 655f 7365           file_se
-00004e20: 7269 6573 5f6e 756d 203d 2069 6e74 2865  ries_num = int(e
-00004e30: 7874 7261 6374 5f73 6572 6965 735f 6e75  xtract_series_nu
-00004e40: 6d28 6669 6c65 5f6e 616d 6529 290a 2020  m(file_name)).  
-00004e50: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00004e60: 2020 2020 2020 2023 2065 7874 7261 6374         # extract
-00004e70: 2064 756d 7020 6e75 6d62 6572 0a20 2020   dump number.   
-00004e80: 2020 2020 2020 2020 2066 696c 655f 6475           file_du
-00004e90: 6d70 5f6e 756d 203d 204e 6f6e 6520 200a  mp_num = None  .
-00004ea0: 2020 2020 2020 2020 2020 2020 6966 2027              if '
-00004eb0: 6475 6d70 5f6e 756d 2720 696e 206d 6574  dump_num' in met
-00004ec0: 6164 6174 613a 0a20 2020 2020 2020 2020  adata:.         
-00004ed0: 2020 2020 2020 2066 696c 655f 6475 6d70         file_dump
-00004ee0: 5f6e 756d 203d 2069 6e74 286d 6574 6164  _num = int(metad
-00004ef0: 6174 615b 2764 756d 705f 6e75 6d27 5d29  ata['dump_num'])
-00004f00: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00004f10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00004f20: 2020 2066 696c 655f 6475 6d70 5f6e 756d     file_dump_num
-00004f30: 203d 2069 6e74 2865 7874 7261 6374 5f64   = int(extract_d
-00004f40: 756d 705f 6e75 6d28 6669 6c65 5f6e 616d  ump_num(file_nam
-00004f50: 6529 290a 0a20 2020 2020 2020 2020 2020  e))..           
-00004f60: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-00004f70: 2020 2020 2020 2020 2020 2320 6966 2065            # if e
-00004f80: 7665 6e74 5f6e 756d 733a 2020 6368 6563  vent_nums:  chec
-00004f90: 6b20 6669 6c65 2069 6620 6176 6169 6c61  k file if availa
-00004fa0: 626c 6520 616e 6420 7374 6f72 6520 6974  ble and store it
-00004fb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00004fc0: 6576 656e 745f 6e75 6d73 2069 7320 6e6f  event_nums is no
-00004fd0: 7420 4e6f 6e65 3a0a 0a20 2020 2020 2020  t None:..       
-00004fe0: 2020 2020 2020 2020 206b 6565 705f 6669           keep_fi
-00004ff0: 6c65 203d 2046 616c 7365 0a0a 2020 2020  le = False..    
-00005000: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00005010: 6965 7665 6e74 2069 6e20 7261 6e67 6528  ievent in range(
-00005020: 6c65 6e28 6576 656e 745f 6e75 6d73 2929  len(event_nums))
-00005030: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005040: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
-00005050: 6620 6475 6d70 206e 756d 6265 7220 6d61  f dump number ma
-00005060: 7463 6820 6375 7272 656e 7420 6669 6c65  tch current file
-00005070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005080: 2020 2020 2069 6620 2869 6e74 2864 756d       if (int(dum
-00005090: 705f 6e75 6d73 5b69 6576 656e 745d 2921  p_nums[ievent])!
-000050a0: 3d66 696c 655f 6475 6d70 5f6e 756d 293a  =file_dump_num):
-000050b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000050c0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000050d0: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
-000050e0: 2020 2020 2020 2023 2063 6865 636b 2073         # check s
-000050f0: 6572 6965 7320 6d61 7463 6820 6375 7272  eries match curr
-00005100: 656e 7420 6669 6c65 0a20 2020 2020 2020  ent file.       
-00005110: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005120: 2869 6e74 2873 6572 6965 735f 6e75 6d73  (int(series_nums
-00005130: 5b69 6576 656e 745d 2921 3d66 696c 655f  [ievent])!=file_
-00005140: 7365 7269 6573 5f6e 756d 293a 0a20 2020  series_num):.   
-00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005160: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005180: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
-00005190: 2020 2020 2020 2023 2046 6f75 6e64 2066         # Found f
-000051a0: 696c 6521 0a20 2020 2020 2020 2020 2020  ile!.           
-000051b0: 2020 2020 2020 2020 206b 6565 705f 6669           keep_fi
-000051c0: 6c65 2020 3d20 5472 7565 0a0a 2020 2020  le  = True..    
-000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051e0: 2320 6368 6563 6b20 696e 6465 7820 6176  # check index av
-000051f0: 6169 6c61 626c 650a 2020 2020 2020 2020  ailable.        
-00005200: 2020 2020 2020 2020 2020 2020 6576 656e              even
-00005210: 745f 696e 6465 7820 3d20 6576 656e 745f  t_index = event_
-00005220: 696e 6469 6365 735b 6965 7665 6e74 5d0a  indices[ievent].
-00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005240: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00005250: 2020 2020 2020 2020 2069 6620 2865 7665           if (eve
-00005260: 6e74 5f69 6e64 6578 3e69 6e74 2861 6463  nt_index>int(adc
-00005270: 5f6d 6574 6164 6174 615b 276e 625f 6576  _metadata['nb_ev
-00005280: 656e 7473 275d 2929 3a0a 2020 2020 2020  ents'])):.      
-00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052a0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-000052b0: 6f72 2827 4552 524f 523a 2046 6f75 6e64  or('ERROR: Found
-000052c0: 2066 696c 6520 666f 7220 6576 656e 7420   file for event 
-000052d0: 6e75 6d62 6572 2027 0a20 2020 2020 2020  number '.       
+000047a0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+000047b0: 2827 4552 524f 523a 2054 7261 6365 206c  ('ERROR: Trace l
+000047c0: 656e 6774 6820 7265 7175 6972 6564 2069  ength required i
+000047d0: 6620 270a 2020 2020 2020 2020 2020 2020  f '.            
+000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047f0: 2020 2020 202b 2027 6576 656e 7420 7365       + 'event se
+00004800: 6c65 6374 6564 2077 6974 6820 2274 7269  lected with "tri
+00004810: 6767 6572 2069 6e64 6963 6573 2227 290a  gger indices"').
+00004820: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004830: 2870 7265 7472 6967 6765 725f 6c65 6e67  (pretrigger_leng
+00004840: 7468 5f6d 7365 6320 6973 204e 6f6e 650a  th_msec is None.
+00004850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004860: 616e 6420 7072 6574 7269 6767 6572 5f6c  and pretrigger_l
+00004870: 656e 6774 685f 7361 6d70 6c65 7320 6973  ength_samples is
+00004880: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00004890: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+000048a0: 6c75 6545 7272 6f72 2827 4552 524f 523a  lueError('ERROR:
+000048b0: 2050 7265 7472 6967 6765 7220 6c65 6e67   Pretrigger leng
+000048c0: 7468 2072 6571 7569 7265 6420 6966 2027  th required if '
+000048d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048f0: 2020 2b20 2765 7665 6e74 2073 656c 6563    + 'event selec
+00004900: 7465 6420 7769 7468 2022 7472 6967 6765  ted with "trigge
+00004910: 7220 696e 6469 6365 7322 2729 0a0a 0a0a  r indices"')....
+00004920: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+00004930: 5f6e 756d 7320 6973 206e 6f74 204e 6f6e  _nums is not Non
+00004940: 653a 0a20 2020 2020 2020 2020 2020 200a  e:.            .
+00004950: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00004960: 6572 6965 735f 6e75 6d73 2069 7320 4e6f  eries_nums is No
+00004970: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00004980: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00004990: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+000049a0: 2020 2020 2020 2020 2020 2745 5252 4f52            'ERROR
+000049b0: 3a20 2273 6572 6965 735f 6e75 6d73 2220  : "series_nums" 
+000049c0: 7265 7175 6972 6564 2069 6620 270a 2020  required if '.  
+000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049e0: 2020 2b20 2722 6576 656e 745f 6e75 6d73    + '"event_nums
+000049f0: 2220 6172 6775 6d65 6e74 2075 7365 6421  " argument used!
+00004a00: 2729 0a0a 0a20 2020 2020 2020 2020 2020  ')...           
+00004a10: 200a 2020 2020 2020 2020 2320 3d3d 3d3d   .        # ====
+00004a20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004a30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
+00004a40: 2020 2020 2320 4c69 7374 206f 6620 6669      # List of fi
+00004a50: 6c65 730a 2020 2020 2020 2020 2320 3d3d  les.        # ==
+00004a60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004a70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a20  =============.. 
+00004a80: 2020 2020 2020 2023 206c 6574 2773 206b         # let's k
+00004a90: 6565 7020 6120 636f 7079 2069 6e74 6572  eep a copy inter
+00004aa0: 6e61 6c20 6669 6c65 2064 6963 740a 2020  nal file dict.  
+00004ab0: 2020 2020 2020 6375 7272 656e 745f 6669        current_fi
+00004ac0: 6c65 5f64 6963 7420 3d20 636f 7079 2e64  le_dict = copy.d
+00004ad0: 6565 7063 6f70 7928 7365 6c66 2e5f 6669  eepcopy(self._fi
+00004ae0: 6c65 5f64 6963 7429 0a20 2020 2020 2020  le_dict).       
+00004af0: 200a 2020 2020 2020 2020 2320 636f 6e76   .        # conv
+00004b00: 6572 7420 2265 7665 6e74 5f6e 756d 7322  ert "event_nums"
+00004b10: 2f22 7365 7269 6573 5f6e 756d 7322 2074  /"series_nums" t
+00004b20: 6f20 2265 7665 6e74 5f6c 6973 7422 0a20  o "event_list". 
+00004b30: 2020 2020 2020 2069 6620 6576 656e 745f         if event_
+00004b40: 6e75 6d73 2069 7320 6e6f 7420 4e6f 6e65  nums is not None
+00004b50: 3a0a 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00004b60: 2063 6f6e 7665 7274 2074 6f20 6c69 7374   convert to list
+00004b70: 2069 6620 6e6f 7420 6172 7261 792f 6c69   if not array/li
+00004b80: 7374 0a20 2020 2020 2020 2020 2020 2069  st.            i
+00004b90: 6620 286e 6f74 2069 7369 6e73 7461 6e63  f (not isinstanc
+00004ba0: 6528 6576 656e 745f 6e75 6d73 2c20 6c69  e(event_nums, li
+00004bb0: 7374 290a 2020 2020 2020 2020 2020 2020  st).            
+00004bc0: 2020 2020 616e 6420 6e6f 7420 6973 696e      and not isin
+00004bd0: 7374 616e 6365 2865 7665 6e74 5f6e 756d  stance(event_num
+00004be0: 732c 206e 702e 6e64 6172 7261 7929 293a  s, np.ndarray)):
+00004bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004c00: 2065 7665 6e74 5f6e 756d 7320 3d20 5b65   event_nums = [e
+00004c10: 7665 6e74 5f6e 756d 735d 0a0a 2020 2020  vent_nums]..    
+00004c20: 2020 2020 2020 2020 6966 2028 6e6f 7420          if (not 
+00004c30: 6973 696e 7374 616e 6365 2873 6572 6965  isinstance(serie
+00004c40: 735f 6e75 6d73 2c20 6c69 7374 290a 2020  s_nums, list).  
+00004c50: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00004c60: 6420 6e6f 7420 6973 696e 7374 616e 6365  d not isinstance
+00004c70: 2873 6572 6965 735f 6e75 6d73 2c20 6e70  (series_nums, np
+00004c80: 2e6e 6461 7272 6179 2929 3a0a 2020 2020  .ndarray)):.    
+00004c90: 2020 2020 2020 2020 2020 2020 7365 7269              seri
+00004ca0: 6573 5f6e 756d 7320 3d20 5b73 6572 6965  es_nums = [serie
+00004cb0: 735f 6e75 6d73 5d0a 2020 2020 2020 2020  s_nums].        
+00004cc0: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+00004cd0: 6572 6965 735f 6e75 6d73 293d 3d31 2061  eries_nums)==1 a
+00004ce0: 6e64 206c 656e 2865 7665 6e74 5f6e 756d  nd len(event_num
+00004cf0: 7329 3e31 3a0a 2020 2020 2020 2020 2020  s)>1:.          
+00004d00: 2020 2020 2020 2020 2020 7365 7269 6573            series
+00004d10: 5f6e 756d 7320 2a3d 206c 656e 2865 7665  _nums *= len(eve
+00004d20: 6e74 5f6e 756d 7329 0a20 2020 2020 2020  nt_nums).       
+00004d30: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00004d40: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00004d50: 2020 2020 2020 2069 6620 286c 656e 2865         if (len(e
+00004d60: 7665 6e74 5f6e 756d 7329 213d 6c65 6e28  vent_nums)!=len(
+00004d70: 7365 7269 6573 5f6e 756d 7329 293a 0a20  series_nums)):. 
+00004d80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004d90: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00004da0: 2745 5252 4f52 3a20 2273 6572 6965 735f  'ERROR: "series_
+00004db0: 6e75 6d73 2220 616e 6420 2265 7665 6e74  nums" and "event
+00004dc0: 5f6e 756d 7322 2027 0a20 2020 2020 2020  _nums" '.       
+00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004de0: 2020 2020 2020 2020 2020 2b20 276e 6565            + 'nee
+00004df0: 6420 746f 2062 6520 7361 6d65 206c 656e  d to be same len
+00004e00: 6774 6821 2729 0a0a 2020 2020 2020 2020  gth!')..        
+00004e10: 2020 2020 6966 2074 7269 6767 6572 5f69      if trigger_i
+00004e20: 6e64 6963 6573 2069 7320 6e6f 7420 4e6f  ndices is not No
+00004e30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00004e40: 2020 2020 6966 2028 6e6f 7420 6973 696e      if (not isin
+00004e50: 7374 616e 6365 2874 7269 6767 6572 5f69  stance(trigger_i
+00004e60: 6e64 6963 6573 2c20 6c69 7374 290a 2020  ndices, list).  
+00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e80: 2020 616e 6420 6e6f 7420 6973 696e 7374    and not isinst
+00004e90: 616e 6365 2874 7269 6767 6572 5f69 6e64  ance(trigger_ind
+00004ea0: 6963 6573 2c20 6e70 2e6e 6461 7272 6179  ices, np.ndarray
+00004eb0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00004ec0: 2020 2020 2020 2020 7472 6967 6765 725f          trigger_
+00004ed0: 696e 6469 6365 7320 3d20 5b74 7269 6767  indices = [trigg
+00004ee0: 6572 5f69 6e64 6963 6573 5d0a 2020 2020  er_indices].    
+00004ef0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00004f00: 6c65 6e28 6576 656e 745f 6e75 6d73 2921  len(event_nums)!
+00004f10: 3d6c 656e 2874 7269 6767 6572 5f69 6e64  =len(trigger_ind
+00004f20: 6963 6573 2929 3a0a 2020 2020 2020 2020  ices)):.        
+00004f30: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00004f40: 6520 5661 6c75 6545 7272 6f72 2827 4552  e ValueError('ER
+00004f50: 524f 523a 2022 7472 6967 6765 725f 696e  ROR: "trigger_in
+00004f60: 6469 6365 7322 2061 6e64 2022 6576 656e  dices" and "even
+00004f70: 745f 6e75 6d73 2220 270a 2020 2020 2020  t_nums" '.      
+00004f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f90: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00004fa0: 2027 6e65 6564 2074 6f20 6265 2073 616d   'need to be sam
+00004fb0: 6520 6c65 6e67 7468 2127 290a 2020 2020  e length!').    
+00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004fe0: 200a 2020 2020 2020 2020 2020 2020 2320   .            # 
+00004ff0: 636f 6e76 6572 7420 746f 206c 6973 7420  convert to list 
+00005000: 6f66 2064 6963 7469 6f6e 6172 6965 730a  of dictionaries.
+00005010: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00005020: 745f 6c69 7374 203d 206c 6973 7428 290a  t_list = list().
+00005030: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00005040: 6965 7665 6e74 2020 696e 2072 616e 6765  ievent  in range
+00005050: 286c 656e 2865 7665 6e74 5f6e 756d 7329  (len(event_nums)
+00005060: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00005070: 2020 2065 7665 6e74 5f64 6963 7420 3d20     event_dict = 
+00005080: 7b27 6576 656e 745f 6e75 6d62 6572 273a  {'event_number':
+00005090: 2065 7665 6e74 5f6e 756d 735b 6965 7665   event_nums[ieve
+000050a0: 6e74 5d2c 0a20 2020 2020 2020 2020 2020  nt],.           
+000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050c0: 2020 2027 7365 7269 6573 5f6e 756d 6265     'series_numbe
+000050d0: 7227 3a20 7365 7269 6573 5f6e 756d 735b  r': series_nums[
+000050e0: 6965 7665 6e74 5d7d 0a0a 2020 2020 2020  ievent]}..      
+000050f0: 2020 2020 2020 2020 2020 6966 2074 7269            if tri
+00005100: 6767 6572 5f69 6e64 6963 6573 2069 7320  gger_indices is 
+00005110: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00005120: 2020 2020 2020 2020 2020 2020 2020 6576                ev
+00005130: 656e 745f 6469 6374 5b27 7472 6967 6765  ent_dict['trigge
+00005140: 725f 696e 6465 7827 5d20 3d20 7472 6967  r_index'] = trig
+00005150: 6765 725f 696e 6469 6365 735b 6965 7665  ger_indices[ieve
+00005160: 6e74 5d0a 2020 2020 2020 2020 2020 2020  nt].            
+00005170: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005180: 2020 2020 2020 2020 2065 7665 6e74 5f6c           event_l
+00005190: 6973 742e 6170 7065 6e64 2865 7665 6e74  ist.append(event
+000051a0: 5f64 6963 7429 0a20 2020 2020 2020 2020  _dict).         
+000051b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000051c0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+000051d0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+000051e0: 2020 2020 2020 2320 7365 7420 6669 6c65        # set file
+000051f0: 730a 2020 2020 2020 2020 6669 6c65 5f70  s.        file_p
+00005200: 6174 6820 3d20 6c69 7374 2873 656c 662e  ath = list(self.
+00005210: 5f66 696c 655f 6469 6374 2e6b 6579 7328  _file_dict.keys(
+00005220: 2929 0a20 2020 2020 2020 2069 6620 6669  )).        if fi
+00005230: 6c65 7061 7468 2069 7320 6e6f 7420 4e6f  lepath is not No
+00005240: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00005250: 6669 6c65 5f70 6174 6820 3d20 6669 6c65  file_path = file
+00005260: 7061 7468 0a20 2020 2020 2020 2073 656c  path.        sel
+00005270: 662e 7365 745f 6669 6c65 7328 6669 6c65  f.set_files(file
+00005280: 5f70 6174 682c 2073 6572 6965 733d 7365  _path, series=se
+00005290: 7269 6573 5f6e 756d 732c 0a20 2020 2020  ries_nums,.     
+000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052b0: 2020 6576 656e 745f 6c69 7374 3d65 7665    event_list=eve
+000052c0: 6e74 5f6c 6973 7429 0a20 2020 2020 2020  nt_list).       
+000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005300: 2020 2b20 7374 7228 6576 656e 745f 6e75    + str(event_nu
-00005310: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
-00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005330: 2020 2020 2020 2020 2020 2020 2b20 2720              + ' 
-00005340: 686f 7765 7665 722c 2065 7665 6e74 2064  however, event d
-00005350: 6f65 7320 6e6f 7420 6578 6973 7421 2729  oes not exist!')
-00005360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005370: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00005380: 2020 2020 2020 2020 2020 2320 7374 6f72            # stor
-00005390: 6520 696e 206c 6973 7420 6173 2061 2074  e in list as a t
-000053a0: 7570 6c65 0a20 2020 2020 2020 2020 2020  uple.           
-000053b0: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
-000053c0: 645f 6576 656e 745f 6669 6c65 732e 6170  d_event_files.ap
-000053d0: 7065 6e64 2828 6576 656e 745f 696e 6465  pend((event_inde
-000053e0: 782c 2066 696c 655f 6e61 6d65 2929 0a0a  x, file_name))..
-000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005400: 2020 2020 2320 696e 6372 656d 656e 7420      # increment 
-00005410: 746f 7420 6e75 6d62 6572 206f 6620 6576  tot number of ev
-00005420: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-00005430: 2020 2020 2020 2020 206e 625f 6576 656e           nb_even
-00005440: 7473 5f74 6f74 202b 3d20 310a 2020 2020  ts_tot += 1.    
-00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005460: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005470: 2020 2320 636f 6e74 696e 7565 2066 696c    # continue fil
-00005480: 6520 6c6f 6f70 2069 6620 6e6f 7420 6e65  e loop if not ne
-00005490: 6564 6564 0a20 2020 2020 2020 2020 2020  eded.           
-000054a0: 2020 2020 2069 6620 6e6f 7420 6b65 6570       if not keep
-000054b0: 5f66 696c 6520 3a0a 2020 2020 2020 2020  _file :.        
-000054c0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000054d0: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
-000054e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000054f0: 2020 2020 2020 2020 6e62 5f65 7665 6e74          nb_event
-00005500: 735f 746f 7420 2b3d 2061 6463 5f6d 6574  s_tot += adc_met
-00005510: 6164 6174 615b 276e 625f 6576 656e 7473  adata['nb_events
-00005520: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
-00005530: 2020 2069 6620 6e65 7665 6e74 733e 3020     if nevents>0 
-00005540: 2061 6e64 206e 625f 6576 656e 7473 5f74   and nb_events_t
-00005550: 6f74 3e3d 6e65 7665 6e74 733a 0a20 2020  ot>=nevents:.   
-00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005570: 206e 625f 6576 656e 7473 5f74 6f74 203d   nb_events_tot =
-00005580: 206e 6576 656e 7473 0a20 2020 2020 2020   nevents.       
-00005590: 2020 2020 2020 2020 200a 0a20 2020 2020           ..     
-000055a0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-000055b0: 2020 2023 2063 6865 636b 2063 6861 6e6e     # check chann
-000055c0: 656c 730a 2020 2020 2020 2020 2020 2020  els.            
-000055d0: 6e62 5f63 6861 6e6e 656c 735f 6669 6c65  nb_channels_file
-000055e0: 203d 2061 6463 5f6d 6574 6164 6174 615b   = adc_metadata[
-000055f0: 276e 625f 6368 616e 6e65 6c73 275d 0a20  'nb_channels']. 
-00005600: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00005610: 2020 2020 6966 2064 6574 6563 746f 725f      if detector_
-00005620: 6368 616e 7320 6973 206e 6f74 204e 6f6e  chans is not Non
-00005630: 653a 0a0a 2020 2020 2020 2020 2020 2020  e:..            
-00005640: 2020 2020 2320 636f 6e6e 6563 7469 6f6e      # connection
-00005650: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00005660: 2020 636f 6e6e 6563 7469 6f6e 7320 3d20    connections = 
-00005670: 7365 6c66 2e67 6574 5f63 6f6e 6e65 6374  self.get_connect
-00005680: 696f 6e5f 6469 6374 2861 6463 5f6e 616d  ion_dict(adc_nam
-00005690: 653d 6164 635f 6e61 6d65 2c0a 2020 2020  e=adc_name,.    
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005300: 2320 7365 7420 6669 6c65 206c 6973 740a  # set file list.
+00005310: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00005320: 656c 662e 5f66 696c 655f 6469 6374 3a0a  elf._file_dict:.
+00005330: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00005340: 6520 5661 6c75 6545 7272 6f72 2827 4552  e ValueError('ER
+00005350: 524f 523a 204e 6f20 6669 6c65 7320 7365  ROR: No files se
+00005360: 6c65 6374 6564 2127 290a 2020 2020 2020  lected!').      
+00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005380: 2020 0a0a 2020 2020 0a20 2020 2020 2020    ..    .       
+00005390: 0a20 2020 2020 2020 2023 203d 3d3d 3d3d  .        # =====
+000053a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000053b0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2020  ==========.     
+000053c0: 2020 2023 2043 6865 636b 2072 6177 2064     # Check raw d
+000053d0: 6174 610a 2020 2020 2020 2020 2320 3d3d  ata.        # ==
+000053e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000053f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
+00005400: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00005410: 2069 6e69 7469 616c 697a 6520 7573 6566   initialize usef
+00005420: 756c 2070 6172 616d 6574 6572 730a 2020  ul parameters.  
+00005430: 2020 2020 2020 6e62 5f65 7665 6e74 735f        nb_events_
+00005440: 746f 7420 3d20 300a 2020 2020 2020 2020  tot = 0.        
+00005450: 6e62 5f63 6861 6e6e 656c 7320 3d20 300a  nb_channels = 0.
+00005460: 2020 2020 2020 2020 6e62 5f73 616d 706c          nb_sampl
+00005470: 6573 203d 2030 0a0a 2020 2020 2020 2020  es = 0..        
+00005480: 0a20 2020 2020 2020 2023 206c 6f6f 7020  .        # loop 
+00005490: 6669 6c65 7320 616e 6420 6368 6563 6b20  files and check 
+000054a0: 6e75 6d62 6572 206f 6620 6368 616e 6e65  number of channe
+000054b0: 6c73 2f65 7665 6e74 732f 7361 6d70 6c65  ls/events/sample
+000054c0: 730a 2020 2020 2020 2020 666f 7220 6669  s.        for fi
+000054d0: 6c65 5f6e 616d 652c 2066 696c 655f 6c69  le_name, file_li
+000054e0: 7374 2069 6e20 7365 6c66 2e5f 6669 6c65  st in self._file
+000054f0: 5f64 6963 742e 6974 656d 7328 293a 0a20  _dict.items():. 
+00005500: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00005510: 2020 2020 2020 2020 2320 6765 7420 6d65          # get me
+00005520: 7461 6461 7461 0a20 2020 2020 2020 2020  tadata.         
+00005530: 2020 206d 6574 6164 6174 6120 3d20 7365     metadata = se
+00005540: 6c66 2e67 6574 5f6d 6574 6164 6174 6128  lf.get_metadata(
+00005550: 6669 6c65 5f6e 616d 6529 0a20 2020 2020  file_name).     
+00005560: 2020 2020 2020 2061 6463 5f6d 6574 6164         adc_metad
+00005570: 6174 6120 3d20 6d65 7461 6461 7461 5b27  ata = metadata['
+00005580: 6772 6f75 7073 275d 5b61 6463 5f6e 616d  groups'][adc_nam
+00005590: 655d 0a0a 2020 2020 2020 2020 2020 2020  e]..            
+000055a0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+000055b0: 6865 636b 2063 6861 6e6e 656c 730a 2020  heck channels.  
+000055c0: 2020 2020 2020 2020 2020 6e62 5f63 6861            nb_cha
+000055d0: 6e6e 656c 735f 6669 6c65 203d 2061 6463  nnels_file = adc
+000055e0: 5f6d 6574 6164 6174 615b 276e 625f 6368  _metadata['nb_ch
+000055f0: 616e 6e65 6c73 275d 2020 2020 200a 2020  annels']     .  
+00005600: 2020 2020 2020 2020 2020 6966 2064 6574            if det
+00005610: 6563 746f 725f 6368 616e 7320 6973 206e  ector_chans is n
+00005620: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00005630: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00005640: 2020 2020 2020 2020 2020 2320 636f 6e6e            # conn
+00005650: 6563 7469 6f6e 730a 2020 2020 2020 2020  ections.        
+00005660: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
+00005670: 6f6e 7320 3d20 7365 6c66 2e67 6574 5f63  ons = self.get_c
+00005680: 6f6e 6e65 6374 696f 6e5f 6469 6374 2861  onnection_dict(a
+00005690: 6463 5f6e 616d 653d 6164 635f 6e61 6d65  dc_name=adc_name
+000056a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056d0: 2020 206d 6574 6164 6174 613d 6d65 7461     metadata=meta
-000056e0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
+000056d0: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+000056e0: 613d 6d65 7461 6461 7461 290a 2020 2020  a=metadata).    
 000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00005710: 2020 2020 2020 2023 206c 6f6f 7020 6368         # loop ch
-00005720: 616e 6e65 6c73 0a20 2020 2020 2020 2020  annels.         
-00005730: 2020 2020 2020 206e 625f 6368 616e 6e65         nb_channe
-00005740: 6c73 5f66 696c 6520 203d 2030 0a20 2020  ls_file  = 0.   
-00005750: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00005760: 2063 6861 6e5f 6e61 6d65 2069 6e20 636f   chan_name in co
-00005770: 6e6e 6563 7469 6f6e 735b 2764 6574 6563  nnections['detec
-00005780: 746f 725f 6368 616e 7327 5d3a 0a20 2020  tor_chans']:.   
-00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057a0: 2069 6620 6368 616e 5f6e 616d 6520 696e   if chan_name in
-000057b0: 2064 6574 6563 746f 725f 6368 616e 733a   detector_chans:
-000057c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057d0: 2020 2020 2020 2020 206e 625f 6368 616e           nb_chan
-000057e0: 6e65 6c73 5f66 696c 6520 2b3d 310a 0a20  nels_file +=1.. 
-000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005800: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00005810: 2020 2020 2020 2020 2320 6572 726f 7220          # error 
-00005820: 6966 206e 6f20 6368 616e 6e65 6c20 666f  if no channel fo
-00005830: 756e 640a 2020 2020 2020 2020 2020 2020  und.            
-00005840: 2020 2020 6966 2028 6e62 5f63 6861 6e6e      if (nb_chann
-00005850: 656c 735f 6669 6c65 3d3d 3029 3a0a 2020  els_file==0):.  
-00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005870: 2020 6572 726f 725f 6d73 6720 3d20 2827    error_msg = ('
-00005880: 556e 6162 6c65 2074 6f20 6669 6e64 2073  Unable to find s
-00005890: 656c 6563 7465 6420 6368 616e 6e65 6c28  elected channel(
-000058a0: 7329 2e27 0a20 2020 2020 2020 2020 2020  s).'.           
-000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058c0: 2020 2020 2020 2b20 2720 4368 6563 6b20        + ' Check 
-000058d0: 636f 6e6e 6563 7469 6f6e 2074 6162 6c65  connection table
-000058e0: 2127 290a 2020 2020 2020 2020 2020 2020  !').            
-000058f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00005900: 5f72 6169 7365 5f65 7272 6f72 733a 0a20  _raise_errors:. 
+00005700: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00005710: 2020 2020 2020 2020 2020 2020 2023 206c               # l
+00005720: 6f6f 7020 6368 616e 6e65 6c73 0a20 2020  oop channels.   
+00005730: 2020 2020 2020 2020 2020 2020 206e 625f               nb_
+00005740: 6368 616e 6e65 6c73 5f66 696c 6520 203d  channels_file  =
+00005750: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
+00005760: 2020 2066 6f72 2063 6861 6e5f 6e61 6d65     for chan_name
+00005770: 2069 6e20 636f 6e6e 6563 7469 6f6e 735b   in connections[
+00005780: 2764 6574 6563 746f 725f 6368 616e 7327  'detector_chans'
+00005790: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+000057a0: 2020 2020 2020 2069 6620 6368 616e 5f6e         if chan_n
+000057b0: 616d 6520 696e 2064 6574 6563 746f 725f  ame in detector_
+000057c0: 6368 616e 733a 0a20 2020 2020 2020 2020  chans:.         
+000057d0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000057e0: 625f 6368 616e 6e65 6c73 5f66 696c 6520  b_channels_file 
+000057f0: 2b3d 310a 0a20 2020 2020 2020 2020 2020  +=1..           
+00005800: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00005810: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00005820: 6572 726f 7220 6966 206e 6f20 6368 616e  error if no chan
+00005830: 6e65 6c20 666f 756e 640a 2020 2020 2020  nel found.      
+00005840: 2020 2020 2020 2020 2020 6966 2028 6e62            if (nb
+00005850: 5f63 6861 6e6e 656c 735f 6669 6c65 3d3d  _channels_file==
+00005860: 3029 3a0a 2020 2020 2020 2020 2020 2020  0):.            
+00005870: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
+00005880: 6172 2829 0a20 2020 2020 2020 2020 2020  ar().           
+00005890: 2020 2020 2020 2020 2073 656c 662e 5f66           self._f
+000058a0: 696c 655f 6469 6374 203d 2063 7572 7265  ile_dict = curre
+000058b0: 6e74 5f66 696c 655f 6469 6374 0a20 2020  nt_file_dict.   
+000058c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058d0: 2065 7272 6f72 5f6d 7367 203d 2028 2755   error_msg = ('U
+000058e0: 6e61 626c 6520 746f 2066 696e 6420 7365  nable to find se
+000058f0: 6c65 6374 6564 2063 6861 6e6e 656c 2873  lected channel(s
+00005900: 292e 270a 2020 2020 2020 2020 2020 2020  ).'.            
 00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005920: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00005930: 7565 4572 726f 7228 6572 726f 725f 6d73  ueError(error_ms
-00005940: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
-00005950: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005970: 2020 2020 2070 7269 6e74 2827 4552 524f       print('ERRO
-00005980: 523a 2027 202b 2065 7272 6f72 5f6d 7367  R: ' + error_msg
-00005990: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000059a0: 2020 2020 2020 2020 2020 6966 2069 6e63            if inc
-000059b0: 6c75 6465 5f6d 6574 6164 6174 613a 0a20  lude_metadata:. 
+00005920: 2020 2020 202b 2027 2043 6865 636b 2063       + ' Check c
+00005930: 6f6e 6e65 6374 696f 6e20 7461 626c 6521  onnection table!
+00005940: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00005950: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+00005960: 7261 6973 655f 6572 726f 7273 3a0a 2020  raise_errors:.  
+00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005980: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00005990: 6545 7272 6f72 2865 7272 6f72 5f6d 7367  eError(error_msg
+000059a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000059b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000059e0: 6e20 5b5d 2c5b 5d0a 2020 2020 2020 2020  n [],[].        
-000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a20: 2020 7265 7475 726e 205b 5d0a 2020 2020    return [].    
-00005a30: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
-00005a40: 2020 2020 2020 6966 206e 625f 6368 616e        if nb_chan
-00005a50: 6e65 6c73 3d3d 303a 0a20 2020 2020 2020  nels==0:.       
-00005a60: 2020 2020 2020 2020 206e 625f 6368 616e           nb_chan
-00005a70: 6e65 6c73 203d 2020 6e62 5f63 6861 6e6e  nels =  nb_chann
-00005a80: 656c 735f 6669 6c65 0a20 2020 2020 2020  els_file.       
-00005a90: 2020 2020 2065 6c69 6620 6e62 5f63 6861       elif nb_cha
-00005aa0: 6e6e 656c 7321 3d6e 625f 6368 616e 6e65  nnels!=nb_channe
-00005ab0: 6c73 5f66 696c 653a 0a20 2020 2020 2020  ls_file:.       
-00005ac0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00005ad0: 616c 7565 4572 726f 7228 2745 5252 4f52  alueError('ERROR
-00005ae0: 3a20 696e 636f 6e73 6973 7465 6e74 206e  : inconsistent n
-00005af0: 756d 6265 7220 270a 2020 2020 2020 2020  umber '.        
-00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b10: 2020 2020 2020 2020 202b 2027 6f66 2063           + 'of c
-00005b20: 6861 6e6e 656c 7320 6265 7477 6565 6e20  hannels between 
-00005b30: 6669 6c65 7321 2729 0a20 2020 2020 2020  files!').       
-00005b40: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b60: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00005b70: 2020 2023 206e 756d 6265 7220 6f66 2073     # number of s
-00005b80: 616d 706c 6573 0a20 2020 2020 2020 2020  amples.         
-00005b90: 2020 206e 625f 7361 6d70 6c65 735f 6669     nb_samples_fi
-00005ba0: 6c65 203d 2061 6463 5f6d 6574 6164 6174  le = adc_metadat
-00005bb0: 615b 276e 625f 7361 6d70 6c65 7327 5d20  a['nb_samples'] 
-00005bc0: 2020 0a20 2020 2020 2020 2020 2020 2069    .            i
-00005bd0: 6620 6e62 5f73 616d 706c 6573 3d3d 303a  f nb_samples==0:
-00005be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005bf0: 206e 625f 7361 6d70 6c65 7320 3d20 206e   nb_samples =  n
-00005c00: 625f 7361 6d70 6c65 735f 6669 6c65 0a20  b_samples_file. 
-00005c10: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00005c20: 206f 7574 7075 745f 666f 726d 6174 213d   output_format!=
-00005c30: 3120 616e 6420 6e62 5f73 616d 706c 6573  1 and nb_samples
-00005c40: 5f66 696c 6521 3d6e 625f 7361 6d70 6c65  _file!=nb_sample
-00005c50: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00005c60: 2020 2065 7272 6f72 5f6d 7367 203d 2027     error_msg = '
-00005c70: 556e 6162 6c65 2074 6f20 7265 7475 726e  Unable to return
-00005c80: 2033 4420 6172 7272 6179 2064 7565 2074   3D arrray due t
-00005c90: 6f20 696e 636f 6e73 6973 7465 6e74 206e  o inconsistent n
-00005ca0: 6220 6f66 2073 616d 706c 6573 2127 0a20  b of samples!'. 
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005cc0: 6620 7365 6c66 2e5f 7261 6973 655f 6572  f self._raise_er
-00005cd0: 726f 7273 3a0a 2020 2020 2020 2020 2020  rors:.          
-00005ce0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00005cf0: 5661 6c75 6545 7272 6f72 2865 7272 6f72  ValueError(error
-00005d00: 5f6d 7367 290a 2020 2020 2020 2020 2020  _msg).          
-00005d10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d30: 7072 696e 7428 2745 5252 4f52 3a20 2720  print('ERROR: ' 
-00005d40: 2b20 6572 726f 725f 6d73 6729 0a20 2020  + error_msg).   
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d60: 2070 7269 6e74 2827 5573 6520 6f75 7470   print('Use outp
-00005d70: 7574 3d31 2028 6576 656e 7420 6c69 7374  ut=1 (event list
-00005d80: 2920 696e 7374 6561 6420 6f72 2063 6865  ) instead or che
-00005d90: 636b 2066 696c 6573 2729 0a20 2020 2020  ck files').     
-00005da0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005db0: 6620 696e 636c 7564 655f 6d65 7461 6461  f include_metada
-00005dc0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00005dd0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00005de0: 726e 205b 5d2c 5b5d 0a20 2020 2020 2020  rn [],[].       
-00005df0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00005e00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00005e10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00005e20: 6e20 5b5d 0a0a 2020 2020 2020 2020 2020  n []..          
-00005e30: 2020 2320 6368 6563 6b20 6d61 7820 6576    # check max ev
-00005e40: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-00005e50: 2069 6620 286e 6576 656e 7473 3e30 2020   if (nevents>0  
-00005e60: 616e 6420 6e62 5f65 7665 6e74 735f 746f  and nb_events_to
-00005e70: 743e 3d6e 6576 656e 7473 293a 0a20 2020  t>=nevents):.   
-00005e80: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00005e90: 616b 0a0a 2020 2020 2020 2020 2020 2020  ak..            
-00005ea0: 0a20 2020 2020 2020 2023 2063 6c65 6172  .        # clear
-00005eb0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
-00005ec0: 6561 7228 290a 0a0a 2020 2020 2020 2020  ear()...        
-00005ed0: 2320 6368 6563 6b20 6e75 6d62 6572 206f  # check number o
-00005ee0: 6620 6576 656e 7473 0a20 2020 2020 2020  f events.       
-00005ef0: 2069 6620 6e62 5f65 7665 6e74 735f 746f   if nb_events_to
-00005f00: 7420 3d3d 2030 3a0a 2020 2020 2020 2020  t == 0:.        
-00005f10: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00005f20: 7272 6f72 2827 4552 524f 523a 204e 6f20  rror('ERROR: No 
-00005f30: 6576 656e 7473 2066 6f75 6e64 2127 290a  events found!').
-00005f40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00005f50: 2069 6620 2865 7665 6e74 5f6e 756d 7320   if (event_nums 
-00005f60: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-00005f70: 2020 2020 2020 2020 616e 6420 6e62 5f65          and nb_e
-00005f80: 7665 6e74 735f 746f 743c 6c65 6e28 6576  vents_tot<len(ev
-00005f90: 656e 745f 6e75 6d73 2929 3a0a 2020 2020  ent_nums)):.    
-00005fa0: 2020 2020 2020 2020 7072 696e 7428 2757          print('W
-00005fb0: 4152 4e49 4e47 3a20 4f6e 6c79 2027 202b  ARNING: Only ' +
-00005fc0: 2073 7472 286e 625f 6576 656e 7473 5f74   str(nb_events_t
-00005fd0: 6f74 290a 2020 2020 2020 2020 2020 2020  ot).            
-00005fe0: 2020 2020 2020 2b20 2720 6576 656e 7473        + ' events
-00005ff0: 206f 7574 206f 6620 270a 2020 2020 2020   out of '.      
-00006000: 2020 2020 2020 2020 2020 2020 2b20 7374              + st
-00006010: 7228 6c65 6e28 6576 656e 745f 6e75 6d73  r(len(event_nums
-00006020: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00006030: 2020 2020 202b 2027 2068 6176 6520 6265       + ' have be
-00006040: 656e 2066 6f75 6e64 2127 290a 2020 2020  en found!').    
-00006050: 2020 2020 2020 2020 0a20 2020 200a 0a0a          .    ...
-00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006070: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006080: 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    # ============
-00006090: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000060a0: 3d3d 3d0a 2020 2020 2020 2020 2320 4d65  ===.        # Me
-000060b0: 6d6f 7279 2063 6865 636b 0a20 2020 2020  mory check.     
-000060c0: 2020 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d     # ===========
-000060d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000060e0: 3d3d 3d3d 0a20 2020 2020 2020 2020 2020  ====.           
-000060f0: 2020 2020 200a 2020 2020 2020 2020 7361       .        sa
-00006100: 6d70 6c65 5f62 7974 6573 203d 2032 0a20  mple_bytes = 2. 
-00006110: 2020 2020 2020 2069 6620 6164 6374 6f76         if adctov
-00006120: 6f6c 7420 6f72 2061 6463 746f 616d 7020  olt or adctoamp 
-00006130: 6f72 2062 6173 656c 696e 6573 7562 3a0a  or baselinesub:.
-00006140: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
-00006150: 6c65 5f62 7974 6573 203d 2038 0a20 2020  le_bytes = 8.   
-00006160: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00006170: 2020 6f75 7470 7574 5f6d 656d 6f72 795f    output_memory_
-00006180: 7065 725f 6576 656e 7420 3d20 7361 6d70  per_event = samp
-00006190: 6c65 5f62 7974 6573 2a6e 625f 7361 6d70  le_bytes*nb_samp
-000061a0: 6c65 732a 6e62 5f63 6861 6e6e 656c 732f  les*nb_channels/
-000061b0: 3165 390a 2020 2020 2020 2020 6f75 7470  1e9.        outp
-000061c0: 7574 5f6d 656d 6f72 7920 3d20 6e62 5f65  ut_memory = nb_e
-000061d0: 7665 6e74 735f 746f 742a 6f75 7470 7574  vents_tot*output
-000061e0: 5f6d 656d 6f72 795f 7065 725f 6576 656e  _memory_per_even
-000061f0: 740a 2020 2020 2020 2020 6966 206f 7574  t.        if out
-00006200: 7075 745f 6d65 6d6f 7279 3e6d 656d 6f72  put_memory>memor
-00006210: 795f 6c69 6d69 743a 0a20 2020 2020 2020  y_limit:.       
-00006220: 2020 2020 206e 625f 6576 656e 7473 5f74       nb_events_t
-00006230: 6f74 5f74 656d 7020 3d20 696e 7428 726f  ot_temp = int(ro
-00006240: 756e 6428 6d65 6d6f 7279 5f6c 696d 6974  und(memory_limit
-00006250: 2f6f 7574 7075 745f 6d65 6d6f 7279 5f70  /output_memory_p
-00006260: 6572 5f65 7665 6e74 2929 0a20 2020 2020  er_event)).     
-00006270: 2020 2020 2020 2070 7269 6e74 2827 5741         print('WA
-00006280: 524e 494e 473a 204d 6178 206e 756d 6265  RNING: Max numbe
-00006290: 7220 6576 656e 7473 2062 6173 6564 206f  r events based o
-000062a0: 6e20 6d65 6d6f 7279 206c 696d 6974 206f  n memory limit o
-000062b0: 6620 270a 2020 2020 2020 2020 2020 2020  f '.            
-000062c0: 2020 2020 2020 2b20 7374 7228 6d65 6d6f        + str(memo
-000062d0: 7279 5f6c 696d 6974 2920 2b20 2747 4220  ry_limit) + 'GB 
-000062e0: 6973 2027 0a20 2020 2020 2020 2020 2020  is '.           
-000062f0: 2020 2020 2020 202b 2073 7472 286e 625f         + str(nb_
-00006300: 6576 656e 7473 5f74 6f74 5f74 656d 7029  events_tot_temp)
-00006310: 202b 2027 206f 7574 206f 6620 270a 2020   + ' out of '.  
-00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006330: 2b20 7374 7228 6e62 5f65 7665 6e74 735f  + str(nb_events_
-00006340: 746f 7429 202b 2721 2729 0a20 2020 2020  tot) +'!').     
-00006350: 2020 2020 2020 206e 625f 6576 656e 7473         nb_events
-00006360: 5f74 6f74 203d 206e 625f 6576 656e 7473  _tot = nb_events
-00006370: 5f74 6f74 5f74 656d 700a 0a0a 0a0a 2020  _tot_temp.....  
-00006380: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00006390: 2020 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d     # ===========
+000059d0: 2020 2020 7072 696e 7428 2745 5252 4f52      print('ERROR
+000059e0: 3a20 2720 2b20 6572 726f 725f 6d73 6729  : ' + error_msg)
+000059f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005a00: 2020 2020 2020 2020 2069 6620 696e 636c           if incl
+00005a10: 7564 655f 6d65 7461 6461 7461 3a0a 2020  ude_metadata:.  
+00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a30: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00005a40: 205b 5d2c 5b5d 0a20 2020 2020 2020 2020   [],[].         
+00005a50: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00005a60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a80: 2072 6574 7572 6e20 5b5d 0a20 2020 2020   return [].     
+00005a90: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
+00005aa0: 2020 2020 2069 6620 6e62 5f63 6861 6e6e       if nb_chann
+00005ab0: 656c 733d 3d30 3a0a 2020 2020 2020 2020  els==0:.        
+00005ac0: 2020 2020 2020 2020 6e62 5f63 6861 6e6e          nb_chann
+00005ad0: 656c 7320 3d20 6e62 5f63 6861 6e6e 656c  els = nb_channel
+00005ae0: 735f 6669 6c65 0a20 2020 2020 2020 2020  s_file.         
+00005af0: 2020 2065 6c69 6620 6e62 5f63 6861 6e6e     elif nb_chann
+00005b00: 656c 7320 213d 206e 625f 6368 616e 6e65  els != nb_channe
+00005b10: 6c73 5f66 696c 653a 0a20 2020 2020 2020  ls_file:.       
+00005b20: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
+00005b30: 6561 7228 290a 2020 2020 2020 2020 2020  ear().          
+00005b40: 2020 2020 2020 7365 6c66 2e5f 6669 6c65        self._file
+00005b50: 5f64 6963 7420 3d20 6375 7272 656e 745f  _dict = current_
+00005b60: 6669 6c65 5f64 6963 740a 2020 2020 2020  file_dict.      
+00005b70: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00005b80: 5661 6c75 6545 7272 6f72 2827 4552 524f  ValueError('ERRO
+00005b90: 523a 2069 6e63 6f6e 7369 7374 656e 7420  R: inconsistent 
+00005ba0: 6e75 6d62 6572 2027 0a20 2020 2020 2020  number '.       
+00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bc0: 2020 2020 2020 2020 2020 2b20 276f 6620            + 'of 
+00005bd0: 6368 616e 6e65 6c73 2062 6574 7765 656e  channels between
+00005be0: 2066 696c 6573 2127 290a 2020 2020 2020   files!').      
+00005bf0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00005c00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005c10: 2020 2020 2320 6368 6563 6b20 6e75 6d62      # check numb
+00005c20: 6572 206f 6620 6576 656e 7473 3a0a 2020  er of events:.  
+00005c30: 2020 2020 2020 2020 2020 6e62 5f65 7665            nb_eve
+00005c40: 6e74 735f 6669 6c65 203d 2061 6463 5f6d  nts_file = adc_m
+00005c50: 6574 6164 6174 615b 276e 625f 6576 656e  etadata['nb_even
+00005c60: 7473 275d 0a20 2020 2020 2020 2020 2020  ts'].           
+00005c70: 2069 6620 6669 6c65 5f6c 6973 7420 6973   if file_list is
+00005c80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00005c90: 2020 2020 2020 2020 2020 206e 625f 6576             nb_ev
+00005ca0: 656e 7473 5f66 696c 6520 3d20 6c65 6e28  ents_file = len(
+00005cb0: 6669 6c65 5f6c 6973 7429 0a0a 2020 2020  file_list)..    
+00005cc0: 2020 2020 2020 2020 6e62 5f65 7665 6e74          nb_event
+00005cd0: 735f 746f 7420 2b3d 206e 625f 6576 656e  s_tot += nb_even
+00005ce0: 7473 5f66 696c 650a 2020 2020 2020 2020  ts_file.        
+00005cf0: 2020 2020 6966 206e 6576 656e 7473 3e30      if nevents>0
+00005d00: 2020 616e 6420 6e62 5f65 7665 6e74 735f    and nb_events_
+00005d10: 746f 743e 3d6e 6576 656e 7473 3a0a 2020  tot>=nevents:.  
+00005d20: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
+00005d30: 5f65 7665 6e74 735f 746f 7420 3d20 6e65  _events_tot = ne
+00005d40: 7665 6e74 730a 0a20 2020 2020 2020 2020  vents..         
+00005d50: 2020 2020 2020 2020 2020 2020 2020 200a                 .
+00005d60: 2020 2020 2020 2020 2020 2020 2320 6368              # ch
+00005d70: 6563 6b20 6e75 6d62 6572 206f 6620 7361  eck number of sa
+00005d80: 6d70 6c65 730a 2020 2020 2020 2020 2020  mples.          
+00005d90: 2020 6e62 5f73 616d 706c 6573 5f66 696c    nb_samples_fil
+00005da0: 6520 3d20 6164 635f 6d65 7461 6461 7461  e = adc_metadata
+00005db0: 5b27 6e62 5f73 616d 706c 6573 275d 0a0a  ['nb_samples']..
+00005dc0: 2020 2020 2020 2020 2020 2020 2320 7573              # us
+00005dd0: 6572 2073 656c 6563 7465 6420 6e62 2073  er selected nb s
+00005de0: 616d 706c 6573 0a20 2020 2020 2020 2020  amples.         
+00005df0: 2020 2066 7320 3d20 6164 635f 6d65 7461     fs = adc_meta
+00005e00: 6461 7461 5b27 7361 6d70 6c65 5f72 6174  data['sample_rat
+00005e10: 6527 5d0a 2020 2020 2020 2020 2020 2020  e'].            
+00005e20: 6966 2074 7261 6365 5f6c 656e 6774 685f  if trace_length_
+00005e30: 7361 6d70 6c65 7320 6973 206e 6f74 204e  samples is not N
+00005e40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00005e50: 2020 2020 206e 625f 7361 6d70 6c65 735f       nb_samples_
+00005e60: 6669 6c65 203d 2074 7261 6365 5f6c 656e  file = trace_len
+00005e70: 6774 685f 7361 6d70 6c65 730a 2020 2020  gth_samples.    
+00005e80: 2020 2020 2020 2020 656c 6966 2074 7261          elif tra
+00005e90: 6365 5f6c 656e 6774 685f 6d73 6563 2069  ce_length_msec i
+00005ea0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00005eb0: 2020 2020 2020 2020 2020 2020 6e62 5f73              nb_s
+00005ec0: 616d 706c 6573 5f66 696c 6520 3d20 696e  amples_file = in
+00005ed0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00005ee0: 2020 2020 2020 2066 732a 7472 6163 655f         fs*trace_
+00005ef0: 6c65 6e67 7468 5f6d 7365 632f 3130 3030  length_msec/1000
+00005f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005f10: 2029 0a20 2020 2020 2020 2020 2020 200a   ).            .
+00005f20: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00005f30: 625f 7361 6d70 6c65 733d 3d30 3a0a 2020  b_samples==0:.  
+00005f40: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
+00005f50: 5f73 616d 706c 6573 203d 206e 625f 7361  _samples = nb_sa
+00005f60: 6d70 6c65 735f 6669 6c65 0a20 2020 2020  mples_file.     
+00005f70: 2020 2020 2020 2065 6c69 6620 206f 7574         elif  out
+00005f80: 7075 745f 666f 726d 6174 213d 3120 616e  put_format!=1 an
+00005f90: 6420 6e62 5f73 616d 706c 6573 5f66 696c  d nb_samples_fil
+00005fa0: 6521 3d6e 625f 7361 6d70 6c65 733a 0a20  e!=nb_samples:. 
+00005fb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005fc0: 656c 662e 636c 6561 7228 290a 2020 2020  elf.clear().    
+00005fd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005fe0: 2e5f 6669 6c65 5f64 6963 7420 3d20 6375  ._file_dict = cu
+00005ff0: 7272 656e 745f 6669 6c65 5f64 6963 740a  rrent_file_dict.
+00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006010: 6572 726f 725f 6d73 6720 3d20 2755 6e61  error_msg = 'Una
+00006020: 626c 6520 746f 2072 6574 7572 6e20 3344  ble to return 3D
+00006030: 2061 7272 7261 7920 6475 6520 746f 2069   arrray due to i
+00006040: 6e63 6f6e 7369 7374 656e 7420 6e62 206f  nconsistent nb o
+00006050: 6620 7361 6d70 6c65 7321 270a 2020 2020  f samples!'.    
+00006060: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00006070: 656c 662e 5f72 6169 7365 5f65 7272 6f72  elf._raise_error
+00006080: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00006090: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+000060a0: 7565 4572 726f 7228 6572 726f 725f 6d73  ueError(error_ms
+000060b0: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
+000060c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000060d0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000060e0: 6e74 2827 4552 524f 523a 2027 202b 2065  nt('ERROR: ' + e
+000060f0: 7272 6f72 5f6d 7367 290a 2020 2020 2020  rror_msg).      
+00006100: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00006110: 696e 7428 2755 7365 206f 7574 7075 743d  int('Use output=
+00006120: 3120 2865 7665 6e74 206c 6973 7429 2069  1 (event list) i
+00006130: 6e73 7465 6164 206f 7220 6368 6563 6b20  nstead or check 
+00006140: 6669 6c65 7327 290a 2020 2020 2020 2020  files').        
+00006150: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00006160: 6e63 6c75 6465 5f6d 6574 6164 6174 613a  nclude_metadata:
+00006170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006180: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006190: 5b5d 2c5b 5d0a 2020 2020 2020 2020 2020  [],[].          
+000061a0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000061b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061c0: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+000061d0: 5d0a 0a20 2020 2020 2020 2020 2020 2023  ]..            #
+000061e0: 2063 6865 636b 206d 6178 2065 7665 6e74   check max event
+000061f0: 730a 2020 2020 2020 2020 2020 2020 6966  s.            if
+00006200: 2028 6e65 7665 6e74 733e 3020 2061 6e64   (nevents>0  and
+00006210: 206e 625f 6576 656e 7473 5f74 6f74 3e3d   nb_events_tot>=
+00006220: 6e65 7665 6e74 7329 3a0a 2020 2020 2020  nevents):.      
+00006230: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00006240: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+00006250: 2020 2020 2020 2320 636c 6561 720a 2020        # clear.  
+00006260: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
+00006270: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
+00006280: 2020 2020 2320 6368 6563 6b20 6e75 6d62      # check numb
+00006290: 6572 206f 6620 6576 656e 7473 0a20 2020  er of events.   
+000062a0: 2020 2020 2069 6620 6e62 5f65 7665 6e74       if nb_event
+000062b0: 735f 746f 7420 3d3d 2030 3a0a 2020 2020  s_tot == 0:.    
+000062c0: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
+000062d0: 6172 2829 0a20 2020 2020 2020 2020 2020  ar().           
+000062e0: 2073 656c 662e 5f66 696c 655f 6469 6374   self._file_dict
+000062f0: 203d 2063 7572 7265 6e74 5f66 696c 655f   = current_file_
+00006300: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
+00006310: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00006320: 7228 2745 5252 4f52 3a20 4e6f 2065 7665  r('ERROR: No eve
+00006330: 6e74 7320 666f 756e 6421 2729 0a20 2020  nts found!').   
+00006340: 2020 2020 200a 2020 2020 2020 200a 2020       .       .  
+00006350: 2020 2020 2020 2320 3d3d 3d3d 3d3d 3d3d        # ========
+00006360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006370: 3d3d 3d3d 3d3d 3d0a 2020 2020 2020 2020  =======.        
+00006380: 2320 4d65 6d6f 7279 2063 6865 636b 0a20  # Memory check. 
+00006390: 2020 2020 2020 2023 203d 3d3d 3d3d 3d3d         # =======
 000063a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000063b0: 3d3d 3d3d 0a20 2020 2020 2020 2023 2020  ====.        #  
-000063c0: 496e 6974 6961 6c69 7a65 206f 7574 7075  Initialize outpu
-000063d0: 740a 2020 2020 2020 2020 2320 3d3d 3d3d  t.        # ====
-000063e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000063f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
-00006400: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-00006410: 2020 2020 2020 2020 6f75 7470 7574 5f64          output_d
-00006420: 6174 6120 3d20 6c69 7374 2829 0a20 2020  ata = list().   
-00006430: 2020 2020 2069 6e66 6f5f 6c69 7374 203d       info_list =
-00006440: 206c 6973 7428 290a 2020 2020 200a 2020   list().     .  
-00006450: 2020 2020 2020 6966 206f 7574 7075 745f        if output_
-00006460: 666f 726d 6174 3d3d 323a 0a20 2020 2020  format==2:.     
-00006470: 2020 2020 2020 2069 6620 6164 6374 6f76         if adctov
-00006480: 6f6c 7420 6f72 2061 6463 746f 616d 7020  olt or adctoamp 
-00006490: 6f72 2062 6173 656c 696e 6573 7562 3a0a  or baselinesub:.
-000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064b0: 6f75 7470 7574 5f64 6174 6120 3d20 6e70  output_data = np
-000064c0: 2e7a 6572 6f73 2828 6e62 5f65 7665 6e74  .zeros((nb_event
-000064d0: 735f 746f 742c 206e 625f 6368 616e 6e65  s_tot, nb_channe
-000064e0: 6c73 2c20 6e62 5f73 616d 706c 6573 292c  ls, nb_samples),
-000064f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006510: 2020 2020 2020 2020 6474 7970 653d 6e70          dtype=np
-00006520: 2e66 6c6f 6174 3634 290a 2020 2020 2020  .float64).      
-00006530: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00006540: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00006550: 7574 5f64 6174 6120 3d20 6e70 2e7a 6572  ut_data = np.zer
-00006560: 6f73 2828 6e62 5f65 7665 6e74 735f 746f  os((nb_events_to
-00006570: 742c 206e 625f 6368 616e 6e65 6c73 2c20  t, nb_channels, 
-00006580: 6e62 5f73 616d 706c 6573 292c 0a20 2020  nb_samples),.   
-00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065b0: 2020 2020 6474 7970 653d 6e70 2e69 6e74      dtype=np.int
-000065c0: 3136 290a 0a0a 2020 2020 2020 2020 2020  16)...          
-000065d0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000065e0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-000065f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006600: 0a20 2020 2020 2020 2023 2020 4c6f 6f70  .        #  Loop
-00006610: 2061 6e64 2072 6561 6420 6576 656e 7473   and read events
-00006620: 0a20 2020 2020 2020 2023 203d 3d3d 3d3d  .        # =====
-00006630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006640: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020  ==========..    
-00006650: 200a 2020 2020 2020 2020 2320 6c6f 6f70   .        # loop
-00006660: 2065 7665 6e74 730a 2020 2020 2020 2020   events.        
-00006670: 666f 7220 6965 7665 6e74 2069 6e20 7261  for ievent in ra
-00006680: 6e67 6528 6e62 5f65 7665 6e74 735f 746f  nge(nb_events_to
-00006690: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-000066a0: 0a20 2020 2020 2020 2020 2020 2023 2072  .            # r
-000066b0: 6561 6420 6576 656e 740a 2020 2020 2020  ead event.      
-000066c0: 2020 2020 2020 7472 6163 6573 203d 205b        traces = [
-000066d0: 5d0a 2020 2020 2020 2020 2020 2020 696e  ].            in
-000066e0: 666f 203d 2064 6963 7428 290a 0a20 2020  fo = dict()..   
-000066f0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00006700: 7365 6c65 6374 6564 5f65 7665 6e74 5f66  selected_event_f
-00006710: 696c 6573 3a0a 2020 2020 2020 2020 2020  iles:.          
-00006720: 2020 2020 2020 7472 6163 6573 2c20 696e        traces, in
-00006730: 666f 203d 2073 656c 662e 7265 6164 5f6e  fo = self.read_n
-00006740: 6578 745f 6576 656e 7428 6465 7465 6374  ext_event(detect
-00006750: 6f72 5f63 6861 6e73 3d64 6574 6563 746f  or_chans=detecto
-00006760: 725f 6368 616e 732c 0a20 2020 2020 2020  r_chans,.       
-00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006790: 2020 2020 2020 2020 2020 2020 2061 6463               adc
-000067a0: 746f 766f 6c74 3d61 6463 746f 766f 6c74  tovolt=adctovolt
-000067b0: 2c20 6164 6374 6f61 6d70 3d61 6463 746f  , adctoamp=adcto
-000067c0: 616d 702c 0a20 2020 2020 2020 2020 2020  amp,.           
+000063b0: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2020 2020  ========.       
+000063c0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+000063d0: 2020 7361 6d70 6c65 5f62 7974 6573 203d    sample_bytes =
+000063e0: 2032 0a20 2020 2020 2020 2069 6620 6164   2.        if ad
+000063f0: 6374 6f76 6f6c 7420 6f72 2061 6463 746f  ctovolt or adcto
+00006400: 616d 7020 6f72 2062 6173 656c 696e 6573  amp or baselines
+00006410: 7562 3a0a 2020 2020 2020 2020 2020 2020  ub:.            
+00006420: 7361 6d70 6c65 5f62 7974 6573 203d 2038  sample_bytes = 8
+00006430: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+00006440: 2020 2020 2020 6f75 7470 7574 5f6d 656d        output_mem
+00006450: 6f72 795f 7065 725f 6576 656e 7420 3d20  ory_per_event = 
+00006460: 7361 6d70 6c65 5f62 7974 6573 2a6e 625f  sample_bytes*nb_
+00006470: 7361 6d70 6c65 732a 6e62 5f63 6861 6e6e  samples*nb_chann
+00006480: 656c 732f 3165 390a 2020 2020 2020 2020  els/1e9.        
+00006490: 6f75 7470 7574 5f6d 656d 6f72 7920 3d20  output_memory = 
+000064a0: 6e62 5f65 7665 6e74 735f 746f 742a 6f75  nb_events_tot*ou
+000064b0: 7470 7574 5f6d 656d 6f72 795f 7065 725f  tput_memory_per_
+000064c0: 6576 656e 740a 2020 2020 2020 2020 6966  event.        if
+000064d0: 206f 7574 7075 745f 6d65 6d6f 7279 3e6d   output_memory>m
+000064e0: 656d 6f72 795f 6c69 6d69 743a 0a20 2020  emory_limit:.   
+000064f0: 2020 2020 2020 2020 206e 625f 6576 656e           nb_even
+00006500: 7473 5f74 6f74 5f74 656d 7020 3d20 696e  ts_tot_temp = in
+00006510: 7428 726f 756e 6428 6d65 6d6f 7279 5f6c  t(round(memory_l
+00006520: 696d 6974 2f6f 7574 7075 745f 6d65 6d6f  imit/output_memo
+00006530: 7279 5f70 6572 5f65 7665 6e74 2929 0a20  ry_per_event)). 
+00006540: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00006550: 2827 5741 524e 494e 473a 204d 6178 206e  ('WARNING: Max n
+00006560: 756d 6265 7220 6576 656e 7473 2062 6173  umber events bas
+00006570: 6564 206f 6e20 6d65 6d6f 7279 206c 696d  ed on memory lim
+00006580: 6974 206f 6620 270a 2020 2020 2020 2020  it of '.        
+00006590: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
+000065a0: 6d65 6d6f 7279 5f6c 696d 6974 2920 2b20  memory_limit) + 
+000065b0: 2747 4220 6973 2027 0a20 2020 2020 2020  'GB is '.       
+000065c0: 2020 2020 2020 2020 2020 202b 2073 7472             + str
+000065d0: 286e 625f 6576 656e 7473 5f74 6f74 5f74  (nb_events_tot_t
+000065e0: 656d 7029 202b 2027 206f 7574 206f 6620  emp) + ' out of 
+000065f0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00006600: 2020 2020 2b20 7374 7228 6e62 5f65 7665      + str(nb_eve
+00006610: 6e74 735f 746f 7429 202b 2721 2729 0a20  nts_tot) +'!'). 
+00006620: 2020 2020 2020 2020 2020 206e 625f 6576             nb_ev
+00006630: 656e 7473 5f74 6f74 203d 206e 625f 6576  ents_tot = nb_ev
+00006640: 656e 7473 5f74 6f74 5f74 656d 700a 0a20  ents_tot_temp.. 
+00006650: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00006660: 2020 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d      # ==========
+00006670: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006680: 3d3d 3d3d 3d0a 2020 2020 2020 2020 2320  =====.        # 
+00006690: 2049 6e69 7469 616c 697a 6520 6f75 7470   Initialize outp
+000066a0: 7574 0a20 2020 2020 2020 2023 203d 3d3d  ut.        # ===
+000066b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000066c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020  ============.   
+000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066e0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+000066f0: 6461 7461 203d 206c 6973 7428 290a 2020  data = list().  
+00006700: 2020 2020 2020 696e 666f 5f6c 6973 7420        info_list 
+00006710: 3d20 6c69 7374 2829 0a20 2020 2020 0a20  = list().     . 
+00006720: 2020 2020 2020 2069 6620 6f75 7470 7574         if output
+00006730: 5f66 6f72 6d61 743d 3d32 3a0a 2020 2020  _format==2:.    
+00006740: 2020 2020 2020 2020 6966 2061 6463 746f          if adcto
+00006750: 766f 6c74 206f 7220 6164 6374 6f61 6d70  volt or adctoamp
+00006760: 206f 7220 6261 7365 6c69 6e65 7375 623a   or baselinesub:
+00006770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006780: 206f 7574 7075 745f 6461 7461 203d 206e   output_data = n
+00006790: 702e 7a65 726f 7328 286e 625f 6576 656e  p.zeros((nb_even
+000067a0: 7473 5f74 6f74 2c20 6e62 5f63 6861 6e6e  ts_tot, nb_chann
+000067b0: 656c 732c 206e 625f 7361 6d70 6c65 7329  els, nb_samples)
+000067c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067f0: 2020 2020 2020 2020 2062 6173 656c 696e           baselin
-00006800: 6573 7562 3d62 6173 656c 696e 6573 7562  esub=baselinesub
-00006810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006840: 2020 2020 2020 6261 7365 6c69 6e65 696e        baselinein
-00006850: 6473 3d62 6173 656c 696e 6569 6e64 732c  ds=baselineinds,
-00006860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000067e0: 2020 2020 2020 2020 2064 7479 7065 3d6e           dtype=n
+000067f0: 702e 666c 6f61 7436 3429 0a20 2020 2020  p.float64).     
+00006800: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00006810: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00006820: 7075 745f 6461 7461 203d 206e 702e 7a65  put_data = np.ze
+00006830: 726f 7328 286e 625f 6576 656e 7473 5f74  ros((nb_events_t
+00006840: 6f74 2c20 6e62 5f63 6861 6e6e 656c 732c  ot, nb_channels,
+00006850: 206e 625f 7361 6d70 6c65 7329 2c0a 2020   nb_samples),.  
+00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006890: 2020 2020 2069 6e63 6c75 6465 5f6d 6574       include_met
-000068a0: 6164 6174 613d 5472 7565 290a 2020 2020  adata=True).    
-000068b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000068c0: 2020 2020 2020 2020 2020 2020 2020 6576                ev
-000068d0: 656e 745f 696e 6465 7820 3d20 7365 6c65  ent_index = sele
-000068e0: 6374 6564 5f65 7665 6e74 5f66 696c 6573  cted_event_files
-000068f0: 5b69 6576 656e 745d 5b30 5d0a 2020 2020  [ievent][0].    
-00006900: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00006910: 5f6e 616d 6520 3d20 7365 6c65 6374 6564  _name = selected
-00006920: 5f65 7665 6e74 5f66 696c 6573 5b69 6576  _event_files[iev
-00006930: 656e 745d 5b31 5d0a 2020 2020 2020 2020  ent][1].        
-00006940: 2020 2020 2020 2020 7472 6163 6573 2c20          traces, 
-00006950: 696e 666f 203d 2073 656c 662e 7265 6164  info = self.read
-00006960: 5f73 696e 676c 655f 6576 656e 7428 6576  _single_event(ev
-00006970: 656e 745f 696e 6465 782c 2066 696c 655f  ent_index, file_
-00006980: 6e61 6d65 3d66 696c 655f 6e61 6d65 2c0a  name=file_name,.
-00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069c0: 2020 2020 2020 6465 7465 6374 6f72 5f63        detector_c
-000069d0: 6861 6e73 3d64 6574 6563 746f 725f 6368  hans=detector_ch
-000069e0: 616e 732c 0a20 2020 2020 2020 2020 2020  ans,.           
-000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a10: 2020 2020 2020 2020 2020 2061 6463 746f             adcto
-00006a20: 766f 6c74 3d61 6463 746f 766f 6c74 2c20  volt=adctovolt, 
-00006a30: 6164 6374 6f61 6d70 3d61 6463 746f 616d  adctoamp=adctoam
-00006a40: 702c 0a20 2020 2020 2020 2020 2020 2020  p,.             
-00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a70: 2020 2020 2020 2020 2062 6173 656c 696e           baselin
-00006a80: 6573 7562 3d62 6173 656c 696e 6573 7562  esub=baselinesub
-00006a90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ac0: 2020 2020 2020 2020 6261 7365 6c69 6e65          baseline
-00006ad0: 696e 6473 3d62 6173 656c 696e 6569 6e64  inds=baselineind
-00006ae0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b10: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
-00006b20: 5f6d 6574 6164 6174 613d 5472 7565 290a  _metadata=True).
-00006b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b40: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-00006b50: 6865 636b 2069 6620 7265 6164 696e 6720  heck if reading 
-00006b60: 6572 726f 720a 2020 2020 2020 2020 2020  error.          
-00006b70: 2020 6966 2069 6e66 6f5b 2772 6561 645f    if info['read_
-00006b80: 7374 6174 7573 275d 3e30 3a0a 2020 2020  status']>0:.    
-00006b90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00006ba0: 7428 2757 4152 4e49 4e47 3a20 556e 6162  t('WARNING: Unab
-00006bb0: 6c65 2074 6f20 7265 6164 2065 7665 6e74  le to read event
-00006bc0: 2023 2720 2b20 7374 7228 6965 7665 6e74   #' + str(ievent
-00006bd0: 2920 2b20 2721 2045 7272 6f72 206d 6573  ) + '! Error mes
-00006be0: 7361 6765 3a20 2729 0a20 2020 2020 2020  sage: ').       
-00006bf0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00006c00: 5741 524e 494e 473a 2022 2720 2b20 696e  WARNING: "' + in
-00006c10: 666f 5b27 6572 726f 725f 6d73 6727 5d20  fo['error_msg'] 
-00006c20: 2b20 2722 2e20 5374 6f70 7069 6e67 2065  + '". Stopping e
-00006c30: 7665 6e74 206c 6f6f 7027 290a 2020 2020  vent loop').    
-00006c40: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00006c50: 6b0a 0a20 2020 2020 2020 2020 2020 200a  k..            .
-00006c60: 2020 2020 2020 2020 2020 2020 2320 6164              # ad
-00006c70: 6420 746f 206d 6574 6164 6174 6120 6c69  d to metadata li
-00006c80: 7374 0a20 2020 2020 2020 2020 2020 2069  st.            i
-00006c90: 6620 696e 636c 7564 655f 6d65 7461 6461  f include_metada
-00006ca0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00006cb0: 2020 2020 696e 666f 5f6c 6973 742e 6170      info_list.ap
-00006cc0: 7065 6e64 2869 6e66 6f29 0a0a 2020 2020  pend(info)..    
-00006cd0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006ce0: 2020 2020 2023 2073 746f 7265 0a20 2020       # store.   
-00006cf0: 2020 2020 2020 2020 2069 6620 286f 7574           if (out
-00006d00: 7075 745f 666f 726d 6174 3d3d 3120 6f72  put_format==1 or
-00006d10: 206f 7574 7075 745f 666f 726d 6174 3d3d   output_format==
-00006d20: 3329 3a0a 2020 2020 2020 2020 2020 2020  3):.            
-00006d30: 2020 2020 6f75 7470 7574 5f64 6174 612e      output_data.
-00006d40: 6170 7065 6e64 2874 7261 6365 7329 0a20  append(traces). 
-00006d50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00006d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d70: 206f 7574 7075 745f 6461 7461 5b69 6576   output_data[iev
-00006d80: 656e 742c 3a2c 3a5d 203d 2074 7261 6365  ent,:,:] = trace
-00006d90: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00006da0: 2020 0a0a 2020 2020 2020 2020 2320 7265    ..        # re
-00006db0: 7365 7420 6669 6c65 206c 6973 7420 746f  set file list to
-00006dc0: 206f 7269 6769 6e61 6c20 6c69 7374 0a20   original list. 
-00006dd0: 2020 2020 2020 2023 2069 6620 6e65 6564         # if need
-00006de0: 6564 0a20 2020 2020 2020 2069 6620 6375  ed.        if cu
-00006df0: 7272 656e 745f 6669 6c65 5f6c 6973 7420  rrent_file_list 
-00006e00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00006e10: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00006e20: 745f 6669 6c65 7328 6375 7272 656e 745f  t_files(current_
-00006e30: 6669 6c65 5f6c 6973 7429 0a0a 0a20 2020  file_list)...   
-00006e40: 2020 2020 2069 6620 696e 636c 7564 655f       if include_
-00006e50: 6d65 7461 6461 7461 3a0a 2020 2020 2020  metadata:.      
-00006e60: 2020 2020 2020 7265 7475 726e 206f 7574        return out
-00006e70: 7075 745f 6461 7461 2c20 696e 666f 5f6c  put_data, info_l
-00006e80: 6973 740a 2020 2020 2020 2020 656c 7365  ist.        else
-00006e90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00006ea0: 7475 726e 206f 7574 7075 745f 6461 7461  turn output_data
-00006eb0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006ec0: 2020 0a20 2020 2020 2020 200a 2020 2020    .        .    
-00006ed0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006ee0: 2020 2020 200a 2020 2020 2020 2020 0a0a       .        ..
-00006ef0: 2020 2020 6465 6620 6765 745f 6375 7272      def get_curr
-00006f00: 656e 745f 6669 6c65 5f6e 616d 6528 7365  ent_file_name(se
-00006f10: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00006f20: 0a20 2020 2020 2020 2047 6574 2063 7572  .        Get cur
-00006f30: 7265 6e74 2066 696c 6520 6e61 6d65 0a20  rent file name. 
-00006f40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006f50: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00006f60: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00006f70: 2020 2020 2020 4e6f 6e65 0a0a 0a20 2020        None...   
-00006f80: 2020 2020 2052 6574 7572 6e0a 2020 2020       Return.    
-00006f90: 2020 2020 2d2d 2d2d 2d2d 0a20 2020 2020      ------.     
-00006fa0: 2020 200a 2020 2020 2020 2020 6669 6c65     .        file
-00006fb0: 5f6e 616d 6520 3a20 7374 720a 2020 2020  _name : str.    
-00006fc0: 2020 2020 2020 6375 7272 656e 7420 6669        current fi
-00006fd0: 6c65 206e 616d 650a 0a20 2020 2020 2020  le name..       
-00006fe0: 2022 2222 0a20 2020 2020 2020 200a 2020   """.        .  
-00006ff0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00007000: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
-00007010: 6e61 6d65 0a20 2020 2020 2020 200a 0a0a  name.        ...
-00007020: 2020 2020 0a20 2020 2064 6566 2067 6574      .    def get
-00007030: 5f6d 6574 6164 6174 6128 7365 6c66 2c20  _metadata(self, 
-00007040: 6669 6c65 5f6e 616d 653d 4e6f 6e65 2c20  file_name=None, 
-00007050: 6772 6f75 705f 6e61 6d65 3d4e 6f6e 652c  group_name=None,
-00007060: 2064 6174 6173 6574 5f6e 616d 653d 4e6f   dataset_name=No
-00007070: 6e65 2c20 0a20 2020 2020 2020 2020 2020  ne, .           
-00007080: 2020 2020 2020 2020 2020 696e 636c 7564            includ
-00007090: 655f 6461 7461 7365 745f 6d65 7461 6461  e_dataset_metada
-000070a0: 7461 3d46 616c 7365 293a 0a0a 2020 2020  ta=False):..    
-000070b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000070c0: 4675 6e63 7469 6f6e 2074 6f20 6765 7420  Function to get 
-000070d0: 6d65 7461 6461 7461 2e0a 2020 2020 2020  metadata..      
-000070e0: 200a 2020 2020 2020 2020 5061 7261 6d65   .        Parame
-000070f0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00007100: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00007110: 2020 0a20 2020 2020 2020 2066 696c 655f    .        file_
-00007120: 6e61 6d65 3a20 7374 7269 6e67 2c20 6f70  name: string, op
-00007130: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00007140: 2020 2069 6620 6e6f 2066 696c 6520 6e61     if no file na
-00007150: 6d65 2070 726f 7669 6465 643a 2075 7365  me provided: use
-00007160: 2063 7572 7265 6e74 2066 696c 650a 0a20   current file.. 
-00007170: 2020 2020 2020 2067 726f 7570 5f6e 616d         group_nam
-00007180: 653a 2020 7374 7269 6e67 2c20 6f70 7469  e:  string, opti
-00007190: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-000071a0: 2048 3520 2247 726f 7570 2220 6e61 6d65   H5 "Group" name
-000071b0: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
-000071c0: 6175 6c74 3a20 4e6f 6e65 2c20 7265 6164  ault: None, read
-000071d0: 2061 6c6c 2067 726f 7570 730a 2020 2020   all groups.    
-000071e0: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
-000071f0: 6174 6173 6574 5f6e 616d 653a 2073 7472  ataset_name: str
-00007200: 696e 672c 206f 7074 696f 6e61 6c2c 200a  ing, optional, .
-00007210: 2020 2020 2020 2020 2020 2020 4835 2022              H5 "
-00007220: 4461 7461 7365 7422 206e 616d 650a 2020  Dataset" name.  
-00007230: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00007240: 743a 2061 6c6c 2064 6174 6173 6574 730a  t: all datasets.
-00007250: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00007260: 2020 696e 636c 7564 655f 6461 7461 7365    include_datase
-00007270: 745f 6d65 7461 6461 7461 203a 2062 6f6f  t_metadata : boo
-00007280: 6c2c 206f 7074 696f 6e61 6c0a 2020 2020  l, optional.    
-00007290: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
-000072a0: 2069 6e63 6c75 6465 2064 6174 6173 6574   include dataset
-000072b0: 206d 6574 6164 6174 610a 2020 2020 2020   metadata.      
-000072c0: 2020 2020 2020 4465 6661 756c 743a 2046        Default: F
-000072d0: 616c 7365 0a20 2020 2020 2020 200a 0a20  alse.        .. 
-000072e0: 2020 2020 2020 2052 6574 7572 6e0a 2020         Return.  
-000072f0: 2020 2020 2020 2d2d 2d2d 2d2d 0a20 2020        ------.   
-00007300: 2020 2020 200a 2020 2020 2020 2020 6d65       .        me
-00007310: 7461 6461 7461 3a20 6469 6374 0a20 2020  tadata: dict.   
-00007320: 2020 2020 2020 2020 6469 6374 696f 6e61          dictiona
-00007330: 7279 2077 6974 6820 616c 6c20 6d65 7461  ry with all meta
-00007340: 6461 7461 0a0a 2020 2020 2020 2020 2222  data..        ""
-00007350: 220a 0a20 2020 2020 2020 206d 6574 6164  "..        metad
-00007360: 6174 6120 3d20 6469 6374 2829 0a0a 0a20  ata = dict()... 
-00007370: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
-00007380: 6e70 7574 200a 2020 2020 2020 2020 6966  nput .        if
-00007390: 2066 696c 655f 6e61 6d65 2069 7320 4e6f   file_name is No
-000073a0: 6e65 2061 6e64 2073 656c 662e 5f63 7572  ne and self._cur
-000073b0: 7265 6e74 5f66 696c 6520 6973 204e 6f6e  rent_file is Non
-000073c0: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
-000073d0: 7272 6f72 5f6d 7367 203d 2027 4e6f 2066  rror_msg = 'No f
-000073e0: 696c 6520 6375 7272 656e 746c 7920 6f70  ile currently op
-000073f0: 656e 2061 6e64 206e 6f20 2266 696c 655f  en and no "file_
-00007400: 6e61 6d65 2220 6172 6775 6d65 6e74 206e  name" argument n
-00007410: 6f74 2070 726f 7669 6465 6421 270a 2020  ot provided!'.  
-00007420: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00007430: 662e 5f72 6169 7365 5f65 7272 6f72 733a  f._raise_errors:
-00007440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007450: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00007460: 4572 726f 7228 6572 726f 725f 6d73 6729  Error(error_msg)
-00007470: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00007480: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00007490: 2020 2070 7269 6e74 2827 4552 524f 523a     print('ERROR:
-000074a0: 2027 202b 2065 7272 6f72 5f6d 7367 290a   ' + error_msg).
-000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074c0: 7072 696e 7428 2750 6c65 6173 6520 6f70  print('Please op
-000074d0: 656e 2061 2066 696c 6520 6f72 2070 726f  en a file or pro
-000074e0: 7669 6465 2061 2066 696c 6520 6e61 6d65  vide a file name
-000074f0: 2127 290a 2020 2020 2020 2020 2020 2020  !').            
-00007500: 2020 2020 7265 7475 726e 206d 6574 6164      return metad
-00007510: 6174 610a 0a20 2020 2020 2020 2023 206f  ata..        # o
-00007520: 7065 6e20 6669 6c65 2069 6620 6e65 6564  pen file if need
-00007530: 6564 0a20 2020 2020 2020 2069 6620 2866  ed.        if (f
-00007540: 696c 655f 6e61 6d65 2069 7320 6e6f 7420  ile_name is not 
-00007550: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00007560: 2061 6e64 2073 656c 662e 5f63 7572 7265   and self._curre
-00007570: 6e74 5f66 696c 655f 6e61 6d65 213d 6669  nt_file_name!=fi
-00007580: 6c65 5f6e 616d 6529 3a0a 2020 2020 2020  le_name):.      
-00007590: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-000075a0: 2020 2023 2063 6865 636b 2069 6620 6120     # check if a 
-000075b0: 6669 6c65 2061 6c72 6561 6479 206f 7065  file already ope
-000075c0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
-000075d0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-000075e0: 696c 6520 6973 206e 6f74 204e 6f6e 653a  ile is not None:
-000075f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007600: 2073 656c 662e 5f63 6c6f 7365 5f66 696c   self._close_fil
-00007610: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00007620: 2320 6f70 656e 0a20 2020 2020 2020 2020  # open.         
-00007630: 2020 2073 656c 662e 5f6f 7065 6e5f 6669     self._open_fi
-00007640: 6c65 2866 696c 655f 6e61 6d65 2c20 6c6f  le(file_name, lo
-00007650: 6164 5f6d 6574 6164 6174 613d 4661 6c73  ad_metadata=Fals
-00007660: 6529 0a20 2020 2020 2020 2020 2020 200a  e).            .
-00007670: 0a20 2020 2020 2020 2023 206c 6f61 6420  .        # load 
-00007680: 6d65 7461 6461 7461 2028 6966 2022 6461  metadata (if "da
-00007690: 7461 7365 7422 206d 6574 6164 6174 6120  taset" metadata 
-000076a0: 7265 7175 6573 7465 6420 2d3e 2072 656c  requested -> rel
-000076b0: 6f61 6429 0a20 2020 2020 2020 2069 6620  oad).        if 
-000076c0: 6461 7461 7365 745f 6e61 6d65 2069 7320  dataset_name is 
-000076d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000076e0: 2020 2020 2020 696e 636c 7564 655f 6461        include_da
-000076f0: 7461 7365 745f 6d65 7461 6461 7461 203d  taset_metadata =
-00007700: 2054 7275 650a 0a20 2020 2020 2020 2069   True..        i
-00007710: 6620 7365 6c66 2e5f 6375 7272 656e 745f  f self._current_
-00007720: 6669 6c65 5f6d 6574 6164 6174 6120 6973  file_metadata is
-00007730: 204e 6f6e 6520 6f72 2069 6e63 6c75 6465   None or include
-00007740: 5f64 6174 6173 6574 5f6d 6574 6164 6174  _dataset_metadat
-00007750: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
-00007760: 656c 662e 5f6c 6f61 645f 6d65 7461 6461  elf._load_metada
-00007770: 7461 2869 6e63 6c75 6465 5f64 6174 6173  ta(include_datas
-00007780: 6574 5f6d 6574 6164 6174 6129 0a20 2020  et_metadata).   
-00007790: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-000077a0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-000077b0: 2020 2023 2066 696e 6420 7370 6563 6966     # find specif
-000077c0: 6963 206d 6574 6164 6174 610a 2020 2020  ic metadata.    
-000077d0: 2020 2020 6d65 7461 6461 7461 203d 2064      metadata = d
-000077e0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000077f0: 2067 726f 7570 5f6e 616d 6520 6973 206e   group_name is n
-00007800: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00007810: 2020 2020 2069 6620 6772 6f75 705f 6e61       if group_na
-00007820: 6d65 2069 6e20 7365 6c66 2e5f 6375 7272  me in self._curr
-00007830: 656e 745f 6669 6c65 5f6d 6574 6164 6174  ent_file_metadat
-00007840: 615b 2767 726f 7570 5f6c 6973 7427 5d3a  a['group_list']:
-00007850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007860: 2067 726f 7570 5f6d 6574 6164 6174 6120   group_metadata 
-00007870: 3d20 7365 6c66 2e5f 6375 7272 656e 745f  = self._current_
-00007880: 6669 6c65 5f6d 6574 6164 6174 615b 2767  file_metadata['g
-00007890: 726f 7570 7327 5d5b 6772 6f75 705f 6e61  roups'][group_na
-000078a0: 6d65 5d0a 2020 2020 2020 2020 2020 2020  me].            
-000078b0: 2020 2020 6966 2064 6174 6173 6574 5f6e      if dataset_n
-000078c0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-000078d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000078e0: 2020 2020 2069 6620 6461 7461 7365 745f       if dataset_
-000078f0: 6e61 6d65 2069 6e20 6772 6f75 705f 6d65  name in group_me
-00007900: 7461 6461 7461 5b27 6461 7461 7365 745f  tadata['dataset_
-00007910: 6c69 7374 275d 3a0a 2020 2020 2020 2020  list']:.        
-00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007930: 6d65 7461 6461 7461 203d 2067 726f 7570  metadata = group
-00007940: 5f6d 6574 6164 6174 615b 2764 6174 6173  _metadata['datas
-00007950: 6574 7327 5d5b 6461 7461 7365 745f 6e61  ets'][dataset_na
-00007960: 6d65 5d0a 2020 2020 2020 2020 2020 2020  me].            
-00007970: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00007980: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00007990: 7461 6461 7461 203d 2067 726f 7570 5f6d  tadata = group_m
-000079a0: 6574 6164 6174 610a 2020 2020 2020 2020  etadata.        
-000079b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000079c0: 2020 6d65 7461 6461 7461 203d 2073 656c    metadata = sel
-000079d0: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
-000079e0: 6d65 7461 6461 7461 0a0a 0a20 2020 2020  metadata...     
-000079f0: 2020 2023 2063 6c6f 7365 2066 696c 650a     # close file.
-00007a00: 2020 2020 2020 2020 6966 2066 696c 655f          if file_
-00007a10: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-00007a20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00007a30: 6c66 2e5f 636c 6f73 655f 6669 6c65 2829  lf._close_file()
-00007a40: 0a20 2020 2020 2020 200a 0a20 2020 2020  .        ..     
-00007a50: 2020 2072 6574 7572 6e20 6d65 7461 6461     return metada
-00007a60: 7461 0a20 2020 2020 2020 2020 2020 200a  ta.            .
-00007a70: 0a0a 0a20 2020 2064 6566 2067 6574 5f64  ...    def get_d
-00007a80: 6574 6563 746f 725f 636f 6e66 6967 2873  etector_config(s
-00007a90: 656c 662c 2066 696c 655f 6e61 6d65 3d4e  elf, file_name=N
-00007aa0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 2061 6463 5f6e 616d 653d 2761 6463 3127   adc_name='adc1'
-00007ad0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007ae0: 2020 2020 2020 2020 2020 2020 2020 7573                us
-00007af0: 655f 6368 616e 5f64 6963 743d 5472 7565  e_chan_dict=True
-00007b00: 293a 2020 200a 2020 2020 2020 2020 2222  ):   .        ""
-00007b10: 220a 2020 2020 2020 2020 4765 7420 6465  ".        Get de
-00007b20: 7465 6374 6f72 2063 6f6e 6669 6775 7261  tector configura
-00007b30: 7469 6f6e 0a20 2020 2020 2020 2022 2222  tion.        """
-00007b40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007b50: 2020 6465 7465 6374 6f72 5f63 6f6e 6669    detector_confi
-00007b60: 6720 3d20 6469 6374 2829 0a20 2020 2020  g = dict().     
-00007b70: 2020 200a 2020 2020 2020 2020 2320 6765     .        # ge
-00007b80: 7420 6d65 7461 6461 7461 0a20 2020 2020  t metadata.     
-00007b90: 2020 206d 6574 6164 6174 6120 3d20 4e6f     metadata = No
-00007ba0: 6e65 0a20 2020 2020 2020 2069 6620 6669  ne.        if fi
-00007bb0: 6c65 5f6e 616d 6520 6973 206e 6f74 204e  le_name is not N
-00007bc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00007bd0: 206d 6574 6164 6174 6120 3d20 7365 6c66   metadata = self
-00007be0: 2e67 6574 5f6d 6574 6164 6174 6128 6669  .get_metadata(fi
-00007bf0: 6c65 5f6e 616d 653d 6669 6c65 5f6e 616d  le_name=file_nam
-00007c00: 6529 0a20 2020 2020 2020 2065 6c69 6620  e).        elif 
-00007c10: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
-00007c20: 6c65 5f6d 6574 6164 6174 6120 6973 206e  le_metadata is n
-00007c30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00007c40: 2020 2020 206d 6574 6164 6174 6120 3d20       metadata = 
-00007c50: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
-00007c60: 6c65 5f6d 6574 6164 6174 610a 2020 2020  le_metadata.    
-00007c70: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00007c80: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00007c90: 6545 7272 6f72 2827 4552 524f 5220 696e  eError('ERROR in
-00007ca0: 2067 6574 5f64 6574 6563 746f 725f 636f   get_detector_co
-00007cb0: 6e66 6967 3a20 6120 6669 6c65 206e 616d  nfig: a file nam
-00007cc0: 6520 6e65 6564 7320 746f 2062 6520 7072  e needs to be pr
-00007cd0: 6f76 6964 6564 2127 290a 2020 2020 2020  ovided!').      
-00007ce0: 2020 0a20 2020 2020 2020 200a 0a20 2020    .        ..   
-00007cf0: 2020 2020 2023 2063 6f6e 6669 6720 6e61       # config na
-00007d00: 6d65 0a20 2020 2020 2020 2063 6f6e 6669  me.        confi
-00007d10: 675f 6e61 6d65 203d 2027 6465 7463 6f6e  g_name = 'detcon
-00007d20: 6669 6731 270a 2020 2020 2020 2020 6966  fig1'.        if
-00007d30: 2061 6463 5f6e 616d 6521 3d27 6164 6331   adc_name!='adc1
-00007d40: 273a 0a20 2020 2020 2020 2020 2020 2063  ':.            c
-00007d50: 6f6e 6669 675f 6e61 6d65 203d 2027 6465  onfig_name = 'de
-00007d60: 7463 6f6e 6669 6727 202b 2061 6463 5f6e  tconfig' + adc_n
-00007d70: 616d 655b 333a 5d0a 0a20 2020 2020 2020  ame[3:]..       
-00007d80: 2023 2063 6865 636b 2069 6620 6176 6169   # check if avai
-00007d90: 6c61 626c 650a 2020 2020 2020 2020 6966  lable.        if
-00007da0: 2063 6f6e 6669 675f 6e61 6d65 206e 6f74   config_name not
-00007db0: 2069 6e20 6d65 7461 6461 7461 5b27 6772   in metadata['gr
-00007dc0: 6f75 705f 6c69 7374 275d 3a0a 2020 2020  oup_list']:.    
-00007dd0: 2020 2020 2020 2020 7072 696e 7428 2745          print('E
-00007de0: 5252 4f52 3a20 756e 6162 6c65 2074 6f20  RROR: unable to 
-00007df0: 6669 6e64 2064 6574 6563 746f 7220 636f  find detector co
-00007e00: 6e66 6967 2127 290a 2020 2020 2020 2020  nfig!').        
-00007e10: 2020 2020 7265 7475 726e 205b 5d0a 0a20      return [].. 
-00007e20: 2020 2020 2020 2023 2067 726f 7570 206d         # group m
-00007e30: 6574 6164 6174 610a 2020 2020 2020 2020  etadata.        
-00007e40: 6465 7465 6374 6f72 5f63 6f6e 6669 675f  detector_config_
-00007e50: 6469 6374 203d 206d 6574 6164 6174 615b  dict = metadata[
-00007e60: 2767 726f 7570 7327 5d5b 636f 6e66 6967  'groups'][config
-00007e70: 5f6e 616d 655d 0a20 2020 2020 2020 2023  _name].        #
-00007e80: 6966 2027 6164 635f 6e61 6d65 2720 696e  if 'adc_name' in
-00007e90: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
-00007ea0: 5f64 6963 7420 616e 6420 6164 635f 6e61  _dict and adc_na
-00007eb0: 6d65 213d 6465 7465 6374 6f72 5f63 6f6e  me!=detector_con
-00007ec0: 6669 675f 6469 6374 5b27 6164 635f 6e61  fig_dict['adc_na
-00007ed0: 6d65 275d 3a0a 2020 2020 2020 2020 2320  me']:.        # 
-00007ee0: 2020 2070 7269 6e74 2827 4552 524f 523a     print('ERROR:
-00007ef0: 2055 6e65 7870 6563 7465 6420 6465 7465   Unexpected dete
-00007f00: 6374 6f72 2063 6f6e 6669 6775 7261 7469  ctor configurati
-00007f10: 6f6e 2066 6f72 6d61 7421 2729 0a20 2020  on format!').   
-00007f20: 2020 2020 2023 2020 2020 7265 7475 726e       #    return
-00007f30: 205b 5d0a 0a0a 2020 2020 2020 2020 2320   []...        # 
-00007f40: 6164 6420 6465 7465 6374 6f72 2f63 6861  add detector/cha
-00007f50: 6e6e 656c 206c 6973 7420 6672 6f6d 2061  nnel list from a
-00007f60: 6463 206d 6574 6164 6174 612c 206e 6565  dc metadata, nee
-00007f70: 6473 2074 6f20 6d61 7463 680a 2020 2020  ds to match.    
-00007f80: 2020 2020 2320 6465 7465 6374 6f72 2073      # detector s
-00007f90: 6574 7469 6e67 7320 6172 7261 7920 6f72  ettings array or
-00007fa0: 6465 720a 2020 2020 2020 2020 7465 735f  der.        tes_
-00007fb0: 6368 616e 7320 3d20 6c69 7374 2829 0a20  chans = list(). 
-00007fc0: 2020 2020 2020 2064 6574 6563 746f 725f         detector_
-00007fd0: 6368 616e 7320 3d20 6c69 7374 2829 0a20  chans = list(). 
-00007fe0: 2020 2020 2020 2063 6f6e 7472 6f6c 6c65         controlle
-00007ff0: 725f 6368 616e 7320 3d20 6c69 7374 2829  r_chans = list()
-00008000: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
-00008010: 696f 6e5f 6469 6374 203d 2073 656c 662e  ion_dict = self.
-00008020: 6765 745f 636f 6e6e 6563 7469 6f6e 5f64  get_connection_d
-00008030: 6963 7428 6164 635f 6e61 6d65 3d61 6463  ict(adc_name=adc
-00008040: 5f6e 616d 652c 0a20 2020 2020 2020 2020  _name,.         
-00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008070: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
-00008080: 7461 3d6d 6574 6164 6174 6129 0a0a 2020  ta=metadata)..  
-00008090: 2020 2020 2020 6966 2063 6f6e 6e65 6374        if connect
-000080a0: 696f 6e5f 6469 6374 3a0a 2020 2020 2020  ion_dict:.      
-000080b0: 2020 2020 2020 6368 616e 5f6c 6973 7420        chan_list 
-000080c0: 3d20 6465 7465 6374 6f72 5f63 6f6e 6669  = detector_confi
-000080d0: 675f 6469 6374 5b27 6368 616e 6e65 6c5f  g_dict['channel_
-000080e0: 6c69 7374 275d 0a20 2020 2020 2020 2020  list'].         
-000080f0: 2020 2069 6620 286e 6f74 2069 7369 6e73     if (not isins
-00008100: 7461 6e63 6528 6368 616e 5f6c 6973 742c  tance(chan_list,
-00008110: 206e 702e 6e64 6172 7261 7929 0a20 2020   np.ndarray).   
-00008120: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00008130: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00008140: 6368 616e 5f6c 6973 742c 206c 6973 7429  chan_list, list)
-00008150: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00008160: 2020 2063 6861 6e5f 6c69 7374 2020 3d20     chan_list  = 
-00008170: 5b63 6861 6e5f 6c69 7374 5d0a 2020 2020  [chan_list].    
-00008180: 2020 2020 2020 2020 666f 7220 6368 616e          for chan
-00008190: 2069 6e20 6368 616e 5f6c 6973 743a 0a20   in chan_list:. 
-000081a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000081b0: 6620 6368 616e 2069 6e20 636f 6e6e 6563  f chan in connec
-000081c0: 7469 6f6e 5f64 6963 745b 2761 6463 5f63  tion_dict['adc_c
-000081d0: 6861 6e73 275d 3a0a 2020 2020 2020 2020  hans']:.        
-000081e0: 2020 2020 2020 2020 2020 2020 696e 6420              ind 
-000081f0: 3d20 636f 6e6e 6563 7469 6f6e 5f64 6963  = connection_dic
-00008200: 745b 2761 6463 5f63 6861 6e73 275d 2e69  t['adc_chans'].i
-00008210: 6e64 6578 2869 6e74 2863 6861 6e29 290a  ndex(int(chan)).
-00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008230: 2020 2020 6966 2063 6f6e 6e65 6374 696f      if connectio
-00008240: 6e5f 6469 6374 5b27 636f 6e74 726f 6c6c  n_dict['controll
-00008250: 6572 5f63 6861 6e73 275d 3a0a 2020 2020  er_chans']:.    
-00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008270: 2020 2020 636f 6e74 726f 6c6c 6572 5f63      controller_c
-00008280: 6861 6e73 2e61 7070 656e 6428 636f 6e6e  hans.append(conn
-00008290: 6563 7469 6f6e 5f64 6963 745b 2763 6f6e  ection_dict['con
-000082a0: 7472 6f6c 6c65 725f 6368 616e 7327 5d5b  troller_chans'][
-000082b0: 696e 645d 290a 2020 2020 2020 2020 2020  ind]).          
-000082c0: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
-000082d0: 6e65 6374 696f 6e5f 6469 6374 5b27 7465  nection_dict['te
-000082e0: 735f 6368 616e 7327 5d3a 0a20 2020 2020  s_chans']:.     
+00006880: 2020 2020 2064 7479 7065 3d6e 702e 696e       dtype=np.in
+00006890: 7431 3629 0a20 2020 2020 2020 2020 2020  t16).           
+000068a0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+000068b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000068c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+000068d0: 2020 2020 2020 2020 2320 204c 6f6f 7020          #  Loop 
+000068e0: 616e 6420 7265 6164 2065 7665 6e74 730a  and read events.
+000068f0: 2020 2020 2020 2020 2320 3d3d 3d3d 3d3d          # ======
+00006900: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00006910: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 200a  =========.     .
+00006920: 2020 2020 2020 2020 2320 6c6f 6f70 2065          # loop e
+00006930: 7665 6e74 730a 2020 2020 2020 2020 666f  vents.        fo
+00006940: 7220 6965 7665 6e74 2069 6e20 7261 6e67  r ievent in rang
+00006950: 6528 6e62 5f65 7665 6e74 735f 746f 7429  e(nb_events_tot)
+00006960: 3a0a 2020 2020 2020 2020 2020 2020 0a20  :.            . 
+00006970: 2020 2020 2020 2020 2020 2023 2072 6561             # rea
+00006980: 6420 6576 656e 740a 2020 2020 2020 2020  d event.        
+00006990: 2020 2020 7472 6163 6573 203d 205b 5d0a      traces = [].
+000069a0: 2020 2020 2020 2020 2020 2020 696e 666f              info
+000069b0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+000069c0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+000069d0: 2020 7472 6163 6573 2c20 696e 666f 203d    traces, info =
+000069e0: 2073 656c 662e 7265 6164 5f6e 6578 745f   self.read_next_
+000069f0: 6576 656e 7428 0a20 2020 2020 2020 2020  event(.         
+00006a00: 2020 2020 2020 2074 7261 6365 5f6c 656e         trace_len
+00006a10: 6774 685f 6d73 6563 3d74 7261 6365 5f6c  gth_msec=trace_l
+00006a20: 656e 6774 685f 6d73 6563 2c0a 2020 2020  ength_msec,.    
+00006a30: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00006a40: 655f 6c65 6e67 7468 5f73 616d 706c 6573  e_length_samples
+00006a50: 3d74 7261 6365 5f6c 656e 6774 685f 7361  =trace_length_sa
+00006a60: 6d70 6c65 732c 0a20 2020 2020 2020 2020  mples,.         
+00006a70: 2020 2020 2020 2070 7265 7472 6967 6765         pretrigge
+00006a80: 725f 6c65 6e67 7468 5f6d 7365 633d 7072  r_length_msec=pr
+00006a90: 6574 7269 6767 6572 5f6c 656e 6774 685f  etrigger_length_
+00006aa0: 6d73 6563 2c0a 2020 2020 2020 2020 2020  msec,.          
+00006ab0: 2020 2020 2020 7072 6574 7269 6767 6572        pretrigger
+00006ac0: 5f6c 656e 6774 685f 7361 6d70 6c65 733d  _length_samples=
+00006ad0: 7072 6574 7269 6767 6572 5f6c 656e 6774  pretrigger_lengt
+00006ae0: 685f 7361 6d70 6c65 732c 0a20 2020 2020  h_samples,.     
+00006af0: 2020 2020 2020 2020 2020 2064 6574 6563             detec
+00006b00: 746f 725f 6368 616e 733d 6465 7465 6374  tor_chans=detect
+00006b10: 6f72 5f63 6861 6e73 2c0a 2020 2020 2020  or_chans,.      
+00006b20: 2020 2020 2020 2020 2020 6164 6374 6f76            adctov
+00006b30: 6f6c 743d 6164 6374 6f76 6f6c 742c 2061  olt=adctovolt, a
+00006b40: 6463 746f 616d 703d 6164 6374 6f61 6d70  dctoamp=adctoamp
+00006b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006b60: 2020 6261 7365 6c69 6e65 7375 623d 6261    baselinesub=ba
+00006b70: 7365 6c69 6e65 7375 622c 0a20 2020 2020  selinesub,.     
+00006b80: 2020 2020 2020 2020 2020 2062 6173 656c             basel
+00006b90: 696e 6569 6e64 733d 6261 7365 6c69 6e65  ineinds=baseline
+00006ba0: 696e 6473 2c0a 2020 2020 2020 2020 2020  inds,.          
+00006bb0: 2020 2020 2020 696e 636c 7564 655f 6d65        include_me
+00006bc0: 7461 6461 7461 3d54 7275 6529 0a20 2020  tadata=True).   
+00006bd0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00006be0: 2020 2020 2020 2020 2020 2320 6368 6563            # chec
+00006bf0: 6b20 6966 2072 6561 6469 6e67 2065 7272  k if reading err
+00006c00: 6f72 0a20 2020 2020 2020 2020 2020 2069  or.            i
+00006c10: 6620 696e 666f 5b27 7265 6164 5f73 7461  f info['read_sta
+00006c20: 7475 7327 5d3e 303a 0a20 2020 2020 2020  tus']>0:.       
+00006c30: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00006c40: 5741 524e 494e 473a 2055 6e61 626c 6520  WARNING: Unable 
+00006c50: 746f 2072 6561 6420 6576 656e 7420 2327  to read event #'
+00006c60: 202b 2073 7472 2869 6576 656e 7429 202b   + str(ievent) +
+00006c70: 2027 2120 4572 726f 7220 6d65 7373 6167   '! Error messag
+00006c80: 653a 2027 290a 2020 2020 2020 2020 2020  e: ').          
+00006c90: 2020 2020 2020 7072 696e 7428 2757 4152        print('WAR
+00006ca0: 4e49 4e47 3a20 2227 202b 2069 6e66 6f5b  NING: "' + info[
+00006cb0: 2765 7272 6f72 5f6d 7367 275d 202b 2027  'error_msg'] + '
+00006cc0: 222e 2053 746f 7070 696e 6720 6576 656e  ". Stopping even
+00006cd0: 7420 6c6f 6f70 2729 0a20 2020 2020 2020  t loop').       
+00006ce0: 2020 2020 2020 2020 2062 7265 616b 0a0a           break..
+00006cf0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00006d00: 2020 2020 2020 2020 2023 2061 6464 2074           # add t
+00006d10: 6f20 6d65 7461 6461 7461 206c 6973 740a  o metadata list.
+00006d20: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00006d30: 6e63 6c75 6465 5f6d 6574 6164 6174 613a  nclude_metadata:
+00006d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006d50: 2069 6e66 6f5f 6c69 7374 2e61 7070 656e   info_list.appen
+00006d60: 6428 696e 666f 290a 0a20 2020 2020 2020  d(info)..       
+00006d70: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+00006d80: 2020 2320 7374 6f72 650a 2020 2020 2020    # store.      
+00006d90: 2020 2020 2020 6966 2028 6f75 7470 7574        if (output
+00006da0: 5f66 6f72 6d61 743d 3d31 206f 7220 6f75  _format==1 or ou
+00006db0: 7470 7574 5f66 6f72 6d61 743d 3d33 293a  tput_format==3):
+00006dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006dd0: 206f 7574 7075 745f 6461 7461 2e61 7070   output_data.app
+00006de0: 656e 6428 7472 6163 6573 290a 2020 2020  end(traces).    
+00006df0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00006e00: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00006e10: 7470 7574 5f64 6174 615b 6965 7665 6e74  tput_data[ievent
+00006e20: 2c3a 2c3a 5d20 3d20 7472 6163 6573 0a20  ,:,:] = traces. 
+00006e30: 2020 2020 2020 2020 2020 2020 2020 200a                 .
+00006e40: 0a20 2020 2020 2020 2023 2072 6573 6574  .        # reset
+00006e50: 2066 696c 6520 6c69 7374 2074 6f20 6f72   file list to or
+00006e60: 6967 696e 616c 206c 6973 740a 2020 2020  iginal list.    
+00006e70: 2020 2020 2320 6966 206e 6565 6465 640a      # if needed.
+00006e80: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
+00006e90: 6172 2829 0a20 2020 2020 2020 2073 656c  ar().        sel
+00006ea0: 662e 5f66 696c 655f 6469 6374 203d 2063  f._file_dict = c
+00006eb0: 7572 7265 6e74 5f66 696c 655f 6469 6374  urrent_file_dict
+00006ec0: 0a0a 0a20 2020 2020 2020 2069 6620 696e  ...        if in
+00006ed0: 636c 7564 655f 6d65 7461 6461 7461 3a0a  clude_metadata:.
+00006ee0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00006ef0: 726e 206f 7574 7075 745f 6461 7461 2c20  rn output_data, 
+00006f00: 696e 666f 5f6c 6973 740a 2020 2020 2020  info_list.      
+00006f10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00006f20: 2020 2020 7265 7475 726e 206f 7574 7075      return outpu
+00006f30: 745f 6461 7461 0a20 2020 2020 2020 200a  t_data.        .
+00006f40: 2020 2020 2020 2020 2020 2020 200a 0a20               .. 
+00006f50: 2020 2064 6566 2067 6574 5f63 7572 7265     def get_curre
+00006f60: 6e74 5f66 696c 655f 6e61 6d65 2873 656c  nt_file_name(sel
+00006f70: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00006f80: 2020 2020 2020 2020 4765 7420 6375 7272          Get curr
+00006f90: 656e 7420 6669 6c65 206e 616d 650a 2020  ent file name.  
+00006fa0: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
+00006fb0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00006fc0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00006fd0: 2020 2020 204e 6f6e 650a 0a0a 2020 2020       None...    
+00006fe0: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
+00006ff0: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
+00007000: 2020 0a20 2020 2020 2020 2066 696c 655f    .        file_
+00007010: 6e61 6d65 203a 2073 7472 0a20 2020 2020  name : str.     
+00007020: 2020 2020 2063 7572 7265 6e74 2066 696c       current fil
+00007030: 6520 6e61 6d65 0a0a 2020 2020 2020 2020  e name..        
+00007040: 2222 220a 2020 2020 2020 2020 0a20 2020  """.        .   
+00007050: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00007060: 2e5f 6375 7272 656e 745f 6669 6c65 5f6e  ._current_file_n
+00007070: 616d 650a 2020 2020 2020 2020 0a0a 0a20  ame.        ... 
+00007080: 2020 200a 2020 2020 6465 6620 6765 745f     .    def get_
+00007090: 6d65 7461 6461 7461 2873 656c 662c 2066  metadata(self, f
+000070a0: 696c 655f 6e61 6d65 3d4e 6f6e 652c 2067  ile_name=None, g
+000070b0: 726f 7570 5f6e 616d 653d 4e6f 6e65 2c20  roup_name=None, 
+000070c0: 6461 7461 7365 745f 6e61 6d65 3d4e 6f6e  dataset_name=Non
+000070d0: 652c 200a 2020 2020 2020 2020 2020 2020  e, .            
+000070e0: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
+000070f0: 5f64 6174 6173 6574 5f6d 6574 6164 6174  _dataset_metadat
+00007100: 613d 4661 6c73 6529 3a0a 0a20 2020 2020  a=False):..     
+00007110: 2020 2022 2222 0a20 2020 2020 2020 2046     """.        F
+00007120: 756e 6374 696f 6e20 746f 2067 6574 206d  unction to get m
+00007130: 6574 6164 6174 612e 0a20 2020 2020 2020  etadata..       
+00007140: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00007150: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00007160: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2020  ------.         
+00007170: 200a 2020 2020 2020 2020 6669 6c65 5f6e   .        file_n
+00007180: 616d 653a 2073 7472 696e 672c 206f 7074  ame: string, opt
+00007190: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+000071a0: 2020 6966 206e 6f20 6669 6c65 206e 616d    if no file nam
+000071b0: 6520 7072 6f76 6964 6564 3a20 7573 6520  e provided: use 
+000071c0: 6375 7272 656e 7420 6669 6c65 0a0a 2020  current file..  
+000071d0: 2020 2020 2020 6772 6f75 705f 6e61 6d65        group_name
+000071e0: 3a20 2073 7472 696e 672c 206f 7074 696f  :  string, optio
+000071f0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+00007200: 4835 2022 4772 6f75 7022 206e 616d 650a  H5 "Group" name.
+00007210: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00007220: 756c 743a 204e 6f6e 652c 2072 6561 6420  ult: None, read 
+00007230: 616c 6c20 6772 6f75 7073 0a20 2020 2020  all groups.     
+00007240: 2020 2020 200a 2020 2020 2020 2020 6461       .        da
+00007250: 7461 7365 745f 6e61 6d65 3a20 7374 7269  taset_name: stri
+00007260: 6e67 2c20 6f70 7469 6f6e 616c 2c20 0a20  ng, optional, . 
+00007270: 2020 2020 2020 2020 2020 2048 3520 2244             H5 "D
+00007280: 6174 6173 6574 2220 6e61 6d65 0a20 2020  ataset" name.   
+00007290: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+000072a0: 3a20 616c 6c20 6461 7461 7365 7473 0a20  : all datasets. 
+000072b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000072c0: 2069 6e63 6c75 6465 5f64 6174 6173 6574   include_dataset
+000072d0: 5f6d 6574 6164 6174 6120 3a20 626f 6f6c  _metadata : bool
+000072e0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+000072f0: 2020 2020 2020 2049 6620 5472 7565 2c20         If True, 
+00007300: 696e 636c 7564 6520 6461 7461 7365 7420  include dataset 
+00007310: 6d65 7461 6461 7461 0a20 2020 2020 2020  metadata.       
+00007320: 2020 2020 2044 6566 6175 6c74 3a20 4661       Default: Fa
+00007330: 6c73 650a 2020 2020 2020 2020 0a0a 2020  lse.        ..  
+00007340: 2020 2020 2020 5265 7475 726e 0a20 2020        Return.   
+00007350: 2020 2020 202d 2d2d 2d2d 2d0a 2020 2020       ------.    
+00007360: 2020 2020 0a20 2020 2020 2020 206d 6574      .        met
+00007370: 6164 6174 613a 2064 6963 740a 2020 2020  adata: dict.    
+00007380: 2020 2020 2020 2064 6963 7469 6f6e 6172         dictionar
+00007390: 7920 7769 7468 2061 6c6c 206d 6574 6164  y with all metad
+000073a0: 6174 610a 0a20 2020 2020 2020 2022 2222  ata..        """
+000073b0: 0a0a 2020 2020 2020 2020 6d65 7461 6461  ..        metada
+000073c0: 7461 203d 2064 6963 7428 290a 0a0a 2020  ta = dict()...  
+000073d0: 2020 2020 2020 2320 6368 6563 6b20 696e        # check in
+000073e0: 7075 7420 0a20 2020 2020 2020 2069 6620  put .        if 
+000073f0: 6669 6c65 5f6e 616d 6520 6973 204e 6f6e  file_name is Non
+00007400: 6520 616e 6420 7365 6c66 2e5f 6375 7272  e and self._curr
+00007410: 656e 745f 6669 6c65 2069 7320 4e6f 6e65  ent_file is None
+00007420: 3a0a 2020 2020 2020 2020 2020 2020 6572  :.            er
+00007430: 726f 725f 6d73 6720 3d20 274e 6f20 6669  ror_msg = 'No fi
+00007440: 6c65 2063 7572 7265 6e74 6c79 206f 7065  le currently ope
+00007450: 6e20 616e 6420 6e6f 2022 6669 6c65 5f6e  n and no "file_n
+00007460: 616d 6522 2061 7267 756d 656e 7420 6e6f  ame" argument no
+00007470: 7420 7072 6f76 6964 6564 2127 0a20 2020  t provided!'.   
+00007480: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00007490: 2e5f 7261 6973 655f 6572 726f 7273 3a0a  ._raise_errors:.
+000074a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074b0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+000074c0: 7272 6f72 2865 7272 6f72 5f6d 7367 290a  rror(error_msg).
+000074d0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000074e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000074f0: 2020 7072 696e 7428 2745 5252 4f52 3a20    print('ERROR: 
+00007500: 2720 2b20 6572 726f 725f 6d73 6729 0a20  ' + error_msg). 
+00007510: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00007520: 7269 6e74 2827 506c 6561 7365 206f 7065  rint('Please ope
+00007530: 6e20 6120 6669 6c65 206f 7220 7072 6f76  n a file or prov
+00007540: 6964 6520 6120 6669 6c65 206e 616d 6521  ide a file name!
+00007550: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00007560: 2020 2072 6574 7572 6e20 6d65 7461 6461     return metada
+00007570: 7461 0a0a 2020 2020 2020 2020 2320 6f70  ta..        # op
+00007580: 656e 2066 696c 6520 6966 206e 6565 6465  en file if neede
+00007590: 640a 2020 2020 2020 2020 6966 2028 6669  d.        if (fi
+000075a0: 6c65 5f6e 616d 6520 6973 206e 6f74 204e  le_name is not N
+000075b0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000075c0: 616e 6420 7365 6c66 2e5f 6375 7272 656e  and self._curren
+000075d0: 745f 6669 6c65 5f6e 616d 6521 3d66 696c  t_file_name!=fil
+000075e0: 655f 6e61 6d65 293a 0a20 2020 2020 2020  e_name):.       
+000075f0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+00007600: 2020 2320 6368 6563 6b20 6966 2061 2066    # check if a f
+00007610: 696c 6520 616c 7265 6164 7920 6f70 656e  ile already open
+00007620: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00007630: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+00007640: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
+00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 7365 6c66 2e5f 636c 6f73 655f 6669 6c65  self._close_file
+00007670: 2829 0a20 2020 2020 2020 2020 2020 2023  ().            #
+00007680: 206f 7065 6e0a 2020 2020 2020 2020 2020   open.          
+00007690: 2020 7365 6c66 2e5f 6f70 656e 5f66 696c    self._open_fil
+000076a0: 6528 6669 6c65 5f6e 616d 652c 2065 7665  e(file_name, eve
+000076b0: 6e74 5f6c 6973 743d 4e6f 6e65 2c0a 2020  nt_list=None,.  
+000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076d0: 2020 2020 2020 2020 2020 6c6f 6164 5f6d            load_m
+000076e0: 6574 6164 6174 613d 4661 6c73 6529 0a20  etadata=False). 
+000076f0: 2020 2020 2020 2020 2020 200a 0a20 2020             ..   
+00007700: 2020 2020 2023 206c 6f61 6420 6d65 7461       # load meta
+00007710: 6461 7461 2028 6966 2022 6461 7461 7365  data (if "datase
+00007720: 7422 206d 6574 6164 6174 6120 7265 7175  t" metadata requ
+00007730: 6573 7465 6420 2d3e 2072 656c 6f61 6429  ested -> reload)
+00007740: 0a20 2020 2020 2020 2069 6620 6461 7461  .        if data
+00007750: 7365 745f 6e61 6d65 2069 7320 6e6f 7420  set_name is not 
+00007760: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00007770: 2020 696e 636c 7564 655f 6461 7461 7365    include_datase
+00007780: 745f 6d65 7461 6461 7461 203d 2054 7275  t_metadata = Tru
+00007790: 650a 0a20 2020 2020 2020 2069 6620 7365  e..        if se
+000077a0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+000077b0: 5f6d 6574 6164 6174 6120 6973 204e 6f6e  _metadata is Non
+000077c0: 6520 6f72 2069 6e63 6c75 6465 5f64 6174  e or include_dat
+000077d0: 6173 6574 5f6d 6574 6164 6174 613a 0a20  aset_metadata:. 
+000077e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000077f0: 5f6c 6f61 645f 6d65 7461 6461 7461 2869  _load_metadata(i
+00007800: 6e63 6c75 6465 5f64 6174 6173 6574 5f6d  nclude_dataset_m
+00007810: 6574 6164 6174 6129 0a20 2020 2020 2020  etadata).       
+00007820: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00007830: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00007840: 2066 696e 6420 7370 6563 6966 6963 206d   find specific m
+00007850: 6574 6164 6174 610a 2020 2020 2020 2020  etadata.        
+00007860: 6d65 7461 6461 7461 203d 2064 6963 7428  metadata = dict(
+00007870: 290a 2020 2020 2020 2020 6966 2067 726f  ).        if gro
+00007880: 7570 5f6e 616d 6520 6973 206e 6f74 204e  up_name is not N
+00007890: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000078a0: 2069 6620 6772 6f75 705f 6e61 6d65 2069   if group_name i
+000078b0: 6e20 7365 6c66 2e5f 6375 7272 656e 745f  n self._current_
+000078c0: 6669 6c65 5f6d 6574 6164 6174 615b 2767  file_metadata['g
+000078d0: 726f 7570 5f6c 6973 7427 5d3a 0a20 2020  roup_list']:.   
+000078e0: 2020 2020 2020 2020 2020 2020 2067 726f               gro
+000078f0: 7570 5f6d 6574 6164 6174 6120 3d20 7365  up_metadata = se
+00007900: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+00007910: 5f6d 6574 6164 6174 615b 2767 726f 7570  _metadata['group
+00007920: 7327 5d5b 6772 6f75 705f 6e61 6d65 5d0a  s'][group_name].
+00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007940: 6966 2064 6174 6173 6574 5f6e 616d 6520  if dataset_name 
+00007950: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007970: 2069 6620 6461 7461 7365 745f 6e61 6d65   if dataset_name
+00007980: 2069 6e20 6772 6f75 705f 6d65 7461 6461   in group_metada
+00007990: 7461 5b27 6461 7461 7365 745f 6c69 7374  ta['dataset_list
+000079a0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+000079b0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+000079c0: 6461 7461 203d 2067 726f 7570 5f6d 6574  data = group_met
+000079d0: 6164 6174 615b 2764 6174 6173 6574 7327  adata['datasets'
+000079e0: 5d5b 6461 7461 7365 745f 6e61 6d65 5d0a  ][dataset_name].
+000079f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00007a10: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+00007a20: 7461 203d 2067 726f 7570 5f6d 6574 6164  ta = group_metad
+00007a30: 6174 610a 2020 2020 2020 2020 656c 7365  ata.        else
+00007a40: 3a0a 2020 2020 2020 2020 2020 2020 6d65  :.            me
+00007a50: 7461 6461 7461 203d 2073 656c 662e 5f63  tadata = self._c
+00007a60: 7572 7265 6e74 5f66 696c 655f 6d65 7461  urrent_file_meta
+00007a70: 6461 7461 0a0a 0a20 2020 2020 2020 2023  data...        #
+00007a80: 2063 6c6f 7365 2066 696c 650a 2020 2020   close file.    
+00007a90: 2020 2020 6966 2066 696c 655f 6e61 6d65      if file_name
+00007aa0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00007ab0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00007ac0: 636c 6f73 655f 6669 6c65 2829 0a20 2020  close_file().   
+00007ad0: 2020 2020 200a 0a20 2020 2020 2020 2072       ..        r
+00007ae0: 6574 7572 6e20 6d65 7461 6461 7461 0a20  eturn metadata. 
+00007af0: 2020 2020 2020 2020 2020 200a 0a0a 0a20             .... 
+00007b00: 2020 2064 6566 2067 6574 5f64 6574 6563     def get_detec
+00007b10: 746f 725f 636f 6e66 6967 2873 656c 662c  tor_config(self,
+00007b20: 2066 696c 655f 6e61 6d65 3d4e 6f6e 652c   file_name=None,
+00007b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b40: 2020 2020 2020 2020 2020 2020 2061 6463               adc
+00007b50: 5f6e 616d 653d 2761 6463 3127 2c0a 2020  _name='adc1',.  
+00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b70: 2020 2020 2020 2020 2020 7573 655f 6368            use_ch
+00007b80: 616e 5f64 6963 743d 5472 7565 293a 2020  an_dict=True):  
+00007b90: 200a 2020 2020 2020 2020 2222 220a 2020   .        """.  
+00007ba0: 2020 2020 2020 4765 7420 6465 7465 6374        Get detect
+00007bb0: 6f72 2063 6f6e 6669 6775 7261 7469 6f6e  or configuration
+00007bc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007bd0: 2020 2020 200a 2020 2020 2020 2020 6465       .        de
+00007be0: 7465 6374 6f72 5f63 6f6e 6669 6720 3d20  tector_config = 
+00007bf0: 6469 6374 2829 0a20 2020 2020 2020 200a  dict().        .
+00007c00: 2020 2020 2020 2020 2320 6765 7420 6d65          # get me
+00007c10: 7461 6461 7461 0a20 2020 2020 2020 206d  tadata.        m
+00007c20: 6574 6164 6174 6120 3d20 4e6f 6e65 0a20  etadata = None. 
+00007c30: 2020 2020 2020 2069 6620 6669 6c65 5f6e         if file_n
+00007c40: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+00007c50: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+00007c60: 6164 6174 6120 3d20 7365 6c66 2e67 6574  adata = self.get
+00007c70: 5f6d 6574 6164 6174 6128 6669 6c65 5f6e  _metadata(file_n
+00007c80: 616d 653d 6669 6c65 5f6e 616d 6529 0a20  ame=file_name). 
+00007c90: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+00007ca0: 2e5f 6375 7272 656e 745f 6669 6c65 5f6d  ._current_file_m
+00007cb0: 6574 6164 6174 6120 6973 206e 6f74 204e  etadata is not N
+00007cc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007cd0: 206d 6574 6164 6174 6120 3d20 7365 6c66   metadata = self
+00007ce0: 2e5f 6375 7272 656e 745f 6669 6c65 5f6d  ._current_file_m
+00007cf0: 6574 6164 6174 610a 2020 2020 2020 2020  etadata.        
+00007d00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00007d10: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00007d20: 6f72 2827 4552 524f 5220 696e 2067 6574  or('ERROR in get
+00007d30: 5f64 6574 6563 746f 725f 636f 6e66 6967  _detector_config
+00007d40: 3a20 6120 6669 6c65 206e 616d 6520 6e65  : a file name ne
+00007d50: 6564 7320 746f 2062 6520 7072 6f76 6964  eds to be provid
+00007d60: 6564 2127 290a 2020 2020 2020 2020 0a20  ed!').        . 
+00007d70: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
+00007d80: 2023 2063 6f6e 6669 6720 6e61 6d65 0a20   # config name. 
+00007d90: 2020 2020 2020 2063 6f6e 6669 675f 6e61         config_na
+00007da0: 6d65 203d 2027 6465 7463 6f6e 6669 6731  me = 'detconfig1
+00007db0: 270a 2020 2020 2020 2020 6966 2061 6463  '.        if adc
+00007dc0: 5f6e 616d 6521 3d27 6164 6331 273a 0a20  _name!='adc1':. 
+00007dd0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00007de0: 675f 6e61 6d65 203d 2027 6465 7463 6f6e  g_name = 'detcon
+00007df0: 6669 6727 202b 2061 6463 5f6e 616d 655b  fig' + adc_name[
+00007e00: 333a 5d0a 0a20 2020 2020 2020 2023 2063  3:]..        # c
+00007e10: 6865 636b 2069 6620 6176 6169 6c61 626c  heck if availabl
+00007e20: 650a 2020 2020 2020 2020 6966 2063 6f6e  e.        if con
+00007e30: 6669 675f 6e61 6d65 206e 6f74 2069 6e20  fig_name not in 
+00007e40: 6d65 7461 6461 7461 5b27 6772 6f75 705f  metadata['group_
+00007e50: 6c69 7374 275d 3a0a 2020 2020 2020 2020  list']:.        
+00007e60: 2020 2020 7072 696e 7428 2745 5252 4f52      print('ERROR
+00007e70: 3a20 756e 6162 6c65 2074 6f20 6669 6e64  : unable to find
+00007e80: 2064 6574 6563 746f 7220 636f 6e66 6967   detector config
+00007e90: 2127 290a 2020 2020 2020 2020 2020 2020  !').            
+00007ea0: 7265 7475 726e 205b 5d0a 0a20 2020 2020  return []..     
+00007eb0: 2020 2023 2067 726f 7570 206d 6574 6164     # group metad
+00007ec0: 6174 610a 2020 2020 2020 2020 6465 7465  ata.        dete
+00007ed0: 6374 6f72 5f63 6f6e 6669 675f 6469 6374  ctor_config_dict
+00007ee0: 203d 206d 6574 6164 6174 615b 2767 726f   = metadata['gro
+00007ef0: 7570 7327 5d5b 636f 6e66 6967 5f6e 616d  ups'][config_nam
+00007f00: 655d 0a20 2020 2020 2020 2023 6966 2027  e].        #if '
+00007f10: 6164 635f 6e61 6d65 2720 696e 2064 6574  adc_name' in det
+00007f20: 6563 746f 725f 636f 6e66 6967 5f64 6963  ector_config_dic
+00007f30: 7420 616e 6420 6164 635f 6e61 6d65 213d  t and adc_name!=
+00007f40: 6465 7465 6374 6f72 5f63 6f6e 6669 675f  detector_config_
+00007f50: 6469 6374 5b27 6164 635f 6e61 6d65 275d  dict['adc_name']
+00007f60: 3a0a 2020 2020 2020 2020 2320 2020 2070  :.        #    p
+00007f70: 7269 6e74 2827 4552 524f 523a 2055 6e65  rint('ERROR: Une
+00007f80: 7870 6563 7465 6420 6465 7465 6374 6f72  xpected detector
+00007f90: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00007fa0: 6f72 6d61 7421 2729 0a20 2020 2020 2020  ormat!').       
+00007fb0: 2023 2020 2020 7265 7475 726e 205b 5d0a   #    return [].
+00007fc0: 0a0a 2020 2020 2020 2020 2320 6164 6420  ..        # add 
+00007fd0: 6465 7465 6374 6f72 2f63 6861 6e6e 656c  detector/channel
+00007fe0: 206c 6973 7420 6672 6f6d 2061 6463 206d   list from adc m
+00007ff0: 6574 6164 6174 612c 206e 6565 6473 2074  etadata, needs t
+00008000: 6f20 6d61 7463 680a 2020 2020 2020 2020  o match.        
+00008010: 2320 6465 7465 6374 6f72 2073 6574 7469  # detector setti
+00008020: 6e67 7320 6172 7261 7920 6f72 6465 720a  ngs array order.
+00008030: 2020 2020 2020 2020 7465 735f 6368 616e          tes_chan
+00008040: 7320 3d20 6c69 7374 2829 0a20 2020 2020  s = list().     
+00008050: 2020 2064 6574 6563 746f 725f 6368 616e     detector_chan
+00008060: 7320 3d20 6c69 7374 2829 0a20 2020 2020  s = list().     
+00008070: 2020 2063 6f6e 7472 6f6c 6c65 725f 6368     controller_ch
+00008080: 616e 7320 3d20 6c69 7374 2829 0a20 2020  ans = list().   
+00008090: 2020 2020 2063 6f6e 6e65 6374 696f 6e5f       connection_
+000080a0: 6469 6374 203d 2073 656c 662e 6765 745f  dict = self.get_
+000080b0: 636f 6e6e 6563 7469 6f6e 5f64 6963 7428  connection_dict(
+000080c0: 6164 635f 6e61 6d65 3d61 6463 5f6e 616d  adc_name=adc_nam
+000080d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008100: 2020 2020 2020 6d65 7461 6461 7461 3d6d        metadata=m
+00008110: 6574 6164 6174 6129 0a0a 2020 2020 2020  etadata)..      
+00008120: 2020 6966 2063 6f6e 6e65 6374 696f 6e5f    if connection_
+00008130: 6469 6374 3a0a 2020 2020 2020 2020 2020  dict:.          
+00008140: 2020 6368 616e 5f6c 6973 7420 3d20 6465    chan_list = de
+00008150: 7465 6374 6f72 5f63 6f6e 6669 675f 6469  tector_config_di
+00008160: 6374 5b27 6368 616e 6e65 6c5f 6c69 7374  ct['channel_list
+00008170: 275d 0a20 2020 2020 2020 2020 2020 2069  '].            i
+00008180: 6620 286e 6f74 2069 7369 6e73 7461 6e63  f (not isinstanc
+00008190: 6528 6368 616e 5f6c 6973 742c 206e 702e  e(chan_list, np.
+000081a0: 6e64 6172 7261 7929 0a20 2020 2020 2020  ndarray).       
+000081b0: 2020 2020 2020 2020 2061 6e64 206e 6f74           and not
+000081c0: 2069 7369 6e73 7461 6e63 6528 6368 616e   isinstance(chan
+000081d0: 5f6c 6973 742c 206c 6973 7429 293a 0a20  _list, list)):. 
+000081e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000081f0: 6861 6e5f 6c69 7374 2020 3d20 5b63 6861  han_list  = [cha
+00008200: 6e5f 6c69 7374 5d0a 2020 2020 2020 2020  n_list].        
+00008210: 2020 2020 666f 7220 6368 616e 2069 6e20      for chan in 
+00008220: 6368 616e 5f6c 6973 743a 0a20 2020 2020  chan_list:.     
+00008230: 2020 2020 2020 2020 2020 2069 6620 6368             if ch
+00008240: 616e 2069 6e20 636f 6e6e 6563 7469 6f6e  an in connection
+00008250: 5f64 6963 745b 2761 6463 5f63 6861 6e73  _dict['adc_chans
+00008260: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+00008270: 2020 2020 2020 2020 696e 6420 3d20 636f          ind = co
+00008280: 6e6e 6563 7469 6f6e 5f64 6963 745b 2761  nnection_dict['a
+00008290: 6463 5f63 6861 6e73 275d 2e69 6e64 6578  dc_chans'].index
+000082a0: 2869 6e74 2863 6861 6e29 290a 2020 2020  (int(chan)).    
+000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082c0: 6966 2063 6f6e 6e65 6374 696f 6e5f 6469  if connection_di
+000082d0: 6374 5b27 636f 6e74 726f 6c6c 6572 5f63  ct['controller_c
+000082e0: 6861 6e73 275d 3a0a 2020 2020 2020 2020  hans']:.        
 000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008300: 2020 2074 6573 5f63 6861 6e73 2e61 7070     tes_chans.app
-00008310: 656e 6428 636f 6e6e 6563 7469 6f6e 5f64  end(connection_d
-00008320: 6963 745b 2774 6573 5f63 6861 6e73 275d  ict['tes_chans']
-00008330: 5b69 6e64 5d29 0a20 2020 2020 2020 2020  [ind]).         
-00008340: 2020 2020 2020 2020 2020 2069 6620 636f             if co
-00008350: 6e6e 6563 7469 6f6e 5f64 6963 745b 2764  nnection_dict['d
-00008360: 6574 6563 746f 725f 6368 616e 7327 5d3a  etector_chans']:
-00008370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008380: 2020 2020 2020 2020 2064 6574 6563 746f           detecto
-00008390: 725f 6368 616e 732e 6170 7065 6e64 2863  r_chans.append(c
-000083a0: 6f6e 6e65 6374 696f 6e5f 6469 6374 5b27  onnection_dict['
-000083b0: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
-000083c0: 5b69 6e64 5d29 0a20 2020 2020 2020 2020  [ind]).         
-000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008400: 200a 2020 2020 2020 2020 6465 7465 6374   .        detect
-00008410: 6f72 5f63 6f6e 6669 675f 6469 6374 5b27  or_config_dict['
-00008420: 7465 735f 6368 616e 7327 5d20 3d20 2074  tes_chans'] =  t
-00008430: 6573 5f63 6861 6e73 0a20 2020 2020 2020  es_chans.       
-00008440: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
-00008450: 5f64 6963 745b 2764 6574 6563 746f 725f  _dict['detector_
-00008460: 6368 616e 7327 5d20 3d20 2064 6574 6563  chans'] =  detec
-00008470: 746f 725f 6368 616e 730a 2020 2020 2020  tor_chans.      
-00008480: 2020 6465 7465 6374 6f72 5f63 6f6e 6669    detector_confi
-00008490: 675f 6469 6374 5b27 636f 6e74 726f 6c6c  g_dict['controll
-000084a0: 6572 5f63 6861 6e73 275d 203d 2020 636f  er_chans'] =  co
-000084b0: 6e74 726f 6c6c 6572 5f63 6861 6e73 2020  ntroller_chans  
-000084c0: 200a 0a20 2020 2020 2020 2023 2063 6f6e   ..        # con
-000084d0: 7665 7274 2074 6f20 6c69 7374 2069 6620  vert to list if 
-000084e0: 6e65 6564 6564 2028 7369 7a65 206f 6620  needed (size of 
-000084f0: 6e62 2063 6861 6e6e 656c 7329 0a20 2020  nb channels).   
-00008500: 2020 2020 206e 625f 6368 616e 203d 206c       nb_chan = l
-00008510: 656e 2864 6574 6563 746f 725f 636f 6e66  en(detector_conf
-00008520: 6967 5f64 6963 745b 2764 6574 6563 746f  ig_dict['detecto
-00008530: 725f 6368 616e 7327 5d29 0a20 2020 2020  r_chans']).     
-00008540: 2020 2066 6f72 2063 6f6e 6669 6720 696e     for config in
-00008550: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
-00008560: 5f64 6963 742e 6b65 7973 2829 3a0a 2020  _dict.keys():.  
-00008570: 2020 2020 2020 2020 2020 7061 7261 6d20            param 
-00008580: 3d20 6465 7465 6374 6f72 5f63 6f6e 6669  = detector_confi
-00008590: 675f 6469 6374 5b63 6f6e 6669 675d 0a20  g_dict[config]. 
-000085a0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000085b0: 7420 6973 696e 7374 616e 6365 2870 6172  t isinstance(par
-000085c0: 616d 2c20 6c69 7374 2920 616e 6420 6e6f  am, list) and no
-000085d0: 7420 6973 696e 7374 616e 6365 2870 6172  t isinstance(par
-000085e0: 616d 2c20 6e70 2e6e 6461 7272 6179 293a  am, np.ndarray):
-000085f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008600: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
-00008610: 5f64 6963 745b 636f 6e66 6967 5d20 3d20  _dict[config] = 
-00008620: 5b64 6574 6563 746f 725f 636f 6e66 6967  [detector_config
-00008630: 5f64 6963 745b 636f 6e66 6967 5d5d 2a6e  _dict[config]]*n
-00008640: 625f 6368 616e 0a20 2020 200a 2020 2020  b_chan.    .    
-00008650: 2020 2020 2320 636f 6e76 6572 7420 746f      # convert to
-00008660: 2064 6963 7469 6f6e 6172 790a 2020 2020   dictionary.    
-00008670: 2020 2020 6465 7465 6374 6f72 5f63 6f6e      detector_con
-00008680: 6669 6720 3d20 6469 6374 2829 0a20 2020  fig = dict().   
-00008690: 2020 2020 2069 6620 7573 655f 6368 616e       if use_chan
-000086a0: 5f64 6963 743a 0a20 2020 2020 2020 2020  _dict:.         
-000086b0: 2020 2063 6861 6e5f 6c69 7374 203d 2064     chan_list = d
-000086c0: 6574 6563 746f 725f 636f 6e66 6967 5f64  etector_config_d
-000086d0: 6963 745b 2764 6574 6563 746f 725f 6368  ict['detector_ch
-000086e0: 616e 7327 5d0a 2020 2020 2020 2020 2020  ans'].          
-000086f0: 2020 666f 7220 6368 616e 2069 6e20 6368    for chan in ch
-00008700: 616e 5f6c 6973 743a 0a20 2020 2020 2020  an_list:.       
-00008710: 2020 2020 2020 2020 2063 6861 6e5f 696e           chan_in
-00008720: 6465 7820 3d20 6465 7465 6374 6f72 5f63  dex = detector_c
-00008730: 6f6e 6669 675f 6469 6374 5b27 6465 7465  onfig_dict['dete
-00008740: 6374 6f72 5f63 6861 6e73 275d 2e69 6e64  ctor_chans'].ind
-00008750: 6578 2863 6861 6e29 0a20 2020 2020 2020  ex(chan).       
-00008760: 2020 2020 2020 2020 2064 6574 6563 746f           detecto
-00008770: 725f 636f 6e66 6967 5b63 6861 6e5d 203d  r_config[chan] =
-00008780: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00008790: 2020 2020 2020 2020 666f 7220 636f 6e66          for conf
-000087a0: 6967 2069 6e20 6465 7465 6374 6f72 5f63  ig in detector_c
-000087b0: 6f6e 6669 675f 6469 6374 3a0a 2020 2020  onfig_dict:.    
-000087c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087d0: 6966 206c 656e 2864 6574 6563 746f 725f  if len(detector_
-000087e0: 636f 6e66 6967 5f64 6963 745b 636f 6e66  config_dict[conf
-000087f0: 6967 5d29 3d3d 6e62 5f63 6861 6e3a 0a20  ig])==nb_chan:. 
-00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 2020 2020 2020 2064 6574 6563 746f 725f         detector_
-00008820: 636f 6e66 6967 5b63 6861 6e5d 5b63 6f6e  config[chan][con
-00008830: 6669 675d 203d 2064 6574 6563 746f 725f  fig] = detector_
-00008840: 636f 6e66 6967 5f64 6963 745b 636f 6e66  config_dict[conf
-00008850: 6967 5d5b 6368 616e 5f69 6e64 6578 5d0a  ig][chan_index].
-00008860: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00008870: 2020 2020 2020 2020 2020 6465 7465 6374            detect
-00008880: 6f72 5f63 6f6e 6669 6720 3d20 6465 7465  or_config = dete
-00008890: 6374 6f72 5f63 6f6e 6669 675f 6469 6374  ctor_config_dict
-000088a0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-000088b0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088d0: 200a 2020 2020 2020 2020 7265 7475 726e   .        return
-000088e0: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
-000088f0: 0a0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008910: 2020 2020 2020 200a 2020 2020 6465 6620         .    def 
-00008920: 6765 745f 636f 6e6e 6563 7469 6f6e 5f64  get_connection_d
-00008930: 6963 7428 7365 6c66 2c20 6669 6c65 5f6e  ict(self, file_n
-00008940: 616d 653d 4e6f 6e65 2c20 6164 635f 6e61  ame=None, adc_na
-00008950: 6d65 3d27 6164 6331 272c 206d 6574 6164  me='adc1', metad
-00008960: 6174 613d 4e6f 6e65 293a 0a20 2020 2020  ata=None):.     
-00008970: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-00008980: 6574 2063 6f6e 6e65 6374 696f 6e20 6469  et connection di
-00008990: 6374 696f 6e61 7279 2066 6f72 2073 7065  ctionary for spe
-000089a0: 6369 6669 6420 6164 6320 6e61 6d65 0a20  cifid adc name. 
-000089b0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-000089c0: 2020 2020 2320 696e 6974 6961 6c69 7a65      # initialize
-000089d0: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
-000089e0: 696f 6e5f 6469 6374 3d64 6963 7428 290a  ion_dict=dict().
-000089f0: 0a20 2020 2020 2020 2023 206d 6574 6164  .        # metad
-00008a00: 6174 610a 2020 2020 2020 2020 6164 635f  ata.        adc_
-00008a10: 6d65 7461 6461 7461 203d 204e 6f6e 650a  metadata = None.
-00008a20: 2020 2020 2020 2020 6966 206d 6574 6164          if metad
-00008a30: 6174 6120 6973 204e 6f6e 6520 6f72 2027  ata is None or '
-00008a40: 6772 6f75 705f 6c69 7374 2720 6e6f 7420  group_list' not 
-00008a50: 696e 206d 6574 6164 6174 613a 0a20 2020  in metadata:.   
-00008a60: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-00008a70: 6120 3d20 7365 6c66 2e67 6574 5f6d 6574  a = self.get_met
-00008a80: 6164 6174 6128 6669 6c65 5f6e 616d 653d  adata(file_name=
-00008a90: 6669 6c65 5f6e 616d 6529 0a0a 2020 2020  file_name)..    
-00008aa0: 2020 2020 6966 2027 6772 6f75 705f 6c69      if 'group_li
-00008ab0: 7374 2720 696e 206d 6574 6164 6174 6120  st' in metadata 
-00008ac0: 616e 6420 6164 635f 6e61 6d65 2069 6e20  and adc_name in 
-00008ad0: 6d65 7461 6461 7461 5b27 6772 6f75 705f  metadata['group_
-00008ae0: 6c69 7374 275d 3a0a 2020 2020 2020 2020  list']:.        
-00008af0: 2020 2020 6164 635f 6d65 7461 6461 7461      adc_metadata
-00008b00: 2020 3d20 6d65 7461 6461 7461 5b27 6772    = metadata['gr
-00008b10: 6f75 7073 275d 5b61 6463 5f6e 616d 655d  oups'][adc_name]
-00008b20: 0a0a 2020 2020 2020 2020 6966 2061 6463  ..        if adc
-00008b30: 5f6d 6574 6164 6174 6120 6973 204e 6f6e  _metadata is Non
-00008b40: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
-00008b50: 7272 6f72 5f6d 7367 203d 2027 4144 4320  rror_msg = 'ADC 
-00008b60: 6d65 7461 6461 7461 206e 6f74 2066 6f75  metadata not fou
-00008b70: 6e64 2127 0a20 2020 2020 2020 2020 2020  nd!'.           
-00008b80: 2069 6620 7365 6c66 2e5f 7261 6973 655f   if self._raise_
-00008b90: 6572 726f 7273 3a0a 2020 2020 2020 2020  errors:.        
-00008ba0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00008bb0: 6520 5661 6c75 6545 7272 6f72 2865 7272  e ValueError(err
-00008bc0: 6f72 5f6d 7367 290a 2020 2020 2020 2020  or_msg).        
-00008bd0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008be0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00008bf0: 2757 4152 4e49 4e47 3a20 2720 2b20 6572  'WARNING: ' + er
-00008c00: 726f 725f 6d73 6729 0a20 2020 2020 2020  ror_msg).       
-00008c10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00008c20: 636f 6e65 6374 696f 6e5f 6469 6374 0a0a  conection_dict..
-00008c30: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
-00008c40: 696f 6e5f 6469 6374 5b27 6164 635f 6368  ion_dict['adc_ch
-00008c50: 616e 7327 5d20 3d20 6c69 7374 2829 0a20  ans'] = list(). 
-00008c60: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-00008c70: 6e5f 6469 6374 5b27 636f 6e74 726f 6c6c  n_dict['controll
-00008c80: 6572 5f63 6861 6e73 275d 203d 206c 6973  er_chans'] = lis
-00008c90: 7428 290a 2020 2020 2020 2020 636f 6e6e  t().        conn
-00008ca0: 6563 7469 6f6e 5f64 6963 745b 2774 6573  ection_dict['tes
-00008cb0: 5f63 6861 6e73 275d 203d 206c 6973 7428  _chans'] = list(
-00008cc0: 290a 2020 2020 2020 2020 636f 6e6e 6563  ).        connec
-00008cd0: 7469 6f6e 5f64 6963 745b 2764 6574 6563  tion_dict['detec
-00008ce0: 746f 725f 6368 616e 7327 5d20 3d20 6c69  tor_chans'] = li
-00008cf0: 7374 2829 0a20 2020 2020 2020 200a 2020  st().        .  
-00008d00: 2020 2020 2020 2320 6c6f 6f70 206d 6574        # loop met
-00008d10: 6164 6174 6120 746f 2066 696e 6420 636f  adata to find co
-00008d20: 6e6e 6563 7469 6f6e 730a 2020 2020 2020  nnections.      
-00008d30: 2020 666f 7220 6b65 792c 7661 6c75 6520    for key,value 
-00008d40: 696e 2061 6463 5f6d 6574 6164 6174 612e  in adc_metadata.
-00008d50: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-00008d60: 2020 2020 2069 6620 6b65 792e 6669 6e64       if key.find
-00008d70: 2827 636f 6e6e 6563 7469 6f6e 2729 213d  ('connection')!=
-00008d80: 2d31 3a0a 2020 2020 2020 2020 2020 2020  -1:.            
-00008d90: 2020 2020 636f 6e6e 6563 7469 6f6e 5f64      connection_d
-00008da0: 6963 745b 2761 6463 5f63 6861 6e73 275d  ict['adc_chans']
-00008db0: 2e61 7070 656e 6428 696e 7428 6b65 795b  .append(int(key[
-00008dc0: 3130 3a5d 2929 0a20 2020 2020 2020 2020  10:])).         
-00008dd0: 2020 2020 2020 2066 6f72 2063 6f6e 6e65         for conne
-00008de0: 6374 696f 6e5f 7479 7065 2069 6e20 7661  ction_type in va
-00008df0: 6c75 653a 0a20 2020 2020 2020 2020 2020  lue:.           
-00008e00: 2020 2020 2020 2020 2063 6861 6e6e 656c           channel
-00008e10: 5f6e 616d 6520 3d20 636f 6e6e 6563 7469  _name = connecti
-00008e20: 6f6e 5f74 7970 655b 636f 6e6e 6563 7469  on_type[connecti
-00008e30: 6f6e 5f74 7970 652e 6669 6e64 2827 3a27  on_type.find(':'
-00008e40: 292b 313a 5d0a 2020 2020 2020 2020 2020  )+1:].          
-00008e50: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
-00008e60: 6e65 6374 696f 6e5f 7479 7065 2e66 696e  nection_type.fin
-00008e70: 6428 2774 6573 3a27 2921 3d2d 313a 0a20  d('tes:')!=-1:. 
-00008e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e90: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
-00008ea0: 6e5f 6469 6374 5b27 7465 735f 6368 616e  n_dict['tes_chan
-00008eb0: 7327 5d2e 6170 7065 6e64 2863 6861 6e6e  s'].append(chann
-00008ec0: 656c 5f6e 616d 6529 0a20 2020 2020 2020  el_name).       
-00008ed0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00008ee0: 636f 6e6e 6563 7469 6f6e 5f74 7970 652e  connection_type.
-00008ef0: 6669 6e64 2827 6465 7465 6374 6f72 3a27  find('detector:'
-00008f00: 2921 3d2d 313a 0a20 2020 2020 2020 2020  )!=-1:.         
-00008f10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00008f20: 6f6e 6e65 6374 696f 6e5f 6469 6374 5b27  onnection_dict['
-00008f30: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
-00008f40: 2e61 7070 656e 6428 6368 616e 6e65 6c5f  .append(channel_
-00008f50: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
-00008f60: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
-00008f70: 6e65 6374 696f 6e5f 7479 7065 2e66 696e  nection_type.fin
-00008f80: 6428 2763 6f6e 7472 6f6c 6c65 723a 2729  d('controller:')
-00008f90: 213d 2d31 3a0a 2020 2020 2020 2020 2020  !=-1:.          
-00008fa0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00008fb0: 6e6e 6563 7469 6f6e 5f64 6963 745b 2763  nnection_dict['c
-00008fc0: 6f6e 7472 6f6c 6c65 725f 6368 616e 7327  ontroller_chans'
-00008fd0: 5d2e 6170 7065 6e64 2863 6861 6e6e 656c  ].append(channel
-00008fe0: 5f6e 616d 6529 0a0a 2020 2020 2020 2020  _name)..        
-00008ff0: 7265 7475 726e 2063 6f6e 6e65 6374 696f  return connectio
-00009000: 6e5f 6469 6374 2020 2020 2020 2020 2020  n_dict          
-00009010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009020: 2020 2020 0a0a 0a20 2020 200a 0a20 2020      ...    ..   
-00009030: 2064 6566 2067 6574 5f63 6f6e 6e65 6374   def get_connect
-00009040: 696f 6e5f 7461 626c 6528 7365 6c66 2c20  ion_table(self, 
-00009050: 6669 6c65 5f6e 616d 653d 4e6f 6e65 2c20  file_name=None, 
-00009060: 6d65 7461 6461 7461 3d4e 6f6e 6529 3a0a  metadata=None):.
-00009070: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009080: 2020 2020 4765 7420 636f 6e6e 6563 7469      Get connecti
-00009090: 6f6e 2074 6162 6c65 0a20 2020 2020 2020  on table.       
-000090a0: 2022 2222 0a20 2020 2020 2020 200a 2020   """.        .  
-000090b0: 2020 2020 2020 6966 206d 6574 6164 6174        if metadat
-000090c0: 6120 6973 204e 6f6e 653a 0a20 2020 2020  a is None:.     
-000090d0: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
-000090e0: 3d20 7365 6c66 2e67 6574 5f6d 6574 6164  = self.get_metad
-000090f0: 6174 6128 6669 6c65 5f6e 616d 653d 6669  ata(file_name=fi
-00009100: 6c65 5f6e 616d 6529 0a20 2020 2020 2020  le_name).       
-00009110: 200a 2020 2020 2020 2020 2320 6368 6563   .        # chec
-00009120: 6b20 6164 6320 6c69 7374 2065 7869 7374  k adc list exist
-00009130: 200a 2020 2020 2020 2020 6966 2027 6164   .        if 'ad
-00009140: 635f 6c69 7374 2720 6e6f 7420 696e 206d  c_list' not in m
-00009150: 6574 6164 6174 613a 0a20 2020 2020 2020  etadata:.       
-00009160: 2020 2020 2070 7269 6e74 2827 4552 524f       print('ERRO
-00009170: 523a 204e 6f20 4144 4320 6d65 7461 6461  R: No ADC metada
-00009180: 7461 2066 6f75 6e64 2069 6e20 7468 6520  ta found in the 
-00009190: 6669 6c65 2127 290a 2020 2020 2020 2020  file!').        
-000091a0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
-000091b0: 2020 2020 0a20 2020 2020 2020 2023 206c      .        # l
-000091c0: 6f6f 7020 6164 6320 616e 6420 6669 6e64  oop adc and find
-000091d0: 2063 6f6e 6e65 6374 696f 6e0a 2020 2020   connection.    
-000091e0: 2020 2020 636f 6e6e 6563 7469 6f6e 5f6c      connection_l
-000091f0: 6973 7420 3d20 6c69 7374 2829 0a20 2020  ist = list().   
-00009200: 2020 2020 2063 6f6e 6e65 6374 696f 6e5f       connection_
-00009210: 6e61 6d65 5f6c 6973 7420 3d20 6c69 7374  name_list = list
-00009220: 2829 0a20 2020 2020 2020 2066 6f72 2061  ().        for a
-00009230: 6463 5f69 6420 696e 206d 6574 6164 6174  dc_id in metadat
-00009240: 615b 2761 6463 5f6c 6973 7427 5d3a 0a20  a['adc_list']:. 
-00009250: 2020 2020 2020 2020 2020 2061 6463 5f6d             adc_m
-00009260: 6574 6164 6174 6120 3d20 6d65 7461 6461  etadata = metada
-00009270: 7461 5b27 6772 6f75 7073 275d 5b61 6463  ta['groups'][adc
-00009280: 5f69 645d 0a20 2020 2020 2020 2020 2020  _id].           
-00009290: 2066 6f72 206b 6579 2c76 616c 2069 6e20   for key,val in 
-000092a0: 6164 635f 6d65 7461 6461 7461 2e69 7465  adc_metadata.ite
-000092b0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-000092c0: 2020 2020 2020 6966 206b 6579 5b30 3a31        if key[0:1
-000092d0: 305d 3d3d 2763 6f6e 6e65 6374 696f 6e27  0]=='connection'
-000092e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000092f0: 2020 2020 2020 6164 635f 6368 616e 203d        adc_chan =
-00009300: 2072 652e 7375 6228 7227 5c73 2b27 2c27   re.sub(r'\s+','
-00009310: 272c 2073 7472 286b 6579 2929 5b31 303a  ', str(key))[10:
-00009320: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00009330: 2020 2020 2020 6e61 6d65 5f76 616c 5f6c        name_val_l
-00009340: 6973 742c 206e 616d 655f 6c69 7374 2c20  ist, name_list, 
-00009350: 7661 6c5f 6c69 7374 203d 2028 0a20 2020  val_list = (.   
-00009360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009370: 2020 2020 2063 6f6e 6e65 6374 696f 6e5f       connection_
-00009380: 7574 696c 732e 6578 7472 6163 745f 6164  utils.extract_ad
-00009390: 635f 636f 6e6e 6563 7469 6f6e 286c 6973  c_connection(lis
-000093a0: 7428 7661 6c29 2929 0a20 2020 2020 2020  t(val))).       
-000093b0: 2020 2020 2020 2020 2020 2020 2076 616c               val
-000093c0: 5f6c 6973 7420 203d 205b 6164 635f 6964  _list  = [adc_id
-000093d0: 2c61 6463 5f63 6861 6e5d 202b 2076 616c  ,adc_chan] + val
-000093e0: 5f6c 6973 740a 2020 2020 2020 2020 2020  _list.          
-000093f0: 2020 2020 2020 2020 2020 6e61 6d65 5f6c            name_l
-00009400: 6973 7420 3d20 5b27 6164 635f 6964 272c  ist = ['adc_id',
-00009410: 2761 6463 5f63 6861 6e6e 656c 275d 202b  'adc_channel'] +
-00009420: 206e 616d 655f 6c69 7374 0a20 2020 2020   name_list.     
-00009430: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009440: 6f6e 6e65 6374 696f 6e5f 6c69 7374 2e61  onnection_list.a
-00009450: 7070 656e 6428 7661 6c5f 6c69 7374 290a  ppend(val_list).
-00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009470: 2020 2020 6966 206e 6f74 2063 6f6e 6e65      if not conne
-00009480: 6374 696f 6e5f 6e61 6d65 5f6c 6973 743a  ction_name_list:
-00009490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000094a0: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
-000094b0: 696f 6e5f 6e61 6d65 5f6c 6973 7420 3d20  ion_name_list = 
-000094c0: 6e61 6d65 5f6c 6973 740a 2020 2020 2020  name_list.      
-000094d0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000094e0: 6966 2063 6f6e 6e65 6374 696f 6e5f 6e61  if connection_na
-000094f0: 6d65 5f6c 6973 7421 3d6e 616d 655f 6c69  me_list!=name_li
-00009500: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
-00009510: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00009520: 7428 2745 5252 4f52 3a20 6d69 7373 696e  t('ERROR: missin
-00009530: 6720 6164 6320 636f 6e6e 6563 7469 6f6e  g adc connection
-00009540: 2076 616c 7565 7321 2729 0a20 2020 2020   values!').     
-00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009560: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00009570: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00009580: 2063 6f6e 6e65 6374 696f 6e5f 7461 626c   connection_tabl
-00009590: 6520 3d20 7064 2e44 6174 6146 7261 6d65  e = pd.DataFrame
-000095a0: 2863 6f6e 6e65 6374 696f 6e5f 6c69 7374  (connection_list
-000095b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095d0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-000095e0: 733d 636f 6e6e 6563 7469 6f6e 5f6e 616d  s=connection_nam
-000095f0: 655f 6c69 7374 2029 0a20 2020 2020 2020  e_list ).       
-00009600: 2072 6574 7572 6e20 636f 6e6e 6563 7469   return connecti
-00009610: 6f6e 5f74 6162 6c65 0a0a 0a20 2020 200a  on_table...    .
-00009620: 2020 0a0a 2020 2020 6465 6620 5f6f 7065    ..    def _ope
-00009630: 6e5f 6669 6c65 2873 656c 662c 2066 696c  n_file(self, fil
-00009640: 655f 6e61 6d65 2c20 7277 5f73 7472 696e  e_name, rw_strin
-00009650: 673d 2772 272c 206c 6f61 645f 6d65 7461  g='r', load_meta
-00009660: 6461 7461 3d54 7275 6529 3a0a 2020 2020  data=True):.    
-00009670: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00009680: 6f70 656e 2066 696c 6520 0a20 2020 2020  open file .     
-00009690: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-000096a0: 6620 7365 6c66 2e5f 6375 7272 656e 745f  f self._current_
-000096b0: 6669 6c65 2069 7320 6e6f 7420 4e6f 6e65  file is not None
-000096c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000096d0: 6c66 2e5f 636c 6f73 655f 6669 6c65 2829  lf._close_file()
-000096e0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
-000096f0: 2020 2020 2020 6669 6c65 203d 204e 6f6e        file = Non
-00009700: 650a 2020 2020 2020 2020 7472 793a 0a20  e.        try:. 
-00009710: 2020 2020 2020 2020 2020 2066 696c 6520             file 
-00009720: 3d20 6835 7079 2e46 696c 6528 6669 6c65  = h5py.File(file
-00009730: 5f6e 616d 652c 7277 5f73 7472 696e 6729  _name,rw_string)
-00009740: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
-00009750: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00009760: 6e74 2827 4552 524f 523a 2075 6e61 626c  nt('ERROR: unabl
-00009770: 6520 746f 206f 7065 6e20 6669 6c65 2027  e to open file '
-00009780: 202b 2066 696c 655f 6e61 6d65 290a 2020   + file_name).  
-00009790: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000097a0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-000097b0: 6375 7272 656e 745f 6669 6c65 203d 2066  current_file = f
-000097c0: 696c 650a 2020 2020 2020 2020 7365 6c66  ile.        self
-000097d0: 2e5f 6375 7272 656e 745f 6669 6c65 5f6e  ._current_file_n
-000097e0: 616d 6520 3d20 6669 6c65 5f6e 616d 650a  ame = file_name.
-000097f0: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-00009800: 7272 656e 745f 6669 6c65 5f6e 625f 6576  rrent_file_nb_ev
-00009810: 656e 7473 203d 2030 0a20 2020 2020 2020  ents = 0.       
-00009820: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-00009830: 696c 655f 6576 656e 745f 636f 756e 7465  ile_event_counte
-00009840: 7220 3d20 300a 2020 2020 2020 2020 0a20  r = 0.        . 
-00009850: 2020 2020 2020 2023 206c 6f61 6420 6d65         # load me
-00009860: 7461 6461 7461 0a20 2020 2020 2020 2069  tadata.        i
-00009870: 6620 6c6f 6164 5f6d 6574 6164 6174 613a  f load_metadata:
-00009880: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00009890: 6c66 2e5f 6c6f 6164 5f6d 6574 6164 6174  lf._load_metadat
-000098a0: 6128 290a 2020 2020 2020 2020 2020 2020  a().            
-000098b0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-000098c0: 6865 636b 2065 7665 6e74 730a 2020 2020  heck events.    
-000098d0: 2020 2020 2020 2020 6966 2027 6164 635f          if 'adc_
-000098e0: 6c69 7374 2720 6e6f 7420 696e 2073 656c  list' not in sel
-000098f0: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
-00009900: 6d65 7461 6461 7461 3a0a 2020 2020 2020  metadata:.      
-00009910: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00009920: 2757 4152 4e49 4e47 3a20 4e6f 2041 4443  'WARNING: No ADC
-00009930: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f75   information fou
-00009940: 6e64 2069 6e20 7468 6520 6669 6c65 2729  nd in the file')
-00009950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009960: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-00009970: 2020 2020 2066 6f72 2061 6463 5f6e 616d       for adc_nam
-00009980: 6520 696e 2073 656c 662e 5f63 7572 7265  e in self._curre
-00009990: 6e74 5f66 696c 655f 6d65 7461 6461 7461  nt_file_metadata
-000099a0: 5b27 6164 635f 6c69 7374 275d 3a0a 2020  ['adc_list']:.  
-000099b0: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
-000099c0: 5f65 7665 6e74 735f 6164 6320 3d20 7365  _events_adc = se
-000099d0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-000099e0: 5f6d 6574 6164 6174 615b 2767 726f 7570  _metadata['group
-000099f0: 7327 5d5b 6164 635f 6e61 6d65 5d5b 276e  s'][adc_name]['n
-00009a00: 625f 6461 7461 7365 7473 275d 0a20 2020  b_datasets'].   
-00009a10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009a20: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
-00009a30: 6c65 5f6e 625f 6576 656e 7473 3d3d 303a  le_nb_events==0:
-00009a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009a50: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
-00009a60: 6e74 5f66 696c 655f 6e62 5f65 7665 6e74  nt_file_nb_event
-00009a70: 7320 3d20 6e62 5f65 7665 6e74 735f 6164  s = nb_events_ad
-00009a80: 630a 2020 2020 2020 2020 2020 2020 2020  c.              
-00009a90: 2020 656c 6966 2073 656c 662e 5f63 7572    elif self._cur
-00009aa0: 7265 6e74 5f66 696c 655f 6e62 5f65 7665  rent_file_nb_eve
-00009ab0: 6e74 7320 213d 206e 625f 6576 656e 7473  nts != nb_events
-00009ac0: 5f61 6463 3a0a 2020 2020 2020 2020 2020  _adc:.          
-00009ad0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00009ae0: 2745 5252 4f52 3a20 496e 636f 6e73 6973  'ERROR: Inconsis
-00009af0: 7465 6e74 206e 756d 6265 7220 6f66 2065  tent number of e
-00009b00: 7665 6e74 7320 6265 7477 6565 6e20 4144  vents between AD
-00009b10: 4320 6465 7669 6365 7321 2729 0a20 2020  C devices!').   
-00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b30: 2073 656c 662e 5f63 6c6f 7365 5f66 696c   self._close_fil
-00009b40: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00009b50: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00009b60: 616c 7365 0a0a 2020 2020 2020 2020 7365  alse..        se
-00009b70: 6c66 2e5f 6669 6c65 5f63 6f75 6e74 6572  lf._file_counter
-00009b80: 202b 3d20 3120 0a20 2020 2020 2020 2072   += 1 .        r
-00009b90: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00009ba0: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00009bb0: 2020 2020 2020 2020 200a 2020 2020 0a0a           .    ..
-00009bc0: 2020 2020 6465 6620 5f63 6c6f 7365 5f66      def _close_f
-00009bd0: 696c 6528 7365 6c66 293a 0a20 2020 2020  ile(self):.     
-00009be0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00009bf0: 6c6f 7365 2063 7572 7265 6e74 2066 696c  lose current fil
-00009c00: 6520 616e 6420 7265 7365 740a 2020 2020  e and reset.    
-00009c10: 2020 2020 6375 7272 656e 7420 6669 6c65      current file
-00009c20: 2070 6172 616d 6574 6572 730a 0a20 2020   parameters..   
-00009c30: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00009c40: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00009c50: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
-00009c60: 0a20 2020 2020 2020 2052 6574 7572 6e0a  .        Return.
-00009c70: 2020 2020 2020 2020 2d2d 2d2d 2d2d 0a20          ------. 
-00009c80: 2020 2020 2020 204e 6f6e 650a 0a20 2020         None..   
-00009c90: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00009ca0: 2020 6966 2073 656c 662e 5f63 7572 7265    if self._curre
-00009cb0: 6e74 5f66 696c 6520 6973 206e 6f74 204e  nt_file is not N
-00009cc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00009cd0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-00009ce0: 696c 652e 636c 6f73 6528 290a 2020 0a20  ile.close().  . 
-00009cf0: 2020 2020 2020 2023 2069 6e69 7469 616c         # initial
-00009d00: 697a 650a 2020 2020 2020 2020 7365 6c66  ize.        self
-00009d10: 2e5f 6375 7272 656e 745f 6669 6c65 203d  ._current_file =
-00009d20: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-00009d30: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-00009d40: 5f6e 616d 6520 3d20 4e6f 6e65 0a20 2020  _name = None.   
-00009d50: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
-00009d60: 6e74 5f66 696c 655f 6d65 7461 6461 7461  nt_file_metadata
-00009d70: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00009d80: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
-00009d90: 6c65 5f6e 625f 6576 656e 7473 203d 2030  le_nb_events = 0
-00009da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009db0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-00009dc0: 2020 2020 2020 0a0a 0a20 2020 2064 6566        ...    def
-00009dd0: 205f 6c6f 6164 5f6d 6574 6164 6174 6128   _load_metadata(
-00009de0: 7365 6c66 2c20 696e 636c 7564 655f 6461  self, include_da
-00009df0: 7461 7365 745f 6d65 7461 6461 7461 3d46  taset_metadata=F
-00009e00: 616c 7365 293a 0a0a 2020 2020 2020 2020  alse):..        
-00009e10: 2222 220a 2020 2020 2020 2020 4675 6e63  """.        Func
-00009e20: 7469 6f6e 2074 6f20 6c6f 6164 2061 6c6c  tion to load all
-00009e30: 206d 6574 6164 6174 6120 6672 6f6d 2063   metadata from c
-00009e40: 7572 7265 6e74 2066 696c 652e 2053 746f  urrent file. Sto
-00009e50: 7265 2069 6e20 0a20 2020 2020 2020 2061  re in .        a
-00009e60: 6e20 696e 7465 726e 616c 2064 6963 7469  n internal dicti
-00009e70: 6f6e 6172 790a 0a20 2020 2020 2020 2050  onary..        P
-00009e80: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00009e90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020    ----------..  
-00009ea0: 2020 2020 2020 696e 636c 7564 655f 6461        include_da
-00009eb0: 7461 7365 745f 6d65 7461 6461 7461 203a  taset_metadata :
-00009ec0: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
-00009ed0: 2020 2020 2020 2020 2020 2069 6620 5472             if Tr
-00009ee0: 7565 2c20 7265 6164 2064 6174 6173 6574  ue, read dataset
-00009ef0: 206d 6574 6164 6174 610a 2020 2020 2020   metadata.      
-00009f00: 2020 2020 2044 6566 6175 6c74 3a20 4661       Default: Fa
-00009f10: 6c73 650a 0a0a 2020 2020 2020 2020 5265  lse...        Re
-00009f20: 7475 726e 0a20 2020 2020 2020 202d 2d2d  turn.        ---
-00009f30: 2d2d 2d0a 2020 2020 2020 2020 0a20 2020  ---.        .   
-00009f40: 2020 2020 206d 6574 6164 6174 615f 6469       metadata_di
-00009f50: 6374 203a 2064 6963 740a 2020 2020 2020  ct : dict.      
-00009f60: 2020 2020 6469 6374 696f 6e61 7279 2077      dictionary w
-00009f70: 6974 6820 6d65 7461 6461 7461 0a20 2020  ith metadata.   
-00009f80: 2020 2020 200a 0a20 2020 2020 2020 2022       ..        "
-00009f90: 2222 0a0a 2020 2020 2020 2020 2320 6368  ""..        # ch
-00009fa0: 6563 6b20 6966 2066 696c 6520 6578 6973  eck if file exis
-00009fb0: 740a 2020 2020 2020 2020 6966 2073 656c  t.        if sel
-00009fc0: 662e 5f63 7572 7265 6e74 5f66 696c 6520  f._current_file 
-00009fd0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00009fe0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00009ff0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-0000a000: 2020 2020 2320 696e 6974 6961 6c69 7a65      # initialize
-0000a010: 2063 6f6e 7461 696e 6e65 720a 2020 2020   containner.    
-0000a020: 2020 2020 6d65 7461 6461 7461 5f64 6963      metadata_dic
-0000a030: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0000a040: 200a 0a20 2020 2020 2020 2023 2066 696c   ..        # fil
-0000a050: 6520 6d61 7461 6461 7461 0a20 2020 2020  e matadata.     
-0000a060: 2020 206d 6574 6164 6174 615f 6469 6374     metadata_dict
-0000a070: 203d 2073 656c 662e 5f65 7874 7261 6374   = self._extract
-0000a080: 5f6d 6574 6164 6174 6128 7365 6c66 2e5f  _metadata(self._
-0000a090: 6375 7272 656e 745f 6669 6c65 2e61 7474  current_file.att
-0000a0a0: 7273 290a 2020 2020 2020 0a20 2020 200a  rs).      .    .
-0000a0b0: 2020 2020 2020 2020 2320 6772 6f75 702f          # group/
-0000a0c0: 6461 7461 7365 7420 6d65 7461 6461 7461  dataset metadata
-0000a0d0: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
-0000a0e0: 615f 6469 6374 5b27 6772 6f75 705f 6c69  a_dict['group_li
-0000a0f0: 7374 275d 203d 206c 6973 7428 290a 2020  st'] = list().  
-0000a100: 2020 2020 2020 6d65 7461 6461 7461 5f64        metadata_d
-0000a110: 6963 745b 2761 6463 5f6c 6973 7427 5d20  ict['adc_list'] 
-0000a120: 3d20 6c69 7374 2829 0a20 2020 2020 2020  = list().       
-0000a130: 206d 6574 6164 6174 615f 6469 6374 5b27   metadata_dict['
-0000a140: 6772 6f75 7073 275d 203d 2064 6963 7428  groups'] = dict(
-0000a150: 290a 2020 2020 2020 2020 2020 200a 2020  ).           .  
-0000a160: 2020 2020 2020 2320 4c6f 6f70 2067 726f        # Loop gro
-0000a170: 7570 730a 2020 2020 2020 2020 666f 7220  ups.        for 
-0000a180: 6b65 792c 2067 726f 7570 2069 6e20 7365  key, group in se
-0000a190: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-0000a1a0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-0000a1b0: 200a 2020 2020 2020 2020 2020 2020 2320   .            # 
-0000a1c0: 7570 6461 7465 206c 6973 740a 2020 2020  update list.    
-0000a1d0: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-0000a1e0: 5f64 6963 745b 2767 726f 7570 5f6c 6973  _dict['group_lis
-0000a1f0: 7427 5d2e 6170 7065 6e64 286b 6579 290a  t'].append(key).
-0000a200: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-0000a210: 6579 5b30 3a33 5d3d 3d27 6164 6327 3a0a  ey[0:3]=='adc':.
-0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a230: 6d65 7461 6461 7461 5f64 6963 745b 2761  metadata_dict['a
-0000a240: 6463 5f6c 6973 7427 5d2e 6170 7065 6e64  dc_list'].append
-0000a250: 286b 6579 290a 2020 2020 2020 2020 2020  (key).          
-0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a270: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-0000a280: 2020 2023 2073 6176 6520 6d65 7461 6461     # save metada
-0000a290: 7461 0a20 2020 2020 2020 2020 2020 206d  ta.            m
-0000a2a0: 6574 6164 6174 615f 6469 6374 5b27 6772  etadata_dict['gr
-0000a2b0: 6f75 7073 275d 5b6b 6579 5d20 3d20 6469  oups'][key] = di
-0000a2c0: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-0000a2d0: 206d 6574 6164 6174 615f 6469 6374 5b27   metadata_dict['
-0000a2e0: 6772 6f75 7073 275d 5b6b 6579 5d20 3d20  groups'][key] = 
-0000a2f0: 2073 656c 662e 5f65 7874 7261 6374 5f6d   self._extract_m
-0000a300: 6574 6164 6174 6128 6772 6f75 702e 6174  etadata(group.at
-0000a310: 7472 7329 0a20 2020 2020 2020 200a 2020  trs).        .  
-0000a320: 2020 2020 2020 2020 2020 2320 6461 7461            # data
-0000a330: 7365 7473 0a20 2020 2020 2020 2020 2020  sets.           
-0000a340: 2064 6174 6173 6574 5f6c 6973 7420 3d20   dataset_list = 
-0000a350: 6c69 7374 2867 726f 7570 2e6b 6579 7328  list(group.keys(
-0000a360: 2929 0a20 2020 2020 2020 2020 2020 206d  )).            m
-0000a370: 6574 6164 6174 615f 6469 6374 5b27 6772  etadata_dict['gr
-0000a380: 6f75 7073 275d 5b6b 6579 5d5b 2764 6174  oups'][key]['dat
-0000a390: 6173 6574 5f6c 6973 7427 5d20 3d20 6461  aset_list'] = da
-0000a3a0: 7461 7365 745f 6c69 7374 0a20 2020 2020  taset_list.     
-0000a3b0: 2020 2020 2020 206d 6574 6164 6174 615f         metadata_
-0000a3c0: 6469 6374 5b27 6772 6f75 7073 275d 5b6b  dict['groups'][k
-0000a3d0: 6579 5d5b 276e 625f 6461 7461 7365 7473  ey]['nb_datasets
-0000a3e0: 275d 203d 206c 656e 2864 6174 6173 6574  '] = len(dataset
-0000a3f0: 5f6c 6973 7429 0a20 2020 2020 2020 2020  _list).         
-0000a400: 2020 2020 2020 200a 0a20 2020 2020 2020         ..       
-0000a410: 2020 2020 2069 6620 696e 636c 7564 655f       if include_
-0000a420: 6461 7461 7365 745f 6d65 7461 6461 7461  dataset_metadata
-0000a430: 2061 6e64 206c 656e 2864 6174 6173 6574   and len(dataset
-0000a440: 5f6c 6973 7429 3e30 3a0a 2020 2020 2020  _list)>0:.      
-0000a450: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-0000a460: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000a470: 204c 6f6f 7020 6461 7461 7365 7473 2061   Loop datasets a
-0000a480: 6e64 2061 6464 206d 6574 6164 6174 610a  nd add metadata.
-0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 6d65 7461 6461 7461 5f64 6963 745b 2767  metadata_dict['g
-0000a4b0: 726f 7570 7327 5d5b 6b65 795d 5b27 6461  roups'][key]['da
-0000a4c0: 7461 7365 7473 275d 203d 2064 6963 7428  tasets'] = dict(
-0000a4d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a4e0: 2020 666f 7220 6461 7461 7365 745f 6b65    for dataset_ke
-0000a4f0: 792c 2064 6174 6173 6574 2069 6e20 6772  y, dataset in gr
-0000a500: 6f75 702e 6974 656d 7328 293a 0a20 2020  oup.items():.   
-0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a520: 206d 6574 6164 6174 615f 6469 6374 5b27   metadata_dict['
-0000a530: 6772 6f75 7073 275d 5b6b 6579 5d5b 2764  groups'][key]['d
-0000a540: 6174 6173 6574 7327 5d5b 6461 7461 7365  atasets'][datase
-0000a550: 745f 6b65 795d 203d 2028 0a20 2020 2020  t_key] = (.     
-0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a570: 2020 2073 656c 662e 5f65 7874 7261 6374     self._extract
-0000a580: 5f6d 6574 6164 6174 6128 6461 7461 7365  _metadata(datase
-0000a590: 742e 6174 7472 7329 0a20 2020 2020 2020  t.attrs).       
-0000a5a0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5c0: 2020 2020 2020 2020 0a0a 2020 2020 2020          ..      
-0000a5d0: 2020 2320 7361 7665 0a20 2020 2020 2020    # save.       
-0000a5e0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-0000a5f0: 696c 655f 6d65 7461 6461 7461 203d 206d  ile_metadata = m
-0000a600: 6574 6164 6174 615f 6469 6374 0a20 2020  etadata_dict.   
-0000a610: 2020 0a0a 0a0a 0a0a 0a20 2020 2064 6566    .......    def
-0000a620: 205f 6578 7472 6163 745f 6d65 7461 6461   _extract_metada
-0000a630: 7461 2873 656c 662c 2061 7474 7269 6275  ta(self, attribu
-0000a640: 7465 7329 3a0a 2020 2020 2020 2020 2222  tes):.        ""
-0000a650: 220a 2020 2020 2020 2020 4578 7472 6163  ".        Extrac
-0000a660: 7420 6d65 7461 6461 7461 2066 726f 6d20  t metadata from 
-0000a670: 6174 7472 6962 7574 6520 6469 6374 696f  attribute dictio
-0000a680: 6e61 7279 0a20 2020 2020 2020 2022 2222  nary.        """
-0000a690: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-0000a6a0: 2020 6d65 7461 6461 7461 5f64 6963 7420    metadata_dict 
-0000a6b0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0000a6c0: 2066 6f72 206b 6579 2c76 616c 7565 2069   for key,value i
-0000a6d0: 6e20 6174 7472 6962 7574 6573 2e69 7465  n attributes.ite
-0000a6e0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-0000a6f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000a700: 7661 6c75 652c 2062 7974 6573 293a 0a20  value, bytes):. 
-0000a710: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000a720: 616c 7565 203d 2076 616c 7565 2e64 6563  alue = value.dec
-0000a730: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
-0000a740: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-0000a750: 6528 7661 6c75 652c 206e 702e 6e64 6172  e(value, np.ndar
-0000a760: 7261 7929 3a0a 2020 2020 2020 2020 2020  ray):.          
-0000a770: 2020 2020 2020 6966 2076 616c 7565 2e64        if value.d
-0000a780: 7479 7065 203d 3d20 6e70 2e6f 626a 6563  type == np.objec
-0000a790: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0000a7a0: 2020 2020 2020 2076 616c 7565 203d 2076         value = v
-0000a7b0: 616c 7565 2e61 7374 7970 6528 7374 7229  alue.astype(str)
-0000a7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a7d0: 2023 2061 2066 6577 2070 6172 7469 6375   # a few particu
-0000a7e0: 6c61 7220 6361 7365 730a 2020 2020 2020  lar cases.      
-0000a7f0: 2020 2020 2020 2020 2020 6966 206b 6579            if key
-0000a800: 203d 3d20 2772 756e 5f70 7572 706f 7365   == 'run_purpose
-0000a810: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-0000a820: 2020 2020 2020 2076 616c 7565 203d 2027         value = '
-0000a830: 2027 2e6a 6f69 6e28 6c69 7374 2876 616c   '.join(list(val
-0000a840: 7565 2929 2020 2020 2020 2020 2020 2020  ue))            
-0000a850: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000a860: 2020 2020 206d 6574 6164 6174 615f 6469       metadata_di
-0000a870: 6374 5b6b 6579 5d20 3d20 7661 6c75 650a  ct[key] = value.
-0000a880: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-0000a890: 6574 6164 6174 615f 6469 6374 0a20 2020  etadata_dict.   
-0000a8a0: 2020 2020 200a 0a20 2020 200a 2020 2020       ..    .    
-0000a8b0: 6465 6620 5f6c 6f61 645f 6576 656e 7428  def _load_event(
-0000a8c0: 7365 6c66 2c20 6576 656e 745f 696e 6465  self, event_inde
-0000a8d0: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
-0000a8e0: 2020 2020 2020 2064 6574 6563 746f 725f         detector_
-0000a8f0: 6368 616e 733d 4e6f 6e65 2c0a 2020 2020  chans=None,.    
-0000a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a910: 6164 6374 6f76 6f6c 743d 4661 6c73 652c  adctovolt=False,
-0000a920: 2061 6463 746f 616d 703d 4661 6c73 652c   adctoamp=False,
-0000a930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a940: 2020 2020 2062 6173 656c 696e 6573 7562       baselinesub
-0000a950: 3d46 616c 7365 2c20 6261 7365 6c69 6e65  =False, baseline
-0000a960: 696e 6473 3d4e 6f6e 652c 0a20 2020 2020  inds=None,.     
-0000a970: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000a980: 6463 5f6e 616d 653d 2761 6463 3127 293a  dc_name='adc1'):
-0000a990: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-0000a9a0: 2020 2222 220a 2020 2020 2020 2020 4c6f    """.        Lo
-0000a9b0: 6164 2074 7261 6365 7320 616e 6420 6d65  ad traces and me
-0000a9c0: 7461 6461 7461 2066 726f 6d20 6375 7272  tadata from curr
-0000a9d0: 656e 7420 6669 6c65 2020 6261 7365 6420  ent file  based 
-0000a9e0: 6f6e 0a20 2020 2020 2020 2065 7665 6e74  on.        event
-0000a9f0: 2069 6e64 6578 0a20 0a20 2020 2020 2020   index. .       
-0000aa00: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000aa10: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000aa20: 2020 2020 2020 2065 7665 6e74 5f69 6e64         event_ind
-0000aa30: 6578 203a 2069 6e74 0a20 2020 2020 2020  ex : int.       
-0000aa40: 2020 2065 7665 6e74 2028 6864 6635 2022     event (hdf5 "
-0000aa50: 6461 7461 7365 7422 2920 206e 756d 6265  dataset")  numbe
-0000aa60: 7220 0a20 2020 2020 2020 200a 2020 2020  r .        .    
-0000aa70: 2020 2020 6465 7465 6374 6f72 5f63 6861      detector_cha
-0000aa80: 6e73 203a 2073 7472 206f 7220 6c69 7374  ns : str or list
-0000aa90: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000aaa0: 2020 2020 2064 6574 6563 746f 722f 6368       detector/ch
-0000aab0: 616e 6e65 6c20 6e61 6d65 206f 7220 6c69  annel name or li
-0000aac0: 7374 206f 6620 6465 7465 6374 6f72 732f  st of detectors/
-0000aad0: 6368 616e 6e65 6c73 0a20 2020 2020 2020  channels.       
-0000aae0: 2020 2069 6620 4e6f 6e65 2c20 6765 7420     if None, get 
-0000aaf0: 616c 6c20 6368 616e 6e65 6c73 2028 6465  all channels (de
-0000ab00: 6661 756c 7429 0a0a 2020 2020 2020 2020  fault)..        
-0000ab10: 6164 6374 6f76 6f6c 7420 3a20 626f 6f6c  adctovolt : bool
-0000ab20: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000ab30: 2020 2020 2063 6f6e 7665 7274 2066 726f       convert fro
-0000ab40: 6d20 4144 4320 746f 2076 6f6c 7473 0a20  m ADC to volts. 
-0000ab50: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-0000ab60: 3a20 4661 6c73 650a 0a20 2020 2020 2020  : False..       
-0000ab70: 2061 6463 746f 616d 7020 3a20 626f 6f6c   adctoamp : bool
-0000ab80: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000ab90: 2020 2020 2063 6f6e 7665 7274 2066 726f       convert fro
-0000aba0: 6d20 4144 4320 746f 2063 7572 7265 6e74  m ADC to current
-0000abb0: 2061 6d70 730a 2020 2020 2020 2020 2020   amps.          
-0000abc0: 6465 6661 756c 743a 2046 616c 7365 0a20  default: False. 
-0000abd0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000abe0: 2020 2020 2020 0a20 2020 2020 2020 2062        .        b
-0000abf0: 6173 656c 696e 6573 7562 3a20 626f 6f6c  aselinesub: bool
-0000ac00: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000ac10: 2020 2020 2069 6620 5472 7565 2c20 7375       if True, su
-0000ac20: 6274 7261 6374 2070 7265 2d70 756c 7365  btract pre-pulse
-0000ac30: 2062 6173 656c 696e 650a 2020 2020 2020   baseline.      
-0000ac40: 2020 2020 6465 6661 756c 743a 2046 616c      default: Fal
-0000ac50: 7365 0a0a 2020 2020 2020 2020 6261 7365  se..        base
-0000ac60: 6c69 6e65 696e 6473 3a20 7475 706c 6520  lineinds: tuple 
-0000ac70: 2869 6e74 2c20 696e 7429 206f 7220 6c69  (int, int) or li
-0000ac80: 7374 205b 696e 742c 2069 6e74 5d0a 2020  st [int, int].  
-0000ac90: 2020 2020 2020 2020 6d69 6e2f 6d61 7820          min/max 
-0000aca0: 696e 6465 7820 666f 7220 2062 6173 656c  index for  basel
-0000acb0: 696e 6520 6361 6c63 756c 6174 696f 6e20  ine calculation 
-0000acc0: 0a20 2020 2020 2020 2020 2064 6566 6175  .          defau
-0000acd0: 6c74 3a20 2831 302c 2030 2e38 2a70 7265  lt: (10, 0.8*pre
-0000ace0: 7472 6967 6765 7220 6c65 6e67 7468 2929  trigger length))
-0000acf0: 0a20 2020 2020 2020 2020 200a 2020 2020  .          .    
-0000ad00: 2020 2020 6164 635f 6e61 6d65 203a 2073      adc_name : s
-0000ad10: 7472 2c20 6f70 7469 6f6e 616c 0a20 2020  tr, optional.   
-0000ad20: 2020 2020 2020 206e 616d 652f 4944 206f         name/ID o
-0000ad30: 6620 7468 6520 6164 630a 2020 2020 2020  f the adc.      
-0000ad40: 2020 2020 6465 6661 756c 743a 2022 6164      default: "ad
-0000ad50: 6331 220a 0a20 2020 2020 2020 2052 6574  c1"..        Ret
-0000ad60: 7572 6e0a 2020 2020 2020 2020 2d2d 2d2d  urn.        ----
-0000ad70: 2d2d 0a20 2020 2020 2020 200a 2020 2020  --.        .    
-0000ad80: 2020 2020 6172 7261 7920 3a20 3244 206e      array : 2D n
-0000ad90: 756d 7079 2061 7272 6179 0a20 2020 2020  umpy array.     
-0000ada0: 2020 2020 2020 7472 6163 6573 2066 6f72        traces for
-0000adb0: 2065 6163 6820 6368 616e 6e65 6c20 5b6e   each channel [n
-0000adc0: 6220 6368 616e 6e65 6c2c 206e 6220 7361  b channel, nb sa
-0000add0: 6d70 6c65 735d 0a0a 2020 2020 2020 2020  mples]..        
-0000ade0: 696e 666f 203a 2064 6963 740a 2020 2020  info : dict.    
-0000adf0: 2020 2020 2020 2066 696c 652f 6576 656e         file/even
-0000ae00: 742f 6465 7465 6374 6f72 206d 6574 6164  t/detector metad
-0000ae10: 6174 6120 2869 6620 2269 6e63 6c75 6465  ata (if "include
-0000ae20: 5f6d 6574 6164 6174 6122 203d 2054 7275  _metadata" = Tru
-0000ae30: 6529 0a0a 0a20 2020 2020 2020 200a 2020  e)...        .  
-0000ae40: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000ae50: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-0000ae60: 2020 2020 2020 2023 2063 6865 636b 2066         # check f
-0000ae70: 696c 6520 6f70 656e 0a20 2020 2020 2020  ile open.       
-0000ae80: 2069 6620 7365 6c66 2e5f 6375 7272 656e   if self._curren
-0000ae90: 745f 6669 6c65 2069 7320 4e6f 6e65 3a0a  t_file is None:.
-0000aea0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000aeb0: 6520 5661 6c75 6545 7272 6f72 2827 4e6f  e ValueError('No
-0000aec0: 2066 696c 6520 6f70 656e 2127 290a 2020   file open!').  
-0000aed0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-0000aee0: 2067 6574 2064 6174 6173 6574 0a20 2020   get dataset.   
-0000aef0: 2020 2020 2064 6174 6173 6574 5f6e 616d       dataset_nam
-0000af00: 6520 3d20 2765 7665 6e74 5f27 202b 2073  e = 'event_' + s
-0000af10: 7472 2865 7665 6e74 5f69 6e64 6578 290a  tr(event_index).
-0000af20: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
-0000af30: 3d20 7365 6c66 2e5f 6375 7272 656e 745f  = self._current_
-0000af40: 6669 6c65 5b61 6463 5f6e 616d 655d 5b64  file[adc_name][d
-0000af50: 6174 6173 6574 5f6e 616d 655d 0a20 2020  ataset_name].   
-0000af60: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-0000af70: 7265 6164 2064 6174 6173 6574 0a20 2020  read dataset.   
-0000af80: 2020 2020 2064 696d 7320 3d20 6461 7461       dims = data
-0000af90: 7365 742e 7368 6170 650a 2020 2020 2020  set.shape.      
-0000afa0: 2020 7472 6163 6573 5f69 6e74 203d 206e    traces_int = n
-0000afb0: 702e 7a65 726f 7328 2864 696d 735b 305d  p.zeros((dims[0]
-0000afc0: 2c64 696d 735b 315d 292c 2064 7479 7065  ,dims[1]), dtype
-0000afd0: 3d6e 702e 696e 7431 3629 0a20 2020 2020  =np.int16).     
-0000afe0: 2020 2064 6174 6173 6574 2e72 6561 645f     dataset.read_
-0000aff0: 6469 7265 6374 2874 7261 6365 735f 696e  direct(traces_in
-0000b000: 7429 0a20 2020 2020 200a 2020 2020 2020  t).      .      
-0000b010: 2020 2320 6765 7420 6d65 7461 6461 7461    # get metadata
-0000b020: 0a20 2020 2020 2020 2069 6e66 6f20 3d20  .        info = 
-0000b030: 7365 6c66 2e5f 6578 7472 6163 745f 6d65  self._extract_me
-0000b040: 7461 6461 7461 2864 6174 6173 6574 2e61  tadata(dataset.a
-0000b050: 7474 7273 290a 2020 2020 2020 2020 696e  ttrs).        in
-0000b060: 666f 2e75 7064 6174 6528 7365 6c66 2e5f  fo.update(self._
-0000b070: 6578 7472 6163 745f 6d65 7461 6461 7461  extract_metadata
-0000b080: 2873 656c 662e 5f63 7572 7265 6e74 5f66  (self._current_f
-0000b090: 696c 652e 6174 7472 7329 290a 2020 2020  ile.attrs)).    
-0000b0a0: 2020 2020 696e 666f 2e75 7064 6174 6528      info.update(
-0000b0b0: 7365 6c66 2e5f 6578 7472 6163 745f 6d65  self._extract_me
-0000b0c0: 7461 6461 7461 2873 656c 662e 5f63 7572  tadata(self._cur
-0000b0d0: 7265 6e74 5f66 696c 655b 6164 635f 6e61  rent_file[adc_na
-0000b0e0: 6d65 5d2e 6174 7472 7329 290a 2020 2020  me].attrs)).    
-0000b0f0: 2020 2020 696e 666f 5b27 7265 6164 5f73      info['read_s
-0000b100: 7461 7475 7327 5d20 3d20 300a 2020 2020  tatus'] = 0.    
-0000b110: 2020 2020 696e 666f 5b27 6572 726f 725f      info['error_
-0000b120: 6d73 6727 5d20 3d20 2727 0a0a 0a20 2020  msg'] = ''...   
-0000b130: 2020 2020 2023 2065 7874 7261 6374 206c       # extract l
-0000b140: 6973 7420 6f66 2061 6463 2063 6861 6e6e  ist of adc chann
-0000b150: 656c 732c 2069 6e64 6578 2063 6f72 7265  els, index corre
-0000b160: 7370 6f6e 6420 746f 2061 7272 6179 2069  spond to array i
-0000b170: 6e64 6578 210a 2020 2020 2020 2020 6164  ndex!.        ad
-0000b180: 635f 6e75 6d73 5f66 696c 6520 3d20 696e  c_nums_file = in
-0000b190: 666f 5b27 6164 635f 6368 616e 6e65 6c5f  fo['adc_channel_
-0000b1a0: 696e 6469 6365 7327 5d0a 2020 2020 2020  indices'].      
-0000b1b0: 2020 6966 2028 6e6f 7420 6973 696e 7374    if (not isinst
-0000b1c0: 616e 6365 2861 6463 5f6e 756d 735f 6669  ance(adc_nums_fi
-0000b1d0: 6c65 2c20 6c69 7374 290a 2020 2020 2020  le, list).      
-0000b1e0: 2020 2020 2020 616e 6420 6e6f 7420 6973        and not is
-0000b1f0: 696e 7374 616e 6365 2861 6463 5f6e 756d  instance(adc_num
-0000b200: 735f 6669 6c65 2c20 6e70 2e6e 6461 7272  s_file, np.ndarr
-0000b210: 6179 2929 3a0a 2020 2020 2020 2020 2020  ay)):.          
-0000b220: 2020 6164 635f 6e75 6d73 5f66 696c 6520    adc_nums_file 
-0000b230: 3d20 6e70 2e61 7272 6179 285b 6164 635f  = np.array([adc_
-0000b240: 6e75 6d73 5f66 696c 655d 290a 2020 2020  nums_file]).    
-0000b250: 2020 2020 6e62 5f63 6861 6e6e 656c 735f      nb_channels_
-0000b260: 6669 6c65 203d 206c 656e 2861 6463 5f6e  file = len(adc_n
-0000b270: 756d 735f 6669 6c65 290a 0a0a 2020 2020  ums_file)...    
-0000b280: 2020 2020 2320 6765 7420 636f 6e6e 6563      # get connec
-0000b290: 7469 6f6e 206d 6170 2061 6e64 2063 6f6e  tion map and con
-0000b2a0: 7665 7274 2074 6f20 6e75 6d70 7920 6172  vert to numpy ar
-0000b2b0: 7261 790a 2020 2020 2020 2020 636f 6e6e  ray.        conn
-0000b2c0: 6563 7469 6f6e 7320 3d20 7365 6c66 2e67  ections = self.g
-0000b2d0: 6574 5f63 6f6e 6e65 6374 696f 6e5f 6469  et_connection_di
-0000b2e0: 6374 2861 6463 5f6e 616d 653d 6164 635f  ct(adc_name=adc_
-0000b2f0: 6e61 6d65 2c20 6d65 7461 6461 7461 3d69  name, metadata=i
-0000b300: 6e66 6f29 0a20 2020 2020 2020 2020 2020  nfo).           
-0000b310: 2020 200a 2020 2020 2020 2020 2320 4669     .        # Fi
-0000b320: 6c74 6572 2062 6173 6564 206f 6e20 6465  lter based on de
-0000b330: 7465 6374 6f72 5f63 6861 6e73 2061 7267  tector_chans arg
-0000b340: 756d 656e 740a 2020 2020 2020 2020 7365  ument.        se
-0000b350: 6c65 6374 6564 5f61 7272 6179 5f69 6e64  lected_array_ind
-0000b360: 6963 6573 203d 206c 6973 7428 290a 2020  ices = list().  
-0000b370: 2020 2020 2020 7365 6c65 6374 6564 5f61        selected_a
-0000b380: 6463 5f6e 756d 7320 3d20 6c69 7374 2829  dc_nums = list()
-0000b390: 0a20 2020 2020 2020 2073 656c 6563 7465  .        selecte
-0000b3a0: 645f 6465 7465 6374 6f72 5f63 6861 6e73  d_detector_chans
-0000b3b0: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
-0000b3c0: 2020 7365 6c65 6374 6564 5f74 6573 5f63    selected_tes_c
-0000b3d0: 6861 6e73 203d 206c 6973 7428 290a 2020  hans = list().  
-0000b3e0: 2020 2020 2020 7365 6c65 6374 6564 5f63        selected_c
-0000b3f0: 6f6e 7472 6f6c 6c65 725f 6368 616e 7320  ontroller_chans 
-0000b400: 3d20 6c69 7374 2829 0a20 2020 2020 2020  = list().       
-0000b410: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
-0000b420: 2020 2069 6620 6465 7465 6374 6f72 5f63     if detector_c
-0000b430: 6861 6e73 2069 7320 6e6f 7420 4e6f 6e65  hans is not None
-0000b440: 3a0a 2020 2020 2020 2020 2020 2020 0a20  :.            . 
-0000b450: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
-0000b460: 7665 7274 2064 6574 6563 746f 725f 6368  vert detector_ch
-0000b470: 616e 7320 746f 206c 6973 7420 6966 206e  ans to list if n
-0000b480: 6565 6465 640a 2020 2020 2020 2020 2020  eeded.          
-0000b490: 2020 6966 2028 6e6f 7420 6973 696e 7374    if (not isinst
-0000b4a0: 616e 6365 2864 6574 6563 746f 725f 6368  ance(detector_ch
-0000b4b0: 616e 732c 206c 6973 7429 0a20 2020 2020  ans, list).     
-0000b4c0: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
-0000b4d0: 6f74 2069 7369 6e73 7461 6e63 6528 6465  ot isinstance(de
-0000b4e0: 7465 6374 6f72 5f63 6861 6e73 2c20 6e70  tector_chans, np
-0000b4f0: 2e6e 6461 7272 6179 2929 3a0a 2020 2020  .ndarray)):.    
-0000b500: 2020 2020 2020 2020 2020 2020 6465 7465              dete
-0000b510: 6374 6f72 5f63 6861 6e73 203d 205b 6465  ctor_chans = [de
-0000b520: 7465 6374 6f72 5f63 6861 6e73 5d0a 2020  tector_chans].  
-0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b540: 2020 2020 2020 2020 2020 0a0a 2020 2020            ..    
-0000b550: 2020 2020 2020 2020 2320 6c6f 6f70 2073          # loop s
-0000b560: 656c 6563 7465 6420 6368 616e 6e65 6c73  elected channels
-0000b570: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000b580: 2063 6861 6e20 696e 2064 6574 6563 746f   chan in detecto
-0000b590: 725f 6368 616e 733a 0a0a 2020 2020 2020  r_chans:..      
-0000b5a0: 2020 2020 2020 2020 2020 2320 6368 6563            # chec
-0000b5b0: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
-0000b5c0: 2020 6966 2063 6861 6e20 6e6f 7420 696e    if chan not in
-0000b5d0: 2063 6f6e 6e65 6374 696f 6e73 5b27 6465   connections['de
-0000b5e0: 7465 6374 6f72 5f63 6861 6e73 275d 3a0a  tector_chans']:.
-0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b600: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000b610: 7272 6f72 2827 4465 7465 6374 6f72 2063  rror('Detector c
-0000b620: 6861 6e6e 656c 2027 202b 2063 6861 6e0a  hannel ' + chan.
-0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b650: 2020 2020 202b 2027 206e 6f74 2061 7661       + ' not ava
-0000b660: 696c 6162 6c65 2069 6e20 7261 7720 6461  ilable in raw da
-0000b670: 7461 2e27 0a20 2020 2020 2020 2020 2020  ta.'.           
-0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b690: 2020 2020 2020 2020 2020 2b20 2720 4368            + ' Ch
-0000b6a0: 6563 6b20 636f 6e6e 6563 7469 6f6e 206d  eck connection m
-0000b6b0: 6170 2127 290a 2020 2020 2020 2020 2020  ap!').          
-0000b6c0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-0000b6d0: 2020 2020 2020 2023 2066 696e 6420 6368         # find ch
-0000b6e0: 616e 6e65 6c20 696e 6465 7820 696e 2063  annel index in c
-0000b6f0: 6f6e 6e65 6374 696f 6e20 6d61 700a 2020  onnection map.  
-0000b700: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000b710: 6420 3d20 636f 6e6e 6563 7469 6f6e 735b  d = connections[
-0000b720: 2764 6574 6563 746f 725f 6368 616e 7327  'detector_chans'
-0000b730: 5d2e 696e 6465 7828 6368 616e 290a 0a20  ].index(chan).. 
-0000b740: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000b750: 2065 7874 7261 6374 2073 656c 6563 7465   extract selecte
-0000b760: 6420 4144 4320 6e75 6d62 6572 0a20 2020  d ADC number.   
-0000b770: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b780: 6563 7465 645f 6164 6320 3d20 696e 7428  ected_adc = int(
-0000b790: 636f 6e6e 6563 7469 6f6e 735b 2761 6463  connections['adc
-0000b7a0: 5f63 6861 6e73 275d 5b69 6e64 5d29 0a20  _chans'][ind]). 
-0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000b7c0: 6620 7365 6c65 6374 6564 5f61 6463 206e  f selected_adc n
-0000b7d0: 6f74 2069 6e20 6164 635f 6e75 6d73 5f66  ot in adc_nums_f
-0000b7e0: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
-0000b7f0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-0000b800: 616c 7565 4572 726f 7228 2750 726f 626c  alueError('Probl
-0000b810: 656d 2077 6974 6820 7261 7720 6461 7461  em with raw data
-0000b820: 2e20 556e 6162 6c65 2074 6f20 6669 6e64  . Unable to find
-0000b830: 2041 4443 2063 6861 6e6e 656c 2729 0a20   ADC channel'). 
-0000b840: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2320 7361 7665 2063 6f6e 6e65 6374 696f  # save connectio
-0000b870: 6e73 0a20 2020 2020 2020 2020 2020 2020  ns.             
-0000b880: 2020 2073 656c 6563 7465 645f 6164 635f     selected_adc_
-0000b890: 6e75 6d73 2e61 7070 656e 6428 7365 6c65  nums.append(sele
-0000b8a0: 6374 6564 5f61 6463 290a 2020 2020 2020  cted_adc).      
-0000b8b0: 2020 2020 2020 2020 2020 7365 6c65 6374            select
-0000b8c0: 6564 5f64 6574 6563 746f 725f 6368 616e  ed_detector_chan
-0000b8d0: 732e 6170 7065 6e64 2863 6f6e 6e65 6374  s.append(connect
-0000b8e0: 696f 6e73 5b27 6465 7465 6374 6f72 5f63  ions['detector_c
-0000b8f0: 6861 6e73 275d 5b69 6e64 5d29 0a20 2020  hans'][ind]).   
-0000b900: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000b910: 2774 6573 5f63 6861 6e73 2720 696e 2063  'tes_chans' in c
-0000b920: 6f6e 6e65 6374 696f 6e73 3a0a 2020 2020  onnections:.    
+00008300: 636f 6e74 726f 6c6c 6572 5f63 6861 6e73  controller_chans
+00008310: 2e61 7070 656e 6428 636f 6e6e 6563 7469  .append(connecti
+00008320: 6f6e 5f64 6963 745b 2763 6f6e 7472 6f6c  on_dict['control
+00008330: 6c65 725f 6368 616e 7327 5d5b 696e 645d  ler_chans'][ind]
+00008340: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008350: 2020 2020 2020 6966 2063 6f6e 6e65 6374        if connect
+00008360: 696f 6e5f 6469 6374 5b27 7465 735f 6368  ion_dict['tes_ch
+00008370: 616e 7327 5d3a 0a20 2020 2020 2020 2020  ans']:.         
+00008380: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00008390: 6573 5f63 6861 6e73 2e61 7070 656e 6428  es_chans.append(
+000083a0: 636f 6e6e 6563 7469 6f6e 5f64 6963 745b  connection_dict[
+000083b0: 2774 6573 5f63 6861 6e73 275d 5b69 6e64  'tes_chans'][ind
+000083c0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+000083d0: 2020 2020 2020 2069 6620 636f 6e6e 6563         if connec
+000083e0: 7469 6f6e 5f64 6963 745b 2764 6574 6563  tion_dict['detec
+000083f0: 746f 725f 6368 616e 7327 5d3a 0a20 2020  tor_chans']:.   
+00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008410: 2020 2020 2064 6574 6563 746f 725f 6368       detector_ch
+00008420: 616e 732e 6170 7065 6e64 2863 6f6e 6e65  ans.append(conne
+00008430: 6374 696f 6e5f 6469 6374 5b27 6465 7465  ction_dict['dete
+00008440: 6374 6f72 5f63 6861 6e73 275d 5b69 6e64  ctor_chans'][ind
+00008450: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00008460: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008480: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00008490: 2020 2020 2020 6465 7465 6374 6f72 5f63        detector_c
+000084a0: 6f6e 6669 675f 6469 6374 5b27 7465 735f  onfig_dict['tes_
+000084b0: 6368 616e 7327 5d20 3d20 2074 6573 5f63  chans'] =  tes_c
+000084c0: 6861 6e73 0a20 2020 2020 2020 2064 6574  hans.        det
+000084d0: 6563 746f 725f 636f 6e66 6967 5f64 6963  ector_config_dic
+000084e0: 745b 2764 6574 6563 746f 725f 6368 616e  t['detector_chan
+000084f0: 7327 5d20 3d20 2064 6574 6563 746f 725f  s'] =  detector_
+00008500: 6368 616e 730a 2020 2020 2020 2020 6465  chans.        de
+00008510: 7465 6374 6f72 5f63 6f6e 6669 675f 6469  tector_config_di
+00008520: 6374 5b27 636f 6e74 726f 6c6c 6572 5f63  ct['controller_c
+00008530: 6861 6e73 275d 203d 2020 636f 6e74 726f  hans'] =  contro
+00008540: 6c6c 6572 5f63 6861 6e73 2020 200a 0a20  ller_chans   .. 
+00008550: 2020 2020 2020 2023 2063 6f6e 7665 7274         # convert
+00008560: 2074 6f20 6c69 7374 2069 6620 6e65 6564   to list if need
+00008570: 6564 2028 7369 7a65 206f 6620 6e62 2063  ed (size of nb c
+00008580: 6861 6e6e 656c 7329 0a20 2020 2020 2020  hannels).       
+00008590: 206e 625f 6368 616e 203d 206c 656e 2864   nb_chan = len(d
+000085a0: 6574 6563 746f 725f 636f 6e66 6967 5f64  etector_config_d
+000085b0: 6963 745b 2764 6574 6563 746f 725f 6368  ict['detector_ch
+000085c0: 616e 7327 5d29 0a20 2020 2020 2020 2066  ans']).        f
+000085d0: 6f72 2063 6f6e 6669 6720 696e 2064 6574  or config in det
+000085e0: 6563 746f 725f 636f 6e66 6967 5f64 6963  ector_config_dic
+000085f0: 742e 6b65 7973 2829 3a0a 2020 2020 2020  t.keys():.      
+00008600: 2020 2020 2020 7061 7261 6d20 3d20 6465        param = de
+00008610: 7465 6374 6f72 5f63 6f6e 6669 675f 6469  tector_config_di
+00008620: 6374 5b63 6f6e 6669 675d 0a20 2020 2020  ct[config].     
+00008630: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+00008640: 696e 7374 616e 6365 2870 6172 616d 2c20  instance(param, 
+00008650: 6c69 7374 2920 616e 6420 6e6f 7420 6973  list) and not is
+00008660: 696e 7374 616e 6365 2870 6172 616d 2c20  instance(param, 
+00008670: 6e70 2e6e 6461 7272 6179 293a 0a20 2020  np.ndarray):.   
+00008680: 2020 2020 2020 2020 2020 2020 2064 6574               det
+00008690: 6563 746f 725f 636f 6e66 6967 5f64 6963  ector_config_dic
+000086a0: 745b 636f 6e66 6967 5d20 3d20 5b64 6574  t[config] = [det
+000086b0: 6563 746f 725f 636f 6e66 6967 5f64 6963  ector_config_dic
+000086c0: 745b 636f 6e66 6967 5d5d 2a6e 625f 6368  t[config]]*nb_ch
+000086d0: 616e 0a20 2020 200a 2020 2020 2020 2020  an.    .        
+000086e0: 2320 636f 6e76 6572 7420 746f 2064 6963  # convert to dic
+000086f0: 7469 6f6e 6172 790a 2020 2020 2020 2020  tionary.        
+00008700: 6465 7465 6374 6f72 5f63 6f6e 6669 6720  detector_config 
+00008710: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00008720: 2069 6620 7573 655f 6368 616e 5f64 6963   if use_chan_dic
+00008730: 743a 0a20 2020 2020 2020 2020 2020 2063  t:.            c
+00008740: 6861 6e5f 6c69 7374 203d 2064 6574 6563  han_list = detec
+00008750: 746f 725f 636f 6e66 6967 5f64 6963 745b  tor_config_dict[
+00008760: 2764 6574 6563 746f 725f 6368 616e 7327  'detector_chans'
+00008770: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00008780: 7220 6368 616e 2069 6e20 6368 616e 5f6c  r chan in chan_l
+00008790: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
+000087a0: 2020 2020 2063 6861 6e5f 696e 6465 7820       chan_index 
+000087b0: 3d20 6465 7465 6374 6f72 5f63 6f6e 6669  = detector_confi
+000087c0: 675f 6469 6374 5b27 6465 7465 6374 6f72  g_dict['detector
+000087d0: 5f63 6861 6e73 275d 2e69 6e64 6578 2863  _chans'].index(c
+000087e0: 6861 6e29 0a20 2020 2020 2020 2020 2020  han).           
+000087f0: 2020 2020 2064 6574 6563 746f 725f 636f       detector_co
+00008800: 6e66 6967 5b63 6861 6e5d 203d 2064 6963  nfig[chan] = dic
+00008810: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+00008820: 2020 2020 666f 7220 636f 6e66 6967 2069      for config i
+00008830: 6e20 6465 7465 6374 6f72 5f63 6f6e 6669  n detector_confi
+00008840: 675f 6469 6374 3a0a 2020 2020 2020 2020  g_dict:.        
+00008850: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00008860: 656e 2864 6574 6563 746f 725f 636f 6e66  en(detector_conf
+00008870: 6967 5f64 6963 745b 636f 6e66 6967 5d29  ig_dict[config])
+00008880: 3d3d 6e62 5f63 6861 6e3a 0a20 2020 2020  ==nb_chan:.     
+00008890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088a0: 2020 2064 6574 6563 746f 725f 636f 6e66     detector_conf
+000088b0: 6967 5b63 6861 6e5d 5b63 6f6e 6669 675d  ig[chan][config]
+000088c0: 203d 2064 6574 6563 746f 725f 636f 6e66   = detector_conf
+000088d0: 6967 5f64 6963 745b 636f 6e66 6967 5d5b  ig_dict[config][
+000088e0: 6368 616e 5f69 6e64 6578 5d0a 2020 2020  chan_index].    
+000088f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008900: 2020 2020 2020 6465 7465 6374 6f72 5f63        detector_c
+00008910: 6f6e 6669 6720 3d20 6465 7465 6374 6f72  onfig = detector
+00008920: 5f63 6f6e 6669 675f 6469 6374 0a20 2020  _config_dict.   
+00008930: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00008940: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00008950: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00008960: 2020 2020 2020 7265 7475 726e 2064 6574        return det
+00008970: 6563 746f 725f 636f 6e66 6967 0a0a 0a20  ector_config... 
+00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089a0: 2020 200a 2020 2020 6465 6620 6765 745f     .    def get_
+000089b0: 636f 6e6e 6563 7469 6f6e 5f64 6963 7428  connection_dict(
+000089c0: 7365 6c66 2c20 6669 6c65 5f6e 616d 653d  self, file_name=
+000089d0: 4e6f 6e65 2c20 6164 635f 6e61 6d65 3d27  None, adc_name='
+000089e0: 6164 6331 272c 206d 6574 6164 6174 613d  adc1', metadata=
+000089f0: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
+00008a00: 2222 0a20 2020 2020 2020 2047 6574 2063  "".        Get c
+00008a10: 6f6e 6e65 6374 696f 6e20 6469 6374 696f  onnection dictio
+00008a20: 6e61 7279 2066 6f72 2073 7065 6369 6669  nary for specifi
+00008a30: 6420 6164 6320 6e61 6d65 0a20 2020 2020  d adc name.     
+00008a40: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00008a50: 2320 696e 6974 6961 6c69 7a65 0a20 2020  # initialize.   
+00008a60: 2020 2020 2063 6f6e 6e65 6374 696f 6e5f       connection_
+00008a70: 6469 6374 3d64 6963 7428 290a 0a20 2020  dict=dict()..   
+00008a80: 2020 2020 2023 206d 6574 6164 6174 610a       # metadata.
+00008a90: 2020 2020 2020 2020 6164 635f 6d65 7461          adc_meta
+00008aa0: 6461 7461 203d 204e 6f6e 650a 2020 2020  data = None.    
+00008ab0: 2020 2020 6966 206d 6574 6164 6174 6120      if metadata 
+00008ac0: 6973 204e 6f6e 6520 6f72 2027 6772 6f75  is None or 'grou
+00008ad0: 705f 6c69 7374 2720 6e6f 7420 696e 206d  p_list' not in m
+00008ae0: 6574 6164 6174 613a 0a20 2020 2020 2020  etadata:.       
+00008af0: 2020 2020 206d 6574 6164 6174 6120 3d20       metadata = 
+00008b00: 7365 6c66 2e67 6574 5f6d 6574 6164 6174  self.get_metadat
+00008b10: 6128 6669 6c65 5f6e 616d 653d 6669 6c65  a(file_name=file
+00008b20: 5f6e 616d 6529 0a0a 2020 2020 2020 2020  _name)..        
+00008b30: 6966 2027 6772 6f75 705f 6c69 7374 2720  if 'group_list' 
+00008b40: 696e 206d 6574 6164 6174 6120 616e 6420  in metadata and 
+00008b50: 6164 635f 6e61 6d65 2069 6e20 6d65 7461  adc_name in meta
+00008b60: 6461 7461 5b27 6772 6f75 705f 6c69 7374  data['group_list
+00008b70: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+00008b80: 6164 635f 6d65 7461 6461 7461 2020 3d20  adc_metadata  = 
+00008b90: 6d65 7461 6461 7461 5b27 6772 6f75 7073  metadata['groups
+00008ba0: 275d 5b61 6463 5f6e 616d 655d 0a0a 2020  '][adc_name]..  
+00008bb0: 2020 2020 2020 6966 2061 6463 5f6d 6574        if adc_met
+00008bc0: 6164 6174 6120 6973 204e 6f6e 653a 0a20  adata is None:. 
+00008bd0: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+00008be0: 5f6d 7367 203d 2027 4144 4320 6d65 7461  _msg = 'ADC meta
+00008bf0: 6461 7461 206e 6f74 2066 6f75 6e64 2127  data not found!'
+00008c00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00008c10: 7365 6c66 2e5f 7261 6973 655f 6572 726f  self._raise_erro
+00008c20: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00008c30: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00008c40: 6c75 6545 7272 6f72 2865 7272 6f72 5f6d  lueError(error_m
+00008c50: 7367 290a 2020 2020 2020 2020 2020 2020  sg).            
+00008c60: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00008c70: 2020 2020 2020 7072 696e 7428 2757 4152        print('WAR
+00008c80: 4e49 4e47 3a20 2720 2b20 6572 726f 725f  NING: ' + error_
+00008c90: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
+00008ca0: 2020 2020 2072 6574 7572 6e20 636f 6e65       return cone
+00008cb0: 6374 696f 6e5f 6469 6374 0a0a 0a20 2020  ction_dict...   
+00008cc0: 2020 2020 2063 6f6e 6e65 6374 696f 6e5f       connection_
+00008cd0: 6469 6374 5b27 6164 635f 6368 616e 7327  dict['adc_chans'
+00008ce0: 5d20 3d20 6c69 7374 2829 0a20 2020 2020  ] = list().     
+00008cf0: 2020 2063 6f6e 6e65 6374 696f 6e5f 6469     connection_di
+00008d00: 6374 5b27 636f 6e74 726f 6c6c 6572 5f63  ct['controller_c
+00008d10: 6861 6e73 275d 203d 206c 6973 7428 290a  hans'] = list().
+00008d20: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
+00008d30: 6f6e 5f64 6963 745b 2774 6573 5f63 6861  on_dict['tes_cha
+00008d40: 6e73 275d 203d 206c 6973 7428 290a 2020  ns'] = list().  
+00008d50: 2020 2020 2020 636f 6e6e 6563 7469 6f6e        connection
+00008d60: 5f64 6963 745b 2764 6574 6563 746f 725f  _dict['detector_
+00008d70: 6368 616e 7327 5d20 3d20 6c69 7374 2829  chans'] = list()
+00008d80: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00008d90: 2020 2320 6c6f 6f70 206d 6574 6164 6174    # loop metadat
+00008da0: 6120 746f 2066 696e 6420 636f 6e6e 6563  a to find connec
+00008db0: 7469 6f6e 730a 2020 2020 2020 2020 666f  tions.        fo
+00008dc0: 7220 6b65 792c 7661 6c75 6520 696e 2061  r key,value in a
+00008dd0: 6463 5f6d 6574 6164 6174 612e 6974 656d  dc_metadata.item
+00008de0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00008df0: 2069 6620 6b65 792e 6669 6e64 2827 636f   if key.find('co
+00008e00: 6e6e 6563 7469 6f6e 2729 213d 2d31 3a0a  nnection')!=-1:.
+00008e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e20: 636f 6e6e 6563 7469 6f6e 5f64 6963 745b  connection_dict[
+00008e30: 2761 6463 5f63 6861 6e73 275d 2e61 7070  'adc_chans'].app
+00008e40: 656e 6428 696e 7428 6b65 795b 3130 3a5d  end(int(key[10:]
+00008e50: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00008e60: 2020 2066 6f72 2063 6f6e 6e65 6374 696f     for connectio
+00008e70: 6e5f 7479 7065 2069 6e20 7661 6c75 653a  n_type in value:
+00008e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008e90: 2020 2020 2063 6861 6e6e 656c 5f6e 616d       channel_nam
+00008ea0: 6520 3d20 636f 6e6e 6563 7469 6f6e 5f74  e = connection_t
+00008eb0: 7970 655b 636f 6e6e 6563 7469 6f6e 5f74  ype[connection_t
+00008ec0: 7970 652e 6669 6e64 2827 3a27 292b 313a  ype.find(':')+1:
+00008ed0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00008ee0: 2020 2020 2020 6966 2063 6f6e 6e65 6374        if connect
+00008ef0: 696f 6e5f 7479 7065 2e66 696e 6428 2774  ion_type.find('t
+00008f00: 6573 3a27 2921 3d2d 313a 0a20 2020 2020  es:')!=-1:.     
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f20: 2020 2063 6f6e 6e65 6374 696f 6e5f 6469     connection_di
+00008f30: 6374 5b27 7465 735f 6368 616e 7327 5d2e  ct['tes_chans'].
+00008f40: 6170 7065 6e64 2863 6861 6e6e 656c 5f6e  append(channel_n
+00008f50: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+00008f60: 2020 2020 2020 2020 2069 6620 636f 6e6e           if conn
+00008f70: 6563 7469 6f6e 5f74 7970 652e 6669 6e64  ection_type.find
+00008f80: 2827 6465 7465 6374 6f72 3a27 2921 3d2d  ('detector:')!=-
+00008f90: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+00008fa0: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
+00008fb0: 6374 696f 6e5f 6469 6374 5b27 6465 7465  ction_dict['dete
+00008fc0: 6374 6f72 5f63 6861 6e73 275d 2e61 7070  ctor_chans'].app
+00008fd0: 656e 6428 6368 616e 6e65 6c5f 6e61 6d65  end(channel_name
+00008fe0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008ff0: 2020 2020 2020 6966 2063 6f6e 6e65 6374        if connect
+00009000: 696f 6e5f 7479 7065 2e66 696e 6428 2763  ion_type.find('c
+00009010: 6f6e 7472 6f6c 6c65 723a 2729 213d 2d31  ontroller:')!=-1
+00009020: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009030: 2020 2020 2020 2020 2020 636f 6e6e 6563            connec
+00009040: 7469 6f6e 5f64 6963 745b 2763 6f6e 7472  tion_dict['contr
+00009050: 6f6c 6c65 725f 6368 616e 7327 5d2e 6170  oller_chans'].ap
+00009060: 7065 6e64 2863 6861 6e6e 656c 5f6e 616d  pend(channel_nam
+00009070: 6529 0a0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00009080: 726e 2063 6f6e 6e65 6374 696f 6e5f 6469  rn connection_di
+00009090: 6374 2020 2020 2020 2020 2020 2020 2020  ct              
+000090a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090b0: 0a20 2020 200a 0a20 2020 2064 6566 2067  .    ..    def g
+000090c0: 6574 5f63 6f6e 6e65 6374 696f 6e5f 7461  et_connection_ta
+000090d0: 626c 6528 7365 6c66 2c20 6669 6c65 5f6e  ble(self, file_n
+000090e0: 616d 653d 4e6f 6e65 2c20 6d65 7461 6461  ame=None, metada
+000090f0: 7461 3d4e 6f6e 6529 3a0a 2020 2020 2020  ta=None):.      
+00009100: 2020 2222 220a 2020 2020 2020 2020 4765    """.        Ge
+00009110: 7420 636f 6e6e 6563 7469 6f6e 2074 6162  t connection tab
+00009120: 6c65 0a20 2020 2020 2020 2022 2222 0a20  le.        """. 
+00009130: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00009140: 6966 206d 6574 6164 6174 6120 6973 204e  if metadata is N
+00009150: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00009160: 206d 6574 6164 6174 6120 3d20 7365 6c66   metadata = self
+00009170: 2e67 6574 5f6d 6574 6164 6174 6128 6669  .get_metadata(fi
+00009180: 6c65 5f6e 616d 653d 6669 6c65 5f6e 616d  le_name=file_nam
+00009190: 6529 0a20 2020 2020 2020 200a 2020 2020  e).        .    
+000091a0: 2020 2020 2320 6368 6563 6b20 6164 6320      # check adc 
+000091b0: 6c69 7374 2065 7869 7374 200a 2020 2020  list exist .    
+000091c0: 2020 2020 6966 2027 6164 635f 6c69 7374      if 'adc_list
+000091d0: 2720 6e6f 7420 696e 206d 6574 6164 6174  ' not in metadat
+000091e0: 613a 0a20 2020 2020 2020 2020 2020 2070  a:.            p
+000091f0: 7269 6e74 2827 4552 524f 523a 204e 6f20  rint('ERROR: No 
+00009200: 4144 4320 6d65 7461 6461 7461 2066 6f75  ADC metadata fou
+00009210: 6e64 2069 6e20 7468 6520 6669 6c65 2127  nd in the file!'
+00009220: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00009230: 7475 726e 0a0a 2020 2020 2020 2020 0a20  turn..        . 
+00009240: 2020 2020 2020 2023 206c 6f6f 7020 6164         # loop ad
+00009250: 6320 616e 6420 6669 6e64 2063 6f6e 6e65  c and find conne
+00009260: 6374 696f 6e0a 2020 2020 2020 2020 636f  ction.        co
+00009270: 6e6e 6563 7469 6f6e 5f6c 6973 7420 3d20  nnection_list = 
+00009280: 6c69 7374 2829 0a20 2020 2020 2020 2063  list().        c
+00009290: 6f6e 6e65 6374 696f 6e5f 6e61 6d65 5f6c  onnection_name_l
+000092a0: 6973 7420 3d20 6c69 7374 2829 0a20 2020  ist = list().   
+000092b0: 2020 2020 2066 6f72 2061 6463 5f69 6420       for adc_id 
+000092c0: 696e 206d 6574 6164 6174 615b 2761 6463  in metadata['adc
+000092d0: 5f6c 6973 7427 5d3a 0a20 2020 2020 2020  _list']:.       
+000092e0: 2020 2020 2061 6463 5f6d 6574 6164 6174       adc_metadat
+000092f0: 6120 3d20 6d65 7461 6461 7461 5b27 6772  a = metadata['gr
+00009300: 6f75 7073 275d 5b61 6463 5f69 645d 0a20  oups'][adc_id]. 
+00009310: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+00009320: 6579 2c76 616c 2069 6e20 6164 635f 6d65  ey,val in adc_me
+00009330: 7461 6461 7461 2e69 7465 6d73 2829 3a0a  tadata.items():.
+00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009350: 6966 206b 6579 5b30 3a31 305d 3d3d 2763  if key[0:10]=='c
+00009360: 6f6e 6e65 6374 696f 6e27 3a0a 2020 2020  onnection':.    
+00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009380: 6164 635f 6368 616e 203d 2072 652e 7375  adc_chan = re.su
+00009390: 6228 7227 5c73 2b27 2c27 272c 2073 7472  b(r'\s+','', str
+000093a0: 286b 6579 2929 5b31 303a 5d0a 2020 2020  (key))[10:].    
+000093b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093c0: 6e61 6d65 5f76 616c 5f6c 6973 742c 206e  name_val_list, n
+000093d0: 616d 655f 6c69 7374 2c20 7661 6c5f 6c69  ame_list, val_li
+000093e0: 7374 203d 2028 0a20 2020 2020 2020 2020  st = (.         
+000093f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009400: 6f6e 6e65 6374 696f 6e5f 7574 696c 732e  onnection_utils.
+00009410: 6578 7472 6163 745f 6164 635f 636f 6e6e  extract_adc_conn
+00009420: 6563 7469 6f6e 286c 6973 7428 7661 6c29  ection(list(val)
+00009430: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00009440: 2020 2020 2020 2076 616c 5f6c 6973 7420         val_list 
+00009450: 203d 205b 6164 635f 6964 2c61 6463 5f63   = [adc_id,adc_c
+00009460: 6861 6e5d 202b 2076 616c 5f6c 6973 740a  han] + val_list.
+00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009480: 2020 2020 6e61 6d65 5f6c 6973 7420 3d20      name_list = 
+00009490: 5b27 6164 635f 6964 272c 2761 6463 5f63  ['adc_id','adc_c
+000094a0: 6861 6e6e 656c 275d 202b 206e 616d 655f  hannel'] + name_
+000094b0: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
+000094c0: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
+000094d0: 696f 6e5f 6c69 7374 2e61 7070 656e 6428  ion_list.append(
+000094e0: 7661 6c5f 6c69 7374 290a 2020 2020 2020  val_list).      
+000094f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00009500: 206e 6f74 2063 6f6e 6e65 6374 696f 6e5f   not connection_
+00009510: 6e61 6d65 5f6c 6973 743a 0a20 2020 2020  name_list:.     
+00009520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009530: 2020 2063 6f6e 6e65 6374 696f 6e5f 6e61     connection_na
+00009540: 6d65 5f6c 6973 7420 3d20 6e61 6d65 5f6c  me_list = name_l
+00009550: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
+00009560: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
+00009570: 6e65 6374 696f 6e5f 6e61 6d65 5f6c 6973  nection_name_lis
+00009580: 7421 3d6e 616d 655f 6c69 7374 3a0a 2020  t!=name_list:.  
+00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095a0: 2020 2020 2020 7072 696e 7428 2745 5252        print('ERR
+000095b0: 4f52 3a20 6d69 7373 696e 6720 6164 6320  OR: missing adc 
+000095c0: 636f 6e6e 6563 7469 6f6e 2076 616c 7565  connection value
+000095d0: 7321 2729 0a20 2020 2020 2020 2020 2020  s!').           
+000095e0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009600: 2020 0a20 2020 2020 2020 2063 6f6e 6e65    .        conne
+00009610: 6374 696f 6e5f 7461 626c 6520 3d20 7064  ction_table = pd
+00009620: 2e44 6174 6146 7261 6d65 2863 6f6e 6e65  .DataFrame(conne
+00009630: 6374 696f 6e5f 6c69 7374 2c0a 2020 2020  ction_list,.    
+00009640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009660: 2020 2020 636f 6c75 6d6e 733d 636f 6e6e      columns=conn
+00009670: 6563 7469 6f6e 5f6e 616d 655f 6c69 7374  ection_name_list
+00009680: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+00009690: 6e20 636f 6e6e 6563 7469 6f6e 5f74 6162  n connection_tab
+000096a0: 6c65 0a0a 0a0a 2020 2020 0a20 2020 2064  le....    .    d
+000096b0: 6566 205f 6f70 656e 5f66 696c 6528 7365  ef _open_file(se
+000096c0: 6c66 2c20 6669 6c65 5f6e 616d 652c 2065  lf, file_name, e
+000096d0: 7665 6e74 5f6c 6973 743d 4e6f 6e65 2c0a  vent_list=None,.
+000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096f0: 2020 2072 775f 7374 7269 6e67 3d27 7227     rw_string='r'
+00009700: 2c20 6c6f 6164 5f6d 6574 6164 6174 613d  , load_metadata=
+00009710: 5472 7565 293a 0a20 2020 2020 2020 2022  True):.        "
+00009720: 2222 0a20 2020 2020 2020 206f 7065 6e20  "".        open 
+00009730: 6669 6c65 200a 2020 2020 2020 2020 2222  file .        ""
+00009740: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+00009750: 662e 5f63 7572 7265 6e74 5f66 696c 6520  f._current_file 
+00009760: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00009770: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00009780: 6c6f 7365 5f66 696c 6528 290a 2020 2020  lose_file().    
+00009790: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000097a0: 2066 696c 6520 3d20 4e6f 6e65 0a20 2020   file = None.   
+000097b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000097c0: 2020 2020 2020 6669 6c65 203d 2068 3570        file = h5p
+000097d0: 792e 4669 6c65 2866 696c 655f 6e61 6d65  y.File(file_name
+000097e0: 2c20 7277 5f73 7472 696e 6729 0a20 2020  , rw_string).   
+000097f0: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+00009800: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00009810: 4552 524f 523a 2075 6e61 626c 6520 746f  ERROR: unable to
+00009820: 206f 7065 6e20 6669 6c65 2027 202b 2066   open file ' + f
+00009830: 696c 655f 6e61 6d65 290a 2020 2020 2020  ile_name).      
+00009840: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+00009850: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
+00009860: 656e 745f 6669 6c65 203d 2066 696c 650a  ent_file = file.
+00009870: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
+00009880: 7272 656e 745f 6669 6c65 5f6e 616d 6520  rrent_file_name 
+00009890: 3d20 6669 6c65 5f6e 616d 650a 2020 2020  = file_name.    
+000098a0: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
+000098b0: 745f 6669 6c65 5f6e 625f 6576 656e 7473  t_file_nb_events
+000098c0: 203d 2030 0a20 2020 2020 2020 2073 656c   = 0.        sel
+000098d0: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
+000098e0: 6576 656e 745f 636f 756e 7465 7220 3d20  event_counter = 
+000098f0: 300a 2020 2020 2020 2020 0a20 2020 2020  0.        .     
+00009900: 2020 2023 206c 6f61 6420 6d65 7461 6461     # load metada
+00009910: 7461 0a20 2020 2020 2020 2069 6620 6c6f  ta.        if lo
+00009920: 6164 5f6d 6574 6164 6174 613a 0a0a 2020  ad_metadata:..  
+00009930: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00009940: 6c6f 6164 5f6d 6574 6164 6174 6128 290a  load_metadata().
+00009950: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00009960: 2020 2020 2020 2020 2023 2063 6865 636b           # check
+00009970: 206e 6220 6f66 2065 7665 6e74 7320 696e   nb of events in
+00009980: 2066 696c 650a 2020 2020 2020 2020 2020   file.          
+00009990: 2020 6966 2027 6164 635f 6c69 7374 2720    if 'adc_list' 
+000099a0: 6e6f 7420 696e 2073 656c 662e 5f63 7572  not in self._cur
+000099b0: 7265 6e74 5f66 696c 655f 6d65 7461 6461  rent_file_metada
+000099c0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
+000099d0: 2020 2020 7072 696e 7428 2757 4152 4e49      print('WARNI
+000099e0: 4e47 3a20 4e6f 2041 4443 2069 6e66 6f72  NG: No ADC infor
+000099f0: 6d61 7469 6f6e 2066 6f75 6e64 2069 6e20  mation found in 
+00009a00: 7468 6520 6669 6c65 2729 0a20 2020 2020  the file').     
+00009a10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009a20: 6e0a 0a20 2020 2020 2020 2020 2020 2066  n..            f
+00009a30: 6f72 2061 6463 5f6e 616d 6520 696e 2073  or adc_name in s
+00009a40: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+00009a50: 655f 6d65 7461 6461 7461 5b27 6164 635f  e_metadata['adc_
+00009a60: 6c69 7374 275d 3a0a 2020 2020 2020 2020  list']:.        
+00009a70: 2020 2020 2020 2020 6e62 5f65 7665 6e74          nb_event
+00009a80: 735f 6164 6320 3d20 7365 6c66 2e5f 6375  s_adc = self._cu
+00009a90: 7272 656e 745f 6669 6c65 5f6d 6574 6164  rrent_file_metad
+00009aa0: 6174 615b 2767 726f 7570 7327 5d5b 6164  ata['groups'][ad
+00009ab0: 635f 6e61 6d65 5d5b 276e 625f 6461 7461  c_name]['nb_data
+00009ac0: 7365 7473 275d 0a20 2020 2020 2020 2020  sets'].         
+00009ad0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+00009ae0: 6375 7272 656e 745f 6669 6c65 5f6e 625f  current_file_nb_
+00009af0: 6576 656e 7473 3d3d 303a 0a20 2020 2020  events==0:.     
+00009b00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009b10: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+00009b20: 655f 6e62 5f65 7665 6e74 7320 3d20 6e62  e_nb_events = nb
+00009b30: 5f65 7665 6e74 735f 6164 630a 2020 2020  _events_adc.    
+00009b40: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00009b50: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
+00009b60: 696c 655f 6e62 5f65 7665 6e74 7320 213d  ile_nb_events !=
+00009b70: 206e 625f 6576 656e 7473 5f61 6463 3a0a   nb_events_adc:.
+00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b90: 2020 2020 7072 696e 7428 2745 5252 4f52      print('ERROR
+00009ba0: 3a20 496e 636f 6e73 6973 7465 6e74 206e  : Inconsistent n
+00009bb0: 756d 6265 7220 6f66 2065 7665 6e74 7320  umber of events 
+00009bc0: 6265 7477 6565 6e20 4144 4320 6465 7669  between ADC devi
+00009bd0: 6365 7321 2729 0a20 2020 2020 2020 2020  ces!').         
+00009be0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009bf0: 5f63 6c6f 7365 5f66 696c 6528 290a 2020  _close_file().  
+00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c10: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00009c20: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
+00009c30: 6c65 5f63 6f75 6e74 6572 202b 3d20 310a  le_counter += 1.
+00009c40: 0a0a 2020 2020 2020 2020 2320 6576 656e  ..        # even
+00009c50: 7420 6c69 7374 0a20 2020 2020 2020 2073  t list.        s
+00009c60: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+00009c70: 655f 6576 656e 745f 6c69 7374 203d 2065  e_event_list = e
+00009c80: 7665 6e74 5f6c 6973 740a 2020 2020 2020  vent_list.      
+00009c90: 2020 6966 2065 7665 6e74 5f6c 6973 7420    if event_list 
+00009ca0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00009cb0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00009cc0: 7572 7265 6e74 5f66 696c 655f 6e62 5f65  urrent_file_nb_e
+00009cd0: 7665 6e74 7320 3d20 6c65 6e28 6576 656e  vents = len(even
+00009ce0: 745f 6c69 7374 290a 2020 2020 2020 2020  t_list).        
+00009cf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009d00: 5472 7565 0a20 2020 2020 2020 200a 2020  True.        .  
+00009d10: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00009d20: 2020 200a 2020 2020 0a0a 2020 2020 6465     .    ..    de
+00009d30: 6620 5f63 6c6f 7365 5f66 696c 6528 7365  f _close_file(se
+00009d40: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00009d50: 0a20 2020 2020 2020 2043 6c6f 7365 2063  .        Close c
+00009d60: 7572 7265 6e74 2066 696c 6520 616e 6420  urrent file and 
+00009d70: 7265 7365 740a 2020 2020 2020 2020 6375  reset.        cu
+00009d80: 7272 656e 7420 6669 6c65 2070 6172 616d  rrent file param
+00009d90: 6574 6572 730a 0a20 2020 2020 2020 2050  eters..        P
+00009da0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00009db0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00009dc0: 2020 2020 204e 6f6e 650a 0a20 2020 2020       None..     
+00009dd0: 2020 2052 6574 7572 6e0a 2020 2020 2020     Return.      
+00009de0: 2020 2d2d 2d2d 2d2d 0a20 2020 2020 2020    ------.       
+00009df0: 204e 6f6e 650a 0a20 2020 2020 2020 2022   None..        "
+00009e00: 2222 0a0a 2020 2020 2020 2020 6966 2073  ""..        if s
+00009e10: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+00009e20: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00009e30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009e40: 5f63 7572 7265 6e74 5f66 696c 652e 636c  _current_file.cl
+00009e50: 6f73 6528 290a 2020 0a20 2020 2020 2020  ose().  .       
+00009e60: 2023 2069 6e69 7469 616c 697a 650a 2020   # initialize.  
+00009e70: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
+00009e80: 656e 745f 6669 6c65 203d 204e 6f6e 650a  ent_file = None.
+00009e90: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
+00009ea0: 7272 656e 745f 6669 6c65 5f6e 616d 6520  rrent_file_name 
+00009eb0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00009ec0: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+00009ed0: 655f 6d65 7461 6461 7461 203d 204e 6f6e  e_metadata = Non
+00009ee0: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00009ef0: 6375 7272 656e 745f 6669 6c65 5f6e 625f  current_file_nb_
+00009f00: 6576 656e 7473 203d 2030 0a20 2020 2020  events = 0.     
+00009f10: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
+00009f20: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
+00009f30: 7465 7220 3d20 300a 2020 2020 2020 2020  ter = 0.        
+00009f40: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+00009f50: 6c65 5f65 7665 6e74 5f6c 6973 7420 3d20  le_event_list = 
+00009f60: 4e6f 6e65 0a20 2020 2020 2020 200a 0a20  None.        .. 
+00009f70: 2020 2064 6566 205f 6c6f 6164 5f6d 6574     def _load_met
+00009f80: 6164 6174 6128 7365 6c66 2c20 696e 636c  adata(self, incl
+00009f90: 7564 655f 6461 7461 7365 745f 6d65 7461  ude_dataset_meta
+00009fa0: 6461 7461 3d46 616c 7365 293a 0a0a 2020  data=False):..  
+00009fb0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00009fc0: 2020 4675 6e63 7469 6f6e 2074 6f20 6c6f    Function to lo
+00009fd0: 6164 2061 6c6c 206d 6574 6164 6174 6120  ad all metadata 
+00009fe0: 6672 6f6d 2063 7572 7265 6e74 2066 696c  from current fil
+00009ff0: 652e 2053 746f 7265 2069 6e20 0a20 2020  e. Store in .   
+0000a000: 2020 2020 2061 6e20 696e 7465 726e 616c       an internal
+0000a010: 2064 6963 7469 6f6e 6172 790a 0a20 2020   dictionary..   
+0000a020: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+0000a030: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000a040: 2d2d 0a0a 2020 2020 2020 2020 696e 636c  --..        incl
+0000a050: 7564 655f 6461 7461 7365 745f 6d65 7461  ude_dataset_meta
+0000a060: 6461 7461 203a 2062 6f6f 6c2c 206f 7074  data : bool, opt
+0000a070: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000a080: 2069 6620 5472 7565 2c20 7265 6164 2064   if True, read d
+0000a090: 6174 6173 6574 206d 6574 6164 6174 610a  ataset metadata.
+0000a0a0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+0000a0b0: 6c74 3a20 4661 6c73 650a 0a0a 2020 2020  lt: False...    
+0000a0c0: 2020 2020 5265 7475 726e 0a20 2020 2020      Return.     
+0000a0d0: 2020 202d 2d2d 2d2d 2d0a 2020 2020 2020     ------.      
+0000a0e0: 2020 0a20 2020 2020 2020 206d 6574 6164    .        metad
+0000a0f0: 6174 615f 6469 6374 203a 2064 6963 740a  ata_dict : dict.
+0000a100: 2020 2020 2020 2020 2020 6469 6374 696f            dictio
+0000a110: 6e61 7279 2077 6974 6820 6d65 7461 6461  nary with metada
+0000a120: 7461 0a20 2020 2020 2020 200a 0a20 2020  ta.        ..   
+0000a130: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+0000a140: 2020 2320 6368 6563 6b20 6966 2066 696c    # check if fil
+0000a150: 6520 6578 6973 740a 2020 2020 2020 2020  e exist.        
+0000a160: 6966 2073 656c 662e 5f63 7572 7265 6e74  if self._current
+0000a170: 5f66 696c 6520 6973 204e 6f6e 653a 0a20  _file is None:. 
+0000a180: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a190: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+0000a1a0: 200a 2020 2020 2020 2020 2320 696e 6974   .        # init
+0000a1b0: 6961 6c69 7a65 2063 6f6e 7461 696e 6e65  ialize containne
+0000a1c0: 720a 2020 2020 2020 2020 6d65 7461 6461  r.        metada
+0000a1d0: 7461 5f64 6963 7420 3d20 6469 6374 2829  ta_dict = dict()
+0000a1e0: 0a20 2020 2020 200a 0a20 2020 2020 2020  .      ..       
+0000a1f0: 2023 2066 696c 6520 6d61 7461 6461 7461   # file matadata
+0000a200: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
+0000a210: 615f 6469 6374 203d 2073 656c 662e 5f65  a_dict = self._e
+0000a220: 7874 7261 6374 5f6d 6574 6164 6174 6128  xtract_metadata(
+0000a230: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+0000a240: 6c65 2e61 7474 7273 290a 2020 2020 2020  le.attrs).      
+0000a250: 0a20 2020 200a 2020 2020 2020 2020 2320  .    .        # 
+0000a260: 6772 6f75 702f 6461 7461 7365 7420 6d65  group/dataset me
+0000a270: 7461 6461 7461 0a20 2020 2020 2020 206d  tadata.        m
+0000a280: 6574 6164 6174 615f 6469 6374 5b27 6772  etadata_dict['gr
+0000a290: 6f75 705f 6c69 7374 275d 203d 206c 6973  oup_list'] = lis
+0000a2a0: 7428 290a 2020 2020 2020 2020 6d65 7461  t().        meta
+0000a2b0: 6461 7461 5f64 6963 745b 2761 6463 5f6c  data_dict['adc_l
+0000a2c0: 6973 7427 5d20 3d20 6c69 7374 2829 0a20  ist'] = list(). 
+0000a2d0: 2020 2020 2020 206d 6574 6164 6174 615f         metadata_
+0000a2e0: 6469 6374 5b27 6772 6f75 7073 275d 203d  dict['groups'] =
+0000a2f0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0000a300: 2020 200a 2020 2020 2020 2020 2320 4c6f     .        # Lo
+0000a310: 6f70 2067 726f 7570 730a 2020 2020 2020  op groups.      
+0000a320: 2020 666f 7220 6b65 792c 2067 726f 7570    for key, group
+0000a330: 2069 6e20 7365 6c66 2e5f 6375 7272 656e   in self._curren
+0000a340: 745f 6669 6c65 2e69 7465 6d73 2829 3a0a  t_file.items():.
+0000a350: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000a360: 2020 2020 2320 7570 6461 7465 206c 6973      # update lis
+0000a370: 740a 2020 2020 2020 2020 2020 2020 6d65  t.            me
+0000a380: 7461 6461 7461 5f64 6963 745b 2767 726f  tadata_dict['gro
+0000a390: 7570 5f6c 6973 7427 5d2e 6170 7065 6e64  up_list'].append
+0000a3a0: 286b 6579 290a 2020 2020 2020 2020 2020  (key).          
+0000a3b0: 2020 6966 206b 6579 5b30 3a33 5d3d 3d27    if key[0:3]=='
+0000a3c0: 6164 6327 3a0a 2020 2020 2020 2020 2020  adc':.          
+0000a3d0: 2020 2020 2020 6d65 7461 6461 7461 5f64        metadata_d
+0000a3e0: 6963 745b 2761 6463 5f6c 6973 7427 5d2e  ict['adc_list'].
+0000a3f0: 6170 7065 6e64 286b 6579 290a 2020 2020  append(key).    
+0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a410: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000a420: 2020 2020 2020 2020 2023 2073 6176 6520           # save 
+0000a430: 6d65 7461 6461 7461 0a20 2020 2020 2020  metadata.       
+0000a440: 2020 2020 206d 6574 6164 6174 615f 6469       metadata_di
+0000a450: 6374 5b27 6772 6f75 7073 275d 5b6b 6579  ct['groups'][key
+0000a460: 5d20 3d20 6469 6374 2829 0a20 2020 2020  ] = dict().     
+0000a470: 2020 2020 2020 206d 6574 6164 6174 615f         metadata_
+0000a480: 6469 6374 5b27 6772 6f75 7073 275d 5b6b  dict['groups'][k
+0000a490: 6579 5d20 3d20 2073 656c 662e 5f65 7874  ey] =  self._ext
+0000a4a0: 7261 6374 5f6d 6574 6164 6174 6128 6772  ract_metadata(gr
+0000a4b0: 6f75 702e 6174 7472 7329 0a20 2020 2020  oup.attrs).     
+0000a4c0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+0000a4d0: 2320 6461 7461 7365 7473 0a20 2020 2020  # datasets.     
+0000a4e0: 2020 2020 2020 2064 6174 6173 6574 5f6c         dataset_l
+0000a4f0: 6973 7420 3d20 6c69 7374 2867 726f 7570  ist = list(group
+0000a500: 2e6b 6579 7328 2929 0a20 2020 2020 2020  .keys()).       
+0000a510: 2020 2020 206d 6574 6164 6174 615f 6469       metadata_di
+0000a520: 6374 5b27 6772 6f75 7073 275d 5b6b 6579  ct['groups'][key
+0000a530: 5d5b 2764 6174 6173 6574 5f6c 6973 7427  ]['dataset_list'
+0000a540: 5d20 3d20 6461 7461 7365 745f 6c69 7374  ] = dataset_list
+0000a550: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+0000a560: 6164 6174 615f 6469 6374 5b27 6772 6f75  adata_dict['grou
+0000a570: 7073 275d 5b6b 6579 5d5b 276e 625f 6461  ps'][key]['nb_da
+0000a580: 7461 7365 7473 275d 203d 206c 656e 2864  tasets'] = len(d
+0000a590: 6174 6173 6574 5f6c 6973 7429 0a20 2020  ataset_list).   
+0000a5a0: 2020 2020 2020 2020 2020 2020 200a 0a20               .. 
+0000a5b0: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+0000a5c0: 636c 7564 655f 6461 7461 7365 745f 6d65  clude_dataset_me
+0000a5d0: 7461 6461 7461 2061 6e64 206c 656e 2864  tadata and len(d
+0000a5e0: 6174 6173 6574 5f6c 6973 7429 3e30 3a0a  ataset_list)>0:.
+0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a600: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+0000a610: 2020 2020 2023 204c 6f6f 7020 6461 7461       # Loop data
+0000a620: 7365 7473 2061 6e64 2061 6464 206d 6574  sets and add met
+0000a630: 6164 6174 610a 2020 2020 2020 2020 2020  adata.          
+0000a640: 2020 2020 2020 6d65 7461 6461 7461 5f64        metadata_d
+0000a650: 6963 745b 2767 726f 7570 7327 5d5b 6b65  ict['groups'][ke
+0000a660: 795d 5b27 6461 7461 7365 7473 275d 203d  y]['datasets'] =
+0000a670: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0000a680: 2020 2020 2020 2020 666f 7220 6461 7461          for data
+0000a690: 7365 745f 6b65 792c 2064 6174 6173 6574  set_key, dataset
+0000a6a0: 2069 6e20 6772 6f75 702e 6974 656d 7328   in group.items(
+0000a6b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000a6c0: 2020 2020 2020 206d 6574 6164 6174 615f         metadata_
+0000a6d0: 6469 6374 5b27 6772 6f75 7073 275d 5b6b  dict['groups'][k
+0000a6e0: 6579 5d5b 2764 6174 6173 6574 7327 5d5b  ey]['datasets'][
+0000a6f0: 6461 7461 7365 745f 6b65 795d 203d 2028  dataset_key] = (
+0000a700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a710: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
+0000a720: 7874 7261 6374 5f6d 6574 6164 6174 6128  xtract_metadata(
+0000a730: 6461 7461 7365 742e 6174 7472 7329 0a20  dataset.attrs). 
+0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a750: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+0000a760: 2020 2020 2020 2020 2020 2020 2020 0a0a                ..
+0000a770: 2020 2020 2020 2020 2320 7361 7665 0a20          # save. 
+0000a780: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
+0000a790: 7265 6e74 5f66 696c 655f 6d65 7461 6461  rent_file_metada
+0000a7a0: 7461 203d 206d 6574 6164 6174 615f 6469  ta = metadata_di
+0000a7b0: 6374 0a0a 2020 2020 2020 2020 0a20 2020  ct..        .   
+0000a7c0: 2064 6566 205f 6578 7472 6163 745f 6d65   def _extract_me
+0000a7d0: 7461 6461 7461 2873 656c 662c 2061 7474  tadata(self, att
+0000a7e0: 7269 6275 7465 7329 3a0a 2020 2020 2020  ributes):.      
+0000a7f0: 2020 2222 220a 2020 2020 2020 2020 4578    """.        Ex
+0000a800: 7472 6163 7420 6d65 7461 6461 7461 2066  tract metadata f
+0000a810: 726f 6d20 6174 7472 6962 7574 6520 6469  rom attribute di
+0000a820: 6374 696f 6e61 7279 0a20 2020 2020 2020  ctionary.       
+0000a830: 2022 2222 0a20 2020 2020 2020 200a 2020   """.        .  
+0000a840: 2020 2020 2020 6d65 7461 6461 7461 5f64        metadata_d
+0000a850: 6963 7420 3d20 6469 6374 2829 0a20 2020  ict = dict().   
+0000a860: 2020 2020 2066 6f72 206b 6579 2c76 616c       for key,val
+0000a870: 7565 2069 6e20 6174 7472 6962 7574 6573  ue in attributes
+0000a880: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+0000a890: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000a8a0: 6e63 6528 7661 6c75 652c 2062 7974 6573  nce(value, bytes
+0000a8b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000a8c0: 2020 2076 616c 7565 203d 2076 616c 7565     value = value
+0000a8d0: 2e64 6563 6f64 6528 290a 2020 2020 2020  .decode().      
+0000a8e0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+0000a8f0: 7461 6e63 6528 7661 6c75 652c 206e 702e  tance(value, np.
+0000a900: 6e64 6172 7261 7929 3a0a 2020 2020 2020  ndarray):.      
+0000a910: 2020 2020 2020 2020 2020 6966 2076 616c            if val
+0000a920: 7565 2e64 7479 7065 203d 3d20 6e70 2e6f  ue.dtype == np.o
+0000a930: 626a 6563 743a 0a20 2020 2020 2020 2020  bject:.         
+0000a940: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0000a950: 203d 2076 616c 7565 2e61 7374 7970 6528   = value.astype(
+0000a960: 7374 7229 0a20 2020 2020 2020 2020 2020  str).           
+0000a970: 2020 2020 2023 2061 2066 6577 2070 6172       # a few par
+0000a980: 7469 6375 6c61 7220 6361 7365 730a 2020  ticular cases.  
+0000a990: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000a9a0: 206b 6579 203d 3d20 2772 756e 5f70 7572   key == 'run_pur
+0000a9b0: 706f 7365 273a 0a20 2020 2020 2020 2020  pose':.         
+0000a9c0: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0000a9d0: 203d 2027 2027 2e6a 6f69 6e28 6c69 7374   = ' '.join(list
+0000a9e0: 2876 616c 7565 2929 2020 2020 2020 2020  (value))        
+0000a9f0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000aa00: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+0000aa10: 615f 6469 6374 5b6b 6579 5d20 3d20 7661  a_dict[key] = va
+0000aa20: 6c75 650a 2020 2020 2020 2020 7265 7475  lue.        retu
+0000aa30: 726e 206d 6574 6164 6174 615f 6469 6374  rn metadata_dict
+0000aa40: 0a20 2020 2020 2020 200a 2020 2020 0a20  .        .    . 
+0000aa50: 2020 2064 6566 205f 6c6f 6164 5f65 7665     def _load_eve
+0000aa60: 6e74 2873 656c 662c 2065 7665 6e74 5f69  nt(self, event_i
+0000aa70: 6e64 6578 2c0a 2020 2020 2020 2020 2020  ndex,.          
+0000aa80: 2020 2020 2020 2020 2020 7472 6967 6765            trigge
+0000aa90: 725f 696e 6465 783d 4e6f 6e65 2c0a 2020  r_index=None,.  
+0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aab0: 2020 7472 6163 655f 6c65 6e67 7468 5f6d    trace_length_m
+0000aac0: 7365 633d 4e6f 6e65 2c0a 2020 2020 2020  sec=None,.      
+0000aad0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0000aae0: 6163 655f 6c65 6e67 7468 5f73 616d 706c  ace_length_sampl
+0000aaf0: 6573 3d4e 6f6e 652c 0a20 2020 2020 2020  es=None,.       
+0000ab00: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+0000ab10: 7472 6967 6765 725f 6c65 6e67 7468 5f6d  trigger_length_m
+0000ab20: 7365 633d 4e6f 6e65 2c0a 2020 2020 2020  sec=None,.      
+0000ab30: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000ab40: 6574 7269 6767 6572 5f6c 656e 6774 685f  etrigger_length_
+0000ab50: 7361 6d70 6c65 733d 4e6f 6e65 2c0a 2020  samples=None,.  
+0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab70: 2020 6465 7465 6374 6f72 5f63 6861 6e73    detector_chans
+0000ab80: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0000ab90: 2020 2020 2020 2020 2020 2061 6463 746f             adcto
+0000aba0: 766f 6c74 3d46 616c 7365 2c20 6164 6374  volt=False, adct
+0000abb0: 6f61 6d70 3d46 616c 7365 2c0a 2020 2020  oamp=False,.    
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 6261 7365 6c69 6e65 7375 623d 4661 6c73  baselinesub=Fals
+0000abe0: 652c 2062 6173 656c 696e 6569 6e64 733d  e, baselineinds=
+0000abf0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000ac00: 2020 2020 2020 2020 2020 6164 635f 6e61            adc_na
+0000ac10: 6d65 3d27 6164 6331 2729 3a0a 2020 2020  me='adc1'):.    
+0000ac20: 2020 2020 0a20 2020 2020 2020 2022 2222      .        """
+0000ac30: 0a20 2020 2020 2020 204c 6f61 6420 7472  .        Load tr
+0000ac40: 6163 6573 2061 6e64 206d 6574 6164 6174  aces and metadat
+0000ac50: 6120 6672 6f6d 2063 7572 7265 6e74 2066  a from current f
+0000ac60: 696c 6520 2062 6173 6564 206f 6e0a 2020  ile  based on.  
+0000ac70: 2020 2020 2020 6576 656e 7420 696e 6465        event inde
+0000ac80: 780a 200a 2020 2020 2020 2020 5061 7261  x. .        Para
+0000ac90: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+0000aca0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+0000acb0: 2020 6576 656e 745f 696e 6465 7820 3a20    event_index : 
+0000acc0: 696e 740a 2020 2020 2020 2020 2020 6576  int.          ev
+0000acd0: 656e 7420 2868 6466 3520 2264 6174 6173  ent (hdf5 "datas
+0000ace0: 6574 2229 2020 6e75 6d62 6572 200a 2020  et")  number .  
+0000acf0: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
+0000ad00: 6574 6563 746f 725f 6368 616e 7320 3a20  etector_chans : 
+0000ad10: 7374 7220 6f72 206c 6973 742c 206f 7074  str or list, opt
+0000ad20: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000ad30: 6465 7465 6374 6f72 2f63 6861 6e6e 656c  detector/channel
+0000ad40: 206e 616d 6520 6f72 206c 6973 7420 6f66   name or list of
+0000ad50: 2064 6574 6563 746f 7273 2f63 6861 6e6e   detectors/chann
+0000ad60: 656c 730a 2020 2020 2020 2020 2020 6966  els.          if
+0000ad70: 204e 6f6e 652c 2067 6574 2061 6c6c 2063   None, get all c
+0000ad80: 6861 6e6e 656c 7320 2864 6566 6175 6c74  hannels (default
+0000ad90: 290a 0a20 2020 2020 2020 2061 6463 746f  )..        adcto
+0000ada0: 766f 6c74 203a 2062 6f6f 6c2c 206f 7074  volt : bool, opt
+0000adb0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000adc0: 636f 6e76 6572 7420 6672 6f6d 2041 4443  convert from ADC
+0000add0: 2074 6f20 766f 6c74 730a 2020 2020 2020   to volts.      
+0000ade0: 2020 2020 6465 6661 756c 743a 2046 616c      default: Fal
+0000adf0: 7365 0a0a 2020 2020 2020 2020 6164 6374  se..        adct
+0000ae00: 6f61 6d70 203a 2062 6f6f 6c2c 206f 7074  oamp : bool, opt
+0000ae10: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000ae20: 636f 6e76 6572 7420 6672 6f6d 2041 4443  convert from ADC
+0000ae30: 2074 6f20 6375 7272 656e 7420 616d 7073   to current amps
+0000ae40: 0a20 2020 2020 2020 2020 2064 6566 6175  .          defau
+0000ae50: 6c74 3a20 4661 6c73 650a 2020 2020 2020  lt: False.      
+0000ae60: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
+0000ae70: 200a 2020 2020 2020 2020 6261 7365 6c69   .        baseli
+0000ae80: 6e65 7375 623a 2062 6f6f 6c2c 206f 7074  nesub: bool, opt
+0000ae90: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0000aea0: 6966 2054 7275 652c 2073 7562 7472 6163  if True, subtrac
+0000aeb0: 7420 7072 652d 7075 6c73 6520 6261 7365  t pre-pulse base
+0000aec0: 6c69 6e65 0a20 2020 2020 2020 2020 2064  line.          d
+0000aed0: 6566 6175 6c74 3a20 4661 6c73 650a 0a20  efault: False.. 
+0000aee0: 2020 2020 2020 2062 6173 656c 696e 6569         baselinei
+0000aef0: 6e64 733a 2074 7570 6c65 2028 696e 742c  nds: tuple (int,
+0000af00: 2069 6e74 2920 6f72 206c 6973 7420 5b69   int) or list [i
+0000af10: 6e74 2c20 696e 745d 0a20 2020 2020 2020  nt, int].       
+0000af20: 2020 206d 696e 2f6d 6178 2069 6e64 6578     min/max index
+0000af30: 2066 6f72 2020 6261 7365 6c69 6e65 2063   for  baseline c
+0000af40: 616c 6375 6c61 7469 6f6e 200a 2020 2020  alculation .    
+0000af50: 2020 2020 2020 6465 6661 756c 743a 2028        default: (
+0000af60: 3130 2c20 302e 382a 7072 6574 7269 6767  10, 0.8*pretrigg
+0000af70: 6572 206c 656e 6774 6829 290a 2020 2020  er length)).    
+0000af80: 2020 2020 2020 0a20 2020 2020 2020 2061        .        a
+0000af90: 6463 5f6e 616d 6520 3a20 7374 722c 206f  dc_name : str, o
+0000afa0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000afb0: 2020 6e61 6d65 2f49 4420 6f66 2074 6865    name/ID of the
+0000afc0: 2061 6463 0a20 2020 2020 2020 2020 2064   adc.          d
+0000afd0: 6566 6175 6c74 3a20 2261 6463 3122 0a0a  efault: "adc1"..
+0000afe0: 2020 2020 2020 2020 5265 7475 726e 0a20          Return. 
+0000aff0: 2020 2020 2020 202d 2d2d 2d2d 2d0a 2020         ------.  
+0000b000: 2020 2020 2020 0a20 2020 2020 2020 2061        .        a
+0000b010: 7272 6179 203a 2032 4420 6e75 6d70 7920  rray : 2D numpy 
+0000b020: 6172 7261 790a 2020 2020 2020 2020 2020  array.          
+0000b030: 2074 7261 6365 7320 666f 7220 6561 6368   traces for each
+0000b040: 2063 6861 6e6e 656c 205b 6e62 2063 6861   channel [nb cha
+0000b050: 6e6e 656c 2c20 6e62 2073 616d 706c 6573  nnel, nb samples
+0000b060: 5d0a 0a20 2020 2020 2020 2069 6e66 6f20  ]..        info 
+0000b070: 3a20 6469 6374 0a20 2020 2020 2020 2020  : dict.         
+0000b080: 2020 6669 6c65 2f65 7665 6e74 2f64 6574    file/event/det
+0000b090: 6563 746f 7220 6d65 7461 6461 7461 2028  ector metadata (
+0000b0a0: 6966 2022 696e 636c 7564 655f 6d65 7461  if "include_meta
+0000b0b0: 6461 7461 2220 3d20 5472 7565 290a 0a0a  data" = True)...
+0000b0c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000b0d0: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
+0000b0e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b0f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b100: 3d3d 3d0a 2020 2020 2020 2020 2320 4765  ===.        # Ge
+0000b110: 7420 4844 4635 2064 6174 6173 6574 0a20  t HDF5 dataset. 
+0000b120: 2020 2020 2020 2023 203d 3d3d 3d3d 3d3d         # =======
+0000b130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b140: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020  ============..  
+0000b150: 2020 2020 2020 2320 6368 6563 6b20 6669        # check fi
+0000b160: 6c65 206f 7065 6e0a 2020 2020 2020 2020  le open.        
+0000b170: 6966 2073 656c 662e 5f63 7572 7265 6e74  if self._current
+0000b180: 5f66 696c 6520 6973 204e 6f6e 653a 0a20  _file is None:. 
+0000b190: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000b1a0: 2056 616c 7565 4572 726f 7228 274e 6f20   ValueError('No 
+0000b1b0: 6669 6c65 206f 7065 6e21 2729 0a0a 2020  file open!')..  
+0000b1c0: 2020 2020 2020 2320 6765 7420 6461 7461        # get data
+0000b1d0: 7365 740a 2020 2020 2020 2020 6461 7461  set.        data
+0000b1e0: 7365 745f 6e61 6d65 203d 2027 6576 656e  set_name = 'even
+0000b1f0: 745f 2720 2b20 7374 7228 6576 656e 745f  t_' + str(event_
+0000b200: 696e 6465 7829 0a20 2020 2020 2020 2064  index).        d
+0000b210: 6174 6173 6574 203d 2073 656c 662e 5f63  ataset = self._c
+0000b220: 7572 7265 6e74 5f66 696c 655b 6164 635f  urrent_file[adc_
+0000b230: 6e61 6d65 5d5b 6461 7461 7365 745f 6e61  name][dataset_na
+0000b240: 6d65 5d0a 2020 2020 2020 2020 6461 7461  me].        data
+0000b250: 7365 745f 6469 6d73 203d 2064 6174 6173  set_dims = datas
+0000b260: 6574 2e73 6861 7065 0a0a 2020 2020 2020  et.shape..      
+0000b270: 2020 2320 6765 7420 6461 7461 7365 7420    # get dataset 
+0000b280: 6d65 7461 6461 7461 0a20 2020 2020 2020  metadata.       
+0000b290: 2069 6e66 6f20 3d20 7365 6c66 2e5f 6578   info = self._ex
+0000b2a0: 7472 6163 745f 6d65 7461 6461 7461 2864  tract_metadata(d
+0000b2b0: 6174 6173 6574 2e61 7474 7273 290a 2020  ataset.attrs).  
+0000b2c0: 2020 2020 2020 696e 666f 2e75 7064 6174        info.updat
+0000b2d0: 6528 7365 6c66 2e5f 6578 7472 6163 745f  e(self._extract_
+0000b2e0: 6d65 7461 6461 7461 2873 656c 662e 5f63  metadata(self._c
+0000b2f0: 7572 7265 6e74 5f66 696c 652e 6174 7472  urrent_file.attr
+0000b300: 7329 290a 2020 2020 2020 2020 696e 666f  s)).        info
+0000b310: 2e75 7064 6174 6528 7365 6c66 2e5f 6578  .update(self._ex
+0000b320: 7472 6163 745f 6d65 7461 6461 7461 2873  tract_metadata(s
+0000b330: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+0000b340: 655b 6164 635f 6e61 6d65 5d2e 6174 7472  e[adc_name].attr
+0000b350: 7329 290a 2020 2020 2020 2020 696e 666f  s)).        info
+0000b360: 5b27 7265 6164 5f73 7461 7475 7327 5d20  ['read_status'] 
+0000b370: 3d20 300a 2020 2020 2020 2020 696e 666f  = 0.        info
+0000b380: 5b27 6572 726f 725f 6d73 6727 5d20 3d20  ['error_msg'] = 
+0000b390: 2727 0a20 2020 2020 2020 200a 2020 2020  ''.        .    
+0000b3a0: 2020 2020 0a20 2020 2020 2020 2023 203d      .        # =
+0000b3b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b3c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b3d0: 3d3d 0a20 2020 2020 2020 2023 2043 6861  ==.        # Cha
+0000b3e0: 6e6e 656c 2069 6e64 6963 6573 0a20 2020  nnel indices.   
+0000b3f0: 2020 2020 2023 203d 3d3d 3d3d 3d3d 3d3d       # =========
+0000b400: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b410: 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020  ==========..    
+0000b420: 2020 2020 2320 6578 7472 6163 7420 6c69      # extract li
+0000b430: 7374 206f 6620 6164 6320 6368 616e 6e65  st of adc channe
+0000b440: 6c73 2c20 696e 6465 7820 636f 7272 6573  ls, index corres
+0000b450: 706f 6e64 2074 6f20 6172 7261 7920 696e  pond to array in
+0000b460: 6465 7821 0a20 2020 2020 2020 2061 6463  dex!.        adc
+0000b470: 5f6e 756d 735f 6669 6c65 203d 2069 6e66  _nums_file = inf
+0000b480: 6f5b 2761 6463 5f63 6861 6e6e 656c 5f69  o['adc_channel_i
+0000b490: 6e64 6963 6573 275d 0a20 2020 2020 2020  ndices'].       
+0000b4a0: 2069 6620 286e 6f74 2069 7369 6e73 7461   if (not isinsta
+0000b4b0: 6e63 6528 6164 635f 6e75 6d73 5f66 696c  nce(adc_nums_fil
+0000b4c0: 652c 206c 6973 7429 0a20 2020 2020 2020  e, list).       
+0000b4d0: 2020 2020 2061 6e64 206e 6f74 2069 7369       and not isi
+0000b4e0: 6e73 7461 6e63 6528 6164 635f 6e75 6d73  nstance(adc_nums
+0000b4f0: 5f66 696c 652c 206e 702e 6e64 6172 7261  _file, np.ndarra
+0000b500: 7929 293a 0a20 2020 2020 2020 2020 2020  y)):.           
+0000b510: 2061 6463 5f6e 756d 735f 6669 6c65 203d   adc_nums_file =
+0000b520: 206e 702e 6172 7261 7928 5b61 6463 5f6e   np.array([adc_n
+0000b530: 756d 735f 6669 6c65 5d29 0a20 2020 2020  ums_file]).     
+0000b540: 2020 206e 625f 6368 616e 6e65 6c73 5f66     nb_channels_f
+0000b550: 696c 6520 3d20 6c65 6e28 6164 635f 6e75  ile = len(adc_nu
+0000b560: 6d73 5f66 696c 6529 0a0a 0a20 2020 2020  ms_file)...     
+0000b570: 2020 2023 2067 6574 2063 6f6e 6e65 6374     # get connect
+0000b580: 696f 6e20 6d61 7020 616e 6420 636f 6e76  ion map and conv
+0000b590: 6572 7420 746f 206e 756d 7079 2061 7272  ert to numpy arr
+0000b5a0: 6179 0a20 2020 2020 2020 2063 6f6e 6e65  ay.        conne
+0000b5b0: 6374 696f 6e73 203d 2073 656c 662e 6765  ctions = self.ge
+0000b5c0: 745f 636f 6e6e 6563 7469 6f6e 5f64 6963  t_connection_dic
+0000b5d0: 7428 6164 635f 6e61 6d65 3d61 6463 5f6e  t(adc_name=adc_n
+0000b5e0: 616d 652c 206d 6574 6164 6174 613d 696e  ame, metadata=in
+0000b5f0: 666f 290a 2020 2020 2020 2020 2020 2020  fo).            
+0000b600: 2020 0a20 2020 2020 2020 2023 2046 696c    .        # Fil
+0000b610: 7465 7220 6261 7365 6420 6f6e 2064 6574  ter based on det
+0000b620: 6563 746f 725f 6368 616e 7320 6172 6775  ector_chans argu
+0000b630: 6d65 6e74 0a20 2020 2020 2020 2073 656c  ment.        sel
+0000b640: 6563 7465 645f 6172 7261 795f 696e 6469  ected_array_indi
+0000b650: 6365 7320 3d20 6c69 7374 2829 0a20 2020  ces = list().   
+0000b660: 2020 2020 2073 656c 6563 7465 645f 6164       selected_ad
+0000b670: 635f 6e75 6d73 203d 206c 6973 7428 290a  c_nums = list().
+0000b680: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+0000b690: 5f64 6574 6563 746f 725f 6368 616e 7320  _detector_chans 
+0000b6a0: 3d20 6c69 7374 2829 0a20 2020 2020 2020  = list().       
+0000b6b0: 2073 656c 6563 7465 645f 7465 735f 6368   selected_tes_ch
+0000b6c0: 616e 7320 3d20 6c69 7374 2829 0a20 2020  ans = list().   
+0000b6d0: 2020 2020 2073 656c 6563 7465 645f 636f       selected_co
+0000b6e0: 6e74 726f 6c6c 6572 5f63 6861 6e73 203d  ntroller_chans =
+0000b6f0: 206c 6973 7428 290a 2020 2020 2020 2020   list().        
+0000b700: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0000b710: 2020 6966 2064 6574 6563 746f 725f 6368    if detector_ch
+0000b720: 616e 7320 6973 206e 6f74 204e 6f6e 653a  ans is not None:
+0000b730: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+0000b740: 2020 2020 2020 2020 2020 2320 636f 6e76            # conv
+0000b750: 6572 7420 6465 7465 6374 6f72 5f63 6861  ert detector_cha
+0000b760: 6e73 2074 6f20 6c69 7374 2069 6620 6e65  ns to list if ne
+0000b770: 6564 6564 0a20 2020 2020 2020 2020 2020  eded.           
+0000b780: 2069 6620 286e 6f74 2069 7369 6e73 7461   if (not isinsta
+0000b790: 6e63 6528 6465 7465 6374 6f72 5f63 6861  nce(detector_cha
+0000b7a0: 6e73 2c20 6c69 7374 290a 2020 2020 2020  ns, list).      
+0000b7b0: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+0000b7c0: 7420 6973 696e 7374 616e 6365 2864 6574  t isinstance(det
+0000b7d0: 6563 746f 725f 6368 616e 732c 206e 702e  ector_chans, np.
+0000b7e0: 6e64 6172 7261 7929 293a 0a20 2020 2020  ndarray)):.     
+0000b7f0: 2020 2020 2020 2020 2020 2064 6574 6563             detec
+0000b800: 746f 725f 6368 616e 7320 3d20 5b64 6574  tor_chans = [det
+0000b810: 6563 746f 725f 6368 616e 735d 0a20 2020  ector_chans].   
+0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b830: 2020 2020 2020 2020 200a 0a20 2020 2020           ..     
+0000b840: 2020 2020 2020 2023 206c 6f6f 7020 7365         # loop se
+0000b850: 6c65 6374 6564 2063 6861 6e6e 656c 730a  lected channels.
+0000b860: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000b870: 6368 616e 2069 6e20 6465 7465 6374 6f72  chan in detector
+0000b880: 5f63 6861 6e73 3a0a 0a20 2020 2020 2020  _chans:..       
+0000b890: 2020 2020 2020 2020 2023 2063 6865 636b           # check
+0000b8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b8b0: 2069 6620 6368 616e 206e 6f74 2069 6e20   if chan not in 
+0000b8c0: 636f 6e6e 6563 7469 6f6e 735b 2764 6574  connections['det
+0000b8d0: 6563 746f 725f 6368 616e 7327 5d3a 0a20  ector_chans']:. 
+0000b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8f0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000b900: 726f 7228 2744 6574 6563 746f 7220 6368  ror('Detector ch
+0000b910: 616e 6e65 6c20 2720 2b20 6368 616e 0a20  annel ' + chan. 
+0000b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b940: 7365 6c65 6374 6564 5f74 6573 5f63 6861  selected_tes_cha
-0000b950: 6e73 2e61 7070 656e 6428 636f 6e6e 6563  ns.append(connec
-0000b960: 7469 6f6e 735b 2774 6573 5f63 6861 6e73  tions['tes_chans
-0000b970: 275d 5b69 6e64 5d29 0a20 2020 2020 2020  '][ind]).       
-0000b980: 2020 2020 2020 2020 2069 6620 2763 6f6e           if 'con
-0000b990: 7472 6f6c 6c65 725f 6368 616e 7327 2069  troller_chans' i
-0000b9a0: 6e20 636f 6e6e 6563 7469 6f6e 733a 0a20  n connections:. 
-0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9c0: 2020 2073 656c 6563 7465 645f 636f 6e74     selected_cont
-0000b9d0: 726f 6c6c 6572 5f63 6861 6e73 2e61 7070  roller_chans.app
-0000b9e0: 656e 6428 636f 6e6e 6563 7469 6f6e 735b  end(connections[
-0000b9f0: 2763 6f6e 7472 6f6c 6c65 725f 6368 616e  'controller_chan
-0000ba00: 7327 5d5b 696e 645d 290a 0a20 2020 2020  s'][ind])..     
-0000ba10: 2020 2020 2020 2020 2020 2023 2073 6176             # sav
-0000ba20: 6520 6172 7261 7920 696e 6465 780a 2020  e array index.  
-0000ba30: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000ba40: 645f 6164 6320 3d20 696e 7428 6e70 2e77  d_adc = int(np.w
-0000ba50: 6865 7265 2861 6463 5f6e 756d 735f 6669  here(adc_nums_fi
-0000ba60: 6c65 3d3d 7365 6c65 6374 6564 5f61 6463  le==selected_adc
-0000ba70: 295b 305d 290a 2020 2020 2020 2020 2020  )[0]).          
-0000ba80: 2020 2020 2020 7365 6c65 6374 6564 5f61        selected_a
-0000ba90: 7272 6179 5f69 6e64 6963 6573 2e61 7070  rray_indices.app
-0000baa0: 656e 6428 696e 645f 6164 6329 2020 2020  end(ind_adc)    
-0000bab0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-0000bac0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-0000bad0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000bae0: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
-0000baf0: 5f61 7272 6179 5f69 6e64 6963 6573 203d  _array_indices =
-0000bb00: 206c 6973 7428 7261 6e67 6528 6e62 5f63   list(range(nb_c
-0000bb10: 6861 6e6e 656c 735f 6669 6c65 2929 0a20  hannels_file)). 
-0000bb20: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-0000bb30: 7465 645f 6164 635f 6e75 6d73 203d 206c  ted_adc_nums = l
-0000bb40: 6973 7428 6164 635f 6e75 6d73 5f66 696c  ist(adc_nums_fil
-0000bb50: 6529 0a20 2020 2020 2020 2020 2020 2066  e).            f
-0000bb60: 6f72 2061 6463 5f63 6861 6e20 696e 2073  or adc_chan in s
-0000bb70: 656c 6563 7465 645f 6164 635f 6e75 6d73  elected_adc_nums
-0000bb80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000bb90: 2020 696e 6420 3d20 636f 6e6e 6563 7469    ind = connecti
-0000bba0: 6f6e 735b 2761 6463 5f63 6861 6e73 275d  ons['adc_chans']
-0000bbb0: 2e69 6e64 6578 2861 6463 5f63 6861 6e29  .index(adc_chan)
-0000bbc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bbd0: 2073 656c 6563 7465 645f 6465 7465 6374   selected_detect
-0000bbe0: 6f72 5f63 6861 6e73 2e61 7070 656e 6428  or_chans.append(
-0000bbf0: 636f 6e6e 6563 7469 6f6e 735b 2764 6574  connections['det
-0000bc00: 6563 746f 725f 6368 616e 7327 5d5b 696e  ector_chans'][in
-0000bc10: 645d 290a 2020 2020 2020 2020 2020 2020  d]).            
-0000bc20: 2020 2020 6966 2027 7465 735f 6368 616e      if 'tes_chan
-0000bc30: 7327 2069 6e20 636f 6e6e 6563 7469 6f6e  s' in connection
-0000bc40: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000bc50: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
-0000bc60: 7465 735f 6368 616e 732e 6170 7065 6e64  tes_chans.append
-0000bc70: 2863 6f6e 6e65 6374 696f 6e73 5b27 7465  (connections['te
-0000bc80: 735f 6368 616e 7327 5d5b 696e 645d 290a  s_chans'][ind]).
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 6966 2027 636f 6e74 726f 6c6c 6572 5f63  if 'controller_c
-0000bcb0: 6861 6e73 2720 696e 2063 6f6e 6e65 6374  hans' in connect
-0000bcc0: 696f 6e73 3a0a 2020 2020 2020 2020 2020  ions:.          
-0000bcd0: 2020 2020 2020 2020 2020 7365 6c65 6374            select
-0000bce0: 6564 5f63 6f6e 7472 6f6c 6c65 725f 6368  ed_controller_ch
-0000bcf0: 616e 732e 6170 7065 6e64 280a 2020 2020  ans.append(.    
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd10: 2020 2020 636f 6e6e 6563 7469 6f6e 735b      connections[
-0000bd20: 2763 6f6e 7472 6f6c 6c65 725f 6368 616e  'controller_chan
-0000bd30: 7327 5d5b 696e 645d 0a20 2020 2020 2020  s'][ind].       
-0000bd40: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-0000bd50: 0a20 2020 2020 2020 2023 2063 6865 636b  .        # check
-0000bd60: 206e 756d 6265 7220 6368 616e 6e65 6c73   number channels
-0000bd70: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000bd80: 7365 6c65 6374 6564 5f61 7272 6179 5f69  selected_array_i
-0000bd90: 6e64 6963 6573 206f 7220 6c65 6e28 7365  ndices or len(se
-0000bda0: 6c65 6374 6564 5f61 7272 6179 5f69 6e64  lected_array_ind
-0000bdb0: 6963 6573 293d 3d30 3a0a 2020 2020 2020  ices)==0:.      
-0000bdc0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000bdd0: 6545 7272 6f72 2827 556e 6162 6c65 2074  eError('Unable t
-0000bde0: 6f20 6669 6e64 2073 656c 6563 7465 6420  o find selected 
-0000bdf0: 6368 616e 6e65 6c28 7329 2e20 4368 6563  channel(s). Chec
-0000be00: 6b20 636f 6e6e 6563 7469 6f6e 2074 6162  k connection tab
-0000be10: 6c65 2127 290a 0a20 2020 2020 2020 2023  le!')..        #
-0000be20: 2065 7874 7261 6374 2061 7272 6179 2066   extract array f
-0000be30: 6f72 2073 656c 6563 7465 6420 6368 616e  or selected chan
-0000be40: 6e65 6c73 0a20 2020 2020 2020 2074 7261  nels.        tra
-0000be50: 6365 735f 696e 7420 3d20 7472 6163 6573  ces_int = traces
-0000be60: 5f69 6e74 5b73 656c 6563 7465 645f 6172  _int[selected_ar
-0000be70: 7261 795f 696e 6469 6365 732c 3a5d 0a20  ray_indices,:]. 
-0000be80: 2020 2020 2020 2069 6e66 6f5b 2761 6463         info['adc
-0000be90: 5f63 6861 6e6e 656c 5f69 6e64 6963 6573  _channel_indices
-0000bea0: 275d 203d 2073 656c 6563 7465 645f 6164  '] = selected_ad
-0000beb0: 635f 6e75 6d73 0a20 2020 2020 2020 2069  c_nums.        i
-0000bec0: 6e66 6f5b 2761 6463 5f63 6861 6e73 275d  nfo['adc_chans']
-0000bed0: 203d 2073 656c 6563 7465 645f 6164 635f   = selected_adc_
-0000bee0: 6e75 6d73 0a20 2020 2020 2020 2069 6e66  nums.        inf
-0000bef0: 6f5b 2764 6574 6563 746f 725f 6368 616e  o['detector_chan
-0000bf00: 7327 5d20 3d20 7365 6c65 6374 6564 5f64  s'] = selected_d
-0000bf10: 6574 6563 746f 725f 6368 616e 730a 2020  etector_chans.  
-0000bf20: 2020 2020 2020 696e 666f 5b27 7465 735f        info['tes_
-0000bf30: 6368 616e 7327 5d20 3d20 7365 6c65 6374  chans'] = select
-0000bf40: 6564 5f74 6573 5f63 6861 6e73 0a20 2020  ed_tes_chans.   
-0000bf50: 2020 2020 2069 6e66 6f5b 2763 6f6e 7472       info['contr
-0000bf60: 6f6c 6c65 725f 6368 616e 7327 5d20 3d20  oller_chans'] = 
-0000bf70: 7365 6c65 6374 6564 5f63 6f6e 7472 6f6c  selected_control
-0000bf80: 6c65 725f 6368 616e 730a 2020 2020 2020  ler_chans.      
-0000bf90: 2020 696e 666f 5b27 6164 635f 636f 6e76    info['adc_conv
-0000bfa0: 6572 7369 6f6e 5f66 6163 746f 7227 5d20  ersion_factor'] 
-0000bfb0: 3d20 2069 6e66 6f5b 2761 6463 5f63 6f6e  =  info['adc_con
-0000bfc0: 7665 7273 696f 6e5f 6661 6374 6f72 275d  version_factor']
-0000bfd0: 5b73 656c 6563 7465 645f 6172 7261 795f  [selected_array_
-0000bfe0: 696e 6469 6365 732c 3a5d 0a20 2020 2020  indices,:].     
-0000bff0: 2020 2069 6e66 6f5b 2776 6f6c 7461 6765     info['voltage
-0000c000: 5f72 616e 6765 275d 203d 2069 6e66 6f5b  _range'] = info[
-0000c010: 2776 6f6c 7461 6765 5f72 616e 6765 275d  'voltage_range']
-0000c020: 5b73 656c 6563 7465 645f 6172 7261 795f  [selected_array_
-0000c030: 696e 6469 6365 732c 3a5d 0a0a 0a20 2020  indices,:]...   
-0000c040: 2020 2020 2023 2067 6574 2064 6574 6563       # get detec
-0000c050: 746f 7220 636f 6e66 6967 0a20 2020 2020  tor config.     
-0000c060: 2020 2064 6574 6563 746f 725f 636f 6e66     detector_conf
-0000c070: 6967 203d 2073 656c 662e 6765 745f 6465  ig = self.get_de
-0000c080: 7465 6374 6f72 5f63 6f6e 6669 6728 290a  tector_config().
-0000c090: 2020 2020 2020 2020 696e 666f 5b27 6465          info['de
-0000c0a0: 7465 6374 6f72 5f63 6f6e 6669 6727 5d20  tector_config'] 
-0000c0b0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0000c0c0: 2066 6f72 2064 6574 2069 6e20 696e 666f   for det in info
-0000c0d0: 5b27 6465 7465 6374 6f72 5f63 6861 6e73  ['detector_chans
-0000c0e0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-0000c0f0: 696e 666f 5b27 6465 7465 6374 6f72 5f63  info['detector_c
-0000c100: 6f6e 6669 6727 5d5b 6465 745d 203d 2064  onfig'][det] = d
-0000c110: 6574 6563 746f 725f 636f 6e66 6967 5b64  etector_config[d
-0000c120: 6574 5d0a 2020 2020 2020 2020 0a20 2020  et].        .   
-0000c130: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-0000c140: 636f 6e76 6572 7420 746f 2076 6f6c 742f  convert to volt/
-0000c150: 616d 7073 0a20 2020 2020 2020 2074 7261  amps.        tra
-0000c160: 6365 7320 3d20 5b5d 0a20 2020 2020 2020  ces = [].       
-0000c170: 2069 6620 6164 6374 6f76 6f6c 7420 6f72   if adctovolt or
-0000c180: 2061 6463 746f 616d 703a 0a0a 2020 2020   adctoamp:..    
-0000c190: 2020 2020 2020 2020 2320 696e 6974 6961          # initia
-0000c1a0: 6c69 7a65 0a20 2020 2020 2020 2020 2020  lize.           
-0000c1b0: 2074 7261 6365 7320 3d20 6e70 2e7a 6572   traces = np.zer
-0000c1c0: 6f73 5f6c 696b 6528 7472 6163 6573 5f69  os_like(traces_i
-0000c1d0: 6e74 2c20 6474 7970 653d 6e70 2e66 6c6f  nt, dtype=np.flo
-0000c1e0: 6174 3634 290a 0a20 2020 2020 2020 2020  at64)..         
-0000c1f0: 2020 2023 2063 6f6e 7665 7274 2074 6f20     # convert to 
-0000c200: 766f 6c74 730a 2020 2020 2020 2020 2020  volts.          
-0000c210: 2020 666f 7220 6963 6861 6e20 696e 2072    for ichan in r
-0000c220: 616e 6765 2874 7261 6365 735f 696e 742e  ange(traces_int.
-0000c230: 7368 6170 655b 305d 293a 0a20 2020 2020  shape[0]):.     
-0000c240: 2020 2020 2020 2020 2020 2063 616c 5f63             cal_c
-0000c250: 6f65 6666 203d 2069 6e66 6f5b 2761 6463  oeff = info['adc
-0000c260: 5f63 6f6e 7665 7273 696f 6e5f 6661 6374  _conversion_fact
-0000c270: 6f72 275d 5b69 6368 616e 5d5b 3a3a 2d31  or'][ichan][::-1
-0000c280: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000c290: 2020 706f 6c79 203d 206e 702e 706f 6c79    poly = np.poly
-0000c2a0: 3164 2863 616c 5f63 6f65 6666 290a 2020  1d(cal_coeff).  
-0000c2b0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000c2c0: 6163 6573 5b69 6368 616e 2c3a 5d20 3d20  aces[ichan,:] = 
-0000c2d0: 706f 6c79 2874 7261 6365 735f 696e 745b  poly(traces_int[
-0000c2e0: 6963 6861 6e2c 3a5d 290a 0a20 2020 2020  ichan,:])..     
-0000c2f0: 2020 2020 2020 2023 2063 6f6e 7665 7274         # convert
-0000c300: 2074 6f20 616d 7073 0a20 2020 2020 2020   to amps.       
-0000c310: 2020 2020 2069 6620 6164 6374 6f61 6d70       if adctoamp
-0000c320: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c330: 2020 6966 2064 6574 6563 746f 725f 636f    if detector_co
-0000c340: 6e66 6967 2069 7320 4e6f 6e65 3a0a 2020  nfig is None:.  
-0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c360: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000c370: 6f72 2827 4552 524f 523a 2055 6e61 626c  or('ERROR: Unabl
-0000c380: 6520 746f 2063 6f6e 7665 7274 2074 6f20  e to convert to 
-0000c390: 616d 7073 2e20 270a 2020 2020 2020 2020  amps. '.        
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3b0: 2020 2020 2020 2020 2020 2020 202b 2027               + '
-0000c3c0: 4e6f 2064 6574 6563 746f 7220 636f 6e66  No detector conf
-0000c3d0: 6967 2061 7661 696c 6162 6c65 2127 290a  ig available!').
-0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3f0: 666f 7220 6963 6861 6e20 696e 2072 616e  for ichan in ran
-0000c400: 6765 2874 7261 6365 732e 7368 6170 655b  ge(traces.shape[
-0000c410: 305d 293a 0a20 2020 2020 2020 2020 2020  0]):.           
-0000c420: 2020 2020 2020 2020 2064 6574 203d 2069           det = i
-0000c430: 6e66 6f5b 2764 6574 6563 746f 725f 6368  nfo['detector_ch
-0000c440: 616e 7327 5d5b 6963 6861 6e5d 0a20 2020  ans'][ichan].   
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2069 6620 2763 6c6f 7365 5f6c 6f6f 705f   if 'close_loop_
-0000c470: 6e6f 726d 2720 696e 2064 6574 6563 746f  norm' in detecto
-0000c480: 725f 636f 6e66 6967 5b64 6574 5d3a 0a20  r_config[det]:. 
-0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4a0: 2020 2020 2020 2074 7261 6365 735b 6963         traces[ic
-0000c4b0: 6861 6e2c 3a5d 203d 2074 7261 6365 735b  han,:] = traces[
-0000c4c0: 6963 6861 6e2c 3a5d 2f64 6574 6563 746f  ichan,:]/detecto
-0000c4d0: 725f 636f 6e66 6967 5b64 6574 5d5b 2763  r_config[det]['c
-0000c4e0: 6c6f 7365 5f6c 6f6f 705f 6e6f 726d 275d  lose_loop_norm']
-0000c4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c500: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c520: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000c530: 726f 7228 2745 5252 4f52 3a20 556e 6162  ror('ERROR: Unab
-0000c540: 6c65 2074 6f20 636f 6e76 6572 7420 746f  le to convert to
-0000c550: 2061 6d70 732e 2027 0a20 2020 2020 2020   amps. '.       
-0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b940: 2020 2020 2b20 2720 6e6f 7420 6176 6169      + ' not avai
+0000b950: 6c61 626c 6520 696e 2072 6177 2064 6174  lable in raw dat
+0000b960: 612e 270a 2020 2020 2020 2020 2020 2020  a.'.            
+0000b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b980: 2020 2020 2020 2020 202b 2027 2043 6865           + ' Che
+0000b990: 636b 2063 6f6e 6e65 6374 696f 6e20 6d61  ck connection ma
+0000b9a0: 7021 2729 0a20 2020 2020 2020 2020 2020  p!').           
+0000b9b0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+0000b9c0: 2020 2020 2020 2320 6669 6e64 2063 6861        # find cha
+0000b9d0: 6e6e 656c 2069 6e64 6578 2069 6e20 636f  nnel index in co
+0000b9e0: 6e6e 6563 7469 6f6e 206d 6170 0a20 2020  nnection map.   
+0000b9f0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+0000ba00: 203d 2063 6f6e 6e65 6374 696f 6e73 5b27   = connections['
+0000ba10: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
+0000ba20: 2e69 6e64 6578 2863 6861 6e29 0a0a 2020  .index(chan)..  
+0000ba30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000ba40: 6578 7472 6163 7420 7365 6c65 6374 6564  extract selected
+0000ba50: 2041 4443 206e 756d 6265 720a 2020 2020   ADC number.    
+0000ba60: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
+0000ba70: 6374 6564 5f61 6463 203d 2069 6e74 2863  cted_adc = int(c
+0000ba80: 6f6e 6e65 6374 696f 6e73 5b27 6164 635f  onnections['adc_
+0000ba90: 6368 616e 7327 5d5b 696e 645d 290a 2020  chans'][ind]).  
+0000baa0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000bab0: 2073 656c 6563 7465 645f 6164 6320 6e6f   selected_adc no
+0000bac0: 7420 696e 2061 6463 5f6e 756d 735f 6669  t in adc_nums_fi
+0000bad0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+0000bae0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0000baf0: 6c75 6545 7272 6f72 2827 5072 6f62 6c65  lueError('Proble
+0000bb00: 6d20 7769 7468 2072 6177 2064 6174 612e  m with raw data.
+0000bb10: 2055 6e61 626c 6520 746f 2066 696e 6420   Unable to find 
+0000bb20: 4144 4320 6368 616e 6e65 6c27 290a 2020  ADC channel').  
+0000bb30: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
+0000bb40: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000bb50: 2073 6176 6520 636f 6e6e 6563 7469 6f6e   save connection
+0000bb60: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000bb70: 2020 7365 6c65 6374 6564 5f61 6463 5f6e    selected_adc_n
+0000bb80: 756d 732e 6170 7065 6e64 2873 656c 6563  ums.append(selec
+0000bb90: 7465 645f 6164 6329 0a20 2020 2020 2020  ted_adc).       
+0000bba0: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
+0000bbb0: 645f 6465 7465 6374 6f72 5f63 6861 6e73  d_detector_chans
+0000bbc0: 2e61 7070 656e 6428 636f 6e6e 6563 7469  .append(connecti
+0000bbd0: 6f6e 735b 2764 6574 6563 746f 725f 6368  ons['detector_ch
+0000bbe0: 616e 7327 5d5b 696e 645d 290a 2020 2020  ans'][ind]).    
+0000bbf0: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+0000bc00: 7465 735f 6368 616e 7327 2069 6e20 636f  tes_chans' in co
+0000bc10: 6e6e 6563 7469 6f6e 733a 0a20 2020 2020  nnections:.     
+0000bc20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000bc30: 656c 6563 7465 645f 7465 735f 6368 616e  elected_tes_chan
+0000bc40: 732e 6170 7065 6e64 2863 6f6e 6e65 6374  s.append(connect
+0000bc50: 696f 6e73 5b27 7465 735f 6368 616e 7327  ions['tes_chans'
+0000bc60: 5d5b 696e 645d 290a 2020 2020 2020 2020  ][ind]).        
+0000bc70: 2020 2020 2020 2020 6966 2027 636f 6e74          if 'cont
+0000bc80: 726f 6c6c 6572 5f63 6861 6e73 2720 696e  roller_chans' in
+0000bc90: 2063 6f6e 6e65 6374 696f 6e73 3a0a 2020   connections:.  
+0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcb0: 2020 7365 6c65 6374 6564 5f63 6f6e 7472    selected_contr
+0000bcc0: 6f6c 6c65 725f 6368 616e 732e 6170 7065  oller_chans.appe
+0000bcd0: 6e64 2863 6f6e 6e65 6374 696f 6e73 5b27  nd(connections['
+0000bce0: 636f 6e74 726f 6c6c 6572 5f63 6861 6e73  controller_chans
+0000bcf0: 275d 5b69 6e64 5d29 0a0a 2020 2020 2020  '][ind])..      
+0000bd00: 2020 2020 2020 2020 2020 2320 7361 7665            # save
+0000bd10: 2061 7272 6179 2069 6e64 6578 0a20 2020   array index.   
+0000bd20: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+0000bd30: 5f61 6463 203d 2069 6e74 286e 702e 7768  _adc = int(np.wh
+0000bd40: 6572 6528 6164 635f 6e75 6d73 5f66 696c  ere(adc_nums_fil
+0000bd50: 653d 3d73 656c 6563 7465 645f 6164 6329  e==selected_adc)
+0000bd60: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0000bd70: 2020 2020 2073 656c 6563 7465 645f 6172       selected_ar
+0000bd80: 7261 795f 696e 6469 6365 732e 6170 7065  ray_indices.appe
+0000bd90: 6e64 2869 6e64 5f61 6463 2920 2020 2020  nd(ind_adc)     
+0000bda0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0000bdb0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000bdc0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000bdd0: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
+0000bde0: 6172 7261 795f 696e 6469 6365 7320 3d20  array_indices = 
+0000bdf0: 6c69 7374 2872 616e 6765 286e 625f 6368  list(range(nb_ch
+0000be00: 616e 6e65 6c73 5f66 696c 6529 290a 2020  annels_file)).  
+0000be10: 2020 2020 2020 2020 2020 7365 6c65 6374            select
+0000be20: 6564 5f61 6463 5f6e 756d 7320 3d20 6c69  ed_adc_nums = li
+0000be30: 7374 2861 6463 5f6e 756d 735f 6669 6c65  st(adc_nums_file
+0000be40: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000be50: 7220 6164 635f 6368 616e 2069 6e20 7365  r adc_chan in se
+0000be60: 6c65 6374 6564 5f61 6463 5f6e 756d 733a  lected_adc_nums:
+0000be70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000be80: 2069 6e64 203d 2063 6f6e 6e65 6374 696f   ind = connectio
+0000be90: 6e73 5b27 6164 635f 6368 616e 7327 5d2e  ns['adc_chans'].
+0000bea0: 696e 6465 7828 6164 635f 6368 616e 290a  index(adc_chan).
+0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bec0: 7365 6c65 6374 6564 5f64 6574 6563 746f  selected_detecto
+0000bed0: 725f 6368 616e 732e 6170 7065 6e64 2863  r_chans.append(c
+0000bee0: 6f6e 6e65 6374 696f 6e73 5b27 6465 7465  onnections['dete
+0000bef0: 6374 6f72 5f63 6861 6e73 275d 5b69 6e64  ctor_chans'][ind
+0000bf00: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000bf10: 2020 2069 6620 2774 6573 5f63 6861 6e73     if 'tes_chans
+0000bf20: 2720 696e 2063 6f6e 6e65 6374 696f 6e73  ' in connections
+0000bf30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bf40: 2020 2020 2020 7365 6c65 6374 6564 5f74        selected_t
+0000bf50: 6573 5f63 6861 6e73 2e61 7070 656e 6428  es_chans.append(
+0000bf60: 636f 6e6e 6563 7469 6f6e 735b 2774 6573  connections['tes
+0000bf70: 5f63 6861 6e73 275d 5b69 6e64 5d29 0a20  _chans'][ind]). 
+0000bf80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000bf90: 6620 2763 6f6e 7472 6f6c 6c65 725f 6368  f 'controller_ch
+0000bfa0: 616e 7327 2069 6e20 636f 6e6e 6563 7469  ans' in connecti
+0000bfb0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+0000bfc0: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
+0000bfd0: 645f 636f 6e74 726f 6c6c 6572 5f63 6861  d_controller_cha
+0000bfe0: 6e73 2e61 7070 656e 6428 0a20 2020 2020  ns.append(.     
+0000bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c000: 2020 2063 6f6e 6e65 6374 696f 6e73 5b27     connections['
+0000c010: 636f 6e74 726f 6c6c 6572 5f63 6861 6e73  controller_chans
+0000c020: 275d 5b69 6e64 5d0a 2020 2020 2020 2020  '][ind].        
+0000c030: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000c040: 2020 2020 2020 2023 2063 6865 636b 206e         # check n
+0000c050: 756d 6265 7220 6368 616e 6e65 6c73 0a20  umber channels. 
+0000c060: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000c070: 6c65 6374 6564 5f61 7272 6179 5f69 6e64  lected_array_ind
+0000c080: 6963 6573 206f 7220 6c65 6e28 7365 6c65  ices or len(sele
+0000c090: 6374 6564 5f61 7272 6179 5f69 6e64 6963  cted_array_indic
+0000c0a0: 6573 293d 3d30 3a0a 2020 2020 2020 2020  es)==0:.        
+0000c0b0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000c0c0: 7272 6f72 2827 556e 6162 6c65 2074 6f20  rror('Unable to 
+0000c0d0: 6669 6e64 2073 656c 6563 7465 6420 6368  find selected ch
+0000c0e0: 616e 6e65 6c28 7329 2e20 4368 6563 6b20  annel(s). Check 
+0000c0f0: 636f 6e6e 6563 7469 6f6e 2074 6162 6c65  connection table
+0000c100: 2127 290a 0a20 2020 2020 2020 2023 2073  !')..        # s
+0000c110: 746f 7265 2069 6e66 6f0a 2020 2020 2020  tore info.      
+0000c120: 2020 696e 666f 5b27 6164 635f 6368 616e    info['adc_chan
+0000c130: 6e65 6c5f 696e 6469 6365 7327 5d20 3d20  nel_indices'] = 
+0000c140: 7365 6c65 6374 6564 5f61 6463 5f6e 756d  selected_adc_num
+0000c150: 730a 2020 2020 2020 2020 696e 666f 5b27  s.        info['
+0000c160: 6164 635f 6368 616e 7327 5d20 3d20 7365  adc_chans'] = se
+0000c170: 6c65 6374 6564 5f61 6463 5f6e 756d 730a  lected_adc_nums.
+0000c180: 2020 2020 2020 2020 696e 666f 5b27 6465          info['de
+0000c190: 7465 6374 6f72 5f63 6861 6e73 275d 203d  tector_chans'] =
+0000c1a0: 2073 656c 6563 7465 645f 6465 7465 6374   selected_detect
+0000c1b0: 6f72 5f63 6861 6e73 0a20 2020 2020 2020  or_chans.       
+0000c1c0: 2069 6e66 6f5b 2774 6573 5f63 6861 6e73   info['tes_chans
+0000c1d0: 275d 203d 2073 656c 6563 7465 645f 7465  '] = selected_te
+0000c1e0: 735f 6368 616e 730a 2020 2020 2020 2020  s_chans.        
+0000c1f0: 696e 666f 5b27 636f 6e74 726f 6c6c 6572  info['controller
+0000c200: 5f63 6861 6e73 275d 203d 2073 656c 6563  _chans'] = selec
+0000c210: 7465 645f 636f 6e74 726f 6c6c 6572 5f63  ted_controller_c
+0000c220: 6861 6e73 0a20 2020 2020 2020 2069 6e66  hans.        inf
+0000c230: 6f5b 2761 6463 5f63 6f6e 7665 7273 696f  o['adc_conversio
+0000c240: 6e5f 6661 6374 6f72 275d 203d 2020 696e  n_factor'] =  in
+0000c250: 666f 5b27 6164 635f 636f 6e76 6572 7369  fo['adc_conversi
+0000c260: 6f6e 5f66 6163 746f 7227 5d5b 7365 6c65  on_factor'][sele
+0000c270: 6374 6564 5f61 7272 6179 5f69 6e64 6963  cted_array_indic
+0000c280: 6573 2c3a 5d0a 2020 2020 2020 2020 696e  es,:].        in
+0000c290: 666f 5b27 766f 6c74 6167 655f 7261 6e67  fo['voltage_rang
+0000c2a0: 6527 5d20 3d20 696e 666f 5b27 766f 6c74  e'] = info['volt
+0000c2b0: 6167 655f 7261 6e67 6527 5d5b 7365 6c65  age_range'][sele
+0000c2c0: 6374 6564 5f61 7272 6179 5f69 6e64 6963  cted_array_indic
+0000c2d0: 6573 2c3a 5d0a 0a20 2020 2020 2020 2023  es,:]..        #
+0000c2e0: 2067 6574 2064 6574 6563 746f 7220 636f   get detector co
+0000c2f0: 6e66 6967 0a20 2020 2020 2020 2064 6574  nfig.        det
+0000c300: 6563 746f 725f 636f 6e66 6967 203d 2073  ector_config = s
+0000c310: 656c 662e 6765 745f 6465 7465 6374 6f72  elf.get_detector
+0000c320: 5f63 6f6e 6669 6728 290a 2020 2020 2020  _config().      
+0000c330: 2020 696e 666f 5b27 6465 7465 6374 6f72    info['detector
+0000c340: 5f63 6f6e 6669 6727 5d20 3d20 6469 6374  _config'] = dict
+0000c350: 2829 0a20 2020 2020 2020 2066 6f72 2064  ().        for d
+0000c360: 6574 2069 6e20 696e 666f 5b27 6465 7465  et in info['dete
+0000c370: 6374 6f72 5f63 6861 6e73 275d 3a0a 2020  ctor_chans']:.  
+0000c380: 2020 2020 2020 2020 2020 696e 666f 5b27            info['
+0000c390: 6465 7465 6374 6f72 5f63 6f6e 6669 6727  detector_config'
+0000c3a0: 5d5b 6465 745d 203d 2064 6574 6563 746f  ][det] = detecto
+0000c3b0: 725f 636f 6e66 6967 5b64 6574 5d0a 0a0a  r_config[det]...
+0000c3c0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000c3d0: 2020 2020 2023 203d 3d3d 3d3d 3d3d 3d3d       # =========
+0000c3e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c3f0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2020  ==========.     
+0000c400: 2020 2023 2054 7269 6767 6572 2069 6e64     # Trigger ind
+0000c410: 6963 6573 0a20 2020 2020 2020 2023 203d  ices.        # =
+0000c420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c440: 3d3d 0a20 2020 2020 2020 200a 2020 2020  ==.        .    
+0000c450: 2020 2020 7472 6163 655f 6d69 6e5f 696e      trace_min_in
+0000c460: 6465 7820 3d20 4e6f 6e65 0a20 2020 2020  dex = None.     
+0000c470: 2020 2074 7261 6365 5f6d 6178 5f69 6e64     trace_max_ind
+0000c480: 6578 203d 204e 6f6e 650a 0a20 2020 2020  ex = None..     
+0000c490: 2020 2023 2063 6865 636b 2074 7269 6767     # check trigg
+0000c4a0: 6572 2069 6e64 6578 0a20 2020 2020 2020  er index.       
+0000c4b0: 2069 6620 7472 6967 6765 725f 696e 6465   if trigger_inde
+0000c4c0: 7820 6973 206e 6f74 204e 6f6e 653a 0a20  x is not None:. 
+0000c4d0: 2020 2020 2020 2020 2020 2069 6620 2874             if (t
+0000c4e0: 7261 6365 5f6c 656e 6774 685f 6d73 6563  race_length_msec
+0000c4f0: 2069 7320 4e6f 6e65 200a 2020 2020 2020   is None .      
+0000c500: 2020 2020 2020 2020 2020 616e 6420 7472            and tr
+0000c510: 6163 655f 6c65 6e67 7468 5f73 616d 706c  ace_length_sampl
+0000c520: 6573 2069 7320 4e6f 6e65 293a 0a20 2020  es is None):.   
+0000c530: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+0000c540: 6e74 2827 5741 524e 494e 473a 2055 6e61  nt('WARNING: Una
+0000c550: 626c 6520 746f 2065 7874 7261 6374 2074  ble to extract t
+0000c560: 7261 6365 2062 6173 6564 206f 6e20 270a  race based on '.
 0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c580: 2020 2b20 274e 6f20 6e6f 726d 616c 697a    + 'No normaliz
-0000c590: 6174 696f 6e20 6176 6169 6c61 626c 6520  ation available 
-0000c5a0: 666f 7220 2720 2b20 6465 7429 2020 2020  for ' + det)    
-0000c5b0: 2020 0a20 2020 2020 2020 2065 6c73 653a    .        else:
-0000c5c0: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-0000c5d0: 6365 7320 3d20 7472 6163 6573 5f69 6e74  ces = traces_int
-0000c5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c5f0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-0000c600: 2020 0a20 2020 2020 2020 2023 2062 6173    .        # bas
-0000c610: 656c 696e 6520 7375 6274 7261 6374 0a20  eline subtract. 
-0000c620: 2020 2020 2020 2069 6620 6261 7365 6c69         if baseli
-0000c630: 6e65 7375 623a 0a20 2020 2020 2020 2020  nesub:.         
-0000c640: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-0000c650: 2320 6669 6e64 2062 6173 656c 696e 6520  # find baseline 
-0000c660: 7374 6172 742f 7374 6f70 0a20 2020 2020  start/stop.     
-0000c670: 2020 2020 2020 2062 6173 656c 696e 655f         baseline_
-0000c680: 7374 6172 7420 3d20 4e6f 6e65 0a20 2020  start = None.   
-0000c690: 2020 2020 2020 2020 2062 6173 656c 696e           baselin
-0000c6a0: 655f 7374 6f70 203d 204e 6f6e 650a 2020  e_stop = None.  
-0000c6b0: 2020 2020 2020 2020 2020 6966 2062 6173            if bas
-0000c6c0: 656c 696e 6569 6e64 7320 6973 206e 6f74  elineinds is not
-0000c6d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000c6e0: 2020 2020 2020 2069 6620 6c65 6e28 6261         if len(ba
-0000c6f0: 7365 6c69 6e65 696e 6473 2921 3d32 3a0a  selineinds)!=2:.
-0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c710: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000c720: 7272 6f72 2827 4552 524f 523a 2062 6173  rror('ERROR: bas
-0000c730: 656c 696e 6569 6e64 7320 7368 6f75 6c64  elineinds should
-0000c740: 2062 6520 6c69 7374 2f74 7570 6c65 206f   be list/tuple o
-0000c750: 6620 6c65 6e67 7468 2032 2729 0a20 2020  f length 2').   
-0000c760: 2020 2020 2020 2020 2020 2020 2062 6173               bas
-0000c770: 656c 696e 655f 7374 6172 7420 3d20 6261  eline_start = ba
-0000c780: 7365 6c69 6e65 696e 6473 5b30 5d0a 2020  selineinds[0].  
-0000c790: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-0000c7a0: 7365 6c69 6e65 5f73 746f 7020 3d20 2062  seline_stop =  b
-0000c7b0: 6173 656c 696e 6569 6e64 735b 315d 0a20  aselineinds[1]. 
-0000c7c0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-0000c7d0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000c7e0: 2027 6e62 5f73 616d 706c 6573 5f70 7265   'nb_samples_pre
-0000c7f0: 7472 6967 6765 7227 2069 6e20 696e 666f  trigger' in info
-0000c800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c810: 2020 6261 7365 6c69 6e65 5f73 7461 7274    baseline_start
-0000c820: 203d 2031 300a 2020 2020 2020 2020 2020   = 10.          
-0000c830: 2020 2020 2020 6261 7365 6c69 6e65 5f73        baseline_s
-0000c840: 746f 7020 3d20 696e 7428 726f 756e 6428  top = int(round(
-0000c850: 696e 666f 5b27 6e62 5f73 616d 706c 6573  info['nb_samples
-0000c860: 5f70 7265 7472 6967 6765 7227 5d2a 302e  _pretrigger']*0.
-0000c870: 3829 290a 0a20 2020 2020 2020 2020 2020  8))..           
-0000c880: 2069 6620 2862 6173 656c 696e 655f 7374   if (baseline_st
-0000c890: 6172 7420 6973 204e 6f6e 6520 6f72 2062  art is None or b
-0000c8a0: 6173 656c 696e 655f 7374 6f70 2069 7320  aseline_stop is 
-0000c8b0: 4e6f 6e65 206f 720a 2020 2020 2020 2020  None or.        
-0000c8c0: 2020 2020 2020 2020 6261 7365 6c69 6e65          baseline
-0000c8d0: 5f73 746f 703c 3d62 6173 656c 696e 655f  _stop<=baseline_
-0000c8e0: 7374 6172 7420 6f72 2062 6173 656c 696e  start or baselin
-0000c8f0: 655f 7374 6f70 3e3d 7472 6163 6573 2e73  e_stop>=traces.s
-0000c900: 6861 7065 5b31 5d29 3a0a 2020 2020 2020  hape[1]):.      
-0000c910: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000c920: 5661 6c75 6545 7272 6f72 2827 4552 524f  ValueError('ERRO
-0000c930: 523a 2055 6e61 626c 6520 746f 2066 696e  R: Unable to fin
-0000c940: 6420 6261 7365 6c69 6e65 2073 7461 7274  d baseline start
-0000c950: 2f73 746f 702e 2027 0a20 2020 2020 2020  /stop. '.       
-0000c960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c970: 2020 2020 2020 2020 2020 2b20 2741 6464            + 'Add
-0000c980: 2061 7267 756d 656e 7420 2262 6173 656c   argument "basel
-0000c990: 696e 6569 6e64 7322 2729 0a0a 2020 2020  ineinds"')..    
-0000c9a0: 2020 2020 2020 2020 7472 6163 6573 203d          traces =
-0000c9b0: 2074 7261 6365 7320 2d20 6e70 2e6d 6561   traces - np.mea
-0000c9c0: 6e28 7472 6163 6573 5b3a 2c62 6173 656c  n(traces[:,basel
-0000c9d0: 696e 655f 7374 6172 743a 6261 7365 6c69  ine_start:baseli
-0000c9e0: 6e65 5f73 746f 705d 2c0a 2020 2020 2020  ne_stop],.      
-0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca10: 6178 6973 3d2d 312c 206b 6565 7064 696d  axis=-1, keepdim
-0000ca20: 733d 5472 7565 290a 2020 2020 2020 2020  s=True).        
-0000ca30: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
-0000ca40: 2020 2020 2020 7265 7475 726e 2074 7261        return tra
-0000ca50: 6365 732c 2069 6e66 6f0a 2020 2020 2020  ces, info.      
-0000ca60: 2020 0a0a 0a20 2020 2020 2020 200a 2020    ...        .  
-0000ca70: 2020 0a20 2020 2020 2020 200a 0a0a 0a0a    .        .....
-0000ca80: 0a0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caa0: 200a 0a0a 2020 2020 0a63 6c61 7373 2048   ...    .class H
-0000cab0: 3557 7269 7465 723a 0a20 2020 200a 2020  5Writer:.    .  
-0000cac0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000cad0: 656c 662c 2072 6169 7365 5f65 7272 6f72  elf, raise_error
-0000cae0: 733d 5472 7565 2c20 7665 7262 6f73 653d  s=True, verbose=
-0000caf0: 5472 7565 293a 0a0a 0a20 2020 2020 2020  True):...       
-0000cb00: 2073 656c 662e 5f72 6169 7365 5f65 7272   self._raise_err
-0000cb10: 6f72 7320 3d20 7261 6973 655f 6572 726f  ors = raise_erro
-0000cb20: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
-0000cb30: 5f76 6572 626f 7365 203d 2076 6572 626f  _verbose = verbo
-0000cb40: 7365 0a20 2020 2020 2020 200a 2020 2020  se.        .    
-0000cb50: 2020 2020 2320 6669 6c65 2070 6174 680a      # file path.
-0000cb60: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
-0000cb70: 7269 6573 5f70 6174 6820 3d20 4e6f 6e65  ries_path = None
-0000cb80: 0a0a 2020 2020 2020 2020 2320 7365 7269  ..        # seri
-0000cb90: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
-0000cba0: 5f73 6572 6965 735f 6e61 6d65 203d 204e  _series_name = N
-0000cbb0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000cbc0: 2e5f 7365 7269 6573 5f6e 756d 203d 204e  ._series_num = N
-0000cbd0: 6f6e 650a 2020 2020 2020 2020 0a20 2020  one.        .   
-0000cbe0: 2020 2020 2023 2063 7572 7265 6e74 2066       # current f
-0000cbf0: 696c 6520 696e 666f 0a20 2020 2020 2020  ile info.       
-0000cc00: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-0000cc10: 696c 6520 3d20 4e6f 6e65 0a20 2020 2020  ile = None.     
-0000cc20: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000cc30: 5f66 696c 655f 6e61 6d65 203d 204e 6f6e  _file_name = Non
-0000cc40: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-0000cc50: 6375 7272 656e 745f 6669 6c65 5f6e 625f  current_file_nb_
-0000cc60: 6576 656e 7473 203d 2030 0a20 2020 2020  events = 0.     
-0000cc70: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000cc80: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
-0000cc90: 7465 7220 3d20 300a 2020 2020 2020 2020  ter = 0.        
-0000cca0: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
-0000ccb0: 6c65 5f61 6463 5f67 726f 7570 203d 204e  le_adc_group = N
-0000ccc0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000ccd0: 2e5f 6375 7272 656e 745f 6669 6c65 5f64  ._current_file_d
-0000cce0: 6574 636f 6e66 6967 5f67 726f 7570 203d  etconfig_group =
-0000ccf0: 204e 6f6e 650a 2020 2020 2020 2020 0a20   None.        . 
-0000cd00: 2020 2020 2020 2023 206d 6574 6164 6174         # metadat
-0000cd10: 610a 2020 2020 2020 2020 7365 6c66 2e5f  a.        self._
-0000cd20: 6669 6c65 5f6d 6574 6164 6174 6120 3d20  file_metadata = 
-0000cd30: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000cd40: 662e 5f64 6574 6563 746f 725f 636f 6e66  f._detector_conf
-0000cd50: 6967 203d 204e 6f6e 650a 2020 2020 2020  ig = None.      
-0000cd60: 2020 7365 6c66 2e5f 6164 635f 636f 6e66    self._adc_conf
-0000cd70: 6967 2020 3d20 4e6f 6e65 0a0a 2020 2020  ig  = None..    
-0000cd80: 2020 2020 0a20 2020 2020 2020 2023 2065      .        # e
-0000cd90: 7665 6e74 2063 6f75 6e74 6572 0a20 2020  vent counter.   
-0000cda0: 2020 2020 2073 656c 662e 5f67 6c6f 6261       self._globa
-0000cdb0: 6c5f 6576 656e 745f 636f 756e 7465 7220  l_event_counter 
-0000cdc0: 3d20 300a 2020 2020 2020 2020 200a 2020  = 0.         .  
-0000cdd0: 2020 2020 2020 2320 6669 6c65 2063 6f75        # file cou
-0000cde0: 6e74 6572 0a20 2020 2020 2020 2073 656c  nter.        sel
-0000cdf0: 662e 5f66 696c 655f 636f 756e 7465 7220  f._file_counter 
-0000ce00: 3d20 300a 0a20 2020 2020 2020 2023 206d  = 0..        # m
-0000ce10: 6178 2065 7665 6e74 2070 6572 2064 756d  ax event per dum
-0000ce20: 700a 2020 2020 2020 2020 7365 6c66 2e5f  p.        self._
-0000ce30: 6e62 5f65 7665 6e74 735f 7065 725f 6475  nb_events_per_du
-0000ce40: 6d70 5f6d 6178 203d 2031 3030 300a 2020  mp_max = 1000.  
-0000ce50: 2020 2020 2020 7365 6c66 2e5f 6164 635f        self._adc_
-0000ce60: 6e61 6d65 203d 2027 6164 6331 270a 0a0a  name = 'adc1'...
-0000ce70: 2020 2020 6465 6620 696e 6974 6961 6c69      def initiali
-0000ce80: 7a65 2873 656c 662c 2073 6572 6965 735f  ze(self, series_
-0000ce90: 6e61 6d65 2c20 6461 7461 5f70 6174 683d  name, data_path=
-0000cea0: 272e 2f27 293a 0a20 2020 2020 2020 2022  './'):.        "
-0000ceb0: 2222 0a20 2020 2020 2020 2049 6e69 7469  "".        Initi
-0000cec0: 616c 697a 6520 6e65 7720 7772 6974 696e  alize new writin
-0000ced0: 670a 2020 2020 2020 2020 2222 220a 2020  g.        """.  
-0000cee0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-0000cef0: 2063 6c65 6172 2065 7665 7279 7468 696e   clear everythin
-0000cf00: 670a 2020 2020 2020 2020 7365 6c66 2e63  g.        self.c
-0000cf10: 6c65 6172 2829 0a20 2020 2020 2020 200a  lear().        .
-0000cf20: 2020 2020 2020 2020 2320 7365 7269 6573          # series
-0000cf30: 206e 616d 6520 0a20 2020 2020 2020 2073   name .        s
-0000cf40: 656c 662e 5f73 6572 6965 735f 6e61 6d65  elf._series_name
-0000cf50: 203d 2073 6572 6965 735f 6e61 6d65 0a20   = series_name. 
-0000cf60: 2020 2020 2020 2073 656c 662e 5f73 6572         self._ser
-0000cf70: 6965 735f 6e75 6d20 3d20 6578 7472 6163  ies_num = extrac
-0000cf80: 745f 7365 7269 6573 5f6e 756d 2873 6572  t_series_num(ser
-0000cf90: 6965 735f 6e61 6d65 290a 2020 2020 2020  ies_name).      
-0000cfa0: 2020 0a0a 0a20 2020 2020 2020 2023 2063    ...        # c
-0000cfb0: 7265 6174 6520 6e65 7720 6469 7265 6374  reate new direct
-0000cfc0: 6f72 790a 2020 2020 2020 2020 2373 656c  ory.        #sel
-0000cfd0: 662e 5f73 6572 6965 735f 7061 7468 203d  f._series_path =
-0000cfe0: 2064 6174 615f 7061 7468 202b 2027 2f27   data_path + '/'
-0000cff0: 202b 2073 6572 6965 735f 6e61 6d65 0a20   + series_name. 
-0000d000: 2020 2020 2020 2073 656c 662e 5f73 6572         self._ser
-0000d010: 6965 735f 7061 7468 203d 2064 6174 615f  ies_path = data_
-0000d020: 7061 7468 0a20 2020 2020 2020 200a 2020  path.        .  
-0000d030: 2020 2020 2020 6966 206e 6f74 206f 732e        if not os.
-0000d040: 7061 7468 2e69 7364 6972 2873 656c 662e  path.isdir(self.
-0000d050: 5f73 6572 6965 735f 7061 7468 293a 0a20  _series_path):. 
-0000d060: 2020 2020 2020 2020 2020 206f 732e 6d6b             os.mk
-0000d070: 6469 7228 7365 6c66 2e5f 7365 7269 6573  dir(self._series
-0000d080: 5f70 6174 6829 0a20 2020 2020 2020 2020  _path).         
-0000d090: 2020 206f 732e 6368 6d6f 6428 7365 6c66     os.chmod(self
-0000d0a0: 2e5f 7365 7269 6573 5f70 6174 682c 0a20  ._series_path,. 
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 2020 2020 7374 6174 2e53 5f49 5257 5847      stat.S_IRWXG
-0000d0d0: 207c 2073 7461 742e 535f 4952 5758 5520   | stat.S_IRWXU 
-0000d0e0: 7c20 7374 6174 2e53 5f49 524f 5448 207c  | stat.S_IROTH |
-0000d0f0: 2073 7461 742e 535f 4958 4f54 4829 0a0a   stat.S_IXOTH)..
-0000d100: 0a20 2020 2064 6566 2073 6574 5f6d 6574  .    def set_met
-0000d110: 6164 6174 6128 7365 6c66 2c20 6669 6c65  adata(self, file
-0000d120: 5f6d 6574 6164 6174 613d 4e6f 6e65 2c20  _metadata=None, 
-0000d130: 6164 635f 636f 6e66 6967 3d4e 6f6e 652c  adc_config=None,
-0000d140: 2064 6574 6563 746f 725f 636f 6e66 6967   detector_config
-0000d150: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0000d160: 2222 220a 2020 2020 2020 2020 5365 7420  """.        Set 
-0000d170: 6d65 7461 6461 7461 2077 6869 6368 2077  metadata which w
-0000d180: 696c 6c20 6265 2077 7269 7474 656e 2020  ill be written  
-0000d190: 696e 2065 6163 6820 6669 6c65 730a 2020  in each files.  
-0000d1a0: 2020 2020 2020 6669 6c65 5f6d 6574 6164        file_metad
-0000d1b0: 6174 6120 3d20 6765 6e65 7261 6c20 6461  ata = general da
-0000d1c0: 7461 2074 616b 696e 6720 696e 666f 726d  ta taking inform
-0000d1d0: 6174 696f 6e20 2866 696c 6520 6c65 7665  ation (file leve
-0000d1e0: 6c20 6d65 7461 6461 7461 290a 2020 2020  l metadata).    
-0000d1f0: 2020 2020 6164 635f 636f 6e66 6967 203d      adc_config =
-0000d200: 2061 6463 2063 6f6e 6669 6775 7261 7469   adc configurati
-0000d210: 6f6e 2028 6772 6f75 7020 6c65 7665 6c20  on (group level 
-0000d220: 6d65 7461 6461 7461 290a 2020 2020 2020  metadata).      
-0000d230: 2020 6465 7465 6374 6f72 5f63 6f6e 6669    detector_confi
-0000d240: 6720 3d20 6465 7465 6374 6f72 2073 6574  g = detector set
-0000d250: 7469 6e67 7320 2867 726f 7570 206c 6576  tings (group lev
-0000d260: 656c 206d 6574 6164 6174 6129 0a20 2020  el metadata).   
-0000d270: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000d280: 2020 6966 2066 696c 655f 6d65 7461 6461    if file_metada
-0000d290: 7461 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ta is not None:.
-0000d2a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000d2b0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0000d2c0: 6365 2866 696c 655f 6d65 7461 6461 7461  ce(file_metadata
-0000d2d0: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
-0000d2e0: 2020 2020 2020 2020 2073 656c 662e 5f66           self._f
-0000d2f0: 696c 655f 6d65 7461 6461 7461 203d 2066  ile_metadata = f
-0000d300: 696c 655f 6d65 7461 6461 7461 0a20 2020  ile_metadata.   
-0000d310: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000d320: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000d330: 7269 6e74 2827 5741 524e 494e 473a 206d  rint('WARNING: m
-0000d340: 6574 6164 6174 6120 6e65 6564 7320 746f  etadata needs to
-0000d350: 2062 6520 6120 6469 6374 696f 6e61 7279   be a dictionary
-0000d360: 2729 0a0a 2020 2020 2020 2020 2020 2020  ')..            
-0000d370: 2020 2020 0a20 2020 2020 2020 2069 6620      .        if 
-0000d380: 6164 635f 636f 6e66 6967 2069 7320 6e6f  adc_config is no
-0000d390: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000d3a0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-0000d3b0: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
-0000d3c0: 6463 5f63 6f6e 6669 672c 2064 6963 7429  dc_config, dict)
-0000d3d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d3e0: 2020 7365 6c66 2e5f 6164 635f 636f 6e66    self._adc_conf
-0000d3f0: 6967 203d 2061 6463 5f63 6f6e 6669 670a  ig = adc_config.
-0000d400: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000d410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d420: 2020 7072 696e 7428 2757 4152 4e49 4e47    print('WARNING
-0000d430: 3a20 6164 635f 636f 6e66 6967 206e 6565  : adc_config nee
-0000d440: 6473 2074 6f20 6265 2061 2064 6963 7469  ds to be a dicti
-0000d450: 6f6e 6172 7927 290a 0a0a 2020 2020 2020  onary')...      
-0000d460: 2020 6966 2064 6574 6563 746f 725f 636f    if detector_co
-0000d470: 6e66 6967 2069 7320 6e6f 7420 4e6f 6e65  nfig is not None
-0000d480: 3a0a 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0000d490: 6620 6973 696e 7374 616e 6365 2864 6574  f isinstance(det
-0000d4a0: 6563 746f 725f 636f 6e66 6967 2c20 6469  ector_config, di
-0000d4b0: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
-0000d4c0: 2020 2020 2073 656c 662e 5f64 6574 6563       self._detec
-0000d4d0: 746f 725f 636f 6e66 6967 203d 2064 6574  tor_config = det
-0000d4e0: 6563 746f 725f 636f 6e66 6967 0a20 2020  ector_config.   
-0000d4f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000d500: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000d510: 7269 6e74 2827 5741 524e 494e 473a 2064  rint('WARNING: d
-0000d520: 6574 6563 746f 7220 636f 6e66 6967 206e  etector config n
-0000d530: 6565 6473 2074 6f20 6265 2061 2064 6963  eeds to be a dic
-0000d540: 7469 6f6e 6172 7927 290a 0a0a 2020 2020  tionary')...    
-0000d550: 2020 2020 2020 2020 2020 2020 0a0a 2020              ..  
-0000d560: 2020 2020 2020 2020 2020 0a0a 2020 2020            ..    
-0000d570: 6465 6620 636c 6f73 6528 7365 6c66 293a  def close(self):
-0000d580: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d590: 2020 2020 2063 6c6f 7365 2063 7572 7265       close curre
-0000d5a0: 6e74 2066 696c 650a 2020 2020 2020 2020  nt file.        
-0000d5b0: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
-0000d5c0: 662e 5f63 6c6f 7365 5f66 696c 6528 290a  f._close_file().
-0000d5d0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-0000d5e0: 2020 2020 200a 2020 2020 6465 6620 636c       .    def cl
-0000d5f0: 6561 7228 7365 6c66 293a 0a20 2020 2020  ear(self):.     
-0000d600: 2020 2073 656c 662e 5f63 6c6f 7365 5f66     self._close_f
-0000d610: 696c 6528 290a 2020 2020 2020 2020 7365  ile().        se
-0000d620: 6c66 2e5f 6669 6c65 5f63 6f75 6e74 6572  lf._file_counter
-0000d630: 203d 2030 0a20 2020 2020 2020 2073 656c   = 0.        sel
-0000d640: 662e 5f63 7572 7265 6e74 5f66 696c 6520  f._current_file 
-0000d650: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0000d660: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
-0000d670: 655f 6e61 6d65 203d 204e 6f6e 650a 2020  e_name = None.  
-0000d680: 2020 2020 2020 7365 6c66 2e5f 6375 7272        self._curr
-0000d690: 656e 745f 6669 6c65 5f61 6463 5f67 726f  ent_file_adc_gro
-0000d6a0: 7570 203d 204e 6f6e 650a 2020 2020 2020  up = None.      
-0000d6b0: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
-0000d6c0: 6669 6c65 5f64 6574 636f 6e66 6967 5f67  file_detconfig_g
-0000d6d0: 726f 7570 203d 204e 6f6e 6520 2020 200a  roup = None    .
-0000d6e0: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-0000d6f0: 7272 656e 745f 6669 6c65 5f65 7665 6e74  rrent_file_event
-0000d700: 5f63 6f75 6e74 6572 203d 2030 0a20 2020  _counter = 0.   
-0000d710: 2020 2020 2073 656c 662e 5f67 6c6f 6261       self._globa
-0000d720: 6c5f 6576 656e 745f 636f 756e 7465 7220  l_event_counter 
-0000d730: 3d20 300a 2020 2020 2020 2020 7365 6c66  = 0.        self
-0000d740: 2e5f 6669 6c65 5f6d 6574 6164 6174 6120  ._file_metadata 
-0000d750: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-0000d760: 656c 662e 5f64 6574 6563 746f 725f 636f  elf._detector_co
-0000d770: 6e66 6967 203d 204e 6f6e 650a 2020 2020  nfig = None.    
-0000d780: 2020 2020 7365 6c66 2e5f 6164 635f 636f      self._adc_co
-0000d790: 6e66 6967 203d 204e 6f6e 650a 2020 2020  nfig = None.    
-0000d7a0: 200a 2020 2020 2020 2020 0a20 2020 2064   .        .    d
-0000d7b0: 6566 2077 7269 7465 5f65 7665 6e74 2873  ef write_event(s
-0000d7c0: 656c 662c 2064 6174 615f 6172 7261 792c  elf, data_array,
-0000d7d0: 2070 7265 6669 783d 4e6f 6e65 2c20 6461   prefix=None, da
-0000d7e0: 7461 7365 745f 6d65 7461 6461 7461 3d4e  taset_metadata=N
-0000d7f0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0000d800: 2020 2020 2020 2020 2064 6174 615f 6d6f           data_mo
-0000d810: 6465 3d4e 6f6e 652c 2061 6463 5f6e 616d  de=None, adc_nam
-0000d820: 653d 2761 6463 3127 293a 0a20 2020 2020  e='adc1'):.     
-0000d830: 2020 2022 2222 0a20 2020 2020 2020 2077     """.        w
-0000d840: 7269 7465 2070 756c 7365 2064 6174 6120  rite pulse data 
-0000d850: 696e 2066 696c 6573 0a20 2020 2020 2020  in files.       
-0000d860: 2022 2222 0a0a 0a20 2020 2020 2020 2023   """...        #
-0000d870: 206f 7065 6e20 6669 6c65 2069 6620 6e65   open file if ne
-0000d880: 6564 6564 0a20 2020 2020 2020 2069 6620  eded.        if 
-0000d890: 2873 656c 662e 5f63 7572 7265 6e74 5f66  (self._current_f
-0000d8a0: 696c 6520 6973 204e 6f6e 6520 6f72 0a20  ile is None or. 
-0000d8b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d8c0: 5f63 7572 7265 6e74 5f66 696c 655f 6576  _current_file_ev
-0000d8d0: 656e 745f 636f 756e 7465 7220 3e3d 2073  ent_counter >= s
-0000d8e0: 656c 662e 5f6e 625f 6576 656e 7473 5f70  elf._nb_events_p
-0000d8f0: 6572 5f64 756d 705f 6d61 7829 3a0a 2020  er_dump_max):.  
-0000d900: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000d910: 6f70 656e 5f66 696c 6528 7072 6566 6978  open_file(prefix
-0000d920: 3d70 7265 6669 7829 0a0a 0a20 2020 2020  =prefix)...     
-0000d930: 2020 2023 2065 7665 6e74 2063 6f75 6e74     # event count
-0000d940: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
-0000d950: 5f63 7572 7265 6e74 5f66 696c 655f 6576  _current_file_ev
-0000d960: 656e 745f 636f 756e 7465 7220 2b3d 2031  ent_counter += 1
-0000d970: 0a20 2020 2020 2020 2073 656c 662e 5f67  .        self._g
-0000d980: 6c6f 6261 6c5f 6576 656e 745f 636f 756e  lobal_event_coun
-0000d990: 7465 7220 2b3d 2031 0a20 2020 2020 2020  ter += 1.       
-0000d9a0: 200a 2020 2020 2020 2020 2320 6372 6561   .        # crea
-0000d9b0: 7465 2064 6174 6173 6574 0a20 2020 2020  te dataset.     
-0000d9c0: 2020 2064 6174 6173 6574 5f6e 616d 6520     dataset_name 
-0000d9d0: 3d20 2765 7665 6e74 5f27 202b 2073 7472  = 'event_' + str
-0000d9e0: 2873 656c 662e 5f63 7572 7265 6e74 5f66  (self._current_f
-0000d9f0: 696c 655f 6576 656e 745f 636f 756e 7465  ile_event_counte
-0000da00: 7229 0a20 2020 2020 2020 2064 6174 6173  r).        datas
-0000da10: 6574 203d 2073 656c 662e 5f63 7572 7265  et = self._curre
-0000da20: 6e74 5f66 696c 655f 6164 635f 6772 6f75  nt_file_adc_grou
-0000da30: 702e 6372 6561 7465 5f64 6174 6173 6574  p.create_dataset
-0000da40: 2864 6174 6173 6574 5f6e 616d 652c 2064  (dataset_name, d
-0000da50: 6174 613d 6461 7461 5f61 7272 6179 290a  ata=data_array).
-0000da60: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-0000da70: 2061 6464 206d 6574 6164 6174 610a 2020   add metadata.  
-0000da80: 2020 2020 2020 6966 2064 6174 6173 6574        if dataset
-0000da90: 5f6d 6574 6164 6174 6120 6973 206e 6f74  _metadata is not
-0000daa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000dab0: 2020 2066 6f72 206b 6579 2c76 616c 2069     for key,val i
-0000dac0: 6e20 6461 7461 7365 745f 6d65 7461 6461  n dataset_metada
-0000dad0: 7461 2e69 7465 6d73 2829 3a0a 2020 2020  ta.items():.    
-0000dae0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-0000daf0: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
-0000db00: 6e70 2e6e 6461 7272 6179 2920 616e 6420  np.ndarray) and 
-0000db10: 7661 6c2e 6474 7970 652e 7479 7065 2069  val.dtype.type i
-0000db20: 7320 6e70 2e73 7472 5f29 3a0a 2020 2020  s np.str_):.    
-0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 6474 203d 2068 3570 792e 7374 7269 6e67  dt = h5py.string
-0000db50: 5f64 7479 7065 2829 0a20 2020 2020 2020  _dtype().       
-0000db60: 2020 2020 2020 2020 2020 2020 2076 616c               val
-0000db70: 203d 2076 616c 2e61 7374 7970 6528 6474   = val.astype(dt
-0000db80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000db90: 2020 6461 7461 7365 742e 6174 7472 735b    dataset.attrs[
-0000dba0: 6b65 795d 203d 2076 616c 0a0a 2020 2020  key] = val..    
-0000dbb0: 2020 2020 6461 7461 7365 742e 6174 7472      dataset.attr
-0000dbc0: 735b 2765 7665 6e74 5f69 6427 5d20 3d20  s['event_id'] = 
-0000dbd0: 7365 6c66 2e5f 676c 6f62 616c 5f65 7665  self._global_eve
-0000dbe0: 6e74 5f63 6f75 6e74 6572 200a 2020 2020  nt_counter .    
-0000dbf0: 2020 2020 6461 7461 7365 742e 6174 7472      dataset.attr
-0000dc00: 735b 2765 7665 6e74 5f69 6e64 6578 275d  s['event_index']
-0000dc10: 203d 2073 656c 662e 5f63 7572 7265 6e74   = self._current
-0000dc20: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
-0000dc30: 7465 720a 2020 2020 2020 2020 6461 7461  ter.        data
-0000dc40: 7365 742e 6174 7472 735b 2765 7665 6e74  set.attrs['event
-0000dc50: 5f6e 756d 275d 203d 2073 656c 662e 5f66  _num'] = self._f
-0000dc60: 696c 655f 636f 756e 7465 7220 2a31 3030  ile_counter *100
-0000dc70: 3030 3020 2b20 7365 6c66 2e5f 6375 7272  000 + self._curr
-0000dc80: 656e 745f 6669 6c65 5f65 7665 6e74 5f63  ent_file_event_c
-0000dc90: 6f75 6e74 6572 0a20 2020 2020 2020 2020  ounter.         
-0000dca0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000dcb0: 2320 7570 6461 7465 206e 756d 6265 7220  # update number 
-0000dcc0: 6f66 2065 7665 6e74 730a 2020 2020 2020  of events.      
-0000dcd0: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
-0000dce0: 6669 6c65 5f61 6463 5f67 726f 7570 2e61  file_adc_group.a
-0000dcf0: 7474 7273 5b27 6e62 5f65 7665 6e74 7327  ttrs['nb_events'
-0000dd00: 5d20 3d20 7365 6c66 2e5f 6375 7272 656e  ] = self._curren
-0000dd10: 745f 6669 6c65 5f65 7665 6e74 5f63 6f75  t_file_event_cou
-0000dd20: 6e74 6572 0a20 2020 2020 2020 2069 6620  nter.        if 
-0000dd30: 6461 7461 5f6d 6f64 6520 6973 206e 6f74  data_mode is not
-0000dd40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000dd50: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000dd60: 5f66 696c 655f 6164 635f 6772 6f75 702e  _file_adc_group.
-0000dd70: 6174 7472 735b 2764 6174 615f 6d6f 6465  attrs['data_mode
-0000dd80: 275d 203d 2073 7472 2864 6174 615f 6d6f  '] = str(data_mo
-0000dd90: 6465 290a 0a0a 2020 2020 2020 2020 2320  de)...        # 
-0000dda0: 666c 7573 680a 2020 2020 2020 2020 7365  flush.        se
-0000ddb0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-0000ddc0: 2e66 6c75 7368 2829 0a20 2020 2020 2020  .flush().       
-0000ddd0: 200a 0a0a 0a0a 0a20 2020 2020 2020 2020   ......         
-0000dde0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-0000ddf0: 6465 6620 5f6f 7065 6e5f 6669 6c65 2873  def _open_file(s
-0000de00: 656c 662c 2070 7265 6669 783d 4e6f 6e65  elf, prefix=None
-0000de10: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000de20: 2020 2020 2020 206f 7065 6e20 6669 6c65         open file
-0000de30: 200a 2020 2020 2020 2020 2222 220a 0a20   .        """.. 
-0000de40: 2020 2020 2020 2023 2063 6c6f 7365 2066         # close f
-0000de50: 696c 6520 6966 206e 6565 6465 640a 2020  ile if needed.  
-0000de60: 2020 2020 2020 6966 2073 656c 662e 5f63        if self._c
-0000de70: 7572 7265 6e74 5f66 696c 6520 6973 206e  urrent_file is n
-0000de80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000de90: 2020 2020 2073 656c 662e 5f63 6c6f 7365       self._close
-0000dea0: 5f66 696c 6528 290a 0a0a 2020 2020 2020  _file()...      
-0000deb0: 2020 2320 6475 6d70 0a20 2020 2020 2020    # dump.       
-0000dec0: 2073 656c 662e 5f66 696c 655f 636f 756e   self._file_coun
-0000ded0: 7465 7220 2b3d 310a 2020 2020 2020 2020  ter +=1.        
-0000dee0: 6475 6d70 203d 2073 7472 2873 656c 662e  dump = str(self.
-0000def0: 5f66 696c 655f 636f 756e 7465 7229 0a20  _file_counter). 
-0000df00: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
-0000df10: 7261 6e67 6528 312c 352d 6c65 6e28 6475  range(1,5-len(du
-0000df20: 6d70 2929 3a0a 2020 2020 2020 2020 2020  mp)):.          
-0000df30: 2020 6966 2078 3e3d 313a 0a20 2020 2020    if x>=1:.     
-0000df40: 2020 2020 2020 2020 2020 2064 756d 7020             dump 
-0000df50: 3d20 2730 272b 6475 6d70 0a0a 0a20 2020  = '0'+dump...   
-0000df60: 2020 2020 2023 2066 756c 6c20 6669 6c65       # full file
-0000df70: 206e 616d 650a 2020 2020 2020 2020 6669   name.        fi
-0000df80: 6c65 5f6e 616d 6520 3d20 7365 6c66 2e5f  le_name = self._
-0000df90: 7365 7269 6573 5f70 6174 6820 2b20 272f  series_path + '/
-0000dfa0: 270a 2020 2020 2020 2020 6966 2070 7265  '.        if pre
-0000dfb0: 6669 7820 6973 206e 6f74 204e 6f6e 653a  fix is not None:
-0000dfc0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-0000dfd0: 655f 6e61 6d65 202b 3d20 7072 6566 6978  e_name += prefix
-0000dfe0: 202b 2027 5f27 0a20 2020 2020 2020 2066   + '_'.        f
-0000dff0: 696c 655f 6e61 6d65 202b 3d20 7365 6c66  ile_name += self
-0000e000: 2e5f 7365 7269 6573 5f6e 616d 6520 2b20  ._series_name + 
-0000e010: 275f 4627 202b 2064 756d 7020 2b20 272e  '_F' + dump + '.
-0000e020: 6864 6635 270a 2020 2020 2020 2020 7072  hdf5'.        pr
-0000e030: 696e 7428 2749 4e46 4f3a 204f 7065 6e69  int('INFO: Openi
-0000e040: 6e67 2066 696c 6520 6e61 6d65 2022 2720  ng file name "' 
-0000e050: 2b20 6669 6c65 5f6e 616d 6520 2b20 2722  + file_name + '"
-0000e060: 2729 0a20 2020 2020 2020 200a 2020 2020  ').        .    
-0000e070: 2020 2020 0a20 2020 2020 2020 2066 696c      .        fil
-0000e080: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
-0000e090: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000e0a0: 2020 6669 6c65 203d 2068 3570 792e 4669    file = h5py.Fi
-0000e0b0: 6c65 2866 696c 655f 6e61 6d65 2c20 2777  le(file_name, 'w
-0000e0c0: 2729 0a20 2020 2020 2020 2065 7863 6570  ').        excep
-0000e0d0: 743a 0a20 2020 2020 2020 2020 2020 2070  t:.            p
-0000e0e0: 7269 6e74 2827 4552 524f 523a 2055 6e61  rint('ERROR: Una
-0000e0f0: 626c 6520 746f 206f 7065 6e20 6669 6c65  ble to open file
-0000e100: 2027 202b 2066 696c 655f 6e61 6d65 290a   ' + file_name).
-0000e110: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000e120: 726e 0a0a 2020 2020 2020 2020 7365 6c66  rn..        self
-0000e130: 2e5f 6375 7272 656e 745f 6669 6c65 203d  ._current_file =
-0000e140: 2066 696c 650a 2020 2020 2020 2020 7365   file.        se
-0000e150: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-0000e160: 5f6e 616d 6520 3d20 6669 6c65 5f6e 616d  _name = file_nam
-0000e170: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-0000e180: 6375 7272 656e 745f 6669 6c65 5f6e 625f  current_file_nb_
-0000e190: 6576 656e 7473 203d 2030 0a20 2020 2020  events = 0.     
-0000e1a0: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000e1b0: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
-0000e1c0: 7465 7220 3d20 300a 0a0a 2020 2020 2020  ter = 0...      
-0000e1d0: 2020 2320 6669 6c65 206d 6574 6164 6174    # file metadat
-0000e1e0: 610a 2020 2020 2020 2020 6966 2073 656c  a.        if sel
-0000e1f0: 662e 5f66 696c 655f 6d65 7461 6461 7461  f._file_metadata
-0000e200: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e210: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
-0000e220: 792c 7661 6c20 696e 2073 656c 662e 5f66  y,val in self._f
-0000e230: 696c 655f 6d65 7461 6461 7461 2e69 7465  ile_metadata.ite
-0000e240: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-0000e250: 2020 2020 2020 6966 2028 6973 696e 7374        if (isinst
-0000e260: 616e 6365 2876 616c 2c20 6e70 2e6e 6461  ance(val, np.nda
-0000e270: 7272 6179 2920 616e 6420 7661 6c2e 6474  rray) and val.dt
-0000e280: 7970 652e 7479 7065 2069 7320 6e70 2e73  ype.type is np.s
-0000e290: 7472 5f29 3a0a 2020 2020 2020 2020 2020  tr_):.          
-0000e2a0: 2020 2020 2020 2020 2020 6474 203d 2068            dt = h
-0000e2b0: 3570 792e 7374 7269 6e67 5f64 7479 7065  5py.string_dtype
-0000e2c0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000e2d0: 2020 2020 2020 2076 616c 203d 2076 616c         val = val
-0000e2e0: 2e61 7374 7970 6528 6474 290a 2020 2020  .astype(dt).    
-0000e2f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e300: 2e5f 6375 7272 656e 745f 6669 6c65 2e61  ._current_file.a
-0000e310: 7474 7273 5b6b 6579 5d20 3d20 7661 6c0a  ttrs[key] = val.
-0000e320: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
-0000e330: 7272 656e 745f 6669 6c65 2e61 7474 7273  rrent_file.attrs
-0000e340: 5b27 7072 6566 6978 275d 203d 2070 7265  ['prefix'] = pre
-0000e350: 6669 780a 2020 2020 2020 2020 7365 6c66  fix.        self
-0000e360: 2e5f 6375 7272 656e 745f 6669 6c65 2e61  ._current_file.a
-0000e370: 7474 7273 5b27 7365 7269 6573 5f6e 756d  ttrs['series_num
-0000e380: 275d 203d 2073 656c 662e 5f73 6572 6965  '] = self._serie
-0000e390: 735f 6e75 6d0a 2020 2020 2020 2020 7365  s_num.        se
-0000e3a0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-0000e3b0: 2e61 7474 7273 5b27 6475 6d70 5f6e 756d  .attrs['dump_num
-0000e3c0: 275d 203d 2069 6e74 2864 756d 7029 0a20  '] = int(dump). 
-0000e3d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0000e3e0: 2320 6465 7465 6374 6f72 2063 6f6e 6669  # detector confi
-0000e3f0: 670a 2020 2020 2020 2020 6966 2073 656c  g.        if sel
-0000e400: 662e 5f64 6574 6563 746f 725f 636f 6e66  f._detector_conf
-0000e410: 6967 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ig is not None:.
-0000e420: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000e430: 636f 6e66 6967 5f6b 6579 2c63 6f6e 6669  config_key,confi
-0000e440: 675f 7661 6c20 696e 2073 656c 662e 5f64  g_val in self._d
-0000e450: 6574 6563 746f 725f 636f 6e66 6967 2e69  etector_config.i
-0000e460: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-0000e470: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000e480: 7461 6e63 6528 636f 6e66 6967 5f76 616c  tance(config_val
-0000e490: 2c64 6963 7429 3a0a 2020 2020 2020 2020  ,dict):.        
-0000e4a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e4b0: 2e5f 6375 7272 656e 745f 6669 6c65 5f64  ._current_file_d
-0000e4c0: 6574 636f 6e66 6967 5f67 726f 7570 203d  etconfig_group =
-0000e4d0: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
-0000e4e0: 696c 652e 6372 6561 7465 5f67 726f 7570  ile.create_group
-0000e4f0: 2863 6f6e 6669 675f 6b65 7929 0a20 2020  (config_key).   
-0000e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e510: 2066 6f72 206b 6579 2c76 616c 2069 6e20   for key,val in 
-0000e520: 636f 6e66 6967 5f76 616c 2e69 7465 6d73  config_val.items
-0000e530: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000e540: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-0000e550: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
-0000e560: 6e70 2e6e 6461 7272 6179 2920 616e 6420  np.ndarray) and 
-0000e570: 7661 6c2e 6474 7970 652e 7479 7065 2069  val.dtype.type i
-0000e580: 7320 6e70 2e73 7472 5f29 3a0a 2020 2020  s np.str_):.    
-0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5a0: 2020 2020 2020 2020 6474 203d 2068 3570          dt = h5p
-0000e5b0: 792e 7374 7269 6e67 5f64 7479 7065 2829  y.string_dtype()
-0000e5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e5d0: 2020 2020 2020 2020 2020 2020 2076 616c               val
-0000e5e0: 203d 2076 616c 2e61 7374 7970 6528 6474   = val.astype(dt
-0000e5f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e600: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e610: 6375 7272 656e 745f 6669 6c65 5f64 6574  current_file_det
-0000e620: 636f 6e66 6967 5f67 726f 7570 2e61 7474  config_group.att
-0000e630: 7273 5b6b 6579 5d20 3d20 7661 6c0a 2020  rs[key] = val.  
-0000e640: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-0000e650: 2063 7265 6174 6520 6164 6320 6772 6f75   create adc grou
-0000e660: 700a 2020 2020 2020 2020 6966 2073 656c  p.        if sel
-0000e670: 662e 5f61 6463 5f63 6f6e 6669 6720 6973  f._adc_config is
-0000e680: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000e690: 2020 2020 2020 2066 6f72 2063 6f6e 6669         for confi
-0000e6a0: 675f 6b65 792c 636f 6e66 6967 5f76 616c  g_key,config_val
-0000e6b0: 2069 6e20 7365 6c66 2e5f 6164 635f 636f   in self._adc_co
-0000e6c0: 6e66 6967 2e69 7465 6d73 2829 3a0a 2020  nfig.items():.  
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000e6e0: 2069 7369 6e73 7461 6e63 6528 636f 6e66   isinstance(conf
-0000e6f0: 6967 5f76 616c 2c64 6963 7429 3a0a 2020  ig_val,dict):.  
-0000e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e710: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
-0000e720: 6669 6c65 5f61 6463 5f67 726f 7570 2020  file_adc_group  
-0000e730: 3d20 7365 6c66 2e5f 6375 7272 656e 745f  = self._current_
-0000e740: 6669 6c65 2e63 7265 6174 655f 6772 6f75  file.create_grou
-0000e750: 7028 636f 6e66 6967 5f6b 6579 290a 2020  p(config_key).  
-0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e770: 2020 666f 7220 6b65 792c 7661 6c20 696e    for key,val in
-0000e780: 2063 6f6e 6669 675f 7661 6c2e 6974 656d   config_val.item
-0000e790: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-0000e7a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000e7b0: 2869 7369 6e73 7461 6e63 6528 7661 6c2c  (isinstance(val,
-0000e7c0: 206e 702e 6e64 6172 7261 7929 2061 6e64   np.ndarray) and
-0000e7d0: 2076 616c 2e64 7479 7065 2e74 7970 6520   val.dtype.type 
-0000e7e0: 6973 206e 702e 7374 725f 293a 0a20 2020  is np.str_):.   
-0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e800: 2020 2020 2020 2020 2064 7420 3d20 6835           dt = h5
-0000e810: 7079 2e73 7472 696e 675f 6474 7970 6528  py.string_dtype(
-0000e820: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e830: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0000e840: 6c20 3d20 7661 6c2e 6173 7479 7065 2864  l = val.astype(d
-0000e850: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-0000e860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e870: 5f63 7572 7265 6e74 5f66 696c 655f 6164  _current_file_ad
-0000e880: 635f 6772 6f75 702e 6174 7472 735b 6b65  c_group.attrs[ke
-0000e890: 795d 203d 2076 616c 0a20 2020 2020 2020  y] = val.       
-0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8b0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-0000e8c0: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
-0000e8d0: 2020 2020 2020 0a20 2020 2064 6566 205f        .    def _
-0000e8e0: 636c 6f73 655f 6669 6c65 2873 656c 6629  close_file(self)
-0000e8f0: 3a0a 0a20 2020 2020 2020 2069 6620 7365  :..        if se
-0000e900: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-0000e910: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e920: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e930: 6375 7272 656e 745f 6669 6c65 2e63 6c6f  current_file.clo
-0000e940: 7365 2829 0a20 200a 2020 2020 2020 2020  se().  .        
-0000e950: 2320 696e 6974 6961 6c69 7a65 0a20 2020  # initialize.   
-0000e960: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
-0000e970: 6e74 5f66 696c 6520 3d20 4e6f 6e65 0a20  nt_file = None. 
-0000e980: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
-0000e990: 7265 6e74 5f66 696c 655f 6e61 6d65 203d  rent_file_name =
-0000e9a0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-0000e9b0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
-0000e9c0: 5f6e 625f 6576 656e 7473 203d 2030 0a20  _nb_events = 0. 
-0000e9d0: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
-0000e9e0: 7265 6e74 5f66 696c 655f 6164 635f 6772  rent_file_adc_gr
-0000e9f0: 6f75 7020 3d20 4e6f 6e65 0a20 2020 2020  oup = None.     
-0000ea00: 2020 2073 656c 662e 5f63 7572 7265 6e74     self._current
-0000ea10: 5f66 696c 655f 6465 7463 6f6e 6669 675f  _file_detconfig_
-0000ea20: 6772 6f75 7020 3d20 4e6f 6e65 0a20 2020  group = None.   
-0000ea30: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
-0000ea40: 6e74 5f66 696c 655f 6576 656e 745f 636f  nt_file_event_co
-0000ea50: 756e 7465 7220 3d20 300a 0a0a 2020 2020  unter = 0...    
-0000ea60: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-0000ea70: 2020 0a0a 6465 6620 6765 7472 616e 6465    ..def getrande
-0000ea80: 7665 6e74 7328 6261 7365 7061 7468 2c20  vents(basepath, 
-0000ea90: 6576 746e 756d 732c 2073 6572 6965 736e  evtnums, seriesn
-0000eaa0: 756d 732c 2063 7574 3d4e 6f6e 652c 2063  ums, cut=None, c
-0000eab0: 6861 6e6e 656c 733d 4e6f 6e65 2c0a 2020  hannels=None,.  
-0000eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ead0: 7375 6d63 6861 6e73 3d46 616c 7365 2c20  sumchans=False, 
-0000eae0: 6c67 6370 6c6f 743d 4661 6c73 652c 206e  lgcplot=False, n
-0000eaf0: 7472 6163 6573 3d31 2c20 6e70 6c6f 743d  traces=1, nplot=
-0000eb00: 3230 2c0a 2020 2020 2020 2020 2020 2020  20,.            
-0000eb10: 2020 2020 2020 7365 6564 3d4e 6f6e 652c        seed=None,
-0000eb20: 2069 6e64 6261 7365 7072 653d 4e6f 6e65   indbasepre=None
-0000eb30: 293a 0a20 2020 2022 2222 0a20 2020 2046  ):.    """.    F
-0000eb40: 756e 6374 696f 6e20 666f 7220 6c6f 6164  unction for load
-0000eb50: 696e 6720 2861 6e64 2070 6c6f 7474 696e  ing (and plottin
-0000eb60: 6729 2072 616e 646f 6d20 6576 656e 7473  g) random events
-0000eb70: 2066 726f 6d20 6120 6461 7461 7365 7473   from a datasets
-0000eb80: 2e0a 2020 2020 4861 7320 6675 6e63 7469  ..    Has functi
-0000eb90: 6f6e 616c 6974 7920 746f 2070 756c 6c20  onality to pull 
-0000eba0: 7261 6e64 6f6d 6c79 2066 726f 6d20 6120  randomly from a 
-0000ebb0: 7370 6563 6966 6965 6420 6375 742e 0a0a  specified cut...
-0000ebc0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-0000ebd0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000ebe0: 2020 6261 7365 7061 7468 203a 2073 7472    basepath : str
-0000ebf0: 0a20 2020 2020 2020 2054 6865 2062 6173  .        The bas
-0000ec00: 6520 7061 7468 2074 6f20 7468 6520 6469  e path to the di
-0000ec10: 7265 6374 6f72 7920 7468 6174 2063 6f6e  rectory that con
-0000ec20: 7461 696e 7320 7468 6520 666f 6c64 6572  tains the folder
-0000ec30: 7320 7468 6174 0a20 2020 2020 2020 2074  s that.        t
-0000ec40: 6865 2065 7665 6e74 2064 756d 7073 2061  he event dumps a
-0000ec50: 7265 2069 6e2e 2054 6865 2066 6f6c 6465  re in. The folde
-0000ec60: 7273 2069 6e20 7468 6973 2064 6972 6563  rs in this direc
-0000ec70: 746f 7279 2073 686f 756c 6420 6265 0a20  tory should be. 
-0000ec80: 2020 2020 2020 2074 6865 2073 6572 6965         the serie
-0000ec90: 7320 6e75 6d62 6572 732e 0a20 2020 2065  s numbers..    e
-0000eca0: 7674 6e75 6d73 203a 2061 7272 6179 5f6c  vtnums : array_l
-0000ecb0: 696b 650a 2020 2020 2020 2020 416e 2061  ike.        An a
-0000ecc0: 7272 6179 206f 6620 616c 6c20 6576 656e  rray of all even
-0000ecd0: 7420 6e75 6d62 6572 7320 666f 7220 7468  t numbers for th
-0000ece0: 6520 6576 656e 7473 2069 6e20 616c 6c20  e events in all 
-0000ecf0: 6461 7461 7365 7473 2e0a 2020 2020 7365  datasets..    se
-0000ed00: 7269 6573 6e75 6d73 203a 2061 7272 6179  riesnums : array
-0000ed10: 5f6c 696b 650a 2020 2020 2020 2020 416e  _like.        An
-0000ed20: 2061 7272 6179 206f 6620 7468 6520 636f   array of the co
-0000ed30: 7272 6573 706f 6e64 696e 6720 7365 7269  rresponding seri
-0000ed40: 6573 206e 756d 6265 7273 2066 6f72 2065  es numbers for e
-0000ed50: 6163 6820 6576 656e 740a 2020 2020 2020  ach event.      
-0000ed60: 2020 6e75 6d62 6572 2069 6e20 6576 746e    number in evtn
-0000ed70: 756d 732e 0a20 2020 2063 7574 203a 2061  ums..    cut : a
-0000ed80: 7272 6179 5f6c 696b 652c 206f 7074 696f  rray_like, optio
-0000ed90: 6e61 6c0a 2020 2020 2020 2020 4120 626f  nal.        A bo
-0000eda0: 6f6c 6561 6e20 6172 7261 7920 6f66 2074  olean array of t
-0000edb0: 6865 2063 7574 2074 6861 7420 7368 6f75  he cut that shou
-0000edc0: 6c64 2062 6520 6170 706c 6965 6420 746f  ld be applied to
-0000edd0: 2074 6865 2064 6174 612e 0a20 2020 2020   the data..     
-0000ede0: 2020 2049 6620 6c65 6674 2061 7320 4e6f     If left as No
-0000edf0: 6e65 2c20 7468 656e 206e 6f20 6375 7420  ne, then no cut 
-0000ee00: 6973 2061 7070 6c69 6564 2e0a 2020 2020  is applied..    
-0000ee10: 6368 616e 6e65 6c73 203a 206c 6973 742c  channels : list,
-0000ee20: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0000ee30: 2020 4120 6c69 7374 206f 6620 7374 7269    A list of stri
-0000ee40: 6e67 7320 7468 6174 2063 6f6e 7461 696e  ngs that contain
-0000ee50: 7320 616c 6c20 6f66 2074 6865 2063 6861  s all of the cha
-0000ee60: 6e6e 656c 7320 7468 6174 2073 686f 756c  nnels that shoul
-0000ee70: 640a 2020 2020 2020 2020 6265 206c 6f61  d.        be loa
-0000ee80: 6465 642e 2049 6620 6c65 6674 2061 7320  ded. If left as 
-0000ee90: 4e6f 6e65 2c20 616c 6c20 6368 616e 6e65  None, all channe
-0000eea0: 6c73 2061 7265 206c 6f61 6465 642e 0a20  ls are loaded.. 
-0000eeb0: 2020 2073 756d 6368 616e 7320 3a20 626f     sumchans : bo
-0000eec0: 6f6c 2c20 6f70 7469 6f6e 616c 0a20 2020  ol, optional.   
-0000eed0: 2020 2020 2041 2062 6f6f 6c65 616e 2066       A boolean f
-0000eee0: 6c61 6720 666f 7220 7768 6574 6865 7220  lag for whether 
-0000eef0: 6f72 206e 6f74 2074 6f20 7375 6d20 7468  or not to sum th
-0000ef00: 6520 6368 616e 6e65 6c73 2077 6865 6e0a  e channels when.
-0000ef10: 2020 2020 2020 2020 706c 6f74 7469 6e67          plotting
-0000ef20: 2e20 4966 2046 616c 7365 2c20 6561 6368  . If False, each
-0000ef30: 2063 6861 6e6e 656c 2069 7320 706c 6f74   channel is plot
-0000ef40: 7465 6420 696e 6469 7669 6475 616c 6c79  ted individually
-0000ef50: 2e0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
-0000ef60: 7420 6973 2046 616c 7365 2e0a 2020 2020  t is False..    
-0000ef70: 6e74 7261 6365 7320 3a20 696e 742c 2073  ntraces : int, s
-0000ef80: 7472 2c20 6f70 7469 6f6e 616c 0a20 2020  tr, optional.   
-0000ef90: 2020 2020 2054 6865 206e 756d 6265 7220       The number 
-0000efa0: 6f66 2074 7261 6365 7320 746f 2072 616e  of traces to ran
-0000efb0: 646f 6d6c 7920 6c6f 6164 2066 726f 6d20  domly load from 
-0000efc0: 7468 6520 6461 7461 2028 7769 7468 2074  the data (with t
-0000efd0: 6865 0a20 2020 2020 2020 2063 7574 2c20  he.        cut, 
-0000efe0: 6966 2073 7065 6369 6669 6564 292e 2049  if specified). I
-0000eff0: 6620 616c 6c20 7472 6163 6573 2066 726f  f all traces fro
-0000f000: 6d20 6120 7370 6563 6669 6564 2063 7574  m a specfied cut
-0000f010: 2061 7265 0a20 2020 2020 2020 2064 6573   are.        des
-0000f020: 6972 6564 2c20 7061 7373 2074 6865 2073  ired, pass the s
-0000f030: 7472 696e 6720 2261 6c6c 222e 2044 6566  tring "all". Def
-0000f040: 6175 6c74 2069 7320 312e 0a20 2020 206c  ault is 1..    l
-0000f050: 6763 706c 6f74 203a 2062 6f6f 6c2c 206f  gcplot : bool, o
-0000f060: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000f070: 4c6f 6769 6361 6c20 666c 6167 206f 6e20  Logical flag on 
-0000f080: 7768 6574 6865 7220 6f72 206e 6f74 2074  whether or not t
-0000f090: 6f20 706c 6f74 2074 6865 2070 756c 6c65  o plot the pulle
-0000f0a0: 6420 7472 6163 6573 2e0a 2020 2020 6e70  d traces..    np
-0000f0b0: 6c6f 7420 3a20 696e 742c 206f 7074 696f  lot : int, optio
-0000f0c0: 6e61 6c0a 2020 2020 2020 2020 4966 206c  nal.        If l
-0000f0d0: 6763 706c 6f74 2069 7320 5472 7565 2c20  gcplot is True, 
-0000f0e0: 7468 6520 6e75 6d62 6572 206f 6620 7472  the number of tr
-0000f0f0: 6163 6573 2074 6f20 706c 6f74 2e0a 2020  aces to plot..  
-0000f100: 2020 7365 6564 203a 2069 6e74 2c20 6f70    seed : int, op
-0000f110: 7469 6f6e 616c 0a20 2020 2020 2020 2041  tional.        A
-0000f120: 2076 616c 7565 2074 6f20 7061 7373 2074   value to pass t
-0000f130: 6f20 6e70 2e72 616e 646f 6d2e 7365 6564  o np.random.seed
-0000f140: 2069 6620 7468 6520 7573 6572 2077 6973   if the user wis
-0000f150: 6865 7320 746f 2075 7365 0a20 2020 2020  hes to use.     
-0000f160: 2020 2074 6865 2073 616d 6520 7261 6e64     the same rand
-0000f170: 6f6d 2073 6565 6420 6561 6368 2074 696d  om seed each tim
-0000f180: 6520 6765 7472 616e 6465 7665 6e74 7320  e getrandevents 
-0000f190: 6973 2063 616c 6c65 642e 0a20 2020 2069  is called..    i
-0000f1a0: 6e64 6261 7365 7072 6520 3a20 4e6f 6e65  ndbasepre : None
-0000f1b0: 5479 7065 2c20 696e 742c 206f 7074 696f  Type, int, optio
-0000f1c0: 6e61 6c0a 2020 2020 2020 2020 5468 6520  nal.        The 
-0000f1d0: 6e75 6d62 6572 206f 6620 696e 6469 6365  number of indice
-0000f1e0: 7320 7570 2074 6f20 7768 6963 6820 6120  s up to which a 
-0000f1f0: 7472 6163 6520 7368 6f75 6c64 2062 6520  trace should be 
-0000f200: 6176 6572 6167 6564 2074 6f0a 2020 2020  averaged to.    
-0000f210: 2020 2020 6465 7465 726d 696e 6520 7468      determine th
-0000f220: 6520 6261 7365 6c69 6e65 2e20 5468 6973  e baseline. This
-0000f230: 2062 6173 656c 696e 6520 7769 6c6c 2074   baseline will t
-0000f240: 6865 6e20 6265 2073 7562 7472 6163 7465  hen be subtracte
-0000f250: 640a 2020 2020 2020 2020 6672 6f6d 2074  d.        from t
-0000f260: 6865 2074 7261 6365 7320 7768 656e 2070  he traces when p
-0000f270: 6c6f 7474 696e 672e 2049 6620 6c65 6674  lotting. If left
-0000f280: 2061 7320 4e6f 6e65 2c20 6e6f 2062 6173   as None, no bas
-0000f290: 656c 696e 650a 2020 2020 2020 2020 7375  eline.        su
-0000f2a0: 6274 7261 6374 696f 6e20 7769 6c6c 2062  btraction will b
-0000f2b0: 6520 646f 6e65 2e0a 0a20 2020 2052 6574  e done...    Ret
-0000f2c0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
-0000f2d0: 0a20 2020 2074 203a 206e 6461 7272 6179  .    t : ndarray
-0000f2e0: 0a20 2020 2020 2020 2054 6865 2074 696d  .        The tim
-0000f2f0: 6520 7661 6c75 6573 2066 6f72 2070 6c6f  e values for plo
-0000f300: 7474 696e 6720 7468 6520 6576 656e 7473  tting the events
-0000f310: 2e0a 2020 2020 7820 3a20 6e64 6172 7261  ..    x : ndarra
-0000f320: 790a 2020 2020 2020 2020 4172 7261 7920  y.        Array 
-0000f330: 636f 6e74 6169 6e69 6e67 2061 6c6c 206f  containing all o
-0000f340: 6620 7468 6520 6576 656e 7473 2074 6861  f the events tha
-0000f350: 7420 7765 7265 2070 756c 6c65 642e 0a20  t were pulled.. 
-0000f360: 2020 2063 7261 6e64 203a 206e 6461 7272     crand : ndarr
-0000f370: 6179 0a20 2020 2020 2020 2042 6f6f 6c65  ay.        Boole
-0000f380: 616e 2061 7272 6179 2074 6861 7420 636f  an array that co
-0000f390: 6e74 6169 6e73 2074 6865 2063 7574 206f  ntains the cut o
-0000f3a0: 6e20 7468 6520 6c6f 6164 6564 2064 6174  n the loaded dat
-0000f3b0: 612e 0a0a 2020 2020 2222 220a 0a20 2020  a...    """..   
-0000f3c0: 2069 6620 7365 6564 2069 7320 6e6f 7420   if seed is not 
-0000f3d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6e70  None:.        np
-0000f3e0: 2e72 616e 646f 6d2e 7365 6564 2873 6565  .random.seed(see
-0000f3f0: 6429 0a0a 2020 2020 6966 2069 7369 6e73  d)..    if isins
-0000f400: 7461 6e63 6528 6368 616e 6e65 6c73 2c20  tance(channels, 
-0000f410: 7374 7229 3a0a 2020 2020 2020 2020 6368  str):.        ch
-0000f420: 616e 6e65 6c73 203d 205b 6368 616e 6e65  annels = [channe
-0000f430: 6c73 5d0a 0a20 2020 2069 6620 6e6f 7420  ls]..    if not 
-0000f440: 6973 696e 7374 616e 6365 2865 7674 6e75  isinstance(evtnu
-0000f450: 6d73 2c20 7064 2e53 6572 6965 7329 3a0a  ms, pd.Series):.
-0000f460: 2020 2020 2020 2020 6576 746e 756d 7320          evtnums 
-0000f470: 3d20 7064 2e53 6572 6965 7328 6461 7461  = pd.Series(data
-0000f480: 3d65 7674 6e75 6d73 290a 2020 2020 6966  =evtnums).    if
-0000f490: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-0000f4a0: 7365 7269 6573 6e75 6d73 2c20 7064 2e53  seriesnums, pd.S
-0000f4b0: 6572 6965 7329 3a0a 2020 2020 2020 2020  eries):.        
-0000f4c0: 7365 7269 6573 6e75 6d73 203d 2070 642e  seriesnums = pd.
-0000f4d0: 5365 7269 6573 2864 6174 613d 7365 7269  Series(data=seri
-0000f4e0: 6573 6e75 6d73 290a 0a20 2020 2069 6620  esnums)..    if 
-0000f4f0: 6375 7420 6973 204e 6f6e 653a 0a20 2020  cut is None:.   
-0000f500: 2020 2020 2063 7574 203d 206e 702e 6f6e       cut = np.on
-0000f510: 6573 286c 656e 2865 7674 6e75 6d73 292c  es(len(evtnums),
-0000f520: 2064 7479 7065 3d62 6f6f 6c29 0a0a 2020   dtype=bool)..  
-0000f530: 2020 6966 206e 702e 7375 6d28 6375 7429    if np.sum(cut)
-0000f540: 203d 3d20 303a 0a20 2020 2020 2020 2072   == 0:.        r
-0000f550: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000f560: 0a20 2020 2020 2020 2020 2020 2022 5468  .            "Th
-0000f570: 6520 696e 7075 7474 6564 2063 7574 2068  e inputted cut h
-0000f580: 6173 206e 6f20 6576 656e 7473 2c20 6361  as no events, ca
-0000f590: 6e6e 6f74 206c 6f61 6420 616e 7920 7472  nnot load any tr
-0000f5a0: 6163 6573 2e22 0a20 2020 2020 2020 2029  aces.".        )
-0000f5b0: 0a0a 2020 2020 6966 206e 7472 6163 6573  ..    if ntraces
-0000f5c0: 203d 3d20 2761 6c6c 2720 6f72 206e 7472   == 'all' or ntr
-0000f5d0: 6163 6573 203e 206e 702e 7375 6d28 6375  aces > np.sum(cu
-0000f5e0: 7429 3a0a 2020 2020 2020 2020 6e74 7261  t):.        ntra
-0000f5f0: 6365 7320 3d20 6e70 2e73 756d 2863 7574  ces = np.sum(cut
-0000f600: 290a 2020 2020 2020 2020 6966 206e 7472  ).        if ntr
-0000f610: 6163 6573 203e 2031 3030 303a 0a20 2020  aces > 1000:.   
-0000f620: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
-0000f630: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
-0000f640: 2020 2020 2020 2020 2259 6f75 2061 7265          "You are
-0000f650: 206c 6f61 6469 6e67 2061 206c 6172 6765   loading a large
-0000f660: 206e 756d 6265 7220 6f66 2074 7261 6365   number of trace
-0000f670: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
-0000f680: 2020 2020 6622 287b 6e74 7261 6365 737d      f"({ntraces}
-0000f690: 292e 2042 6520 6361 7265 6675 6c20 7769  ). Be careful wi
-0000f6a0: 7468 2079 6f75 7220 5241 4d20 7573 6167  th your RAM usag
-0000f6b0: 652e 220a 2020 2020 2020 2020 2020 2020  e.".            
-0000f6c0: 290a 0a20 2020 2069 6e64 7320 3d20 6e70  )..    inds = np
-0000f6d0: 2e72 616e 646f 6d2e 6368 6f69 6365 280a  .random.choice(.
-0000f6e0: 2020 2020 2020 2020 6e70 2e66 6c61 746e          np.flatn
-0000f6f0: 6f6e 7a65 726f 2863 7574 292c 0a20 2020  onzero(cut),.   
-0000f700: 2020 2020 2073 697a 653d 6e74 7261 6365       size=ntrace
-0000f710: 732c 0a20 2020 2020 2020 2072 6570 6c61  s,.        repla
-0000f720: 6365 3d46 616c 7365 2c0a 2020 2020 290a  ce=False,.    ).
-0000f730: 0a20 2020 2063 7261 6e64 203d 206e 702e  .    crand = np.
-0000f740: 7a65 726f 7328 6c65 6e28 6576 746e 756d  zeros(len(evtnum
-0000f750: 7329 2c20 6474 7970 653d 626f 6f6c 290a  s), dtype=bool).
-0000f760: 2020 2020 6372 616e 645b 696e 6473 5d20      crand[inds] 
-0000f770: 3d20 5472 7565 0a0a 2020 2020 6835 5f72  = True..    h5_r
-0000f780: 6561 6465 7220 3d20 4835 5265 6164 6572  eader = H5Reader
-0000f790: 2829 0a0a 2020 2020 6669 7273 745f 6669  ()..    first_fi
-0000f7a0: 6c65 203d 2073 6f72 7465 6428 676c 6f62  le = sorted(glob
-0000f7b0: 2866 277b 6261 7365 7061 7468 7d2f 2a2a  (f'{basepath}/**
-0000f7c0: 2f2a 2e68 6466 3527 2c20 7265 6375 7273  /*.hdf5', recurs
-0000f7d0: 6976 653d 5472 7565 2929 5b30 5d0a 0a20  ive=True))[0].. 
-0000f7e0: 2020 2069 6620 6368 616e 6e65 6c73 2069     if channels i
-0000f7f0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000f800: 636f 6e6e 6563 7469 6f6e 5f64 6963 7420  connection_dict 
-0000f810: 3d20 6835 5f72 6561 6465 722e 6765 745f  = h5_reader.get_
-0000f820: 636f 6e6e 6563 7469 6f6e 5f64 6963 7428  connection_dict(
-0000f830: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-0000f840: 655f 6e61 6d65 3d66 6972 7374 5f66 696c  e_name=first_fil
-0000f850: 652c 0a20 2020 2020 2020 2029 0a20 2020  e,.        ).   
-0000f860: 2020 2020 2063 6861 6e6e 656c 7320 3d20       channels = 
-0000f870: 636f 6e6e 6563 7469 6f6e 5f64 6963 745b  connection_dict[
-0000f880: 2764 6574 6563 746f 725f 6368 616e 7327  'detector_chans'
-0000f890: 5d0a 0a20 2020 2066 735f 6c69 7374 203d  ]..    fs_list =
-0000f8a0: 205b 5d0a 2020 2020 6d65 7461 6461 7461   [].    metadata
-0000f8b0: 203d 2068 355f 7265 6164 6572 2e67 6574   = h5_reader.get
-0000f8c0: 5f6d 6574 6164 6174 6128 6669 6c65 5f6e  _metadata(file_n
-0000f8d0: 616d 653d 6669 7273 745f 6669 6c65 290a  ame=first_file).
-0000f8e0: 2020 2020 666f 7220 6c61 6265 6c20 696e      for label in
-0000f8f0: 206d 6574 6164 6174 615b 2767 726f 7570   metadata['group
-0000f900: 5f6c 6973 7427 5d3a 0a20 2020 2020 2020  _list']:.       
-0000f910: 2066 735f 6c69 7374 2e61 7070 656e 6428   fs_list.append(
-0000f920: 6d65 7461 6461 7461 5b27 6772 6f75 7073  metadata['groups
-0000f930: 275d 5b6c 6162 656c 5d2e 6765 7428 2773  '][label].get('s
-0000f940: 616d 706c 655f 7261 7465 2729 290a 0a20  ample_rate')).. 
-0000f950: 2020 2066 7320 3d20 6e70 2e75 6e69 7175     fs = np.uniqu
-0000f960: 6528 6c69 7374 2866 696c 7465 7228 4e6f  e(list(filter(No
-0000f970: 6e65 2c20 6673 5f6c 6973 7429 2929 5b30  ne, fs_list)))[0
-0000f980: 5d0a 0a20 2020 2061 7272 2c20 6d65 7461  ]..    arr, meta
-0000f990: 6461 7461 203d 2068 355f 7265 6164 6572  data = h5_reader
-0000f9a0: 2e72 6561 645f 6d61 6e79 5f65 7665 6e74  .read_many_event
-0000f9b0: 7328 0a20 2020 2020 2020 2066 696c 6570  s(.        filep
-0000f9c0: 6174 683d 676c 6f62 2866 277b 6261 7365  ath=glob(f'{base
-0000f9d0: 7061 7468 7d2f 2a27 292c 0a20 2020 2020  path}/*'),.     
-0000f9e0: 2020 2065 7665 6e74 5f6e 756d 733d 6e70     event_nums=np
-0000f9f0: 2e61 7361 7272 6179 2865 7674 6e75 6d73  .asarray(evtnums
-0000fa00: 5b63 7574 2026 2063 7261 6e64 5d29 2c0a  [cut & crand]),.
-0000fa10: 2020 2020 2020 2020 7365 7269 6573 5f6e          series_n
-0000fa20: 756d 733d 6e70 2e61 7361 7272 6179 2873  ums=np.asarray(s
-0000fa30: 6572 6965 736e 756d 735b 6375 7420 2620  eriesnums[cut & 
-0000fa40: 6372 616e 645d 292c 0a20 2020 2020 2020  crand]),.       
-0000fa50: 206f 7574 7075 745f 666f 726d 6174 3d32   output_format=2
-0000fa60: 2c0a 2020 2020 2020 2020 696e 636c 7564  ,.        includ
-0000fa70: 655f 6d65 7461 6461 7461 3d54 7275 652c  e_metadata=True,
-0000fa80: 0a20 2020 2020 2020 2064 6574 6563 746f  .        detecto
-0000fa90: 725f 6368 616e 733d 6368 616e 6e65 6c73  r_chans=channels
-0000faa0: 2c0a 2020 2020 2020 2020 6164 6374 6f61  ,.        adctoa
-0000fab0: 6d70 3d54 7275 652c 0a20 2020 2029 0a0a  mp=True,.    )..
-0000fac0: 2020 2020 6966 2063 6861 6e6e 656c 7320      if channels 
-0000fad0: 213d 206d 6574 6164 6174 615b 305d 5b27  != metadata[0]['
-0000fae0: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
-0000faf0: 3a0a 2020 2020 2020 2020 6368 616e 7320  :.        chans 
-0000fb00: 3d20 5b6d 6574 6164 6174 615b 305d 5b27  = [metadata[0]['
-0000fb10: 6465 7465 6374 6f72 5f63 6861 6e73 275d  detector_chans']
-0000fb20: 2e69 6e64 6578 2863 6829 2066 6f72 2063  .index(ch) for c
-0000fb30: 6820 696e 2063 6861 6e6e 656c 735d 0a20  h in channels]. 
-0000fb40: 2020 2020 2020 2078 203d 2061 7272 5b3a         x = arr[:
-0000fb50: 2c20 6368 616e 735d 2e61 7374 7970 6528  , chans].astype(
-0000fb60: 666c 6f61 7429 0a20 2020 2065 6c73 653a  float).    else:
-0000fb70: 0a20 2020 2020 2020 2078 203d 2061 7272  .        x = arr
-0000fb80: 2e61 7374 7970 6528 666c 6f61 7429 0a0a  .astype(float)..
-0000fb90: 2020 2020 7420 3d20 6e70 2e61 7261 6e67      t = np.arang
-0000fba0: 6528 782e 7368 6170 655b 2d31 5d29 2f66  e(x.shape[-1])/f
-0000fbb0: 730a 0a20 2020 2069 6620 6c67 6370 6c6f  s..    if lgcplo
-0000fbc0: 743a 0a20 2020 2020 2020 2069 6620 6e70  t:.        if np
-0000fbd0: 6c6f 743e 6e74 7261 6365 733a 0a20 2020  lot>ntraces:.   
-0000fbe0: 2020 2020 2020 2020 206e 706c 6f74 203d           nplot =
-0000fbf0: 206e 7472 6163 6573 0a0a 2020 2020 2020   ntraces..      
-0000fc00: 2020 666f 7220 6969 2069 6e20 7261 6e67    for ii in rang
-0000fc10: 6528 6e70 6c6f 7429 3a0a 0a20 2020 2020  e(nplot):..     
-0000fc20: 2020 2020 2020 2066 6967 2c20 6178 203d         fig, ax =
-0000fc30: 2070 6c74 2e73 7562 706c 6f74 7328 6669   plt.subplots(fi
-0000fc40: 6773 697a 653d 2831 302c 2036 2929 0a20  gsize=(10, 6)). 
-0000fc50: 2020 2020 2020 2020 2020 2069 6620 7375             if su
-0000fc60: 6d63 6861 6e73 3a0a 2020 2020 2020 2020  mchans:.        
-0000fc70: 2020 2020 2020 2020 7472 6163 655f 7375          trace_su
-0000fc80: 6d20 3d20 785b 6969 5d2e 7375 6d28 6178  m = x[ii].sum(ax
-0000fc90: 6973 3d30 290a 0a20 2020 2020 2020 2020  is=0)..         
-0000fca0: 2020 2020 2020 2069 6620 696e 6462 6173         if indbas
-0000fcb0: 6570 7265 2069 7320 6e6f 7420 4e6f 6e65  epre is not None
-0000fcc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fcd0: 2020 2020 2020 6261 7365 6c69 6e65 203d        baseline =
-0000fce0: 206e 702e 6d65 616e 2874 7261 6365 5f73   np.mean(trace_s
-0000fcf0: 756d 5b2e 2e2e 2c20 3a69 6e64 6261 7365  um[..., :indbase
-0000fd00: 7072 655d 290a 2020 2020 2020 2020 2020  pre]).          
-0000fd10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd30: 6261 7365 6c69 6e65 203d 2030 0a0a 2020  baseline = 0..  
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-0000fd50: 2e70 6c6f 7428 7420 2a20 3165 362c 2074  .plot(t * 1e6, t
-0000fd60: 7261 6365 5f73 756d 202a 2031 6536 2c20  race_sum * 1e6, 
-0000fd70: 6c61 6265 6c3d 2253 756d 6d65 6420 4368  label="Summed Ch
-0000fd80: 616e 6e65 6c73 2229 0a20 2020 2020 2020  annels").       
-0000fd90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000fda0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-0000fdb0: 7320 3d20 706c 742e 636d 2e76 6972 6964  s = plt.cm.virid
-0000fdc0: 6973 280a 2020 2020 2020 2020 2020 2020  is(.            
-0000fdd0: 2020 2020 2020 2020 6e70 2e6c 696e 7370          np.linsp
-0000fde0: 6163 6528 302c 2031 2c20 6e75 6d3d 782e  ace(0, 1, num=x.
-0000fdf0: 7368 6170 655b 315d 292c 0a20 2020 2020  shape[1]),.     
-0000fe00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000fe10: 6c70 6861 3d30 2e35 2c0a 2020 2020 2020  lpha=0.5,.      
-0000fe20: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000fe30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000fe40: 6a6a 2c20 6368 616e 2069 6e20 656e 756d  jj, chan in enum
-0000fe50: 6572 6174 6528 6368 616e 6e65 6c73 293a  erate(channels):
-0000fe60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fe70: 2020 2020 206c 6162 656c 203d 2066 2243       label = f"C
-0000fe80: 6861 6e6e 656c 207b 6368 616e 7d22 0a0a  hannel {chan}"..
-0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fea0: 2020 2020 6966 2069 6e64 6261 7365 7072      if indbasepr
-0000feb0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-0000fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fed0: 2020 2020 2020 2062 6173 656c 696e 6520         baseline 
-0000fee0: 3d20 6e70 2e6d 6561 6e28 785b 6969 2c20  = np.mean(x[ii, 
-0000fef0: 6a6a 2c20 3a69 6e64 6261 7365 7072 655d  jj, :indbasepre]
-0000ff00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ff10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff30: 2020 2020 6261 7365 6c69 6e65 203d 2030      baseline = 0
-0000ff40: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ff50: 2020 2020 2020 6178 2e70 6c6f 7428 0a20        ax.plot(. 
-0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff70: 2020 2020 2020 2074 202a 2031 6536 2c0a         t * 1e6,.
-0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff90: 2020 2020 2020 2020 785b 6969 2c20 6a6a          x[ii, jj
-0000ffa0: 5d20 2a20 3165 3620 2d20 6261 7365 6c69  ] * 1e6 - baseli
-0000ffb0: 6e65 202a 2031 6536 2c0a 2020 2020 2020  ne * 1e6,.      
-0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffd0: 2020 636f 6c6f 723d 636f 6c6f 7273 5b6a    color=colors[j
-0000ffe0: 6a5d 2c0a 2020 2020 2020 2020 2020 2020  j],.            
-0000fff0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
-00010000: 6c3d 6c61 6265 6c2c 0a20 2020 2020 2020  l=label,.       
-00010010: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00010020: 2020 2020 2020 2020 2020 2061 782e 6772             ax.gr
-00010030: 6964 2829 0a20 2020 2020 2020 2020 2020  id().           
-00010040: 2061 782e 7365 745f 796c 6162 656c 2822   ax.set_ylabel("
-00010050: 4375 7272 656e 7420 5bce bc41 5d22 290a  Current [..A]").
-00010060: 2020 2020 2020 2020 2020 2020 6178 2e73              ax.s
-00010070: 6574 5f78 6c61 6265 6c28 2254 696d 6520  et_xlabel("Time 
-00010080: 5bce bc73 5d22 290a 2020 2020 2020 2020  [..s]").        
-00010090: 2020 2020 6178 2e73 6574 5f74 6974 6c65      ax.set_title
-000100a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000100b0: 2020 6622 5075 6c73 6573 2c20 4576 7420    f"Pulses, Evt 
-000100c0: 4e75 6d20 7b65 7674 6e75 6d73 5b63 7261  Num {evtnums[cra
-000100d0: 6e64 5d2e 696c 6f63 5b69 695d 7d2c 2022  nd].iloc[ii]}, "
-000100e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000100f0: 2066 2253 6572 6965 7320 4e75 6d20 7b73   f"Series Num {s
-00010100: 6572 6965 736e 756d 735b 6372 616e 645d  eriesnums[crand]
-00010110: 2e69 6c6f 635b 6969 5d7d 220a 2020 2020  .iloc[ii]}".    
-00010120: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00010130: 2020 2020 2020 6178 2e6c 6567 656e 6428        ax.legend(
-00010140: 290a 0a20 2020 2072 6574 7572 6e20 742c  )..    return t,
-00010150: 2078 2c20 6372 616e 640a 2020 0a          x, crand.  .
+0000c580: 2020 2020 2020 2b20 2774 7269 6767 6572        + 'trigger
+0000c590: 2069 6e64 6578 2077 6974 686f 7574 2074   index without t
+0000c5a0: 7261 6365 206c 656e 6774 682e 2027 0a20  race length. '. 
+0000c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5c0: 2020 2020 202b 2027 5265 7475 726e 696e       + 'Returnin
+0000c5d0: 6720 6675 6c6c 2074 7261 6365 2127 290a  g full trace!').
+0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5f0: 7472 6967 6765 725f 696e 6465 7820 3d20  trigger_index = 
+0000c600: 4e6f 6e65 0a20 2020 2020 2020 2065 6c73  None.        els
+0000c610: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+0000c620: 6620 2874 7261 6365 5f6c 656e 6774 685f  f (trace_length_
+0000c630: 6d73 6563 2069 7320 6e6f 7420 4e6f 6e65  msec is not None
+0000c640: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000c650: 2020 6f72 2020 7472 6163 655f 6c65 6e67    or  trace_leng
+0000c660: 7468 5f73 616d 706c 6573 2069 7320 6e6f  th_samples is no
+0000c670: 7420 4e6f 6e65 293a 0a20 2020 2020 2020  t None):.       
+0000c680: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000c690: 2827 5741 524e 494e 473a 2055 6e61 626c  ('WARNING: Unabl
+0000c6a0: 6520 746f 2075 7365 2074 7261 6365 206c  e to use trace l
+0000c6b0: 656e 6768 7420 6172 6775 6d65 6e74 270a  enght argument'.
+0000c6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6d0: 2020 2020 2020 2020 2b20 2720 7769 7468          + ' with
+0000c6e0: 6f75 7420 7472 6967 6765 7220 696e 666f  out trigger info
+0000c6f0: 2e20 270a 2020 2020 2020 2020 2020 2020  . '.            
+0000c700: 2020 2020 2020 2020 2020 2020 2b20 2752              + 'R
+0000c710: 6574 7572 6e69 6e67 2066 756c 6c20 7472  eturning full tr
+0000c720: 6163 6521 2729 0a0a 2020 2020 2020 2020  ace!')..        
+0000c730: 2320 6578 7472 6163 7420 7472 6967 6765  # extract trigge
+0000c740: 720a 2020 2020 2020 2020 6966 2074 7269  r.        if tri
+0000c750: 6767 6572 5f69 6e64 6578 2069 7320 6e6f  gger_index is no
+0000c760: 7420 4e6f 6e65 3a0a 0a20 2020 2020 2020  t None:..       
+0000c770: 2020 2020 2074 7269 6767 6572 5f69 6e64       trigger_ind
+0000c780: 6578 203d 2069 6e74 2874 7269 6767 6572  ex = int(trigger
+0000c790: 5f69 6e64 6578 290a 2020 2020 0a20 2020  _index).    .   
+0000c7a0: 2020 2020 2020 2020 2023 206e 756d 6265           # numbe
+0000c7b0: 7220 7361 6d70 6c65 730a 2020 2020 2020  r samples.      
+0000c7c0: 2020 2020 2020 6e62 5f73 616d 706c 6573        nb_samples
+0000c7d0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000c7e0: 2020 2020 6673 203d 2069 6e66 6f5b 2773      fs = info['s
+0000c7f0: 616d 706c 655f 7261 7465 275d 0a20 2020  ample_rate'].   
+0000c800: 2020 2020 2020 2020 2069 6620 7472 6163           if trac
+0000c810: 655f 6c65 6e67 7468 5f73 616d 706c 6573  e_length_samples
+0000c820: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000c830: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
+0000c840: 5f73 616d 706c 6573 203d 2074 7261 6365  _samples = trace
+0000c850: 5f6c 656e 6774 685f 7361 6d70 6c65 730a  _length_samples.
+0000c860: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000c870: 2074 7261 6365 5f6c 656e 6774 685f 6d73   trace_length_ms
+0000c880: 6563 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ec is not None:.
+0000c890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8a0: 6e62 5f73 616d 706c 6573 203d 2069 6e74  nb_samples = int
+0000c8b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000c8c0: 2020 2020 2020 6673 2a74 7261 6365 5f6c        fs*trace_l
+0000c8d0: 656e 6774 685f 6d73 6563 2f31 3030 300a  ength_msec/1000.
+0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8f0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000c900: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000c910: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000c920: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000c930: 2020 2020 2020 2020 2020 2745 5252 4f52            'ERROR
+0000c940: 3a20 4e75 6d62 6572 206f 6620 7361 6d70  : Number of samp
+0000c950: 6c65 7320 7265 7175 6972 6564 2074 6f20  les required to 
+0000c960: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000c970: 2020 2020 2020 2b20 2765 7874 7261 6374        + 'extract
+0000c980: 2074 7261 6365 270a 2020 2020 2020 2020   trace'.        
+0000c990: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000c9a0: 2020 2020 2020 2023 2070 7265 2d74 7269         # pre-tri
+0000c9b0: 6767 6572 0a20 2020 2020 2020 2020 2020  gger.           
+0000c9c0: 206e 625f 7072 6574 7269 6767 6572 5f73   nb_pretrigger_s
+0000c9d0: 616d 706c 6573 203d 2069 6e74 286e 625f  amples = int(nb_
+0000c9e0: 7361 6d70 6c65 732f 3229 0a20 2020 2020  samples/2).     
+0000c9f0: 2020 2020 2020 2069 6620 7072 6574 7269         if pretri
+0000ca00: 6767 6572 5f6c 656e 6774 685f 7361 6d70  gger_length_samp
+0000ca10: 6c65 7320 6973 206e 6f74 204e 6f6e 653a  les is not None:
+0000ca20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ca30: 206e 625f 7072 6574 7269 6767 6572 5f73   nb_pretrigger_s
+0000ca40: 616d 706c 6573 203d 2070 7265 7472 6967  amples = pretrig
+0000ca50: 6765 725f 6c65 6e67 7468 5f73 616d 706c  ger_length_sampl
+0000ca60: 6573 0a20 2020 2020 2020 2020 2020 2065  es.            e
+0000ca70: 6c69 6620 7072 6574 7269 6767 6572 5f6c  lif pretrigger_l
+0000ca80: 656e 6774 685f 6d73 6563 2069 7320 6e6f  ength_msec is no
+0000ca90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000caa0: 2020 2020 2020 2020 6e62 5f70 7265 7472          nb_pretr
+0000cab0: 6967 6765 725f 7361 6d70 6c65 7320 3d20  igger_samples = 
+0000cac0: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+0000cad0: 2020 2020 2020 2020 2066 732a 7072 6574           fs*pret
+0000cae0: 7269 6767 6572 5f6c 656e 6774 685f 6d73  rigger_length_ms
+0000caf0: 6563 2f31 3030 300a 2020 2020 2020 2020  ec/1000.        
+0000cb00: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000cb10: 2020 2020 2020 2023 206d 696e 2f6d 6178         # min/max
+0000cb20: 2069 6e64 6578 0a20 2020 2020 2020 2020   index.         
+0000cb30: 2020 2074 7261 6365 5f6d 696e 5f69 6e64     trace_min_ind
+0000cb40: 6578 203d 2069 6e74 2874 7269 6767 6572  ex = int(trigger
+0000cb50: 5f69 6e64 6578 202d 206e 625f 7072 6574  _index - nb_pret
+0000cb60: 7269 6767 6572 5f73 616d 706c 6573 290a  rigger_samples).
+0000cb70: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+0000cb80: 655f 6d61 785f 696e 6465 7820 3d20 696e  e_max_index = in
+0000cb90: 7428 7472 6163 655f 6d69 6e5f 696e 6465  t(trace_min_inde
+0000cba0: 7820 2b20 6e62 5f73 616d 706c 6573 290a  x + nb_samples).
+0000cbb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000cbc0: 2874 7261 6365 5f6d 696e 5f69 6e64 6578  (trace_min_index
+0000cbd0: 3c30 0a20 2020 2020 2020 2020 2020 2020  <0.             
+0000cbe0: 2020 206f 7220 7472 6163 655f 6d61 785f     or trace_max_
+0000cbf0: 696e 6465 783e 6461 7461 7365 745f 6469  index>dataset_di
+0000cc00: 6d73 5b31 5d29 3a0a 2020 2020 2020 2020  ms[1]):.        
+0000cc10: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0000cc20: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+0000cc30: 2020 2020 2020 2020 2020 2020 2020 2745                'E
+0000cc40: 5252 4f52 3a20 556e 6162 6c65 2074 6f20  RROR: Unable to 
+0000cc50: 6578 7472 6163 7420 7472 6967 6765 722e  extract trigger.
+0000cc60: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
+0000cc70: 2020 2020 2020 202b 2027 2054 7261 6365         + ' Trace
+0000cc80: 206c 656e 6774 6820 746f 6f20 6c6f 6e67   length too long
+0000cc90: 2127 290a 2020 2020 2020 2020 2020 2020  !').            
+0000cca0: 0a0a 0a20 2020 2020 2020 2023 203d 3d3d  ...        # ===
+0000ccb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ccc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ccd0: 0a20 2020 2020 2020 2023 2045 7874 7261  .        # Extra
+0000cce0: 6374 2074 7261 6365 0a20 2020 2020 2020  ct trace.       
+0000ccf0: 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   # =============
+0000cd00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000cd10: 3d3d 3d3d 3d3d 0a0a 0a20 2020 2020 2020  ======...       
+0000cd20: 2023 2069 6e69 7469 616c 697a 6520 656d   # initialize em
+0000cd30: 7074 7920 7472 6163 650a 2020 2020 2020  pty trace.      
+0000cd40: 2020 736c 6963 655f 7361 6d70 6c65 7320    slice_samples 
+0000cd50: 3d20 4e6f 6e65 0a20 2020 2020 2020 2064  = None.        d
+0000cd60: 696d 5f30 203d 206c 656e 2873 656c 6563  im_0 = len(selec
+0000cd70: 7465 645f 6172 7261 795f 696e 6469 6365  ted_array_indice
+0000cd80: 7329 0a20 2020 2020 2020 2064 696d 5f31  s).        dim_1
+0000cd90: 203d 2064 6174 6173 6574 5f64 696d 735b   = dataset_dims[
+0000cda0: 315d 0a20 2020 2020 2020 200a 2020 2020  1].        .    
+0000cdb0: 2020 2020 6966 2028 7472 6163 655f 6d69      if (trace_mi
+0000cdc0: 6e5f 696e 6465 7820 6973 206e 6f74 204e  n_index is not N
+0000cdd0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000cde0: 616e 6420 7472 6163 655f 6d61 785f 696e  and trace_max_in
+0000cdf0: 6465 7820 6973 206e 6f74 204e 6f6e 6529  dex is not None)
+0000ce00: 3a0a 2020 2020 2020 2020 2020 2020 6469  :.            di
+0000ce10: 6d5f 3120 3d20 7472 6163 655f 6d61 785f  m_1 = trace_max_
+0000ce20: 696e 6465 782d 7472 6163 655f 6d69 6e5f  index-trace_min_
+0000ce30: 696e 6465 780a 2020 2020 2020 2020 2020  index.          
+0000ce40: 2020 736c 6963 655f 7361 6d70 6c65 7320    slice_samples 
+0000ce50: 3d20 736c 6963 6528 7472 6163 655f 6d69  = slice(trace_mi
+0000ce60: 6e5f 696e 6465 782c 2074 7261 6365 5f6d  n_index, trace_m
+0000ce70: 6178 5f69 6e64 6578 290a 2020 2020 2020  ax_index).      
+0000ce80: 2020 2020 2020 0a20 2020 2020 2020 2074        .        t
+0000ce90: 7261 6365 735f 696e 7420 3d20 6e70 2e65  races_int = np.e
+0000cea0: 6d70 7479 2828 6469 6d5f 302c 2064 696d  mpty((dim_0, dim
+0000ceb0: 5f31 292c 2064 7479 7065 3d64 6174 6173  _1), dtype=datas
+0000cec0: 6574 2e64 7479 7065 290a 2020 2020 2020  et.dtype).      
+0000ced0: 2020 0a20 2020 2020 2020 2023 2052 6561    .        # Rea
+0000cee0: 6420 7468 6520 706f 7274 696f 6e20 6f66  d the portion of
+0000cef0: 2074 6865 2061 7272 6179 2075 7369 6e67   the array using
+0000cf00: 2072 6561 645f 6469 7265 6374 0a20 2020   read_direct.   
+0000cf10: 2020 2020 2066 6f72 2069 2c20 696e 6465       for i, inde
+0000cf20: 7820 696e 2065 6e75 6d65 7261 7465 2873  x in enumerate(s
+0000cf30: 656c 6563 7465 645f 6172 7261 795f 696e  elected_array_in
+0000cf40: 6469 6365 7329 3a0a 2020 2020 2020 2020  dices):.        
+0000cf50: 2020 2020 6966 2020 736c 6963 655f 7361      if  slice_sa
+0000cf60: 6d70 6c65 7320 6973 206e 6f74 204e 6f6e  mples is not Non
+0000cf70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000cf80: 2020 2064 6174 6173 6574 2e72 6561 645f     dataset.read_
+0000cf90: 6469 7265 6374 2874 7261 6365 735f 696e  direct(traces_in
+0000cfa0: 745b 695d 2c0a 2020 2020 2020 2020 2020  t[i],.          
+0000cfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfc0: 2020 2020 2020 2020 2020 6e70 2e73 5f5b            np.s_[
+0000cfd0: 696e 6465 782c 2073 6c69 6365 5f73 616d  index, slice_sam
+0000cfe0: 706c 6573 5d29 0a20 2020 2020 2020 2020  ples]).         
+0000cff0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000d000: 2020 2020 2020 2020 2064 6174 6173 6574           dataset
+0000d010: 2e72 6561 645f 6469 7265 6374 2874 7261  .read_direct(tra
+0000d020: 6365 735f 696e 745b 695d 2c20 6e70 2e73  ces_int[i], np.s
+0000d030: 5f5b 696e 6465 785d 290a 2020 2020 2020  _[index]).      
+0000d040: 2020 0a20 2020 2020 2020 200a 2020 2020    .        .    
+0000d050: 2020 2020 2320 636f 6e76 6572 7420 746f      # convert to
+0000d060: 2076 6f6c 742f 616d 7073 0a20 2020 2020   volt/amps.     
+0000d070: 2020 2074 7261 6365 7320 3d20 5b5d 0a20     traces = []. 
+0000d080: 2020 2020 2020 2069 6620 6164 6374 6f76         if adctov
+0000d090: 6f6c 7420 6f72 2061 6463 746f 616d 703a  olt or adctoamp:
+0000d0a0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000d0b0: 696e 6974 6961 6c69 7a65 0a20 2020 2020  initialize.     
+0000d0c0: 2020 2020 2020 2074 7261 6365 7320 3d20         traces = 
+0000d0d0: 6e70 2e7a 6572 6f73 5f6c 696b 6528 7472  np.zeros_like(tr
+0000d0e0: 6163 6573 5f69 6e74 2c20 6474 7970 653d  aces_int, dtype=
+0000d0f0: 6e70 2e66 6c6f 6174 3634 290a 0a20 2020  np.float64)..   
+0000d100: 2020 2020 2020 2020 2023 2063 6f6e 7665           # conve
+0000d110: 7274 2074 6f20 766f 6c74 730a 2020 2020  rt to volts.    
+0000d120: 2020 2020 2020 2020 666f 7220 6963 6861          for icha
+0000d130: 6e20 696e 2072 616e 6765 2874 7261 6365  n in range(trace
+0000d140: 735f 696e 742e 7368 6170 655b 305d 293a  s_int.shape[0]):
+0000d150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d160: 2063 616c 5f63 6f65 6666 203d 2069 6e66   cal_coeff = inf
+0000d170: 6f5b 2761 6463 5f63 6f6e 7665 7273 696f  o['adc_conversio
+0000d180: 6e5f 6661 6374 6f72 275d 5b69 6368 616e  n_factor'][ichan
+0000d190: 5d5b 3a3a 2d31 5d0a 2020 2020 2020 2020  ][::-1].        
+0000d1a0: 2020 2020 2020 2020 706f 6c79 203d 206e          poly = n
+0000d1b0: 702e 706f 6c79 3164 2863 616c 5f63 6f65  p.poly1d(cal_coe
+0000d1c0: 6666 290a 2020 2020 2020 2020 2020 2020  ff).            
+0000d1d0: 2020 2020 7472 6163 6573 5b69 6368 616e      traces[ichan
+0000d1e0: 2c3a 5d20 3d20 706f 6c79 2874 7261 6365  ,:] = poly(trace
+0000d1f0: 735f 696e 745b 6963 6861 6e2c 3a5d 290a  s_int[ichan,:]).
+0000d200: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+0000d210: 6f6e 7665 7274 2074 6f20 616d 7073 0a20  onvert to amps. 
+0000d220: 2020 2020 2020 2020 2020 2069 6620 6164             if ad
+0000d230: 6374 6f61 6d70 3a0a 2020 2020 2020 2020  ctoamp:.        
+0000d240: 2020 2020 2020 2020 6966 2064 6574 6563          if detec
+0000d250: 746f 725f 636f 6e66 6967 2069 7320 4e6f  tor_config is No
+0000d260: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000d270: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0000d280: 6c75 6545 7272 6f72 2827 4552 524f 523a  lueError('ERROR:
+0000d290: 2055 6e61 626c 6520 746f 2063 6f6e 7665   Unable to conve
+0000d2a0: 7274 2074 6f20 616d 7073 2e20 270a 2020  rt to amps. '.  
+0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2d0: 2020 202b 2027 4e6f 2064 6574 6563 746f     + 'No detecto
+0000d2e0: 7220 636f 6e66 6967 2061 7661 696c 6162  r config availab
+0000d2f0: 6c65 2127 290a 2020 2020 2020 2020 2020  le!').          
+0000d300: 2020 2020 2020 666f 7220 6963 6861 6e20        for ichan 
+0000d310: 696e 2072 616e 6765 2874 7261 6365 732e  in range(traces.
+0000d320: 7368 6170 655b 305d 293a 0a20 2020 2020  shape[0]):.     
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000d340: 6574 203d 2069 6e66 6f5b 2764 6574 6563  et = info['detec
+0000d350: 746f 725f 6368 616e 7327 5d5b 6963 6861  tor_chans'][icha
+0000d360: 6e5d 0a20 2020 2020 2020 2020 2020 2020  n].             
+0000d370: 2020 2020 2020 2069 6620 2763 6c6f 7365         if 'close
+0000d380: 5f6c 6f6f 705f 6e6f 726d 2720 696e 2064  _loop_norm' in d
+0000d390: 6574 6563 746f 725f 636f 6e66 6967 5b64  etector_config[d
+0000d3a0: 6574 5d3a 0a20 2020 2020 2020 2020 2020  et]:.           
+0000d3b0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+0000d3c0: 6365 735b 6963 6861 6e2c 3a5d 203d 2074  ces[ichan,:] = t
+0000d3d0: 7261 6365 735b 6963 6861 6e2c 3a5d 2f64  races[ichan,:]/d
+0000d3e0: 6574 6563 746f 725f 636f 6e66 6967 5b64  etector_config[d
+0000d3f0: 6574 5d5b 2763 6c6f 7365 5f6c 6f6f 705f  et]['close_loop_
+0000d400: 6e6f 726d 275d 0a20 2020 2020 2020 2020  norm'].         
+0000d410: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000d420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d430: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000d440: 616c 7565 4572 726f 7228 2745 5252 4f52  alueError('ERROR
+0000d450: 3a20 556e 6162 6c65 2074 6f20 636f 6e76  : Unable to conv
+0000d460: 6572 7420 746f 2061 6d70 732e 2027 0a20  ert to amps. '. 
+0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d490: 2020 2020 2020 2020 2b20 274e 6f20 6e6f          + 'No no
+0000d4a0: 726d 616c 697a 6174 696f 6e20 6176 6169  rmalization avai
+0000d4b0: 6c61 626c 6520 666f 7220 2720 2b20 6465  lable for ' + de
+0000d4c0: 7429 2020 2020 2020 0a20 2020 2020 2020  t)      .       
+0000d4d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d4e0: 2020 2074 7261 6365 7320 3d20 7472 6163     traces = trac
+0000d4f0: 6573 5f69 6e74 0a20 2020 2020 2020 2020  es_int.         
+0000d500: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0000d510: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000d520: 2023 2062 6173 656c 696e 6520 7375 6274   # baseline subt
+0000d530: 7261 6374 0a20 2020 2020 2020 2069 6620  ract.        if 
+0000d540: 6261 7365 6c69 6e65 7375 623a 0a20 2020  baselinesub:.   
+0000d550: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+0000d560: 2020 2020 2020 2320 6669 6e64 2062 6173        # find bas
+0000d570: 656c 696e 6520 7374 6172 742f 7374 6f70  eline start/stop
+0000d580: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+0000d590: 656c 696e 655f 7374 6172 7420 3d20 4e6f  eline_start = No
+0000d5a0: 6e65 0a20 2020 2020 2020 2020 2020 2062  ne.            b
+0000d5b0: 6173 656c 696e 655f 7374 6f70 203d 204e  aseline_stop = N
+0000d5c0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000d5d0: 6966 2062 6173 656c 696e 6569 6e64 7320  if baselineinds 
+0000d5e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000d5f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d600: 6c65 6e28 6261 7365 6c69 6e65 696e 6473  len(baselineinds
+0000d610: 2921 3d32 3a0a 2020 2020 2020 2020 2020  )!=2:.          
+0000d620: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000d630: 5661 6c75 6545 7272 6f72 2827 4552 524f  ValueError('ERRO
+0000d640: 523a 2062 6173 656c 696e 6569 6e64 7320  R: baselineinds 
+0000d650: 7368 6f75 6c64 2062 6520 6c69 7374 2f74  should be list/t
+0000d660: 7570 6c65 206f 6620 6c65 6e67 7468 2032  uple of length 2
+0000d670: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+0000d680: 2020 2062 6173 656c 696e 655f 7374 6172     baseline_star
+0000d690: 7420 3d20 6261 7365 6c69 6e65 696e 6473  t = baselineinds
+0000d6a0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+0000d6b0: 2020 2020 6261 7365 6c69 6e65 5f73 746f      baseline_sto
+0000d6c0: 7020 3d20 2062 6173 656c 696e 6569 6e64  p =  baselineind
+0000d6d0: 735b 315d 0a20 2020 2020 2020 2020 2020  s[1].           
+0000d6e0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+0000d6f0: 2020 656c 6966 2027 6e62 5f73 616d 706c    elif 'nb_sampl
+0000d700: 6573 5f70 7265 7472 6967 6765 7227 2069  es_pretrigger' i
+0000d710: 6e20 696e 666f 3a0a 2020 2020 2020 2020  n info:.        
+0000d720: 2020 2020 2020 2020 6261 7365 6c69 6e65          baseline
+0000d730: 5f73 7461 7274 203d 2031 300a 2020 2020  _start = 10.    
+0000d740: 2020 2020 2020 2020 2020 2020 6261 7365              base
+0000d750: 6c69 6e65 5f73 746f 7020 3d20 696e 7428  line_stop = int(
+0000d760: 726f 756e 6428 696e 666f 5b27 6e62 5f73  round(info['nb_s
+0000d770: 616d 706c 6573 5f70 7265 7472 6967 6765  amples_pretrigge
+0000d780: 7227 5d2a 302e 3829 290a 0a20 2020 2020  r']*0.8))..     
+0000d790: 2020 2020 2020 2069 6620 2862 6173 656c         if (basel
+0000d7a0: 696e 655f 7374 6172 7420 6973 204e 6f6e  ine_start is Non
+0000d7b0: 6520 6f72 2062 6173 656c 696e 655f 7374  e or baseline_st
+0000d7c0: 6f70 2069 7320 4e6f 6e65 206f 720a 2020  op is None or.  
+0000d7d0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+0000d7e0: 7365 6c69 6e65 5f73 746f 703c 3d62 6173  seline_stop<=bas
+0000d7f0: 656c 696e 655f 7374 6172 7420 6f72 2062  eline_start or b
+0000d800: 6173 656c 696e 655f 7374 6f70 3e3d 7472  aseline_stop>=tr
+0000d810: 6163 6573 2e73 6861 7065 5b31 5d29 3a0a  aces.shape[1]):.
+0000d820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d830: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000d840: 2827 4552 524f 523a 2055 6e61 626c 6520  ('ERROR: Unable 
+0000d850: 746f 2066 696e 6420 6261 7365 6c69 6e65  to find baseline
+0000d860: 2073 7461 7274 2f73 746f 702e 2027 0a20   start/stop. '. 
+0000d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d890: 2b20 2741 6464 2061 7267 756d 656e 7420  + 'Add argument 
+0000d8a0: 2262 6173 656c 696e 6569 6e64 7322 2729  "baselineinds"')
+0000d8b0: 0a0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+0000d8c0: 6163 6573 203d 2074 7261 6365 7320 2d20  aces = traces - 
+0000d8d0: 6e70 2e6d 6561 6e28 7472 6163 6573 5b3a  np.mean(traces[:
+0000d8e0: 2c62 6173 656c 696e 655f 7374 6172 743a  ,baseline_start:
+0000d8f0: 6261 7365 6c69 6e65 5f73 746f 705d 2c0a  baseline_stop],.
+0000d900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d920: 2020 2020 2020 6178 6973 3d2d 312c 206b        axis=-1, k
+0000d930: 6565 7064 696d 733d 5472 7565 290a 2020  eepdims=True).  
+0000d940: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+0000d950: 2020 200a 2020 2020 2020 2020 7265 7475     .        retu
+0000d960: 726e 2074 7261 6365 732c 2069 6e66 6f0a  rn traces, info.
+0000d970: 2020 2020 2020 2020 0a0a 0a20 2020 2064          ...    d
+0000d980: 6566 205f 6765 745f 6669 6c65 5f64 6963  ef _get_file_dic
+0000d990: 7428 7365 6c66 2c20 6669 6c65 7061 7468  t(self, filepath
+0000d9a0: 732c 2073 6572 6965 733d 4e6f 6e65 2c20  s, series=None, 
+0000d9b0: 6576 656e 745f 6c69 7374 3d4e 6f6e 6529  event_list=None)
+0000d9c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000d9d0: 2020 2020 2020 4765 7420 6120 6c69 7374        Get a list
+0000d9e0: 206f 6620 6669 6c65 7320 2866 756c 6c20   of files (full 
+0000d9f0: 7061 7468 2920 2066 726f 6d20 6469 7265  path)  from dire
+0000da00: 6374 6f72 6965 732f 6669 6c65 730a 2020  ctories/files.  
+0000da10: 2020 2020 2020 616e 6420 6669 6c74 6572        and filter
+0000da20: 2062 6173 6564 206f 6e20 6576 656e 745f   based on event_
+0000da30: 6c69 7374 0a0a 2020 2020 2020 2020 5061  list..        Pa
+0000da40: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000da50: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000da60: 2020 2020 6669 6c65 7061 7468 7320 3a20      filepaths : 
+0000da70: 7374 7220 6f72 206c 6973 740a 2020 2020  str or list.    
+0000da80: 2020 2020 2066 696c 652f 6469 7265 6374       file/direct
+0000da90: 6f72 7920 616e 642f 6f72 206c 6973 7420  ory and/or list 
+0000daa0: 6f66 2066 696c 6573 2f64 6972 6563 746f  of files/directo
+0000dab0: 7269 6573 0a0a 2020 2020 2020 2020 7365  ries..        se
+0000dac0: 7269 6573 203a 2073 7472 2f69 6e74 206f  ries : str/int o
+0000dad0: 7220 6c69 7374 2f61 7272 6179 206f 6620  r list/array of 
+0000dae0: 7374 722f 696e 740a 2020 2020 2020 2020  str/int.        
+0000daf0: 2066 696c 7465 7220 6669 6c65 206c 6973   filter file lis
+0000db00: 7420 6261 7365 6420 6f6e 2073 6572 6965  t based on serie
+0000db10: 7320 6e75 6d62 6572 2873 2920 6f72 2073  s number(s) or s
+0000db20: 6572 6965 7320 6e61 6d65 2873 290a 0a20  eries name(s).. 
+0000db30: 2020 2020 2020 2065 7665 6e74 5f6c 6973         event_lis
+0000db40: 7420 3a20 6c69 7374 2c20 6f70 7469 6f6e  t : list, option
+0000db50: 616c 0a20 2020 2020 2020 2020 206c 6973  al.          lis
+0000db60: 7420 636f 6e74 6169 6e69 6e67 2064 6963  t containing dic
+0000db70: 7469 6f6e 6172 7920 7769 7468 2065 7665  tionary with eve
+0000db80: 6e74 7320 6d65 7461 6461 7461 0a20 2020  nts metadata.   
+0000db90: 2020 2020 2020 2073 7563 6820 6173 200a         such as .
+0000dba0: 2020 2020 2020 2020 2020 2020 202d 2022               - "
+0000dbb0: 7365 7269 6573 5f6e 756d 6265 7222 0a20  series_number". 
+0000dbc0: 2020 2020 2020 2020 2020 2020 2d20 2265              - "e
+0000dbd0: 7665 6e74 5f6e 756d 6265 7222 0a20 2020  vent_number".   
+0000dbe0: 2020 2020 2020 2020 2020 2d20 2267 726f            - "gro
+0000dbf0: 7570 5f6e 616d 6522 200a 2020 2020 2020  up_name" .      
+0000dc00: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+0000dc10: 2046 696c 6520 6c69 7374 2069 7320 6669   File list is fi
+0000dc20: 6c74 6572 6564 2062 6173 6564 206f 6e20  ltered based on 
+0000dc30: 7265 7175 6573 7465 6420 6576 656e 7473  requested events
+0000dc40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000dc50: 2020 200a 0a20 2020 2020 2020 2052 6574     ..        Ret
+0000dc60: 7572 6e0a 2020 2020 2020 2020 2d2d 2d2d  urn.        ----
+0000dc70: 2d2d 0a20 2020 2020 2020 200a 2020 2020  --.        .    
+0000dc80: 2020 2020 6669 6c65 5f6c 6973 7420 3a20      file_list : 
+0000dc90: 6c69 7374 200a 2020 2020 2020 2020 2020  list .          
+0000dca0: 6c69 7374 206f 6620 6669 6c65 7320 2866  list of files (f
+0000dcb0: 756c 6c20 7061 7468 290a 0a20 2020 2020  ull path)..     
+0000dcc0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0000dcd0: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
+0000dce0: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 2020  =========.      
+0000dcf0: 2020 2320 4765 7420 6c69 7374 206f 6620    # Get list of 
+0000dd00: 6669 6c65 730a 2020 2020 2020 2020 2320  files.        # 
+0000dd10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000dd20: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2020 2020  =======..       
+0000dd30: 2023 2063 6865 636b 2069 6620 6772 6f75   # check if grou
+0000dd40: 7020 6e61 6d65 0a20 2020 2020 2020 2023  p name.        #
+0000dd50: 2061 7661 696c 6162 6c65 2069 6e20 6576   available in ev
+0000dd60: 656e 745f 6c69 7374 0a20 2020 2020 2020  ent_list.       
+0000dd70: 2067 726f 7570 5f6e 616d 6573 203d 206c   group_names = l
+0000dd80: 6973 7428 290a 2020 2020 2020 2020 6966  ist().        if
+0000dd90: 2065 7665 6e74 5f6c 6973 7420 6973 206e   event_list is n
+0000dda0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000ddb0: 2020 2020 2066 6f72 2065 7665 6e74 5f64       for event_d
+0000ddc0: 6963 7420 696e 2065 7665 6e74 5f6c 6973  ict in event_lis
+0000ddd0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0000dde0: 2020 2069 6620 2767 726f 7570 5f6e 616d     if 'group_nam
+0000ddf0: 6527 2069 6e20 6576 656e 745f 6469 6374  e' in event_dict
+0000de00: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+0000de10: 2020 2020 2020 2020 2020 2020 2067 726f               gro
+0000de20: 7570 5f6e 616d 6573 2e61 7070 656e 6428  up_names.append(
+0000de30: 7374 7228 6576 656e 745f 6469 6374 5b27  str(event_dict['
+0000de40: 6772 6f75 705f 6e61 6d65 275d 2929 0a20  group_name'])). 
+0000de50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000de60: 2320 6d61 6b65 2075 6e69 7175 650a 2020  # make unique.  
+0000de70: 2020 2020 2020 6772 6f75 705f 6e61 6d65        group_name
+0000de80: 7320 3d20 6c69 7374 2873 6574 2867 726f  s = list(set(gro
+0000de90: 7570 5f6e 616d 6573 2929 0a20 2020 2020  up_names)).     
+0000dea0: 0a20 2020 2020 2020 2023 206c 6f6f 7020  .        # loop 
+0000deb0: 6669 6c65 2f70 6174 6820 6c69 7374 2074  file/path list t
+0000dec0: 6f20 6765 7420 6c69 7374 206f 6620 6669  o get list of fi
+0000ded0: 6c65 730a 2020 2020 2020 2020 6669 6c65  les.        file
+0000dee0: 5f6c 6973 7420 203d 206c 6973 7428 290a  _list  = list().
+0000def0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0000df00: 7461 6e63 6528 6669 6c65 7061 7468 732c  tance(filepaths,
+0000df10: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+0000df20: 2020 2066 696c 6570 6174 6873 203d 205b     filepaths = [
+0000df30: 6669 6c65 7061 7468 735d 0a0a 2020 2020  filepaths]..    
+0000df40: 2020 2020 666f 7220 6669 6c65 7061 7468      for filepath
+0000df50: 2069 6e20 6669 6c65 7061 7468 733a 0a20   in filepaths:. 
+0000df60: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0000df70: 2020 2020 2020 2020 2320 6361 7365 2064          # case d
+0000df80: 6972 6563 746f 7279 0a20 2020 2020 2020  irectory.       
+0000df90: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
+0000dfa0: 6973 6469 7228 6669 6c65 7061 7468 293a  isdir(filepath):
+0000dfb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dfc0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000dfd0: 2020 7365 6172 6368 5f6c 6973 7420 3d20    search_list = 
+0000dfe0: 6c69 7374 2829 0a20 2020 2020 2020 2020  list().         
+0000dff0: 2020 2020 2020 2066 6f72 2067 726f 7570         for group
+0000e000: 5f6e 616d 6520 696e 2067 726f 7570 5f6e  _name in group_n
+0000e010: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
+0000e020: 2020 2020 2020 2020 2020 2320 6164 6420            # add 
+0000e030: 6772 6f75 7020 6e61 6d65 2074 6f20 7061  group name to pa
+0000e040: 7468 2069 6620 6e6f 740a 2020 2020 2020  th if not.      
+0000e050: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000e060: 616c 7265 6164 7920 696e 2070 6174 680a  already in path.
+0000e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e080: 2020 2020 6966 2067 726f 7570 5f6e 616d      if group_nam
+0000e090: 6520 6e6f 7420 696e 2066 696c 6570 6174  e not in filepat
+0000e0a0: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+0000e0b0: 2020 2020 2020 2020 2020 2066 696c 6570             filep
+0000e0c0: 6174 6820 3d20 2028 6669 6c65 7061 7468  ath =  (filepath
+0000e0d0: 202b 2027 2f27 0a20 2020 2020 2020 2020   + '/'.         
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0f0: 2020 2020 2020 2020 2020 2020 2b20 6772              + gr
+0000e100: 6f75 705f 6e61 6d65 290a 2020 2020 2020  oup_name).      
+0000e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e120: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
+0000e130: 2020 2020 2020 2023 2061 6464 2074 6f20         # add to 
+0000e140: 7365 6172 6368 206c 6973 740a 2020 2020  search list.    
+0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e160: 7365 6172 6368 5f73 7472 203d 2066 696c  search_str = fil
+0000e170: 6570 6174 6820 2b20 272f 2a2e 6864 6635  epath + '/*.hdf5
+0000e180: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000e190: 2020 2020 2020 6966 2073 6561 7263 685f        if search_
+0000e1a0: 7374 7220 6e6f 7420 696e 2073 6561 7263  str not in searc
+0000e1b0: 685f 6c69 7374 3a0a 2020 2020 2020 2020  h_list:.        
+0000e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1d0: 7365 6172 6368 5f6c 6973 742e 6170 7065  search_list.appe
+0000e1e0: 6e64 2873 6561 7263 685f 7374 7229 0a0a  nd(search_str)..
+0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e200: 6966 206e 6f74 2073 6561 7263 685f 6c69  if not search_li
+0000e210: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+0000e220: 2020 2020 2020 2020 7365 6172 6368 5f6c          search_l
+0000e230: 6973 7420 3d20 5b66 696c 6570 6174 6820  ist = [filepath 
+0000e240: 2b20 272f 2a2e 6864 6635 275d 0a0a 2020  + '/*.hdf5']..  
+0000e250: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000e260: 6765 7420 6669 6c65 730a 2020 2020 2020  get files.      
+0000e270: 2020 2020 2020 2020 2020 666f 7220 7365            for se
+0000e280: 6172 6368 5f73 7472 2069 6e20 7365 6172  arch_str in sear
+0000e290: 6368 5f6c 6973 743a 0a20 2020 2020 2020  ch_list:.       
+0000e2a0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0000e2b0: 655f 6c69 7374 2e65 7874 656e 6428 676c  e_list.extend(gl
+0000e2c0: 6f62 2873 6561 7263 685f 7374 7229 290a  ob(search_str)).
+0000e2d0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+0000e2e0: 6173 6520 6120 6669 6c65 0a20 2020 2020  ase a file.     
+0000e2f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000e300: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000e310: 6669 6c65 7061 7468 5b2d 343a 5d21 3d27  filepath[-4:]!='
+0000e320: 6864 6635 273a 0a20 2020 2020 2020 2020  hdf5':.         
+0000e330: 2020 2020 2020 2020 2020 2066 696c 6570             filep
+0000e340: 6174 6820 2b3d 2027 2e68 6466 3527 0a20  ath += '.hdf5'. 
+0000e350: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000e360: 6620 6f73 2e70 6174 682e 6973 6669 6c65  f os.path.isfile
+0000e370: 2866 696c 6570 6174 6829 3a0a 2020 2020  (filepath):.    
+0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e390: 6669 6c65 5f6c 6973 742e 6170 7065 6e64  file_list.append
+0000e3a0: 2866 696c 6570 6174 6829 0a0a 2020 2020  (filepath)..    
+0000e3b0: 2020 2020 6966 206e 6f74 2066 696c 655f      if not file_
+0000e3c0: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
+0000e3d0: 2020 6966 2073 656c 662e 5f72 6169 7365    if self._raise
+0000e3e0: 5f65 7272 6f72 733a 0a20 2020 2020 2020  _errors:.       
+0000e3f0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000e400: 616c 7565 4572 726f 7228 274e 6f20 6669  alueError('No fi
+0000e410: 6c65 7320 666f 756e 6421 2729 0a20 2020  les found!').   
+0000e420: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000e430: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000e440: 7269 6e74 2827 4552 524f 523a 204e 6f20  rint('ERROR: No 
+0000e450: 6669 6c65 7320 666f 756e 6421 2729 0a20  files found!'). 
+0000e460: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000e470: 6574 7572 6e0a 0a20 2020 2020 2020 2023  eturn..        #
+0000e480: 206d 616b 6520 756e 6971 7565 2061 6e64   make unique and
+0000e490: 2073 6f72 740a 2020 2020 2020 2020 6669   sort.        fi
+0000e4a0: 6c65 5f6c 6973 7420 3d20 6c69 7374 2873  le_list = list(s
+0000e4b0: 6574 2866 696c 655f 6c69 7374 2929 0a20  et(file_list)). 
+0000e4c0: 2020 2020 2020 2066 696c 655f 6c69 7374         file_list
+0000e4d0: 203d 2073 6f72 7465 6428 6669 6c65 5f6c   = sorted(file_l
+0000e4e0: 6973 7429 0a0a 0a20 2020 2020 2020 2023  ist)...        #
+0000e4f0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+0000e500: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2020 2020  ========.       
+0000e510: 2023 2046 696c 7465 7220 6669 6c65 7320   # Filter files 
+0000e520: 6261 7365 6420 6f6e 0a20 2020 2020 2020  based on.       
+0000e530: 2023 2073 6572 6965 730a 2020 2020 2020   # series.      
+0000e540: 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    # ============
+0000e550: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a20 2020  ===========..   
+0000e560: 2020 2020 2023 2073 6572 6965 730a 2020       # series.  
+0000e570: 2020 2020 2020 6966 2073 6572 6965 7320        if series 
+0000e580: 6973 206e 6f74 204e 6f6e 653a 0a0a 2020  is not None:..  
+0000e590: 2020 2020 2020 2020 2020 2320 636f 6e76            # conv
+0000e5a0: 6572 7420 746f 2061 7272 6179 0a20 2020  ert to array.   
+0000e5b0: 2020 2020 2020 2020 2069 6620 286e 6f74           if (not
+0000e5c0: 2069 7369 6e73 7461 6e63 6528 7365 7269   isinstance(seri
+0000e5d0: 6573 2c20 6c69 7374 290a 2020 2020 2020  es, list).      
+0000e5e0: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+0000e5f0: 7420 6973 696e 7374 616e 6365 2873 6572  t isinstance(ser
+0000e600: 6965 732c 2073 6574 290a 2020 2020 2020  ies, set).      
+0000e610: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+0000e620: 7420 6973 696e 7374 616e 6365 2873 6572  t isinstance(ser
+0000e630: 6965 732c 206e 702e 6e64 6172 7261 7929  ies, np.ndarray)
+0000e640: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000e650: 2020 2073 6572 6965 7320 3d20 5b73 6572     series = [ser
+0000e660: 6965 735d 0a0a 0a20 2020 2020 2020 2020  ies]...         
+0000e670: 2020 2023 2075 6e69 7175 650a 2020 2020     # unique.    
+0000e680: 2020 2020 2020 2020 7365 7269 6573 203d          series =
+0000e690: 206c 6973 7428 7365 7428 7365 7269 6573   list(set(series
+0000e6a0: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+0000e6b0: 2320 6c6f 6f70 2061 6e64 2063 6f6e 7665  # loop and conve
+0000e6c0: 7274 2074 6f20 7365 7269 6573 206e 616d  rt to series nam
+0000e6d0: 6520 6966 206e 6565 6465 640a 2020 2020  e if needed.    
+0000e6e0: 2020 2020 2020 2020 666f 7220 6974 2069          for it i
+0000e6f0: 6e20 7261 6e67 6528 6c65 6e28 7365 7269  n range(len(seri
+0000e700: 6573 2929 3a0a 2020 2020 2020 2020 2020  es)):.          
+0000e710: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+0000e720: 6e63 6528 7365 7269 6573 5b69 745d 2c20  nce(series[it], 
+0000e730: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+0000e740: 2020 2020 2020 2020 2020 7365 7269 6573            series
+0000e750: 5b69 745d 203d 2065 7874 7261 6374 5f73  [it] = extract_s
+0000e760: 6572 6965 735f 6e61 6d65 2873 6572 6965  eries_name(serie
+0000e770: 735b 6974 5d29 0a0a 0a20 2020 2020 2020  s[it])...       
+0000e780: 2020 2020 2023 2066 696c 7465 7220 6c69       # filter li
+0000e790: 7374 0a20 2020 2020 2020 2020 2020 2066  st.            f
+0000e7a0: 696c 655f 6c69 7374 5f74 656d 7020 3d20  ile_list_temp = 
+0000e7b0: 6c69 7374 2829 0a20 2020 2020 2020 2020  list().         
+0000e7c0: 2020 2066 6f72 2061 6669 6c65 2069 6e20     for afile in 
+0000e7d0: 6669 6c65 5f6c 6973 743a 0a20 2020 2020  file_list:.     
+0000e7e0: 2020 2020 2020 2020 2020 2066 6f72 2061             for a
+0000e7f0: 7365 7269 6573 2069 6e20 7365 7269 6573  series in series
+0000e800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e810: 2020 2020 2020 6966 2061 7365 7269 6573        if aseries
+0000e820: 2069 6e20 6166 696c 653a 0a20 2020 2020   in afile:.     
+0000e830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e840: 2020 2066 696c 655f 6c69 7374 5f74 656d     file_list_tem
+0000e850: 702e 6170 7065 6e64 2861 6669 6c65 290a  p.append(afile).
+0000e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e870: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
+0000e880: 2020 2020 2020 2020 2020 2320 7265 706c            # repl
+0000e890: 6163 650a 2020 2020 2020 2020 2020 2020  ace.            
+0000e8a0: 6669 6c65 5f6c 6973 7420 3d20 6669 6c65  file_list = file
+0000e8b0: 5f6c 6973 745f 7465 6d70 0a20 2020 2020  _list_temp.     
+0000e8c0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0000e8d0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000e8e0: 2020 2020 2023 203d 3d3d 3d3d 3d3d 3d3d       # =========
+0000e8f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20  ==============. 
+0000e900: 2020 2020 2020 2023 2046 696c 7465 7220         # Filter 
+0000e910: 6669 6c65 7320 6261 7365 6420 6f6e 0a20  files based on. 
+0000e920: 2020 2020 2020 2023 2065 7665 6e74 5f6c         # event_l
+0000e930: 6973 740a 2020 2020 2020 2020 2320 6275  ist.        # bu
+0000e940: 696c 6420 6469 6374 696f 6e61 7279 0a20  ild dictionary. 
+0000e950: 2020 2020 2020 2023 203d 3d3d 3d3d 3d3d         # =======
+0000e960: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000e970: 0a0a 2020 2020 2020 2020 2320 696e 6974  ..        # init
+0000e980: 6961 6c69 7a65 0a20 2020 2020 2020 206f  ialize.        o
+0000e990: 7574 7075 745f 6469 6374 203d 2064 6963  utput_dict = dic
+0000e9a0: 7428 290a 0a20 2020 2020 2020 2023 2063  t()..        # c
+0000e9b0: 6173 6520 6e6f 2065 7665 6e74 206c 6973  ase no event lis
+0000e9c0: 740a 2020 2020 2020 2020 6966 2065 7665  t.        if eve
+0000e9d0: 6e74 5f6c 6973 7420 6973 204e 6f6e 653a  nt_list is None:
+0000e9e0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000e9f0: 2061 6669 6c65 2069 6e20 6669 6c65 5f6c   afile in file_l
+0000ea00: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
+0000ea10: 2020 2020 206f 7574 7075 745f 6469 6374       output_dict
+0000ea20: 5b61 6669 6c65 5d20 3d20 4e6f 6e65 0a20  [afile] = None. 
+0000ea30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000ea40: 6e20 6f75 7470 7574 5f64 6963 740a 0a0a  n output_dict...
+0000ea50: 2020 2020 2020 2020 2320 6361 7365 2065          # case e
+0000ea60: 7665 6e74 206c 6973 740a 2020 2020 2020  vent list.      
+0000ea70: 2020 0a20 2020 2020 2020 2066 6f72 2065    .        for e
+0000ea80: 7665 6e74 5f64 6963 7420 696e 2065 7665  vent_dict in eve
+0000ea90: 6e74 5f6c 6973 743a 0a0a 2020 2020 2020  nt_list:..      
+0000eaa0: 2020 2020 2020 2320 6368 6563 6b73 0a20        # checks. 
+0000eab0: 2020 2020 2020 2020 2020 2069 6620 2773             if 's
+0000eac0: 6572 6965 735f 6e75 6d62 6572 2720 6e6f  eries_number' no
+0000ead0: 7420 696e 2065 7665 6e74 5f64 6963 742e  t in event_dict.
+0000eae0: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
+0000eaf0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0000eb00: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+0000eb10: 2020 2020 2020 2020 2020 2020 2020 2745                'E
+0000eb20: 5252 4f52 3a20 2273 6572 6965 735f 6e75  RROR: "series_nu
+0000eb30: 6d62 6572 2220 7265 7175 6972 6564 2069  mber" required i
+0000eb40: 6e20 6576 656e 7420 6469 6374 696f 6e61  n event dictiona
+0000eb50: 7279 2127 0a20 2020 2020 2020 2020 2020  ry!'.           
+0000eb60: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000eb70: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+0000eb80: 6966 2027 6576 656e 745f 6e75 6d62 6572  if 'event_number
+0000eb90: 2720 6e6f 7420 696e 2065 7665 6e74 5f64  ' not in event_d
+0000eba0: 6963 742e 6b65 7973 2829 3a0a 2020 2020  ict.keys():.    
+0000ebb0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000ebc0: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+0000ebd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebe0: 2020 2745 5252 4f52 3a20 2265 7665 6e74    'ERROR: "event
+0000ebf0: 5f6e 756d 6265 7222 2072 6571 7569 7265  _number" require
+0000ec00: 6420 696e 2065 7665 6e74 2064 6963 7469  d in event dicti
+0000ec10: 6f6e 6172 7921 270a 2020 2020 2020 2020  onary!'.        
+0000ec20: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000ec30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000ec40: 2020 2020 2320 6275 696c 6420 6669 6c65      # build file
+0000ec50: 206e 616d 6520 2877 6974 686f 7574 2070   name (without p
+0000ec60: 7265 6669 7829 0a20 2020 2020 2020 2020  refix).         
+0000ec70: 2020 2073 6572 6965 735f 6e75 6d20 3d20     series_num = 
+0000ec80: 2069 6e74 2865 7665 6e74 5f64 6963 745b   int(event_dict[
+0000ec90: 2773 6572 6965 735f 6e75 6d62 6572 275d  'series_number']
+0000eca0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000ecb0: 7269 6573 5f6e 616d 6520 3d20 6578 7472  ries_name = extr
+0000ecc0: 6163 745f 7365 7269 6573 5f6e 616d 6528  act_series_name(
+0000ecd0: 7365 7269 6573 5f6e 756d 290a 2020 2020  series_num).    
+0000ece0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000ecf0: 2020 2020 2064 756d 705f 6e75 6d20 3d20       dump_num = 
+0000ed00: 696e 7428 6576 656e 745f 6469 6374 5b27  int(event_dict['
+0000ed10: 6576 656e 745f 6e75 6d62 6572 275d 2f31  event_number']/1
+0000ed20: 3030 3030 3029 0a20 2020 2020 2020 2020  00000).         
+0000ed30: 2020 2064 756d 705f 6e61 6d65 203d 2073     dump_name = s
+0000ed40: 7472 2864 756d 705f 6e75 6d29 0a20 2020  tr(dump_num).   
+0000ed50: 2020 2020 2020 2020 2066 6f72 2078 2069           for x i
+0000ed60: 6e20 7261 6e67 6528 312c 352d 6c65 6e28  n range(1,5-len(
+0000ed70: 6475 6d70 5f6e 616d 6529 293a 0a20 2020  dump_name)):.   
+0000ed80: 2020 2020 2020 2020 2020 2020 2064 756d               dum
+0000ed90: 705f 6e61 6d65 203d 2027 3027 202b 2064  p_name = '0' + d
+0000eda0: 756d 705f 6e61 6d65 0a0a 2020 2020 2020  ump_name..      
+0000edb0: 2020 2020 2020 6669 6c65 5f6e 616d 6520        file_name 
+0000edc0: 3d20 2873 6572 6965 735f 6e61 6d65 0a20  = (series_name. 
+0000edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ede0: 2020 2020 2020 2020 2b20 275f 4627 0a20          + '_F'. 
+0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee00: 2020 2020 2020 2020 2b20 6475 6d70 5f6e          + dump_n
+0000ee10: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+0000ee20: 2020 2020 2020 2020 2020 2020 202b 2027               + '
+0000ee30: 2e68 6466 3527 290a 0a20 2020 2020 2020  .hdf5')..       
+0000ee40: 2020 2020 2023 2066 696e 6420 6669 6c65       # find file
+0000ee50: 2069 6e20 6669 6c65 5f6c 6973 740a 2020   in file_list.  
+0000ee60: 2020 2020 2020 2020 2020 6675 6c6c 5f66            full_f
+0000ee70: 696c 655f 6e61 6d65 203d 2073 7472 2829  ile_name = str()
+0000ee80: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000ee90: 2061 6669 6c65 2069 6e20 6669 6c65 5f6c   afile in file_l
+0000eea0: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
+0000eeb0: 2020 2020 2069 6620 6669 6c65 5f6e 616d       if file_nam
+0000eec0: 6520 696e 2061 6669 6c65 3a0a 2020 2020  e in afile:.    
+0000eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eee0: 6675 6c6c 5f66 696c 655f 6e61 6d65 203d  full_file_name =
+0000eef0: 2061 6669 6c65 0a20 2020 2020 2020 2020   afile.         
+0000ef00: 2020 2020 2020 2020 2020 2062 7265 616b             break
+0000ef10: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000ef20: 206e 6f74 2066 756c 6c5f 6669 6c65 5f6e   not full_file_n
+0000ef30: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+0000ef40: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0000ef50: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0000ef60: 2020 2020 2020 2020 2020 2027 4552 524f             'ERRO
+0000ef70: 523a 2055 6e61 626c 6520 746f 2066 696e  R: Unable to fin
+0000ef80: 6420 6669 6c65 2066 6f72 2061 2072 6571  d file for a req
+0000ef90: 7565 7374 6564 2065 7665 6e74 2e27 0a20  uested event.'. 
+0000efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efb0: 2020 202b 2027 2043 6865 636b 2070 6174     + ' Check pat
+0000efc0: 6821 2720 290a 0a20 2020 2020 2020 2020  h!' )..         
+0000efd0: 2020 2023 2064 6f75 626c 6520 6368 6563     # double chec
+0000efe0: 6b20 6772 6f75 7020 6966 2061 7661 696c  k group if avail
+0000eff0: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
+0000f000: 2069 6620 2767 726f 7570 5f6e 616d 6527   if 'group_name'
+0000f010: 2069 6e20 6576 656e 745f 6469 6374 2e6b   in event_dict.k
+0000f020: 6579 7328 293a 0a20 2020 2020 2020 2020  eys():.         
+0000f030: 2020 2020 2020 2067 726f 7570 5f6e 616d         group_nam
+0000f040: 6520 3d20 7374 7228 6576 656e 745f 6469  e = str(event_di
+0000f050: 6374 5b27 6772 6f75 705f 6e61 6d65 275d  ct['group_name']
+0000f060: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f070: 2020 6966 2067 726f 7570 5f6e 616d 6520    if group_name 
+0000f080: 6e6f 7420 696e 2066 756c 6c5f 6669 6c65  not in full_file
+0000f090: 5f6e 616d 653a 0a20 2020 2020 2020 2020  _name:.         
+0000f0a0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000f0b0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0d0: 2020 2020 2027 4552 524f 523a 2049 6e63       'ERROR: Inc
+0000f0e0: 6f6e 7369 7374 656e 7420 6772 6f75 7020  onsistent group 
+0000f0f0: 6e61 6d65 2e20 556e 6162 6c65 2074 6f20  name. Unable to 
+0000f100: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000f110: 2020 2020 2020 2020 2020 2720 6669 6e64            ' find
+0000f120: 2070 726f 7065 7220 6461 7461 2127 0a20   proper data!'. 
+0000f130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f140: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+0000f150: 2020 2320 7361 7665 0a20 2020 2020 2020    # save.       
+0000f160: 2020 2020 2069 6620 6675 6c6c 5f66 696c       if full_fil
+0000f170: 655f 6e61 6d65 2069 6e20 6f75 7470 7574  e_name in output
+0000f180: 5f64 6963 742e 6b65 7973 2829 3a0a 2020  _dict.keys():.  
+0000f190: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+0000f1a0: 7470 7574 5f64 6963 745b 6675 6c6c 5f66  tput_dict[full_f
+0000f1b0: 696c 655f 6e61 6d65 5d2e 6170 7065 6e64  ile_name].append
+0000f1c0: 2865 7665 6e74 5f64 6963 7429 0a20 2020  (event_dict).   
+0000f1d0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000f1e0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000f1f0: 7574 7075 745f 6469 6374 5b66 756c 6c5f  utput_dict[full_
+0000f200: 6669 6c65 5f6e 616d 655d 203d 205b 6576  file_name] = [ev
+0000f210: 656e 745f 6469 6374 5d0a 2020 2020 2020  ent_dict].      
+0000f220: 2020 2020 2020 0a20 2020 2020 2020 2072        .        r
+0000f230: 6574 7572 6e20 6f75 7470 7574 5f64 6963  eturn output_dic
+0000f240: 740a 2020 2020 2020 2020 2020 2020 0a20  t.            . 
+0000f250: 2020 200a 2020 2020 2020 2020 0a0a 0a0a     .        ....
+0000f260: 0a0a 0a0a 2020 2020 2020 2020 2020 2020  ....            
+0000f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f280: 2020 0a0a 0a20 2020 200a 636c 6173 7320    ...    .class 
+0000f290: 4835 5772 6974 6572 3a0a 2020 2020 0a20  H5Writer:.    . 
+0000f2a0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000f2b0: 7365 6c66 2c20 7261 6973 655f 6572 726f  self, raise_erro
+0000f2c0: 7273 3d54 7275 652c 2076 6572 626f 7365  rs=True, verbose
+0000f2d0: 3d54 7275 6529 3a0a 0a0a 2020 2020 2020  =True):...      
+0000f2e0: 2020 7365 6c66 2e5f 7261 6973 655f 6572    self._raise_er
+0000f2f0: 726f 7273 203d 2072 6169 7365 5f65 7272  rors = raise_err
+0000f300: 6f72 730a 2020 2020 2020 2020 7365 6c66  ors.        self
+0000f310: 2e5f 7665 7262 6f73 6520 3d20 7665 7262  ._verbose = verb
+0000f320: 6f73 650a 2020 2020 2020 2020 0a20 2020  ose.        .   
+0000f330: 2020 2020 2023 2066 696c 6520 7061 7468       # file path
+0000f340: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+0000f350: 6572 6965 735f 7061 7468 203d 204e 6f6e  eries_path = Non
+0000f360: 650a 0a20 2020 2020 2020 2023 2073 6572  e..        # ser
+0000f370: 6965 730a 2020 2020 2020 2020 7365 6c66  ies.        self
+0000f380: 2e5f 7365 7269 6573 5f6e 616d 6520 3d20  ._series_name = 
+0000f390: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000f3a0: 662e 5f73 6572 6965 735f 6e75 6d20 3d20  f._series_num = 
+0000f3b0: 4e6f 6e65 0a20 2020 2020 2020 200a 2020  None.        .  
+0000f3c0: 2020 2020 2020 2320 6375 7272 656e 7420        # current 
+0000f3d0: 6669 6c65 2069 6e66 6f0a 2020 2020 2020  file info.      
+0000f3e0: 2020 7365 6c66 2e5f 6375 7272 656e 745f    self._current_
+0000f3f0: 6669 6c65 203d 204e 6f6e 650a 2020 2020  file = None.    
+0000f400: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
+0000f410: 745f 6669 6c65 5f6e 616d 6520 3d20 4e6f  t_file_name = No
+0000f420: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000f430: 5f63 7572 7265 6e74 5f66 696c 655f 6e62  _current_file_nb
+0000f440: 5f65 7665 6e74 7320 3d20 300a 2020 2020  _events = 0.    
+0000f450: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
+0000f460: 745f 6669 6c65 5f65 7665 6e74 5f63 6f75  t_file_event_cou
+0000f470: 6e74 6572 203d 2030 0a20 2020 2020 2020  nter = 0.       
+0000f480: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
+0000f490: 696c 655f 6164 635f 6772 6f75 7020 3d20  ile_adc_group = 
+0000f4a0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000f4b0: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
+0000f4c0: 6465 7463 6f6e 6669 675f 6772 6f75 7020  detconfig_group 
+0000f4d0: 3d20 4e6f 6e65 0a20 2020 2020 2020 200a  = None.        .
+0000f4e0: 2020 2020 2020 2020 2320 6d65 7461 6461          # metada
+0000f4f0: 7461 0a20 2020 2020 2020 2073 656c 662e  ta.        self.
+0000f500: 5f66 696c 655f 6d65 7461 6461 7461 203d  _file_metadata =
+0000f510: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+0000f520: 6c66 2e5f 6465 7465 6374 6f72 5f63 6f6e  lf._detector_con
+0000f530: 6669 6720 3d20 4e6f 6e65 0a20 2020 2020  fig = None.     
+0000f540: 2020 2073 656c 662e 5f61 6463 5f63 6f6e     self._adc_con
+0000f550: 6669 6720 203d 204e 6f6e 650a 0a20 2020  fig  = None..   
+0000f560: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+0000f570: 6576 656e 7420 636f 756e 7465 720a 2020  event counter.  
+0000f580: 2020 2020 2020 7365 6c66 2e5f 676c 6f62        self._glob
+0000f590: 616c 5f65 7665 6e74 735f 636f 756e 7465  al_events_counte
+0000f5a0: 7220 3d20 300a 2020 2020 2020 2020 200a  r = 0.         .
+0000f5b0: 2020 2020 2020 2020 2320 6669 6c65 2063          # file c
+0000f5c0: 6f75 6e74 6572 0a20 2020 2020 2020 2073  ounter.        s
+0000f5d0: 656c 662e 5f66 696c 655f 636f 756e 7465  elf._file_counte
+0000f5e0: 7220 3d20 300a 0a20 2020 2020 2020 2023  r = 0..        #
+0000f5f0: 206d 6178 2065 7665 6e74 2070 6572 2064   max event per d
+0000f600: 756d 700a 2020 2020 2020 2020 7365 6c66  ump.        self
+0000f610: 2e5f 6e62 5f65 7665 6e74 735f 7065 725f  ._nb_events_per_
+0000f620: 6475 6d70 5f6d 6178 203d 2031 3030 300a  dump_max = 1000.
+0000f630: 2020 2020 2020 2020 7365 6c66 2e5f 6164          self._ad
+0000f640: 635f 6e61 6d65 203d 2027 6164 6331 270a  c_name = 'adc1'.
+0000f650: 0a0a 2020 2020 6465 6620 696e 6974 6961  ..    def initia
+0000f660: 6c69 7a65 2873 656c 662c 2073 6572 6965  lize(self, serie
+0000f670: 735f 6e61 6d65 2c20 6461 7461 5f70 6174  s_name, data_pat
+0000f680: 683d 272e 2f27 293a 0a20 2020 2020 2020  h='./'):.       
+0000f690: 2022 2222 0a20 2020 2020 2020 2049 6e69   """.        Ini
+0000f6a0: 7469 616c 697a 6520 6e65 7720 7772 6974  tialize new writ
+0000f6b0: 696e 670a 2020 2020 2020 2020 2222 220a  ing.        """.
+0000f6c0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000f6d0: 2023 2063 6c65 6172 2065 7665 7279 7468   # clear everyth
+0000f6e0: 696e 670a 2020 2020 2020 2020 7365 6c66  ing.        self
+0000f6f0: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
+0000f700: 200a 2020 2020 2020 2020 2320 7365 7269   .        # seri
+0000f710: 6573 206e 616d 6520 0a20 2020 2020 2020  es name .       
+0000f720: 2073 656c 662e 5f73 6572 6965 735f 6e61   self._series_na
+0000f730: 6d65 203d 2073 6572 6965 735f 6e61 6d65  me = series_name
+0000f740: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+0000f750: 6572 6965 735f 6e75 6d20 3d20 6578 7472  eries_num = extr
+0000f760: 6163 745f 7365 7269 6573 5f6e 756d 2873  act_series_num(s
+0000f770: 6572 6965 735f 6e61 6d65 290a 2020 2020  eries_name).    
+0000f780: 2020 2020 0a0a 0a20 2020 2020 2020 2023      ...        #
+0000f790: 2063 7265 6174 6520 6e65 7720 6469 7265   create new dire
+0000f7a0: 6374 6f72 790a 2020 2020 2020 2020 2373  ctory.        #s
+0000f7b0: 656c 662e 5f73 6572 6965 735f 7061 7468  elf._series_path
+0000f7c0: 203d 2064 6174 615f 7061 7468 202b 2027   = data_path + '
+0000f7d0: 2f27 202b 2073 6572 6965 735f 6e61 6d65  /' + series_name
+0000f7e0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+0000f7f0: 6572 6965 735f 7061 7468 203d 2064 6174  eries_path = dat
+0000f800: 615f 7061 7468 0a20 2020 2020 2020 200a  a_path.        .
+0000f810: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
+0000f820: 732e 7061 7468 2e69 7364 6972 2873 656c  s.path.isdir(sel
+0000f830: 662e 5f73 6572 6965 735f 7061 7468 293a  f._series_path):
+0000f840: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
+0000f850: 6d6b 6469 7228 7365 6c66 2e5f 7365 7269  mkdir(self._seri
+0000f860: 6573 5f70 6174 6829 0a20 2020 2020 2020  es_path).       
+0000f870: 2020 2020 206f 732e 6368 6d6f 6428 7365       os.chmod(se
+0000f880: 6c66 2e5f 7365 7269 6573 5f70 6174 682c  lf._series_path,
+0000f890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f8a0: 2020 2020 2020 7374 6174 2e53 5f49 5257        stat.S_IRW
+0000f8b0: 5847 207c 2073 7461 742e 535f 4952 5758  XG | stat.S_IRWX
+0000f8c0: 5520 7c20 7374 6174 2e53 5f49 524f 5448  U | stat.S_IROTH
+0000f8d0: 207c 2073 7461 742e 535f 4958 4f54 4829   | stat.S_IXOTH)
+0000f8e0: 0a0a 0a20 2020 2064 6566 2073 6574 5f6d  ...    def set_m
+0000f8f0: 6574 6164 6174 6128 7365 6c66 2c20 6669  etadata(self, fi
+0000f900: 6c65 5f6d 6574 6164 6174 613d 4e6f 6e65  le_metadata=None
+0000f910: 2c20 6164 635f 636f 6e66 6967 3d4e 6f6e  , adc_config=Non
+0000f920: 652c 2064 6574 6563 746f 725f 636f 6e66  e, detector_conf
+0000f930: 6967 3d4e 6f6e 6529 3a0a 2020 2020 2020  ig=None):.      
+0000f940: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
+0000f950: 7420 6d65 7461 6461 7461 2077 6869 6368  t metadata which
+0000f960: 2077 696c 6c20 6265 2077 7269 7474 656e   will be written
+0000f970: 2020 696e 2065 6163 6820 6669 6c65 730a    in each files.
+0000f980: 2020 2020 2020 2020 6669 6c65 5f6d 6574          file_met
+0000f990: 6164 6174 6120 3d20 6765 6e65 7261 6c20  adata = general 
+0000f9a0: 6461 7461 2074 616b 696e 6720 696e 666f  data taking info
+0000f9b0: 726d 6174 696f 6e20 2866 696c 6520 6c65  rmation (file le
+0000f9c0: 7665 6c20 6d65 7461 6461 7461 290a 2020  vel metadata).  
+0000f9d0: 2020 2020 2020 6164 635f 636f 6e66 6967        adc_config
+0000f9e0: 203d 2061 6463 2063 6f6e 6669 6775 7261   = adc configura
+0000f9f0: 7469 6f6e 2028 6772 6f75 7020 6c65 7665  tion (group leve
+0000fa00: 6c20 6d65 7461 6461 7461 290a 2020 2020  l metadata).    
+0000fa10: 2020 2020 6465 7465 6374 6f72 5f63 6f6e      detector_con
+0000fa20: 6669 6720 3d20 6465 7465 6374 6f72 2073  fig = detector s
+0000fa30: 6574 7469 6e67 7320 2867 726f 7570 206c  ettings (group l
+0000fa40: 6576 656c 206d 6574 6164 6174 6129 0a20  evel metadata). 
+0000fa50: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+0000fa60: 2020 2020 6966 2066 696c 655f 6d65 7461      if file_meta
+0000fa70: 6461 7461 2069 7320 6e6f 7420 4e6f 6e65  data is not None
+0000fa80: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
+0000fa90: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0000faa0: 616e 6365 2866 696c 655f 6d65 7461 6461  ance(file_metada
+0000fab0: 7461 2c20 6469 6374 293a 0a20 2020 2020  ta, dict):.     
+0000fac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fad0: 5f66 696c 655f 6d65 7461 6461 7461 203d  _file_metadata =
+0000fae0: 2066 696c 655f 6d65 7461 6461 7461 0a20   file_metadata. 
+0000faf0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000fb00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fb10: 2070 7269 6e74 2827 5741 524e 494e 473a   print('WARNING:
+0000fb20: 206d 6574 6164 6174 6120 6e65 6564 7320   metadata needs 
+0000fb30: 746f 2062 6520 6120 6469 6374 696f 6e61  to be a dictiona
+0000fb40: 7279 2729 0a0a 2020 2020 2020 2020 2020  ry')..          
+0000fb50: 2020 2020 2020 0a20 2020 2020 2020 2069        .        i
+0000fb60: 6620 6164 635f 636f 6e66 6967 2069 7320  f adc_config is 
+0000fb70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000fb80: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+0000fb90: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000fba0: 2861 6463 5f63 6f6e 6669 672c 2064 6963  (adc_config, dic
+0000fbb0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+0000fbc0: 2020 2020 7365 6c66 2e5f 6164 635f 636f      self._adc_co
+0000fbd0: 6e66 6967 203d 2061 6463 5f63 6f6e 6669  nfig = adc_confi
+0000fbe0: 670a 2020 2020 2020 2020 2020 2020 656c  g.            el
+0000fbf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000fc00: 2020 2020 7072 696e 7428 2757 4152 4e49      print('WARNI
+0000fc10: 4e47 3a20 6164 635f 636f 6e66 6967 206e  NG: adc_config n
+0000fc20: 6565 6473 2074 6f20 6265 2061 2064 6963  eeds to be a dic
+0000fc30: 7469 6f6e 6172 7927 290a 0a0a 2020 2020  tionary')...    
+0000fc40: 2020 2020 6966 2064 6574 6563 746f 725f      if detector_
+0000fc50: 636f 6e66 6967 2069 7320 6e6f 7420 4e6f  config is not No
+0000fc60: 6e65 3a0a 0a20 2020 2020 2020 2020 2020  ne:..           
+0000fc70: 2069 6620 6973 696e 7374 616e 6365 2864   if isinstance(d
+0000fc80: 6574 6563 746f 725f 636f 6e66 6967 2c20  etector_config, 
+0000fc90: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
+0000fca0: 2020 2020 2020 2073 656c 662e 5f64 6574         self._det
+0000fcb0: 6563 746f 725f 636f 6e66 6967 203d 2064  ector_config = d
+0000fcc0: 6574 6563 746f 725f 636f 6e66 6967 0a20  etector_config. 
+0000fcd0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000fce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fcf0: 2070 7269 6e74 2827 5741 524e 494e 473a   print('WARNING:
+0000fd00: 2064 6574 6563 746f 7220 636f 6e66 6967   detector config
+0000fd10: 206e 6565 6473 2074 6f20 6265 2061 2064   needs to be a d
+0000fd20: 6963 7469 6f6e 6172 7927 290a 0a0a 2020  ictionary')...  
+0000fd30: 2020 2020 2020 2020 2020 2020 2020 0a0a                ..
+0000fd40: 2020 2020 2020 2020 2020 2020 0a0a 2020              ..  
+0000fd50: 2020 6465 6620 636c 6f73 6528 7365 6c66    def close(self
+0000fd60: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000fd70: 2020 2020 2020 2063 6c6f 7365 2063 7572         close cur
+0000fd80: 7265 6e74 2066 696c 650a 2020 2020 2020  rent file.      
+0000fd90: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
+0000fda0: 656c 662e 5f63 6c6f 7365 5f66 696c 6528  elf._close_file(
+0000fdb0: 290a 2020 2020 2020 2020 2020 2020 0a20  ).            . 
+0000fdc0: 2020 2020 2020 200a 2020 2020 6465 6620         .    def 
+0000fdd0: 636c 6561 7228 7365 6c66 293a 0a20 2020  clear(self):.   
+0000fde0: 2020 2020 2073 656c 662e 5f63 6c6f 7365       self._close
+0000fdf0: 5f66 696c 6528 290a 2020 2020 2020 2020  _file().        
+0000fe00: 7365 6c66 2e5f 6669 6c65 5f63 6f75 6e74  self._file_count
+0000fe10: 6572 203d 2030 0a20 2020 2020 2020 2073  er = 0.        s
+0000fe20: 656c 662e 5f63 7572 7265 6e74 5f66 696c  elf._current_fil
+0000fe30: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
+0000fe40: 2073 656c 662e 5f63 7572 7265 6e74 5f66   self._current_f
+0000fe50: 696c 655f 6e61 6d65 203d 204e 6f6e 650a  ile_name = None.
+0000fe60: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
+0000fe70: 7272 656e 745f 6669 6c65 5f61 6463 5f67  rrent_file_adc_g
+0000fe80: 726f 7570 203d 204e 6f6e 650a 2020 2020  roup = None.    
+0000fe90: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
+0000fea0: 745f 6669 6c65 5f64 6574 636f 6e66 6967  t_file_detconfig
+0000feb0: 5f67 726f 7570 203d 204e 6f6e 6520 2020  _group = None   
+0000fec0: 200a 2020 2020 2020 2020 7365 6c66 2e5f   .        self._
+0000fed0: 6375 7272 656e 745f 6669 6c65 5f65 7665  current_file_eve
+0000fee0: 6e74 5f63 6f75 6e74 6572 203d 2030 0a20  nt_counter = 0. 
+0000fef0: 2020 2020 2020 2073 656c 662e 5f67 6c6f         self._glo
+0000ff00: 6261 6c5f 6576 656e 745f 636f 756e 7465  bal_event_counte
+0000ff10: 7220 3d20 300a 2020 2020 2020 2020 7365  r = 0.        se
+0000ff20: 6c66 2e5f 6669 6c65 5f6d 6574 6164 6174  lf._file_metadat
+0000ff30: 6120 3d20 4e6f 6e65 0a20 2020 2020 2020  a = None.       
+0000ff40: 2073 656c 662e 5f64 6574 6563 746f 725f   self._detector_
+0000ff50: 636f 6e66 6967 203d 204e 6f6e 650a 2020  config = None.  
+0000ff60: 2020 2020 2020 7365 6c66 2e5f 6164 635f        self._adc_
+0000ff70: 636f 6e66 6967 203d 204e 6f6e 650a 2020  config = None.  
+0000ff80: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
+0000ff90: 2064 6566 2077 7269 7465 5f65 7665 6e74   def write_event
+0000ffa0: 2873 656c 662c 2064 6174 615f 6172 7261  (self, data_arra
+0000ffb0: 792c 2070 7265 6669 783d 4e6f 6e65 2c20  y, prefix=None, 
+0000ffc0: 6461 7461 7365 745f 6d65 7461 6461 7461  dataset_metadata
+0000ffd0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0000ffe0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+0000fff0: 6d6f 6465 3d4e 6f6e 652c 2061 6463 5f6e  mode=None, adc_n
+00010000: 616d 653d 2761 6463 3127 293a 0a20 2020  ame='adc1'):.   
+00010010: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00010020: 2077 7269 7465 2070 756c 7365 2064 6174   write pulse dat
+00010030: 6120 696e 2066 696c 6573 0a20 2020 2020  a in files.     
+00010040: 2020 2022 2222 0a0a 0a20 2020 2020 2020     """...       
+00010050: 2023 206f 7065 6e20 6669 6c65 2069 6620   # open file if 
+00010060: 6e65 6564 6564 0a20 2020 2020 2020 2069  needed.        i
+00010070: 6620 2873 656c 662e 5f63 7572 7265 6e74  f (self._current
+00010080: 5f66 696c 6520 6973 204e 6f6e 6520 6f72  _file is None or
+00010090: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000100a0: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
+000100b0: 6576 656e 745f 636f 756e 7465 7220 3e3d  event_counter >=
+000100c0: 2073 656c 662e 5f6e 625f 6576 656e 7473   self._nb_events
+000100d0: 5f70 6572 5f64 756d 705f 6d61 7829 3a0a  _per_dump_max):.
+000100e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000100f0: 2e5f 6f70 656e 5f66 696c 6528 7072 6566  ._open_file(pref
+00010100: 6978 3d70 7265 6669 7829 0a0a 0a20 2020  ix=prefix)...   
+00010110: 2020 2020 2023 2065 7665 6e74 2063 6f75       # event cou
+00010120: 6e74 6572 0a20 2020 2020 2020 2073 656c  nter.        sel
+00010130: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
+00010140: 6576 656e 745f 636f 756e 7465 7220 2b3d  event_counter +=
+00010150: 2031 0a20 2020 2020 2020 2073 656c 662e   1.        self.
+00010160: 5f67 6c6f 6261 6c5f 6576 656e 745f 636f  _global_event_co
+00010170: 756e 7465 7220 2b3d 2031 0a20 2020 2020  unter += 1.     
+00010180: 2020 200a 2020 2020 2020 2020 2320 6372     .        # cr
+00010190: 6561 7465 2064 6174 6173 6574 0a20 2020  eate dataset.   
+000101a0: 2020 2020 2064 6174 6173 6574 5f6e 616d       dataset_nam
+000101b0: 6520 3d20 2765 7665 6e74 5f27 202b 2073  e = 'event_' + s
+000101c0: 7472 2873 656c 662e 5f63 7572 7265 6e74  tr(self._current
+000101d0: 5f66 696c 655f 6576 656e 745f 636f 756e  _file_event_coun
+000101e0: 7465 7229 0a20 2020 2020 2020 2064 6174  ter).        dat
+000101f0: 6173 6574 203d 2073 656c 662e 5f63 7572  aset = self._cur
+00010200: 7265 6e74 5f66 696c 655f 6164 635f 6772  rent_file_adc_gr
+00010210: 6f75 702e 6372 6561 7465 5f64 6174 6173  oup.create_datas
+00010220: 6574 2864 6174 6173 6574 5f6e 616d 652c  et(dataset_name,
+00010230: 2064 6174 613d 6461 7461 5f61 7272 6179   data=data_array
+00010240: 290a 2020 2020 2020 0a20 2020 2020 2020  ).      .       
+00010250: 2023 2061 6464 206d 6574 6164 6174 610a   # add metadata.
+00010260: 2020 2020 2020 2020 6966 2064 6174 6173          if datas
+00010270: 6574 5f6d 6574 6164 6174 6120 6973 206e  et_metadata is n
+00010280: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00010290: 2020 2020 2066 6f72 206b 6579 2c76 616c       for key,val
+000102a0: 2069 6e20 6461 7461 7365 745f 6d65 7461   in dataset_meta
+000102b0: 6461 7461 2e69 7465 6d73 2829 3a0a 2020  data.items():.  
+000102c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000102d0: 2028 6973 696e 7374 616e 6365 2876 616c   (isinstance(val
+000102e0: 2c20 6e70 2e6e 6461 7272 6179 2920 616e  , np.ndarray) an
+000102f0: 6420 7661 6c2e 6474 7970 652e 7479 7065  d val.dtype.type
+00010300: 2069 7320 6e70 2e73 7472 5f29 3a0a 2020   is np.str_):.  
+00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010320: 2020 6474 203d 2068 3570 792e 7374 7269    dt = h5py.stri
+00010330: 6e67 5f64 7479 7065 2829 0a20 2020 2020  ng_dtype().     
+00010340: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00010350: 616c 203d 2076 616c 2e61 7374 7970 6528  al = val.astype(
+00010360: 6474 290a 2020 2020 2020 2020 2020 2020  dt).            
+00010370: 2020 2020 6461 7461 7365 742e 6174 7472      dataset.attr
+00010380: 735b 6b65 795d 203d 2076 616c 0a0a 2020  s[key] = val..  
+00010390: 2020 2020 2020 6461 7461 7365 742e 6174        dataset.at
+000103a0: 7472 735b 2765 7665 6e74 5f69 6427 5d20  trs['event_id'] 
+000103b0: 3d20 7365 6c66 2e5f 676c 6f62 616c 5f65  = self._global_e
+000103c0: 7665 6e74 5f63 6f75 6e74 6572 200a 2020  vent_counter .  
+000103d0: 2020 2020 2020 6461 7461 7365 742e 6174        dataset.at
+000103e0: 7472 735b 2765 7665 6e74 5f69 6e64 6578  trs['event_index
+000103f0: 275d 203d 2073 656c 662e 5f63 7572 7265  '] = self._curre
+00010400: 6e74 5f66 696c 655f 6576 656e 745f 636f  nt_file_event_co
+00010410: 756e 7465 720a 2020 2020 2020 2020 6461  unter.        da
+00010420: 7461 7365 742e 6174 7472 735b 2765 7665  taset.attrs['eve
+00010430: 6e74 5f6e 756d 275d 203d 2073 656c 662e  nt_num'] = self.
+00010440: 5f66 696c 655f 636f 756e 7465 7220 2a31  _file_counter *1
+00010450: 3030 3030 3020 2b20 7365 6c66 2e5f 6375  00000 + self._cu
+00010460: 7272 656e 745f 6669 6c65 5f65 7665 6e74  rrent_file_event
+00010470: 5f63 6f75 6e74 6572 0a20 2020 2020 2020  _counter.       
+00010480: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00010490: 2020 2320 7570 6461 7465 206e 756d 6265    # update numbe
+000104a0: 7220 6f66 2065 7665 6e74 730a 2020 2020  r of events.    
+000104b0: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
+000104c0: 745f 6669 6c65 5f61 6463 5f67 726f 7570  t_file_adc_group
+000104d0: 2e61 7474 7273 5b27 6e62 5f65 7665 6e74  .attrs['nb_event
+000104e0: 7327 5d20 3d20 7365 6c66 2e5f 6375 7272  s'] = self._curr
+000104f0: 656e 745f 6669 6c65 5f65 7665 6e74 5f63  ent_file_event_c
+00010500: 6f75 6e74 6572 0a20 2020 2020 2020 2069  ounter.        i
+00010510: 6620 6461 7461 5f6d 6f64 6520 6973 206e  f data_mode is n
+00010520: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00010530: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
+00010540: 6e74 5f66 696c 655f 6164 635f 6772 6f75  nt_file_adc_grou
+00010550: 702e 6174 7472 735b 2764 6174 615f 6d6f  p.attrs['data_mo
+00010560: 6465 275d 203d 2073 7472 2864 6174 615f  de'] = str(data_
+00010570: 6d6f 6465 290a 0a0a 2020 2020 2020 2020  mode)...        
+00010580: 2320 666c 7573 680a 2020 2020 2020 2020  # flush.        
+00010590: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+000105a0: 6c65 2e66 6c75 7368 2829 0a20 2020 2020  le.flush().     
+000105b0: 2020 200a 0a0a 0a0a 0a20 2020 2020 2020     ......       
+000105c0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+000105d0: 2020 6465 6620 5f6f 7065 6e5f 6669 6c65    def _open_file
+000105e0: 2873 656c 662c 2070 7265 6669 783d 4e6f  (self, prefix=No
+000105f0: 6e65 293a 0a20 2020 2020 2020 2022 2222  ne):.        """
+00010600: 0a20 2020 2020 2020 206f 7065 6e20 6669  .        open fi
+00010610: 6c65 200a 2020 2020 2020 2020 2222 220a  le .        """.
+00010620: 0a20 2020 2020 2020 2023 2063 6c6f 7365  .        # close
+00010630: 2066 696c 6520 6966 206e 6565 6465 640a   file if needed.
+00010640: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010650: 5f63 7572 7265 6e74 5f66 696c 6520 6973  _current_file is
+00010660: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00010670: 2020 2020 2020 2073 656c 662e 5f63 6c6f         self._clo
+00010680: 7365 5f66 696c 6528 290a 0a0a 2020 2020  se_file()...    
+00010690: 2020 2020 2320 6475 6d70 0a20 2020 2020      # dump.     
+000106a0: 2020 2073 656c 662e 5f66 696c 655f 636f     self._file_co
+000106b0: 756e 7465 7220 2b3d 310a 2020 2020 2020  unter +=1.      
+000106c0: 2020 6475 6d70 203d 2073 7472 2873 656c    dump = str(sel
+000106d0: 662e 5f66 696c 655f 636f 756e 7465 7229  f._file_counter)
+000106e0: 0a20 2020 2020 2020 2066 6f72 2078 2069  .        for x i
+000106f0: 6e20 7261 6e67 6528 312c 352d 6c65 6e28  n range(1,5-len(
+00010700: 6475 6d70 2929 3a0a 2020 2020 2020 2020  dump)):.        
+00010710: 2020 2020 6966 2078 3e3d 313a 0a20 2020      if x>=1:.   
+00010720: 2020 2020 2020 2020 2020 2020 2064 756d               dum
+00010730: 7020 3d20 2730 272b 6475 6d70 0a0a 0a20  p = '0'+dump... 
+00010740: 2020 2020 2020 2023 2066 756c 6c20 6669         # full fi
+00010750: 6c65 206e 616d 650a 2020 2020 2020 2020  le name.        
+00010760: 6669 6c65 5f6e 616d 6520 3d20 7365 6c66  file_name = self
+00010770: 2e5f 7365 7269 6573 5f70 6174 6820 2b20  ._series_path + 
+00010780: 272f 270a 2020 2020 2020 2020 6966 2070  '/'.        if p
+00010790: 7265 6669 7820 6973 206e 6f74 204e 6f6e  refix is not Non
+000107a0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+000107b0: 696c 655f 6e61 6d65 202b 3d20 7072 6566  ile_name += pref
+000107c0: 6978 202b 2027 5f27 0a20 2020 2020 2020  ix + '_'.       
+000107d0: 2066 696c 655f 6e61 6d65 202b 3d20 7365   file_name += se
+000107e0: 6c66 2e5f 7365 7269 6573 5f6e 616d 6520  lf._series_name 
+000107f0: 2b20 275f 4627 202b 2064 756d 7020 2b20  + '_F' + dump + 
+00010800: 272e 6864 6635 270a 2020 2020 2020 2020  '.hdf5'.        
+00010810: 7072 696e 7428 2749 4e46 4f3a 204f 7065  print('INFO: Ope
+00010820: 6e69 6e67 2066 696c 6520 6e61 6d65 2022  ning file name "
+00010830: 2720 2b20 6669 6c65 5f6e 616d 6520 2b20  ' + file_name + 
+00010840: 2722 2729 0a20 2020 2020 2020 200a 2020  '"').        .  
+00010850: 2020 2020 2020 0a20 2020 2020 2020 2066        .        f
+00010860: 696c 6520 3d20 4e6f 6e65 0a20 2020 2020  ile = None.     
+00010870: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00010880: 2020 2020 6669 6c65 203d 2068 3570 792e      file = h5py.
+00010890: 4669 6c65 2866 696c 655f 6e61 6d65 2c20  File(file_name, 
+000108a0: 2777 2729 0a20 2020 2020 2020 2065 7863  'w').        exc
+000108b0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
+000108c0: 2070 7269 6e74 2827 4552 524f 523a 2055   print('ERROR: U
+000108d0: 6e61 626c 6520 746f 206f 7065 6e20 6669  nable to open fi
+000108e0: 6c65 2027 202b 2066 696c 655f 6e61 6d65  le ' + file_name
+000108f0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00010900: 7475 726e 0a0a 2020 2020 2020 2020 7365  turn..        se
+00010910: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+00010920: 203d 2066 696c 650a 2020 2020 2020 2020   = file.        
+00010930: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+00010940: 6c65 5f6e 616d 6520 3d20 6669 6c65 5f6e  le_name = file_n
+00010950: 616d 650a 2020 2020 2020 2020 7365 6c66  ame.        self
+00010960: 2e5f 6375 7272 656e 745f 6669 6c65 5f6e  ._current_file_n
+00010970: 625f 6576 656e 7473 203d 2030 0a20 2020  b_events = 0.   
+00010980: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
+00010990: 6e74 5f66 696c 655f 6576 656e 745f 636f  nt_file_event_co
+000109a0: 756e 7465 7220 3d20 300a 0a0a 2020 2020  unter = 0...    
+000109b0: 2020 2020 2320 6669 6c65 206d 6574 6164      # file metad
+000109c0: 6174 610a 2020 2020 2020 2020 6966 2073  ata.        if s
+000109d0: 656c 662e 5f66 696c 655f 6d65 7461 6461  elf._file_metada
+000109e0: 7461 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ta is not None:.
+000109f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00010a00: 6b65 792c 7661 6c20 696e 2073 656c 662e  key,val in self.
+00010a10: 5f66 696c 655f 6d65 7461 6461 7461 2e69  _file_metadata.i
+00010a20: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00010a30: 2020 2020 2020 2020 6966 2028 6973 696e          if (isin
+00010a40: 7374 616e 6365 2876 616c 2c20 6e70 2e6e  stance(val, np.n
+00010a50: 6461 7272 6179 2920 616e 6420 7661 6c2e  darray) and val.
+00010a60: 6474 7970 652e 7479 7065 2069 7320 6e70  dtype.type is np
+00010a70: 2e73 7472 5f29 3a0a 2020 2020 2020 2020  .str_):.        
+00010a80: 2020 2020 2020 2020 2020 2020 6474 203d              dt =
+00010a90: 2068 3570 792e 7374 7269 6e67 5f64 7479   h5py.string_dty
+00010aa0: 7065 2829 0a20 2020 2020 2020 2020 2020  pe().           
+00010ab0: 2020 2020 2020 2020 2076 616c 203d 2076           val = v
+00010ac0: 616c 2e61 7374 7970 6528 6474 290a 2020  al.astype(dt).  
+00010ad0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010ae0: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+00010af0: 2e61 7474 7273 5b6b 6579 5d20 3d20 7661  .attrs[key] = va
+00010b00: 6c0a 2020 2020 2020 2020 7365 6c66 2e5f  l.        self._
+00010b10: 6375 7272 656e 745f 6669 6c65 2e61 7474  current_file.att
+00010b20: 7273 5b27 7072 6566 6978 275d 203d 2070  rs['prefix'] = p
+00010b30: 7265 6669 780a 2020 2020 2020 2020 7365  refix.        se
+00010b40: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+00010b50: 2e61 7474 7273 5b27 7365 7269 6573 5f6e  .attrs['series_n
+00010b60: 756d 275d 203d 2073 656c 662e 5f73 6572  um'] = self._ser
+00010b70: 6965 735f 6e75 6d0a 2020 2020 2020 2020  ies_num.        
+00010b80: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+00010b90: 6c65 2e61 7474 7273 5b27 6475 6d70 5f6e  le.attrs['dump_n
+00010ba0: 756d 275d 203d 2069 6e74 2864 756d 7029  um'] = int(dump)
+00010bb0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00010bc0: 2020 2320 6465 7465 6374 6f72 2063 6f6e    # detector con
+00010bd0: 6669 670a 2020 2020 2020 2020 6966 2073  fig.        if s
+00010be0: 656c 662e 5f64 6574 6563 746f 725f 636f  elf._detector_co
+00010bf0: 6e66 6967 2069 7320 6e6f 7420 4e6f 6e65  nfig is not None
+00010c00: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00010c10: 7220 636f 6e66 6967 5f6b 6579 2c63 6f6e  r config_key,con
+00010c20: 6669 675f 7661 6c20 696e 2073 656c 662e  fig_val in self.
+00010c30: 5f64 6574 6563 746f 725f 636f 6e66 6967  _detector_config
+00010c40: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00010c50: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00010c60: 6e73 7461 6e63 6528 636f 6e66 6967 5f76  nstance(config_v
+00010c70: 616c 2c64 6963 7429 3a0a 2020 2020 2020  al,dict):.      
+00010c80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010c90: 6c66 2e5f 6375 7272 656e 745f 6669 6c65  lf._current_file
+00010ca0: 5f64 6574 636f 6e66 6967 5f67 726f 7570  _detconfig_group
+00010cb0: 203d 2073 656c 662e 5f63 7572 7265 6e74   = self._current
+00010cc0: 5f66 696c 652e 6372 6561 7465 5f67 726f  _file.create_gro
+00010cd0: 7570 2863 6f6e 6669 675f 6b65 7929 0a20  up(config_key). 
+00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cf0: 2020 2066 6f72 206b 6579 2c76 616c 2069     for key,val i
+00010d00: 6e20 636f 6e66 6967 5f76 616c 2e69 7465  n config_val.ite
+00010d10: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+00010d20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00010d30: 2028 6973 696e 7374 616e 6365 2876 616c   (isinstance(val
+00010d40: 2c20 6e70 2e6e 6461 7272 6179 2920 616e  , np.ndarray) an
+00010d50: 6420 7661 6c2e 6474 7970 652e 7479 7065  d val.dtype.type
+00010d60: 2069 7320 6e70 2e73 7472 5f29 3a0a 2020   is np.str_):.  
+00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d80: 2020 2020 2020 2020 2020 6474 203d 2068            dt = h
+00010d90: 3570 792e 7374 7269 6e67 5f64 7479 7065  5py.string_dtype
+00010da0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00010db0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00010dc0: 616c 203d 2076 616c 2e61 7374 7970 6528  al = val.astype(
+00010dd0: 6474 290a 2020 2020 2020 2020 2020 2020  dt).            
+00010de0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010df0: 2e5f 6375 7272 656e 745f 6669 6c65 5f64  ._current_file_d
+00010e00: 6574 636f 6e66 6967 5f67 726f 7570 2e61  etconfig_group.a
+00010e10: 7474 7273 5b6b 6579 5d20 3d20 7661 6c0a  ttrs[key] = val.
+00010e20: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00010e30: 2023 2063 7265 6174 6520 6164 6320 6772   # create adc gr
+00010e40: 6f75 700a 2020 2020 2020 2020 6966 2073  oup.        if s
+00010e50: 656c 662e 5f61 6463 5f63 6f6e 6669 6720  elf._adc_config 
+00010e60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00010e70: 2020 2020 2020 2020 2066 6f72 2063 6f6e           for con
+00010e80: 6669 675f 6b65 792c 636f 6e66 6967 5f76  fig_key,config_v
+00010e90: 616c 2069 6e20 7365 6c66 2e5f 6164 635f  al in self._adc_
+00010ea0: 636f 6e66 6967 2e69 7465 6d73 2829 3a0a  config.items():.
+00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ec0: 6966 2069 7369 6e73 7461 6e63 6528 636f  if isinstance(co
+00010ed0: 6e66 6967 5f76 616c 2c64 6963 7429 3a0a  nfig_val,dict):.
+00010ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ef0: 2020 2020 7365 6c66 2e5f 6375 7272 656e      self._curren
+00010f00: 745f 6669 6c65 5f61 6463 5f67 726f 7570  t_file_adc_group
+00010f10: 2020 3d20 7365 6c66 2e5f 6375 7272 656e    = self._curren
+00010f20: 745f 6669 6c65 2e63 7265 6174 655f 6772  t_file.create_gr
+00010f30: 6f75 7028 636f 6e66 6967 5f6b 6579 290a  oup(config_key).
+00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f50: 2020 2020 666f 7220 6b65 792c 7661 6c20      for key,val 
+00010f60: 696e 2063 6f6e 6669 675f 7661 6c2e 6974  in config_val.it
+00010f70: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+00010f80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010f90: 6620 2869 7369 6e73 7461 6e63 6528 7661  f (isinstance(va
+00010fa0: 6c2c 206e 702e 6e64 6172 7261 7929 2061  l, np.ndarray) a
+00010fb0: 6e64 2076 616c 2e64 7479 7065 2e74 7970  nd val.dtype.typ
+00010fc0: 6520 6973 206e 702e 7374 725f 293a 0a20  e is np.str_):. 
+00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fe0: 2020 2020 2020 2020 2020 2064 7420 3d20             dt = 
+00010ff0: 6835 7079 2e73 7472 696e 675f 6474 7970  h5py.string_dtyp
+00011000: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011020: 7661 6c20 3d20 7661 6c2e 6173 7479 7065  val = val.astype
+00011030: 2864 7429 0a20 2020 2020 2020 2020 2020  (dt).           
+00011040: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011050: 662e 5f63 7572 7265 6e74 5f66 696c 655f  f._current_file_
+00011060: 6164 635f 6772 6f75 702e 6174 7472 735b  adc_group.attrs[
+00011070: 6b65 795d 203d 2076 616c 0a20 2020 2020  key] = val.     
+00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011090: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+000110a0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+000110b0: 2020 2020 2020 2020 0a20 2020 2064 6566          .    def
+000110c0: 205f 636c 6f73 655f 6669 6c65 2873 656c   _close_file(sel
+000110d0: 6629 3a0a 0a20 2020 2020 2020 2069 6620  f):..        if 
+000110e0: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+000110f0: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
+00011100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011110: 2e5f 6375 7272 656e 745f 6669 6c65 2e63  ._current_file.c
+00011120: 6c6f 7365 2829 0a20 200a 2020 2020 2020  lose().  .      
+00011130: 2020 2320 696e 6974 6961 6c69 7a65 0a20    # initialize. 
+00011140: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
+00011150: 7265 6e74 5f66 696c 6520 3d20 4e6f 6e65  rent_file = None
+00011160: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+00011170: 7572 7265 6e74 5f66 696c 655f 6e61 6d65  urrent_file_name
+00011180: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00011190: 7365 6c66 2e5f 6375 7272 656e 745f 6669  self._current_fi
+000111a0: 6c65 5f6e 625f 6576 656e 7473 203d 2030  le_nb_events = 0
+000111b0: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+000111c0: 7572 7265 6e74 5f66 696c 655f 6164 635f  urrent_file_adc_
+000111d0: 6772 6f75 7020 3d20 4e6f 6e65 0a20 2020  group = None.   
+000111e0: 2020 2020 2073 656c 662e 5f63 7572 7265       self._curre
+000111f0: 6e74 5f66 696c 655f 6465 7463 6f6e 6669  nt_file_detconfi
+00011200: 675f 6772 6f75 7020 3d20 4e6f 6e65 0a20  g_group = None. 
+00011210: 2020 2020 2020 2073 656c 662e 5f63 7572         self._cur
+00011220: 7265 6e74 5f66 696c 655f 6576 656e 745f  rent_file_event_
+00011230: 636f 756e 7465 7220 3d20 300a 0a0a 2020  counter = 0...  
+00011240: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00011250: 2020 2020 0a                                 .
```

### Comparing `pytesdaq-0.3.1/pytesdaq/io/redis.py` & `pytesdaq-0.3.3/pytesdaq/io/redis.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/processing/_iv_didv_tools.py` & `pytesdaq-0.3.3/pytesdaq/processing/_iv_didv_tools.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/processing/_iv_didv_tools_plotting.py` & `pytesdaq-0.3.3/pytesdaq/processing/_iv_didv_tools_plotting.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/processing/_process_iv_didv.py` & `pytesdaq-0.3.3/pytesdaq/processing/_process_iv_didv.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/processing/trigger.py` & `pytesdaq-0.3.3/pytesdaq/processing/trigger.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/scope/readout.py` & `pytesdaq-0.3.3/pytesdaq/scope/readout.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/scope/scope.py` & `pytesdaq-0.3.3/pytesdaq/scope/scope.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/sequencer/iv_didv.py` & `pytesdaq-0.3.3/pytesdaq/sequencer/iv_didv.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/sequencer/sequencer.py` & `pytesdaq-0.3.3/pytesdaq/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/sequencer/tc.py` & `pytesdaq-0.3.3/pytesdaq/sequencer/tc.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/utils/arg_utils.py` & `pytesdaq-0.3.3/pytesdaq/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/utils/connection_utils.py` & `pytesdaq-0.3.3/pytesdaq/utils/connection_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq/utils/remote.py` & `pytesdaq-0.3.3/pytesdaq/utils/remote.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/pytesdaq.egg-info/PKG-INFO` & `pytesdaq-0.3.3/pytesdaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.3.1
+Version: 0.3.3
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 
 # `pytesdaq`
```

### Comparing `pytesdaq-0.3.1/pytesdaq.egg-info/SOURCES.txt` & `pytesdaq-0.3.3/pytesdaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.1/setup.py` & `pytesdaq-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
       long_description = f.read()
 
 
 setup(name='pytesdaq',
-      version='0.3.1',
+      version='0.3.3',
       description='DAQ and Intruments control for TES development',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Bruno Serfass',
       author_email='serfass@berkeley.edu',
       url="https://github.com/spice-herald/pytesdaq",
       zip_safe = False,
```

