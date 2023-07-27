# Comparing `tmp/sdss_clu-2.1.2.tar.gz` & `tmp/sdss_clu-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_clu-2.1.2.tar", max compression
+gzip compressed data, was "sdss_clu-2.1.3.tar", max compression
```

## Comparing `sdss_clu-2.1.2.tar` & `sdss_clu-2.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1504 2023-07-20 15:34:14.327438 sdss_clu-2.1.2/LICENSE.md
--rw-r--r--   0        0        0     5049 2023-07-20 15:34:14.408466 sdss_clu-2.1.2/README.rst
--rw-r--r--   0        0        0     2774 2023-07-20 15:34:17.207379 sdss_clu-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      889 2023-07-20 15:34:17.328344 sdss_clu-2.1.2/python/clu/__init__.py
--rwxr-xr-x   0        0        0     9086 2023-07-20 15:34:17.449005 sdss_clu-2.1.2/python/clu/__main__.py
--rw-r--r--   0        0        0    13556 2023-07-20 15:34:17.569279 sdss_clu-2.1.2/python/clu/actor.py
--rw-r--r--   0        0        0    19832 2023-07-20 15:34:17.609935 sdss_clu-2.1.2/python/clu/base.py
--rw-r--r--   0        0        0    14706 2023-07-20 15:34:17.690889 sdss_clu-2.1.2/python/clu/client.py
--rw-r--r--   0        0        0    20069 2023-07-20 15:34:17.731289 sdss_clu-2.1.2/python/clu/command.py
--rw-r--r--   0        0        0     4135 2023-07-20 15:34:17.851501 sdss_clu-2.1.2/python/clu/device.py
--rw-r--r--   0        0        0     1347 2023-07-20 15:34:17.932576 sdss_clu-2.1.2/python/clu/exceptions.py
--rw-r--r--   0        0        0       41 2023-07-20 15:34:17.973459 sdss_clu-2.1.2/python/clu/legacy/__init__.py
--rw-r--r--   0        0        0    17892 2023-07-20 15:34:18.054967 sdss_clu-2.1.2/python/clu/legacy/actor.py
--rw-r--r--   0        0        0    13538 2023-07-20 15:34:18.096028 sdss_clu-2.1.2/python/clu/legacy/tron.py
--rw-r--r--   0        0        0        0 2023-07-20 15:34:18.177534 sdss_clu-2.1.2/python/clu/legacy/types/__init__.py
--rw-r--r--   0        0        0    15014 2023-07-20 15:34:18.177887 sdss_clu-2.1.2/python/clu/legacy/types/html.py
--rw-r--r--   0        0        0    17888 2023-07-20 15:34:18.218575 sdss_clu-2.1.2/python/clu/legacy/types/keys.py
--rw-r--r--   0        0        0    17508 2023-07-20 15:34:18.299383 sdss_clu-2.1.2/python/clu/legacy/types/messages.py
--rw-r--r--   0        0        0     9489 2023-07-20 15:34:18.423132 sdss_clu-2.1.2/python/clu/legacy/types/parser.py
--rwxr-xr-x   0        0        0      104 2023-07-20 15:34:18.464332 sdss_clu-2.1.2/python/clu/legacy/types/ply/__init__.py
--rwxr-xr-x   0        0        0    38405 2023-07-20 15:34:18.546530 sdss_clu-2.1.2/python/clu/legacy/types/ply/cpp.py
--rwxr-xr-x   0        0        0     2877 2023-07-20 15:34:18.671963 sdss_clu-2.1.2/python/clu/legacy/types/ply/ctokens.py
--rwxr-xr-x   0        0        0    45219 2023-07-20 15:34:18.795903 sdss_clu-2.1.2/python/clu/legacy/types/ply/lex.py
--rwxr-xr-x   0        0        0   140885 2023-07-20 15:34:18.837071 sdss_clu-2.1.2/python/clu/legacy/types/ply/yacc.py
--rwxr-xr-x   0        0        0     2314 2023-07-20 15:34:18.917938 sdss_clu-2.1.2/python/clu/legacy/types/ply/ygen.py
--rw-r--r--   0        0        0     5487 2023-07-20 15:34:18.958843 sdss_clu-2.1.2/python/clu/legacy/types/pvt.py
--rw-r--r--   0        0        0    19685 2023-07-20 15:34:19.040751 sdss_clu-2.1.2/python/clu/legacy/types/types.py
--rw-r--r--   0        0        0    11789 2023-07-20 15:34:19.081647 sdss_clu-2.1.2/python/clu/model.py
--rw-r--r--   0        0        0      309 2023-07-20 15:34:19.163983 sdss_clu-2.1.2/python/clu/parsers/__init__.py
--rw-r--r--   0        0        0    20428 2023-07-20 15:34:19.204399 sdss_clu-2.1.2/python/clu/parsers/click.py
--rw-r--r--   0        0        0     2685 2023-07-20 15:34:19.287197 sdss_clu-2.1.2/python/clu/parsers/json.py
--rw-r--r--   0        0        0    19724 2023-07-20 15:34:19.328753 sdss_clu-2.1.2/python/clu/protocol.py
--rw-r--r--   0        0        0     2805 2023-07-20 15:34:19.411667 sdss_clu-2.1.2/python/clu/store.py
--rw-r--r--   0        0        0     7820 2023-07-20 15:34:19.453190 sdss_clu-2.1.2/python/clu/testing.py
--rw-r--r--   0        0        0    16901 2023-07-20 15:34:19.535400 sdss_clu-2.1.2/python/clu/tools.py
--rw-r--r--   0        0        0     3648 2023-07-20 15:34:19.576545 sdss_clu-2.1.2/python/clu/websocket.py
--rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 sdss_clu-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-27 15:48:12.702001 sdss_clu-2.1.3/LICENSE.md
+-rw-r--r--   0        0        0     5049 2023-07-27 15:48:12.702338 sdss_clu-2.1.3/README.rst
+-rw-r--r--   0        0        0     2774 2023-07-27 15:48:12.717709 sdss_clu-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0      889 2023-07-27 15:48:12.718149 sdss_clu-2.1.3/python/clu/__init__.py
+-rwxr-xr-x   0        0        0     9086 2023-07-27 15:48:12.718542 sdss_clu-2.1.3/python/clu/__main__.py
+-rw-r--r--   0        0        0    14246 2023-07-27 15:48:12.718884 sdss_clu-2.1.3/python/clu/actor.py
+-rw-r--r--   0        0        0    20523 2023-07-27 15:48:12.719271 sdss_clu-2.1.3/python/clu/base.py
+-rw-r--r--   0        0        0    14706 2023-07-27 15:48:12.719668 sdss_clu-2.1.3/python/clu/client.py
+-rw-r--r--   0        0        0    20416 2023-07-27 15:48:12.720053 sdss_clu-2.1.3/python/clu/command.py
+-rw-r--r--   0        0        0     4135 2023-07-27 15:48:12.720449 sdss_clu-2.1.3/python/clu/device.py
+-rw-r--r--   0        0        0     1347 2023-07-27 15:48:12.720728 sdss_clu-2.1.3/python/clu/exceptions.py
+-rw-r--r--   0        0        0       41 2023-07-27 15:48:12.721070 sdss_clu-2.1.3/python/clu/legacy/__init__.py
+-rw-r--r--   0        0        0    18698 2023-07-27 15:48:12.721435 sdss_clu-2.1.3/python/clu/legacy/actor.py
+-rw-r--r--   0        0        0    13538 2023-07-27 15:48:12.721797 sdss_clu-2.1.3/python/clu/legacy/tron.py
+-rw-r--r--   0        0        0        0 2023-07-27 15:48:12.722054 sdss_clu-2.1.3/python/clu/legacy/types/__init__.py
+-rw-r--r--   0        0        0    15014 2023-07-27 15:48:12.722329 sdss_clu-2.1.3/python/clu/legacy/types/html.py
+-rw-r--r--   0        0        0    17888 2023-07-27 15:48:12.722735 sdss_clu-2.1.3/python/clu/legacy/types/keys.py
+-rw-r--r--   0        0        0    17508 2023-07-27 15:48:12.723148 sdss_clu-2.1.3/python/clu/legacy/types/messages.py
+-rw-r--r--   0        0        0     9489 2023-07-27 15:48:12.723473 sdss_clu-2.1.3/python/clu/legacy/types/parser.py
+-rwxr-xr-x   0        0        0      104 2023-07-27 15:48:12.723810 sdss_clu-2.1.3/python/clu/legacy/types/ply/__init__.py
+-rwxr-xr-x   0        0        0    38405 2023-07-27 15:48:12.724233 sdss_clu-2.1.3/python/clu/legacy/types/ply/cpp.py
+-rwxr-xr-x   0        0        0     2877 2023-07-27 15:48:12.724544 sdss_clu-2.1.3/python/clu/legacy/types/ply/ctokens.py
+-rwxr-xr-x   0        0        0    45219 2023-07-27 15:48:12.724983 sdss_clu-2.1.3/python/clu/legacy/types/ply/lex.py
+-rwxr-xr-x   0        0        0   140885 2023-07-27 15:48:12.725887 sdss_clu-2.1.3/python/clu/legacy/types/ply/yacc.py
+-rwxr-xr-x   0        0        0     2314 2023-07-27 15:48:12.726247 sdss_clu-2.1.3/python/clu/legacy/types/ply/ygen.py
+-rw-r--r--   0        0        0     5487 2023-07-27 15:48:12.726614 sdss_clu-2.1.3/python/clu/legacy/types/pvt.py
+-rw-r--r--   0        0        0    19685 2023-07-27 15:48:12.727001 sdss_clu-2.1.3/python/clu/legacy/types/types.py
+-rw-r--r--   0        0        0    11789 2023-07-27 15:48:12.727403 sdss_clu-2.1.3/python/clu/model.py
+-rw-r--r--   0        0        0      309 2023-07-27 15:48:12.727838 sdss_clu-2.1.3/python/clu/parsers/__init__.py
+-rw-r--r--   0        0        0    20583 2023-07-27 15:48:12.729163 sdss_clu-2.1.3/python/clu/parsers/click.py
+-rw-r--r--   0        0        0     2685 2023-07-27 15:48:12.729516 sdss_clu-2.1.3/python/clu/parsers/json.py
+-rw-r--r--   0        0        0    19724 2023-07-27 15:48:12.729902 sdss_clu-2.1.3/python/clu/protocol.py
+-rw-r--r--   0        0        0     2805 2023-07-27 15:48:12.730232 sdss_clu-2.1.3/python/clu/store.py
+-rw-r--r--   0        0        0     7820 2023-07-27 15:48:12.730622 sdss_clu-2.1.3/python/clu/testing.py
+-rw-r--r--   0        0        0    16945 2023-07-27 15:48:12.731058 sdss_clu-2.1.3/python/clu/tools.py
+-rw-r--r--   0        0        0     3648 2023-07-27 15:48:12.731387 sdss_clu-2.1.3/python/clu/websocket.py
+-rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 sdss_clu-2.1.3/PKG-INFO
```

### Comparing `sdss_clu-2.1.2/LICENSE.md` & `sdss_clu-2.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/README.rst` & `sdss_clu-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/pyproject.toml` & `sdss_clu-2.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-clu"
-version = "2.1.2"
+version = "2.1.3"
 description = "A new protocol for SDSS actors."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/sdss/clu"
 repository = "https://github.com/sdss/clu"
 documentation = "https://clu.readthedocs.io/en/latest/"
