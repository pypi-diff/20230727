# Comparing `tmp/oms-mqclient-2.4.1.tar.gz` & `tmp/oms-mqclient-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.4.1.tar", last modified: Thu Jul 27 18:08:41 2023, max compression
+gzip compressed data, was "oms-mqclient-2.4.2.tar", last modified: Thu Jul 27 21:12:58 2023, max compression
```

## Comparing `oms-mqclient-2.4.1.tar` & `oms-mqclient-2.4.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.372916 oms-mqclient-2.4.1/mqclient/
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-27 18:08:38.000000 oms-mqclient-2.4.1/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6720 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.372916 oms-mqclient-2.4.1/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    14392 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    18112 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_clients/utils.py
--rw-r--r--   0 root         (0) root         (0)      395 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    23476 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.372916 oms-mqclient-2.4.1/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 18:08:41.000000 oms-mqclient-2.4.1/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-27 18:08:41.000000 oms-mqclient-2.4.1/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 18:08:41.000000 oms-mqclient-2.4.1/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      502 2023-07-27 18:08:41.000000 oms-mqclient-2.4.1/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 18:08:41.000000 oms-mqclient-2.4.1/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2780 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.372916 oms-mqclient-2.4.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8990 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    38880 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    19982 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9102 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 21:12:58.373948 oms-mqclient-2.4.2/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 21:12:58.373948 oms-mqclient-2.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 21:12:58.369948 oms-mqclient-2.4.2/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-27 21:12:55.000000 oms-mqclient-2.4.2/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6592 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 21:12:58.369948 oms-mqclient-2.4.2/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14308 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    18145 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/broker_clients/utils.py
+-rw-r--r--   0 root         (0) root         (0)      395 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    23476 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 21:12:58.373948 oms-mqclient-2.4.2/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 21:12:58.000000 oms-mqclient-2.4.2/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-27 21:12:58.000000 oms-mqclient-2.4.2/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 21:12:58.000000 oms-mqclient-2.4.2/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      502 2023-07-27 21:12:58.000000 oms-mqclient-2.4.2/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 21:12:58.000000 oms-mqclient-2.4.2/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-07-27 21:12:58.377948 oms-mqclient-2.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 21:12:58.365948 oms-mqclient-2.4.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 21:12:58.373948 oms-mqclient-2.4.2/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8990 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    38880 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    19982 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 21:12:58.373948 oms-mqclient-2.4.2/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 21:12:58.373948 oms-mqclient-2.4.2/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 21:12:58.373948 oms-mqclient-2.4.2/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 21:12:58.373948 oms-mqclient-2.4.2/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9102 2023-07-27 21:12:54.000000 oms-mqclient-2.4.2/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.4.1/LICENSE` & `oms-mqclient-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/PKG-INFO` & `oms-mqclient-2.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.4.1
+Version: 2.4.2
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.4.1/README.md` & `oms-mqclient-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/mqclient/__init__.py` & `oms-mqclient-2.4.2/mqclient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.4.1"
+__version__ = "2.4.2"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.4.1/mqclient/broker_client_interface.py` & `oms-mqclient-2.4.2/mqclient/broker_client_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,14 @@
     """Raised when a `connect()` fails."""
 
 
 class ClosingFailedException(MQClientException):
     """Raised when a `close()` fails."""
 
 
-class AlreadyClosedException(ClosingFailedException):
-    """Raised when a `close()` fails on an already closed interface."""
-
-
 class AckException(MQClientException):
     """Raised when there's a problem with acking."""
 
 
 class NackException(MQClientException):
     """Raised when there's a problem with nacking."""
```

### Comparing `oms-mqclient-2.4.1/mqclient/broker_client_manager.py` & `oms-mqclient-2.4.2/mqclient/broker_client_manager.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.4.2/mqclient/broker_clients/apachepulsar.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import os
 from typing import AsyncGenerator, Optional
 
 import pulsar  # type: ignore
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
-    AlreadyClosedException,
     ClosingFailedException,
     Message,
     MQClientException,
     Pub,
     RawQueue,
     Sub,
 )
@@ -65,15 +64,16 @@
         if not self.client:
             raise ClosingFailedException("No client to close.")
         try:
             self.client.close()
         except Exception as e:
             # https://github.com/apache/pulsar/issues/3127
             if str(e) == "Pulsar error: AlreadyClosed":
-                raise AlreadyClosedException(str(e)) from e
+                LOGGER.warning("Attempted to close a connection that is already closed")
+                return
             raise ClosingFailedException(str(e)) from e
 
 
 class PulsarPub(Pulsar, Pub):
     """Wrapper around pulsar.Producer.
 
     Extends:
```

### Comparing `oms-mqclient-2.4.1/mqclient/broker_clients/nats.py` & `oms-mqclient-2.4.2/mqclient/broker_clients/nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.4.2/mqclient/broker_clients/rabbitmq.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import urllib
 from typing import Any, AsyncGenerator, AsyncIterator, Dict, Optional, Tuple, Union
 
 import pika  # type: ignore
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
-    AlreadyClosedException,
     ClosingFailedException,
     ConnectingFailedException,
     Message,
     MQClientException,
     Pub,
     RawQueue,
     Sub,
@@ -121,15 +120,16 @@
         await super().close()
 
         if not self.channel:
             raise ClosingFailedException("No channel to close.")
         if not self.connection:
             raise ClosingFailedException("No connection to close.")
         if self.connection.is_closed:
-            raise AlreadyClosedException()
+            LOGGER.warning("Attempted to close a connection that is already closed")
+            return
 
         try:
             # self.channel.cancel() -- done by self.connection.close()
             self.connection.close()
         except Exception as e:
             raise ClosingFailedException() from e
```

### Comparing `oms-mqclient-2.4.1/mqclient/broker_clients/utils.py` & `oms-mqclient-2.4.2/mqclient/broker_clients/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/mqclient/log_msgs.py` & `oms-mqclient-2.4.2/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/mqclient/queue.py` & `oms-mqclient-2.4.2/mqclient/queue.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/mqclient/telemetry.py` & `oms-mqclient-2.4.2/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.4.2/oms_mqclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.4.1
+Version: 2.4.2
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.4.1/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.4.2/oms_mqclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/setup.cfg` & `oms-mqclient-2.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.4.2/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.4.2/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.4.2/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.4.2/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/tests/integrate/conftest.py` & `oms-mqclient-2.4.2/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/tests/integrate/test_nats.py` & `oms-mqclient-2.4.2/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/tests/integrate/test_pulsar.py` & `oms-mqclient-2.4.2/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.4.2/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.4.2/tests/unit/pulsar/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.1/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.4.2/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files identical despite different names*

