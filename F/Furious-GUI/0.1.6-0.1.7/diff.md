# Comparing `tmp/Furious-GUI-0.1.6.tar.gz` & `tmp/Furious-GUI-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.1.6.tar", last modified: Thu Jul 27 00:28:46 2023, max compression
+gzip compressed data, was "Furious-GUI-0.1.7.tar", last modified: Thu Jul 27 01:16:38 2023, max compression
```

## Comparing `Furious-GUI-0.1.6.tar` & `Furious-GUI-0.1.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.473743 Furious-GUI-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.098334 Furious-GUI-0.1.6/Furious/
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.161047 Furious-GUI-0.1.6/Furious/Action/
--rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Action/Connect.py
--rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Action/EditConfiguration.py
--rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Action/Exit.py
--rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Action/Export.py
--rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Action/Import.py
--rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Action/Language.py
--rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Action/Routing.py
--rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Action/Settings.py
--rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Action/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.192067 Furious-GUI-0.1.6/Furious/Core/
--rw-rw-rw-   0        0        0    19756 2023-07-25 08:47:36.000000 Furious-GUI-0.1.6/Furious/Core/Configuration.py
--rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Core/Core.py
--rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Core/Intellisense.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.067201 Furious-GUI-0.1.6/Furious/Data/
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.207662 Furious-GUI-0.1.6/Furious/Data/font/
--rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.6/Furious/Data/font/CascadiaMono
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.226019 Furious-GUI-0.1.6/Furious/Data/hysteria/
--rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.6/Furious/Data/hysteria/bypass-mainland-China.acl
--rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.6/Furious/Data/hysteria/country.mmdb
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.270593 Furious-GUI-0.1.6/Furious/Data/xray/
--rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.6/Furious/Data/xray/geoip.dat
--rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.6/Furious/Data/xray/geosite.dat
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.286163 Furious-GUI-0.1.6/Furious/Gui/
--rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Gui/Action.py
--rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Gui/Icon.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.379812 Furious-GUI-0.1.6/Furious/Utility/
--rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.6/Furious/Utility/Constants.py
--rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Utility/Process.py
--rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Utility/Proxy.py
--rw-rw-rw-   0        0        0    42815 2023-07-26 11:22:03.000000 Furious-GUI-0.1.6/Furious/Utility/Resources.py
--rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Utility/Settings.py
--rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Utility/StartupOnBoot.py
--rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Utility/Theme.py
--rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Utility/Translator.py
--rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Utility/Utility.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Utility/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-27 00:27:00.000000 Furious-GUI-0.1.6/Furious/Version.py
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.442104 Furious-GUI-0.1.6/Furious/Widget/
--rw-rw-rw-   0        0        0     8709 2023-07-26 11:36:26.000000 Furious-GUI-0.1.6/Furious/Widget/Application.py
--rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Widget/ConnectingProgressBar.py
--rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Widget/EditConfiguration.py
--rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Widget/ExportQRCode.py
--rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Widget/IndentSpinBox.py
--rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Widget/LogViewer.py
--rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Widget/SystemTrayIcon.py
--rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Widget/Widget.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/Widget/__init__.py
--rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/__init__.py
--rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.6/Furious/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 00:28:46.473743 Furious-GUI-0.1.6/Furious_GUI.egg-info/
--rw-rw-rw-   0        0        0     6940 2023-07-27 00:28:45.000000 Furious-GUI-0.1.6/Furious_GUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2023-07-27 00:28:45.000000 Furious-GUI-0.1.6/Furious_GUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 00:28:45.000000 Furious-GUI-0.1.6/Furious_GUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-27 00:28:45.000000 Furious-GUI-0.1.6/Furious_GUI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2023-07-27 00:28:45.000000 Furious-GUI-0.1.6/Furious_GUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 00:28:45.000000 Furious-GUI-0.1.6/Furious_GUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     6940 2023-07-27 00:28:46.473743 Furious-GUI-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5924 2023-07-26 23:53:22.000000 Furious-GUI-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 00:28:46.473743 Furious-GUI-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2030 2023-07-27 00:27:00.000000 Furious-GUI-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.261416 Furious-GUI-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.120968 Furious-GUI-0.1.7/Furious/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.120968 Furious-GUI-0.1.7/Furious/Action/
+-rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Connect.py
+-rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/EditConfiguration.py
+-rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Exit.py
+-rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Export.py
+-rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Import.py
+-rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Language.py
+-rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Routing.py
+-rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/Settings.py
+-rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Action/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.136420 Furious-GUI-0.1.7/Furious/Core/
+-rw-rw-rw-   0        0        0    19756 2023-07-25 08:47:36.000000 Furious-GUI-0.1.7/Furious/Core/Configuration.py
+-rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Core/Core.py
+-rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Core/Intellisense.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.105147 Furious-GUI-0.1.7/Furious/Data/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.136420 Furious-GUI-0.1.7/Furious/Data/font/
+-rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/Furious/Data/font/CascadiaMono
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.136420 Furious-GUI-0.1.7/Furious/Data/hysteria/
+-rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/Furious/Data/hysteria/bypass-mainland-China.acl
+-rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/Furious/Data/hysteria/country.mmdb
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.183121 Furious-GUI-0.1.7/Furious/Data/xray/
+-rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/Furious/Data/xray/geoip.dat
+-rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/Furious/Data/xray/geosite.dat
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.214718 Furious-GUI-0.1.7/Furious/Gui/
+-rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Gui/Action.py
+-rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Gui/Icon.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.230103 Furious-GUI-0.1.7/Furious/Utility/
+-rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.7/Furious/Utility/Constants.py
+-rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Process.py
+-rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Proxy.py
+-rw-rw-rw-   0        0        0    42815 2023-07-26 11:22:03.000000 Furious-GUI-0.1.7/Furious/Utility/Resources.py
+-rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Settings.py
+-rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/StartupOnBoot.py
+-rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Theme.py
+-rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Translator.py
+-rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/Utility.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Utility/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-27 01:16:05.000000 Furious-GUI-0.1.7/Furious/Version.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.230103 Furious-GUI-0.1.7/Furious/Widget/
+-rw-rw-rw-   0        0        0     8709 2023-07-26 11:36:26.000000 Furious-GUI-0.1.7/Furious/Widget/Application.py
+-rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/ConnectingProgressBar.py
+-rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/EditConfiguration.py
+-rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/ExportQRCode.py
+-rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/IndentSpinBox.py
+-rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/LogViewer.py
+-rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/SystemTrayIcon.py
+-rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/Widget.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/Widget/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/__init__.py
+-rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.7/Furious/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:16:38.261416 Furious-GUI-0.1.7/Furious_GUI.egg-info/
+-rw-rw-rw-   0        0        0     6940 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      201 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 01:16:38.000000 Furious-GUI-0.1.7/Furious_GUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     6940 2023-07-27 01:16:38.261416 Furious-GUI-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5924 2023-07-26 23:53:22.000000 Furious-GUI-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 01:16:38.261416 Furious-GUI-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1886 2023-07-27 01:16:05.000000 Furious-GUI-0.1.7/setup.py
```

### Comparing `Furious-GUI-0.1.6/Furious/Action/Connect.py` & `Furious-GUI-0.1.7/Furious/Action/Connect.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Action/Export.py` & `Furious-GUI-0.1.7/Furious/Action/Export.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Action/Import.py` & `Furious-GUI-0.1.7/Furious/Action/Import.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Action/Language.py` & `Furious-GUI-0.1.7/Furious/Action/Language.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Action/Routing.py` & `Furious-GUI-0.1.7/Furious/Action/Routing.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Action/Settings.py` & `Furious-GUI-0.1.7/Furious/Action/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Core/Configuration.py` & `Furious-GUI-0.1.7/Furious/Core/Configuration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Core/Core.py` & `Furious-GUI-0.1.7/Furious/Core/Core.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Core/Intellisense.py` & `Furious-GUI-0.1.7/Furious/Core/Intellisense.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Data/font/CascadiaMono` & `Furious-GUI-0.1.7/Furious/Data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.1.7/Furious/Data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Data/hysteria/country.mmdb` & `Furious-GUI-0.1.7/Furious/Data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Data/xray/geoip.dat` & `Furious-GUI-0.1.7/Furious/Data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Data/xray/geosite.dat` & `Furious-GUI-0.1.7/Furious/Data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Gui/Action.py` & `Furious-GUI-0.1.7/Furious/Gui/Action.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Utility/Constants.py` & `Furious-GUI-0.1.7/Furious/Utility/Constants.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Utility/Process.py` & `Furious-GUI-0.1.7/Furious/Utility/Process.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Utility/Proxy.py` & `Furious-GUI-0.1.7/Furious/Utility/Proxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Utility/Resources.py` & `Furious-GUI-0.1.7/Furious/Utility/Resources.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Utility/Settings.py` & `Furious-GUI-0.1.7/Furious/Utility/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.1.7/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Utility/Theme.py` & `Furious-GUI-0.1.7/Furious/Utility/Theme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Utility/Translator.py` & `Furious-GUI-0.1.7/Furious/Utility/Translator.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Utility/Utility.py` & `Furious-GUI-0.1.7/Furious/Utility/Utility.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Widget/Application.py` & `Furious-GUI-0.1.7/Furious/Widget/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Widget/ConnectingProgressBar.py` & `Furious-GUI-0.1.7/Furious/Widget/ConnectingProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Widget/EditConfiguration.py` & `Furious-GUI-0.1.7/Furious/Widget/EditConfiguration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Widget/ExportQRCode.py` & `Furious-GUI-0.1.7/Furious/Widget/ExportQRCode.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.1.7/Furious/Widget/IndentSpinBox.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Widget/LogViewer.py` & `Furious-GUI-0.1.7/Furious/Widget/LogViewer.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Widget/SystemTrayIcon.py` & `Furious-GUI-0.1.7/Furious/Widget/SystemTrayIcon.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/Widget/Widget.py` & `Furious-GUI-0.1.7/Furious/Widget/Widget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious/__main__.py` & `Furious-GUI-0.1.7/Furious/__main__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.1.7/Furious_GUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.6
+Version: 0.1.7
 Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Furious-GUI-0.1.6/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.1.7/Furious_GUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/LICENSE` & `Furious-GUI-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/PKG-INFO` & `Furious-GUI-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.6
