# Comparing `tmp/sddp_discovery_protocol-1.3.0.tar.gz` & `tmp/sddp_discovery_protocol-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddp_discovery_protocol-1.3.0.tar", max compression
+gzip compressed data, was "sddp_discovery_protocol-1.5.0.tar", max compression
```

## Comparing `sddp_discovery_protocol-1.3.0.tar` & `sddp_discovery_protocol-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1075 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/LICENSE
--rw-r--r--   0        0        0    13789 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/README.md
--rw-r--r--   0        0        0     1353 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1812 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/__init__.py
--rwxr-xr-x   0        0        0    12686 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/__main__.py
--rwxr-xr-x   0        0        0    17332 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/client.py
--rw-r--r--   0        0        0      319 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/constants.py
--rw-r--r--   0        0        0      253 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/exceptions.py
--rw-r--r--   0        0        0     1466 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/internal_types.py
--rwxr-xr-x   0        0        0      269 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/pkg_logging.py
--rw-r--r--   0        0        0        0 2023-07-24 23:44:52.003127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/py.typed
--rwxr-xr-x   0        0        0    19088 2023-07-24 23:44:52.007127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/sddp_datagram.py
--rwxr-xr-x   0        0        0    20519 2023-07-24 23:44:52.007127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/sddp_socket.py
--rwxr-xr-x   0        0        0    17429 2023-07-24 23:44:52.007127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/server.py
--rwxr-xr-x   0        0        0     8360 2023-07-24 23:44:52.007127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/util.py
--rw-r--r--   0        0        0      454 2023-07-24 23:44:52.007127 sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/version.py
--rw-r--r--   0        0        0    14748 1970-01-01 00:00:00.000000 sddp_discovery_protocol-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-27 21:40:14.868158 sddp_discovery_protocol-1.5.0/LICENSE
+-rw-r--r--   0        0        0    13789 2023-07-27 21:40:14.868158 sddp_discovery_protocol-1.5.0/README.md
+-rw-r--r--   0        0        0     1391 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1812 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/__init__.py
+-rwxr-xr-x   0        0        0    12785 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/__main__.py
+-rwxr-xr-x   0        0        0    17271 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/client.py
+-rw-r--r--   0        0        0      319 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/constants.py
+-rw-r--r--   0        0        0      253 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/exceptions.py
+-rw-r--r--   0        0        0     1466 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/internal_types.py
+-rwxr-xr-x   0        0        0      269 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/pkg_logging.py
+-rw-r--r--   0        0        0        0 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/py.typed
+-rwxr-xr-x   0        0        0    19088 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/sddp_datagram.py
+-rwxr-xr-x   0        0        0    20616 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/sddp_socket.py
+-rwxr-xr-x   0        0        0    17564 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/server.py
+-rwxr-xr-x   0        0        0     8364 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/util.py
+-rw-r--r--   0        0        0      454 2023-07-27 21:40:14.872158 sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/version.py
+-rw-r--r--   0        0        0    14748 1970-01-01 00:00:00.000000 sddp_discovery_protocol-1.5.0/PKG-INFO
```

### Comparing `sddp_discovery_protocol-1.3.0/LICENSE` & `sddp_discovery_protocol-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.3.0/README.md` & `sddp_discovery_protocol-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.3.0/pyproject.toml` & `sddp_discovery_protocol-1.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sddp-discovery-protocol"
-version = "1.3.0"
+version = "1.5.0"
 description = "Implementation of Control4's Simple Device Discovery Protocol (SDDP)"
 authors = [ "Sam McKelvie <dev@mckelvie.org>" ]
 license = "MIT"
 keywords = [ "Control4", "SDDP", "SSDP", "UPnP", "protocol", "multicast", "UDP",
              "discovery", "network", "automation", "smart-home" ]
 readme = "README.md"
 homepage = "https://github.com/sammck/sddp-discovery-protocol"
@@ -17,15 +17,17 @@
 #jq = "^1.2.2"
 #colorama = "^0.4.4"
 typing-extensions = "^4.7.1"
 netifaces-plus = "^0.12.0"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "^0.931"