```

### Comparing `sdss_clu-2.1.2/python/clu/__init__.py` & `sdss_clu-2.1.3/python/clu/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/__main__.py` & `sdss_clu-2.1.3/python/clu/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/actor.py` & `sdss_clu-2.1.3/python/clu/actor.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,16 +125,27 @@
                     f"{command_string!r}. {ee!r}"
                 },
             )
             return
 
         return self.parse_command(command)
 
-    async def _write_internal(self, reply: Reply):
-        """Writes a message to user(s)."""
+    async def _write_internal(self, reply: Reply, write_to_log: bool = True):
+        """Writes a message to user(s).
+
+        Parameters
+        ----------
+        reply
+            The reply object to output to users.
+        write_to_log
+            Whether to write the reply to the log. Defaults to yes but
+            it may be useful to prevent large repetitive replies cluttering
+            the log.
+
+        """
 
         assert self.connection
 
         message = reply.message
         message_json = json.dumps(message)
 
         command = reply.command
@@ -162,15 +173,15 @@
                 headers=headers,
                 correlation_id=str(command_id) if command_id is not None else None,
                 timestamp=datetime.utcnow(),
             ),
             routing_key=routing_key,
         )
 
-        if self.log:
+        if self.log and write_to_log:
             log_reply(self.log, reply.message_code, message_json)
 
 
 class AMQPActor(ClickParser, AMQPBaseActor):
     """An `AMQP actor <.AMQPBaseActor>` that uses a `click parser <.ClickParser>`."""
 
     pass
