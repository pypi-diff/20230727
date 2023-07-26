# Comparing `tmp/nclib-1.0.2.tar.gz` & `tmp/nclib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nclib-1.0.2.tar", last modified: Wed Aug  3 23:50:00 2022, max compression
+gzip compressed data, was "nclib-1.0.3.tar", last modified: Wed Jul 26 22:49:13 2023, max compression
```

## Comparing `nclib-1.0.2.tar` & `nclib-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2022-08-03 23:50:00.741348 nclib-1.0.2/
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     1774 2022-08-03 23:50:00.741348 nclib-1.0.2/PKG-INFO
--rw-r--r--   0 audrey    (1000) audrey    (1000)     1169 2020-06-08 20:54:44.000000 nclib-1.0.2/README.rst
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2022-08-03 23:50:00.741348 nclib-1.0.2/nclib/
--rw-r--r--   0 audrey    (1000) audrey    (1000)      302 2020-06-08 20:54:44.000000 nclib-1.0.2/nclib/__init__.py
--rw-r--r--   0 audrey    (1000) audrey    (1000)      154 2020-06-08 20:54:44.000000 nclib-1.0.2/nclib/errors.py
--rw-r--r--   0 audrey    (1000) audrey    (1000)    10614 2020-06-08 20:54:44.000000 nclib-1.0.2/nclib/logger.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)    33495 2022-08-03 23:46:21.000000 nclib-1.0.2/nclib/netcat.py
--rw-r--r--   0 audrey    (1000) audrey    (1000)     6506 2020-06-08 20:54:44.000000 nclib-1.0.2/nclib/process.py
--rw-r--r--   0 audrey    (1000) audrey    (1000)     1951 2020-06-08 20:54:44.000000 nclib-1.0.2/nclib/select.py
--rw-r--r--   0 audrey    (1000) audrey    (1000)     2926 2020-06-08 20:54:44.000000 nclib-1.0.2/nclib/server.py
--rw-rw-r--   0 audrey    (1000) audrey    (1000)    11485 2021-05-03 09:37:29.000000 nclib-1.0.2/nclib/simplesock.py
-drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2022-08-03 23:50:00.741348 nclib-1.0.2/nclib.egg-info/
--rw-r--r--   0 audrey    (1000) audrey    (1000)     1774 2022-08-03 23:50:00.000000 nclib-1.0.2/nclib.egg-info/PKG-INFO
--rw-r--r--   0 audrey    (1000) audrey    (1000)      282 2022-08-03 23:50:00.000000 nclib-1.0.2/nclib.egg-info/SOURCES.txt
--rw-r--r--   0 audrey    (1000) audrey    (1000)        1 2022-08-03 23:50:00.000000 nclib-1.0.2/nclib.egg-info/dependency_links.txt
--rw-r--r--   0 audrey    (1000) audrey    (1000)        6 2022-08-03 23:50:00.000000 nclib-1.0.2/nclib.egg-info/top_level.txt
--rwxr-xr-x   0 audrey    (1000) audrey    (1000)     1906 2020-06-08 20:54:44.000000 nclib-1.0.2/serve-stdio
--rw-rw-r--   0 audrey    (1000) audrey    (1000)       38 2022-08-03 23:50:00.741348 nclib-1.0.2/setup.cfg
--rw-rw-r--   0 audrey    (1000) audrey    (1000)     1796 2022-08-03 23:47:03.000000 nclib-1.0.2/setup.py
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-26 22:49:13.997812 nclib-1.0.3/
+-rw-r--r--   0 audrey    (1000) audrey    (1000)     1082 2020-06-08 20:54:44.000000 nclib-1.0.3/LICENSE
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1541 2023-07-26 22:49:13.997812 nclib-1.0.3/PKG-INFO
+-rw-r--r--   0 audrey    (1000) audrey    (1000)     1169 2020-06-08 20:54:44.000000 nclib-1.0.3/README.rst
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-26 22:49:13.997812 nclib-1.0.3/nclib/
+-rw-r--r--   0 audrey    (1000) audrey    (1000)      302 2020-06-08 20:54:44.000000 nclib-1.0.3/nclib/__init__.py
+-rw-r--r--   0 audrey    (1000) audrey    (1000)      154 2020-06-08 20:54:44.000000 nclib-1.0.3/nclib/errors.py
+-rw-r--r--   0 audrey    (1000) audrey    (1000)    10614 2020-06-08 20:54:44.000000 nclib-1.0.3/nclib/logger.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    33617 2023-07-25 17:49:03.000000 nclib-1.0.3/nclib/netcat.py
+-rw-r--r--   0 audrey    (1000) audrey    (1000)     6506 2020-06-08 20:54:44.000000 nclib-1.0.3/nclib/process.py
+-rw-r--r--   0 audrey    (1000) audrey    (1000)     1951 2020-06-08 20:54:44.000000 nclib-1.0.3/nclib/select.py
+-rw-r--r--   0 audrey    (1000) audrey    (1000)     3342 2023-07-25 17:37:26.000000 nclib-1.0.3/nclib/server.py
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)    11485 2021-05-03 09:37:29.000000 nclib-1.0.3/nclib/simplesock.py
+drwxrwxr-x   0 audrey    (1000) audrey    (1000)        0 2023-07-26 22:49:13.997812 nclib-1.0.3/nclib.egg-info/
+-rw-r--r--   0 audrey    (1000) audrey    (1000)     1541 2023-07-26 22:49:13.000000 nclib-1.0.3/nclib.egg-info/PKG-INFO
+-rw-r--r--   0 audrey    (1000) audrey    (1000)      290 2023-07-26 22:49:13.000000 nclib-1.0.3/nclib.egg-info/SOURCES.txt
+-rw-r--r--   0 audrey    (1000) audrey    (1000)        1 2023-07-26 22:49:13.000000 nclib-1.0.3/nclib.egg-info/dependency_links.txt
+-rw-r--r--   0 audrey    (1000) audrey    (1000)        6 2023-07-26 22:49:13.000000 nclib-1.0.3/nclib.egg-info/top_level.txt
+-rwxr-xr-x   0 audrey    (1000) audrey    (1000)     1906 2020-06-08 20:54:44.000000 nclib-1.0.3/serve-stdio
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)       38 2023-07-26 22:49:13.997812 nclib-1.0.3/setup.cfg
+-rw-rw-r--   0 audrey    (1000) audrey    (1000)     1796 2023-07-26 22:48:41.000000 nclib-1.0.3/setup.py
```

### Comparing `nclib-1.0.2/PKG-INFO` & `nclib-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,47 @@
-Metadata-Version: 1.2
-Name: nclib
-Version: 1.0.2
-Summary: Netcat as a library: convienent socket interfaces
-Home-page: https://github.com/rhelmot/nclib
-Author: rhelmot
-Author-email: audrey@rhelmot.io
-License: MIT
-Description: 
-        nclib is a python socket library that wants to be your friend.
-        
-        nclib provides:
-        
-        - Easy-to-use interfaces for connecting to and listening on TCP and UDP sockets
-        - The ability to handle any python stream-like object with a single interface
-        - A better socket class, the Netcat object
-        
-          - Convenient receive methods for common socket usage patterns
-          - Highly customizable logging
-          - Interactive mode, connecting the socket to your stdin/stdout
-          - Intelligent detection of socket closes and connection drops
-          - Long-running functions cleanly abortable with ctrl-c
-          - Lots of aliases in case you forget the right method name
-        
-        - Mechanisms to launch processes with their in/out streams connected to sockets
-        
-          - Launch a process with gdb attached
-        
-        - TCP and UDP server classes for writing simple python daemons
-        - A script to easily daemonize command-line programs
-        
-        Documentation is available at https://nclib.readthedocs.io/ and source code is
-        available at https://github.com/rhelmot/nclib
-        
-        If you are familiar with pwntools, nclib provides much of the functionaly that
-        pwntools' socket wrappers do, but with the bonus feature of not being pwntools.
-        
-Keywords: netcat nc socket sock file pipe tcp udp recv until logging interact handle listen connect server serve stdio process gdb
-Platform: UNKNOWN
-Requires-Python: >=3.5
+long_description = '''
+nclib is a python socket library that wants to be your friend.
+
+nclib provides:
+
+- Easy-to-use interfaces for connecting to and listening on TCP and UDP sockets
+- The ability to handle any python stream-like object with a single interface
+- A better socket class, the Netcat object
+
+  - Convenient receive methods for common socket usage patterns
+  - Highly customizable logging
+  - Interactive mode, connecting the socket to your stdin/stdout
+  - Intelligent detection of socket closes and connection drops
+  - Long-running functions cleanly abortable with ctrl-c
+  - Lots of aliases in case you forget the right method name
+
+- Mechanisms to launch processes with their in/out streams connected to sockets
+
+  - Launch a process with gdb attached
+
+- TCP and UDP server classes for writing simple python daemons
+- A script to easily daemonize command-line programs
+
+Documentation is available at https://nclib.readthedocs.io/ and source code is
+available at https://github.com/rhelmot/nclib
+
+If you are familiar with pwntools, nclib provides much of the functionaly that
+pwntools' socket wrappers do, but with the bonus feature of not being pwntools.
+'''
+
+if bytes is str:
+  raise Exception("nclib is python 3 only now :(")
+
+from setuptools import setup
+setup(name='nclib',
+      version='1.0.3',
+      python_requires='>=3.5',
+      packages=['nclib'],
+      scripts=['serve-stdio'],
+      description='Netcat as a library: convienent socket interfaces',
+      long_description=long_description,
+      url='https://github.com/rhelmot/nclib',
+      author='rhelmot',
+      author_email='audrey@rhelmot.io',
+      license='MIT',
+      keywords='netcat nc socket sock file pipe tcp udp recv until logging interact handle listen connect server serve stdio process gdb'
+      )
```

### Comparing `nclib-1.0.2/README.rst` & `nclib-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `nclib-1.0.2/nclib/logger.py` & `nclib-1.0.3/nclib/logger.py`

 * *Files identical despite different names*

