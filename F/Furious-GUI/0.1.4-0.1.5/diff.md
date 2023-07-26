# Comparing `tmp/Furious-GUI-0.1.4.tar.gz` & `tmp/Furious-GUI-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.1.4.tar", last modified: Wed Jul 26 11:28:02 2023, max compression
+gzip compressed data, was "Furious-GUI-0.1.5.tar", last modified: Wed Jul 26 23:54:34 2023, max compression
```

## Comparing `Furious-GUI-0.1.4.tar` & `Furious-GUI-0.1.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.325799 Furious-GUI-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.091125 Furious-GUI-0.1.4/Furious/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.138258 Furious-GUI-0.1.4/Furious/Action/
--rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Action/Connect.py
--rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Action/EditConfiguration.py
--rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Action/Exit.py
--rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Action/Export.py
--rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Action/Import.py
--rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Action/Language.py
--rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Action/Routing.py
--rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Action/Settings.py
--rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Action/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.153653 Furious-GUI-0.1.4/Furious/Core/
--rw-rw-rw-   0        0        0    19756 2023-07-25 08:47:36.000000 Furious-GUI-0.1.4/Furious/Core/Configuration.py
--rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Core/Core.py
--rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Core/Intellisense.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.075452 Furious-GUI-0.1.4/Furious/Data/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.153653 Furious-GUI-0.1.4/Furious/Data/font/
--rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.4/Furious/Data/font/CascadiaMono
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.185238 Furious-GUI-0.1.4/Furious/Data/hysteria/
--rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.4/Furious/Data/hysteria/bypass-mainland-China.acl
--rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.4/Furious/Data/hysteria/country.mmdb
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.216091 Furious-GUI-0.1.4/Furious/Data/xray/
--rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.4/Furious/Data/xray/geoip.dat
--rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.4/Furious/Data/xray/geosite.dat
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.216091 Furious-GUI-0.1.4/Furious/Gui/
--rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Gui/Action.py
--rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Gui/Icon.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.247528 Furious-GUI-0.1.4/Furious/Utility/
--rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.4/Furious/Utility/Constants.py
--rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Utility/Process.py
--rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Utility/Proxy.py
--rw-rw-rw-   0        0        0    42815 2023-07-26 11:22:03.000000 Furious-GUI-0.1.4/Furious/Utility/Resources.py
--rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Utility/Settings.py
--rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Utility/StartupOnBoot.py
--rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Utility/Theme.py
--rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Utility/Translator.py
--rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Utility/Utility.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Utility/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-26 11:18:03.000000 Furious-GUI-0.1.4/Furious/Version.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.294435 Furious-GUI-0.1.4/Furious/Widget/
--rw-rw-rw-   0        0        0     8812 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Widget/Application.py
--rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Widget/ConnectingProgressBar.py
--rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Widget/EditConfiguration.py
--rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Widget/ExportQRCode.py
--rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Widget/IndentSpinBox.py
--rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Widget/LogViewer.py
--rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Widget/SystemTrayIcon.py
--rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Widget/Widget.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/Widget/__init__.py
--rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/__init__.py
--rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.4/Furious/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:28:02.325799 Furious-GUI-0.1.4/Furious_GUI.egg-info/
--rw-rw-rw-   0        0        0     6894 2023-07-26 11:28:01.000000 Furious-GUI-0.1.4/Furious_GUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2023-07-26 11:28:01.000000 Furious-GUI-0.1.4/Furious_GUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:28:01.000000 Furious-GUI-0.1.4/Furious_GUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-26 11:28:01.000000 Furious-GUI-0.1.4/Furious_GUI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       82 2023-07-26 11:28:01.000000 Furious-GUI-0.1.4/Furious_GUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 11:28:01.000000 Furious-GUI-0.1.4/Furious_GUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     6894 2023-07-26 11:28:02.325799 Furious-GUI-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5881 2023-07-26 11:18:03.000000 Furious-GUI-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-26 11:28:02.325799 Furious-GUI-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2009 2023-07-25 08:58:53.000000 Furious-GUI-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.480729 Furious-GUI-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.121495 Furious-GUI-0.1.5/Furious/
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.199761 Furious-GUI-0.1.5/Furious/Action/
+-rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Action/Connect.py
+-rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Action/EditConfiguration.py
+-rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Action/Exit.py
+-rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Action/Export.py
+-rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Action/Import.py
+-rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Action/Language.py
+-rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Action/Routing.py
+-rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Action/Settings.py
+-rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Action/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.215301 Furious-GUI-0.1.5/Furious/Core/
+-rw-rw-rw-   0        0        0    19756 2023-07-25 08:47:36.000000 Furious-GUI-0.1.5/Furious/Core/Configuration.py
+-rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Core/Core.py
+-rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Core/Intellisense.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.105557 Furious-GUI-0.1.5/Furious/Data/
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.230631 Furious-GUI-0.1.5/Furious/Data/font/
+-rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.5/Furious/Data/font/CascadiaMono
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.246171 Furious-GUI-0.1.5/Furious/Data/hysteria/
+-rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.5/Furious/Data/hysteria/bypass-mainland-China.acl
+-rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.5/Furious/Data/hysteria/country.mmdb
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.277509 Furious-GUI-0.1.5/Furious/Data/xray/
+-rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.5/Furious/Data/xray/geoip.dat
+-rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.5/Furious/Data/xray/geosite.dat
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.308724 Furious-GUI-0.1.5/Furious/Gui/
+-rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Gui/Action.py
+-rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Gui/Icon.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.386792 Furious-GUI-0.1.5/Furious/Utility/
+-rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.5/Furious/Utility/Constants.py
+-rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Utility/Process.py
+-rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Utility/Proxy.py
+-rw-rw-rw-   0        0        0    42815 2023-07-26 11:22:03.000000 Furious-GUI-0.1.5/Furious/Utility/Resources.py
+-rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Utility/Settings.py
+-rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Utility/StartupOnBoot.py
+-rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Utility/Theme.py
+-rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Utility/Translator.py
+-rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Utility/Utility.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Utility/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-26 23:53:22.000000 Furious-GUI-0.1.5/Furious/Version.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.464937 Furious-GUI-0.1.5/Furious/Widget/
+-rw-rw-rw-   0        0        0     8709 2023-07-26 11:36:26.000000 Furious-GUI-0.1.5/Furious/Widget/Application.py
+-rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Widget/ConnectingProgressBar.py
+-rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Widget/EditConfiguration.py
+-rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Widget/ExportQRCode.py
+-rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Widget/IndentSpinBox.py
+-rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Widget/LogViewer.py
+-rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Widget/SystemTrayIcon.py
+-rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Widget/Widget.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/Widget/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/__init__.py
+-rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.5/Furious/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:54:34.480729 Furious-GUI-0.1.5/Furious_GUI.egg-info/
+-rw-rw-rw-   0        0        0     6940 2023-07-26 23:54:33.000000 Furious-GUI-0.1.5/Furious_GUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-07-26 23:54:33.000000 Furious-GUI-0.1.5/Furious_GUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 23:54:33.000000 Furious-GUI-0.1.5/Furious_GUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-26 23:54:33.000000 Furious-GUI-0.1.5/Furious_GUI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2023-07-26 23:54:33.000000 Furious-GUI-0.1.5/Furious_GUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 23:54:33.000000 Furious-GUI-0.1.5/Furious_GUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6940 2023-07-26 23:54:34.480729 Furious-GUI-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5924 2023-07-26 23:53:22.000000 Furious-GUI-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 23:54:34.480729 Furious-GUI-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2012 2023-07-26 23:53:22.000000 Furious-GUI-0.1.5/setup.py
```

### Comparing `Furious-GUI-0.1.4/Furious/Action/Connect.py` & `Furious-GUI-0.1.5/Furious/Action/Connect.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Action/Export.py` & `Furious-GUI-0.1.5/Furious/Action/Export.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Action/Import.py` & `Furious-GUI-0.1.5/Furious/Action/Import.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Action/Language.py` & `Furious-GUI-0.1.5/Furious/Action/Language.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Action/Routing.py` & `Furious-GUI-0.1.5/Furious/Action/Routing.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Action/Settings.py` & `Furious-GUI-0.1.5/Furious/Action/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Core/Configuration.py` & `Furious-GUI-0.1.5/Furious/Core/Configuration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Core/Core.py` & `Furious-GUI-0.1.5/Furious/Core/Core.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Core/Intellisense.py` & `Furious-GUI-0.1.5/Furious/Core/Intellisense.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Data/font/CascadiaMono` & `Furious-GUI-0.1.5/Furious/Data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.1.5/Furious/Data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Data/hysteria/country.mmdb` & `Furious-GUI-0.1.5/Furious/Data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Data/xray/geoip.dat` & `Furious-GUI-0.1.5/Furious/Data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Data/xray/geosite.dat` & `Furious-GUI-0.1.5/Furious/Data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Gui/Action.py` & `Furious-GUI-0.1.5/Furious/Gui/Action.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Utility/Constants.py` & `Furious-GUI-0.1.5/Furious/Utility/Constants.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Utility/Process.py` & `Furious-GUI-0.1.5/Furious/Utility/Process.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Utility/Proxy.py` & `Furious-GUI-0.1.5/Furious/Utility/Proxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Utility/Resources.py` & `Furious-GUI-0.1.5/Furious/Utility/Resources.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Utility/Settings.py` & `Furious-GUI-0.1.5/Furious/Utility/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.1.5/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Utility/Theme.py` & `Furious-GUI-0.1.5/Furious/Utility/Theme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Utility/Translator.py` & `Furious-GUI-0.1.5/Furious/Utility/Translator.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Utility/Utility.py` & `Furious-GUI-0.1.5/Furious/Utility/Utility.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Widget/Application.py` & `Furious-GUI-0.1.5/Furious/Widget/Application.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,18 +145,14 @@
         self.logStreamHandle = None
 
         self.themeDetector = None
         self.themeListenerThread = None
 
         self.MainWidget = None
 
