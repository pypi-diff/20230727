# Comparing `tmp/oms-mqclient-2.4.0.tar.gz` & `tmp/oms-mqclient-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.4.0.tar", last modified: Thu Jul 27 00:11:46 2023, max compression
+gzip compressed data, was "oms-mqclient-2.4.1.tar", last modified: Thu Jul 27 18:08:41 2023, max compression
```

## Comparing `oms-mqclient-2.4.0.tar` & `oms-mqclient-2.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.835681 oms-mqclient-2.4.0/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 00:11:46.835681 oms-mqclient-2.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/mqclient/
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-27 00:11:44.000000 oms-mqclient-2.4.0/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6595 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14226 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    14314 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    16838 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_clients/utils.py
--rw-r--r--   0 root         (0) root         (0)      395 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    23348 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 00:11:46.000000 oms-mqclient-2.4.0/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-27 00:11:46.000000 oms-mqclient-2.4.0/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 00:11:46.000000 oms-mqclient-2.4.0/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      502 2023-07-27 00:11:46.000000 oms-mqclient-2.4.0/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 00:11:46.000000 oms-mqclient-2.4.0/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2780 2023-07-27 00:11:46.835681 oms-mqclient-2.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.827680 oms-mqclient-2.4.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8990 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    38812 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    19982 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.835681 oms-mqclient-2.4.0/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.835681 oms-mqclient-2.4.0/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9078 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.372916 oms-mqclient-2.4.1/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-27 18:08:38.000000 oms-mqclient-2.4.1/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6720 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.372916 oms-mqclient-2.4.1/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    14392 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    18112 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/broker_clients/utils.py
+-rw-r--r--   0 root         (0) root         (0)      395 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    23476 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.372916 oms-mqclient-2.4.1/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 18:08:41.000000 oms-mqclient-2.4.1/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-27 18:08:41.000000 oms-mqclient-2.4.1/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 18:08:41.000000 oms-mqclient-2.4.1/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      502 2023-07-27 18:08:41.000000 oms-mqclient-2.4.1/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 18:08:41.000000 oms-mqclient-2.4.1/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.372916 oms-mqclient-2.4.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8990 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    38880 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    19982 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:08:41.376916 oms-mqclient-2.4.1/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9102 2023-07-27 18:08:37.000000 oms-mqclient-2.4.1/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.4.0/LICENSE` & `oms-mqclient-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/PKG-INFO` & `oms-mqclient-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.4.0
+Version: 2.4.1
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.4.0/README.md` & `oms-mqclient-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/mqclient/__init__.py` & `oms-mqclient-2.4.1/mqclient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.4.0/mqclient/broker_client_interface.py` & `oms-mqclient-2.4.1/mqclient/broker_client_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,31 +6,35 @@
 from typing import Any, AsyncGenerator, Dict, Optional, Union
 
 from .config import MIN_PREFETCH
 
 MessageID = Union[int, str, bytes]
 
 
-class ConnectingFailedException(Exception):
+class MQClientException(Exception):
+    """Any exception for an error originating here."""
+
+
+class ConnectingFailedException(MQClientException):
     """Raised when a `connect()` fails."""
 
 
-class ClosingFailedException(Exception):
+class ClosingFailedException(MQClientException):
     """Raised when a `close()` fails."""
 
 
 class AlreadyClosedException(ClosingFailedException):
     """Raised when a `close()` fails on an already closed interface."""
 
 
-class AckException(Exception):
+class AckException(MQClientException):
     """Raised when there's a problem with acking."""
 
 
-class NackException(Exception):
+class NackException(MQClientException):
     """Raised when there's a problem with nacking."""
 
 
 class Message:
     """Message object.
 
     Holds msg_id and data.
```

### Comparing `oms-mqclient-2.4.0/mqclient/broker_client_manager.py` & `oms-mqclient-2.4.1/mqclient/broker_client_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Manage the different broker_clients."""
 
 from types import ModuleType
 from typing import Dict, Optional
 
-from .broker_client_interface import BrokerClient
+from .broker_client_interface import BrokerClient, MQClientException
 
 # Import all the broker clients at package import, so any bindings can be built/compiled
 # fmt: off
 _INSTALLED_BROKERS: Dict[str, Optional[ModuleType]] = {}
 # Pulsar
 try:
     from .broker_clients import apachepulsar
@@ -30,15 +30,15 @@
 
 
 def get_broker_client(broker_client_name: str) -> BrokerClient:
     """Get the `BrokerClient` instance per the given name."""
     try:
         module = _INSTALLED_BROKERS[broker_client_name]
     except KeyError:
-        raise RuntimeError(f"Unknown broker client: {broker_client_name}")
+        raise MQClientException(f"Unknown broker client: {broker_client_name}")
 
     if not module:
