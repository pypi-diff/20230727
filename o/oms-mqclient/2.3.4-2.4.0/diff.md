# Comparing `tmp/oms-mqclient-2.3.4.tar.gz` & `tmp/oms-mqclient-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.3.4.tar", last modified: Tue Jul 25 18:56:48 2023, max compression
+gzip compressed data, was "oms-mqclient-2.4.0.tar", last modified: Thu Jul 27 00:11:46 2023, max compression
```

## Comparing `oms-mqclient-2.3.4.tar` & `oms-mqclient-2.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.877866 oms-mqclient-2.3.4/mqclient/
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-25 18:56:46.000000 oms-mqclient-2.3.4/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6667 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.877866 oms-mqclient-2.3.4/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14402 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    14188 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    17161 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/broker_clients/utils.py
--rw-r--r--   0 root         (0) root         (0)      395 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    23781 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-25 18:56:48.000000 oms-mqclient-2.3.4/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-25 18:56:48.000000 oms-mqclient-2.3.4/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 18:56:48.000000 oms-mqclient-2.3.4/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      502 2023-07-25 18:56:48.000000 oms-mqclient-2.3.4/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-25 18:56:48.000000 oms-mqclient-2.3.4/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2780 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.877866 oms-mqclient-2.3.4/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9038 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    38812 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    20234 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5586 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 18:56:48.881866 oms-mqclient-2.3.4/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9196 2023-07-25 18:56:45.000000 oms-mqclient-2.3.4/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.835681 oms-mqclient-2.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 00:11:46.835681 oms-mqclient-2.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-27 00:11:44.000000 oms-mqclient-2.4.0/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6595 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14226 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    14314 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    16838 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/broker_clients/utils.py
+-rw-r--r--   0 root         (0) root         (0)      395 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    23348 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-27 00:11:46.000000 oms-mqclient-2.4.0/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-27 00:11:46.000000 oms-mqclient-2.4.0/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 00:11:46.000000 oms-mqclient-2.4.0/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      502 2023-07-27 00:11:46.000000 oms-mqclient-2.4.0/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 00:11:46.000000 oms-mqclient-2.4.0/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-07-27 00:11:46.835681 oms-mqclient-2.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.827680 oms-mqclient-2.4.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8990 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    38812 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    19982 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.831680 oms-mqclient-2.4.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.835681 oms-mqclient-2.4.0/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:11:46.835681 oms-mqclient-2.4.0/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9078 2023-07-27 00:11:43.000000 oms-mqclient-2.4.0/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.3.4/LICENSE` & `oms-mqclient-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/PKG-INFO` & `oms-mqclient-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.3.4
+Version: 2.4.0
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.3.4/README.md` & `oms-mqclient-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/mqclient/__init__.py` & `oms-mqclient-2.4.0/mqclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.3.4"
+__version__ = "2.4.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.3.4/mqclient/broker_client_interface.py` & `oms-mqclient-2.4.0/mqclient/broker_client_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,22 +209,20 @@
     NAME = "abstract-broker_client"
 
     @staticmethod
     async def create_pub_queue(
         address: str,
         name: str,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> Pub:
         """Create a publishing queue."""
         raise NotImplementedError()
 
     @staticmethod
     async def create_sub_queue(
         address: str,
         name: str,
         prefetch: int,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> Sub:
         """Create a subscription queue."""
         raise NotImplementedError()
```

### Comparing `oms-mqclient-2.3.4/mqclient/broker_client_manager.py` & `oms-mqclient-2.4.0/mqclient/broker_client_manager.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.4.0/mqclient/broker_clients/apachepulsar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Back-end using Apache Pulsar."""
 
 import asyncio
 import functools
 import logging
+import os
 from typing import AsyncGenerator, Optional
 
 import pulsar  # type: ignore
 
 from .. import broker_client_interface, log_msgs
 from ..broker_client_interface import (
     AlreadyClosedException,
@@ -29,15 +30,14 @@
     """
 
     def __init__(
         self,
         address: str,
         topic: str,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> None:
         """Set address, topic, and client.
 
         Arguments:
             address {str} -- the pulsar server address, if address doesn't start with 'pulsar', append 'pulsar://'
             topic {str} -- the name of the topic
             auth_token {str} -- the (jwt) authentication token
@@ -48,15 +48,14 @@
         self.address = address
         if not self.address.startswith("pulsar"):
             self.address = "pulsar://" + self.address
         self.topic = topic
         self.client: pulsar.Client = None
         self.auth = pulsar.AuthenticationToken(auth_token) if auth_token else None
         self._auth_token = auth_token
-        self.ack_timeout = ack_timeout
 
     async def connect(self) -> None:
         """Set up client."""
         await super().connect()
         self.client = pulsar.Client(self.address, authentication=self.auth)
 
     async def close(self) -> None:
@@ -82,33 +81,31 @@
     """
 
     def __init__(
         self,
         address: str,
         topic: str,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> None:
         LOGGER.debug(f"{log_msgs.INIT_PUB} ({address}; {topic})")
-        super().__init__(address, topic, auth_token, ack_timeout)
+        super().__init__(address, topic, auth_token)
         self.producer: pulsar.Producer = None
 
     async def connect(self) -> None:
         """Connect to producer."""
         LOGGER.debug(log_msgs.CONNECTING_PUB)
         await super().connect()
 
         # create sub so that subscription is created so messages are forwarded from topic
         # https://pulsar.apache.org/assets/images/pulsar-subscription-types-664733b68c7124129ca7d0e04dedcb96.png
         inner_sub = PulsarSub(
             self.address,
             self.topic,
             BrokerClient.SUBSCRIPTION_NAME,
             self._auth_token,
-            self.ack_timeout,
             prefetch=1,
         )
         await inner_sub.connect()
         await inner_sub.close()
 
         self.producer = self.client.create_producer(self.topic)
         LOGGER.debug(log_msgs.CONNECTED_PUB)
@@ -168,38 +165,41 @@
 
     def __init__(
         self,
         address: str,
         topic: str,
         subscription_name: str,
         auth_token: str,
-        ack_timeout: Optional[int],
         prefetch: int,
     ) -> None:
         LOGGER.debug(f"{log_msgs.INIT_SUB} ({address}; {topic})")
-        super().__init__(address, topic, auth_token, ack_timeout)
+        super().__init__(address, topic, auth_token)
         self.consumer: pulsar.Consumer = None
         self.subscription_name = subscription_name
         self.prefetch = prefetch
 
     async def connect(self) -> None:
         """Connect to subscriber."""
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
 
+        ack_timeout: Optional[int]  # for mypy
+        try:
+            ack_timeout = int(os.environ["PULSAR_UNACKED_MESSAGES_TIMEOUT_SEC"])
+            if ack_timeout < 10:
+                ack_timeout = None
+        except:  # noqa: E722
+            ack_timeout = None
+
         self.consumer = self.client.subscribe(
             self.topic,
             self.subscription_name,
             # Neither receive with timeout nor partitioned topics can be used if the consumer queue size is zero.
             receiver_queue_size=max(self.prefetch, 1),
-            unacked_messages_timeout_ms=(
-                self.ack_timeout * 1000
-                if self.ack_timeout and self.ack_timeout > 10
-                else None
-            ),
+            unacked_messages_timeout_ms=ack_timeout,
             consumer_type=pulsar.ConsumerType.Shared,
             initial_position=pulsar.InitialPosition.Earliest,
             negative_ack_redelivery_delay_ms=0,
         )
         LOGGER.debug(log_msgs.CONNECTED_SUB)
 
     async def close(self) -> None:
@@ -415,38 +415,34 @@
     SUBSCRIPTION_NAME = "i3-pulsar-sub"
 
     @staticmethod
     async def create_pub_queue(
         address: str,
         name: str,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> PulsarPub:
         """Create a publishing queue."""
         q = PulsarPub(  # pylint: disable=invalid-name
             address,
             name,
             auth_token,
-            ack_timeout,
         )
         await q.connect()
         return q
 
     @staticmethod
     async def create_sub_queue(
         address: str,
         name: str,
         prefetch: int,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> PulsarSub:
         """Create a subscription queue."""
         q = PulsarSub(  # pylint: disable=invalid-name
             address,
             name,
             BrokerClient.SUBSCRIPTION_NAME,
             auth_token,
-            ack_timeout,
             prefetch,
         )
         await q.connect()
         return q
```

### Comparing `oms-mqclient-2.3.4/mqclient/broker_clients/nats.py` & `oms-mqclient-2.4.0/mqclient/broker_clients/nats.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,40 +411,44 @@
     NAME = "nats"
 
     @staticmethod
     async def create_pub_queue(
         address: str,
         name: str,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> NATSPub:
         """Create a publishing queue.
 
         # NOTE - `auth_token` is not used currently
         """
+        if auth_token:
+            LOGGER.warning("NATS broker client does not use 'auth_token'")
+
         q = NATSPub(  # pylint: disable=invalid-name
             address,
             name + "-stream",
             name + "-subject",
         )
         await q.connect()
         return q
 
     @staticmethod
     async def create_sub_queue(
         address: str,
         name: str,
         prefetch: int,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> NATSSub:
         """Create a subscription queue.
 
         # NOTE - `auth_token` is not used currently
         """
+        if auth_token:
+            LOGGER.warning("NATS broker client does not use 'auth_token'")
+
         q = NATSSub(  # pylint: disable=invalid-name
             address,
             name + "-stream",
             name + "-subject",
             prefetch,
         )
         await q.connect()
```

### Comparing `oms-mqclient-2.3.4/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.4.0/mqclient/broker_clients/rabbitmq.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,25 +76,23 @@
     """
 
     def __init__(
         self,
         address: str,
         queue: str,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> None:
         super().__init__()
         LOGGER.info(f"Requested MQClient for queue '{queue}' @ {address}")
-        cp_args, username, password = _parse_url(address)
+        cp_args, _user, _pass = _parse_url(address)
 
         # set up connection parameters
-        if creds := _get_credentials(username, password, auth_token):
+        if creds := _get_credentials(_user, _pass, auth_token):
             cp_args["credentials"] = creds
-        if ack_timeout:
-            cp_args["heartbeat"] = ack_timeout
+
         self.parameters = pika.connection.ConnectionParameters(**cp_args)
 
         self.queue = queue
         self.connection: Optional[pika.BlockingConnection] = None
         self.channel: Optional[pika.adapters.blocking_connection.BlockingChannel] = None
 
     async def connect(self) -> None:
@@ -143,18 +141,17 @@
     """
 
     def __init__(
         self,
         address: str,
         name: str,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> None:
         LOGGER.debug(f"{log_msgs.INIT_PUB} ({address}; {name})")
-        super().__init__(address, name, auth_token, ack_timeout)
+        super().__init__(address, name, auth_token)
 
     async def connect(self) -> None:
         """Set up connection, channel, and queue.
 
         Turn on delivery confirmations.
         """
         LOGGER.debug(log_msgs.CONNECTING_PUB)
@@ -233,19 +230,18 @@
     """
 
     def __init__(
         self,
         address: str,
         name: str,
         auth_token: str,
-        ack_timeout: Optional[int],
         prefetch: int,
     ) -> None:
         LOGGER.debug(f"{log_msgs.INIT_SUB} ({address}; {name})")
-        super().__init__(address, name, auth_token, ack_timeout)
+        super().__init__(address, name, auth_token)
         self.consumer_id = None
         self.prefetch = prefetch
 
     async def connect(self) -> None:
         """Set up connection, channel, and queue.
 
         Turn on prefetching.
@@ -497,44 +493,42 @@
     NAME = "rabbitmq"
 
     @staticmethod
     async def create_pub_queue(
         address: str,
         name: str,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> RabbitMQPub:
         """Create a publishing queue.
 
         Args:
             address (str): address of queue
             name (str): name of queue on address
 
         Returns:
             RawQueue: queue
         """
         # pylint: disable=invalid-name
-        q = RabbitMQPub(address, name, auth_token, ack_timeout)
+        q = RabbitMQPub(address, name, auth_token)
         await q.connect()
         return q
 
     @staticmethod
     async def create_sub_queue(
         address: str,
         name: str,
         prefetch: int,
         auth_token: str,
-        ack_timeout: Optional[int],
     ) -> RabbitMQSub:
         """Create a subscription queue.
 
         Args:
             address (str): address of queue
             name (str): name of queue on address
 
         Returns:
             RawQueue: queue
         """
         # pylint: disable=invalid-name
-        q = RabbitMQSub(address, name, auth_token, ack_timeout, prefetch=prefetch)
+        q = RabbitMQSub(address, name, auth_token, prefetch)
         await q.connect()
         return q
```

### Comparing `oms-mqclient-2.3.4/mqclient/broker_clients/utils.py` & `oms-mqclient-2.4.0/mqclient/broker_clients/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/mqclient/log_msgs.py` & `oms-mqclient-2.4.0/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/mqclient/queue.py` & `oms-mqclient-2.4.0/mqclient/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     MIN_PREFETCH,
 )
 
 LOGGER = logging.getLogger("mqclient")
 
 
 # deprecation check
-for envvar in ["RABBITMQ_HEARTBEAT", "PULSAR_UNACKED_MESSAGES_TIMEOUT_SEC"]:
+for envvar in ["RABBITMQ_HEARTBEAT"]:
     if os.getenv(envvar):
         raise RuntimeError(f"Environment variable {envvar} has been deprecated.")
 
 
 def _message_size_message(msg: Message) -> str:
     return (
         f"{sys.getsizeof(msg.payload)} bytes "
@@ -42,30 +42,27 @@
 
     Args:
         broker_client: the broker_client to use
         address: address of queue
         name: name of queue
         prefetch: size of prefetch buffer for receiving messages (min 1)
         timeout: seconds to wait for a message to be delivered
-        ack_timeout: max time (seconds) to acknowledge a message
-                     before broker considers it lost (and re-queues)
         except_errors: whether to suppress interior context errors for
                         the consumer (when `True`, the context manager
                         will act like a `try-except` block)
         auth_token: the (jwt) authentication token
     """
 
     def __init__(
         self,
         broker_client: str,
         address: str = "localhost",
         name: str = "",
         prefetch: int = DEFAULT_PREFETCH,
         timeout: int = DEFAULT_TIMEOUT,
-        ack_timeout: Optional[int] = None,
         retry_delay: float = DEFAULT_RETRY_DELAY,  # seconds
         retries: int = DEFAULT_RETRIES,  # ex: 2 means 1 initial try and 2 retries
         except_errors: bool = DEFAULT_EXCEPT_ERRORS,
         auth_token: str = "",
     ) -> None:
         self._broker_client = broker_client_manager.get_broker_client(broker_client)
         self._address = address
@@ -73,18 +70,14 @@
 
         if prefetch < MIN_PREFETCH:
             raise ValueError(f"prefetch must be >= {MIN_PREFETCH}")
         self._prefetch = prefetch
 
         self._auth_token = auth_token
 
-        if ack_timeout is not None and ack_timeout <= 0:
-            raise ValueError("timeout must be positive")
-        self._ack_timeout = ack_timeout
-
         # properties
         self._timeout = -1
         self.timeout = timeout
         self._retries = -1
         self.retries = retries
         self._retry_delay = -1.0
         self.retry_delay = retry_delay
@@ -139,27 +132,25 @@
     async def _create_pub_queue(self) -> Pub:
         """Wrap `self._broker_client.create_pub_queue()` with instance's
         config."""
         return await self._broker_client.create_pub_queue(
             self._address,
             self._name,
             self._auth_token,
-            self._ack_timeout,
         )
 
     async def _create_sub_queue(self, prefetch_override: Optional[int] = None) -> Sub:
         """Wrap `self._broker_client.create_sub_queue()` with instance's
         config."""
         return await self._broker_client.create_sub_queue(
             self._address,
             self._name,
             # 0 is okay
             prefetch_override if prefetch_override is not None else self._prefetch,
             self._auth_token,
-            self._ack_timeout,
         )
 
     @contextlib.asynccontextmanager  # needs to wrap @wtt stuff to span children correctly
     @wtt.spanned(
         these=[
             "self._broker_client",
             "self._address",
```

### Comparing `oms-mqclient-2.3.4/mqclient/telemetry.py` & `oms-mqclient-2.4.0/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.4.0/oms_mqclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.3.4
+Version: 2.4.0
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.3.4/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.4.0/oms_mqclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/setup.cfg` & `oms-mqclient-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.4.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,18 @@
     broker_client: BrokerClient
     timeout = 1
 
     @pytest.mark.asyncio
     async def test_00(self, queue_name: str, auth_token: str) -> None:
         """Sanity test."""
         pub = await self.broker_client.create_pub_queue(
-            "localhost", queue_name, auth_token, None
+            "localhost", queue_name, auth_token
         )
         sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, auth_token, None
+            "localhost", queue_name, 1, auth_token
         )
 
         # send
         for msg in DATA_LIST:
             raw_data = Message.serialize(msg)
             await pub.send_message(
                 raw_data,
@@ -87,18 +87,18 @@
     @pytest.mark.asyncio
     async def test_10(self, queue_name: str, auth_token: str) -> None:
         """Test nacking, front-loaded sending.
 
         Order is not guaranteed on redelivery.
         """
         pub = await self.broker_client.create_pub_queue(
-            "localhost", queue_name, auth_token, None
+            "localhost", queue_name, auth_token
         )
         sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, auth_token, None
+            "localhost", queue_name, 1, auth_token
         )
 
         # send
         for msg in DATA_LIST:
             raw_data = Message.serialize(msg)
             await pub.send_message(
                 raw_data,
@@ -158,18 +158,18 @@
     @pytest.mark.asyncio
     async def test_11(self, queue_name: str, auth_token: str) -> None:
         """Test nacking, mixed sending and receiving.
 
         Order is not guaranteed on redelivery.
         """
         pub = await self.broker_client.create_pub_queue(
-            "localhost", queue_name, auth_token, None
+            "localhost", queue_name, auth_token
         )
         sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, auth_token, None
+            "localhost", queue_name, 1, auth_token
         )
 
         data_to_send = copy.deepcopy(DATA_LIST)
         nacked_msgs: List[Message] = []
         redelivered_msgs: List[Message] = []
         for i in itertools.count():
             logging.info(i)
@@ -229,18 +229,18 @@
         await pub.close()
         await sub.close()
 
     @pytest.mark.asyncio
     async def test_20(self, queue_name: str, auth_token: str) -> None:
         """Sanity test message generator."""
         pub = await self.broker_client.create_pub_queue(
-            "localhost", queue_name, auth_token, None
+            "localhost", queue_name, auth_token
         )
         sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, auth_token, None
+            "localhost", queue_name, 1, auth_token
         )
 
         # send
         for msg in DATA_LIST:
             raw_data = Message.serialize(msg)
             await pub.send_message(
                 raw_data,
```

### Comparing `oms-mqclient-2.3.4/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.4.0/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.4.0/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,51 +75,45 @@
     async def test_get_message(self, mock_con: Any, queue_name: str) -> None:
         """Test getting message."""
         raise NotImplementedError()
 
     @pytest.mark.asyncio
     async def test_ack_message(self, mock_con: Any, queue_name: str) -> None:
         """Test acking message."""
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
         await sub.ack_message(
             Message(12, b""),
             retries=DEFAULT_RETRIES,
             retry_delay=DEFAULT_RETRY_DELAY,
         )
         self._get_ack_mock_fn(mock_con).assert_called_with(12)
 
     @pytest.mark.asyncio
     async def test_reject_message(self, mock_con: Any, queue_name: str) -> None:
         """Test rejecting message."""
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
         await sub.reject_message(
             Message(12, b""),
             retries=DEFAULT_RETRIES,
             retry_delay=DEFAULT_RETRY_DELAY,
         )
         self._get_nack_mock_fn(mock_con).assert_called_with(12)
 
     @pytest.mark.asyncio
     async def test_message_generator_00(self, mock_con: Any, queue_name: str) -> None:
         """Test message generator."""
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
 
         num_msgs = 100
 
@@ -149,17 +143,15 @@
         self._get_ack_mock_fn(mock_con).assert_not_called()  # would be called by Queue
         # would be called by Queue
         self._get_close_mock_fn(mock_con).assert_not_called()
 
     @pytest.mark.asyncio
     async def test_message_generator_01(self, mock_con: Any, queue_name: str) -> None:
         """Test message generator."""
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
 
         fake_data = [b"foo, bar", b"baz"]
         fake_ids = [12, 20]
@@ -187,17 +179,15 @@
         self._get_ack_mock_fn(mock_con).assert_not_called()  # would be called by Queue
         # would be called by Queue
         self._get_close_mock_fn(mock_con).assert_not_called()
 
     @pytest.mark.asyncio
     async def test_message_generator_02(self, mock_con: Any, queue_name: str) -> None:
         """Test message generator."""
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
 
         await self._enqueue_mock_messages(mock_con, [b"foo, bar"], [12])
 
@@ -235,17 +225,15 @@
     async def test_message_generator_20_no_auto_ack(
         self, mock_con: Any, queue_name: str
     ) -> None:
         """Test message generator.
 
         Generator should not ack messages.
         """
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
 
         fake_data = [b"baz-0", b"baz-1", b"baz-2"]
         fake_ids = [0, 1, 2]
@@ -275,17 +263,15 @@
         self, mock_con: Any, queue_name: str
     ) -> None:
         """Failure-test message generator.
 
         Generator should raise Exception, nack, and close. Unlike in an
         integration test, nacked messages are not put back on the queue.
         """
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
 
         fake_data = [b"baz-0", b"baz-1", b"baz-2"]
         fake_ids = [0, 1, 2]
@@ -326,17 +312,15 @@
         self, mock_con: Any, queue_name: str
     ) -> None:
         """Failure-test message generator.
 
         Generator should not raise Exception. Unlike in an integration
         test, nacked messages are not put back on the queue.
         """
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
 
         num_msgs = 11
         if num_msgs % 2 == 0:
@@ -375,17 +359,15 @@
         self, mock_con: Any, queue_name: str
     ) -> None:
         """Failure-test message generator.
 
         Not so much a test, as an example of why QueueSubResource is
         needed.
         """
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         if is_inst_name(
             self.broker_client, "rabbitmq.BrokerClient"
         ):  # HACK: manually set attr
             mock_con.return_value.is_closed = False
 
         await self._enqueue_mock_messages(mock_con, [b"baz"], [0], append_none=False)
```

### Comparing `oms-mqclient-2.3.4/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.4.0/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/tests/integrate/conftest.py` & `oms-mqclient-2.4.0/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/tests/integrate/test_nats.py` & `oms-mqclient-2.4.0/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/tests/integrate/test_pulsar.py` & `oms-mqclient-2.4.0/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.4.0/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.4/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.4.0/tests/unit/pulsar/test_pulsar.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,51 +50,45 @@
         mock_con.return_value.subscribe.return_value.receive.return_value.message_id.side_effect = (
             ids
         )
 
     @pytest.mark.asyncio
     async def test_create_pub_queue(self, mock_con: Any, queue_name: str) -> None:
         """Test creating pub queue."""
-        pub = await self.broker_client.create_pub_queue(
-            "localhost", queue_name, "", None
-        )
+        pub = await self.broker_client.create_pub_queue("localhost", queue_name, "")
         assert pub.topic == queue_name  # type: ignore
         mock_con.return_value.create_producer.assert_called()
 
     @pytest.mark.asyncio
     async def test_create_sub_queue(self, mock_con: Any, queue_name: str) -> None:
         """Test creating sub queue."""
         sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 213, "", None
+            "localhost", queue_name, 213, ""
         )
         assert sub.topic == queue_name  # type: ignore
         assert sub.prefetch == 213  # type: ignore
         mock_con.return_value.subscribe.assert_called()
 
     @pytest.mark.asyncio
     async def test_send_message(self, mock_con: Any, queue_name: str) -> None:
         """Test sending message."""
-        pub = await self.broker_client.create_pub_queue(
-            "localhost", queue_name, "", None
-        )
+        pub = await self.broker_client.create_pub_queue("localhost", queue_name, "")
         await pub.send_message(
             b"foo, bar, baz",
             retries=DEFAULT_RETRIES,
             retry_delay=DEFAULT_RETRY_DELAY,
         )
         mock_con.return_value.create_producer.return_value.send.assert_called_with(
             b"foo, bar, baz"
         )
 
     @pytest.mark.asyncio
     async def test_get_message(self, mock_con: Any, queue_name: str) -> None:
         """Test getting message."""
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         mock_con.return_value.subscribe.return_value.receive.return_value.data.return_value = Message.serialize(
             "foo, bar"
         )
         mock_con.return_value.subscribe.return_value.receive.return_value.message_id.return_value = (
             12
         )
         m = await sub.get_message(
@@ -112,17 +106,15 @@
         self, mock_con: Any, queue_name: str
     ) -> None:
         """Failure-test message generator.
 
         Generator should raise Exception originating upstream (a.k.a.
         from pulsar-package code).
         """
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
 
         retries = 2  # >= 0
 
         class _MyException(Exception):
             pass
 
         mock_con.return_value.subscribe.return_value.receive.side_effect = (
```

### Comparing `oms-mqclient-2.3.4/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.4.0/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,51 +53,45 @@
         mock_con.return_value.channel.return_value.consume.return_value.__next__.side_effect = (
             messages
         )
 
     @pytest.mark.asyncio
     async def test_create_pub_queue(self, mock_con: Any, queue_name: str) -> None:
         """Test creating pub queue."""
-        pub = await self.broker_client.create_pub_queue(
-            "localhost", queue_name, "", None
-        )
+        pub = await self.broker_client.create_pub_queue("localhost", queue_name, "")
         assert pub.queue == queue_name  # type: ignore
         mock_con.return_value.channel.assert_called()
 
     @pytest.mark.asyncio
     async def test_create_sub_queue(self, mock_con: Any, queue_name: str) -> None:
         """Test creating sub queue."""
         sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 213, "", None
+            "localhost", queue_name, 213, ""
         )
         assert sub.queue == queue_name  # type: ignore
         assert sub.prefetch == 213
         mock_con.return_value.channel.assert_called()
 
     @pytest.mark.asyncio
     async def test_send_message(self, mock_con: Any, queue_name: str) -> None:
         """Test sending message."""
-        pub = await self.broker_client.create_pub_queue(
-            "localhost", queue_name, "", None
-        )
+        pub = await self.broker_client.create_pub_queue("localhost", queue_name, "")
         await pub.send_message(
             b"foo, bar, baz",
             retries=DEFAULT_RETRIES,
             retry_delay=DEFAULT_RETRY_DELAY,
         )
         mock_con.return_value.channel.return_value.basic_publish.assert_called_with(
             exchange="", routing_key=queue_name, body=b"foo, bar, baz"
         )
 
     @pytest.mark.asyncio
     async def test_get_message(self, mock_con: Any, queue_name: str) -> None:
         """Test getting message."""
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         mock_con.return_value.is_closed = False  # HACK - manually set attr
 
         fake_message = (MagicMock(delivery_tag=12), None, Message.serialize("foo, bar"))
         mock_con.return_value.channel.return_value.consume.return_value.__next__.side_effect = [
             fake_message
         ]
         m = await sub.get_message(
@@ -114,17 +108,15 @@
         self, mock_con: Any, queue_name: str
     ) -> None:
         """Failure-test message generator.
 
         Generator should raise Exception originating upstream (a.k.a.
         from pika-package code).
         """
-        sub = await self.broker_client.create_sub_queue(
-            "localhost", queue_name, 1, "", None
-        )
+        sub = await self.broker_client.create_sub_queue("localhost", queue_name, 1, "")
         mock_con.return_value.is_closed = False  # HACK - manually set attr
 
         retries = 2  # >= 0
 
         class _MyException(Exception):
             pass
```