+
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.4.1"
 #dunamai = "^1.9.0"
 python-semantic-release = "^7.25.2"
 #pydoc-markdown = "^4.6.0"
 #doc2md = "^0.1.0"
 #Sphinx = "^4.4.0"
 #sphinx-markdown-builder = "^0.5.5"
 types-requests = "^2.31.0.2"
```

### Comparing `sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/__init__.py` & `sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/__main__.py` & `sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,30 +57,31 @@
 
     def __init__(self, argv: Optional[Sequence[str]]=None):
         self._argv = argv
 
     async def cmd_bare(self) -> int:
         print("A command is required", file=sys.stderr)
         return 1
-    
+
     def _parse_arg_headers(self, arg_headers: List[str]) -> CaseInsensitiveDict:
-        headers = CaseInsensitiveDict()
+        headers: CaseInsensitiveDict[Union[str, int]] = CaseInsensitiveDict()
         for header_assignment in arg_headers:
+            value: Union[str, int]
             name, value = header_assignment.split('=', 1)
             if name.lower() in [x.lower() for x in integer_sddp_headers]:
                 value = int(value)
             headers[name] = value
         return headers
-        
+
 
     async def cmd_server(self) -> int:
         async def notify_handler(info: SddpAdvertisementInfo) -> None:
             results: List[JsonableDict] = []
             datagram = info.datagram
-            header_dict: Dict[str, str] = dict(datagram.headers)
+            header_dict: Dict[str, Union[str, int, float]] = dict(datagram.headers)
             summary: JsonableDict = {
                 "sddp_version": info.sddp_version,
                 "src_addr": f"{info.src_addr[0]}:{info.src_addr[1]}",
                 "local_addr": f"{info.socket_binding.unicast_addr[0]}:{info.socket_binding.unicast_addr[1]}",
                 "headers": header_dict,
                 "monotonic_time": info.monotonic_time,
                 "utc_time": info.utc_time.isoformat(),
@@ -141,15 +142,15 @@
                     response_wait_time=response_wait_time,
                     max_responses=max_responses,
                     include_error_responses=include_error_responses,
                     filter_headers=filter_headers,
                 ) as search_request:
                 async for info in search_request.iter_responses():
                     datagram = info.datagram
-                    header_dict: Dict[str, str] = dict(datagram.headers)
+                    header_dict: Dict[str, Union[str, int, float]] = dict(datagram.headers)
                     summary: JsonableDict = {
                         "sddp_version": info.sddp_version,
                         "status_code": info.status_code,
                         "status": info.status,
                         "src_addr": f"{info.src_addr[0]}:{info.src_addr[1]}",
                         "local_addr": f"{info.socket_binding.unicast_addr[0]}:{info.socket_binding.unicast_addr[1]}",
                         "headers": header_dict,
```

### Comparing `sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/client.py` & `sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,37 +85,37 @@
         AsyncContextManager['SddpSearchRequest'],
         AsyncIterable[SddpResponseInfo]
       ):
     """An object that manages a single search request on an SddpClient and all of the received responses
        within an AsyncContextManager/AsyncInterable interface."""
 
     _response_statement_re = re.compile(r'^SDDP/(?P<version_major>[0-9]*)\.(?P<version_minor>[0-9]+) +(?P<status_code>[0-9]+) +(?P<status>.*[^ ]) *$')
-    
+
     sddp_client: SddpClient
     search_pattern: str
     include_error_responses: bool
-    
+
     dg_subscriber: SddpDatagramSubscriber
     response_wait_time: float
     max_responses: int
     end_time: float = 0.0
