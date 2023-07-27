# Comparing `tmp/pih-1.47201.tar.gz` & `tmp/pih-1.47202.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47201.tar", last modified: Thu Jul 27 12:44:31 2023, max compression
+gzip compressed data, was "pih-1.47202.tar", last modified: Thu Jul 27 14:09:52 2023, max compression
```

## Comparing `pih-1.47201.tar` & `pih-1.47202.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 12:44:30.986915 pih-1.47201/
--rw-rw-rw-   0        0        0      261 2023-07-27 12:44:32.068396 pih-1.47201/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 12:44:31.771566 pih-1.47201/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47201/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47201/pih/collection.py
--rw-rw-rw-   0        0        0    61082 2023-07-27 07:03:42.000000 pih-1.47201/pih/console_api.py
--rw-rw-rw-   0        0        0   110191 2023-07-27 06:39:11.000000 pih-1.47201/pih/const.py
--rw-rw-rw-   0        0        0   309358 2023-07-27 07:23:27.000000 pih-1.47201/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-17 14:57:37.000000 pih-1.47201/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47201/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47201/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47201/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47201/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47201/pih/service_example.py
--rw-rw-rw-   0        0        0    38109 2023-07-26 00:20:00.000000 pih-1.47201/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47201/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-27 12:44:32.021521 pih-1.47201/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-27 12:44:29.000000 pih-1.47201/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-27 12:44:30.000000 pih-1.47201/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 12:44:29.000000 pih-1.47201/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-27 12:44:30.000000 pih-1.47201/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-27 12:44:30.000000 pih-1.47201/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-07-14 01:37:00.000000 pih-1.47201/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-27 12:44:32.084019 pih-1.47201/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 14:09:52.711517 pih-1.47202/
+-rw-rw-rw-   0        0        0      261 2023-07-27 14:09:52.711517 pih-1.47202/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 14:09:52.367803 pih-1.47202/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47202/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47202/pih/collection.py
+-rw-rw-rw-   0        0        0    61082 2023-07-27 07:03:42.000000 pih-1.47202/pih/console_api.py
+-rw-rw-rw-   0        0        0   110191 2023-07-27 06:39:11.000000 pih-1.47202/pih/const.py
+-rw-rw-rw-   0        0        0   309543 2023-07-27 14:09:25.000000 pih-1.47202/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-17 14:57:37.000000 pih-1.47202/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47202/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47202/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47202/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47202/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47202/pih/service_example.py
+-rw-rw-rw-   0        0        0    38109 2023-07-26 00:20:00.000000 pih-1.47202/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47202/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:09:52.695889 pih-1.47202/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-27 14:09:48.000000 pih-1.47202/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-27 14:09:49.000000 pih-1.47202/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 14:09:48.000000 pih-1.47202/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-27 14:09:48.000000 pih-1.47202/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-27 14:09:49.000000 pih-1.47202/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47202/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-27 14:09:52.727141 pih-1.47202/setup.cfg
```

### Comparing `pih-1.47201/pih/collection.py` & `pih-1.47202/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih/console_api.py` & `pih-1.47202/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih/const.py` & `pih-1.47202/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih/pih.py` & `pih-1.47202/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1628,15 +1628,15 @@
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
         @staticmethod
         def local() -> str:
-            return "1.47201"
+            return "1.47202"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -2767,19 +2767,21 @@
                     for service_command_item in description.commands:
                         service_command_item: ServiceCommands = service_command_item
                         PIH.SERVICE.command_map[service_command_item.name] = description
             return PIH.SERVICE.command_map[value.name] if value.name in PIH.SERVICE.command_map else None
 
         @staticmethod
         def get_host(role_or_information: ServiceRoles | ServiceInformationBase) -> str:
+            def add_donain(value: str) -> str:
+                return j((value, AD.DOMAIN), ".")
             information: ServiceInformationBase | None = ServiceRoles.description(role_or_information)
             if isinstance(information, ServiceDescription):
                 if not DataTool.is_empty(information.port):
-                    return information.host
-            return (PIH.SERVICE.get_information(role_or_information) or ServiceInformationBase()).host or information.host
+                    return add_donain(information.host)
+            return add_donain((PIH.SERVICE.get_information(role_or_information) or ServiceInformationBase()).host or information.host)
 
         @staticmethod
         def get_port(role_or_information: ServiceRoles | ServiceInformationBase) -> int | None:
             information: ServiceInformationBase | None = ServiceRoles.description(role_or_information)
             if isinstance(information, ServiceDescription):
                 if not DataTool.is_empty(information.port):
                     return information.port
@@ -4756,19 +4758,20 @@
 
         executor = ThreadPoolExecutor(max_workers=1)
 
         @staticmethod
         def send(value: str, channel: LogMessageChannels = LogMessageChannels.DEFAULT, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
             level = level or LogMessageFlags.DEFAULT
             def internal_send_message(message: str, channel_name: str, level_value: int) -> None:
-                try:
-                    PIH.SERVICE.call_command(ServiceCommands.send_log_message,
-                            (message, channel_name, level_value))
-                except Error as error:
-                    PIH.output.error("Log send error")
+                with PIH.ERROR.detect():
+                    try:
+                        PIH.SERVICE.call_command(ServiceCommands.send_log_message,
+                                (message, channel_name, level_value))
+                    except Error as error:
+                        PIH.output.error("Log send error")
             PIH.LOG.executor.submit(internal_send_message, value,
                                         channel.name, DataTool.as_bitmask_value(level))
             return value
 
         @staticmethod
         def debug_bot(message: str, level: int | tuple[Enum] | Enum | list[Enum] | list[int] | None = None) -> str:
             return PIH.LOG.send(message, LogMessageChannels.DEBUG_BOT, level)
```

### Comparing `pih-1.47201/pih/rpc.py` & `pih-1.47202/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih/rpcCommandCall_pb2.py` & `pih-1.47202/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47202/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih/rpc_collection.py` & `pih-1.47202/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih/rpc_const.py` & `pih-1.47202/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih/service_example.py` & `pih-1.47202/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih/tools.py` & `pih-1.47202/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih/widgets.py` & `pih-1.47202/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47201/pih_setup.py` & `pih-1.47202/pih_setup.py`

 * *Files identical despite different names*

