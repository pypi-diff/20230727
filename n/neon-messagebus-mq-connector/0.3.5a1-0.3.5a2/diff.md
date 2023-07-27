# Comparing `tmp/neon-messagebus-mq-connector-0.3.5a1.tar.gz` & `tmp/neon-messagebus-mq-connector-0.3.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-messagebus-mq-connector-0.3.5a1.tar", last modified: Tue Jul 25 23:25:43 2023, max compression
+gzip compressed data, was "neon-messagebus-mq-connector-0.3.5a2.tar", last modified: Thu Jul 27 20:22:35 2023, max compression
```

## Comparing `neon-messagebus-mq-connector-0.3.5a1.tar` & `neon-messagebus-mq-connector-0.3.5a2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:25:43.724092 neon-messagebus-mq-connector-0.3.5a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-25 23:25:43.724092 neon-messagebus-mq-connector-0.3.5a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:25:43.724092 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:25:43.724092 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-25 23:25:43.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-25 23:25:43.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:25:43.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-25 23:25:43.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-25 23:25:43.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:25:43.724092 neon-messagebus-mq-connector-0.3.5a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:22:35.307256 neon-messagebus-mq-connector-0.3.5a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-27 20:22:29.000000 neon-messagebus-mq-connector-0.3.5a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-27 20:22:35.307256 neon-messagebus-mq-connector-0.3.5a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-27 20:22:29.000000 neon-messagebus-mq-connector-0.3.5a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:22:35.307256 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-27 20:22:29.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-27 20:22:29.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-27 20:22:29.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-07-27 20:22:29.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-27 20:22:29.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-27 20:22:29.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:22:35.307256 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-27 20:22:35.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-27 20:22:35.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:22:35.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-27 20:22:35.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 20:22:35.000000 neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:22:35.307256 neon-messagebus-mq-connector-0.3.5a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-27 20:22:29.000000 neon-messagebus-mq-connector-0.3.5a2/setup.py
```

### Comparing `neon-messagebus-mq-connector-0.3.5a1/LICENSE.md` & `neon-messagebus-mq-connector-0.3.5a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.5a1/PKG-INFO` & `neon-messagebus-mq-connector-0.3.5a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-messagebus-mq-connector
-Version: 0.3.5a1
+Version: 0.3.5a2
 Summary: MQ-Messagebus Connector Module
 Home-page: https://github.com/neongeckocom/neon-messagebus-mq-connector
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/__init__.py` & `neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/__main__.py` & `neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/config.py` & `neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/config.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/controller.py` & `neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -132,15 +132,18 @@
         else:
             body = {'msg_type': message.msg_type,
                     'data': message.data, 'context': message.context}
         LOG.debug(f'Received neon response body: {body}')
         if not body:
             LOG.warning('Something went wrong while formatting - received empty body')
         else:
-            routing_key = message.context.get("klat_data", {}).get("routing_key", 'neon_chat_api_response')
+            routing_key = message.context.get("mq",
+                                              {}).get("routing_key",
+                                                      'neon_chat_api_response')
+            LOG.debug(f"Got routing_key={routing_key}")
             self.send_message(request_data=body, queue=routing_key)
 
     def handle_neon_profile_update(self, message: Message):
         """
         Handles profile updates from Neon Core. Ensures routing_key is defined
         to avoid publishing private profile values to a shared queue
         :param message: Message containing the updated user profile
@@ -166,22 +169,22 @@
                      2) fetched message data;
         """
 
         if not message_templates:
             LOG.warning('No matching templates found, skipping template fetching')
             return '', msg_data
 
-        LOG.info('Initiating template validation')
+        LOG.debug('Initiating template validation')
         for message_template in message_templates:
             try:
                 msg_data = message_template(**msg_data).dict()
             except (ValueError, ValidationError) as err:
                 LOG.error(f'Failed to validate {msg_data} with template = {message_template.__name__}, exception={err}')
                 return str(err), msg_data
-        LOG.info('Template validation completed successfully')
+        LOG.debug('Template validation completed successfully')
         return '', msg_data
 
     @classmethod
     def validate_request(cls, msg_data: dict):
         """
             Fetches the relevant template models and validates provided message data iteratively through them
 
@@ -219,36 +222,44 @@
 
     def handle_user_message(self,
                             channel: pika.channel.Channel,
                             method: pika.spec.Basic.Return,
                             properties: pika.spec.BasicProperties,
                             body: bytes):
         """
-            Transfers requests from MQ API to Neon Message Bus API
+        Transfers requests from MQ API to Neon Message Bus API
 
