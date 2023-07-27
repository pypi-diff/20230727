# Comparing `tmp/wgconfig-0.3.0.tar.gz` & `tmp/wgconfig-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgconfig-0.3.0.tar", last modified: Sat Nov 19 14:34:00 2022, max compression
+gzip compressed data, was "wgconfig-1.0.0.tar", last modified: Thu Jul 27 12:56:20 2023, max compression
```

## Comparing `wgconfig-0.3.0.tar` & `wgconfig-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 14:33:59.852755 wgconfig-0.3.0/
--rwxrw-r--   0 root         (0) root         (0)    34523 2020-07-09 19:46:10.000000 wgconfig-0.3.0/LICENSE.txt
--rwxrw-r--   0 root         (0) root         (0)       21 2020-07-12 10:54:35.000000 wgconfig-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12721 2022-11-19 14:34:00.200750 wgconfig-0.3.0/PKG-INFO
--rwxrw-r--   0 root         (0) root         (0)     9596 2022-11-19 12:58:29.000000 wgconfig-0.3.0/README.md
--rwxrw-r--   0 root         (0) root         (0)      105 2022-11-19 14:34:00.780740 wgconfig-0.3.0/setup.cfg
--rwxrw-r--   0 root         (0) root         (0)     1308 2022-11-18 17:03:36.000000 wgconfig-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 14:33:55.792820 wgconfig-0.3.0/wgconfig/
--rwxrw-r--   0 root         (0) root         (0)    14688 2022-11-19 14:09:29.000000 wgconfig-0.3.0/wgconfig/__init__.py
--rwxrw-r--   0 root         (0) root         (0)     2108 2020-11-11 19:54:33.000000 wgconfig-0.3.0/wgconfig/wgexec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 14:33:59.152767 wgconfig-0.3.0/wgconfig.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12721 2022-11-19 14:29:45.000000 wgconfig-0.3.0/wgconfig.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      251 2022-11-19 14:29:47.000000 wgconfig-0.3.0/wgconfig.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-19 14:29:46.000000 wgconfig-0.3.0/wgconfig.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2022-11-19 14:29:46.000000 wgconfig-0.3.0/wgconfig.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-19 14:29:47.000000 wgconfig-0.3.0/wgconfig.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:56:20.050401 wgconfig-1.0.0/
+-rwxrw-r--   0 root         (0) root         (0)    34523 2020-07-09 19:46:10.000000 wgconfig-1.0.0/LICENSE.txt
+-rwxrw-r--   0 root         (0) root         (0)       21 2020-07-12 10:54:35.000000 wgconfig-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11977 2023-07-27 12:56:20.078400 wgconfig-1.0.0/PKG-INFO
+-rwxrw-r--   0 root         (0) root         (0)    11098 2023-07-27 12:38:00.000000 wgconfig-1.0.0/README.md
+-rwxrw-r--   0 root         (0) root         (0)      105 2023-07-27 12:56:20.146400 wgconfig-1.0.0/setup.cfg
+-rwxrw-r--   0 root         (0) root         (0)     1308 2023-07-26 16:06:26.000000 wgconfig-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:56:19.286410 wgconfig-1.0.0/wgconfig/
+-rwxrw-r--   0 root         (0) root         (0)    15707 2023-07-27 11:46:04.000000 wgconfig-1.0.0/wgconfig/__init__.py
+-rwxrw-r--   0 root         (0) root         (0)     2108 2020-11-11 19:54:33.000000 wgconfig-1.0.0/wgconfig/wgexec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:56:19.922402 wgconfig-1.0.0/wgconfig.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11977 2023-07-27 12:56:17.000000 wgconfig-1.0.0/wgconfig.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-27 12:56:18.000000 wgconfig-1.0.0/wgconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 12:56:17.000000 wgconfig-1.0.0/wgconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-27 12:56:18.000000 wgconfig-1.0.0/wgconfig.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-27 12:56:18.000000 wgconfig-1.0.0/wgconfig.egg-info/top_level.txt
```

### Comparing `wgconfig-0.3.0/LICENSE.txt` & `wgconfig-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wgconfig-0.3.0/PKG-INFO` & `wgconfig-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,300 +1,337 @@
 Metadata-Version: 2.1
 Name: wgconfig
-Version: 0.3.0
+Version: 1.0.0
 Summary: parsing and writing WireGuard configuration files
 Home-page: https://www.github.com/towalink/wgconfig
 Author: Dirk Henrici
 Author-email: towalink.wgconfig@henrici.name
-License: UNKNOWN
 Project-URL: Repository, https://www.github.com/towalink/wgconfig
 Project-URL: PyPi, https://pypi.org/project/wgconfig/
