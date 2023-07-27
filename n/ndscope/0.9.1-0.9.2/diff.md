# Comparing `tmp/ndscope-0.9.1.tar.gz` & `tmp/ndscope-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndscope-0.9.1.tar", last modified: Thu Dec 10 20:23:29 2020, max compression
+gzip compressed data, was "ndscope-0.9.2.tar", last modified: Wed Dec 16 20:13:30 2020, max compression
```

## Comparing `ndscope-0.9.1.tar` & `ndscope-0.9.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2020-12-10 20:23:29.563718 ndscope-0.9.1/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      375 2020-12-10 19:13:03.000000 ndscope-0.9.1/CHANGELOG.md
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1761 2018-10-26 19:38:05.000000 ndscope-0.9.1/COPYING
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    35068 2018-07-24 17:06:42.000000 ndscope-0.9.1/COPYING-GPL-3
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      162 2020-12-10 19:13:03.000000 ndscope-0.9.1/MANIFEST.in
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2932 2020-12-10 20:23:29.563718 ndscope-0.9.1/PKG-INFO
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1916 2020-12-10 19:13:03.000000 ndscope-0.9.1/README.md
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2020-12-10 20:23:29.559718 ndscope-0.9.1/ndscope/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      411 2020-12-10 20:02:02.000000 ndscope-0.9.1/ndscope/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11692 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/__main__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      116 2020-12-10 20:23:29.000000 ndscope-0.9.1/ndscope/__version__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4982 2020-11-09 18:24:05.000000 ndscope-0.9.1/ndscope/axisCtrlTemplate.ui
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1113 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/const.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     6600 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/cursors.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    19639 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/data.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     7979 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/export.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    10575 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/layout.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     9395 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/nds.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11291 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/plot.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11077 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/plotMenu.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    38211 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/scope.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    53877 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/scope.ui
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2020-12-10 20:23:29.563718 ndscope-0.9.1/ndscope/test/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       27 2018-10-31 10:06:58.000000 ndscope-0.9.1/ndscope/test/__init__.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2020-12-10 20:23:29.563718 ndscope-0.9.1/ndscope/test/templates/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      376 2020-11-09 18:24:05.000000 ndscope-0.9.1/ndscope/test/templates/test.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      530 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/test/templates/test0.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      559 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/test/templates/test1-1.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      559 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/test/templates/test1-2.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      385 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/test/templates/test1-3.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      501 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/test/templates/test1.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2653 2018-10-31 10:06:58.000000 ndscope-0.9.1/ndscope/test/templates/test2.stp
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1076 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/test/templates/test2.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      524 2018-10-31 10:06:58.000000 ndscope-0.9.1/ndscope/test/templates/test3.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1312 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/test/templates/test3.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2751 2020-11-09 18:24:05.000000 ndscope-0.9.1/ndscope/test/templates/test4.xml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1340 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/test/templates/test4.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2820 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/test/test_layout.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      413 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/test/test_window.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1794 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/trigger.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2689 2020-12-10 19:13:03.000000 ndscope-0.9.1/ndscope/util.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2020-12-10 20:23:29.563718 ndscope-0.9.1/ndscope.egg-info/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2932 2020-12-10 20:23:29.000000 ndscope-0.9.1/ndscope.egg-info/PKG-INFO
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1043 2020-12-10 20:23:29.000000 ndscope-0.9.1/ndscope.egg-info/SOURCES.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)        1 2020-12-10 20:23:29.000000 ndscope-0.9.1/ndscope.egg-info/dependency_links.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       51 2020-12-10 20:23:29.000000 ndscope-0.9.1/ndscope.egg-info/entry_points.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       80 2020-12-10 20:23:29.000000 ndscope-0.9.1/ndscope.egg-info/requires.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)        8 2020-12-10 20:23:29.000000 ndscope-0.9.1/ndscope.egg-info/top_level.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       38 2020-12-10 20:23:29.563718 ndscope-0.9.1/setup.cfg
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1383 2020-12-10 19:13:03.000000 ndscope-0.9.1/setup.py
+drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2020-12-16 20:13:30.494266 ndscope-0.9.2/
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      375 2020-12-12 01:47:00.000000 ndscope-0.9.2/CHANGELOG.md
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1761 2018-10-26 19:38:05.000000 ndscope-0.9.2/COPYING
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    35068 2018-07-24 17:06:42.000000 ndscope-0.9.2/COPYING-GPL-3
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      162 2020-12-12 01:47:00.000000 ndscope-0.9.2/MANIFEST.in
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2989 2020-12-16 20:13:30.494266 ndscope-0.9.2/PKG-INFO
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1965 2020-12-12 01:47:00.000000 ndscope-0.9.2/README.md
+drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2020-12-16 20:13:30.486266 ndscope-0.9.2/ndscope/
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      411 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/__init__.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11687 2020-12-16 19:54:59.000000 ndscope-0.9.2/ndscope/__main__.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      116 2020-12-16 20:13:30.000000 ndscope-0.9.2/ndscope/__version__.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4982 2020-11-09 18:24:05.000000 ndscope-0.9.2/ndscope/axisCtrlTemplate.ui
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1113 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/const.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     6600 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/cursors.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    19787 2020-12-16 19:54:59.000000 ndscope-0.9.2/ndscope/data.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     8639 2020-12-12 02:20:28.000000 ndscope-0.9.2/ndscope/export.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    10575 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/layout.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     9395 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/nds.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11337 2020-12-16 19:54:59.000000 ndscope-0.9.2/ndscope/plot.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11077 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/plotMenu.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    38249 2020-12-16 19:54:59.000000 ndscope-0.9.2/ndscope/scope.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)    53877 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/scope.ui
+drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2020-12-16 20:13:30.486266 ndscope-0.9.2/ndscope/test/
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)       27 2018-10-31 10:06:58.000000 ndscope-0.9.2/ndscope/test/__init__.py
+drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2020-12-16 20:13:30.494266 ndscope-0.9.2/ndscope/test/templates/
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      376 2020-11-09 18:24:05.000000 ndscope-0.9.2/ndscope/test/templates/test.yaml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      530 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/test/templates/test0.yaml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      559 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/test/templates/test1-1.yaml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      559 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/test/templates/test1-2.yaml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      385 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/test/templates/test1-3.yaml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      501 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/test/templates/test1.yaml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2653 2018-10-31 10:06:58.000000 ndscope-0.9.2/ndscope/test/templates/test2.stp
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1076 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/test/templates/test2.yaml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      524 2018-10-31 10:06:58.000000 ndscope-0.9.2/ndscope/test/templates/test3.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1312 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/test/templates/test3.yaml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2751 2020-11-09 18:24:05.000000 ndscope-0.9.2/ndscope/test/templates/test4.xml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1340 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/test/templates/test4.yaml
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2820 2020-12-10 19:13:03.000000 ndscope-0.9.2/ndscope/test/test_layout.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)      413 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/test/test_window.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1794 2020-12-12 01:47:00.000000 ndscope-0.9.2/ndscope/trigger.py
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2654 2020-12-16 19:54:59.000000 ndscope-0.9.2/ndscope/util.py
+drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2020-12-16 20:13:30.486266 ndscope-0.9.2/ndscope.egg-info/
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2989 2020-12-16 20:13:30.000000 ndscope-0.9.2/ndscope.egg-info/PKG-INFO
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1043 2020-12-16 20:13:30.000000 ndscope-0.9.2/ndscope.egg-info/SOURCES.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)        1 2020-12-16 20:13:30.000000 ndscope-0.9.2/ndscope.egg-info/dependency_links.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)       51 2020-12-16 20:13:30.000000 ndscope-0.9.2/ndscope.egg-info/entry_points.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)       80 2020-12-16 20:13:30.000000 ndscope-0.9.2/ndscope.egg-info/requires.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)        8 2020-12-16 20:13:30.000000 ndscope-0.9.2/ndscope.egg-info/top_level.txt
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)       38 2020-12-16 20:13:30.494266 ndscope-0.9.2/setup.cfg
+-rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1383 2020-12-12 01:47:00.000000 ndscope-0.9.2/setup.py
```

### Comparing `ndscope-0.9.1/COPYING` & `ndscope-0.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/COPYING-GPL-3` & `ndscope-0.9.2/COPYING-GPL-3`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/PKG-INFO` & `ndscope-0.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndscope
-Version: 0.9.1
+Version: 0.9.2
 Summary: Next-generation NDS time series plotting
 Home-page: https://git.ligo.org/cds/ndscope
 Author: Jameson Graef Rollins
 Author-email: jameson.rollins@ligo.org
 License: GPL-3.0-or-later
 Description: # Next-generation NDS oscilloscope
         
@@ -54,15 +54,16 @@
         
         * pyqt5-dev-tools
         * qt5-designer
         * python3-setuptools_scm
         * pytest3-pytest
         
         Pre-built binary packages are available via
-        [conda](https://anaconda.org/conda-forge/ndscope) and the various
+        [pip](https://pypi.org/projects/ndscope) and
+        [conda](https://anaconda.org/conda-forge/ndscope) and for the various
         [IGWN supported operating
         systems](https://computing.docs.ligo.org/guide/software/installation/).
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `ndscope-0.9.1/README.md` & `ndscope-0.9.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -46,10 +46,11 @@
 
 * pyqt5-dev-tools
 * qt5-designer
 * python3-setuptools_scm
 * pytest3-pytest
 
 Pre-built binary packages are available via