-        # Shared action
-        self.ImportLinkAction = None
-        self.ImportJSONAction = None
-
     def __getattr__(self, key):
         try:
             return Settings.get(key)
         except AttributeError:
             raise
 
     def __setattr__(self, key, value):
```

### Comparing `Furious-GUI-0.1.4/Furious/Widget/ConnectingProgressBar.py` & `Furious-GUI-0.1.5/Furious/Widget/ConnectingProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Widget/EditConfiguration.py` & `Furious-GUI-0.1.5/Furious/Widget/EditConfiguration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Widget/ExportQRCode.py` & `Furious-GUI-0.1.5/Furious/Widget/ExportQRCode.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.1.5/Furious/Widget/IndentSpinBox.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Widget/LogViewer.py` & `Furious-GUI-0.1.5/Furious/Widget/LogViewer.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Widget/SystemTrayIcon.py` & `Furious-GUI-0.1.5/Furious/Widget/SystemTrayIcon.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/Widget/Widget.py` & `Furious-GUI-0.1.5/Furious/Widget/Widget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious/__main__.py` & `Furious-GUI-0.1.5/Furious/__main__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.1.5/Furious_GUI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.4
-Summary: A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.
+Version: 0.1.5
+Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: End Users/Desktop
@@ -93,14 +93,16 @@
 
     * For Linux users: type `sudo apt update && sudo apt install g++` and that should work out fine.
     * For Windows users: install [MinGW-w64](https://sourceforge.net/projects/mingw-w64/files/mingw-w64/)
       or [Cygwin](https://www.cygwin.com/) and make sure you have add them to PATH.
 
 ### Install Furious
 
+Furious requires Python 3.8 and above.
+
 ```
 pip install Furious-GUI
 ```
 
 If the installation is successful, you will have a executable script(or `.exe` on Windows) in your PATH(if it's not in
 the PATH, you can always add the script location to the PATH later). That's Furious's application entry point.
 
@@ -136,8 +138,8 @@
 | [mack-a/v2ray-agent](https://github.com/mack-a/v2ray-agent)       | v2ray-core/Xray-core/hysteria |            Yes             |         Yes          |
 | [zxcvos/Xray-script](https://github.com/zxcvos/Xray-script)       |           Xray-core           |            Yes             |          /           |
 | [aleskxyz/reality-ezpz](https://github.com/aleskxyz/reality-ezpz) |           Xray-core           |            Yes             |          /           |
 | [emptysuns/Hi_Hysteria](https://github.com/emptysuns/Hi_Hysteria) |           hysteria            |             No             |         Yes          |
 
 ## License
 
-License under [GPL v3.0](https://github.com/LorenEteval/Furious/blob/main/LICENSE)
+License under [GPL v3.0](https://github.com/LorenEteval/Furious/blob/main/LICENSE).
```

### Comparing `Furious-GUI-0.1.4/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.1.5/Furious_GUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/LICENSE` & `Furious-GUI-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.4/PKG-INFO` & `Furious-GUI-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.4
-Summary: A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.
+Version: 0.1.5
+Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: End Users/Desktop
@@ -93,14 +93,16 @@
 
     * For Linux users: type `sudo apt update && sudo apt install g++` and that should work out fine.
     * For Windows users: install [MinGW-w64](https://sourceforge.net/projects/mingw-w64/files/mingw-w64/)
       or [Cygwin](https://www.cygwin.com/) and make sure you have add them to PATH.
 
 ### Install Furious
 
+Furious requires Python 3.8 and above.
+
 ```
 pip install Furious-GUI
 ```
 
 If the installation is successful, you will have a executable script(or `.exe` on Windows) in your PATH(if it's not in
 the PATH, you can always add the script location to the PATH later). That's Furious's application entry point.
 
@@ -136,8 +138,8 @@
 | [mack-a/v2ray-agent](https://github.com/mack-a/v2ray-agent)       | v2ray-core/Xray-core/hysteria |            Yes             |         Yes          |
 | [zxcvos/Xray-script](https://github.com/zxcvos/Xray-script)       |           Xray-core           |            Yes             |          /           |
 | [aleskxyz/reality-ezpz](https://github.com/aleskxyz/reality-ezpz) |           Xray-core           |            Yes             |          /           |
 | [emptysuns/Hi_Hysteria](https://github.com/emptysuns/Hi_Hysteria) |           hysteria            |             No             |         Yes          |
 
 ## License
 
-License under [GPL v3.0](https://github.com/LorenEteval/Furious/blob/main/LICENSE)
+License under [GPL v3.0](https://github.com/LorenEteval/Furious/blob/main/LICENSE).
```

### Comparing `Furious-GUI-0.1.4/README.md` & `Furious-GUI-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 
     * For Linux users: type `sudo apt update && sudo apt install g++` and that should work out fine.
     * For Windows users: install [MinGW-w64](https://sourceforge.net/projects/mingw-w64/files/mingw-w64/)
       or [Cygwin](https://www.cygwin.com/) and make sure you have add them to PATH.
 
 ### Install Furious
 
+Furious requires Python 3.8 and above.
+
 ```
 pip install Furious-GUI
 ```
 
 If the installation is successful, you will have a executable script(or `.exe` on Windows) in your PATH(if it's not in
 the PATH, you can always add the script location to the PATH later). That's Furious's application entry point.
 
@@ -113,8 +115,8 @@
 | [mack-a/v2ray-agent](https://github.com/mack-a/v2ray-agent)       | v2ray-core/Xray-core/hysteria |            Yes             |         Yes          |
 | [zxcvos/Xray-script](https://github.com/zxcvos/Xray-script)       |           Xray-core           |            Yes             |          /           |
 | [aleskxyz/reality-ezpz](https://github.com/aleskxyz/reality-ezpz) |           Xray-core           |            Yes             |          /           |
 | [emptysuns/Hi_Hysteria](https://github.com/emptysuns/Hi_Hysteria) |           hysteria            |             No             |         Yes          |
 
 ## License
 
-License under [GPL v3.0](https://github.com/LorenEteval/Furious/blob/main/LICENSE)
+License under [GPL v3.0](https://github.com/LorenEteval/Furious/blob/main/LICENSE).
```

### Comparing `Furious-GUI-0.1.4/setup.py` & `Furious-GUI-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='Furious-GUI',
     version=__version__,
     license='GPL v3.0',
-    description='A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.',
+    description='A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Loren Eteval',
     author_email='loren.eteval@proton.me',
     url='https://github.com/LorenEteval/Furious',
     packages=find_packages(),
     package_data={'Furious': ['Data/**']},
```