-Description: # wgconfig
-        
-        Parsing and writing WireGuard configuration files (comment preserving)
-        
-        WireGuard config files are ini-style. Since all "Peer" sections have the same name, these files cannot be parsed and modified by most modules handling configuration files. Most existing modules are not able to preserve or even add comments when modifying a config file. "wgconfig" was created to work with WireGuard configuration files and to preserve comments.
-        
-        ---
-        
-        ## Features
-        
-        - Read and parse WireGuard configuration files and make the data available as Python dictionaries
-        - Create new WireGuard configuration files
-        - Add peers to WireGuard configuration files and delete peers from WireGuard configuration files
-        - Save and clone WireGuard configuration files
-        - Comments are preserved when reading and writing WireGuard configuration files
-        - Leading comments may be added when creating sections or attributes
-        - Such comments may be deleted when removing sections or attributes
-        - No other modules are needed, i.e. no dependencies
-        
-        ---
-        
-        ## Installation
-        
-        Install using PyPi:
-        
-        ```shell
-        pip3 install wgconfig
-        ```
-        
-        ---
-        
-        ## Quickstart
-        
-        ### Reading and parsing an existing WireGuard configuration file
-        
-        Read and parse the existing WireGuard configuration file 'wg0.conf' located in '/etc/wireguard':
-        
-        ```python
-        import wgconfig
-        wc = wgconfig.WGConfig('wg0')
-        wc.read_file()
-        print('INTERFACE DATA:', wc.interface)
-        print('PEER DATA:', wc.peers)
-        ```
-        
-        Add a new peer with a comment line before the peer section:
-        ```python
-        wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Newly added peer')
-        ```
-        
-        Add an attribute to that peer:
-        ```python
-        wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'Endpoint', 'wg.example.com:51820', '# Added for demonstration purposes')
-        ```
-        
-        Write the changes to disk. Comments that were present when reading the file are preserved.
-        ```python
-        wc.write_file()
-        ```
-        
-        Please see below for more detailed usage information.
-        
-        ### Creating a new WireGuard configuration file
-        
-        Create a new WireGuard configuration file as '/root/wgtest.conf':
-        
-        ```python
-        import wgconfig
-        wc = wgconfig.WGConfig('/root/wgtest.conf')
-        # Add attribute to Interface section (denoted by 'None')
-        wc.add_attr(None, 'PrivateKey', '6FYKQKEtGFAb5HSwyj5cQl3wgS1E9d6SqVjdVksOn2s=')
-        # Save to disk
-        wc.write_file()
-        # Access the data
-        print('INTERFACE DATA:', wc.interface)
-        print('PEER DATA (there are no peers yet):', wc.peers)
-        ```
-        
-        The module also contains simple wrappers around the wg command to generate and manage keys:
-        
-        ```python
-        import wgconfig.wgexec as wgexec
-        # Create a new WireGuard private key
-        private_key = wgexec.generate_privatekey()
-        ```
-        
-        Please see below for more detailed usage information.
-        
-        ---
-        
-        ## Usage / API
-        
-        ### Properties
-        
-        * interface: Returns attributes and values of the Interface section as a dictionary
-        
-        * peers: Returns attributes and values of all peers as a nested dictionary
-        
-        ### Methods for interaction
-        
-        * `__init__(file)`
-        
-          *Initializes the instance*
-          
-          Parameters:
-          * "file" (str): Path of the WireGuard configuration file
-              You may also just provide the interface name. In this case, the path '/etc/wireguard' is assumed along with a file extension '.conf'.
-          
-          Examples:
-          * `wc = wgconfig.WGConfig('wg0')`
-          * `wc = wgconfig.WGConfig('/etc/wireguard/wg0.conf')`
-        
-        * `read_file()`
-        
-          *Reads the WireGuard config file into memory*
-                
-        * `write_file(file)`
-        
-          *Writes a WireGuard config file from memory to file*
-                
-          Parameters:
-          * "file" (str, optional, default: None): Path of the WireGuard configuration file
-              You may also just provide the interface name. In this case the path '/etc/wireguard' is assumed along with a file extension '.conf'.
-              In case the parameter is missing, the config file defined on object initialization is used.
-        
-          Examples:
-          * `wc.write_file()`
-          * `wc.write_file('wg0')`
-          * `wc.write_file('/etc/wireguard/wg0.conf')`
-        
-        * `initialize_file(leading_comment)`
-        
-          *Empties the file and adds the interface section header*
-        
-          Parameters:
-          * "leading_comment" (str, optional, default: None): Comment line to be added before the Interface section. Must start with a '#' to indicate a comment.
-        
-          Examples:
-          * `wc.initialize_file()`
-          * `wc.initialize_file('# Here comes the Interface section:')`
-        
-        * `get_peer(key, include_details)`
-        
-          *Returns the data of the peer with the given (public) key*
-          
-          Parameters:
-          * "key" (str): Public key of the peer
-          * "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
-        
-          Examples:
-          * `wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-          * `wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', include_details = True)`
-        
-          Notes:
-          * Don't forget to call `read_file()` before attempting to get data out of a file
-          * Access the `peers` property if you want to retrieve the data of all peers    
-        
-        * `add_peer(key, leading_comment)`
-        
-          *Adds a new peer with the given (public) key*
-        
-          Parameters:
-          * "key" (str): Public key of the new peer
-          * "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
-        
-          Examples:
-          * `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-          * `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Here comes the Interface section:')`
-        
-        * `del_peer(key)`
-        
-          *Removes the peer with the given (public) key*
-          
-          Note: Comment lines immediately before the Peer section are removed, too.
-          
-          Parameters:
-          * "key" (str): Public key of the peer
-        
-          Examples:
-          * `wc.del_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-        
-        * `add_attr(key, attr, value, leading_comment, append_as_line)`
-        
-          *Adds an attribute/value pair to the given peer ('None' for adding an interface attribute)*
-          
-          Parameters:
-          * "key" (str): Key of the peer. Set to 'None' to denote the Interface section
-          * "attr" (str) Name of the attribute to add
-          * "value" (str or int) Value of the attribute to add
-          * "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
-          * "append_as_line" (bool, optional, default: False): Whether to add the attribute as a new line if another attribute with the same name already exists. If "False", adding an attribute that already exists results in comma-separated attribute values. This way, "AllowedIPs" can be added one by one.
-        
-          Examples:
-          * `wc.add_attr(None, 'ListenPort', '51820')`
-          * `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
-          * `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', '# Allow all IPv4 addresses', append_as_line=True)`
-        
-        * `del_attr(self, key, attr, value, remove_leading_comments)`
-        
-          *Removes an attribute/value pair from the given peer ('None' for adding an interface attribute); set 'value' to 'None' to remove all values*
-        
-          Parameters:
-          * "key" (str): Key of the peer. Set to 'None' to denote the Interface section
-          * "attr" (str) Name of the attribute to remove
-          * "value" (str or int, optional, default: None) Value of the attribute to remove
-              Set to 'None' if all values (either comma-separated or is multiple attribute lines) shall be removed. Otherwise specify the specific value to be removed.
-          * "remove_leading_comments" (bool, optional, default: True): Indicates whether comment lines before the attribute line(s) shall be removed, too
-        
-          Examples:
-          * `wc.del_attr(None, 'ListenPort')`
-          * `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs')`
-          * `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
-          * `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', remove_leading_comments=False)`
-        
-        * `disable_peer(self, key)`
-        
-          *Disables the peer with the given (public) key by prepending #! to all lines in a peer section*
-        
-          Parameters:
-          * "key" (str): Public key of the peer
-          
-          Examples:
-          * `wc.disable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-        
-        * `enable_peer(self, key)`
-        
-          *Enables the peer with the given (public) key by removing #! from all lines in a peer section*
-        
-          Parameters:
-          * "key" (str): Public key of the peer
-          
-          Examples:
-          * `wc.enable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-        
-        * `get_peer_enabled(self, key)`
-        
-          *Checks whether the peer with the given (public) key is enabled*
-        
-          Parameters:
-          * "key" (str): Public key of the peer
-          
-          Examples:
-          * `wc.get_peer_enabled('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-        
-        ---
-        
-        ## Reporting bugs
-        
-        In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
-        
-        ---
-        ## Developers
-        
-        ### Clone repository
-        
-        Clone this repo to your local machine using `https://github.com/towalink/wgconfig.git`
-        
-        Install the module temporarily to make it available in your Python installation:
-        ```shell
-        pip3 install -e <path to root of "src" directory>
-        ```
-        
-        ### Run unit tests
-        
-        Call "pytest" to run the unit tests:
-        ```shell
-        pytest <path to root of "test" directory>
-        ```
-        
-        ---
-        
-        ## License
-        
-        [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
-        
-        - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-        - Copyright 2020-2022 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
-        - [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
-        
 Keywords: WireGuard configuration config wg
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# wgconfig
+
+Parsing and writing WireGuard configuration files (comment preserving)
+
+WireGuard config files are ini-style. Since all "Peer" sections have the same name, these files cannot be parsed and modified by most libraries handling configuration files. Most existing libraries are not able to preserve or even add comments when modifying a config file. "wgconfig" was created to work with WireGuard configuration files and to preserve comments.
+
+---
+
+## Features
+
+- Read and parse WireGuard configuration files and make the data available as Python dictionaries.
+- Create new WireGuard configuration files.
+- Add peers to WireGuard configuration files and delete peers from WireGuard configuration files.
+- Save and clone WireGuard configuration files.
+- Comments are preserved when reading and writing WireGuard configuration files.
+- Leading comments may be added when creating sections or attributes.
+- Such comments may be deleted when removing sections or attributes.
+- No other libraries are needed, i.e. no dependencies.
+
+---
+
+## Installation
+
+Install using PyPi:
+
+```shell
+pip3 install wgconfig
+```
+
+---
+
+## Quickstart
+
+### Reading and parsing an existing WireGuard configuration file
+
+Read and parse the existing WireGuard configuration file 'wg0.conf' located in '/etc/wireguard':
+
+```python
+import wgconfig
+wc = wgconfig.WGConfig('wg0')
+wc.read_file()
+print('INTERFACE DATA:', , wc.get_interface())
+print('LIST OF PEERS:', wc.get_peers())
+print('ALL PEER DATA:', wc.get_peers(keys_only=False))
+```
+
+Add a new peer with a comment line before the peer section:
+```python
+wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Newly added peer')
+```
+
+Add an attribute to that peer:
+```python
+wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'Endpoint', 'wg.example.com:51820', '# Added for demonstration purposes')
+```
+
+Write the changes to disk. Comments that were present when reading the file are preserved.
+```python
+wc.write_file()
+```
+
+Please see below for more detailed usage information.
+
+### Creating a new WireGuard configuration file
+
+Create a new WireGuard configuration file as '/root/wgtest.conf':
+
+```python
+import wgconfig
+wc = wgconfig.WGConfig('/root/wgtest.conf')
+# Add attribute to Interface section (denoted by 'None')
+wc.add_attr(None, 'PrivateKey', '6FYKQKEtGFAb5HSwyj5cQl3wgS1E9d6SqVjdVksOn2s=')
+# Save to disk
+wc.write_file()
+# Access the data
+print('INTERFACE DATA:', wc.get_interface())
+print('LIST OF PEERS (there are no peers yet):', wc.get_peers())
+print('ALL PEER DATA (there are no peers yet):', wc.get_peers(keys_only=False))
+```
+
+The module also contains simple wrappers around the wg command to generate and manage keys:
+
+```python
+import wgconfig.wgexec as wgexec
+# Create a new WireGuard private key
+private_key = wgexec.generate_privatekey()
+```
+
+More information and examples can be found here:
+
+- [Detailed example for reading WireGuard config files](https://github.com/towalink/wgconfig/blob/master/doc/example_notebook_1.md)
+- Please see the section below for detailed API description.
+
+---
+
+## Detailed API description
+
+### Properties
+
+#### interface
+
+*Returns attributes and values (including wgconfig-internal ones) of the Interface section as a dictionary*
+
+Notes:
+* You might want to use the more flexible `get_interface()` method (see further below) instead.
+
+#### peers
+
+*Returns attributes and values (including wgconfig-internal ones) of all peers as a nested dictionary*
+
+Notes:
+* You might want to use the more flexible `get_peers()` method (see further below) instead.
+
+### Methods for interaction
+
+#### `__init__(file)`
+
+*Initializes the instance*
+
+Parameters:
+* "file" (str): Path of the WireGuard configuration file
+    You may also just provide the interface name. In this case, the path '/etc/wireguard' is assumed along with a file extension '.conf'.
+
+Examples:
+* `wc = wgconfig.WGConfig('wg0')`
+* `wc = wgconfig.WGConfig('/etc/wireguard/wg0.conf')`
+
+#### `read_file()`
+
+*Reads the WireGuard config file from disk into memory*
+        
+#### `write_file(file)`
+
+*Writes a WireGuard config file from memory to file*
+      
+Parameters:
+* "file" (str, optional, default: None): Path of the WireGuard configuration file
+    You may also just provide the interface name. In this case the path '/etc/wireguard' is assumed along with a file extension '.conf'.
+    In case the parameter is missing, the config file defined on object initialization is used.
+
+Examples:
+* `wc.write_file()`
+* `wc.write_file('wg0')`
+* `wc.write_file('/etc/wireguard/wg0.conf')`
+
+#### `initialize_file(leading_comment)`
+
+*Empties the file and adds the interface section header*
+
+Parameters:
+* "leading_comment" (str, optional, default: None): Comment line to be added before the Interface section. Must start with a '#' to indicate a comment.
+
+Examples:
+* `wc.initialize_file()`
+* `wc.initialize_file('# Here comes the Interface section:')`
+
+#### `get_interface(include_details)`
+
+*Returns a dictionary of the attributes and values of the interface section*
+
+Parameters:
+* "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
+
+Examples:
+* `ifdata = wc.get_interface()`
+
+#### `get_peers(keys_only, include_disabled, include_details)`
+
+*Returns a list of peers or - if selected - a dictionary including peers' data*
+
+Parameters:
+* "keys_only" (boolean, optional, default: True): Return only the public keys as a list or return keys and corresponding data as a dictionary.
+* "include_disabled" (boolean, optional, default: False): Also return data of disabled peers.
+* "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
+
+Examples:
+* `peers = wc.get_peers()`
+* `peerdata = wc.get_peers(keys_only=False)`
+
+#### `get_peer(key, include_details)`
+
+*Returns the data of the peer with the given (public) key*
+
+Parameters:
+* "key" (str): Public key of the peer
+* "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
+
+Examples:
+* `peerdata = wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+* `peerdata = wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', include_details=True)`
+
+Notes:
+* Don't forget to call `read_file()` before attempting to get data out of a file
+* Access the `peers` property if you want to retrieve the data of all peers    
+
+#### `add_peer(key, leading_comment)`
+
+*Adds a new peer with the given (public) key*
+
+Parameters:
+* "key" (str): Public key of the new peer
+* "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
+
+Examples:
+* `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+* `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Here comes the Interface section:')`
+
+#### `del_peer(key)`
+
+*Removes the peer with the given (public) key*
+
+Note: Comment lines immediately before the Peer section are removed, too.
+
+Parameters:
+* "key" (str): Public key of the peer
+
+Examples:
+* `wc.del_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+
+#### `add_attr(key, attr, value, leading_comment, append_as_line)`
+
+*Adds an attribute/value pair to the given peer ('None' for adding an interface attribute)*
+
+Parameters:
+* "key" (str): Key of the peer. Set to 'None' to denote the Interface section
+* "attr" (str) Name of the attribute to add
+* "value" (str or int) Value of the attribute to add
+* "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
+* "append_as_line" (bool, optional, default: False): Whether to add the attribute as a new line if another attribute with the same name already exists. If "False", adding an attribute that already exists results in comma-separated attribute values. This way, "AllowedIPs" can be added one by one.
+
+Examples:
+* `wc.add_attr(None, 'ListenPort', '51820')`
+* `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
+* `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', '# Allow all IPv4 addresses', append_as_line=True)`
+
+#### `del_attr(self, key, attr, value, remove_leading_comments)`
+
+*Removes an attribute/value pair from the given peer ('None' for adding an interface attribute); set 'value' to 'None' to remove all values*
+
+Parameters:
+* "key" (str): Key of the peer. Set to 'None' to denote the Interface section
+* "attr" (str) Name of the attribute to remove
+* "value" (str or int, optional, default: None) Value of the attribute to remove
+    Set to 'None' if all values (either comma-separated or is multiple attribute lines) shall be removed. Otherwise specify the specific value to be removed.
+* "remove_leading_comments" (bool, optional, default: True): Indicates whether comment lines before the attribute line(s) shall be removed, too
+
+Examples:
+* `wc.del_attr(None, 'ListenPort')`
+* `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs')`
+* `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
+* `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', remove_leading_comments=False)`
+
+#### `disable_peer(self, key)`
+
+*Disables the peer with the given (public) key by prepending `#!` to all lines in a peer section*
+
+Parameters:
+* "key" (str): Public key of the peer
+
+Examples:
+* `wc.disable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+
+#### `enable_peer(self, key)`
+
+*Enables the peer with the given (public) key by removing `#!` from all lines in a peer section*
+
+Parameters:
+* "key" (str): Public key of the peer
+
+Examples:
+* `wc.enable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+
+#### `get_peer_enabled(self, key)`
+
+*Checks whether the peer with the given (public) key is enabled*
+
+Parameters:
+* "key" (str): Public key of the peer
+
+Examples:
+* `wc.get_peer_enabled('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+
+---
+
+## Reporting bugs
+
+In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
+
+---
+## Developers
+
+### Clone repository
+
+Clone this repo to your local machine using `https://github.com/towalink/wgconfig.git`
+
+Install the module temporarily to make it available in your Python installation:
+```shell
+pip3 install -e <path to root of "src" directory>
+```
+
+### Run unit tests
+
+Call "pytest" to run the unit tests:
+```shell
+pytest <path to root of "test" directory>
+```
+
+---
+
+## License
+
+[![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
+
+- **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
+- Copyright 2020-2023 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
+- [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
```

### Comparing `wgconfig-0.3.0/README.md` & `wgconfig-1.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # wgconfig
 
 Parsing and writing WireGuard configuration files (comment preserving)
 
-WireGuard config files are ini-style. Since all "Peer" sections have the same name, these files cannot be parsed and modified by most modules handling configuration files. Most existing modules are not able to preserve or even add comments when modifying a config file. "wgconfig" was created to work with WireGuard configuration files and to preserve comments.
+WireGuard config files are ini-style. Since all "Peer" sections have the same name, these files cannot be parsed and modified by most libraries handling configuration files. Most existing libraries are not able to preserve or even add comments when modifying a config file. "wgconfig" was created to work with WireGuard configuration files and to preserve comments.
 
 ---
 
 ## Features
 
-- Read and parse WireGuard configuration files and make the data available as Python dictionaries
-- Create new WireGuard configuration files
-- Add peers to WireGuard configuration files and delete peers from WireGuard configuration files
-- Save and clone WireGuard configuration files
-- Comments are preserved when reading and writing WireGuard configuration files
-- Leading comments may be added when creating sections or attributes
-- Such comments may be deleted when removing sections or attributes
-- No other modules are needed, i.e. no dependencies
+- Read and parse WireGuard configuration files and make the data available as Python dictionaries.
+- Create new WireGuard configuration files.
+- Add peers to WireGuard configuration files and delete peers from WireGuard configuration files.
+- Save and clone WireGuard configuration files.
+- Comments are preserved when reading and writing WireGuard configuration files.
+- Leading comments may be added when creating sections or attributes.
+- Such comments may be deleted when removing sections or attributes.
+- No other libraries are needed, i.e. no dependencies.
 
 ---
 
 ## Installation
 
 Install using PyPi:
 
@@ -35,16 +35,17 @@
 
 Read and parse the existing WireGuard configuration file 'wg0.conf' located in '/etc/wireguard':
 
 ```python
 import wgconfig
 wc = wgconfig.WGConfig('wg0')
 wc.read_file()
-print('INTERFACE DATA:', wc.interface)
-print('PEER DATA:', wc.peers)
+print('INTERFACE DATA:', , wc.get_interface())
+print('LIST OF PEERS:', wc.get_peers())
+print('ALL PEER DATA:', wc.get_peers(keys_only=False))
 ```
 
 Add a new peer with a comment line before the peer section:
 ```python
 wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Newly added peer')
 ```
 
@@ -68,183 +69,220 @@
 import wgconfig
 wc = wgconfig.WGConfig('/root/wgtest.conf')
 # Add attribute to Interface section (denoted by 'None')
 wc.add_attr(None, 'PrivateKey', '6FYKQKEtGFAb5HSwyj5cQl3wgS1E9d6SqVjdVksOn2s=')
 # Save to disk
 wc.write_file()
 # Access the data
-print('INTERFACE DATA:', wc.interface)
-print('PEER DATA (there are no peers yet):', wc.peers)
+print('INTERFACE DATA:', wc.get_interface())
+print('LIST OF PEERS (there are no peers yet):', wc.get_peers())
+print('ALL PEER DATA (there are no peers yet):', wc.get_peers(keys_only=False))
 ```
 
 The module also contains simple wrappers around the wg command to generate and manage keys:
 
 ```python
 import wgconfig.wgexec as wgexec
 # Create a new WireGuard private key
 private_key = wgexec.generate_privatekey()
 ```
 
-Please see below for more detailed usage information.
+More information and examples can be found here:
+
+- [Detailed example for reading WireGuard config files](https://github.com/towalink/wgconfig/blob/master/doc/example_notebook_1.md)
+- Please see the section below for detailed API description.
 
 ---
 
-## Usage / API
+## Detailed API description
 
 ### Properties
 
-* interface: Returns attributes and values of the Interface section as a dictionary
+#### interface
+
+*Returns attributes and values (including wgconfig-internal ones) of the Interface section as a dictionary*
+
+Notes:
+* You might want to use the more flexible `get_interface()` method (see further below) instead.
+
+#### peers
+
+*Returns attributes and values (including wgconfig-internal ones) of all peers as a nested dictionary*
 
-* peers: Returns attributes and values of all peers as a nested dictionary
+Notes:
+* You might want to use the more flexible `get_peers()` method (see further below) instead.
 
 ### Methods for interaction
 
-* `__init__(file)`
+#### `__init__(file)`
 
-  *Initializes the instance*
-  
-  Parameters:
-  * "file" (str): Path of the WireGuard configuration file
-      You may also just provide the interface name. In this case, the path '/etc/wireguard' is assumed along with a file extension '.conf'.
-  
-  Examples:
-  * `wc = wgconfig.WGConfig('wg0')`
-  * `wc = wgconfig.WGConfig('/etc/wireguard/wg0.conf')`
+*Initializes the instance*
 
-* `read_file()`
+Parameters:
+* "file" (str): Path of the WireGuard configuration file
+    You may also just provide the interface name. In this case, the path '/etc/wireguard' is assumed along with a file extension '.conf'.
 
-  *Reads the WireGuard config file into memory*
-        
-* `write_file(file)`
+Examples:
+* `wc = wgconfig.WGConfig('wg0')`
+* `wc = wgconfig.WGConfig('/etc/wireguard/wg0.conf')`
+
+#### `read_file()`
 
-  *Writes a WireGuard config file from memory to file*
+*Reads the WireGuard config file from disk into memory*
         
-  Parameters:
-  * "file" (str, optional, default: None): Path of the WireGuard configuration file
-      You may also just provide the interface name. In this case the path '/etc/wireguard' is assumed along with a file extension '.conf'.
-      In case the parameter is missing, the config file defined on object initialization is used.
+#### `write_file(file)`
+
+*Writes a WireGuard config file from memory to file*
+      
+Parameters:
+* "file" (str, optional, default: None): Path of the WireGuard configuration file
+    You may also just provide the interface name. In this case the path '/etc/wireguard' is assumed along with a file extension '.conf'.
+    In case the parameter is missing, the config file defined on object initialization is used.
+
+Examples:
+* `wc.write_file()`
+* `wc.write_file('wg0')`
+* `wc.write_file('/etc/wireguard/wg0.conf')`
+
+#### `initialize_file(leading_comment)`
+
+*Empties the file and adds the interface section header*
+
+Parameters:
+* "leading_comment" (str, optional, default: None): Comment line to be added before the Interface section. Must start with a '#' to indicate a comment.
+
+Examples:
+* `wc.initialize_file()`
+* `wc.initialize_file('# Here comes the Interface section:')`
+
+#### `get_interface(include_details)`
+
+*Returns a dictionary of the attributes and values of the interface section*
+
+Parameters:
+* "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
+
+Examples:
+* `ifdata = wc.get_interface()`
+
+#### `get_peers(keys_only, include_disabled, include_details)`
+
+*Returns a list of peers or - if selected - a dictionary including peers' data*
+
+Parameters:
+* "keys_only" (boolean, optional, default: True): Return only the public keys as a list or return keys and corresponding data as a dictionary.
+* "include_disabled" (boolean, optional, default: False): Also return data of disabled peers.
+* "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
+
+Examples:
+* `peers = wc.get_peers()`
+* `peerdata = wc.get_peers(keys_only=False)`
+
+#### `get_peer(key, include_details)`
+
+*Returns the data of the peer with the given (public) key*
 
-  Examples:
-  * `wc.write_file()`
-  * `wc.write_file('wg0')`
-  * `wc.write_file('/etc/wireguard/wg0.conf')`
+Parameters:
+* "key" (str): Public key of the peer
+* "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
 
-* `initialize_file(leading_comment)`
+Examples:
+* `peerdata = wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+* `peerdata = wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', include_details=True)`
 
-  *Empties the file and adds the interface section header*
+Notes:
+* Don't forget to call `read_file()` before attempting to get data out of a file
+* Access the `peers` property if you want to retrieve the data of all peers    
 
-  Parameters:
-  * "leading_comment" (str, optional, default: None): Comment line to be added before the Interface section. Must start with a '#' to indicate a comment.
+#### `add_peer(key, leading_comment)`
 
-  Examples:
-  * `wc.initialize_file()`
-  * `wc.initialize_file('# Here comes the Interface section:')`
+*Adds a new peer with the given (public) key*
 
-* `get_peer(key, include_details)`
+Parameters:
+* "key" (str): Public key of the new peer
+* "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
 
-  *Returns the data of the peer with the given (public) key*
-  
-  Parameters:
-  * "key" (str): Public key of the peer
-  * "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
+Examples:
+* `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+* `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Here comes the Interface section:')`
 
-  Examples:
-  * `wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-  * `wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', include_details = True)`
+#### `del_peer(key)`
 
-  Notes:
-  * Don't forget to call `read_file()` before attempting to get data out of a file
-  * Access the `peers` property if you want to retrieve the data of all peers    
+*Removes the peer with the given (public) key*
 
-* `add_peer(key, leading_comment)`
+Note: Comment lines immediately before the Peer section are removed, too.
 
-  *Adds a new peer with the given (public) key*
+Parameters:
+* "key" (str): Public key of the peer
 
-  Parameters:
-  * "key" (str): Public key of the new peer
-  * "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
+Examples:
+* `wc.del_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
 
-  Examples:
-  * `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-  * `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Here comes the Interface section:')`
+#### `add_attr(key, attr, value, leading_comment, append_as_line)`
 
-* `del_peer(key)`
+*Adds an attribute/value pair to the given peer ('None' for adding an interface attribute)*
 
-  *Removes the peer with the given (public) key*
-  
-  Note: Comment lines immediately before the Peer section are removed, too.
-  
-  Parameters:
-  * "key" (str): Public key of the peer
+Parameters:
+* "key" (str): Key of the peer. Set to 'None' to denote the Interface section
+* "attr" (str) Name of the attribute to add
+* "value" (str or int) Value of the attribute to add
+* "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
+* "append_as_line" (bool, optional, default: False): Whether to add the attribute as a new line if another attribute with the same name already exists. If "False", adding an attribute that already exists results in comma-separated attribute values. This way, "AllowedIPs" can be added one by one.
 
-  Examples:
-  * `wc.del_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+Examples:
+* `wc.add_attr(None, 'ListenPort', '51820')`
+* `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
+* `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', '# Allow all IPv4 addresses', append_as_line=True)`
 
-* `add_attr(key, attr, value, leading_comment, append_as_line)`
+#### `del_attr(self, key, attr, value, remove_leading_comments)`
 
-  *Adds an attribute/value pair to the given peer ('None' for adding an interface attribute)*
-  
-  Parameters:
-  * "key" (str): Key of the peer. Set to 'None' to denote the Interface section
-  * "attr" (str) Name of the attribute to add
-  * "value" (str or int) Value of the attribute to add
-  * "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
-  * "append_as_line" (bool, optional, default: False): Whether to add the attribute as a new line if another attribute with the same name already exists. If "False", adding an attribute that already exists results in comma-separated attribute values. This way, "AllowedIPs" can be added one by one.
+*Removes an attribute/value pair from the given peer ('None' for adding an interface attribute); set 'value' to 'None' to remove all values*
 
-  Examples:
-  * `wc.add_attr(None, 'ListenPort', '51820')`
-  * `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
-  * `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', '# Allow all IPv4 addresses', append_as_line=True)`
+Parameters:
+* "key" (str): Key of the peer. Set to 'None' to denote the Interface section
+* "attr" (str) Name of the attribute to remove
+* "value" (str or int, optional, default: None) Value of the attribute to remove
+    Set to 'None' if all values (either comma-separated or is multiple attribute lines) shall be removed. Otherwise specify the specific value to be removed.
+* "remove_leading_comments" (bool, optional, default: True): Indicates whether comment lines before the attribute line(s) shall be removed, too
 
-* `del_attr(self, key, attr, value, remove_leading_comments)`
+Examples:
+* `wc.del_attr(None, 'ListenPort')`
+* `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs')`
+* `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
+* `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', remove_leading_comments=False)`
 
-  *Removes an attribute/value pair from the given peer ('None' for adding an interface attribute); set 'value' to 'None' to remove all values*
+#### `disable_peer(self, key)`
 
-  Parameters:
-  * "key" (str): Key of the peer. Set to 'None' to denote the Interface section
-  * "attr" (str) Name of the attribute to remove
-  * "value" (str or int, optional, default: None) Value of the attribute to remove
-      Set to 'None' if all values (either comma-separated or is multiple attribute lines) shall be removed. Otherwise specify the specific value to be removed.
-  * "remove_leading_comments" (bool, optional, default: True): Indicates whether comment lines before the attribute line(s) shall be removed, too
+*Disables the peer with the given (public) key by prepending `#!` to all lines in a peer section*
 
-  Examples:
-  * `wc.del_attr(None, 'ListenPort')`
-  * `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs')`
-  * `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
-  * `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', remove_leading_comments=False)`
+Parameters:
+* "key" (str): Public key of the peer
 
-* `disable_peer(self, key)`
+Examples:
+* `wc.disable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
 
-  *Disables the peer with the given (public) key by prepending #! to all lines in a peer section*
+#### `enable_peer(self, key)`
 
-  Parameters:
-  * "key" (str): Public key of the peer
-  
-  Examples:
-  * `wc.disable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+*Enables the peer with the given (public) key by removing `#!` from all lines in a peer section*
 
-* `enable_peer(self, key)`
+Parameters:
+* "key" (str): Public key of the peer
 
-  *Enables the peer with the given (public) key by removing #! from all lines in a peer section*
+Examples:
+* `wc.enable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
 
-  Parameters:
-  * "key" (str): Public key of the peer
-  
-  Examples:
-  * `wc.enable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+#### `get_peer_enabled(self, key)`
 
-* `get_peer_enabled(self, key)`
+*Checks whether the peer with the given (public) key is enabled*
 
-  *Checks whether the peer with the given (public) key is enabled*
+Parameters:
+* "key" (str): Public key of the peer
 
-  Parameters:
-  * "key" (str): Public key of the peer
-  
-  Examples:
-  * `wc.get_peer_enabled('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+Examples:
+* `wc.get_peer_enabled('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
 
 ---
 
 ## Reporting bugs
 
 In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
 
@@ -270,9 +308,9 @@
 ---
 
 ## License
 
 [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
 
 - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-- Copyright 2020-2022 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
+- Copyright 2020-2023 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
 - [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
```

### Comparing `wgconfig-0.3.0/setup.py` & `wgconfig-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'wgconfig',
-    'version': '0.3.0',
+    'version': '1.0.0',
     'author': 'Dirk Henrici',
     'author_email': 'towalink.wgconfig@henrici.name',
     'description': 'parsing and writing WireGuard configuration files',
     'long_description': long_description,
     'long_description_content_type': 'text/markdown',
     'url': 'https://www.github.com/towalink/wgconfig',
     'packages': setuptools.find_packages(),
```

### Comparing `wgconfig-0.3.0/wgconfig/__init__.py` & `wgconfig-1.0.0/wgconfig/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-"""wgconfig.py: A class for parsing and writing Wireguard configuration files."""
+"""wgconfig.py: A class for parsing and writing WireGuard configuration files."""
 
 # The following imports are for Python2 support only
 from __future__ import with_statement
 from __future__ import absolute_import
 from __future__ import print_function
 from builtins import str
 from builtins import range
@@ -16,15 +16,15 @@
 __email__ = "towalink.wgconfig@henrici.name"
 
 
 import os
 
 
 class WGConfig():
-    """A class for parsing and writing Wireguard configuration files"""
+    """A class for parsing and writing WireGuard configuration files"""
     SECTION_DISABLED = '_disabled'
     SECTION_FIRSTLINE = '_index_firstline'
     SECTION_LASTLINE = '_index_lastline'
     SECTION_RAW = '_rawdata'
     _interface = None # interface attributes
     _peers = None # peer data
 
@@ -46,21 +46,21 @@
 
     def invalidate_data(self):
         """Clears the data structs"""
         self._interface = None
         self._peers = None
 
     def read_file(self):
-        """Reads the Wireguard config file into memory"""
+        """Reads the WireGuard config file into memory"""
         with open(self.filename, 'r') as wgfile:
             self.lines = [line.rstrip() for line in wgfile.readlines()]
         self.invalidate_data()
 
     def write_file(self, file=None):
-        """Writes a Wireguard config file from memory to file"""
+        """Writes a WireGuard config file from memory to file"""
         if file is None:
             filename = self.filename
         else:
             filename = self.file2filename(file)
         with os.fdopen(os.open(filename, os.O_WRONLY | os.O_CREAT | os.O_TRUNC, 0o640), 'w') as wgfile:
             wgfile.writelines(line + '\n' for line in self.lines)
 
@@ -76,15 +76,15 @@
         if value.isnumeric():
             value = [int(value)]
         else:
             value = [item.strip() for item in value.split(',')] # decompose into list based on commata as separator
         return attr, value, comment
 
     def parse_lines(self):
-        """Parses the lines of a Wireguard config file into memory"""
+        """Parses the lines of a WireGuard config file into memory"""
 
         # There will be two special attributes in the parsed data:
         #_index_firstline: Line (zero indexed) of the section header (including any leading lines with comments)
         #_index_lastline: Line (zero indexed) of the last attribute line of the section (including any directly following comments)
 
         def close_section(section, section_data):
             section_data = {k: (v if len(v) > 1 else v[0]) for k, v in section_data.items()}
@@ -147,26 +147,45 @@
     def initialize_file(self, leading_comment=None):
         """Empties the file and adds the interface section header"""
         self.lines = list()
         self.handle_leading_comment(leading_comment) # add leading comment if needed
         self.lines.append('[Interface]')
         self.invalidate_data()
 
+    def get_filtered_dictionary(self, data, include_details=False):
+        """Return a separated copy of a dictionary and filter private attributes if requested"""
+        if include_details:
+            # Obtain a copy of the complete dictionary
+            data = data.copy()
+        else:
+            # Filter attributes starting with an underscore
+            data = { key: value for key, value in data.items() if not key.startswith('_') }
+        return data    
+
+    def get_interface(self, include_details=False):
+        """Returns the data of the interface section"""
+        return self.get_filtered_dictionary(self.interface, include_details)
+
+    def get_peers(self, keys_only=True, include_disabled=False, include_details=False):
+        """Returns peer data or a list of peers (i.e. their public keys)"""
+        # Get (possibly) filtered peers dictionary
+        peerdata = { key: value for key, value in self.peers.items() if include_disabled or not value.get('_disabled', False) }
+        # Return requested data
+        if keys_only:
+            return list(peerdata.keys())
+        else:
+            return { key: self.get_filtered_dictionary(value, include_details) for key, value in peerdata.items() }
+
     def get_peer(self, key, include_details=False):
         """Returns the data of the peer with the given (public) key"""
         try:
             peerdata = self.peers[key]
         except KeyError:
             raise KeyError('The peer does not exist')
-        # Make sure to have a separated copy and filter details if needed
-        if include_details:
-            peerdata = peerdata.copy()
-        else:
-            peerdata = { key: value for key, value in peerdata.items() if not key.startswith('_') }
-        return peerdata
+        return self.get_filtered_dictionary(peerdata, include_details)
 
     def add_peer(self, key, leading_comment=None):
         """Adds a new peer with the given (public) key"""
         if key in self.peers:
             raise KeyError('Peer to be added already exists')
         self.lines.append('') # append an empty line for separation
         self.handle_leading_comment(leading_comment) # add leading comment if needed
@@ -234,15 +253,15 @@
         # Handle leading comments
         if leading_comment is not None:
             self.lines.insert(line_found, leading_comment)
         # Invalidate data cache
         self.invalidate_data()
 
     def del_attr(self, key, attr, value=None, remove_leading_comments=True):
-        """Removes an attribute/value pair from the given peer ("None" for adding an interface attribute); set 'value' to 'None' to remove all values"""
+        """Removes an attribute/value pair from the given peer ("None" for removing an interface attribute); set 'value' to 'None' to remove all values"""
         section_firstline, section_lastline = self.get_sectioninfo(key)
         # Find all lines with matching attribute name and (if requested) value
         line_found = []
         for i in range(section_firstline + 1, section_lastline + 1):
             line_attr, line_value, line_comment = self.parse_line(self.lines[i])
             if attr == line_attr:
                 if (value is None) or (value in line_value):
```

### Comparing `wgconfig-0.3.0/wgconfig/wgexec.py` & `wgconfig-1.0.0/wgconfig/wgexec.py`

 * *Files identical despite different names*

### Comparing `wgconfig-0.3.0/wgconfig.egg-info/PKG-INFO` & `wgconfig-1.0.0/wgconfig.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,300 +1,337 @@
 Metadata-Version: 2.1
 Name: wgconfig
-Version: 0.3.0
+Version: 1.0.0
 Summary: parsing and writing WireGuard configuration files
 Home-page: https://www.github.com/towalink/wgconfig
 Author: Dirk Henrici
 Author-email: towalink.wgconfig@henrici.name
-License: UNKNOWN
 Project-URL: Repository, https://www.github.com/towalink/wgconfig
 Project-URL: PyPi, https://pypi.org/project/wgconfig/
-Description: # wgconfig
-        
-        Parsing and writing WireGuard configuration files (comment preserving)
-        
-        WireGuard config files are ini-style. Since all "Peer" sections have the same name, these files cannot be parsed and modified by most modules handling configuration files. Most existing modules are not able to preserve or even add comments when modifying a config file. "wgconfig" was created to work with WireGuard configuration files and to preserve comments.
-        
-        ---
-        
-        ## Features
-        
-        - Read and parse WireGuard configuration files and make the data available as Python dictionaries
-        - Create new WireGuard configuration files
-        - Add peers to WireGuard configuration files and delete peers from WireGuard configuration files
-        - Save and clone WireGuard configuration files
-        - Comments are preserved when reading and writing WireGuard configuration files
-        - Leading comments may be added when creating sections or attributes
-        - Such comments may be deleted when removing sections or attributes
-        - No other modules are needed, i.e. no dependencies
-        
-        ---
-        
-        ## Installation
-        
-        Install using PyPi:
-        
-        ```shell
-        pip3 install wgconfig
-        ```
-        
-        ---
-        
-        ## Quickstart
-        
-        ### Reading and parsing an existing WireGuard configuration file
-        
-        Read and parse the existing WireGuard configuration file 'wg0.conf' located in '/etc/wireguard':
-        
-        ```python
-        import wgconfig
-        wc = wgconfig.WGConfig('wg0')
-        wc.read_file()
-        print('INTERFACE DATA:', wc.interface)
-        print('PEER DATA:', wc.peers)
-        ```
-        
-        Add a new peer with a comment line before the peer section:
-        ```python
-        wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Newly added peer')
-        ```
-        
-        Add an attribute to that peer:
-        ```python
-        wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'Endpoint', 'wg.example.com:51820', '# Added for demonstration purposes')
-        ```
-        
-        Write the changes to disk. Comments that were present when reading the file are preserved.
-        ```python
-        wc.write_file()
-        ```
-        
-        Please see below for more detailed usage information.
-        
-        ### Creating a new WireGuard configuration file
-        
-        Create a new WireGuard configuration file as '/root/wgtest.conf':
-        
-        ```python
-        import wgconfig
-        wc = wgconfig.WGConfig('/root/wgtest.conf')
-        # Add attribute to Interface section (denoted by 'None')
-        wc.add_attr(None, 'PrivateKey', '6FYKQKEtGFAb5HSwyj5cQl3wgS1E9d6SqVjdVksOn2s=')
-        # Save to disk
-        wc.write_file()
-        # Access the data
-        print('INTERFACE DATA:', wc.interface)
-        print('PEER DATA (there are no peers yet):', wc.peers)
-        ```
-        
-        The module also contains simple wrappers around the wg command to generate and manage keys:
-        
-        ```python
-        import wgconfig.wgexec as wgexec
-        # Create a new WireGuard private key
-        private_key = wgexec.generate_privatekey()
-        ```
-        
-        Please see below for more detailed usage information.
-        
-        ---
-        
-        ## Usage / API
-        
-        ### Properties
-        
-        * interface: Returns attributes and values of the Interface section as a dictionary
-        
-        * peers: Returns attributes and values of all peers as a nested dictionary
-        
-        ### Methods for interaction
-        
-        * `__init__(file)`
-        
-          *Initializes the instance*
-          
-          Parameters:
-          * "file" (str): Path of the WireGuard configuration file
-              You may also just provide the interface name. In this case, the path '/etc/wireguard' is assumed along with a file extension '.conf'.
-          
-          Examples:
-          * `wc = wgconfig.WGConfig('wg0')`
-          * `wc = wgconfig.WGConfig('/etc/wireguard/wg0.conf')`
-        
-        * `read_file()`
-        
-          *Reads the WireGuard config file into memory*
-                
-        * `write_file(file)`
-        
-          *Writes a WireGuard config file from memory to file*
-                
-          Parameters:
-          * "file" (str, optional, default: None): Path of the WireGuard configuration file
-              You may also just provide the interface name. In this case the path '/etc/wireguard' is assumed along with a file extension '.conf'.
-              In case the parameter is missing, the config file defined on object initialization is used.
-        
-          Examples:
-          * `wc.write_file()`
-          * `wc.write_file('wg0')`
-          * `wc.write_file('/etc/wireguard/wg0.conf')`
-        
-        * `initialize_file(leading_comment)`
-        
-          *Empties the file and adds the interface section header*
-        
-          Parameters:
-          * "leading_comment" (str, optional, default: None): Comment line to be added before the Interface section. Must start with a '#' to indicate a comment.
-        
-          Examples:
-          * `wc.initialize_file()`
-          * `wc.initialize_file('# Here comes the Interface section:')`
-        
-        * `get_peer(key, include_details)`
-        
-          *Returns the data of the peer with the given (public) key*
-          
-          Parameters:
-          * "key" (str): Public key of the peer
-          * "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
-        
-          Examples:
-          * `wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-          * `wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', include_details = True)`
-        
-          Notes:
-          * Don't forget to call `read_file()` before attempting to get data out of a file
-          * Access the `peers` property if you want to retrieve the data of all peers    
-        
-        * `add_peer(key, leading_comment)`
-        
-          *Adds a new peer with the given (public) key*
-        
-          Parameters:
-          * "key" (str): Public key of the new peer
-          * "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
-        
-          Examples:
-          * `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-          * `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Here comes the Interface section:')`
-        
-        * `del_peer(key)`
-        
-          *Removes the peer with the given (public) key*
-          
-          Note: Comment lines immediately before the Peer section are removed, too.
-          
-          Parameters:
-          * "key" (str): Public key of the peer
-        
-          Examples:
-          * `wc.del_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-        
-        * `add_attr(key, attr, value, leading_comment, append_as_line)`
-        
-          *Adds an attribute/value pair to the given peer ('None' for adding an interface attribute)*
-          
-          Parameters:
-          * "key" (str): Key of the peer. Set to 'None' to denote the Interface section
-          * "attr" (str) Name of the attribute to add
-          * "value" (str or int) Value of the attribute to add
-          * "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
-          * "append_as_line" (bool, optional, default: False): Whether to add the attribute as a new line if another attribute with the same name already exists. If "False", adding an attribute that already exists results in comma-separated attribute values. This way, "AllowedIPs" can be added one by one.
-        
-          Examples:
-          * `wc.add_attr(None, 'ListenPort', '51820')`
-          * `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
-          * `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', '# Allow all IPv4 addresses', append_as_line=True)`
-        
-        * `del_attr(self, key, attr, value, remove_leading_comments)`
-        
-          *Removes an attribute/value pair from the given peer ('None' for adding an interface attribute); set 'value' to 'None' to remove all values*
-        
-          Parameters:
-          * "key" (str): Key of the peer. Set to 'None' to denote the Interface section
-          * "attr" (str) Name of the attribute to remove
-          * "value" (str or int, optional, default: None) Value of the attribute to remove
-              Set to 'None' if all values (either comma-separated or is multiple attribute lines) shall be removed. Otherwise specify the specific value to be removed.
-          * "remove_leading_comments" (bool, optional, default: True): Indicates whether comment lines before the attribute line(s) shall be removed, too
-        
-          Examples:
-          * `wc.del_attr(None, 'ListenPort')`
-          * `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs')`
-          * `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
-          * `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', remove_leading_comments=False)`
-        
-        * `disable_peer(self, key)`
-        
-          *Disables the peer with the given (public) key by prepending #! to all lines in a peer section*
-        
-          Parameters:
-          * "key" (str): Public key of the peer
-          
-          Examples:
-          * `wc.disable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-        
-        * `enable_peer(self, key)`
-        
-          *Enables the peer with the given (public) key by removing #! from all lines in a peer section*
-        
-          Parameters:
-          * "key" (str): Public key of the peer
-          
-          Examples:
-          * `wc.enable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-        
-        * `get_peer_enabled(self, key)`
-        
-          *Checks whether the peer with the given (public) key is enabled*
-        
-          Parameters:
-          * "key" (str): Public key of the peer
-          
-          Examples:
-          * `wc.get_peer_enabled('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
-        
-        ---
-        
-        ## Reporting bugs
-        
-        In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
-        
-        ---
-        ## Developers
-        
-        ### Clone repository
-        
-        Clone this repo to your local machine using `https://github.com/towalink/wgconfig.git`
-        
-        Install the module temporarily to make it available in your Python installation:
-        ```shell
-        pip3 install -e <path to root of "src" directory>
-        ```
-        
-        ### Run unit tests
-        
-        Call "pytest" to run the unit tests:
-        ```shell
-        pytest <path to root of "test" directory>
-        ```
-        
-        ---
-        
-        ## License
-        
-        [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
-        
-        - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-        - Copyright 2020-2022 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
-        - [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
-        
 Keywords: WireGuard configuration config wg
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# wgconfig
+
+Parsing and writing WireGuard configuration files (comment preserving)
+
+WireGuard config files are ini-style. Since all "Peer" sections have the same name, these files cannot be parsed and modified by most libraries handling configuration files. Most existing libraries are not able to preserve or even add comments when modifying a config file. "wgconfig" was created to work with WireGuard configuration files and to preserve comments.
+
+---
+
+## Features
+
+- Read and parse WireGuard configuration files and make the data available as Python dictionaries.
+- Create new WireGuard configuration files.
+- Add peers to WireGuard configuration files and delete peers from WireGuard configuration files.
+- Save and clone WireGuard configuration files.
+- Comments are preserved when reading and writing WireGuard configuration files.
+- Leading comments may be added when creating sections or attributes.
+- Such comments may be deleted when removing sections or attributes.
+- No other libraries are needed, i.e. no dependencies.
+
+---
+
+## Installation
+
+Install using PyPi:
+
+```shell
+pip3 install wgconfig
+```
+
+---
+
+## Quickstart
+
+### Reading and parsing an existing WireGuard configuration file
+
+Read and parse the existing WireGuard configuration file 'wg0.conf' located in '/etc/wireguard':
+
+```python
+import wgconfig
+wc = wgconfig.WGConfig('wg0')
+wc.read_file()
+print('INTERFACE DATA:', , wc.get_interface())
+print('LIST OF PEERS:', wc.get_peers())
+print('ALL PEER DATA:', wc.get_peers(keys_only=False))
+```
+
+Add a new peer with a comment line before the peer section:
+```python
+wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Newly added peer')
+```
+
+Add an attribute to that peer:
+```python
+wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'Endpoint', 'wg.example.com:51820', '# Added for demonstration purposes')
+```
+
+Write the changes to disk. Comments that were present when reading the file are preserved.
+```python
+wc.write_file()
+```
+
+Please see below for more detailed usage information.
+
+### Creating a new WireGuard configuration file
+
+Create a new WireGuard configuration file as '/root/wgtest.conf':
+
+```python
+import wgconfig
+wc = wgconfig.WGConfig('/root/wgtest.conf')
+# Add attribute to Interface section (denoted by 'None')
+wc.add_attr(None, 'PrivateKey', '6FYKQKEtGFAb5HSwyj5cQl3wgS1E9d6SqVjdVksOn2s=')
+# Save to disk
+wc.write_file()
+# Access the data
+print('INTERFACE DATA:', wc.get_interface())
+print('LIST OF PEERS (there are no peers yet):', wc.get_peers())
+print('ALL PEER DATA (there are no peers yet):', wc.get_peers(keys_only=False))
+```
+
+The module also contains simple wrappers around the wg command to generate and manage keys:
+
+```python
+import wgconfig.wgexec as wgexec
+# Create a new WireGuard private key
+private_key = wgexec.generate_privatekey()
+```
+
+More information and examples can be found here:
+
+- [Detailed example for reading WireGuard config files](https://github.com/towalink/wgconfig/blob/master/doc/example_notebook_1.md)
+- Please see the section below for detailed API description.
+
+---
+
+## Detailed API description
+
+### Properties
+
+#### interface
+
+*Returns attributes and values (including wgconfig-internal ones) of the Interface section as a dictionary*
+
+Notes:
+* You might want to use the more flexible `get_interface()` method (see further below) instead.
+
+#### peers
+
+*Returns attributes and values (including wgconfig-internal ones) of all peers as a nested dictionary*
+
+Notes:
+* You might want to use the more flexible `get_peers()` method (see further below) instead.
+
+### Methods for interaction
+
+#### `__init__(file)`
+
+*Initializes the instance*
+
+Parameters:
+* "file" (str): Path of the WireGuard configuration file
+    You may also just provide the interface name. In this case, the path '/etc/wireguard' is assumed along with a file extension '.conf'.
+
+Examples:
+* `wc = wgconfig.WGConfig('wg0')`
+* `wc = wgconfig.WGConfig('/etc/wireguard/wg0.conf')`
+
+#### `read_file()`
+
+*Reads the WireGuard config file from disk into memory*
+        
+#### `write_file(file)`
+
+*Writes a WireGuard config file from memory to file*
+      
+Parameters:
+* "file" (str, optional, default: None): Path of the WireGuard configuration file
+    You may also just provide the interface name. In this case the path '/etc/wireguard' is assumed along with a file extension '.conf'.
+    In case the parameter is missing, the config file defined on object initialization is used.
+
+Examples:
+* `wc.write_file()`
+* `wc.write_file('wg0')`
+* `wc.write_file('/etc/wireguard/wg0.conf')`
+
+#### `initialize_file(leading_comment)`
+
+*Empties the file and adds the interface section header*
+
+Parameters:
+* "leading_comment" (str, optional, default: None): Comment line to be added before the Interface section. Must start with a '#' to indicate a comment.
+
+Examples:
+* `wc.initialize_file()`
+* `wc.initialize_file('# Here comes the Interface section:')`
+
+#### `get_interface(include_details)`
+
+*Returns a dictionary of the attributes and values of the interface section*
+
+Parameters:
+* "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
+
+Examples:
+* `ifdata = wc.get_interface()`
+
+#### `get_peers(keys_only, include_disabled, include_details)`
+
+*Returns a list of peers or - if selected - a dictionary including peers' data*
+
+Parameters:
+* "keys_only" (boolean, optional, default: True): Return only the public keys as a list or return keys and corresponding data as a dictionary.
+* "include_disabled" (boolean, optional, default: False): Also return data of disabled peers.
+* "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
+
+Examples:
+* `peers = wc.get_peers()`
+* `peerdata = wc.get_peers(keys_only=False)`
+
+#### `get_peer(key, include_details)`
+
+*Returns the data of the peer with the given (public) key*
+
+Parameters:
+* "key" (str): Public key of the peer
+* "include_details" (boolean, optional, default: False): Also include attributes with a leading underscore (e.g. the disabled state or the raw data).
+
+Examples:
+* `peerdata = wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+* `peerdata = wc.get_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', include_details=True)`
+
+Notes:
+* Don't forget to call `read_file()` before attempting to get data out of a file
+* Access the `peers` property if you want to retrieve the data of all peers    
+
+#### `add_peer(key, leading_comment)`
+
+*Adds a new peer with the given (public) key*
+
+Parameters:
+* "key" (str): Public key of the new peer
+* "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
+
+Examples:
+* `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+* `wc.add_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', '# Here comes the Interface section:')`
+
+#### `del_peer(key)`
+
+*Removes the peer with the given (public) key*
+
+Note: Comment lines immediately before the Peer section are removed, too.
+
+Parameters:
+* "key" (str): Public key of the peer
+
+Examples:
+* `wc.del_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+
+#### `add_attr(key, attr, value, leading_comment, append_as_line)`
+
+*Adds an attribute/value pair to the given peer ('None' for adding an interface attribute)*
+
+Parameters:
+* "key" (str): Key of the peer. Set to 'None' to denote the Interface section
+* "attr" (str) Name of the attribute to add
+* "value" (str or int) Value of the attribute to add
+* "leading_comment" (str, optional, default: None): Comment line to be added before the Peer section. Must start with a '#' to indicate a comment.
+* "append_as_line" (bool, optional, default: False): Whether to add the attribute as a new line if another attribute with the same name already exists. If "False", adding an attribute that already exists results in comma-separated attribute values. This way, "AllowedIPs" can be added one by one.
+
+Examples:
+* `wc.add_attr(None, 'ListenPort', '51820')`
+* `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
+* `wc.add_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', '# Allow all IPv4 addresses', append_as_line=True)`
+
+#### `del_attr(self, key, attr, value, remove_leading_comments)`
+
+*Removes an attribute/value pair from the given peer ('None' for adding an interface attribute); set 'value' to 'None' to remove all values*
+
+Parameters:
+* "key" (str): Key of the peer. Set to 'None' to denote the Interface section
+* "attr" (str) Name of the attribute to remove
+* "value" (str or int, optional, default: None) Value of the attribute to remove
+    Set to 'None' if all values (either comma-separated or is multiple attribute lines) shall be removed. Otherwise specify the specific value to be removed.
+* "remove_leading_comments" (bool, optional, default: True): Indicates whether comment lines before the attribute line(s) shall be removed, too
+
+Examples:
+* `wc.del_attr(None, 'ListenPort')`
+* `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs')`
+* `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0')`
+* `wc.del_attr('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=', 'AllowedIPs', '0.0.0.0/0', remove_leading_comments=False)`
+
+#### `disable_peer(self, key)`
+
+*Disables the peer with the given (public) key by prepending `#!` to all lines in a peer section*
+
+Parameters:
+* "key" (str): Public key of the peer
+
+Examples:
+* `wc.disable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+
+#### `enable_peer(self, key)`
+
+*Enables the peer with the given (public) key by removing `#!` from all lines in a peer section*
+
+Parameters:
+* "key" (str): Public key of the peer
+
+Examples:
+* `wc.enable_peer('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+
+#### `get_peer_enabled(self, key)`
+
+*Checks whether the peer with the given (public) key is enabled*
+
+Parameters:
+* "key" (str): Public key of the peer
+
+Examples:
+* `wc.get_peer_enabled('801mgm2JhjTOCxfihEknzFJGYxDvi+8oVYBrWe3hOWM=')`
+
+---
+
+## Reporting bugs
+
+In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
+
+---
+## Developers
+
+### Clone repository
+
+Clone this repo to your local machine using `https://github.com/towalink/wgconfig.git`
+
+Install the module temporarily to make it available in your Python installation:
+```shell
+pip3 install -e <path to root of "src" directory>
+```
+
+### Run unit tests
+
+Call "pytest" to run the unit tests:
+```shell
+pytest <path to root of "test" directory>
+```
+
+---
+
+## License
+
+[![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
+
+- **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
+- Copyright 2020-2023 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
+- [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
```

