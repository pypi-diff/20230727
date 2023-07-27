# Comparing `tmp/xhac-0.1.1-py3-none-any.whl.zip` & `tmp/xhac-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14139 bytes, number of entries: 11
+Zip file size: 14808 bytes, number of entries: 11
 -rw-r--r--  2.0 unx    10036 b- defN 20-Feb-02 00:00 xhac/HomeClient.py
--rw-r--r--  2.0 unx     1206 b- defN 20-Feb-02 00:00 xhac/Scanner.py
+-rw-r--r--  2.0 unx     1272 b- defN 20-Feb-02 00:00 xhac/Scanner.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 xhac/__init__.py
--rw-r--r--  2.0 unx     1898 b- defN 20-Feb-02 00:00 xhac/cli.py
+-rw-r--r--  2.0 unx     3668 b- defN 20-Feb-02 00:00 xhac/cli.py
 -rw-r--r--  2.0 unx    15994 b- defN 20-Feb-02 00:00 xhac/pyparser.py
 -rw-r--r--  2.0 unx     8536 b- defN 20-Feb-02 00:00 xhac/util.py
-?rw-r--r--  2.0 unx     2094 b- defN 20-Feb-02 00:00 xhac-0.1.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 xhac-0.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       39 b- defN 20-Feb-02 00:00 xhac-0.1.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 xhac-0.1.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      812 b- defN 20-Feb-02 00:00 xhac-0.1.1.dist-info/RECORD
-11 files, 41775 bytes uncompressed, 12793 bytes compressed:  69.4%
+?rw-r--r--  2.0 unx     2094 b- defN 20-Feb-02 00:00 xhac-0.1.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 xhac-0.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx       39 b- defN 20-Feb-02 00:00 xhac-0.1.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 xhac-0.1.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      812 b- defN 20-Feb-02 00:00 xhac-0.1.2.dist-info/RECORD
+11 files, 43611 bytes uncompressed, 13462 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: xhac/pyparser.py
 Comment: 
 
 Filename: xhac/util.py
 Comment: 
 
-Filename: xhac-0.1.1.dist-info/METADATA
+Filename: xhac-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xhac-0.1.1.dist-info/WHEEL
+Filename: xhac-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xhac-0.1.1.dist-info/entry_points.txt
+Filename: xhac-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: xhac-0.1.1.dist-info/licenses/LICENSE
+Filename: xhac-0.1.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: xhac-0.1.1.dist-info/RECORD
+Filename: xhac-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xhac/Scanner.py

```diff
@@ -1,16 +1,18 @@
 from zeroconf import ServiceBrowser, ServiceListener, Zeroconf
 import time
 
 
-class SGWServer:
-    def __init__(self, name, ip, port):
+class HomeServer:
+    def __init__(self, name, ip, port, id, hostname):
         self.name = name
         self.ip = ip
         self.port = port
+        self.id = id
+        self.hostname = hostname
 
 
 class Listener(ServiceListener):
 
     def __init__(self, servers) -> None:
         super().__init__()
         self.servers = servers
@@ -19,28 +21,29 @@
         pass
 
     def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:
         pass
 
     def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:
         info = zc.get_service_info(type_, name)
-        self.servers.append(SGWServer(info.properties[b'name'].decode(), info.parsed_addresses()[0], info.port))
+        self.servers.append(
+            HomeServer(
+                info.properties[b'name'].decode(),
+                info.parsed_addresses()[0],
+                info.port,
+                info.properties[b'id'].decode(),
+                info.server
+            )
+        )
 
 
 class Scanner:
 
     def __init__(self):
         self.servers = []
 
     def scan(self, duration):
         zeroconf = Zeroconf()
         listener = Listener(self.servers)
         ServiceBrowser(zeroconf, "_sgw._tcp.local.", listener)
         time.sleep(duration)
         zeroconf.close()
-
-
-if __name__ == "__main__":
-    scanner = Scanner()
-    scanner.scan(2)
-    for server in scanner.servers:
-        print(f"{server.name} {server.ip} {server.port}")
```

## xhac/cli.py