-        raise RuntimeError(
+        raise MQClientException(
             f"Install the '{broker_client_name.lower()}' extra "
             f"if you want to use the '{broker_client_name}' broker client"
         )
     return module.BrokerClient()  # type: ignore[no-any-return]
```

### Comparing `oms-mqclient-2.4.0/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.4.1/mqclient/broker_clients/apachepulsar.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pulsar  # type: ignore
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
     AlreadyClosedException,
     ClosingFailedException,
     Message,
+    MQClientException,
     Pub,
     RawQueue,
     Sub,
 )
 from . import utils
 
 LOGGER = logging.getLogger("mqclient.pulsar")
@@ -123,20 +124,20 @@
         msg: bytes,
         retries: int,
         retry_delay: float,
     ) -> None:
         """Send a message on a queue."""
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
         if not self.producer:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
         def _send_msg():
             # use wrapper function so connection references can be updated by reconnects
             if not self.producer:
-                raise RuntimeError("queue is not connected")
+                raise MQClientException("queue is not connected")
             return self.producer.send(msg)
 
         await utils.auto_retry_call(
             func=_send_msg,
             retries=retries,
             retry_delay=retry_delay,
             close=(
@@ -238,20 +239,20 @@
         """Get a single message from a queue.
 
         To endlessly block until a message is available, set
         `timeout_millis=None`.
         """
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
         if not self.consumer:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
         def _get_msg():
             # use wrapper function so connection references can be updated by reconnects
             if not self.consumer:
-                raise RuntimeError("queue is not connected")
+                raise MQClientException("queue is not connected")
             return self.consumer.receive(timeout_millis=timeout_millis)
 
         try:
             pulsar_msg = await utils.auto_retry_call(
                 func=_get_msg,
                 retries=retries,
                 retry_delay=retry_delay,
@@ -287,15 +288,15 @@
         msg: Message,
         retries: int,
         retry_delay: float,
     ) -> None:
         """Ack a message from the queue."""
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
         if not self.consumer:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
         if isinstance(msg.msg_id, bytes):
             pulsar_msg = pulsar.MessageId.deserialize(msg.msg_id)
         else:
             pulsar_msg = msg.msg_id
 
         await utils.auto_retry_call(
@@ -317,15 +318,15 @@
         msg: Message,
         retries: int,
         retry_delay: float,
     ) -> None:
         """Reject (nack) a message from the queue."""
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
         if not self.consumer:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
         if isinstance(msg.msg_id, bytes):
             pulsar_msg = pulsar.MessageId.deserialize(msg.msg_id)
         else:
             pulsar_msg = msg.msg_id
 
         await utils.auto_retry_call(
@@ -356,15 +357,15 @@
 
         Keyword Arguments:
             timeout {int} -- timeout in seconds for inactivity (default: {60})
             propagate_error {bool} -- should errors from downstream code kill the generator? (default: {True})
         """
         LOGGER.debug(log_msgs.MSGGEN_ENTERED)
         if not self.consumer:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
         msg = None
         try:
             while True:
                 # get message
                 LOGGER.debug(log_msgs.MSGGEN_GET_NEW_MESSAGE)
                 msg = await self.get_message(
```

### Comparing `oms-mqclient-2.4.0/mqclient/broker_clients/nats.py` & `oms-mqclient-2.4.1/mqclient/broker_clients/nats.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import nats
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
     ClosingFailedException,
     Message,
+    MQClientException,
     Pub,
     RawQueue,
     Sub,
 )
 from ..config import DEFAULT_TIMEOUT_MILLIS
 from . import utils
 
@@ -102,20 +103,20 @@
         msg: bytes,
         retries: int,
         retry_delay: float,
     ) -> None:
         """Send a message (publish)."""
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
         if not self.js:
-            raise RuntimeError("JetStream is not connected")
+            raise MQClientException("JetStream is not connected")
 
         async def _send_msg():
             # use wrapper function so connection references can be updated by reconnects
             if not self.js:
-                raise RuntimeError("JetStream is not connected")
+                raise MQClientException("JetStream is not connected")
             return await self.js.publish(self.subject, msg)
 
         ack: nats.js.api.PubAck = await utils.auto_retry_call(
             func=_send_msg,
             retries=retries,
             retry_delay=retry_delay,
             close=self.close,
@@ -148,15 +149,15 @@
         self.prefetch = prefetch
 
     async def connect(self) -> None:
         """Set up sub (pull subscription)."""
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
         if not self.js:
-            raise RuntimeError("JetStream is not connected.")
+            raise MQClientException("JetStream is not connected.")
 
         self._subscription = await self.js.pull_subscribe(self.subject, "psub")
         LOGGER.debug(log_msgs.CONNECTED_SUB)
 
     async def close(self) -> None:
         """Close sub."""
         LOGGER.debug(log_msgs.CLOSING_SUB)
@@ -174,15 +175,15 @@
 
     def _from_message(self, msg: Message) -> nats.aio.msg.Msg:
         """Transform Message instance to NATS-Message.
 
         Assumes the message came from this NATSSub instance.
         """
         if not self._nats_client:
-            raise RuntimeError("Client is not connected")
+            raise MQClientException("Client is not connected")
 
         return nats.aio.msg.Msg(
             _client=self._nats_client,
             subject=self.subject,
             reply=cast(str, msg.msg_id),  # we know this is str b/c `_to_message()`
             data=msg.data,
             headers=None,  # default
@@ -197,23 +198,23 @@
     ) -> List[Message]:
         """Get n messages.
 
         The subscriber pulls a specific number of messages. The actual
         number of messages pulled may be smaller than `num_messages`.
         """
         if not self._subscription:
-            raise RuntimeError("Subscriber is not connected")
+            raise MQClientException("Subscriber is not connected")
 
         if not timeout_millis:
             timeout_millis = DEFAULT_TIMEOUT_MILLIS
 
         async def _get_msg():
             # use wrapper function so connection references can be updated by reconnects
             if not self._subscription:
-                raise RuntimeError("Subscriber is not connected")
+                raise MQClientException("Subscriber is not connected")
             return await self._subscription.fetch(
                 batch=num_messages,
                 timeout=int(math.ceil(timeout_millis / 1000)),
             )
 
         try:
             nats_msgs: List[nats.aio.msg.Msg] = await utils.auto_retry_call(
@@ -245,15 +246,15 @@
         timeout_millis: Optional[int],
         retries: int,
         retry_delay: float,
     ) -> Optional[Message]:
         """Get a message."""
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
         if not self._subscription:
-            raise RuntimeError("Subscriber is not connected.")
+            raise MQClientException("Subscriber is not connected.")
 
         try:
             msg = (
                 await self._get_messages(
                     timeout_millis,
                     1,
                     retries,
@@ -269,15 +270,15 @@
         timeout_millis: Optional[int],
         num_messages: int,
         retries: int,
         retry_delay: float,
     ) -> AsyncGenerator[Message, None]:
         """Continuously generate messages until there are no more."""
         if not self._subscription:
-            raise RuntimeError("Subscriber is not connected.")
+            raise MQClientException("Subscriber is not connected.")
 
         while True:
             msgs = await self._get_messages(
                 timeout_millis,
                 num_messages,
                 retries,
                 retry_delay,
@@ -292,15 +293,15 @@
         msg: Message,
         retries: int,
         retry_delay: float,
     ) -> None:
         """Ack a message from the queue."""
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
         if not self._subscription:
-            raise RuntimeError("subscriber is not connected")
+            raise MQClientException("subscriber is not connected")
 
         async def _ack_msg():
             # use wrapper function so connection references can be updated by reconnects
             return await self._from_message(msg).ack()
 
         # Acknowledges the received messages so they will not be sent again.
         await utils.auto_retry_call(
@@ -319,15 +320,15 @@
         msg: Message,
         retries: int,
         retry_delay: float,
     ) -> None:
         """Reject (nack) a message from the queue."""
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
         if not self._subscription:
-            raise RuntimeError("subscriber is not connected")
+            raise MQClientException("subscriber is not connected")
 
         async def _nack_msg():
             # use wrapper function so connection references can be updated by reconnects
             return await self._from_message(msg).nak()  # yes, it's "nak"
 
         await utils.auto_retry_call(
             func=_nack_msg,
@@ -354,15 +355,15 @@
 
         Keyword Arguments:
             timeout {int} -- timeout in seconds for inactivity (default: {60})
             propagate_error {bool} -- should errors from downstream code kill the generator? (default: {True})
         """
         LOGGER.debug(log_msgs.MSGGEN_ENTERED)
         if not self._subscription:
-            raise RuntimeError("subscriber is not connected")
+            raise MQClientException("subscriber is not connected")
 
         msg = None
         try:
             gen = self._gen_messages(
                 timeout * 1000,
                 self.prefetch,  # prefetch = # of msgs pulled
                 retries,
```

### Comparing `oms-mqclient-2.4.0/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.4.1/mqclient/broker_clients/rabbitmq.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,24 +9,29 @@
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
     AlreadyClosedException,
     ClosingFailedException,
     ConnectingFailedException,
     Message,
+    MQClientException,
     Pub,
     RawQueue,
     Sub,
 )
 from . import utils
 
 StrDict = Dict[str, Any]
 
 LOGGER = logging.getLogger("mqclient.rabbitmq")
 
+HEARTBEAT_STREAMLOSTERROR_MSG = (
+    "pika.exceptions.StreamLostError: may be due to a missed heartbeat"
+)
+
 
 HUMAN_PATTERN = "[SCHEME://][USER[:PASS]@]HOST[:PORT][/VIRTUAL_HOST]"
 
 
 def _parse_url(url: str) -> Tuple[StrDict, Optional[str], Optional[str]]:
     if "://" not in url:
         url = "//" + url
@@ -39,15 +44,15 @@
         virtual_host=result.path.lstrip("/"),
     )
     # for putting into ConnectionParameters filter ""/None (will rely on defaults)
     parts = {k: v for k, v in parts.items() if v}  # host=..., etc.
 
     # check validity
     if not parts or "host" not in parts:
-        raise RuntimeError(f"Invalid address: {url} (format: {HUMAN_PATTERN})")
+        raise MQClientException(f"Invalid address: {url} (format: {HUMAN_PATTERN})")
 
     return parts, result.username, result.password
 
 
 def _get_credentials(
     username: Optional[str], password: Optional[str], auth_token: str
 ) -> Optional[pika.credentials.PlainCredentials]:
@@ -58,15 +63,15 @@
     if username and password:
         return pika.credentials.PlainCredentials(username, password)
     # Case 2: Only password/token -- Ex: keycloak
     elif (not username) and password:
         return pika.credentials.PlainCredentials("", password)
     # Error: no password for user
     elif username and (not password):
-        raise RuntimeError("username given but no password or token")
+        raise MQClientException("username given but no password or token")
     # Case 3: no auth -- rabbitmq uses guest/guest
     else:  # not username and not password
         return None
 
 
 class RabbitMQ(RawQueue):
     """Base RabbitMQ wrapper.
@@ -183,46 +188,50 @@
             name (str): name of queue on address
 
         Returns:
             RawQueue: queue
         """
         LOGGER.debug(log_msgs.SENDING_MESSAGE)
         if not self.channel:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
         def _send_msg():
             # use wrapper function so connection references can be updated by reconnects
             if not self.channel:
-                raise RuntimeError("queue is not connected")
+                raise MQClientException("queue is not connected")
             return self.channel.basic_publish(
                 exchange="",
                 routing_key=self.queue,
                 body=msg,
             )
 
-        await utils.auto_retry_call(
-            func=_send_msg,
-            nonretriable_conditions=lambda e: isinstance(
-                e, pika.exceptions.AMQPChannelError
-            ),
-            retries=retries,
-            retry_delay=retry_delay,
-            close=(
-                None
-                if self.connection_can_have_multiple_unacked_messages
-                else self.close
-            ),
-            connect=(
-                None
-                if self.connection_can_have_multiple_unacked_messages
-                else self.connect
-            ),
-            logger=LOGGER,
-        )
-        LOGGER.debug(log_msgs.SENT_MESSAGE)
+        try:
+            await utils.auto_retry_call(
+                func=_send_msg,
+                nonretriable_conditions=lambda e: isinstance(
+                    e,
+                    (pika.exceptions.AMQPChannelError, pika.exceptions.StreamLostError),
+                ),
+                retries=retries,
+                retry_delay=retry_delay,
+                close=(
+                    None
+                    if self.connection_can_have_multiple_unacked_messages
+                    else self.close
+                ),
+                connect=(
+                    None
+                    if self.connection_can_have_multiple_unacked_messages
+                    else self.connect
+                ),
+                logger=LOGGER,
+            )
+            LOGGER.debug(log_msgs.SENT_MESSAGE)
+        except pika.exceptions.StreamLostError as e:
+            raise MQClientException(HEARTBEAT_STREAMLOSTERROR_MSG) from e
 
 
 class RabbitMQSub(RabbitMQ, Sub):
     """Wrapper around queue with prefetch-queue QoS.
 
     Extends:
         RabbitMQ
@@ -293,20 +302,20 @@
     async def _iter_messages(
         self,
         timeout_millis: Optional[int],
         retries: int,
         retry_delay: float,
     ) -> AsyncIterator[Optional[Message]]:
         if not self.channel:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
         def _get_msg():
             # use wrapper function so connection references can be updated by reconnects
             if not self.channel:
-                raise RuntimeError("queue is not connected")
+                raise MQClientException("queue is not connected")
             return next(
                 # pika smartly handles re-invocations
                 self.channel.consume(
                     self.queue,
                     inactivity_timeout=timeout_millis / 1000.0
                     if timeout_millis
                     else None,
@@ -314,15 +323,20 @@
             )
 
         while True:
             try:
                 pika_msg = await utils.auto_retry_call(
                     func=_get_msg,
                     nonretriable_conditions=lambda e: isinstance(
-                        e, (pika.exceptions.AMQPChannelError, StopIteration)
+                        e,
+                        (
+                            pika.exceptions.AMQPChannelError,
+                            pika.exceptions.StreamLostError,
+                            StopIteration,
+                        ),
                     ),
                     retries=retries,
                     retry_delay=retry_delay,
                     close=(
                         None
                         if self.connection_can_have_multiple_unacked_messages
                         else self.close
@@ -333,14 +347,16 @@
                         else self.connect
                     ),
                     logger=LOGGER,
                 )
             except StopIteration:
                 LOGGER.debug(log_msgs.GETMSG_TIMEOUT_ERROR)
                 return
+            except pika.exceptions.StreamLostError as e:
+                raise MQClientException(HEARTBEAT_STREAMLOSTERROR_MSG) from e
             if msg := RabbitMQSub._to_message(pika_msg[0], pika_msg[2]):  # type: ignore[index]
                 LOGGER.debug(f"{log_msgs.GETMSG_RECEIVED_MESSAGE} ({msg.msg_id!r}).")
                 yield msg
             else:
                 LOGGER.debug(log_msgs.GETMSG_NO_MESSAGE)
                 yield None
 
@@ -349,15 +365,15 @@
         timeout_millis: Optional[int],
         retries: int,
         retry_delay: float,
     ) -> Optional[Message]:
         """Get a message from a queue."""
         LOGGER.debug(log_msgs.GETMSG_RECEIVE_MESSAGE)
         if not self.channel:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
         msg = None
         async for msg in self._iter_messages(timeout_millis, retries, retry_delay):
             # None -> timeout
             break  # get just one message
 
         # self.channel.cancel()  # this is done by `open_sub_one()` *after* ack/nack via `close()`
@@ -373,62 +389,70 @@
         """Ack a message from the queue.
 
         Note that RabbitMQ acks messages in-order, so acking message 3
         of 3 in-progress messages will ack them all.
         """
         LOGGER.debug(log_msgs.ACKING_MESSAGE)
         if not self.channel:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
-        await utils.auto_retry_call(
-            func=functools.partial(
-                self.channel.basic_ack,
-                msg.msg_id,
-            ),
-            connect=None,
-            close=None,
-            nonretriable_conditions=lambda e: isinstance(
-                e, pika.exceptions.AMQPChannelError
-            ),
-            retries=retries,
-            retry_delay=retry_delay,
-            logger=LOGGER,
-        )
-        LOGGER.debug(f"{log_msgs.ACKED_MESSAGE} ({msg.msg_id!r}).")
+        try:
+            await utils.auto_retry_call(
+                func=functools.partial(
+                    self.channel.basic_ack,
+                    msg.msg_id,
+                ),
+                connect=None,
+                close=None,
+                nonretriable_conditions=lambda e: isinstance(
+                    e,
+                    (pika.exceptions.AMQPChannelError, pika.exceptions.StreamLostError),
+                ),
+                retries=retries,
+                retry_delay=retry_delay,
+                logger=LOGGER,
+            )
+            LOGGER.debug(f"{log_msgs.ACKED_MESSAGE} ({msg.msg_id!r}).")
+        except pika.exceptions.StreamLostError as e:
+            raise MQClientException(HEARTBEAT_STREAMLOSTERROR_MSG) from e
 
     async def reject_message(
         self,
         msg: Message,
         retries: int,
         retry_delay: float,
     ) -> None:
         """Reject (nack) a message from the queue.
 
         Note that RabbitMQ acks messages in-order, so nacking message 3
         of 3 in-progress messages will nack them all.
         """
         LOGGER.debug(log_msgs.NACKING_MESSAGE)
         if not self.channel:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
-        await utils.auto_retry_call(
-            func=functools.partial(
-                self.channel.basic_nack,
-                msg.msg_id,
-            ),
-            close=None,
-            connect=None,
-            nonretriable_conditions=lambda e: isinstance(
-                e, pika.exceptions.AMQPChannelError
-            ),
-            retries=retries,
-            retry_delay=retry_delay,
-            logger=LOGGER,
-        )
-        LOGGER.debug(f"{log_msgs.NACKED_MESSAGE} ({msg.msg_id!r}).")
+        try:
+            await utils.auto_retry_call(
+                func=functools.partial(
+                    self.channel.basic_nack,
+                    msg.msg_id,
+                ),
+                close=None,
+                connect=None,
+                nonretriable_conditions=lambda e: isinstance(
+                    e,
+                    (pika.exceptions.AMQPChannelError, pika.exceptions.StreamLostError),
+                ),
+                retries=retries,
+                retry_delay=retry_delay,
+                logger=LOGGER,
+            )
+            LOGGER.debug(f"{log_msgs.NACKED_MESSAGE} ({msg.msg_id!r}).")
+        except pika.exceptions.StreamLostError as e:
+            raise MQClientException(HEARTBEAT_STREAMLOSTERROR_MSG) from e
 
     async def message_generator(
         self,
         timeout: int,
         propagate_error: bool,
         retries: int,
         retry_delay: float,
@@ -440,15 +464,15 @@
 
         Keyword Arguments:
             timeout {int} -- timeout in seconds for inactivity (default: {60})
             propagate_error -- should errors from downstream kill the generator? (default: {True})
         """
         LOGGER.debug(log_msgs.MSGGEN_ENTERED)
         if not self.channel:
-            raise RuntimeError("queue is not connected")
+            raise MQClientException("queue is not connected")
 
         msg = None
         try:
             async for msg in self._iter_messages(timeout * 1000, retries, retry_delay):
                 LOGGER.debug(log_msgs.MSGGEN_GET_NEW_MESSAGE)
                 if not msg:
                     LOGGER.info(log_msgs.MSGGEN_NO_MESSAGE_LOOK_BACK_IN_QUEUE)
```

### Comparing `oms-mqclient-2.4.0/mqclient/broker_clients/utils.py` & `oms-mqclient-2.4.1/mqclient/broker_clients/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 
 import asyncio
 import inspect
 import logging
 from typing import Awaitable, Callable, Optional, TypeVar, Union
 
+from ..broker_client_interface import MQClientException
+
 T = TypeVar("T")  # the callable/awaitable return type
 
 
 def _ci_test_retry_trigger(i: int) -> None:
     pass
 
 
@@ -31,32 +33,36 @@
             _ci_test_retry_trigger(i)  # only used for testing
             ret = func()
             if inspect.isawaitable(ret):
                 return await ret  # type: ignore[no-any-return]
             else:
                 return ret  # type: ignore[return-value]
         except Exception as e:
+            logger.error(f"Broker client action failed with {type(e).__name__}")
             logger.exception(e)
             if nonretriable_conditions and nonretriable_conditions(e):
+                logger.error(
+                    f"Broker client action failure ({type(e).__name__}) is not retriable"
+                )
                 raise
             elif i == retries:
-                logger.info(
-                    f"[auto_retry_call()] {type(e)}. Reached max retries. Raising..."
+                logger.error(
+                    f"Broker client action failure ({type(e).__name__}) was final try -- raising..."
                 )
                 raise
             else:
-                logger.info(
-                    f"[auto_retry_call()] {type(e)}. Trying again. (attempt #{i+2})..."
+                logger.warning(
+                    f"Broker client action failure ({type(e).__name__}) is retriable -- trying again (attempt #{i+2})..."
                 )
 
         # close, wait, reconnect
         if close:
             try:
                 await close()  # the previous error could've been due to a closed connection
             except:  # noqa: E722
                 pass
         await asyncio.sleep(retry_delay)
         if connect:
             await connect()
 
     # fall through -- this should not be reached in any situation
-    raise RuntimeError("unknown error in auto_retry_call()")
+    raise MQClientException("unknown error in auto_retry_call()")
```

### Comparing `oms-mqclient-2.4.0/mqclient/log_msgs.py` & `oms-mqclient-2.4.1/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/mqclient/queue.py` & `oms-mqclient-2.4.1/mqclient/queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,22 @@
 import sys
 import types
 import uuid
 from typing import Any, AsyncGenerator, AsyncIterator, Dict, List, Optional, Type
 
 from . import broker_client_manager
 from . import telemetry as wtt
-from .broker_client_interface import AckException, Message, NackException, Pub, Sub
+from .broker_client_interface import (
+    AckException,
+    Message,
+    MQClientException,
+    NackException,
+    Pub,
+    Sub,
+)
 from .config import (
     DEFAULT_EXCEPT_ERRORS,
     DEFAULT_PREFETCH,
     DEFAULT_RETRIES,
     DEFAULT_RETRY_DELAY,
     DEFAULT_TIMEOUT,
     MIN_PREFETCH,
@@ -22,15 +29,15 @@
 
 LOGGER = logging.getLogger("mqclient")
 
 
 # deprecation check
 for envvar in ["RABBITMQ_HEARTBEAT"]:
     if os.getenv(envvar):
-        raise RuntimeError(f"Environment variable {envvar} has been deprecated.")
+        raise MQClientException(f"Environment variable {envvar} has been deprecated.")
 
 
 def _message_size_message(msg: Message) -> str:
     return (
         f"{sys.getsizeof(msg.payload)} bytes "
         f"(data={sys.getsizeof(msg.data)}, headers={sys.getsizeof(msg.headers)}) "
         f"[msg_id={msg.msg_id!r}]"
@@ -210,15 +217,15 @@
             raise AckException(
                 f"Message has already been nacked, it cannot be acked: {msg}"
             )
         elif msg._ack_status == Message.AckStatus.ACKED:
             # needless, so we'll skip it
             LOGGER.debug(f"Attempted to ack an already-acked message: {msg}")
         else:
-            raise RuntimeError(f"Unrecognized AckStatus value: {msg}")
+            raise MQClientException(f"Unrecognized AckStatus value: {msg}")
 
     @wtt.spanned(
         these=[
             "self._broker_client",
             "self._address",
             "self._name",
             "self._prefetch",
@@ -243,15 +250,15 @@
             # needless, so we'll skip it
             LOGGER.debug(f"Attempted to nack an already-nacked message: {msg}")
         elif msg._ack_status == Message.AckStatus.ACKED:
             raise NackException(
                 f"Message has already been acked, it cannot be nacked: {msg}"
             )
         else:
-            raise RuntimeError(f"Unrecognized AckStatus value: {msg}")
+            raise MQClientException(f"Unrecognized AckStatus value: {msg}")
 
     def open_sub(self) -> "QueueSubResource":
         """Open a resource to receive messages from the queue as an iterator.
 
         This returns a context-manager/generator. Its iterator stops when no
         messages are received for `timeout` seconds. If an exception is raised
         (inside the context), the message is rejected, the context is exited,
@@ -475,15 +482,15 @@
         )
 
     def _get_sub(self, msg: Message) -> Sub:
         subs = [s for s, addrs in self._subs.items() if id(msg) in addrs]
         if not subs:
             raise ValueError("message cannot be mapped to a sub")
         elif len(subs) != 1:
-            raise RuntimeError("message found in more than one sub")
+            raise MQClientException("message found in more than one sub")
         else:
             return subs[0]
 
     async def ack(self, msg: Message) -> None:
         """Acknowledge the message."""
         sub = self._get_sub(msg)
         await self.queue._safe_ack(sub, msg)
@@ -533,15 +540,17 @@
         """Return instance.
 
         Triggered by 'with ... as'.
         """
         LOGGER.debug("[QueueSubResource.__aenter__()] entered `with-as` block")
 
         if self._sub and self._gen:
-            raise RuntimeError("A 'QueueSubResource' instance cannot be re-entered.")
+            raise MQClientException(
+                "A 'QueueSubResource' instance cannot be re-entered."
+            )
 
         self._sub = await self.queue._create_sub_queue()
         self._gen = self._sub.message_generator(
             timeout=self.queue.timeout,
             propagate_error=(not self.queue.except_errors),
             retries=self.queue.retries,
             retry_delay=self.queue.retry_delay,
@@ -571,15 +580,15 @@
             exc_val {Optional[Type[BaseException]]} -- Exception object.
             exc_tb {Optional[types.TracebackType]} -- Exception Traceback.
         """
         LOGGER.debug(
             f"[QueueSubResource.__aexit__()] exiting `with-as` block (exc:{exc_type})"
         )
         if not (self._sub and self._gen):
-            raise RuntimeError(self.RUNTIME_ERROR_CONTEXT_STRING)
+            raise MQClientException(self.RUNTIME_ERROR_CONTEXT_STRING)
 
         reraise_exception = False
 
         # Exception Was Raised
         if exc_type and exc_val:
             if self.msg:
                 await self.queue._safe_nack(self._sub, self.msg)
@@ -613,15 +622,15 @@
     def __aiter__(self) -> "QueueSubResource":
         """Return instance.
 
         Triggered with 'for'/'aiter()'.
         """
         LOGGER.debug("[QueueSubResource.__aiter__()] entered loop/`aiter()`")
         if not (self._sub and self._gen):
-            raise RuntimeError(self.RUNTIME_ERROR_CONTEXT_STRING)
+            raise MQClientException(self.RUNTIME_ERROR_CONTEXT_STRING)
         return self
 
     @wtt.spanned(
         these=[
             "self.queue._broker_client",
             "self.queue._address",
             "self.queue._name",
@@ -630,15 +639,15 @@
         ],
         carrier="self._span_carrier",
     )
     async def __anext__(self) -> Any:
         """Return next Message in queue."""
         LOGGER.debug("[QueueSubResource.__anext__()] next iteration...")
         if not (self._sub and self._gen):
-            raise RuntimeError(self.RUNTIME_ERROR_CONTEXT_STRING)
+            raise MQClientException(self.RUNTIME_ERROR_CONTEXT_STRING)
 
         # ack the previous message before getting a new one (unless it was already nacked)
         if self.msg and self.msg._ack_status != Message.AckStatus.NACKED:
             await self.queue._safe_ack(self._sub, self.msg)
 
         @wtt.spanned(
             kind=wtt.SpanKind.CONSUMER,
@@ -654,15 +663,15 @@
             self.msg = None  # signal there is no message to ack/nack in `__aexit__()`
             LOGGER.debug(
                 "[QueueSubResource.__anext__()] end of loop (StopAsyncIteration)"
             )
             raise
 
         if not self.msg:
-            raise RuntimeError(
+            raise MQClientException(
                 "Yielded value is `None`. This should not have happened."
             )
 
         LOGGER.info(f"Received Message: {_message_size_message(self.msg)}")
         return self.msg.data
 
     @wtt.spanned(
@@ -673,12 +682,12 @@
             "self.queue._prefetch",
             "self.queue.timeout",
         ],
     )
     async def nack_current(self) -> None:
         """Manually nack the current (most recently yielded) message."""
         if not (self._sub and self._gen):
-            raise RuntimeError(self.RUNTIME_ERROR_CONTEXT_STRING)
+            raise MQClientException(self.RUNTIME_ERROR_CONTEXT_STRING)
         if not self.msg:  # case: calling after iterator stopped (unusual but possible)
             return
         # pylint:disable=protected-access
         await self.queue._safe_nack(self._sub, self.msg)
```

### Comparing `oms-mqclient-2.4.0/mqclient/telemetry.py` & `oms-mqclient-2.4.1/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.4.1/oms_mqclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.4.0
+Version: 2.4.1
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.4.0/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.4.1/oms_mqclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/setup.cfg` & `oms-mqclient-2.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.4.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.4.1/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import random
 from multiprocessing.dummy import Pool as ThreadPool
 from typing import Any, List, Optional
 from unittest.mock import patch
 
 import asyncstdlib as asl
 import pytest
+from mqclient.broker_client_interface import MQClientException
 from mqclient.queue import EmptyQueueException, Queue
 
 from .utils import (
     DATA_LIST,
     _log_recv,
     _log_recv_multiple,
     _log_send,
@@ -733,15 +734,15 @@
             async for i, d in asl.enumerate(gen):
                 print(f"{i}: `{d}`")
                 # assert d == DATA_LIST[i]  # we don't guarantee order
 
         logging.warning("Round 2!")
 
         # continue where we left off
-        with pytest.raises(RuntimeError):
+        with pytest.raises(MQClientException):
             async with recv_gen as gen:
                 assert 0  # we should never get here
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
     async def test_120_break(self, queue_name: str, auth_token: str) -> None:
         """Test open_sub() with a `break` statement."""
```

### Comparing `oms-mqclient-2.4.0/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.4.1/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.4.1/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/tests/integrate/conftest.py` & `oms-mqclient-2.4.1/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/tests/integrate/test_nats.py` & `oms-mqclient-2.4.1/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/tests/integrate/test_pulsar.py` & `oms-mqclient-2.4.1/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.4.1/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.4.1/tests/unit/pulsar/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.4.0/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.4.1/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import itertools
 from typing import Any, List, Optional, Tuple
 from unittest.mock import MagicMock
 
 import pika  # type: ignore[import]
 import pytest
 from mqclient import broker_client_manager
-from mqclient.broker_client_interface import Message
+from mqclient.broker_client_interface import Message, MQClientException
 from mqclient.broker_clients.rabbitmq import HUMAN_PATTERN, _get_credentials, _parse_url
 from mqclient.config import (
     DEFAULT_RETRIES,
     DEFAULT_RETRY_DELAY,
     DEFAULT_TIMEOUT,
     DEFAULT_TIMEOUT_MILLIS,
 )
@@ -213,15 +213,15 @@
         assert _get_credentials("username", "password", "") == cred
         # Sub-case: username/auth_token (override)
         cred = pika.credentials.PlainCredentials("username", "auth_token")
         assert _get_credentials("username", "password", "auth_token") == cred
         assert _get_credentials("username", None, "auth_token") == cred
 
         # Error: no password for user
-        with pytest.raises(RuntimeError):
+        with pytest.raises(MQClientException):
             _get_credentials("username", None, "")
 
         # Case 2: Only password/token -- Ex: keycloak
         cred = pika.credentials.PlainCredentials("", "password")
         assert _get_credentials(None, "password", "") == cred
         #
         cred = pika.credentials.PlainCredentials("", "auth_token")
```