### Comparing `nclib-1.0.2/nclib/netcat.py` & `nclib-1.0.3/nclib/netcat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import getopt
 import re
 import socket
 import sys
 import time
 from urllib.parse import urlparse
-from typing import Optional, Union
+from typing import Optional, Union, Literal
 
 from . import simplesock, select, errors, logger
 
 PROTOCAL_RE = re.compile('^[a-z0-9]+://')
 KNOWN_SCHEMES = {
     # schema: (udp, ipv6, port); None = unchanged
     'tcp': (False, None, None),
@@ -21,14 +21,15 @@
     'https': (False, None, 443),
     'dns': (True, None, 53),
     'ftp': (False, None, 20),
     'ssh': (False, None, 22),
     'smtp': (False, None, 25),
 }
 BYTESISH = Union[bytes, str]
+DFLOAT = Union[float, int, Literal['default'], None]
 
 def encode(b: BYTESISH) -> bytes:
     if type(b) is str:
         return b.encode()
     elif type(b) is bytes:
         return b
     else:
@@ -625,31 +626,31 @@
         self.logger.unbuffering(ret)
         return ret
 
     #
     # Public socket data functions
     #
 
-    def _fixup_timeout(self, timeout='default') -> Optional[float]:
+    def _fixup_timeout(self, timeout: DFLOAT = 'default') -> Optional[float]:
         if timeout == 'default':
             return self._timeout
         return timeout
 