@@ -357,16 +368,27 @@
         ``multiline`` command.
 
         See `~.BaseActor.write` for details on the allowed parameters.
         """
 
         BaseActor.write(self, *args, **kwargs)
 
-    def _write_internal(self, reply: Reply):
-        """Write a reply to the users."""
+    def _write_internal(self, reply: Reply, write_to_log: bool = True):
+        """Write a reply to the users.
+
+        Parameters
+        ----------
+        reply
+            The reply object to output to users.
+        write_to_log
+            Whether to write the reply to the log. Defaults to yes but
+            it may be useful to prevent large repetitive replies cluttering
+            the log.
+
+        """
 
         def send_to_transport(transport, message):
             if getattr(transport, "multiline", False):
                 message_json = json.dumps(message, sort_keys=False, indent=4) + "\n"
             else:
                 message_json = json.dumps(message, sort_keys=False) + "\n"
             transport.write(message_json.encode())
@@ -396,15 +418,15 @@
             for transport in self.transports.values():
                 send_to_transport(transport, message_full)
         else:
             send_to_transport(transport, message_full)
 
         message_json = json.dumps(message_full, sort_keys=False) + "\n"
 
-        if self.log:
+        if self.log and write_to_log:
             log_reply(self.log, reply.message_code, message_json.strip())
 
 
 class JSONActor(ClickParser, TCPBaseActor):
     """An implementation of `.TCPBaseActor` that uses a Click command parser."""
 
     def __init__(self, *args, **kwargs):
```

### Comparing `sdss_clu-2.1.2/python/clu/base.py` & `sdss_clu-2.1.3/python/clu/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -428,33 +428,45 @@
 
     @abc.abstractmethod
     def parse_command(self, command: BaseCommand):
         """Parses and executes a `.Command`. Must be overridden."""
         pass
 
     @abc.abstractmethod
-    def _write_internal(self, reply: Reply):
+    def _write_internal(self, reply: Reply, write_to_log: bool = True):
         """Internally handle the reply and output it to the users.
 
         Must handle converting the general `.Reply` to the specific format of the
         actor transport. Must also handle logging the reply.
