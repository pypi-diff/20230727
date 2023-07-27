# Comparing `tmp/wirepas_gateway-1.4.2rc1.tar.gz` & `tmp/wirepas_gateway-1.4.3rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wirepas_gateway-1.4.2rc1.tar", last modified: Fri May  6 15:57:57 2022, max compression
+gzip compressed data, was "wirepas_gateway-1.4.3rc4.tar", last modified: Thu Jul 27 09:32:25 2023, max compression
```

## Comparing `wirepas_gateway-1.4.2rc1.tar` & `wirepas_gateway-1.4.3rc4.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2022-05-06 15:57:57.131602 wirepas_gateway-1.4.2rc1/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)    11341 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/LICENSE
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     3398 2022-05-06 15:57:57.131602 wirepas_gateway-1.4.2rc1/PKG-INFO
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2165 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/README.md
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      114 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/requirements.txt
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)       38 2022-05-06 15:57:57.131602 wirepas_gateway-1.4.2rc1/setup.cfg
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     3102 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/setup.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2022-05-06 15:57:57.107602 wirepas_gateway-1.4.2rc1/wirepas_gateway/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      858 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/__about__.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      580 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/__init__.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      350 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/__main__.py
--rwxr-xr-x   0 wirepas   (1000) wirepas   (1000)     9859 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/configure_node.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2022-05-06 15:57:57.123602 wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      119 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/__init__.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2022-05-06 15:57:57.123602 wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/c-extension/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     6089 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/c-extension/dbus_c.c
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5857 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/dbus_client.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5125 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/return_code.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)    23097 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/sink_manager.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     1864 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus_print_client.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2022-05-06 15:57:57.127601 wirepas_gateway-1.4.2rc1/wirepas_gateway/protocol/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)        0 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/protocol/__init__.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)    13309 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/protocol/mqtt_wrapper.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5060 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/protocol/topic_helper.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)    33942 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/transport_service.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2022-05-06 15:57:57.131602 wirepas_gateway-1.4.2rc1/wirepas_gateway/utils/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      225 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/utils/__init__.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)    17263 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/utils/argument_tools.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     4486 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/utils/log_tools.py
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      852 2022-05-06 15:56:22.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway/utils/serialization_tools.py
-drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2022-05-06 15:57:57.119602 wirepas_gateway-1.4.2rc1/wirepas_gateway.egg-info/
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)     3398 2022-05-06 15:57:56.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway.egg-info/PKG-INFO
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      929 2022-05-06 15:57:57.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)        1 2022-05-06 15:57:56.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)      172 2022-05-06 15:57:56.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway.egg-info/entry_points.txt
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)       71 2022-05-06 15:57:56.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway.egg-info/requires.txt
--rw-r--r--   0 wirepas   (1000) wirepas   (1000)       31 2022-05-06 15:57:56.000000 wirepas_gateway-1.4.2rc1/wirepas_gateway.egg-info/top_level.txt
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-07-27 09:32:25.070500 wirepas_gateway-1.4.3rc4/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)    11341 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/LICENSE
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2837 2023-07-27 09:32:25.070500 wirepas_gateway-1.4.3rc4/PKG-INFO
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2165 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/README.md
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      120 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/requirements.txt
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)       38 2023-07-27 09:32:25.070500 wirepas_gateway-1.4.3rc4/setup.cfg
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     3102 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/setup.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-07-27 09:32:25.046500 wirepas_gateway-1.4.3rc4/wirepas_gateway/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      858 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/__about__.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      580 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/__init__.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      350 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/__main__.py
+-rwxr-xr-x   0 wirepas   (1000) wirepas   (1000)     9859 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/configure_node.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-07-27 09:32:25.062500 wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      119 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/__init__.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-07-27 09:32:25.062500 wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/c-extension/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     6089 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/c-extension/dbus_c.c
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5617 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/dbus_client.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5047 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/return_code.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)    24804 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/sink_manager.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2010 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus_print_client.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-07-27 09:32:25.066500 wirepas_gateway-1.4.3rc4/wirepas_gateway/protocol/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)        0 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/protocol/__init__.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)    13443 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/protocol/mqtt_wrapper.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     5060 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/protocol/topic_helper.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)    34541 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/transport_service.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-07-27 09:32:25.070500 wirepas_gateway-1.4.3rc4/wirepas_gateway/utils/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      200 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/utils/__init__.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)    17230 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/utils/argument_tools.py
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      852 2023-07-27 09:30:37.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway/utils/serialization_tools.py
+drwxr-sr-x   0 wirepas   (1000) wirepas   (1000)        0 2023-07-27 09:32:25.050500 wirepas_gateway-1.4.3rc4/wirepas_gateway.egg-info/
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)     2837 2023-07-27 09:32:24.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      894 2023-07-27 09:32:25.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)        1 2023-07-27 09:32:24.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)      171 2023-07-27 09:32:24.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway.egg-info/entry_points.txt
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)       75 2023-07-27 09:32:24.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway.egg-info/requires.txt
+-rw-r--r--   0 wirepas   (1000) wirepas   (1000)       31 2023-07-27 09:32:24.000000 wirepas_gateway-1.4.3rc4/wirepas_gateway.egg-info/top_level.txt
```

### Comparing `wirepas_gateway-1.4.2rc1/LICENSE` & `wirepas_gateway-1.4.3rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.2rc1/PKG-INFO` & `wirepas_gateway-1.4.3rc4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 Metadata-Version: 2.1
 Name: wirepas_gateway
-Version: 1.4.2rc1
+Version: 1.4.3rc4
 Summary: Wirepas gateway transport service that connects the local dbus to a remote MQTT broker.
 Home-page: https://github.com/wirepas/gateway
 Author: Wirepas Ltd
 Author-email: opensource@wirepas.com
 License: Apache-2