-            :param channel: MQ channel object (pika.channel.Channel)
-            :param method: MQ return method (pika.spec.Basic.Return)
-            :param properties: MQ properties (pika.spec.BasicProperties)
-            :param body: request body (bytes)
+        :param channel: MQ channel object (pika.channel.Channel)
+        :param method: MQ return method (pika.spec.Basic.Return)
+        :param properties: MQ properties (pika.spec.BasicProperties)
+        :param body: request body (bytes)
 
         """
         if body and isinstance(body, bytes):
             dict_data = b64_to_dict(body)
             LOG.info(f'Received user message: {dict_data}')
-            dict_data["context"].setdefault("mq", dict(routing_key=dict_data.pop('routing_key', ''),
-                                                       message_id=dict_data.pop('message_id', ''),
-                                                       cid=dict_data.pop('cid', ''),
-                                                       sid=dict_data.pop('sid', '')))
+            mq_context = {"routing_key": dict_data.pop('routing_key', ''),
+                          "message_id": dict_data.pop('message_id', '')}
+            klat_context = {"cid": dict_data.pop('cid', ''),
+                            "sid": dict_data.pop('sid', '')}
+            # Klat Context for backwards-compat
+            dict_data["context"].setdefault("mq",
+                                            {**mq_context, **klat_context})
+            dict_data["context"].setdefault("klat_data", klat_context)
 
             validation_error, dict_data = self.validate_request(dict_data)
             if validation_error:
-                response = Message(msg_type="klat.error",
-                                   data=dict(error=validation_error,
-                                             message=dict_data))
-                response.context.setdefault('klat_data', {})['routing_key'] = 'neon_chat_api_error'
+                LOG.error(f"Validation failed with: {validation_error}")
+                # Don't deserialize since this Message may be malformed
+                context = dict_data.pop("context")
+                response = Message("klat.error", {"error": validation_error,
+                                                  "data": dict_data},
+                                   context)
+                response.context['klat_data'].setdefault('routing_key',
+                                                         'neon_chat_api_error')
                 self.handle_neon_message(response)
             else:
                 # dict_data["context"].setdefault('ident', f"{dict_data['msg_type']}.response")
                 message = Message(**dict_data)
                 is_context_valid = self.validate_message_context(message)
                 if is_context_valid:
                     self.bus.emit(message)
@@ -257,28 +268,30 @@
         else:
             channel.basic_nack()
             raise TypeError(f'Invalid body received, expected: bytes string;'
                             f' got: {type(body)}')
 
     def format_response(self, response_type: NeonResponseTypes, message: Message) -> dict:
         """
-            Formats received response by Neon API based on type
+        Formats received response by Neon API based on type
 
-            :param response_type: response type from NeonResponseTypes Enum
-            :param message: Neon MessageBus Message object
+        :param response_type: response type from NeonResponseTypes Enum
+        :param message: Neon MessageBus Message object
 
-            :returns formatted response dict
+        :returns formatted response dict
         """
         msg_error = message.data.get('error')
         if msg_error:
-            LOG.error(f'Failed to fetch data for context={message.context} - {msg_error}')
+            LOG.error(f'Failed to fetch data for context={message.context} - '
+                      f'{msg_error}')
             return {}
         timeout = self.response_timeouts.get(response_type, 30)
         if int(time.time()) - message.context.get('created_on', 0) > timeout:
-            LOG.warning(f'Message = {message} received timeout on {response_type} (>{timeout} seconds)')
+            LOG.warning(f'Message = {message} received timeout on '
+                        f'{response_type} (>{timeout} seconds)')
             response_data = {}
         else:
             if response_type == NeonResponseTypes.TTS:
                 lang = list(message.data)[0]
                 gender = message.data[lang].get('genders', ['female'])[0]
                 audio_data_b64 = message.data[lang]['audio'][gender]
 
@@ -290,19 +303,21 @@
                 }
             elif response_type == NeonResponseTypes.STT:
                 transcripts = message.data.get('transcripts', [''])
                 if transcripts and transcripts[0]:
                     LOG.info(f'transcript candidates received - {transcripts}')
                     response_data = {
                         'transcript': transcripts[0],
-                        'other_transcripts': [transcript for transcript in transcripts if transcript != transcripts[0]],
+                        'other_transcripts': [transcript for transcript in
+                                              transcripts if
+                                              transcript != transcripts[0]],
                         'lang': message.context.get('lang', 'en-us'),
                         'context': message.context
                     }
                 else:
                     LOG.error('No transcripts received')
                     response_data = {}
             else:
-                LOG.warning(f'Failed to response response type -> {response_type}')
+                LOG.warning(f'Failed to response response type -> '
+                            f'{response_type}')
                 response_data = {}
-            # LOG.debug(f'Formatted {response_type} response data = {response_data}')
         return response_data
```

### Comparing `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/enums.py` & `neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/enums.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/messages.py` & `neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector/messages.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/PKG-INFO` & `neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-messagebus-mq-connector
-Version: 0.3.5a1
+Version: 0.3.5a2
 Summary: MQ-Messagebus Connector Module
 Home-page: https://github.com/neongeckocom/neon-messagebus-mq-connector
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/SOURCES.txt` & `neon-messagebus-mq-connector-0.3.5a2/neon_messagebus_mq_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.5a1/setup.py` & `neon-messagebus-mq-connector-0.3.5a2/setup.py`

 * *Files identical despite different names*