+
+        Parameters
+        ----------
+        reply
+            The reply object to output to users.
+        write_to_log
+            Whether to write the reply to the log. Defaults to yes but
+            it may be useful to prevent large repetitive replies cluttering
+            the log.
+
         """
+
         pass
 
     def write(
         self,
         message_code: MessageCode | str = MessageCode.INFO,
         message: Optional[Dict[str, Any] | str] = None,
         command: Optional[BaseCommand] = None,
         broadcast: bool = False,
         validate: bool | None = None,
         expand_exceptions: bool = True,
         silent: bool = False,
         internal: bool = False,
         emit: bool = True,
+        write_to_log: bool = True,
         **kwargs,
     ) -> Reply:
         """Writes a message to user(s).
 
         The reply to the users will be formatted by the actor class into message
         specific to the communication channel. Additional keywords passed to this
         method will be used to complete the message (as long as they don't overlap
@@ -512,14 +524,18 @@
             reply with verbose information that can be skipped from CLI or logs.
         emit
             Whether to call the actor internal write method. Should be `True` but
             it's sometimes useful to call `.write` with ``emit=False`` when
             one is overriding the method and wants to control when to call the
             internal method. In that case, a `.Reply` object is returned but nothing
             is output to the users.
+        write_to_log
+            Whether to write the reply to the log. Defaults to yes but
+            it may be useful to prevent large repetitive replies cluttering
+            the log.
         kwargs
             Keyword arguments that will used to update the message.
         """
 
         message_code = MessageCode(message_code)
 
         if isinstance(message, str):
@@ -573,17 +589,22 @@
                 reply.validated = True
 
         if command:
             command.replies.append(reply)
 
         if emit and silent is False:
             if asyncio.iscoroutinefunction(self._write_internal):
-                asyncio.create_task(self._write_internal(reply))  # type: ignore
+                asyncio.create_task(
+                    self._write_internal(
+                        reply,
+                        write_to_log=write_to_log,
+                    )
+                )
             else:
-                self._write_internal(reply)
+                self._write_internal(reply, write_to_log=write_to_log)
 
         if self.store is not None:
             self.store.add_reply(reply)
 
         return reply
 
     def invoke_mock_command(self, command_str, command_id=0) -> Command:
```

### Comparing `sdss_clu-2.1.2/python/clu/client.py` & `sdss_clu-2.1.3/python/clu/client.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/command.py` & `sdss_clu-2.1.3/python/clu/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,14 +115,17 @@
         A silent command will call the actor ``write`` method with ``silent=True``,
         which will update the internal model and record all the output replies but
         will not write them to the users.
     internal
         A silent command will call the actor ``write`` method with ``internal=True``,
         which will instruct the actor to add the internal flag to the header of the
         reply.
+    write_to_log
+        Whether to write replies to the log. Defaults to yes but it may be useful
+        to prevent large repetitive replies cluttering the log.
     time_limit
         Time out the command if it has been running for this long.
     loop
         The event loop.
 
     """
 
@@ -135,28 +138,30 @@
         parent: Optional[BaseCommand[Actor_co, Future_co]] = None,
         reply_callback: Optional[Callable[[Any], None]] = None,
         status_callback: Optional[Callable[[CommandStatus], Any]] = None,
         call_now: bool = False,
         default_keyword: str = "text",
         silent: bool = False,
         internal: bool = False,
+        write_to_log: bool = True,
         time_limit: float | None = None,
         loop: Optional[asyncio.AbstractEventLoop] = None,
     ):
         self.commander_id = commander_id
         self.consumer_id = consumer_id
         self.command_id = command_id
 
         # Casting here so that we can type Command[SomeActor] and not have to
         # assert command.actor every time.
         self.actor = cast(Actor_co, actor)
         self.parent = parent
 
         self.silent = silent
         self.internal = internal