```diff
@@ -1,40 +1,111 @@
 from rich.console import Console
 from rich.table import Table
 from rich import box
+from typing import Union, Any
+import click
 from .HomeClient import HomeClient
 from .Scanner import Scanner
 
-def main():
+CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
+
+
+def get_version():
+    from pkg_resources import get_distribution
+    return get_distribution("xhac").version
+
+
+def print_version(context: click.Context, param: Union[click.Option, click.Parameter], value: bool) -> Any:
+    """Print the version of mbed-tools."""
+    if not value or context.resilient_parsing:
+        return
+    click.echo(get_version())
+    context.exit()
+
+
+@click.group(context_settings=CONTEXT_SETTINGS)
+@click.option(
+    "--version",
+    is_flag=True,
+    callback=print_version,
+    expose_value=False,
+    is_eager=True,
+    help="Display versions.",
+)
+def cli() -> None:
+    """The MXOS Home Access Client Tool."""
+    pass
+
+
+@click.command()
+@click.argument("duration", type=click.INT, default=2)
+def scan(duration: int) -> None:
+    """Scan for MXCHIP Home Access Server on local network.
+
+    Arguments:
+
+        DURATION : Scan duration time in seconds.
+
+    Example:
+
+        $ xhac scan 2
+    """
     scanner = Scanner()
-    print("Scanning for servers ...")
-    scanner.scan(2)
+    click.echo("Scanning for servers ...")
+    scanner.scan(duration)
+
     if len(scanner.servers) == 0:
-        print("No server found")
-        exit(1)
+        click.echo("No server found")
+        return
+
+    table = Table(title="Servers", box=box.ROUNDED)
+    table.add_column("Name")
+    table.add_column("ID")
+    table.add_column("Host")
     for index, server in enumerate(scanner.servers):
-        print(f"{index}: {server.name} {server.ip} {server.port}")
-    index = int(input("- Select a server: "))
-    server = scanner.servers[index]
+        table.add_row(server.name, server.id, f"{server.ip}:{server.port}")
+    console = Console()
+    console.print(table)
+
+
+@click.command()
+@click.argument("host", type=click.STRING)
+@click.argument("username", type=click.STRING)
+@click.argument("password", type=click.STRING)
+def load(host: str, username: str, password: str) -> None:
+    """Connect to MXCHIP Home Access Server and load Home model.
+
+    Arguments:
+
+        HOST : Format <IP>:<Port>, 192.168.31.66:52348.
+
+        USERNAME: Username of the server.
 
-    password = input("- Input password: ")
+        PASSWORD: Password of the server.
+
+    Example:
+
+        $ xhac load 192.168.31.66:52348 SGW2052 mxchip123
+    """
+
+    ip, port = host.split(":")
 
     def OnEvent(event):
         print(f"OnEvent: {event}")
 
     def OnDisconnect():
         print("Disconnected")
 
     homeClient = HomeClient(OnEvent, OnDisconnect)
-    homeClient.SetHost(server.ip, server.port)
-    homeClient.SetAccount(server.name, password)
+    homeClient.SetHost(ip, int(port))
+    homeClient.SetAccount(username, password)
 
     if not homeClient.Connect():
-        print("Failed to connect")
-        exit(1)
+        click.echo("Failed to connect")
+        return
 
     homeDB = homeClient.GetHome()
 
     console = Console()
 
     table = Table(title="Scenes", box=box.ROUNDED)
     table.add_column("ID")
@@ -57,12 +128,20 @@
         return "Unknown"
 
     table = Table(title="Devices", box=box.ROUNDED)
     table.add_column("ID")
     table.add_column("Name")
     table.add_column("Room")
     for device in homeDB["devices"]:
-        table.add_row(f"{device['did']}", device["name"], FindZone(device["zid"]))
+        table.add_row(f"{device['did']}", device["name"],
+                      FindZone(device["zid"]))
     console.print(table)
 
-if __name__=="__main__":
-    main()
+
+def main():
+    cli.add_command(scan, "scan")
+    cli.add_command(load, "load")
+    cli()
+
+
+if __name__ == "__main__":
+    main()
```

## Comparing `xhac-0.1.1.dist-info/METADATA` & `xhac-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhac
-Version: 0.1.1
+Version: 0.1.2
 Summary: MXCHIP Home Access Client
 Project-URL: Homepage, https://www.mxchip.com/
 Project-URL: Documentation, https://www.mxchip.com/
 Project-URL: Repository, https://www.mxchip.com/
 Project-URL: Changelog, https://www.mxchip.com/
 Author-email: Snow Yang <yangsw@mxchip.com>
 Maintainer-email: Snow Yang <yangsw@mxchip.com>
```

## Comparing `xhac-0.1.1.dist-info/licenses/LICENSE` & `xhac-0.1.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `xhac-0.1.1.dist-info/RECORD` & `xhac-0.1.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 xhac/HomeClient.py,sha256=avRD6pvcpJ8Rcdug-OUC-HEzsN2JMls9ViUXJesc6go,10036
-xhac/Scanner.py,sha256=92gbm1KyuvAWJ_KhSTq4zakIR9pDfaffAVNexNSiKFI,1206
+xhac/Scanner.py,sha256=BM_tddVtw_EdxyeqRyqPkfsx_sROHqJVl1YwC08NrP0,1272
 xhac/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xhac/cli.py,sha256=VuEadAD04MV1Tq-y_evICvEwy8xQITLaQqjD78kGMJA,1898
+xhac/cli.py,sha256=0tstjbVGQbLyo2kG__ZkCoIfqpDA-I6YPZwOHFWuaEo,3668
 xhac/pyparser.py,sha256=uPnBAJZrHVyvDaqPhxvCnL2NmVTcDglwfFNcOFsr-pA,15994
 xhac/util.py,sha256=0wDCmFD4OLxUwKOgK03HkNWo5PW-K2BWierNv6ks0jY,8536
-xhac-0.1.1.dist-info/METADATA,sha256=aNrCYwcjVrlPiWHZEdn1wW0avYgjxTDw3xu3L_4_nkI,2094
-xhac-0.1.1.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-xhac-0.1.1.dist-info/entry_points.txt,sha256=khqPAUxrPdx8solPOTMftLurNpWL52j6gfN6dRsQq5Q,39
-xhac-0.1.1.dist-info/licenses/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
-xhac-0.1.1.dist-info/RECORD,,
+xhac-0.1.2.dist-info/METADATA,sha256=HwGXDTZ8-tR2gNctoFWGVpo-PdoTbwzK96L3DH0aIUA,2094
+xhac-0.1.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+xhac-0.1.2.dist-info/entry_points.txt,sha256=khqPAUxrPdx8solPOTMftLurNpWL52j6gfN6dRsQq5Q,39
+xhac-0.1.2.dist-info/licenses/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
+xhac-0.1.2.dist-info/RECORD,,
```