-Description: # Wirepas Gateway Transport Service
-        [![Documentation Status](https://readthedocs.org/projects/wirepas-gateway/badge/?version=latest)](https://wirepas-gateway.readthedocs.io/en/latest/?badge=latest)
-        
-        ## Building the wheel
-        
-        To build the source distribution and wheel file, make sure you have the
-        wheel package installed
-        
-        ```shell
-           pip install wheel
-        ```
-        and then run
-        
-        ```shell
-           py3clean .
-           python3 setup.py clean --all
-           python3 setup.py sdist bdist_wheel
-        ```
-        
-        A convenience script is available from the [utils folder][here_utils_wheel].
-        
-        ## Installation
-        
-        Before you attempt to build and install this package, please ensure that
-        you have [all the requirements met][wm_gateway_requirements].
-        
-        We highly recommend that you make your installation under a python virtual
-        environment such as [virtualenv][virtualenv] or [pipenv][pipenv].
-        
-        To install this package run (use -e for development mode)
-        
-        ```shell
-           pip install [-e] .
-        ```
-        
-        ## Running inside a virtual environment
-        
-        When running inside a virtual environment you will need to provide access
-        to system libraries. You can achieve this by using *--system-site-packages*
-        when setting up your environment or through [vext][vext].
-        
-        If you opt to install [vext][vext], please install the
-        [PyGObject][pygobject] module with:
-        
-        ```shell
-           pip install vext vext.gi
-        ```
-        
-        You also need to ensure that the following packages are installed inside
-        the virtual environment (as well as their system dependencies):
-        
-        ```shell
-           pip install pygobject gobject
-        ```
-        
-        ## Starting the service
-        
-        Please read on
-        [how to configure and start the transport service][wm_gateway_transport_conf]
-        
-        [wm_gateway_transport_conf]: https://github.com/wirepas/gateway/blob/master/README.md#transport-service-configuration
-        [wm_gateway_requirements]: https://github.com/wirepas/gateway/blob/master/README.md#linux-requirements
-        [here_utils_wheel]: https://github.com/wirepas/gateway/blob/update-readme/python_transport/utils/generate_wheel.sh
-        
-        [virtualenv]: https://docs.python.org/3/tutorial/venv.html
-        [pipenv]: https://github.com/pypa/pipenv
-        [vext]: https://github.com/stuaxo/vext
-        
-        [pygobject]: https://pygobject.readthedocs.io/en/latest/index.html
-        
 Keywords: wirepas connectivity iot mesh
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Wirepas Gateway Transport Service
+[![Documentation Status](https://readthedocs.org/projects/wirepas-gateway/badge/?version=latest)](https://wirepas-gateway.readthedocs.io/en/latest/?badge=latest)
+
+## Building the wheel
+
+To build the source distribution and wheel file, make sure you have the
+wheel package installed
+
+```shell
+   pip install wheel
+```
+and then run
+
+```shell
+   py3clean .
+   python3 setup.py clean --all
+   python3 setup.py sdist bdist_wheel
+```
+
+A convenience script is available from the [utils folder][here_utils_wheel].
+
+## Installation
+
+Before you attempt to build and install this package, please ensure that
+you have [all the requirements met][wm_gateway_requirements].
+
+We highly recommend that you make your installation under a python virtual
+environment such as [virtualenv][virtualenv] or [pipenv][pipenv].
+
+To install this package run (use -e for development mode)
+
+```shell
+   pip install [-e] .
+```
+
+## Running inside a virtual environment
+
+When running inside a virtual environment you will need to provide access
+to system libraries. You can achieve this by using *--system-site-packages*
+when setting up your environment or through [vext][vext].
+
+If you opt to install [vext][vext], please install the
+[PyGObject][pygobject] module with:
+
+```shell
+   pip install vext vext.gi
+```
+
+You also need to ensure that the following packages are installed inside
+the virtual environment (as well as their system dependencies):
+
+```shell
+   pip install pygobject gobject
+```
+
+## Starting the service
+
+Please read on
+[how to configure and start the transport service][wm_gateway_transport_conf]
+
+[wm_gateway_transport_conf]: https://github.com/wirepas/gateway/blob/master/README.md#transport-service-configuration
+[wm_gateway_requirements]: https://github.com/wirepas/gateway/blob/master/README.md#linux-requirements
+[here_utils_wheel]: https://github.com/wirepas/gateway/blob/update-readme/python_transport/utils/generate_wheel.sh
+
+[virtualenv]: https://docs.python.org/3/tutorial/venv.html
+[pipenv]: https://github.com/pypa/pipenv
+[vext]: https://github.com/stuaxo/vext
+
+[pygobject]: https://pygobject.readthedocs.io/en/latest/index.html
```

### Comparing `wirepas_gateway-1.4.2rc1/README.md` & `wirepas_gateway-1.4.3rc4/README.md`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.2rc1/setup.py` & `wirepas_gateway-1.4.3rc4/setup.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/__about__.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/__about__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 ]
 __copyright__ = "2019 Wirepas Ltd"
 __description__ = "Wirepas gateway transport service that connects the local dbus to a remote MQTT broker."
 __license__ = "Apache-2"
 __pkg_name__ = "wirepas_gateway"
 __title__ = "Wirepas Gateway Transport Service"
 __url__ = "https://github.com/wirepas/gateway"
-__version__ = "1.4.2rc1"
+__version__ = "1.4.3rc4"
 __keywords__ = "wirepas connectivity iot mesh"
```

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/__init__.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/configure_node.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/configure_node.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/c-extension/dbus_c.c` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/c-extension/dbus_c.c`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/dbus_client.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/dbus_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,75 +13,67 @@
 class DbusEventHandler(Thread):
     """
     Dedicated Thread to manage DBUS messages signals in C
     The thread is created in Python world but its real execution is
     delegated to C through a Python C extension
     """
 
-    def __init__(self, cb, logger):
+    def __init__(self, cb):
         """
         Initialize the C module wrapper
         :param cb: Python Callback to call from C on packet reception
         """
         Thread.__init__(self)
 
-        # logger
-        self.logger = logger
 
         dbusCExtension.setCallback(cb)
         self.daemon = True  # Daemonize thread
 
     def run(self) -> None:
         """
         Delegate the execution to C Extension
         :return: None, as it is an infinite loop in C
         """
         while True:
             dbusCExtension.infiniteEventLoop()
-            self.logger.error("C extension loop has exited")
+            logging.error("C extension loop has exited")
 
 
 class BusClient:
     """
     Base class to use to implement a DbusClient using the sink services
     It automatically manage sink connection/disconnection and offers some abstraction
     of dbus
     """
 
-    def __init__(self, logger=None, c_extension=True, ignored_ep_filter=None):
-
-        # logger
-        self.logger = logger or logging.getLogger(__name__)
+    def __init__(self, c_extension=True, ignored_ep_filter=None):
 
         # Main loop for events
         self.loop = GLib.MainLoop()
 
         # Connect to session bus
         self.bus = SystemBus()
 
         # Manage sink list
         self.sink_manager = SinkManager(
             bus=self.bus,
             on_new_sink_cb=self.on_sink_connected,
             on_sink_removal_cb=self.on_sink_disconnected,
             on_stack_started=self.on_stack_started,
             on_stack_stopped=self.on_stack_stopped,
-            logger=self.logger,
         )
 
         self.ignore_ep_filter = ignored_ep_filter
 
         # Register for packet on Dbus
         if c_extension:
-            self.logger.info("Starting dbus client with c extension")
-            self.c_extension_thread = DbusEventHandler(
-                self._on_data_received_c, self.logger
-            )
+            logging.info("Starting dbus client with c extension")
+            self.c_extension_thread = DbusEventHandler(self._on_data_received_c)
         else:
-            self.logger.info("Starting dbus client without c extension")
+            logging.info("Starting dbus client without c extension")
             # Subscribe to all massages received from any sink (no need for
             # connected sink for that)
             self.bus.subscribe(
                 signal="MessageReceived",
                 object="/com/wirepas/sink",
                 signal_fired=self._on_data_received,
             )
@@ -100,15 +92,15 @@
         qos,
         hop_count,
         data,
     ):
 
         # Could be done in C extension if needed by providing list to extension
         if self.ignore_ep_filter is not None and dst_ep in self.ignore_ep_filter:
-            self.logger.debug("Message received on ep %s filtered out", dst_ep)
+            logging.debug("Message received on ep %s filtered out", dst_ep)
             return
 
         # Get sink name from sender unique name
         name = self.sink_manager.get_sink_name(sender)
         self.on_data_received(
             sink_id=name,
             timestamp=timestamp,
@@ -123,15 +115,15 @@
         )
 
     def _on_data_received(self, sender, object, iface, signal, params):
         # pylint: disable=unused-argument
         # pylint: disable=redefined-builtin
         # filter out endpoint
         if self.ignore_ep_filter is not None and params[4] in self.ignore_ep_filter:
-            self.logger.debug("Message received on ep %s filtered out", params[4])
+            logging.debug("Message received on ep %s filtered out", params[4])
             return
 
         # Get sink name from sender unique name
         name = self.sink_manager.get_sink_name(sender)
         self.on_data_received(
             sink_id=name,
             timestamp=params[0],
```

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/return_code.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/return_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,15 @@
             # APP_RES_NO_SCRATCHPAD_START, No scratchpad start request sent
             (18, GatewayResultCode.GW_RES_INTERNAL_ERROR),
             # APP_RES_NO_VALID_SCRATCHPAD, No valid scratchpad
             (19, GatewayResultCode.GW_RES_NO_SCRATCHPAD_PRESENT),
             # APP_RES_NOT_A_SINK, Stack is not a sink
             (20, GatewayResultCode.GW_RES_INTERNAL_ERROR),
             # APP_RES_OUT_OF_MEMORY, Out of memory
-            # TODO Change error code to GW_RES_SINK_OUT_OF_MEMORY in next release
-            (21, GatewayResultCode.GW_RES_INTERNAL_ERROR),
+            (21, GatewayResultCode.GW_RES_SINK_OUT_OF_MEMORY),
             # APP_RES_INVALID_DIAG_INTERVAL, Invalid diag interval
             (22, GatewayResultCode.GW_RES_INVALID_DIAG_INTERVAL),
             # APP_RES_INVALID_SEQ,  Invalid sequence number
             (23, GatewayResultCode.GW_RES_INVALID_SEQUENCE_NUMBER),
             # APP_RES_INVALID_START_ADDRESS, Start address is invalid
             (24, GatewayResultCode.GW_RES_INTERNAL_ERROR),
             # APP_RES_INVALID_NUMBER_OF_BYTES, Invalid number of bytes
```

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus/sink_manager.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus/sink_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,25 @@
 from .return_code import ReturnCode
 
 
 DBUS_SINK_PREFIX = "com.wirepas.sink."
 
 
 class Sink:
-    def __init__(self, bus, proxy, sink_id, unique_name, on_stack_started, on_stack_stopped, logger=None):
+    def __init__(self, bus, proxy, sink_id, unique_name, on_stack_started, on_stack_stopped):
 
         self.proxy = proxy
         self.sink_id = sink_id
         self.network_address = None
         self.on_stack_started = on_stack_started
         self.on_stack_stopped = on_stack_stopped
         self.bus = bus
         self.unique_name = unique_name
         self.on_started_handle = None
 
-        self.logger = logger or logging.getLogger(__name__)
-
     def register_for_stack_started(self):
         # Use the subscribe directly to be able to specify the sender
         self.on_started_handle = self.bus.subscribe(
             signal="StackStarted",
             object="/com/wirepas/sink",
             iface="com.wirepas.sink.config1",
             sender=self.unique_name,
@@ -52,15 +50,15 @@
 
     def get_network_address(self, force=False):
         if self.network_address is None or force:
             # Network address is not known or must be updated
             try:
                 self.network_address = self.proxy.NetworkAddress
             except GLib.Error:
-                self.logger.error("Could not get network address")
+                logging.error("Could not get network address")
 
         return self.network_address
 
     def send_data(
         self,
         dst,
         src_ep,
@@ -69,32 +67,33 @@
         initial_time,
         data,
         is_unack_csma_ca=False,
         hop_limit=0,
     ):
         try:
             res = self.proxy.SendMessage(
-                dst,
+                # For some reason on some arch, uint32 are not correctly handled
+                dst & 0xFFFFFFFF,
                 src_ep,
                 dst_ep,
                 initial_time,
                 qos,
                 is_unack_csma_ca,
                 hop_limit,
                 data,
             )
             if res != 0:
-                self.logger.error("Cannot send message err=%s", res)
+                logging.error("Cannot send message err=%s", res)
                 return ReturnCode.error_from_dbus_return_code(res)
         except GLib.Error as e:
-            self.logger.exception("Fail to send message: %s", str(e))
+            logging.exception("Fail to send message: %s", str(e))
             return ReturnCode.error_from_dbus_exception(str(e))
         except OverflowError:
             # It may happens as protobuf has bigger container value
-            self.logger.error("Invalid range value")
+            logging.error("Invalid range value")
             return wmm.GatewayResultCode.GW_RES_INVALID_PARAM
 
         return wmm.GatewayResultCode.GW_RES_OK
 
     def _on_stack_started(self, sender, object, iface, signal, params):
         # pylint: disable=unused-argument
         # pylint: disable=redefined-builtin
@@ -108,41 +107,41 @@
 
     def _get_param(self, dic, key, attribute):
         try:
             dic[key] = getattr(self.proxy, attribute)
         except  GLib.Error:
             if key != "channel_map":
                 # Warning and not an error as normal behavior if not set
-                self.logger.warning("Cannot get %s in config (is it set?)", key)
+                logging.warning("Cannot get %s in config (is it set?)", key)
 
         except AttributeError :
-            self.logger.warning("Attribute %s doesn't exist", key)
+            logging.warning("Attribute %s doesn't exist", key)
 
     def _get_pair_params(self, dic, key1, att1, key2, att2):
         # Some settings are only relevant if the both can be retrieved
         try:
             att1_val = getattr(self.proxy, att1)
             att2_val = getattr(self.proxy, att2)
         except GLib.Error:
-            self.logger.debug("Cannot get one of the pair value (%s-%s)", key1, key2)
+            logging.debug("Cannot get one of the pair value (%s-%s)", key1, key2)
             return
 
         dic[key1] = att1_val
         dic[key2] = att2_val
 
     def read_config(self):
         config = {}
         config["sink_id"] = self.sink_id
 
         # Should always be available
         try:
             config["started"] = (self.proxy.StackStatus & 0x01) == 0
         except GLib.Error as e:
             error = ReturnCode.error_from_dbus_exception(str(e))
-            self.logger.exception("Cannot get Stack state: %s", error)
+            logging.exception("Cannot get Stack state: %s", error)
             return None
 
         self._get_param(config, "node_address", "NodeAddress")
         self._get_param(config, "node_role", "NodeRole")
         self._get_param(config, "network_address", "NetworkAddress")
         self._get_param(config, "network_channel", "NetworkChannel")
         self._get_param(config, "channel_map", "ChannelMap")
@@ -158,66 +157,76 @@
         self._get_param(config, "app_config_max_size", "AppConfigMaxSize")
 
         try:
             are_keys_set = self.proxy.AuthenticationKeySet and self.proxy.CipherKeySet
 
             config["are_keys_set"] = are_keys_set
         except GLib.Error:
-            self.logger.error("Cannot get key status")
+            logging.error("Cannot get key status")
 
         try:
             seq, diag, data = self.proxy.GetAppConfig()
             config["app_config_seq"] = seq
             config["app_config_diag"] = diag
             config["app_config_data"] = bytearray(data)
         except GLib.Error:
             # If node is blank it is not a sink
             # so app config cannot be accessed
-            self.logger.warning("Cannot get App Config")
+            logging.warning("Cannot get App Config")
+
+        # Add scratchpad related info
+        self.get_scratchpad_status(config)
 
         return config
 
     def _set_param(self, dic, key, attribute):
         try:
             value = dic[key]
             # Stop the stack if not already stopped
             if self.proxy.StackStatus == 0:
                 self.proxy.SetStackState(False)
 
             setattr(self.proxy, attribute, value)
 
         except KeyError:
             # key not defined in config
-            self.logger.debug("key not present: %s", key)
+            logging.debug("key not present: %s", key)
         except GLib.Error as e:
             # Exception raised when setting attribute
-            self.logger.error(
+            logging.error(
                 "Cannot set %s for param %s on sink %s: %s",
                 value,
                 key,
                 self.sink_id,
                 str(e),
             )
             return ReturnCode.error_from_dbus_exception(str(e))
         except OverflowError:
             # It may happens as protobuf has bigger container value
-            self.logger.error(
+            logging.error(
                 "Invalid range value for param %s with value %s", key, value
             )
             return wmm.GatewayResultCode.GW_RES_INVALID_PARAM
 
         return wmm.GatewayResultCode.GW_RES_OK
 
     def write_config(self, config):
+        # Force the node address if used
+        try:
+            # For some reason on some arch, uint32 are not correctly handled and result to an overflow
+            config["node_address"] = config["node_address"] & 0xFFFFFFFF
+        except KeyError:
+            # Node addess is not in the config
+            pass
         # Should always be available
         try:
             stack_started = (self.proxy.StackStatus & 0x01) == 0
         except GLib.Error as e:
             res = ReturnCode.error_from_dbus_exception(str(e))
-            self.logger.error(
+            logging.error(
                 "Cannot get Stack state. Problem in communication probably: %s",
                 res.name,
             )
             return res
 
         # The write config has only one return code possible
         # so the last error code will be returned
@@ -245,46 +254,46 @@
 
         # Set app_config after node role config in case role was not sink before
         try:
             seq = config["app_config_seq"]
             diag = config["app_config_diag"]
             data = config["app_config_data"]
 
-            self.logger.info("Set app config with %s", config)
+            logging.info("Set app config with %s", config)
             self.proxy.SetAppConfig(seq, diag, data)
         except KeyError:
             # App config not defined in new config
-            self.logger.debug("Missing key app_config key in config: %s", config)
+            logging.debug("Missing key app_config key in config: %s", config)
         except GLib.Error as e:
             res = ReturnCode.error_from_dbus_exception(str(e))
-            self.logger.error("Cannot set App Config: %s", res.name)
+            logging.error("Cannot set App Config: %s", res.name)
         except OverflowError:
             # It may happens as protobuf has bigger container value
             res = wmm.GatewayResultCode.GW_RES_INVALID_PARAM
-            self.logger.error("Invalid range value")
+            logging.error("Invalid range value")
 
         # Set stack in state defined by new config or set it as it was
         # previously
         try:
             new_state = config["started"]
         except KeyError:
             # Not defined in config
             new_state = stack_started
 
         try:
             current_state = (self.proxy.StackStatus & 0x01) == 0
             # Change stack state only if needed to avoid unnecessary events
             if current_state != new_state:
-                self.logger.debug(
+                logging.debug(
                     "Change stack state from %s to %s", current_state, new_state
                 )
                 self.proxy.SetStackState(new_state)
         except GLib.Error as err:
             res = ReturnCode.error_from_dbus_exception(str(err))
-            self.logger.exception(
+            logging.exception(
                 "Cannot set Stack state. Problem in communication probably: %s",
                 res.name,
             )
             return res
 
         # In case the network address was updated, read it back for our cached
         # value
@@ -293,154 +302,183 @@
         return res
 
     @property
     def cost(self):
         try:
             cost = self.proxy.SinkCost
         except GLib.Error:
-            self.logger.error("Cannot get sink cost for sink {}".format(self.sink_id))
+            logging.error("Cannot get sink cost for sink {}".format(self.sink_id))
             cost = 0
         return cost
 
     @cost.setter
     def cost(self, new_cost):
         if new_cost is None or new_cost < 0 or new_cost > 254:
             raise ValueError("Wrong sink cost value {}".format(new_cost))
 
         try:
             self.proxy.SinkCost = new_cost
         except GLib.Error as err:
             res = ReturnCode.error_from_dbus_exception(err.message)
             if res == wmm.GatewayResultCode.GW_RES_INVALID_ROLE:
-                self.logger.warning("Node role is not a sink, sink cost cannot be modified")
+                logging.warning("Node role is not a sink, sink cost cannot be modified")
                 raise ValueError("Wrong role to set cost value {}".format(new_cost))
             else:
-                self.logger.error("Cannot set sink cost for sink {} ({})".format(self.sink_id, res))
+                logging.error("Cannot set sink cost for sink {} ({})".format(self.sink_id, res))
 
-    def get_scratchpad_status(self):
-        d = {}
+    def get_scratchpad_status(self, out_d=None):
+        if out_d is None:
+            d = {}
+        else:
+            d = out_d
 
         dbus_to_gateway_satus = dict(
             [
                 (0, wmm.ScratchpadStatus.SCRATCHPAD_STATUS_SUCCESS),
                 (255, wmm.ScratchpadStatus.SCRATCHPAD_STATUS_NEW)
                 # Anything else is ERROR
             ]
         )
         try:
             status = self.proxy.StoredStatus
             d["stored_status"] = dbus_to_gateway_satus[status]
         except GLib.Error:
             # Exception raised when getting attribute (probably not set)
-            self.logger.error("Cannot get stored status in config")
+            logging.error("Cannot get stored status in config")
         except KeyError:
             # Between 1 and 254 => Error
-            self.logger.error("Scratchpad stored status has error: %s", status)
+            logging.error("Scratchpad stored status has error: %s", status)
             d["stored_status"] = wmm.ScratchpadStatus.SCRATCHPAD_STATUS_ERROR
 
         dbus_to_gateway_type = dict(
             [
                 (0, wmm.ScratchpadType.SCRATCHPAD_TYPE_BLANK),
                 (1, wmm.ScratchpadType.SCRATCHPAD_TYPE_PRESENT),
                 (2, wmm.ScratchpadType.SCRATCHPAD_TYPE_PROCESS),
             ]
         )
         try:
             stored_type = self.proxy.StoredType
             d["stored_type"] = dbus_to_gateway_type[stored_type]
         except GLib.Error:
             # Exception raised when getting attribute (probably not set)
-            self.logger.error("Cannot get stored type in config\n")
+            logging.error("Cannot get stored type in config\n")
 
         stored = {}
         self._get_param(stored, "seq", "StoredSeq")
         self._get_param(stored, "crc", "StoredCrc")
         self._get_param(stored, "len", "StoredLen")
-        d["stored_scartchpad"] = stored
+        d["stored_scratchpad"] = stored
 
         processed = {}
         self._get_param(processed, "seq", "ProcessedSeq")
         self._get_param(processed, "crc", "ProcessedCrc")
         self._get_param(processed, "len", "ProcessedLen")
-        d["processed_scartchpad"] = processed
+        d["processed_scratchpad"] = processed
 
         self._get_param(d, "firmware_area_id", "FirmwareAreaId")
 
-        try:
-            seq, crc, action, param = self.proxy.GetTargetScratchpad()
-            d["target_action"] = wmm.ScratchpadAction(
-                action + 1
-            )  # Plus one as dualmcu version starts at 0, and we start at 1
-            d["target_seq"] = seq
-            d["target_crc"] = crc
-            d["target_param"] = param
-        except GLib.Error:
-            self.logger.warning("Cannot get Target Scratchpad")
+        # Read Target only if firmware is greater than 5.1
+        stack_version = self.proxy.FirmwareVersion
+        if stack_version[0] > 5 or (stack_version[0] == 5 and stack_version[1] > 0):
+            # Target scratchpad should be supported (except if dualmcu is too old)
+            try:
+                seq, crc, action, param = self.proxy.GetTargetScratchpad()
+                target_and_action = {}
+                target_and_action["action"] = wmm.ScratchpadAction(
+                    action + 1
+                )  # Plus one as dualmcu version starts at 0, and we start at 1
+                target_and_action["target_sequence"] = seq
+                target_and_action["target_crc"] = crc
+                if target_and_action["action"] == wmm.ScratchpadAction.ACTION_PROPAGATE_AND_PROCESS_WITH_DELAY:
+                    # check if delay is in predifined list
+                    param_to_delay_dic = {
+                        0x4A: wmm.ProcessingDelay.DELAY_TEN_MINUTES,
+                        0x5E: wmm.ProcessingDelay.DELAY_THIRTY_MINUTES,
+                        0x81: wmm.ProcessingDelay.DELAY_ONE_HOUR,
+                        0x86: wmm.ProcessingDelay.DELAY_SIX_HOURS,
+                        0xC1: wmm.ProcessingDelay.DELAY_ONE_DAY,
+                        0xC2: wmm.ProcessingDelay.DELAY_TWO_DAYS,
+                        0xC5: wmm.ProcessingDelay.DELAY_FIVE_DAYS
+                    }
+
+                    try:
+                        target_and_action["delay"] = param_to_delay_dic[param]
+                    except KeyError:
+                        logging.debug("Delay not in predifined list: %d", param)
+                        target_and_action["param"] = param
+
+                else:
+                    target_and_action["param"] = param
+
+                d["target_and_action"] = target_and_action
+            except GLib.Error:
+                logging.warning("Cannot get Target Scratchpad")
 
         return d
 
     def process_scratchpad(self):
         ret = wmm.GatewayResultCode.GW_RES_OK
         restart = False
         try:
             # Stop the stack if not already stopped
             if self.proxy.StackStatus == 0:
                 self.proxy.SetStackState(False)
                 restart = True
         except GLib.Error:
-            self.logger.error("Sink in invalid state")
+            logging.error("Sink in invalid state")
             return wmm.GatewayResultCode.GW_RES_INVALID_SINK_STATE
 
         try:
             self.proxy.ProcessScratchpad()
         except GLib.Error as e:
             ret = ReturnCode.error_from_dbus_exception(str(e))
-            self.logger.error("Could not restore sink's state: %s", ret.name)
+            logging.error("Could not restore sink's state: %s", ret.name)
 
         if restart:
             try:
                 self.proxy.SetStackState(True)
             except GLib.Error as e:
                 ret = ReturnCode.error_from_dbus_exception(str(e))
-                self.logger.debug("Sink in invalid state: %s", ret.name)
+                logging.debug("Sink in invalid state: %s", ret.name)
 
         return ret
 
     def upload_scratchpad(self, seq, file):
         ret = wmm.GatewayResultCode.GW_RES_OK
         restart = False
         try:
             # Stop the stack if not already stopped
             if self.proxy.StackStatus == 0:
                 self.proxy.SetStackState(False)
                 restart = True
         except GLib.Error:
-            self.logger.error("Sink in invalid state")
+            logging.error("Sink in invalid state")
             return wmm.GatewayResultCode.GW_RES_INVALID_SINK_STATE
 
         try:
             self.proxy.UploadScratchpad(seq, file)
-            self.logger.info(
+            logging.info(
                 "Scratchpad loaded with seq %d on sink %s", seq, self.sink_id
             )
         except GLib.Error as e:
             ret = ReturnCode.error_from_dbus_exception(str(e))
-            self.logger.error("Cannot upload local scratchpad: %s", ret.name)
+            logging.error("Cannot upload local scratchpad: %s", ret.name)
         except OverflowError:
             # It may happens as protobuf has bigger container value
             ret = wmm.GatewayResultCode.GW_RES_INVALID_PARAM
-            self.logger.error("Invalid range value")
+            logging.error("Invalid range value")
 
         if restart:
             try:
                 # Restart sink if we stopped it for this request
                 self.proxy.SetStackState(True)
             except GLib.Error as e:
                 ret = ReturnCode.error_from_dbus_exception(str(e))
-                self.logger.error("Could not restore sink's state: %s", ret.name)
+                logging.error("Could not restore sink's state: %s", ret.name)
 
         return ret
 
     def set_target_scratchpad(self, action, target_seq, target_crc, param):
         ret = wmm.GatewayResultCode.GW_RES_OK
 
         if (
@@ -459,57 +497,57 @@
                     target_seq = self.proxy.StoredSeq
 
                 if target_crc is None:
                     # Target crc not specified, take local one
                     target_crc = self.proxy.StoredCrc
             except GLib.Error as e:
                 ret = ReturnCode.error_from_dbus_exception(str(e))
-                self.logger.error(
+                logging.error(
                     "Cannot get local scratchpad info for set_target: %s", ret.name
                 )
 
             if target_seq == 0:
-                self.logger.error("Seq 0 is not a valid target")
+                logging.error("Seq 0 is not a valid target")
                 return wmm.GatewayResultCode.GW_RES_INVALID_PARAM
 
         try:
             # If there is no param for the action, default it to 0 before
             # calling sink service through DBUS
             if param is None:
                 param = 0
 
-            # Do a minus 1 as action are shifted by one with dual mcu
-            res = self.proxy.SetTargetScratchpad(
-                target_seq, target_crc, action.value - 1, param
-            )
-            self.logger.info(
+            logging.info(
                 "Scratchpad target set to Action %s (%d) with seq"
-                " %d and crc %d on sink %s (res=%s)",
+                " %d and crc %d on sink %s",
                 action,
                 param,
                 target_seq,
                 target_crc,
                 self.sink_id,
-                res,
             )
+
+            # Do a minus 1 as action are shifted by one with dual mcu
+            self.proxy.SetTargetScratchpad(
+                target_seq, target_crc, action.value - 1, param
+            )
+
         except GLib.Error as e:
             ret = ReturnCode.error_from_dbus_exception(str(e))
-            self.logger.error("Cannot set target scratchpad: %s", ret.name)
+            logging.warning("Cannot set target scratchpad: %s (can be normal if same value as already set)", ret.name)
 
         return ret
 
 
 class SinkManager:
     "Helper class to manage the Sink list"
 
     def __init__(
-        self, bus, on_new_sink_cb, on_sink_removal_cb, on_stack_started, on_stack_stopped, logger=None
+        self, bus, on_new_sink_cb, on_sink_removal_cb, on_stack_started, on_stack_stopped
     ):
 
-        self.logger = logger or logging.getLogger(__name__)
         self.sinks = {}
         # List used to quickly retrieved sink well known name
         self.sender_to_name = {}
         self.bus = bus
 
         self.add_cb = None
         self.rm_cb = None
@@ -533,15 +571,15 @@
 
         # Set them at the end to be sure Sink Manager is ready when cb are fired
         self.add_cb = on_new_sink_cb
         self.rm_cb = on_sink_removal_cb
 
     def _add_sink(self, short_name, unique_name):
         if short_name in self.sinks:
-            self.logger.warning("Sink already in list sink name=%s", short_name)
+            logging.warning("Sink already in list sink name=%s", short_name)
             return
 
         # Open proxy for this sink
         proxy = self.bus.get(
             DBUS_SINK_PREFIX + short_name,  # Bus name
             "/com/wirepas/sink",  # Object path
         )
@@ -549,48 +587,47 @@
         sink = Sink(
             bus=self.bus,
             proxy=proxy,
             sink_id=short_name,
             unique_name=unique_name,
             on_stack_started=self.stack_started_cb,
             on_stack_stopped=self.stack_stopped_cb,
-            logger=self.logger,
         )
 
         sink.register_for_stack_started()
         sink.register_for_stack_stopped()
 
         self.sinks[short_name] = sink
 
         self.sender_to_name[unique_name] = short_name
 
         if self.add_cb is not None:
             self.add_cb(short_name)
 
-        self.logger.info("New sink added with name %s", short_name)
+        logging.info("New sink added with name %s", short_name)
 
     def _remove_sink(self, short_name):
         try:
             sink = self.sinks.pop(short_name)
             sink.unregister_from_stack_started()
 
             # Remove Sink to association list
             for k, v in self.sender_to_name.items():
                 if v == short_name:
                     self.sender_to_name.pop(k)
-                    self.logger.warning("Association removed from %s => %s", k, v)
+                    logging.warning("Association removed from %s => %s", k, v)
                     break
 
             # call client cb
             if self.rm_cb is not None:
                 self.rm_cb(short_name)
         except KeyError:
-            self.logger.error("Cannot remove %s from sink list", short_name)
+            logging.error("Cannot remove %s from sink list", short_name)
 
-        self.logger.info("Sink removed with name %s", short_name)
+        logging.info("Sink removed with name %s", short_name)
 
     def _on_name_owner_changed(self, sender, object, iface, signal, params):
         # pylint: disable=unused-argument
         # pylint: disable=redefined-builtin
         well_known_name = params[0]
         if well_known_name.startswith(DBUS_SINK_PREFIX):
             short_name = well_known_name[len(DBUS_SINK_PREFIX) :]
@@ -600,15 +637,15 @@
             if old_owner == "":
                 # New sink connection
                 self._add_sink(short_name, new_owner)
             elif new_owner == "":
                 # Removal
                 self._remove_sink(short_name)
             else:
-                self.logger.critical(
+                logging.critical(
                     "Not addition nor removal ??? %s: %s => %s",
                     well_known_name,
                     old_owner,
                     new_owner,
                 )
 
     def get_sinks(self):
@@ -616,16 +653,16 @@
         # of list while iterating on it (if new sink is connected)
         return list(self.sinks.values())
 
     def get_sink_name(self, bus_name):
         try:
             return self.sender_to_name[bus_name]
         except KeyError:
-            self.logger.error("Unknown sink %s from sink list", bus_name)
+            logging.error("Unknown sink %s from sink list", bus_name)
             return None
 
     def get_sink(self, short_name):
         try:
             return self.sinks[short_name]
         except KeyError:
-            self.logger.error("Unknown sink %s from sink list", short_name)
+            logging.error("Unknown sink %s from sink list", short_name)
             return None
```

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/dbus_print_client.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/dbus_print_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright 2019 Wirepas Ltd licensed under Apache License, Version 2.0
 #
 # See file LICENSE for full license details.
 
+import logging
 import os
+import sys
 from datetime import datetime
 
 from wirepas_gateway.dbus.dbus_client import BusClient
-from wirepas_gateway.utils import LoggerHelper
 
 
 class PrintClient(BusClient):
     """
     Simple class example that print all received message from dbus
     """
 
@@ -24,15 +25,15 @@
         dst_ep,
         travel_time,
         qos,
         hop_count,
         data,
     ):
         """ logs incoming data from the WM network """
-        self.logger.info(
+        logging.info(
             "[%s] Sink %s FROM %d TO %d on EP %d Data Size is %d",
             datetime.utcfromtimestamp(int(timestamp / 1000)).strftime(
                 "%Y-%m-%d %H:%M:%S"
             ),
             sink_id,
             src,
             dst,
@@ -41,15 +42,15 @@
         )
 
     def on_sink_connected(self, name):
         sink = self.sink_manager.get_sink(name)
 
         if sink is not None:
             # Read Stack status of sink on connection
-            self.logger.info("Sink connected with config: %s", sink.read_config())
+            logging.info("Sink connected with config: %s", sink.read_config())
 
 
 def main():
 
     # Set default debug level
     debug_level = "info"
     try:
@@ -63,18 +64,22 @@
         pass
 
     try:
         debug_level = os.environ["WM_DEBUG_LEVEL"]
     except KeyError:
         pass
 
-    log = LoggerHelper(module_name=__name__, level=debug_level)
-    logger = log.setup()
+    debug_level = "{0}".format(debug_level.upper())
 
+    # Create a "Print Client" object and enable his logger
     obj = PrintClient()
-    obj.logger = logger
+    logging.basicConfig(
+        format='%(asctime)s | [%(levelname)s] %(name)s@%(filename)s:%(lineno)d:%(message)s',
+        level=debug_level,
+        stream=sys.stdout
+    )
     obj.run()
 
 
 if __name__ == "__main__":
 
     main()
```

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/protocol/mqtt_wrapper.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/protocol/mqtt_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright 2019 Wirepas Ltd licensed under Apache License, Version 2.0
 #
 # See file LICENSE for full license details.
 
+import logging
 import queue
 import socket
 import ssl
 from select import select
 from threading import Thread, Lock
 from time import sleep
 from datetime import datetime
@@ -23,24 +24,22 @@
 
     # Keep alive time with broker
     KEEP_ALIVE_S = 20
 
     def __init__(
         self,
         settings,
-        logger,
         on_termination_cb=None,
         on_connect_cb=None,
         last_will_topic=None,
         last_will_data=None,
     ):
         Thread.__init__(self)
         self.daemon = True
         self.running = False
-        self.logger = logger
         self.on_termination_cb = on_termination_cb
         self.on_connect_cb = on_connect_cb
         # Set to track the unpublished packets
         self._unpublished_mid_set = set()
         # Keep track of latest published packet
         self._publish_monitor = PublishMonitor()
 
@@ -64,18 +63,18 @@
                     certfile=settings.mqtt_certfile,
                     keyfile=settings.mqtt_keyfile,
                     cert_reqs=ssl.VerifyMode[settings.mqtt_cert_reqs],
                     tls_version=ssl._SSLMethod[settings.mqtt_tls_version],
                     ciphers=settings.mqtt_ciphers,
                 )
             except Exception as e:
-                self.logger.error("Cannot use secure authentication %s", e)
+                logging.error("Cannot use secure authentication %s", e)
                 exit(-1)
 
-        self.logger.info(
+        logging.info(
             "Max inflight messages set to %s", settings.mqtt_max_inflight_messages
         )
         self._client.max_inflight_messages_set(settings.mqtt_max_inflight_messages)
 
         self._client.username_pw_set(settings.mqtt_username, settings.mqtt_password)
         self._client.on_connect = self._on_connect
         self._client.on_publish = self._on_publish
@@ -87,51 +86,56 @@
         try:
             self._client.connect(
                 settings.mqtt_hostname,
                 settings.mqtt_port,
                 keepalive=MQTTWrapper.KEEP_ALIVE_S,
             )
         except (socket.gaierror, ValueError) as e:
-            self.logger.error(
+            logging.error(
                 "Error on MQTT address %s:%d => %s"
                 % (settings.mqtt_hostname, settings.mqtt_port, str(e))
             )
-            exit(-1)
+            # Do not exit as it and let the retry mechanism
+            # to reconnect. It can happen if connection is not available yet.
+            # mqtt_reconnect_delay setting can be used to limit the retry.
         except ConnectionRefusedError:
-            self.logger.error("Connection Refused by MQTT broker")
+            logging.error("Connection Refused by MQTT broker")
             exit(-1)
+        except OSError as e:
+            logging.error("Cannot establish connection (%s)", str(e))
+            # It will happen if broker is down when trying first connection.
+            # But it can happen also if settings are wrong (host or port)
+            # mqtt_reconnect_delay setting can be used to limit the retry.
 
         self.timeout = settings.mqtt_reconnect_delay
 
         # Set options to initial socket if tcp transport only
-        if not self._use_websockets:
+        if not self._use_websockets and self._client.socket() is not None:
             self._client.socket().setsockopt(socket.SOL_SOCKET, socket.SO_SNDBUF, 2048)
 
         self._publish_queue = SelectableQueue()
 
         # Thread is not started yes
         self.running = False
         self.connected = False
-        self.first_connection_done = False
 
     def _on_connect(self, client, userdata, flags, rc):
         # pylint: disable=unused-argument
         if rc != 0:
-            self.logger.error("MQTT cannot connect: %s (%s)", connack_string(rc), rc)
+            logging.error("MQTT cannot connect: %s (%s)", connack_string(rc), rc)
             self.running = False
             return
 
-        self.first_connection_done = True
         self.connected = True
         if self.on_connect_cb is not None:
             self.on_connect_cb()
 
     def _on_disconnect(self, userdata, rc):
         if rc != 0:
-            self.logger.error(
+            logging.error(
                 "MQTT unexpected disconnection (network or broker originated):"
                 "%s (%s)",
                 connack_string(rc),
                 rc,
             )
             self.connected = False
 
@@ -187,49 +191,45 @@
 
     def _get_socket(self):
         sock = self._client.socket()
         if sock is not None:
             return sock
 
         if self.connected:
-            self.logger.error("MQTT Inner loop, unexpected disconnection")
-        elif not self.first_connection_done:
-            # It's better to avoid retrying if the first connection was not successful
-            self.logger.error("Impossible to connect - authentication failure ?")
-            return None
+            logging.error("MQTT Inner loop, unexpected disconnection")
 
         # Socket is not opened anymore, try to reconnect for timeout if set
         loop_forever = self.timeout == 0
         delay = 0
-        self.logger.info("Starting reconnect loop with timeout %d" % self.timeout)
+        logging.info("Starting reconnect loop with timeout %d" % self.timeout)
         # Loop forever or until timeout is over
         while loop_forever or (delay <= self.timeout):
             try:
-                self.logger.debug("MQTT reconnect attempt delay=%d" % delay)
+                logging.debug("MQTT reconnect attempt delay=%d" % delay)
                 ret = self._client.reconnect()
                 if ret == mqtt.MQTT_ERR_SUCCESS:
                     break
             except Exception:
                 # Retry to connect in 1 sec up to timeout if set
                 sleep(1)
                 delay += 1
-                self.logger.debug("Retrying to connect in 1 sec")
+                logging.debug("Retrying to connect in 1 sec")
 
         if not loop_forever:
             # In case of timeout set, check if it exits because of timeout
             if delay > self.timeout:
-                self.logger.error("Unable to reconnect after %s seconds", delay)
+                logging.error("Unable to reconnect after %s seconds", delay)
                 return None
 
         # Socket must be available once reconnect is successful
         if self._client.socket() is None:
-            self.logger.error("Cannot get socket after reconnect")
+            logging.error("Cannot get socket after reconnect")
             return None
         else:
-            self.logger.info("Successfully acquired socket after reconnect")
+            logging.info("Successfully acquired socket after reconnect")
 
         # Set options to new reopened socket
         if not self._use_websockets:
             self._client.socket().setsockopt(socket.SOL_SOCKET, socket.SO_SNDBUF, 2048)
         return self._client.socket()
 
     def _set_last_will(self, topic, data):
@@ -245,26 +245,26 @@
                 # check if we are connected
                 # Get client socket to select on it
                 # This function manage the reconnect
                 sock = self._get_socket()
                 if sock is None:
                     # Cannot get the socket, probably an issue
                     # with connection. Exit the thread
-                    self.logger.error("Cannot get MQTT socket, exit...")
+                    logging.error("Cannot get MQTT socket, exit...")
                     self.running = False
                 else:
                     self._do_select(sock)
             except TimeoutError:
-                self.logger.error("Timeout in connection, force a reconnect")
+                logging.error("Timeout in connection, force a reconnect")
                 self._client.reconnect()
             except Exception:
                 # If an exception is not caught before this point
                 # All the transport module must be stopped in order to be fully
                 # restarted by the managing agent
-                self.logger.exception("Unexpected exception in MQTT wrapper Thread")
+                logging.exception("Unexpected exception in MQTT wrapper Thread")
                 self.running = False
 
         if self.on_termination_cb is not None:
             # As this thread is daemonized, inform the parent that this
             # thread has exited
             self.on_termination_cb()
 
@@ -293,15 +293,15 @@
 
         """
         # Send it to the queue to be published from Mqtt thread
         self._publish_queue.put((topic, payload, qos, retain))
         self._publish_monitor.on_publish_request()
 
     def subscribe(self, topic, cb, qos=2) -> None:
-        self.logger.debug("Subscribing to: {}".format(topic))
+        logging.debug("Subscribing to: {}".format(topic))
         self._client.subscribe(topic, qos)
         self._client.message_callback_add(topic, cb)
 
     @property
     def publish_queue_size(self):
         return self._publish_monitor.get_publish_queue_size()
```

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/protocol/topic_helper.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/protocol/topic_helper.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/transport_service.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/transport_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Copyright 2019 Wirepas Ltd licensed under Apache License, Version 2.0
 #
 # See file LICENSE for full license details.
 #
 import logging
 import os
+import sys
 import wirepas_mesh_messaging as wmm
 from time import time, sleep
 from uuid import getnode
-from threading import Thread
+from threading import Lock, Thread
 
 from wirepas_gateway.dbus.dbus_client import BusClient
 from wirepas_gateway.protocol.topic_helper import TopicGenerator, TopicParser
 from wirepas_gateway.protocol.mqtt_wrapper import MQTTWrapper
 from wirepas_gateway.utils import ParserHelper
-from wirepas_gateway.utils import LoggerHelper
 
 from wirepas_gateway import __version__ as transport_version
 from wirepas_gateway import __pkg_name__
 
 # This constant is the actual API level implemented by this transport module (cf WP-RM-128)
 IMPLEMENTED_API_VERSION = 2
 
@@ -25,15 +25,14 @@
 class ConnectionToBackendMonitorThread(Thread):
 
     # Maximum cost to disable traffic
     SINK_COST_HIGH = 254
 
     def __init__(
         self,
-        logger,
         period,
         mqtt_wrapper,
         sink_manager,
         minimum_sink_cost,
         max_buffered_packets,
         max_delay_without_publish,
     ):
@@ -42,27 +41,25 @@
         Connection status is monitored thanks to the number of
         messages pushed to the mqtt client queue but not published.
         And the latest successfully published packet is also monitored.
         Mqtt connection is not used as a trigger as it may modify too often
         the sink cost with an unstable connection that would be counterproductive.
 
         Args:
-            logger: logger used to log messages
             period: the period to check the buffer status
             mqtt_wrapper: the mqtt wrapper to get access to queue level
             sink_manager: the sink manager to modify sink cost of all sinks
             minimum_sink_cost: the minimum sink cost for sinks on this gateway
             max_buffered_packets: the maximum number of packets that can be buffered before
                                   rising the sink costs
             max_delay_without_publish: the maximum delay without any successful publish (with
                                        something in the queue before rising the sink costs
         """
         Thread.__init__(self)
 
-        self.logger = logger
         # Daemonize thread to exit with full process
         self.daemon = True
 
         # How often to check the queue
         self.period = period
         self.mqtt_wrapper = mqtt_wrapper
         self.sink_manager = sink_manager
@@ -112,27 +109,27 @@
 
         self.running = True
 
         while self.running:
             if not self.disconnected:
                 # Check if a condition to declare "back hole" is met
                 if self._is_publish_delay_over() or self._is_buffer_threshold_reached():
-                    self.logger.info("Increasing sink cost of all sinks")
-                    self.logger.debug(
+                    logging.info("Increasing sink cost of all sinks")
+                    logging.debug(
                         "Last publish: %s Queue Size %s",
                         self.mqtt_wrapper.publish_waiting_time_s,
                         self.mqtt_wrapper.publish_queue_size,
                     )
 
                     self._set_sinks_cost_high()
                     self.disconnected = True
             else:
                 if self.mqtt_wrapper.publish_queue_size == 0:
                     # Network is back, put the connection back
-                    self.logger.info(
+                    logging.info(
                         "Connection is back, decreasing sink cost of all sinks"
                     )
                     self._set_sinks_cost_low()
                     self.disconnected = False
 
             # Wait for period
             sleep(self.period)
@@ -147,15 +144,15 @@
         """
         Initialize sink cost according to current connection state
         Args:
             name: name of sink to initialize
         """
         sink = self.sink_manager.get_sink(name)
 
-        self.logger.info("Initialize sinkCost of sink %s", name)
+        logging.info("Initialize sinkCost of sink %s", name)
         if sink is not None:
             if self.disconnected:
                 sink.cost = self.SINK_COST_HIGH
             else:
                 sink.cost = self.minimum_sink_cost
 
 
@@ -169,91 +166,144 @@
 
     # Maximum hop limit to send a packet is limited to 15 by API (4 bits)
     MAX_HOP_LIMIT = 15
 
     # Period in s to check for black hole issue
     MONITORING_BUFFERING_PERIOD_S = 1
 
-    def __init__(self, settings, logger=None, **kwargs):
-        self.logger = logger or logging.getLogger(__name__)
-        self.logger.info("Version is: %s", transport_version)
+    def __init__(self, settings, **kwargs):
+        logging.info("Version is: %s", transport_version)
 
         super(TransportService, self).__init__(
-            logger=logger,
             c_extension=(settings.full_python is False),
             ignored_ep_filter=settings.ignored_endpoints_filter,
             **kwargs
         )
 
         self.gw_id = settings.gateway_id
         self.gw_model = settings.gateway_model
         self.gw_version = settings.gateway_version
 
         self.whitened_ep_filter = settings.whitened_endpoints_filter
 
         last_will_topic = TopicGenerator.make_status_topic(self.gw_id)
         last_will_message = wmm.StatusEvent(
-            self.gw_id, wmm.GatewayState.OFFLINE
+            self.gw_id, wmm.GatewayState.OFFLINE,
+            gateway_model=self.gw_model,
+            gateway_version=self.gw_version
         ).payload
 
         self.mqtt_wrapper = MQTTWrapper(
             settings,
-            self.logger,
             self._on_mqtt_wrapper_termination_cb,
             self._on_connect,
             last_will_topic,
             last_will_message,
         )
 
         self.mqtt_wrapper.start()
 
-        self.logger.info("Gateway started with id: %s", self.gw_id)
+        logging.info("Gateway started with id: %s", self.gw_id)
 
         self.monitoring_thread = None
         self.minimum_sink_cost = settings.buffering_minimal_sink_cost
 
         if settings.buffering_max_buffered_packets > 0:
-            self.logger.info(
+            logging.info(
                 " Black hole detection enabled: max_packets=%s packets, max_delay=%s",
                 settings.buffering_max_buffered_packets,
                 settings.buffering_max_delay_without_publish,
             )
             # Create and start a monitoring thread for black hole issue
             self.monitoring_thread = ConnectionToBackendMonitorThread(
-                self.logger,
                 self.MONITORING_BUFFERING_PERIOD_S,
                 self.mqtt_wrapper,
                 self.sink_manager,
                 settings.buffering_minimal_sink_cost,
                 settings.buffering_max_buffered_packets,
                 settings.buffering_max_delay_without_publish,
             )
             self.monitoring_thread.start()
 
         if settings.debug_incr_data_event_id:
             self.data_event_id = 0
         else:
             self.data_event_id = None
 
+        # Flag to know if updating the status is already scheduled
+        self._is_update_status_scheduled = False
+        self._status_lock = Lock()
+
     def _on_mqtt_wrapper_termination_cb(self):
         """
         Callback used to be informed when the MQTT wrapper has exited
         It is not a normal situation and better to exit the program
         to have a change to restart from a clean session
         """
-        self.logger.error("MQTT wrapper ends. Terminate the program")
+        logging.error("MQTT wrapper ends. Terminate the program")
         self.stop_dbus_client()
 
     def _set_status(self):
-        event_online = wmm.StatusEvent(self.gw_id, wmm.GatewayState.ONLINE)
+        # Create a list of different sink configs
+        configs = []
+        for sink in self.sink_manager.get_sinks():
+            config = sink.read_config()
+            if config is not None:
+                configs.append(config)
+
+        topic = TopicGenerator.make_get_configs_response_topic(self.gw_id)
+
+        event_online = wmm.StatusEvent(
+                            self.gw_id,
+                            wmm.GatewayState.ONLINE,
+                            sink_configs=configs,
+                            gateway_model=self.gw_model,
+                            gateway_version=self.gw_version,
+                            )
 
         topic = TopicGenerator.make_status_topic(self.gw_id)
 
         self.mqtt_wrapper.publish(topic, event_online.payload, qos=1, retain=True)
 
+    def _update_status(self):
+        # First check if an update is about to be sent to avoid
+        # multiple updates in a short period (0.5s)
+        with self._status_lock:
+            if self._is_update_status_scheduled:
+                # Update is already scheduled, so our modification
+                # will be handled soon
+                logging.debug("Update already scheduled")
+                return
+            else:
+                logging.debug("Update not scheduled yet")
+                self._is_update_status_scheduled = True
+
+        def set_status_after_delay(delay_s):
+            sleep(delay_s)
+            logging.debug("Time to update the status")
+            self._is_update_status_scheduled = False
+            self._set_status()
+
+        # We are here as there was no update scheduled yet.
+        # Wait a bit
+        thread = Thread(target=set_status_after_delay, args=[0.5])
+        thread.start()
+
+    def update_gateway_status_dec(fn):
+        """
+        Decorator to update the gateway status when needed
+        """
+        def wrapper(self, *args, **kwargs):
+            fn(self, *args, **kwargs)
+            logging.debug("Updating gw status for %s", fn)
+            self._update_status()
+            return
+
+        return wrapper
+
     def _on_connect(self):
         # Register for get gateway info
         topic = TopicGenerator.make_get_gateway_info_request_topic(self.gw_id)
         self.mqtt_wrapper.subscribe(topic, self._on_get_gateway_info_cmd_received)
 
         # Register for get configs request
         topic = TopicGenerator.make_get_configs_request_topic(self.gw_id)
@@ -261,15 +311,15 @@
 
         # Register for set config request for any sink
         topic = TopicGenerator.make_set_config_request_topic(self.gw_id)
         self.mqtt_wrapper.subscribe(topic, self._on_set_config_cmd_received)
 
         # Register for send data request for any sink on the gateway
         topic = TopicGenerator.make_send_data_request_topic(self.gw_id)
-        self.logger.debug("Subscribing to: %s", topic)
+        logging.debug("Subscribing to: %s", topic)
         # It is important to have a qos of 2 and also from the publisher as 1 could generate
         # duplicated packets and we don't know the consequences on end
         # application
         self.mqtt_wrapper.subscribe(topic, self._on_send_data_cmd_received, qos=2)
 
         # Register for otap commands for any sink on the gateway
         topic = TopicGenerator.make_otap_status_request_topic(self.gw_id)
@@ -286,26 +336,17 @@
         )
 
         topic = TopicGenerator.make_otap_set_target_scratchpad_request_topic(self.gw_id)
         self.mqtt_wrapper.subscribe(
             topic, self._on_otap_set_target_scratchpad_request_received
         )
 
-        # Register ourself to our status in case someone else (by mistake)
-        # update our status.
-        # It will work only if we are allowed to register for event topic
-        # at broker level
-        topic = TopicGenerator.make_status_topic(self.gw_id)
-        self.mqtt_wrapper.subscribe(
-            topic, self._on_own_status_received
-        )
-
         self._set_status()
 
-        self.logger.info("MQTT connected!")
+        logging.info("MQTT connected!")
 
     def on_data_received(
         self,
         sink_id,
         timestamp,
         src,
         dst,
@@ -315,25 +356,25 @@
         qos,
         hop_count,
         data,
     ):
 
         if self.whitened_ep_filter is not None and dst_ep in self.whitened_ep_filter:
             # Only publish payload size but not the payload
-            self.logger.debug("Filtering payload data")
+            logging.debug("Filtering payload data")
             data_size = data.__len__()
             data = None
         else:
             data_size = None
 
         sink = self.sink_manager.get_sink(sink_id)
         if sink is None:
             # It can happen at sink connection as messages can be received
             # before sinks are identified
-            self.logger.info(
+            logging.info(
                 "Message received from unknown sink at the moment %s", sink_id
             )
             return
 
         network_address = sink.get_network_address()
 
         event = wmm.ReceivedDataEvent(
@@ -352,40 +393,42 @@
             hop_count=hop_count,
             network_address=network_address,
         )
 
         topic = TopicGenerator.make_received_data_topic(
             self.gw_id, sink_id, network_address, src_ep, dst_ep
         )
-        self.logger.debug("Uplink traffic: %s | %s", topic, event.event_id)
+        logging.debug("Uplink traffic: %s | %s", topic, event.event_id)
 
         # No need to protect data_event_id as on_data_received is always
         # called from same thread
         if self.data_event_id is not None:
             self.data_event_id += 1
 
         # Set qos to 1 to avoid loading too much the broker
         # unique id in event header can be used for duplicate filtering in
         # backends
         self.mqtt_wrapper.publish(topic, event.payload, qos=1)
 
+    @update_gateway_status_dec
     def on_stack_started(self, name):
-        self.logger.debug("Sink started: %s", name)
+        logging.debug("Sink started: %s", name)
         # Generate a setconfig answer with req_id of 0
-        self. _send_asynchronous_set_config_response(name)
+        self._send_asynchronous_set_config_response(name)
 
+    @update_gateway_status_dec
     def on_stack_stopped(self, name):
-        self.logger.debug("Sink stopped: %s", name)
+        logging.debug("Sink stopped: %s", name)
         # Generate a setconfig answer with req_id of 0
-        self. _send_asynchronous_set_config_response(name)
+        self._send_asynchronous_set_config_response(name)
 
     def _send_asynchronous_set_config_response(self, name):
         sink = self.sink_manager.get_sink(name)
         if sink is None:
-            self.logger.error("Sink %s error: unknown sink", name)
+            logging.error("Sink %s error: unknown sink", name)
             return
         response = wmm.SetConfigResponse(
             0,
             self.gw_id,
             wmm.GatewayResultCode.GW_RES_OK,
             sink.sink_id,
             sink.read_config(),
@@ -421,51 +464,53 @@
         def wrapper(*args, **kwargs):
             thread = Thread(target=fn, args=args, kwargs=kwargs)
             thread.start()
             return thread
 
         return wrapper
 
+    @update_gateway_status_dec
     def on_sink_connected(self, name):
-        self.logger.info("Sink connected, sending new configs")
+        logging.info("Sink connected, sending new configs")
         if self.monitoring_thread is not None:
             # Black hole algorithm in place do not initialize here the cost
             self.monitoring_thread.initialize_sink(name)
         else:
             sink = self.sink_manager.get_sink(name)
             if sink is not None:
-                self.logger.info(
+                logging.info(
                     "Initialize sinkCost of sink {} to minimum {}".format(
                         name, self.minimum_sink_cost
                     )
                 )
                 try:
                     sink.cost = self.minimum_sink_cost
                 except ValueError:
-                    self.logger.debug("Cannot set cost, probably not a sink")
+                    logging.debug("Cannot set cost, probably not a sink")
 
         self._send_asynchronous_get_configs_response()
 
+    @update_gateway_status_dec
     def on_sink_disconnected(self, name):
-        self.logger.info("Sink disconnected, sending new configs")
+        logging.info("Sink disconnected, sending new configs")
         self._send_asynchronous_get_configs_response()
 
     @deferred_thread
     def _on_send_data_cmd_received(self, client, userdata, message):
         # pylint: disable=unused-argument
         try:
             request = wmm.SendDataRequest.from_payload(message.payload)
         except wmm.GatewayAPIParsingException as e:
-            self.logger.error(str(e))
+            logging.error(str(e))
             return
 
         # Get the sink-id from topic
         _, sink_id = TopicParser.parse_send_data_topic(message.topic)
 
-        self.logger.debug("Downlink traffic: %s | %s", sink_id, request.req_id)
+        logging.debug("Downlink traffic: %s | %s", sink_id, request.req_id)
 
         sink = self.sink_manager.get_sink(sink_id)
         if sink is not None:
             if request.hop_limit > self.MAX_HOP_LIMIT:
                 res = wmm.GatewayResultCode.GW_RES_INVALID_MAX_HOP_COUNT
             else:
                 res = sink.send_data(
@@ -475,32 +520,32 @@
                     request.qos,
                     request.initial_delay_ms,
                     request.data_payload,
                     request.is_unack_csma_ca,
                     request.hop_limit,
                 )
         else:
-            self.logger.warning("No sink with id: %s", sink_id)
+            logging.warning("No sink with id: %s", sink_id)
             # No sink with  this id
             res = wmm.GatewayResultCode.GW_RES_INVALID_SINK_ID
 
         # Answer to backend
         response = wmm.SendDataResponse(request.req_id, self.gw_id, res, sink_id)
         topic = TopicGenerator.make_send_data_response_topic(self.gw_id, sink_id)
 
         self.mqtt_wrapper.publish(topic, response.payload, qos=2)
 
     @deferred_thread
     def _on_get_configs_cmd_received(self, client, userdata, message):
         # pylint: disable=unused-argument
-        self.logger.info("Config request received")
+        logging.info("Config request received")
         try:
             request = wmm.GetConfigsRequest.from_payload(message.payload)
         except wmm.GatewayAPIParsingException as e:
-            self.logger.error(str(e))
+            logging.error(str(e))
             return
 
         # Create a list of different sink configs
         configs = []
         for sink in self.sink_manager.get_sinks():
             config = sink.read_config()
             if config is not None:
@@ -509,42 +554,25 @@
         response = wmm.GetConfigsResponse(
             request.req_id, self.gw_id, wmm.GatewayResultCode.GW_RES_OK, configs
         )
         topic = TopicGenerator.make_get_configs_response_topic(self.gw_id)
 
         self.mqtt_wrapper.publish(topic, response.payload, qos=2)
 
-    @deferred_thread
-    def _on_own_status_received(self, client, userdata, message):
-        try:
-            if message.payload.__len__() > 0:
-                request = wmm.StatusEvent.from_payload(message.payload)
-                if request.state == wmm.GatewayState.ONLINE:
-                    # Everything is fine, this is our state
-                    return
-        except wmm.GatewayAPIParsingException:
-            pass
-
-        # If we are here, something happened to our status.
-        # Either not online or malformed or empty
-        self.logger.error("Gateway info request is wrong or updated")
-        # Set our status back
-        self._set_status()
-
     def _on_get_gateway_info_cmd_received(self, client, userdata, message):
         # pylint: disable=unused-argument
         """
         This function doesn't need the decorator @deferred_thread as request is handled
         without I/O
         """
-        self.logger.info("Gateway info request received")
+        logging.info("Gateway info request received")
         try:
             request = wmm.GetGatewayInfoRequest.from_payload(message.payload)
         except wmm.GatewayAPIParsingException as e:
-            self.logger.error(str(e))
+            logging.error(str(e))
             return
 
         response = wmm.GetGatewayInfoResponse(
             request.req_id,
             self.gw_id,
             wmm.GatewayResultCode.GW_RES_OK,
             current_time_s_epoch=int(time()),
@@ -553,24 +581,25 @@
             implemented_api_version=IMPLEMENTED_API_VERSION,
         )
 
         topic = TopicGenerator.make_get_gateway_info_response_topic(self.gw_id)
         self.mqtt_wrapper.publish(topic, response.payload, qos=2)
 
     @deferred_thread
+    @update_gateway_status_dec
     def _on_set_config_cmd_received(self, client, userdata, message):
         # pylint: disable=unused-argument
-        self.logger.info("Set config request received")
+        logging.info("Set config request received")
         try:
             request = wmm.SetConfigRequest.from_payload(message.payload)
         except wmm.GatewayAPIParsingException as e:
-            self.logger.error(str(e))
+            logging.error(str(e))
             return
 
-        self.logger.debug("Set sink config: %s", request)
+        logging.debug("Set sink config: %s", request)
         sink = self.sink_manager.get_sink(request.sink_id)
         if sink is not None:
             res = sink.write_config(request.new_config)
             new_config = sink.read_config()
         else:
             res = wmm.GatewayResultCode.GW_RES_INVALID_SINK_ID
             new_config = None
@@ -583,44 +612,39 @@
         )
 
         self.mqtt_wrapper.publish(topic, response.payload, qos=2)
 
     @deferred_thread
     def _on_otap_status_request_received(self, client, userdata, message):
         # pylint: disable=unused-argument
-        self.logger.info("OTAP status request received")
+        logging.info("OTAP status request received")
         try:
             request = wmm.GetScratchpadStatusRequest.from_payload(message.payload)
         except wmm.GatewayAPIParsingException as e:
-            self.logger.error(str(e))
+            logging.error(str(e))
             return
 
         sink = self.sink_manager.get_sink(request.sink_id)
         if sink is not None:
             d = sink.get_scratchpad_status()
 
-            target_and_action = {}
             try:
-                target_and_action["action"] = d["target_action"]
-                target_and_action["target_sequence"] = d["target_seq"]
-                target_and_action["target_crc"] = d["target_crc"]
-                target_and_action["param"] = d["target_param"]
+                target_and_action = d["target_and_action"]
             except KeyError:
-                # If not present, just an old node
                 target_and_action = None
 
             response = wmm.GetScratchpadStatusResponse(
                 request.req_id,
                 self.gw_id,
                 wmm.GatewayResultCode.GW_RES_OK,
                 request.sink_id,
-                d["stored_scartchpad"],
+                d["stored_scratchpad"],
                 d["stored_status"],
                 d["stored_type"],
-                d["processed_scartchpad"],
+                d["processed_scratchpad"],
                 d["firmware_area_id"],
                 target_and_action,
             )
         else:
             response = wmm.GetScratchpadStatusResponse(
                 request.req_id,
                 self.gw_id,
@@ -631,24 +655,25 @@
         topic = TopicGenerator.make_otap_status_response_topic(
             self.gw_id, request.sink_id
         )
 
         self.mqtt_wrapper.publish(topic, response.payload, qos=2)
 
     @deferred_thread
+    @update_gateway_status_dec
     def _on_otap_upload_scratchpad_request_received(self, client, userdata, message):
         # pylint: disable=unused-argument
-        self.logger.info("OTAP upload request received")
+        logging.info("OTAP upload request received")
         try:
             request = wmm.UploadScratchpadRequest.from_payload(message.payload)
         except wmm.GatewayAPIParsingException as e:
-            self.logger.error(str(e))
+            logging.error(str(e))
             return
 
-        self.logger.info("OTAP upload request received for %s", request.sink_id)
+        logging.info("OTAP upload request received for %s", request.sink_id)
 
         sink = self.sink_manager.get_sink(request.sink_id)
         if sink is not None:
             res = sink.upload_scratchpad(request.seq, request.scratchpad)
         else:
             res = wmm.GatewayResultCode.GW_RES_INVALID_SINK_ID
 
@@ -661,19 +686,19 @@
         )
 
         self.mqtt_wrapper.publish(topic, response.payload, qos=2)
 
     @deferred_thread
     def _on_otap_process_scratchpad_request_received(self, client, userdata, message):
         # pylint: disable=unused-argument
-        self.logger.info("OTAP process request received")
+        logging.info("OTAP process request received")
         try:
             request = wmm.ProcessScratchpadRequest.from_payload(message.payload)
         except wmm.GatewayAPIParsingException as e:
-            self.logger.error(str(e))
+            logging.error(str(e))
             return
 
         sink = self.sink_manager.get_sink(request.sink_id)
         if sink is not None:
             res = sink.process_scratchpad()
         else:
             res = wmm.GatewayResultCode.GW_RES_INVALID_SINK_ID
@@ -685,30 +710,31 @@
         topic = TopicGenerator.make_otap_process_scratchpad_response_topic(
             self.gw_id, request.sink_id
         )
 
         self.mqtt_wrapper.publish(topic, response.payload, qos=2)
 
     @deferred_thread
+    @update_gateway_status_dec
     def _on_otap_set_target_scratchpad_request_received(
         self, client, userdata, message
     ):
         # pylint: disable=unused-argument
         res = wmm.GatewayResultCode.GW_RES_OK
-        self.logger.info("OTAP set target request received")
+        logging.info("OTAP set target request received")
         try:
             request = wmm.SetScratchpadTargetAndActionRequest.from_payload(
                 message.payload
             )
             action = request.target["action"]
         except wmm.GatewayAPIParsingException as e:
-            self.logger.error(str(e))
+            logging.error(str(e))
             return
         except KeyError:
-            self.logger.error("Action is mandatory")
+            logging.error("Action is mandatory")
             res = wmm.GatewayResultCode.GW_RES_INVALID_PARAM
 
         if res == wmm.GatewayResultCode.GW_RES_OK:
             # Get optional params (None if not present)
             seq = request.target.get("target_sequence")
             crc = request.target.get("target_crc")
             delay = request.target.get("delay")
@@ -803,93 +829,93 @@
             single_list += list(range(lower, upper + 1))
         except (AttributeError, ValueError):
             raise SyntaxError("Wrong EP range format")
 
     return single_list
 
 
-def _check_duplicate(args, old_param, new_param, default, logger):
+def _check_duplicate(args, old_param, new_param, default):
     old_param_val = getattr(args, old_param, default)
     new_param_val = getattr(args, new_param, default)
     if new_param_val == old_param_val:
         # Nothing to update
         return
 
     if old_param_val != default:
         # Old param is set, check if new_param is also set
         if new_param_val == default:
             setattr(args, new_param, old_param_val)
-            logger.warning(
+            logging.warning(
                 "Param %s is deprecated, please use %s instead", old_param, new_param
             )
         else:
-            logger.error(
+            logging.error(
                 "Param %s and %s cannot be set at the same time", old_param, new_param
             )
             exit()
 
 
-def _update_parameters(settings, logger):
+def _update_parameters(settings):
     """
     Function to handle the backward compatibility with old parameters name
     Args:
         settings: Full parameters
 
     Returns: None
     """
 
-    _check_duplicate(settings, "host", "mqtt_hostname", None, logger)
-    _check_duplicate(settings, "port", "mqtt_port", 8883, logger)
-    _check_duplicate(settings, "username", "mqtt_username", None, logger)
-    _check_duplicate(settings, "password", "mqtt_password", None, logger)
-    _check_duplicate(settings, "tlsfile", "mqtt_certfile", None, logger)
+    _check_duplicate(settings, "host", "mqtt_hostname", None)
+    _check_duplicate(settings, "port", "mqtt_port", 8883)
+    _check_duplicate(settings, "username", "mqtt_username", None)
+    _check_duplicate(settings, "password", "mqtt_password", None)
+    _check_duplicate(settings, "tlsfile", "mqtt_certfile", None)
     _check_duplicate(
-        settings, "unsecure_authentication", "mqtt_force_unsecure", False, logger
+        settings, "unsecure_authentication", "mqtt_force_unsecure", False
     )
-    _check_duplicate(settings, "gwid", "gateway_id", None, logger)
+    _check_duplicate(settings, "gwid", "gateway_id", None)
 
     if settings.gateway_id is None:
         settings.gateway_id = str(getnode())
 
     # Parse EP list that should not be published
     if settings.ignored_endpoints_filter:
         try:
             settings.ignored_endpoints_filter = parse_setting_list(
                 settings.ignored_endpoints_filter
             )
-            logger.debug("Ignored endpoints are: %s", settings.ignored_endpoints_filter)
+            logging.debug("Ignored endpoints are: %s", settings.ignored_endpoints_filter)
         except SyntaxError as e:
-            logger.error("Wrong format for ignored_endpoints_filter EP list (%s)", e)
+            logging.error("Wrong format for ignored_endpoints_filter EP list (%s)", e)
             exit()
 
     if settings.whitened_endpoints_filter:
         try:
             settings.whitened_endpoints_filter = parse_setting_list(
                 settings.whitened_endpoints_filter
             )
-            logger.debug(
+            logging.debug(
                 "Whitened endpoints are: {}".format(settings.whitened_endpoints_filter)
             )
         except SyntaxError as e:
-            logger.error("Wrong format for whitened_endpoints_filter EP list (%s)", e)
+            logging.error("Wrong format for whitened_endpoints_filter EP list (%s)", e)
             exit()
 
 
-def _check_parameters(settings, logger):
+def _check_parameters(settings):
     if settings.mqtt_force_unsecure and settings.mqtt_certfile:
         # If tls cert file is provided, unsecure authentication cannot
         # be set
-        logger.error("Cannot give certfile and disable secure authentication")
+        logging.error("Cannot give certfile and disable secure authentication")
         exit()
 
     try:
         if set(settings.ignored_endpoints_filter) & set(
             settings.whitened_endpoints_filter
         ):
-            logger.error("Some endpoints are both ignored and whitened")
+            logging.error("Some endpoints are both ignored and whitened")
             exit()
     except TypeError:
         # One of the filter list is None
         pass
 
 
 def main():
@@ -925,20 +951,26 @@
         pass
 
     try:
         debug_level = os.environ["WM_DEBUG_LEVEL"]
     except KeyError:
         pass
 
-    log = LoggerHelper(module_name=__pkg_name__, level=debug_level)
-    logger = log.setup()
+    debug_level = "{0}".format(debug_level.upper())
+
+    # enable its logger
+    logging.basicConfig(
+        format=f'%(asctime)s | [%(levelname)s] {__pkg_name__}@%(filename)s:%(lineno)d:%(message)s',
+        level=debug_level,
+        stream=sys.stdout
+    )
 
-    _update_parameters(settings, logger)
+    _update_parameters(settings)
     # after this stage, mqtt deprecated argument cannot be used
 
-    _check_parameters(settings, logger)
+    _check_parameters(settings)
 
-    TransportService(settings=settings, logger=logger).run()
+    TransportService(settings=settings).run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/utils/argument_tools.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/utils/argument_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,36 +231,36 @@
 
         self.mqtt.add_argument(
             "--mqtt_ca_certs",
             default=os.environ.get("WM_SERVICES_MQTT_CA_CERTS", None),
             action="store",
             type=self.str2none,
             help=(
-                "A string path to the Certificate "
+                "Path to the Certificate "
                 "Authority certificate files that "
                 "are to be treated as trusted by "
                 "this client."
             ),
         )
 
         self.mqtt.add_argument(
             "--mqtt_certfile",
             default=os.environ.get("WM_SERVICES_MQTT_CLIENT_CRT", None),
             action="store",
             type=self.str2none,
-            help=("Strings pointing to the PEM encoded client certificate."),
+            help=("Path to the PEM encoded client certificate."),
         )
 
         self.mqtt.add_argument(
             "--mqtt_keyfile",
             default=os.environ.get("WM_SERVICES_MQTT_CLIENT_KEY", None),
             action="store",
             type=self.str2none,
             help=(
-                "Strings pointing to the PEM "
+                "Path to the PEM "
                 "encoded client private keys "
                 "respectively."
             ),
         )
 
         self.mqtt.add_argument(
             "--mqtt_cert_reqs",
```

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway/utils/serialization_tools.py` & `wirepas_gateway-1.4.3rc4/wirepas_gateway/utils/serialization_tools.py`

 * *Files identical despite different names*

### Comparing `wirepas_gateway-1.4.2rc1/wirepas_gateway.egg-info/SOURCES.txt` & `wirepas_gateway-1.4.3rc4/wirepas_gateway.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,9 +20,8 @@
 wirepas_gateway/dbus/sink_manager.py
 wirepas_gateway/dbus/c-extension/dbus_c.c
 wirepas_gateway/protocol/__init__.py
 wirepas_gateway/protocol/mqtt_wrapper.py
 wirepas_gateway/protocol/topic_helper.py
 wirepas_gateway/utils/__init__.py
 wirepas_gateway/utils/argument_tools.py
-wirepas_gateway/utils/log_tools.py
 wirepas_gateway/utils/serialization_tools.py
```

