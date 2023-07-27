# Comparing `tmp/proctracer-0.0.20.tar.gz` & `tmp/proctracer-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.20.tar", last modified: Wed Jul 26 19:54:45 2023, max compression
+gzip compressed data, was "proctracer-0.0.21.tar", last modified: Thu Jul 27 06:23:07 2023, max compression
```

## Comparing `proctracer-0.0.20.tar` & `proctracer-0.0.21.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:54:45.644325 proctracer-0.0.20/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.20/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.20/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3521 2023-07-26 19:54:45.644325 proctracer-0.0.20/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2152 2023-07-26 19:41:27.000000 proctracer-0.0.20/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:54:45.644325 proctracer-0.0.20/proctracer/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-26 19:54:21.000000 proctracer-0.0.20/proctracer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:54:45.644325 proctracer-0.0.20/proctracer/plugins/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3310 2023-07-25 11:37:39.000000 proctracer-0.0.20/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 root         (0) root         (0)     6459 2023-07-25 11:38:03.000000 proctracer-0.0.20/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/plugin_base.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-07-25 10:45:01.000000 proctracer-0.0.20/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/proctracer.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:54:45.644325 proctracer-0.0.20/proctracer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3521 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-26 19:54:45.644325 proctracer-0.0.20/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4895 2023-07-26 19:20:43.000000 proctracer-0.0.20/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:07.071091 proctracer-0.0.21/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.21/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.21/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3670 2023-07-27 06:23:07.071091 proctracer-0.0.21/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-07-26 19:58:26.000000 proctracer-0.0.21/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:07.071091 proctracer-0.0.21/proctracer/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-27 06:22:52.000000 proctracer-0.0.21/proctracer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:07.071091 proctracer-0.0.21/proctracer/plugins/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.21/proctracer/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.21/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-07-25 11:37:39.000000 proctracer-0.0.21/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     6367 2023-07-27 05:46:38.000000 proctracer-0.0.21/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     5635 2023-07-27 05:41:06.000000 proctracer-0.0.21/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-07-27 06:09:24.000000 proctracer-0.0.21/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2023-07-25 10:45:01.000000 proctracer-0.0.21/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.21/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.21/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-07-27 05:38:46.000000 proctracer-0.0.21/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 root         (0) root         (0)     5153 2023-07-27 06:22:36.000000 proctracer-0.0.21/proctracer/proctracer.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 06:13:03.000000 proctracer-0.0.21/proctracer/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:23:07.071091 proctracer-0.0.21/proctracer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3670 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-27 06:23:07.000000 proctracer-0.0.21/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-27 06:23:07.071091 proctracer-0.0.21/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-07-26 19:20:43.000000 proctracer-0.0.21/setup.py
```

### Comparing `proctracer-0.0.20/LICENSE.md` & `proctracer-0.0.21/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.20/PKG-INFO` & `proctracer-0.0.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.20
+Version: 0.0.21
 Summary: /proc Tracer
 Home-page: https://github.com/david-kracht/proctracer
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
@@ -69,25 +69,32 @@
         
         $ stress -c 1 -t 5
         stress: info: [514601] dispatching hogs: 1 cpu, 0 io, 0 vm, 0 hdd
         stress: info: [514601] successful run completed in 5s
         
         $ proctracer stop
         Stop /proc Tracer (Daemon).
+        
+        $ tree ~/1
+        /home/user/1
+        └── 2
+            └── proc_report.pdf
         ```
         
         - Package and Upload
         Place token in ```~/.pypirc```, i.e
         
-        >[pypi]
-        >username = __token__
-        >password = pypi-AgEIcHlwa0A5vasXU4w
+        > [pypi]
+        > username = __token__
+        > password = pypi-AgEIcHlwa0A5vasXU4w
         
         
         ```bash