-    filter_headers: Optional[CaseInsensitiveDict[str]] = None
+    filter_headers: Optional[CaseInsensitiveDict[Union[str, int]]] = None
 
     def __init__(
             self,
             sddp_client: SddpClient,
             search_pattern: str="*",
             response_wait_time: Optional[float]=None,
             max_responses: int=0,
             include_error_responses: bool=False,
-            filter_headers: Optional[Mapping[str, str]]=None
+            filter_headers: Optional[Mapping[str, Union[str, int]]]=None
           ):
         """Create an async context manager/iterable that sends a multicast search request and returns the responses
         as they arrive.
-        
+
         Parameters:
             sddp_client:             The SddpClient instance to use for sending the search request and receiving responses.
             search_pattern:          The search pattern to use. Defaults to "*" (all devices).
             response_wait_time:      The amount of time (in seconds) to wait for responses to come in. Defaults to
                                         sddp_client.response_wait_time.
             max_responses:           The maximum number of responses to return. If 0 (the default), all responses received
                                         within response_wait_time will be returned.
@@ -173,15 +173,15 @@
                 break
             try:
                 resp_tuple = await asyncio.wait_for(self.dg_subscriber.receive(), remaining_time)
             except asyncio.TimeoutError:
                 break
             if resp_tuple is None:
                 break
-            socket_binding, addr, datagram = resp_tuple 
+            socket_binding, addr, datagram = resp_tuple
             m = self._response_statement_re.match(datagram.statement_line)
             if m:
                 version_major: Optional[int] = None
                 version_minor: Optional[int] = None
                 try:
                     version_major = int(m.group('version_major'))
                 except ValueError:
@@ -202,16 +202,16 @@
                         info = SddpResponseInfo(socket_binding, addr, datagram, f"{version_major}.{version_minor}", status_code, status)
                         logger.debug(f"Received SDDP response from {addr} on {socket_binding}: version={info.sddp_version}, status_code={status_code}, status={status}, headers={datagram.headers}")
                         if self.include_error_responses or status_code == 200:
                             if self.filter_headers is None or all(datagram.headers.get(key, None) == value for key, value in self.filter_headers.items()):
                                 n += 1
                                 yield info
 
-    async def __aiter__(self) -> AsyncIterator[SddpResponseInfo]:
-        return await self.iter_responses()
+    def __aiter__(self) -> AsyncIterator[SddpResponseInfo]:
+        return self.iter_responses()
 
 
 class SddpClient(SddpSocket, AsyncContextManager['SddpClient']):
     """
     An SDDP client that can:
 
       1. Send a discovery request to a multicast UDP address (typically 239.255.255.250:1902)
@@ -292,15 +292,15 @@
             response_wait_time: Optional[float]=None,
             max_responses: int=0,
             include_error_responses: bool=False,
             filter_headers: Optional[Mapping[str, str]]=None,
           ) -> SddpSearchRequest:
         """Create an async context manager/iterable that sends a multicast search request and returns the responses
            as they arrive.
-        
+
         Parameters:
             search_pattern:          The search pattern to use. Defaults to "*" (all devices).
             response_wait_time:      The amount of time (in seconds) to wait for responses to come in. Defaults to
                                         sddp_client.response_wait_time.
             max_responses:           The maximum number of responses to return. If 0 (the default), all responses received
                                         within response_wait_time will be returned.
             include_error_responses: If True, responses with a non-200 status code will be included in the results.
@@ -319,29 +319,29 @@
                 self,
                 search_pattern=search_pattern,
                 response_wait_time=response_wait_time,
                 max_responses=max_responses,
                 include_error_responses=include_error_responses,
                 filter_headers=filter_headers,
               )
-    
+
     async def simple_search(
             self,
             search_pattern: str="*",
             response_wait_time: Optional[float]=None,
             max_responses: int=0,
             include_error_responses: bool=False,
             filter_headers: Optional[Mapping[str, str]]=None,
           ) -> List[SddpResponseInfo]:
         """A simple search that creates a search request, waits for a fixed time for all responses to come in,
            and returns the responses. Does not allow for early termination of the search when
            a desired response is received.
-           
+
            Early out/incremental results can be obtained by using the search() method.
-           
+
         Parameters:
             sddp_client:             The SddpClient instance to use for sending the search request and receiving responses.
             search_pattern:          The search pattern to use. Defaults to "*" (all devices).
             response_wait_time:      The amount of time (in seconds) to wait for responses to come in. Defaults to
                                         sddp_client.response_wait_time.
             max_responses:           The maximum number of responses to return. If 0 (the default), all responses received
                                         within response_wait_time will be returned.