+        self.write_to_log = write_to_log
 
         self._reply_callback = reply_callback
 
         self.default_keyword = default_keyword
         self.loop = loop or asyncio.get_event_loop()
 
         #: The click context, if the click parser is used.
@@ -371,22 +376,24 @@
                 message_code = clu.base.MessageCode.INFO
                 if kwargs == {} and (message == {} or not message):
                     return
             elif message_code == clu.base.MessageCode.FAILED:
                 message_code = clu.base.MessageCode.ERROR
 
         internal = kwargs.pop("internal", self.internal)
+        write_to_log = kwargs.pop("write_to_log", self.write_to_log)
 
         self.actor.write(
             message_code,
             message=message,
             command=command,
             broadcast=broadcast,
             silent=self.silent,
             internal=internal,
+            write_to_log=write_to_log,
             **kwargs,
         )
 
     def send_command(
         self,
         target: str,
         command_string: str,
```

### Comparing `sdss_clu-2.1.2/python/clu/device.py` & `sdss_clu-2.1.3/python/clu/device.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/exceptions.py` & `sdss_clu-2.1.3/python/clu/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/actor.py` & `sdss_clu-2.1.3/python/clu/legacy/actor.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,15 +236,15 @@
         """Assigns userID to new client connection."""
 
         if transport.is_closing():
             if hasattr(transport, "user_id"):
                 self.log.debug(f"user {transport.user_id} disconnected.")
                 return self.transports.pop(transport.user_id)
 
-        curr_ids = set(self.transports.keys())
+        curr_ids: set[int] = set(self.transports.keys())
         user_id = 1 if len(curr_ids) == 0 else max(curr_ids) + 1
 
         transport.user_id = user_id
 
         self.transports[user_id] = transport
 
         # report user information and additional info
@@ -432,14 +432,15 @@
         message: Optional[Dict[str, Any]] = None,
         command: Optional[Command] = None,
         user_id: int = 0,
         command_id: int = 0,
         concatenate: bool = True,
         broadcast: bool = False,
         validate: bool = True,
+        write_to_log: bool = True,
         **kwargs,
     ):
         """Writes a message to user(s).
 
         Parameters
         ----------
         message_code
@@ -461,14 +462,18 @@
             reply with the keyword-values joined with semicolons. Otherwise
             each keyword will be output as a different message.
         broadcast
             Whether to broadcast the reply. Equivalent to ``user_id=0``.
         validate
             Validate the reply against the actor model. This is ignored if the actor
             was not started with knowledge of its own schema.
+        write_to_log
+            Whether to write the reply to the log. Defaults to yes but
+            it may be useful to prevent large repetitive replies cluttering
+            the log.
         kwargs
             Keyword arguments that will be added to the message. If a keyword
             is both in ``message`` and in ``kwargs``, the value in ``kwargs``
             supersedes ``message``.
         """
 
         message_code = MessageCode(message_code)
