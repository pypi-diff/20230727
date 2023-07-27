# Comparing `tmp/neon_mq_connector-0.7.1a1.tar.gz` & `tmp/neon_mq_connector-0.7.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_mq_connector-0.7.1a1.tar", last modified: Wed Jul 26 22:55:51 2023, max compression
+gzip compressed data, was "neon_mq_connector-0.7.1a2.tar", last modified: Thu Jul 27 00:59:20 2023, max compression
```

## Comparing `neon_mq_connector-0.7.1a1.tar` & `neon_mq_connector-0.7.1a2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:51.256398 neon_mq_connector-0.7.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-26 22:55:51.256398 neon_mq_connector-0.7.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:51.256398 neon_mq_connector-0.7.1a1/neon_mq_connector/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/neon_mq_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/neon_mq_connector/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    32791 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/neon_mq_connector/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:51.256398 neon_mq_connector-0.7.1a1/neon_mq_connector/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/neon_mq_connector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/neon_mq_connector/utils/client_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/neon_mq_connector/utils/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/neon_mq_connector/utils/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/neon_mq_connector/utils/rabbit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/neon_mq_connector/utils/thread_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:55:51.256398 neon_mq_connector-0.7.1a1/neon_mq_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-26 22:55:51.000000 neon_mq_connector-0.7.1a1/neon_mq_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-26 22:55:51.000000 neon_mq_connector-0.7.1a1/neon_mq_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:55:51.000000 neon_mq_connector-0.7.1a1/neon_mq_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 22:55:51.000000 neon_mq_connector-0.7.1a1/neon_mq_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 22:55:51.000000 neon_mq_connector-0.7.1a1/neon_mq_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:55:51.000000 neon_mq_connector-0.7.1a1/neon_mq_connector.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:55:51.256398 neon_mq_connector-0.7.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-26 22:55:46.000000 neon_mq_connector-0.7.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:59:20.358092 neon_mq_connector-0.7.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-27 00:59:20.358092 neon_mq_connector-0.7.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:59:20.354092 neon_mq_connector-0.7.1a2/neon_mq_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32870 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:59:20.358092 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/rabbit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/neon_mq_connector/utils/thread_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:59:20.358092 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:59:20.000000 neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:59:20.358092 neon_mq_connector-0.7.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-27 00:59:12.000000 neon_mq_connector-0.7.1a2/setup.py
```

### Comparing `neon_mq_connector-0.7.1a1/LICENSE.md` & `neon_mq_connector-0.7.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a1/PKG-INFO` & `neon_mq_connector-0.7.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_mq_connector
-Version: 0.7.1a1
+Version: 0.7.1a2
 Summary: MQ Connector for Neon Modules
 Home-page: https://github.com/NeonGeckoCom/neon_mq_connector
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon_mq_connector-0.7.1a1/README.md` & `neon_mq_connector-0.7.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector/__init__.py` & `neon_mq_connector-0.7.1a2/neon_mq_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector/config.py` & `neon_mq_connector-0.7.1a2/neon_mq_connector/config.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector/connector.py` & `neon_mq_connector-0.7.1a2/neon_mq_connector/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,24 +214,24 @@
         """
         Mapping of basic configurable properties to their default values.
         WARNING: This method should be left untouched to prevent unexpected
         behaviour. To override values of the basic properties specify it in
         self.service_configurable_properties()
         """
         return {
-                'sync_period': 10,  # in seconds
-                'observe_period': 20,  # in seconds
-                'vhost_prefix': '',  # Could be used for scalability purposes
-                'default_testing_prefix': 'test',
-                'testing_envs': (f'{self.service_name.upper()}_TESTING',
-                                 'MQ_TESTING',),  # order matters
-                'testing_prefix_envs': (f'{self.service_name.upper()}'
-                                        f'_TESTING_PREFIX',
-                                        'MQ_TESTING_PREFIX',)  # order matters
-                }
+            'sync_period': 10,  # in seconds
+            'observe_period': 20,  # in seconds
+            'vhost_prefix': '',  # Could be used for scalability purposes
+            'default_testing_prefix': 'test',
+            'testing_envs': (f'{self.service_name.upper()}_TESTING',
+                             'MQ_TESTING',),  # order matters
+            'testing_prefix_envs': (f'{self.service_name.upper()}'
+                                    f'_TESTING_PREFIX',
+                                    'MQ_TESTING_PREFIX',)  # order matters
+        }
 
     @property
     def service_configurable_properties(self) -> Dict[str, Any]:
         """
         Mapping of service-related configurable properties to default values.
         Override to provide service-specific configurable properties AND to
         update the default values of basic properties
@@ -359,35 +359,39 @@
             (defaults to direct)
         :param expiration: mq message expiration time in millis
             (defaults to 1 second)
 
         :raises ValueError: invalid request data provided
         :returns message_id: id of the sent message
         """