@@ -349,15 +349,14 @@
                                         Defaults to False.
             filter_headers:          A mapping of headers to values. If specified, only responses that have all of the
                                         specified headers with the specified values will be included in the results. Defaults
                                         to None.
         """
         results: List[SddpResponseInfo] = []
         async with self.search(
-                self,
                 search_pattern=search_pattern,
                 response_wait_time=response_wait_time,
                 max_responses=max_responses,
                 include_error_responses=include_error_responses,
                 filter_headers=filter_headers,
               ) as search_request:
             async for response in search_request:
```

### Comparing `sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/internal_types.py` & `sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/internal_types.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/sddp_datagram.py` & `sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/sddp_datagram.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/sddp_socket.py` & `sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/sddp_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     def protocol(self, protocol: _SddpSocketProtocol) -> None:
         if protocol != self._protocol:
             assert self._protocol is None
         self._protocol = protocol
 
     def sendto(self, datagram: SddpDatagram, addr: HostAndPort) -> None:
         logger.debug(f"Sending SddpDatagram via {self} to {addr}: {datagram}")
+        assert not self.transport is None
         self.transport.sendto(datagram.raw_data, addr)
 
     def __str__(self) -> str:
         return f"SddpSocketBinding({self.index}: {self.sockname})"
 
     def __repr__(self) -> str:
         return str(self)
@@ -131,14 +132,15 @@
 
     def __init__(self, socket_binding: SddpSocketBinding):
         self.socket_binding = socket_binding
         socket_binding.protocol = self
 
     @property
     def sddp_socket(self) -> SddpSocket:
+        assert self.socket_binding.sddp_socket is not None
         return self.socket_binding.sddp_socket
 
     @property
     def transport(self) -> Optional[asyncio.DatagramTransport]:
         return self.socket_binding.transport
 
     @transport.setter
@@ -226,16 +228,16 @@
     async def iter_datagrams(self) -> AsyncIterator[Tuple[SddpSocketBinding, HostAndPort, SddpDatagram]]:
         while True:
             result = await self.receive()
             if result is None:
                 break
             yield result
 
-    async def __aiter__(self) -> AsyncIterator[Tuple[SddpSocketBinding, HostAndPort, SddpDatagram]]:
-        return await self.iter_datagrams()
+    def __aiter__(self) -> AsyncIterator[Tuple[SddpSocketBinding, HostAndPort, SddpDatagram]]:
+        return self.iter_datagrams()
 
     def set_final_result(self) -> None:
         if not self.final_result.done():
             self.final_result.set_result(None)
             if not self.queue is None:
                 # wake up any waiting tasks
                 try:
@@ -301,15 +303,15 @@
             try:
                 # wake up any waiting tasks
                 self.queue.put_nowait(None)
             except asyncio.QueueFull:
                 # queue is full so waiters will wake up soon
                 pass
 
-class SddpSocket(AsyncContextManager[Self]):
+class SddpSocket(AsyncContextManager['SddpSocket']):
     """
     An abstract async SDDP socket that can:
 
       1. Listen on either a multicast or unicast address
       2. Receive and decode SddpDatagrams from remote nodes and deliver them to any number of async subscribers
       3. Send SddpDatagrams to a remote multicast or unicast address
```

### Comparing `sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/server.py` & `sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
     bind_addresses: List[str]
     """The IP addresses to bind to. If None, all local IP addresses will be used."""
 
     include_loopback: bool = False
     """If True, loopback addresses will be included in the list of local IP addresses to bind to."""
 
-    notify_handlers: Dict[int, SddpServerNotifyHandler] = []
+    notify_handlers: Dict[int, SddpServerNotifyHandler]
     """A set of handlers that will be called when an advertisement notification is received from a remote host,
        indexed by ID number."""
 
     i_next_notify_handler: int = 0
     """The next notify handler ID to assign."""
 
     def __init__(
@@ -191,15 +191,15 @@
             if is_ipv6:
                 assert address_family == socket.AF_INET6
                 mreq = group_bin + bind_bin_addr
                 sock.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_JOIN_GROUP, mreq)
             else:
                 assert address_family == socket.AF_INET
                 mreq = group_bin + bind_bin_addr