@@ -487,18 +492,41 @@
 
         if kwargs.get("silent", False) is False:
             self._write_internal(
                 reply,
                 user_id=user_id,
                 command_id=command_id,
                 concatenate=concatenate,
+                write_to_log=write_to_log,
             )
 
-    def _write_internal(self, reply: Reply, user_id=0, command_id=0, concatenate=True):
-        """Writes reply to users."""
+    def _write_internal(
+        self,
+        reply: Reply,
+        user_id=0,
+        command_id=0,
+        concatenate=True,
+        write_to_log: bool = True,
+    ):
+        """Writes reply to users.
+
+        Parameters
+        ----------
+        reply
+            The reply object to output to users.
+        user_id
+            The user to which we are replying.
+        command_id
+            The command emitting this message.
+        write_to_log
+            Whether to write the reply to the log. Defaults to yes but
+            it may be useful to prevent large repetitive replies cluttering
+            the log.
+
+        """
 
         command = cast(Command, reply.command)
         message = reply.message
 
         # For a reply, the commander ID is the user assigned to the transport
         # that issues this command.
         transport = command.transport if command else None
@@ -542,15 +570,15 @@
                 for transport in self.transports.values():
                     transport.write(msg)
             else:
                 global_transport = self.transports.get(transport.user_id, None)
                 if global_transport is not None and global_transport == transport:
                     transport.write(msg)
 
-            if self.log:
+            if self.log and write_to_log:
                 log_reply(self.log, reply.message_code, full_msg_str)
 
 
 class LegacyActor(ClickParser, BaseLegacyActor):
     """A legacy actor that uses the `.ClickParser`."""
 
     def __init__(self, *args, **kwargs):