-        if request_data and len(request_data) > 0 and isinstance(request_data, dict):
-            message_id = request_data.setdefault('message_id', cls.create_unique_id())
-            with connection.channel() as channel:
-                if exchange:
-                    channel.exchange_declare(exchange=exchange,
-                                             exchange_type=exchange_type,
-                                             auto_delete=False)
-                if queue:
-                    declared_queue = channel.queue_declare(queue=queue,
-                                                           auto_delete=False)
-                    if exchange_type == ExchangeType.fanout.value:
-                        channel.queue_bind(queue=declared_queue.method.queue,
-                                           exchange=exchange)
-                channel.basic_publish(exchange=exchange or '',
-                                      routing_key=queue,
-                                      body=dict_to_b64(request_data),
-                                      properties=pika.BasicProperties(
-                                          expiration=str(expiration)))
-            return message_id
-        else:
-            raise ValueError(f'Invalid request data provided: {request_data}')
+        if not isinstance(request_data, dict):
+            raise TypeError(f"Expected dict and got {type(request_data)}")
+        if not request_data:
+            raise ValueError(f'No request data provided')
+
+        message_id = request_data.setdefault('message_id', cls.create_unique_id())
+
+        with connection.channel() as channel:
+            if exchange:
+                channel.exchange_declare(exchange=exchange,
+                                         exchange_type=exchange_type,
+                                         auto_delete=False)
+            if queue:
+                declared_queue = channel.queue_declare(queue=queue,
+                                                       auto_delete=False)
+                if exchange_type == ExchangeType.fanout.value:
+                    channel.queue_bind(queue=declared_queue.method.queue,
+                                       exchange=exchange)
+            channel.basic_publish(exchange=exchange or '',
+                                  routing_key=queue,
+                                  body=dict_to_b64(request_data),
+                                  properties=pika.BasicProperties(
+                                      expiration=str(expiration)))
+        LOG.debug(f"sent message: {request_data['message_id']}")
+        return request_data['message_id']
 
     @classmethod
     def publish_message(cls,
                         connection: pika.BlockingConnection,
                         request_data: dict,
                         exchange: Optional[str] = '',
                         expiration: int = 1000) -> str:
@@ -431,26 +435,27 @@
 
         :returns message_id: id of the propagated message
         """
         if not vhost:
             vhost = self.vhost
         if not connection_props:
             connection_props = {}
-        LOG.debug(f'Opening connection on vhost={vhost}')
+        LOG.debug(f'Opening connection on vhost={vhost} queue={queue}')
         with self.create_mq_connection(vhost=vhost,
                                        **connection_props) as mq_conn:
             if exchange_type in (ExchangeType.fanout,
                                  ExchangeType.fanout.value,):
-                LOG.debug('Sending fanout request to MQ')
+                LOG.debug(f'Sending fanout request to exchange: {exchange}')
                 msg_id = self.publish_message(connection=mq_conn,
                                               request_data=request_data,
                                               exchange=exchange,
                                               expiration=expiration)
             else:
-                LOG.debug(f'Sending {exchange_type} request to MQ')
+                LOG.debug(f'Sending {exchange_type} request to exchange '
+                          f'{exchange}')
                 msg_id = self.emit_mq_message(mq_conn,
                                               queue=queue,
                                               request_data=request_data,
                                               exchange=exchange,
                                               exchange_type=exchange_type,
                                               expiration=expiration)
         LOG.info(f'Message propagated, id={msg_id}')
@@ -689,15 +694,15 @@
             self._sync_thread = None
 
     def observe_consumers(self):
         """
         Iteratively observes each consumer, and if it was launched but is not
         alive - restarts it
         """
-        LOG.debug('Observers state observation')
+        # LOG.debug('Observers state observation')
         consumers_dict = copy.copy(self.consumers)
         for consumer_name, consumer_instance in consumers_dict.items():
             if self.consumer_properties[consumer_name]['started'] and \
                     not (isinstance(consumer_instance, ConsumerThread)
                          and consumer_instance.is_alive()
                          and consumer_instance.is_consuming):
                 LOG.info(f'Consumer "{consumer_name}" is dead, restarting')
```

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector/utils/__init__.py` & `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector/utils/client_utils.py` & `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/client_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,14 @@
 from pika.exceptions import ProbableAccessDeniedError, StreamLostError
 from neon_mq_connector.connector import MQConnector
 from ovos_config.config import Configuration
 from ovos_utils.log import LOG
 
 from neon_mq_connector.utils.network_utils import b64_to_dict
 
-# TODO: Leave below to configuration
-logging.getLogger("pika").setLevel(logging.CRITICAL)
-
 _default_mq_config = {
     "server": "api.neon.ai",
     "port": 5672,
     "users": {
         "mq_handler": {
             "user": 'neon_api_utils',
             "password": 'Klatchat2021'
@@ -89,19 +86,20 @@
         """
         if isinstance(error, StreamLostError):
             return
         LOG.error(f"{thread} raised {error}")
 
     def handle_mq_response(channel: Channel, method, _, body):
         """
-            Method that handles Neon API output.
-            In case received output message with the desired id, event stops
+        Method that handles Neon API output.
+        In case received output message with the desired id, event stops
         """
         api_output = b64_to_dict(body)
         api_output_msg_id = api_output.get('message_id', None)
+
         if api_output_msg_id == message_id:
             LOG.debug(f'MQ output: {api_output}')
             channel.basic_ack(delivery_tag=method.delivery_tag)
             channel.close()
             response_data.update(api_output)
             response_event.set()
         else:
```

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector/utils/connection_utils.py` & `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/connection_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector/utils/network_utils.py` & `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector/utils/rabbit_utils.py` & `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/rabbit_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector/utils/thread_utils.py` & `neon_mq_connector-0.7.1a2/neon_mq_connector/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector.egg-info/PKG-INFO` & `neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-mq-connector
-Version: 0.7.1a1
+Version: 0.7.1a2
 Summary: MQ Connector for Neon Modules
 Home-page: https://github.com/NeonGeckoCom/neon_mq_connector
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon_mq_connector-0.7.1a1/neon_mq_connector.egg-info/SOURCES.txt` & `neon_mq_connector-0.7.1a2/neon_mq_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon_mq_connector-0.7.1a1/setup.py` & `neon_mq_connector-0.7.1a2/setup.py`

 * *Files identical despite different names*