-    def recv(self, n: int=4096, timeout='default') -> bytes:
+    def recv(self, n: int=4096, timeout: DFLOAT = 'default') -> bytes:
         """
         Receive at most n bytes (default 4096) from the socket
 
         Aliases: read, get
         """
 
         timeout = self._fixup_timeout(timeout)
         self.logger.requesting_recv(n, timeout)
         return self._recv_predicate(lambda s: min(n, len(s)), timeout)
 
-    def recv_until(self, s: BYTESISH, max_size: Optional[int]=None, timeout='default') -> bytes:
+    def recv_until(self, s: BYTESISH, max_size: Optional[int]=None, timeout: DFLOAT = 'default') -> bytes:
         """
         Recieve data from the socket until the given substring is observed.
         Data in the same datagram as the substring, following the substring,
         will not be returned and will be cached for future receives.
 
         Aliases: read_until, readuntil, recvuntil
         """
@@ -663,27 +664,27 @@
         def _predicate(buf):
             try:
                 return min(buf.index(s) + len(s), max_size)
             except ValueError:
                 return 0 if len(buf) < max_size else max_size
         return self._recv_predicate(_predicate, timeout)
 
-    def recv_all(self, timeout='default') -> bytes:
+    def recv_all(self, timeout: DFLOAT = 'default') -> bytes:
         """
         Return all data recieved until connection closes or the timeout
         elapses.
 
         Aliases: read_all, readall, recvall
         """
 
         timeout = self._fixup_timeout(timeout)
         self.logger.requesting_recv_all(timeout)
         return self._recv_predicate(lambda s: 0, timeout, raise_eof=False)
 