-[conda](https://anaconda.org/conda-forge/ndscope) and the various
+[pip](https://pypi.org/projects/ndscope) and
+[conda](https://anaconda.org/conda-forge/ndscope) and for the various
 [IGWN supported operating
 systems](https://computing.docs.ligo.org/guide/software/installation/).
```

### Comparing `ndscope-0.9.1/ndscope/__main__.py` & `ndscope-0.9.2/ndscope/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,32 +280,31 @@
         parser.error("Could not parse time window: {}:".format(args.time_window, e))
 
     if not window:
         window = template.get('time-window')
 
     if len(args.time) == 0:
         online = True
-        t0 = None
         if window:
             if isinstance(window, float):
                 window = (-window, 0)
         else:
             window = const.DEFAULT_TIME_WINDOW_ONLINE
     elif len(args.time) == 1:
         online = False
         t0 = args.time[0]
         if window:
             if isinstance(window, float):
                 window = (-window/2, window/2)
         else:
             window = const.DEFAULT_TIME_WINDOW_OFFLINE
+        kwargs = dict(t0=t0, window=window)
     elif len(args.time) == 2:
         online = False
-        t0 = min(args.time)
-        window = (0, abs(args.time[0] - args.time[1]))
+        kwargs = dict(start=min(args.time), end=max(args.time))
 
     ##########
     # launch app
 
     if args.gen_template:
         template['time-window'] = window
         print(yaml.safe_dump(template, default_style=False))
@@ -328,14 +327,14 @@
     elif online:
         scope.start(window)
     else:
         if args.file:
             def done_export():
                 scope.export(args.file)
             scope.data.signal_data_retrieve_done.connect(done_export)
-        scope.fetch(t0=t0, window=window)
+        scope.fetch(**kwargs)
 
     sys.exit(app.exec_())
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ndscope-0.9.1/ndscope/axisCtrlTemplate.ui` & `ndscope-0.9.2/ndscope/axisCtrlTemplate.ui`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/const.py` & `ndscope-0.9.2/ndscope/const.py`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/cursors.py` & `ndscope-0.9.2/ndscope/cursors.py`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/data.py` & `ndscope-0.9.2/ndscope/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,17 @@
         # FIXME: this is a hack way of doing this, and probably
         # doesn't perform well
         return list(self.data.values())[0].size
 
     def __getitem__(self, mod):
         return self.data[mod]
 
+    def __contains__(self, mod):
+        return mod in self.data
+
     def keys(self):
         return self.data.keys()
 
     def values(self):
         return self.data.values()
 
     def items(self):
@@ -394,14 +397,17 @@
         promptly emits signal_data with all on-hand data for trend,
         then triggers remote requests to fill in what is missing.
 
         `trend` should be one of ['raw', 'sec', 'min'], and
         `start_end` should be a tuple of (start, end) times.
 
         """
+        if not self.channels:
+            return
+
         logger.debug("REQUEST: {} {}".format(trend, start_end))
 
         self.last_trend = trend
 
         if self.online:
             if trend == 'min':
                 # no support for min trends.  the iteration time is
@@ -470,15 +476,15 @@
             self.remote_cmd(trend, 'extendleft', (rstart, dstart))
 
         if dend < rend:
             self.remote_cmd(trend, 'extend', (dend, rend))
 
     ##########
 
-    def _command_description(self, trend, cmd):
+    def _command_description(self, trend, cmd=None):
         if cmd == 'online':
             desc = 'online '
         else:
             desc = ''
         if trend == 'sec':
             desc += "second trend"
         elif trend == 'min':
@@ -520,15 +526,15 @@
         self.threads[tid] = t
 
     @Slot('PyQt_PyObject')
     def remote_recv(self, recv):
         logger.log(5, "")
         logger.log(5, "RECV: {}".format(recv))
         trend, cmd, buffers = recv
-        msg = "Receiving {} data...".format(trend)
+        msg = "Receiving {} data...".format(self._command_description(trend))
         if cmd == 'online':
             self.signal_data_online_start.emit(msg)
         else:
             self.signal_data_retrieve_start.emit(msg)
         # FIXME: should the NDS object just return this directly?
         dbd = DataBufferDict(buffers)
         if not self.db.get(trend):
```

### Comparing `ndscope-0.9.1/ndscope/export.py` & `ndscope-0.9.2/ndscope/export.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,58 +141,80 @@
 }
 
 
 ##################################################
 # EXPORT DATA
 
 
-def export_data_hdf5(ddict, path, **kwargs):
+class ExportData:
+    def __init__(self, datad, start, end):
+        self.sample_rate = datad.sample_rate
+        self.unit = datad.unit
+        ind = np.where(
+            (start <= datad.tarray) & (datad.tarray <= end),
+            True, False,
+        )
+        self.data = {}
+        for mod, data in datad.items():
+            self.data[mod] = data[ind]
+        self.gps_start = start
+        self.span = end - start
+
+    def items(self):
+        return self.data.items()
+
+def export_data_hdf5(ddict, path, start, end, **kwargs):
     """Save data dictionary to an HDF5 file
 
     Each channel key is given it's own group.  Keyword args written as
     attributes.
 
     """
     import h5py
     with h5py.File(path, 'w') as f:
         for chan, datad in ddict.items():
+            datad = ExportData(datad, start, end)
             grp = f.create_group(chan)
             for name, data in datad.items():
                 grp.create_dataset(name, data=data)
             # grp.create_dataset('gps', data=datad.tarray)
             grp.attrs['sample_rate'] = datad.sample_rate
             grp.attrs['gps_start'] = datad.gps_start
             grp.attrs['unit'] = datad.unit
         f.attrs.update(kwargs)
 
 
-def export_data_mat(ddict, path, **kwargs):
+def export_data_mat(ddict, path, start, end, **kwargs):
     """Save data dictionary to a MAT file
 
     """
     from scipy.io import savemat
     out = []
     for chan, datad in ddict.items():
+        datad = ExportData(datad, start, end)
         cd = OrderedDict([
             ('name', np.array(chan.encode('ascii'), dtype=np.string_)),
             ('data', {}),
             ('rate', datad.sample_rate),
             ('start', datad.gps_start),
             ('duration', datad.span),
+            ('unit', datad.unit),
         ])
         for t, d in datad.items():
             cd['data'][t] = d.reshape(-1, 1)
         out.append(cd)
     # turn dict list into record array to conversion to struct array
     # get dtypes from first element dict
     dtypes = [(k, type(v)) for k, v in out[0].items()]
     values = [tuple(el.values()) for el in out]
     out = np.array(values, dtype=dtypes)
     recout = out.view(np.recarray)
-    savemat(path, dict(data=recout))
+    out = kwargs
+    out['data'] = recout
+    savemat(path, out)
 
 
 DATA_EXPORT_FUNCTIONS = {
     '.hdf5': export_data_hdf5,
     '.h5': export_data_hdf5,
     '.mat': export_data_mat,
 }
```

### Comparing `ndscope-0.9.1/ndscope/layout.py` & `ndscope-0.9.2/ndscope/layout.py`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/nds.py` & `ndscope-0.9.2/ndscope/nds.py`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/plot.py` & `ndscope-0.9.2/ndscope/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     y   = [nan, nan,   2,   3,   4,   5, nan, nan, nan,   9,  10]
     out = [  0,   0,   0, nan, nan,   5,   5,   5,   5,   5, nan]
 
     We use this for indicating "bad" data regions in plots.
 
     """
-    out = np.empty_like(y)
+    out = np.empty_like(y, dtype=np.float)
     out[:] = np.nan
     nani = np.where(np.isnan(y))[0]
     ti = np.where(np.diff(nani) > 1)[0]
     if ti.size == 0:
         return out
     nstart = np.append(nani[0], nani[ti+1])
     nend = np.append(nani[ti], nani[-1]) + 1
@@ -265,15 +265,15 @@
                 brush=mmc
             )
         else:
             self.curves['fill'] = None
         # special curve for bad data (nans, infs)
         self.curves['bad'] = PlotDataItem(
             [0, 0],
-            pen=pg.mkPen('r', width=3, style=QtCore.Qt.DotLine)
+            pen=pg.mkPen('r', width=1, style=QtCore.Qt.DotLine)
         )
 
     def set_ctype(self, ctype):
         """Update the channel ctype
 
         Returns True if type changed, False otherwise
 
@@ -323,43 +323,49 @@
         """
         for curve in self.curves.values():
             try:
                 curve.setData(np.array([0, 0]))
             except:
                 pass
 
+    def _set_curve_data(self, mod, y, t):
+        # FIXME: HACK: replace all +-infs with nans.  the infs
+        # were causing the following exception in PlotCurveItem
+        # when it tried to find the min/max of the array:
+        # ValueError: zero-size array to reduction operation minimum which has no identity
+        # using nan is not great, since that's also an indicator
+        # of a gap, but not sure what else to use.
+        try:
+            np.place(y, np.isinf(y), np.nan)
+        except ValueError:
+            # this check throws a value error if y is int.  but in
+            # that case there's nothing we need to convert, so
+            # just pass
+            pass
+        self.curves[mod].setData(
+            x=t,
+            y=self.transform(y),
+            connect="finite",
+        )
+
     def set_data(self, data, t0):
         """set data for curves
 
         Data should be DataBuffer object.
 
         """
         t = data.tarray - t0
 
-        # iterate over all mods (raw, or mean/min/max) in the DataBuffer
-        for mod, y in data.items():
-            if mod in ['raw', 'mean']:
-                mod = 'y'
-            # FIXME: HACK: replace all +-infs with nans.  the infs
-            # were causing the following exception in PlotCurveItem
-            # when it tried to find the min/max of the array:
-            # ValueError: zero-size array to reduction operation minimum which has no identity
-            # using nan is not great, since that's also an indicator
-            # of a gap, but not sure what else to use.
-            try:
-                np.place(y, np.isinf(y), np.nan)
-            except ValueError:
-                # this check throws a value error if y is int.  but in
-                # that case there's nothing we need to convert, so
-                # just pass
-                pass
-            self.curves[mod].setData(
-                x=t,
-                y=self.transform(y),
-                connect="finite",
-            )
+        if 'raw' in data:
+            y = data['raw']
+        else:
+            y = data['mean']
+            for mod in ['min', 'max']:
+                self._set_curve_data(mod, data[mod], t)
+
+        self._set_curve_data('y', y, t)
 
         self.curves['bad'].setData(
             x=t,
             y=hold_over_nan(y),
             connect="finite",
         )
```

### Comparing `ndscope-0.9.1/ndscope/plotMenu.py` & `ndscope-0.9.2/ndscope/plotMenu.py`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/scope.py` & `ndscope-0.9.2/ndscope/scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,16 +524,16 @@
             t0 = kwargs['t0']
             window = kwargs['window']
             start = t0 + window[0]
             end = t0 + window[1]
         else:
             start = kwargs['start']
             end = kwargs['end']
-            t0 = (end+start)/2
-            window = (t0-start, t0-end)
+            t0 = max(start, end)
+            window = (-abs(start-end), 0)
         logger.info('FETCH: {}'.format((start, end)))
         self.triggerGroup.setChecked(False)
         self.set_t0(t0)
         self.set_window(window[0], window[1])
         self._data_request(force=True)
 
     def fetch(self, **kwargs):
@@ -1097,14 +1097,15 @@
         elif ext in export.DATA_EXPORT_FUNCTIONS:
             obj = 'data'
             export_func = export.DATA_EXPORT_FUNCTIONS[ext]
             trend = self.data.last_trend
             args = (
                 self.data.db[trend],
                 path,
+                *self.get_range()
             )
             kwargs = dict(
                 t0=self.t0,
                 window=self.get_window(),
             )
 
         elif ext in export.TEMPLATE_EXPORT_FUNCTIONS:
```

### Comparing `ndscope-0.9.1/ndscope/scope.ui` & `ndscope-0.9.2/ndscope/scope.ui`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/test/templates/test0.yaml` & `ndscope-0.9.2/ndscope/test/templates/test0.yaml`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/test/templates/test1-1.yaml` & `ndscope-0.9.2/ndscope/test/templates/test1-1.yaml`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/test/templates/test1-2.yaml` & `ndscope-0.9.2/ndscope/test/templates/test1-2.yaml`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/test/templates/test2.stp` & `ndscope-0.9.2/ndscope/test/templates/test2.stp`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/test/templates/test2.yaml` & `ndscope-0.9.2/ndscope/test/templates/test2.yaml`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/test/templates/test3.txt` & `ndscope-0.9.2/ndscope/test/templates/test3.txt`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/test/templates/test3.yaml` & `ndscope-0.9.2/ndscope/test/templates/test3.yaml`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/test/templates/test4.xml` & `ndscope-0.9.2/ndscope/test/templates/test4.xml`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/test/templates/test4.yaml` & `ndscope-0.9.2/ndscope/test/templates/test4.yaml`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/test/test_layout.py` & `ndscope-0.9.2/ndscope/test/test_layout.py`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/trigger.py` & `ndscope-0.9.2/ndscope/trigger.py`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/ndscope/util.py` & `ndscope-0.9.2/ndscope/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,17 +72,15 @@
     elif msec > 0:
         si = 5
     elif usec > 0:
         si = 6
     else:
         si = 7
     # this sets the precision, e.g. final time unit
-    if prec >= 8:
-        ei = 1
-    elif prec >= 5:
+    if prec >= 7:
         ei = 2
     elif prec >= 4:
         ei = 3
     elif prec >= 2:
         ei = 4
     elif prec >= 0:
         ei = 5
```

### Comparing `ndscope-0.9.1/ndscope.egg-info/PKG-INFO` & `ndscope-0.9.2/ndscope.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndscope
-Version: 0.9.1
+Version: 0.9.2
 Summary: Next-generation NDS time series plotting
 Home-page: https://git.ligo.org/cds/ndscope
 Author: Jameson Graef Rollins
 Author-email: jameson.rollins@ligo.org
 License: GPL-3.0-or-later
 Description: # Next-generation NDS oscilloscope
         
@@ -54,15 +54,16 @@
         
         * pyqt5-dev-tools
         * qt5-designer
         * python3-setuptools_scm
         * pytest3-pytest
         
         Pre-built binary packages are available via
-        [conda](https://anaconda.org/conda-forge/ndscope) and the various
+        [pip](https://pypi.org/projects/ndscope) and
+        [conda](https://anaconda.org/conda-forge/ndscope) and for the various
         [IGWN supported operating
         systems](https://computing.docs.ligo.org/guide/software/installation/).
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `ndscope-0.9.1/ndscope.egg-info/SOURCES.txt` & `ndscope-0.9.2/ndscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ndscope-0.9.1/setup.py` & `ndscope-0.9.2/setup.py`

 * *Files identical despite different names*