+        $ chmod 600 ~/.pypirc
+        
         $ sudo pip install twine
         
         $ python3 setup.py sdist bdist_wheel
         $ twine upload dist/*
         ```
 Keywords: package,proc ,trace
 Platform: UNKNOWN
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `proctracer-0.0.20/README.md` & `proctracer-0.0.21/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -58,23 +58,30 @@
 
 $ stress -c 1 -t 5
 stress: info: [514601] dispatching hogs: 1 cpu, 0 io, 0 vm, 0 hdd
 stress: info: [514601] successful run completed in 5s
 
 $ proctracer stop
 Stop /proc Tracer (Daemon).
+
+$ tree ~/1
+/home/user/1
+└── 2
+    └── proc_report.pdf
 ```
 
 - Package and Upload
 Place token in ```~/.pypirc```, i.e
 
->[pypi]
->username = __token__
->password = pypi-AgEIcHlwa0A5vasXU4w
+> [pypi]
+> username = __token__
+> password = pypi-AgEIcHlwa0A5vasXU4w
 
 
 ```bash
+$ chmod 600 ~/.pypirc
+
 $ sudo pip install twine
 
 $ python3 setup.py sdist bdist_wheel
 $ twine upload dist/*
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `proctracer-0.0.20/proctracer/plugins/__init__.py` & `proctracer-0.0.21/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.20/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.21/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.20/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.21/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.20/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.21/proctracer/plugins/net_udpX.plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 'time': entry['time'],
                 'socket': "%s -> %s (inode:%s)" % ( self.convert_hex_socket(entry['local_address']),  self.convert_hex_socket(entry['rem_address']), entry['inode'] ) ,
                 'tx_queue': int(h_tx_queue,16),
                 'rx_queue': int(h_rx_queue,16),
                 'drops': int(entry['drops']),
                 'drops-per-sec': 0.0 ,
                  }
-            print(new_sample[k])  
+
             if k in self.sample_old:
                 new_sample[k]['drops-per-sec'] = 1.0*( new_sample[k]['drops'] - self.sample_old[k]['drops'] ) / ( new_sample[k]['time'] - self.sample_old[k]['time'] )
                 if new_sample[k]['drops-per-sec'] < 0:
                     new_sample[k]['drops-per-sec']=0
                     
         return new_sample
 
@@ -140,15 +140,14 @@
 
 
 class net_udp6(net_udp4):
 
     def __init__(self,config_yaml):
         super().__init__(config_yaml=config_yaml)
         self.file='/proc/net/udp6'
-        #self.diff_on = 'tx_queue rx_queue drops'.split()
 
     def convert_hex_socket(self, hex_socket):
         h_addr, h_port = hex_socket.split(':')
         h_addr_list = ["".join(x) for x in zip(*[iter(str(h_addr))]*2)]
         h_addr_list = h_addr_list[:-4] + h_addr_list[:-5:-1] #reversed last 8 byte
         h_addr = ''.join(h_addr_list)
         h_addr_list = ["".join(x) for x in zip(*[iter(str(h_addr))]*4)]
```

### Comparing `proctracer-0.0.20/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.21/proctracer/plugins/pid_stat.plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             if pid not in self.new_pid_map or "cmdline" not in self.new_pid_map:
 
                 proc_data = self.proc_reader('/proc/%s/cmdline' % pid)
                     
                 if pid not in self.new_pid_map:
                     self.new_pid_map[pid] = {}
                     
-                self.new_pid_map[pid]["cmdline"]= proc_data[:-1].replace('\0', ' ').strip()
+                self.new_pid_map[pid]["cmdline"]= " ".join(proc_data[:-1].replace('\0', ' ').split())
             
             if not self.new_pid_map[pid]["cmdline"]:
                 continue
             
             skip = False 
             for pattern in self.blacklist_cmd_patterns:
                 if pattern in self.new_pid_map[pid]["cmdline"]:
```

### Comparing `proctracer-0.0.20/proctracer/plugins/plugin_base.py` & `proctracer-0.0.21/proctracer/plugins/plugin_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,23 +91,7 @@
         pass
 
     def run(self):
         pass
 
     def end(self):
         pass
-
-
-    # def periodicTaskFactory(self, period, function, args, kwargs ):
-
-    #     if self.name in self.taskPool:
-    #         self.taskPool[self.name]["pill2kill"].set()
-
-    #     pill2kill = threading.Event()
-
-    #     self.taskPool[self.name] = {
-    #         "pill2kill":pill2kill,
-    #         "thread":threading.Thread(name=self.name, target=self.task, args=( pill2kill, period,function, args, kwargs))
-    #         }
-
-    #     self.taskPool[self.name]["thread"].daemon = True
-    #     self.taskPool[self.name]["thread"].start()
```

### Comparing `proctracer-0.0.20/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.21/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.20/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.21/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.20/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.21/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.20/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.21/proctracer/plugins/text_pipe.plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,13 +71,13 @@
             for i in pivot_table.columns:
 
                 plt.plot( pivot_table[[i]].dropna(), label="%s" % (i),  marker = 'o')
                 plt.title("Events")
                 plt.xlabel("Time t [s]")
                 plt.ylabel("Events")
                 plt.yticks([])
-                plt.legend(title="Event Labels", fontsize='small', loc= 'upper right')
+                plt.legend(title="Event Labels", fontsize='small', loc= 'upper left')
                 
                 
 
         pdf.savefig(fig)
```

### Comparing `proctracer-0.0.20/proctracer/proctracer.py` & `proctracer-0.0.21/proctracer/proctracer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,60 +8,76 @@
 from string import Template
 from collections import defaultdict
 import argparse
 
 import functools
 from daemonize import Daemonize
 
-sys.dont_write_bytecode = True
-
 try:
     from . import plugins
 except:
     import plugins
 
 from plugin_proc_tracer_base import ProcTracerBase
 
+import ctypes, threading
+LIB = 'libcap.so.2'
+try:
+    libcap = ctypes.CDLL(LIB)
+except OSError:
+    print(
+        'Library {} not found. Unable to set thread name.'.format(LIB)
+    )
+else:
+    def _name_hack(self):
+        # PR_SET_NAME = 15
+        libcap.prctl(15, self.name.encode())
+        threading.Thread._bootstrap_original(self)
+
+    threading.Thread._bootstrap_original = threading.Thread._bootstrap
+    threading.Thread._bootstrap = _name_hack
+
 DEFAULT_CONFIG_YAML_PATH = "~/proctracer-config.yaml"
 
 DEFAULT_CONFIG_YAML= """
 report_name: proctracer-report
 report_output_path: ${HOME}
 pipe_path: ${HOME}/proctracer.pipe
 pid_path: ~/proctracer.pid
 plugins:
     text_pipe:
         active: true
-        period: 0.1
+        period: 0.2
     pressure_cpu:
         active: true
-        period: 0.5
+        period: 1.0
     pressure_io:
         active: true
-        period: 0.5
+        period: 1.0
     pressure_memory:
         active: true
-        period: 0.5
+        period: 1.0
     stat:
         active: true
-        period: 5.0
+        period: 7.0
     pid_stat:
         active: true
         period: 5.0
     net_dev:
         active: true
         period: 1.0
     net_snmp_udp:
         active: true
-        period: 0.3
-    net_udp4: &x
+        period: 0.2
+    net_udp4:
         active: true
         period: 0.2
-    #net_udp6:
-    #    <<: *x
+    net_udp6:
+        active: false
+        period: 0.2
 """
 
 def env_expand(string):
     env_dict = defaultdict(lambda: '')
     env_dict.update(**os.environ)
     return Template(string).substitute(env_dict)
```

### Comparing `proctracer-0.0.20/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.21/proctracer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.20
+Version: 0.0.21
 Summary: /proc Tracer
 Home-page: https://github.com/david-kracht/proctracer
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
@@ -69,25 +69,32 @@
         
         $ stress -c 1 -t 5
         stress: info: [514601] dispatching hogs: 1 cpu, 0 io, 0 vm, 0 hdd
         stress: info: [514601] successful run completed in 5s
         
         $ proctracer stop
         Stop /proc Tracer (Daemon).
+        
+        $ tree ~/1
+        /home/user/1
+        └── 2
+            └── proc_report.pdf
         ```
         
         - Package and Upload
         Place token in ```~/.pypirc```, i.e
         
-        >[pypi]
-        >username = __token__
-        >password = pypi-AgEIcHlwa0A5vasXU4w
+        > [pypi]
+        > username = __token__
+        > password = pypi-AgEIcHlwa0A5vasXU4w
         
         
         ```bash
+        $ chmod 600 ~/.pypirc
+        
         $ sudo pip install twine
         
         $ python3 setup.py sdist bdist_wheel
         $ twine upload dist/*
         ```
 Keywords: package,proc ,trace
 Platform: UNKNOWN
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `proctracer-0.0.20/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.21/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.20/setup.py` & `proctracer-0.0.21/setup.py`

 * *Files identical despite different names*