-    def recv_exactly(self, n: int, timeout='default') -> bytes:
+    def recv_exactly(self, n: int, timeout: DFLOAT = 'default') -> bytes:
         """
         Recieve exactly n bytes
 
         Aliases: read_exactly, readexactly, recvexactly, recv_exact,
         read_exact, readexact, recvexact
         """
 
@@ -722,15 +723,15 @@
     #
     # Public socket data functionality
     # (implemented with other public socket data functions)
     #
 
     LINE_ENDING = b'\n'
 
-    def recv_line(self, max_size: Optional[int]=None, timeout='default', ending: Optional[BYTESISH]=None):
+    def recv_line(self, max_size: Optional[int]=None, timeout: DFLOAT = 'default', ending: Optional[BYTESISH]=None):
         """
         Recieve until the next newline , default "\\n". The newline string can
         be changed by changing ``nc.LINE_ENDING``. The newline will be returned
         as part of the string.
 
         Aliases: recvline, readline, read_line, readln, recvln
         """
```

### Comparing `nclib-1.0.2/nclib/process.py` & `nclib-1.0.3/nclib/process.py`

 * *Files identical despite different names*

### Comparing `nclib-1.0.2/nclib/select.py` & `nclib-1.0.3/nclib/select.py`

 * *Files identical despite different names*

### Comparing `nclib-1.0.2/nclib/server.py` & `nclib-1.0.3/nclib/server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import socket
+import select
 
 from . import Netcat
 
 class TCPServer:
     """
     A simple TCP server model. Iterating over it will yield client sockets as
     Netcat objects.
@@ -26,24 +27,35 @@
         self.kwargs = kwargs
 
         self.sock = socket.socket(type=socket.SOCK_STREAM)
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.sock.bind(bindto)
         self.sock.listen(kernel_backlog)
 
+        self._oob_rsock, self._oob_wsock = socket.socketpair()
+        self.closed = False
+
     def __iter__(self):
         while True:
+            rl, _, _ = select.select([self.sock, self._oob_rsock], [], [])
+            if self._oob_rsock in rl:
+                self._oob_rsock.close()
+                self._oob_wsock.close()
+                break
             client, addr = self.sock.accept()
             yield Netcat(sock=client, server=addr, **self.kwargs)
 
     def close(self):
         """
         Tear down this server and release its resources
         """
-        return self.sock.close()
+        if not self.closed:
+            self.closed = True
+            self._oob_wsock.send(b'.')
+            self.sock.close()
 
 
 class UDPServer:
     """
     A simple UDP server model. Iterating over it will yield of tuples of
     datagrams and peer addresses. To respond, use the respond method, which
     takes the response and the peer address.
```

### Comparing `nclib-1.0.2/nclib/simplesock.py` & `nclib-1.0.3/nclib/simplesock.py`

 * *Files identical despite different names*

### Comparing `nclib-1.0.2/serve-stdio` & `nclib-1.0.3/serve-stdio`

 * *Files identical despite different names*