-                logger.debug(f"Joining multicast group {self.multicast_address} on {bind_address}; mreq={mreq}")
+                logger.debug(f"Joining multicast group {self.multicast_address} on {bind_address}; mreq={mreq!r}")
                 sock.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, mreq)
             socket_binding = SddpSocketBinding(sock, unicast_addr=(bind_address, self.multicast_port))
             await self.add_socket_binding(socket_binding)
 
     def add_notify_handler(self, handler: SddpServerNotifyHandler) -> int:
         """Adds a handler to be called when an advertisement notification is received from a remote host."""
         i = self.i_next_notify_handler
@@ -313,14 +313,15 @@
                             except ValueError:
                                 pass
                             if not version_major is None and not version_minor is None and version_major >= 1:
                                 pattern = m.group('pattern')
                                 # NOTE: in the future when SDDP protocol is documented, we can filter based on pattern
                                 #       but for now we will always respond.
                                 logger.debug(f"Sddp responder received SEARCH request from {addr} on {socket_binding}: pattern='{pattern}', protocol={statement_protocol}, version={version_major}.{version_minor}")
+                                assert not self.advertise_datagram is None
                                 response = self.advertise_datagram.copy()
                                 response.statement_line = f"{statement_protocol}/{version_major}.{version_minor} 200 OK"
                                 if not 'From' in response:
                                     # Fill in the From header with the unicast address that applies to the interface on which the request was received
                                     unicast_ip, unicast_port = socket_binding.unicast_addr
                                     response['From'] = f"{unicast_ip}:{unicast_port}"
                                 socket_binding.sendto(response, addr)
@@ -334,14 +335,15 @@
 
     async def _run_advertiser_task(self) -> None:
         logger.debug(f"Sddp advertiser task starting, advertising every {self.advertise_interval} seconds")
         assert self.advertise_interval > 0.0
         try:
             while not self.final_result.done():
                 for socket_binding in self.socket_bindings:
+                    assert not self.advertise_datagram is None
                     advertise_datagram = self.advertise_datagram.copy()
                     if not 'From' in advertise_datagram:
                         # Fill in the From header with the unicast address that applies to the interface on which the advertisement is being sent
                         unicast_ip, unicast_port = socket_binding.unicast_addr
                         advertise_datagram['From'] = f"{unicast_ip}:{unicast_port}"
                     socket_binding.sendto(advertise_datagram, (self.multicast_address, self.multicast_port))
                 try:
```

### Comparing `sddp_discovery_protocol-1.3.0/sddp_discovery_protocol/util.py` & `sddp_discovery_protocol-1.5.0/sddp_discovery_protocol/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
        returns (None, None) if there is no default gateway in the requested family."""
     assert int(address_family) in (int(socket.AF_INET), int(socket.AF_INET6))
     netiface_family = netifaces.AF_INET if int(address_family) == int(socket.AF_INET) else netifaces.AF_INET6
     gws = netifaces.gateways()
     if "default" in gws:
         default_gateway_infos = gws["default"]
         if netiface_family in default_gateway_infos:
-            gw_ip, gw_interface_name = default_gateway_infos[netiface_family]
+            gw_ip, gw_interface_name = default_gateway_infos[netiface_family][:2]
             return (gw_ip, gw_interface_name)
     return (None, None)
 
 if __name__ == "__main__":
     import sys
     import argparse
```

### Comparing `sddp_discovery_protocol-1.3.0/PKG-INFO` & `sddp_discovery_protocol-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sddp-discovery-protocol
-Version: 1.3.0
+Version: 1.5.0
 Summary: Implementation of Control4's Simple Device Discovery Protocol (SDDP)
 Home-page: https://github.com/sammck/sddp-discovery-protocol
 License: MIT
 Keywords: Control4,SDDP,SSDP,UPnP,protocol,multicast,UDP,discovery,network,automation,smart-home
 Author: Sam McKelvie
 Author-email: dev@mckelvie.org
 Requires-Python: >=3.8,<4.0
```