+Version: 0.1.7
 Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Furious-GUI-0.1.6/README.md` & `Furious-GUI-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.6/setup.py` & `Furious-GUI-0.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,12 @@
 from Furious.Version import __version__
 from Furious.Utility.Constants import PLATFORM
 
 from setuptools import setup, find_packages
 
-
-def get_install_requires():
-    requires = [
-        'wheel',
-        'PySide6-Essentials',
-        'Xray-core',
-        'hysteria',
-        'ujson',
-        'pybase64',
-        'pyqrcode',
-    ]
-
-    if PLATFORM == 'Windows':
-        requires.append('sysproxy')
-
-    if PLATFORM == 'Darwin':
-        requires.append('darkdetect[macos-listener]')
-    else:
-        requires.append('darkdetect')
-
-    return requires
-
-
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='Furious-GUI',
     version=__version__,
     license='GPL v3.0',
@@ -38,15 +15,26 @@
     long_description_content_type='text/markdown',
     author='Loren Eteval',
     author_email='loren.eteval@proton.me',
     url='https://github.com/LorenEteval/Furious',
     packages=find_packages(),
     package_data={'Furious': ['Data/**']},
     include_package_data=True,
-    install_requires=get_install_requires(),
+    install_requires=[
+        'wheel',
+        'PySide6-Essentials',
+        'Xray-core',
+        'hysteria',
+        'ujson',
+        'pybase64',
+        'pyqrcode',
+        'sysproxy; sys_platform == "win32"',
+        'darkdetect; sys_platform != "darwin"',
+        'darkdetect[macos-listener]; sys_platform == "darwin"',
+    ],
     entry_points={
         'gui_scripts': [
             'Furious = Furious.__main__:main',
         ],
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