```

### Comparing `sdss_clu-2.1.2/python/clu/legacy/tron.py` & `sdss_clu-2.1.3/python/clu/legacy/tron.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/html.py` & `sdss_clu-2.1.3/python/clu/legacy/types/html.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/keys.py` & `sdss_clu-2.1.3/python/clu/legacy/types/keys.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/messages.py` & `sdss_clu-2.1.3/python/clu/legacy/types/messages.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/parser.py` & `sdss_clu-2.1.3/python/clu/legacy/types/parser.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/ply/cpp.py` & `sdss_clu-2.1.3/python/clu/legacy/types/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/ply/ctokens.py` & `sdss_clu-2.1.3/python/clu/legacy/types/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/ply/lex.py` & `sdss_clu-2.1.3/python/clu/legacy/types/ply/lex.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/ply/yacc.py` & `sdss_clu-2.1.3/python/clu/legacy/types/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/ply/ygen.py` & `sdss_clu-2.1.3/python/clu/legacy/types/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/pvt.py` & `sdss_clu-2.1.3/python/clu/legacy/types/pvt.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/legacy/types/types.py` & `sdss_clu-2.1.3/python/clu/legacy/types/types.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/model.py` & `sdss_clu-2.1.3/python/clu/model.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/parsers/click.py` & `sdss_clu-2.1.3/python/clu/parsers/click.py`

 * *Files 2% similar despite different names*

```diff
@@ -474,18 +474,18 @@
         match = re.match(r"^Usage: ([A-Za-z-_]+)", line)
         if match:
             line = line.replace(match.groups()[0], command_name)
 
         message.append(line)
 
     if isinstance(command.actor, (actor.AMQPActor, actor.JSONActor)):
-        return command.finish(help=message)
+        return command.finish(help=message, write_to_log=False)
     else:
         for line in message:
-            command.warning(help=line)
+            command.warning(help=line, write_to_log=False)
         return command.finish()
 
 
 @command_parser.command(internal=True)
 @click.argument("COMMAND-NAME", type=str, required=False)
 @click.pass_context
 def get_command_model(
@@ -506,17 +506,17 @@
         if not click_command:
             return command.fail(f"Cannot find command {command_name}.")
 
     model_str = command_to_json(click_command)
     model_dict = json.loads(model_str)
 
     if isinstance(command.actor, LegacyActor):
-        return command.finish(command_model=model_str)
+        return command.finish(command_model=model_str, write_to_log=False)
 
-    return command.finish(command_model=model_dict)
+    return command.finish(command_model=model_dict, write_to_log=False)
 
 
 @command_parser.command(name="keyword")
 @click.argument("KEYWORD", type=str, required=True)
 def keyword(command, *args, keyword):
     """Prints human-readable information about a keyword."""
 
@@ -528,17 +528,20 @@
         return command.fail(error=f"Keyword {keyword!r} is not part of the data model.")
 
     schema = model.schema["properties"][keyword]
 
     lines = json.dumps(schema, indent=2).splitlines()[1:]
     max_length = max([len(line) for line in lines])
 
-    command.info(text=f"{keyword} = {{".ljust(max_length, " "))
+    command.info(text=f"{keyword} = {{".ljust(max_length, " "), write_to_log=False)
     for line in lines:
-        command.info(text=line.replace('"', "").ljust(max_length, " "))
+        command.info(
+            text=line.replace('"', "").ljust(max_length, " "),
+            write_to_log=False,
+        )
 
     command.finish()
 
 
 T = TypeVar("T", bound=Command)
```

### Comparing `sdss_clu-2.1.2/python/clu/parsers/json.py` & `sdss_clu-2.1.3/python/clu/parsers/json.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/protocol.py` & `sdss_clu-2.1.3/python/clu/protocol.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/store.py` & `sdss_clu-2.1.3/python/clu/store.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/testing.py` & `sdss_clu-2.1.3/python/clu/testing.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/python/clu/tools.py` & `sdss_clu-2.1.3/python/clu/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,16 @@
         else:
             self.code = None
 
     @property
     def is_combination(self) -> bool:
         """Returns True if a flag is a combination."""
 
+        assert isinstance(self.value, int)
+
         if bin(self.value).count("1") > 1:
             return True
         return False
 
     @property
     def did_fail(self) -> bool:
         """Command failed or was cancelled."""
```

### Comparing `sdss_clu-2.1.2/python/clu/websocket.py` & `sdss_clu-2.1.3/python/clu/websocket.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.2/PKG-INFO` & `sdss_clu-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-clu
-Version: 2.1.2
+Version: 2.1.3
 Summary: A new protocol for SDSS actors.
 Home-page: https://github.com/sdss/clu
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
```

