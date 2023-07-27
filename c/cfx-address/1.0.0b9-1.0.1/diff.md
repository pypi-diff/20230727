# Comparing `tmp/cfx-address-1.0.0b9.tar.gz` & `tmp/cfx-address-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfx-address-1.0.0b9.tar", last modified: Mon Sep 26 07:33:29 2022, max compression
+gzip compressed data, was "cfx-address-1.0.1.tar", last modified: Thu Jul 27 07:00:38 2023, max compression
```

## Comparing `cfx-address-1.0.0b9.tar` & `cfx-address-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2022-09-26 07:33:29.666116 cfx-address-1.0.0b9/
--rw-r--r--   0 conflux-y   (501) staff       (20)     3815 2022-09-26 07:33:29.665333 cfx-address-1.0.0b9/PKG-INFO
--rw-r--r--   0 conflux-y   (501) staff       (20)     3168 2022-08-19 06:55:26.000000 cfx-address-1.0.0b9/README.md
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2022-09-26 07:33:29.635846 cfx-address-1.0.0b9/cfx_address/
--rw-r--r--   0 conflux-y   (501) staff       (20)      323 2022-09-26 06:54:16.000000 cfx-address-1.0.0b9/cfx_address/__init__.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     2677 2022-09-26 07:01:14.000000 cfx-address-1.0.0b9/cfx_address/_utils.py
--rw-r--r--   0 conflux-y   (501) staff       (20)    25095 2022-09-26 06:56:04.000000 cfx-address-1.0.0b9/cfx_address/address.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     1649 2022-08-19 06:55:26.000000 cfx-address-1.0.0b9/cfx_address/base32.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      344 2022-08-19 06:55:26.000000 cfx-address-1.0.0b9/cfx_address/consts.py
--rw-r--r--   0 conflux-y   (501) staff       (20)      631 2022-08-19 06:55:26.000000 cfx-address-1.0.0b9/cfx_address/types.py
--rw-r--r--   0 conflux-y   (501) staff       (20)     3849 2022-09-26 06:53:53.000000 cfx-address-1.0.0b9/cfx_address/utils.py
-drwxr-xr-x   0 conflux-y   (501) staff       (20)        0 2022-09-26 07:33:29.661308 cfx-address-1.0.0b9/cfx_address.egg-info/
--rw-r--r--   0 conflux-y   (501) staff       (20)     3815 2022-09-26 07:33:29.000000 cfx-address-1.0.0b9/cfx_address.egg-info/PKG-INFO
--rw-r--r--   0 conflux-y   (501) staff       (20)      347 2022-09-26 07:33:29.000000 cfx-address-1.0.0b9/cfx_address.egg-info/SOURCES.txt
--rw-r--r--   0 conflux-y   (501) staff       (20)        1 2022-09-26 07:33:29.000000 cfx-address-1.0.0b9/cfx_address.egg-info/dependency_links.txt
--rw-r--r--   0 conflux-y   (501) staff       (20)      255 2022-09-26 07:33:29.000000 cfx-address-1.0.0b9/cfx_address.egg-info/requires.txt
--rw-r--r--   0 conflux-y   (501) staff       (20)       12 2022-09-26 07:33:29.000000 cfx-address-1.0.0b9/cfx_address.egg-info/top_level.txt
--rw-r--r--   0 conflux-y   (501) staff       (20)       38 2022-09-26 07:33:29.669568 cfx-address-1.0.0b9/setup.cfg
--rw-r--r--   0 conflux-y   (501) staff       (20)     2597 2022-09-26 07:17:41.000000 cfx-address-1.0.0b9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:00:38.248172 cfx-address-1.0.1/
+-rw-rw-rw-   0        0        0     3820 2023-07-27 07:00:38.248172 cfx-address-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3098 2023-07-27 06:48:32.000000 cfx-address-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 07:00:38.216258 cfx-address-1.0.1/cfx_address/
+-rw-rw-rw-   0        0        0      323 2023-07-27 03:42:53.000000 cfx-address-1.0.1/cfx_address/__init__.py
+-rw-rw-rw-   0        0        0     2933 2023-07-27 03:42:53.000000 cfx-address-1.0.1/cfx_address/_utils.py
+-rw-rw-rw-   0        0        0    32579 2023-07-27 06:42:51.000000 cfx-address-1.0.1/cfx_address/address.py
+-rw-rw-rw-   0        0        0     1649 2023-07-27 03:42:53.000000 cfx-address-1.0.1/cfx_address/base32.py
+-rw-rw-rw-   0        0        0      344 2023-07-27 03:42:53.000000 cfx-address-1.0.1/cfx_address/consts.py
+-rw-rw-rw-   0        0        0        0 2023-07-27 03:42:53.000000 cfx-address-1.0.1/cfx_address/py.typed
+-rw-rw-rw-   0        0        0      631 2023-07-27 03:42:53.000000 cfx-address-1.0.1/cfx_address/types.py
+-rw-rw-rw-   0        0        0     4158 2023-07-27 03:42:53.000000 cfx-address-1.0.1/cfx_address/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:00:38.246178 cfx-address-1.0.1/cfx_address.egg-info/
+-rw-rw-rw-   0        0        0     3820 2023-07-27 07:00:38.000000 cfx-address-1.0.1/cfx_address.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-27 07:00:38.000000 cfx-address-1.0.1/cfx_address.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 07:00:38.000000 cfx-address-1.0.1/cfx_address.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      314 2023-07-27 07:00:38.000000 cfx-address-1.0.1/cfx_address.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-27 07:00:38.000000 cfx-address-1.0.1/cfx_address.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      317 2023-07-27 03:42:53.000000 cfx-address-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 07:00:38.249169 cfx-address-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2756 2023-07-27 06:52:08.000000 cfx-address-1.0.1/setup.py
```

### Comparing `cfx-address-1.0.0b9/PKG-INFO` & `cfx-address-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,133 +1,127 @@
-Metadata-Version: 2.1
-Name: cfx-address
-Version: 1.0.0b9
-Summary: UNKNOWN
-Home-page: UNKNOWN
-Author: The Conflux foundation
-Author-email: wangpan@conflux-chain.org
-License: UNKNOWN
-Keywords: Conflux,base32,address
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-Provides-Extra: tester
-Provides-Extra: linter
-Provides-Extra: docs
-Provides-Extra: dev
-
-# cfx-address
-
-Conflux base32 address utilities
-
-Full documentation -> https://conflux-fans.github.io/cfx-address/cfx_address.html#module-cfx_address
-
-## installation
-
-```bash
-pip install cfx-address
-```
-
-### use Base32Address class methods
-
-```python
-from cfx_address import Base32Address
-```
-
-#### validate a base32 address
-``` python
-Base32Address.is_valid_base32("0x1ecde7223747601823f7535d7968ba98b4881e09") 
-# False
-Base32Address.validate("0x1ecde7223747601823f7535d7968ba98b4881e09")
-# will raise an exception
-```
-
-#### encode and decode
-
-``` python
-# encode hex address to base32
-Base32Address.encode("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1)
-#'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
-
-# decode base32 address
-Base32Address.decode("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
-# result:
-# {'network_id': 1,
-# 'hex_address': '0x1ecde7223747601823f7535d7968ba98b4881e09',
-# 'address_type': 'user'}
-```
-
-#### utilities
-
-```python
-address_str = "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4"
-address_verbose_str = "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4"
-assert Base32Address.equals(address_str, address_verbose_str)
-
-Base32Address.calculate_mapped_evm_space_address(address_str)
-Base32Address.zero_address(network_id=1)
-Base32Address.shorten_base32_address(address_str)
-```
-
-### Base32Address instances
-
-#### instance initialization
-
-```python
-address = Base32Address("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
-# 'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
-
-# Base32Address inherits from str
-assert isinstance(address, str)
-
-# init from hex address, in which case network_id is required
-Base32Address("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1029)
-# 'cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu'
-
-# change a base32 address to other network
-Base32Address(address, network_id=1029)
-# 'cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu'
-
-# verbose option defaults to False
-Base32Address(address, verbose=True)
-# 'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4'
-```
-
-#### __eq__ and properties
-
-```python
-# __eq__ is implemented, address in same network is treated equal
-assert address == "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4"
-assert address == "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4"
-assert "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4" == address
-assert "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4" == address
-
-# address in different network is not equal
-mainnet_address = Base32Address(address, 1029)
-assert mainnet_address == "cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu"
-assert not address == mainnet_address
-
-# properties
-[
-    address.address_type,
-    address.network_id,
-    address.hex_address,
-    address.verbose_address,
-    address.short,
-    address.mapped_evm_space_address
-    address.eth_checksum_address
-]
-# ['user',
-#  1,
-#  '0x1ecde7223747601823f7535d7968ba98b4881e09',
-#  'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4',
-#  'cfxtest:aat...95j4',
-#  '0x349f086998cF4a0C5a00b853a0E93239D81A97f6',
-#  '0x1ECdE7223747601823f7535d7968Ba98b4881E09']
-```
-
-
+Metadata-Version: 2.1
+Name: cfx-address
+Version: 1.0.1
+Author: The Conflux foundation
+Author-email: wangpan@conflux-chain.org
+Keywords: Conflux,base32,address
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Education
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: tester
+Provides-Extra: linter
+Provides-Extra: docs
+Provides-Extra: dev
+
+# cfx-address
+
+Conflux base32 address utilities
+
+Full documentation -> https://conflux-fans.github.io/cfx-address/cfx_address.html#module-cfx_address
+
+## installation
+
+```bash
+pip install cfx-address
+```
+
+### use Base32Address class methods
+
+```python
+from cfx_address import Base32Address
+```
+
+#### validate a base32 address
+``` python
+Base32Address.is_valid_base32("0x1ecde7223747601823f7535d7968ba98b4881e09") 
+# False
+Base32Address.validate("0x1ecde7223747601823f7535d7968ba98b4881e09")
+# will raise an exception
+```
+
+#### encode and decode
+
+``` python
+# encode hex address to base32
+Base32Address.encode_base32("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1)
+#'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
+
+# decode base32 address
+Base32Address.decode("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
+# result:
+# {'network_id': 1,
+# 'hex_address': '0x1ecde7223747601823f7535d7968ba98b4881e09',
+# 'address_type': 'user'}
+```
+
+#### utilities
+
+```python
+address_str = "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4"
+address_verbose_str = "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4"
+assert Base32Address.equals(address_str, address_verbose_str)
+
+Base32Address.calculate_mapped_evm_space_address(address_str)
+Base32Address.zero_address(network_id=1)
+Base32Address.shorten_base32_address(address_str)
+```
+
+### Base32Address instances
+
+#### instance initialization
+
+```python
+address = Base32Address("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
+# 'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
+
+# Base32Address inherits from str
+assert isinstance(address, str)
+
+# init from hex address, in which case network_id is required
+Base32Address("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1029)
+# 'cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu'
+
+# change a base32 address to other network
+Base32Address(address, network_id=1029)
+# 'cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu'
+
+# verbose option defaults to False
+Base32Address(address, verbose=True)
+# 'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4'
+```
+
+#### __eq__ and properties
+
+```python
+# __eq__ is implemented, address in same network is treated equal
+assert address == "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4"
+assert address == "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4"
+assert "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4" == address
+assert "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4" == address
+
+# address in different network is not equal
+mainnet_address = Base32Address(address, 1029)
+assert mainnet_address == "cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu"
+assert not address == mainnet_address
+
+# properties
+[
+    address.address_type,
+    address.network_id,
+    address.hex_address,
+    address.verbose_address,
+    address.short,
+    address.mapped_evm_space_address
+]
+# ['user',
+#  1,
+#  '0x1ECdE7223747601823f7535d7968Ba98b4881E09',
+#  'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4',
+#  'cfxtest:aat...95j4',
+#  '0x349f086998cF4a0C5a00b853a0E93239D81A97f6',
+#  ]
+```
```

### Comparing `cfx-address-1.0.0b9/README.md` & `cfx-address-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # will raise an exception
 ```
 
 #### encode and decode
 
 ``` python
 # encode hex address to base32
-Base32Address.encode("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1)
+Base32Address.encode_base32("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1)
 #'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
 
 # decode base32 address
 Base32Address.decode("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
 # result:
 # {'network_id': 1,
 # 'hex_address': '0x1ecde7223747601823f7535d7968ba98b4881e09',
@@ -93,17 +93,16 @@
 [
     address.address_type,
     address.network_id,
     address.hex_address,
     address.verbose_address,
     address.short,
     address.mapped_evm_space_address
-    address.eth_checksum_address
 ]
 # ['user',
 #  1,
-#  '0x1ecde7223747601823f7535d7968ba98b4881e09',
+#  '0x1ECdE7223747601823f7535d7968Ba98b4881E09',
 #  'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4',
 #  'cfxtest:aat...95j4',
 #  '0x349f086998cF4a0C5a00b853a0E93239D81A97f6',
-#  '0x1ECdE7223747601823f7535d7968Ba98b4881E09']
+#  ]
 ```
```

### Comparing `cfx-address-1.0.0b9/cfx_address/_utils.py` & `cfx-address-1.0.1/cfx_address/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # utils do not rely on other modules are defined here to avoid recursive import
 from typing import (
     Any,
-    Literal,
     Union,
     cast,
 )
+from typing_extensions import (
+    Literal
+)
 from hexbytes import (
     HexBytes,
 )
 
 from cfx_utils.exceptions import (
     InvalidNetworkId,
     InvalidHexAddress, 
@@ -26,14 +28,18 @@
 
 def public_key_to_cfx_hex(public_key: Union[str, bytes]) -> HexAddress:
     """
     return the corresponding hex address of a public key in conflux: "0x1" + keccak(pk).hex()[-39]
     
     :param Union[str, bytes] public_key: str or bytes representation of public key
     :return HexAddress: Hex representation of the correspondign hex address
+    
+    
+    >>> public_key_to_cfx_hex("0xdacdaeba8e391e7649d3ac4b5329ca0e202d38facd928d88b5f729b89a497e43cc4ad3816fcfdb241497b3b43862afb4c899bc284bf60feca4ee66ff868d1feb")
+    '0x152d251c36aec31072b90a85b95bf9435b07edb8'
     """    
     public_key = HexBytes(public_key)
     # only EOA has a corresponding public key
     address = "0x1" + keccak(public_key).hex()[-39:]
     return cast(HexAddress, address)
 
 def eth_eoa_address_to_cfx_hex(eoa_address: str) -> HexAddress:
```

### Comparing `cfx-address-1.0.0b9/cfx_address/address.py` & `cfx-address-1.0.1/cfx_address/address.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import (
     Any,
-    Literal,
-    Optional, 
+    Optional,
+    Type, 
     Union,
     cast,
-    get_args
+    ClassVar
 )
-
-import functools
-from ctypes import (
-    ArgumentError
+import warnings
+from typing_extensions import (
+    Literal,
+    get_args,
 )
 
+import sys
+
 from hexbytes import (
     HexBytes
 )
 from eth_typing.evm import (
     ChecksumAddress,
     HexAddress,
 )
@@ -63,43 +65,96 @@
     VERSION_BYTE,
     CHECKSUM_TEMPLATE,
 )
 from cfx_address._utils import (
     public_key_to_cfx_hex
 )
 
+default = object()
+
+if sys.version_info >= (3, 8):
+    from functools import cached_property
+else:
+    from cached_property import cached_property
+
+class Base32AddressMeta(type):
+    """
+    This is the metaclass of Base32Address to add a setter to class variable :attr:`Base32Address.default_network_id`
+    """    
+    @property
+    def default_network_id(self) -> Union[int, None]:
+        """
+        Refer to :attr:`Base32Address.default_network_id` for the document
+        """ 
+        return self._default_network_id
+    
+    @default_network_id.setter
+    def default_network_id(cls, new_default: Union[None, int]) -> None: 
+        if new_default is not None:
+            validate_network_id(new_default)
+        cls._default_network_id = new_default
 
-class Base32Address(str):
+class Base32Address(str, metaclass=Base32AddressMeta):
     """
-    Class Base32Address can be used to create Base32Address instances and provides useful class methods to deal with base32 format addresses.
-    ## Base32Address inherits from str, so the Base32Address can be trivially used as strings
+    This class can be used to create Base32Address instances and provides useful class methods to deal with base32 format addresses.
+    :class:`~Base32Address` inherits from str, so the Base32Address can be trivially used as strings
     
     :examples:
     
     >>> address = Base32Address("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1)
     >>> address
     'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
     >>> [
     ...     address.address_type,
     ...     address.network_id,
     ...     address.hex_address,
     ...     address.verbose_address,
     ...     address.abbr,
     ...     address.mapped_evm_space_address,
-    ...     address.eth_checksum_address,
     ... ]
-    ['user', 1, '0x1ecde7223747601823f7535d7968ba98b4881e09', 'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4', 'cfxtest:aat...95j4', '0x349f086998cF4a0C5a00b853a0E93239D81A97f6', '0x1ECdE7223747601823f7535d7968Ba98b4881E09']
-    """    
+    ['user', 1, '0x1ECdE7223747601823f7535d7968Ba98b4881E09', 'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4', 'cfxtest:aat...95j4', '0x349f086998cF4a0C5a00b853a0E93239D81A97f6']
+    """
     
-    def __new__(cls, address: Union["Base32Address", HexAddress, str], network_id: Optional[int]=None, verbose: Optional[bool] = None, _from_trust: bool = False) -> "Base32Address":
+    _default_network_id: ClassVar[Optional[int]] = None
+    default_network_id: ClassVar[Optional[int]]
+    """
+    | Default network id of Base32Address. :meth:`~Base32Address`, :meth:`~Base32Address.encode`, 
+        and :meth:`~Base32Address.zero_address` will use this variable if `network_id` parameter is not specified.
+    | For most cases, it is recommended not to directly set this variable but use 
+        :meth:`~cfx_address.address.get_base32_address_factory` to set :attr:`Base32Address.default_network_id`
+    | The setter is implemented in the metaclass :class:`cfx_address.address.Base32AddressMeta`
+
+    :param Union[None,int] new_default: new default network id, could be None or positive int
+    :raises InvalidNetworkId: the new_default value is not a positive integer
+    :examples:
+    
+    >>> Base32Address.zero_address()
+    Traceback (most recent call last):
+        ...
+    cfx_utils.exceptions.InvalidNetworkId: Expected network_id to be a positive integer. Receives None of type <class 'NoneType'>
+    >>> from cfx_address.address import get_base32_address_factory
+    >>> base32_address_factory = get_base32_address_factory(default_network_id=1)
+    >>> base32_address_factory.zero_address()
+    'cfxtest:aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa6f0vrcsw'
+    >>> base32_address_factory.default_network_id = 1029
+    >>> base32_address_factory.zero_address()
+    'cfx:aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa0sfbnjm2'
+    >>> base32_address_factory.default_network_id = 2.5
+    Traceback (most recent call last):
+        ...
+    cfx_utils.exceptions.InvalidNetworkId: Expected network_id to be a positive integer. Receives 2.5 of type <class 'float'>
+    """ 
+    
+    def __new__(cls, address: Union["Base32Address", HexAddress, str], network_id: Optional[int]=cast(int, default), verbose: Optional[bool] = None, *, _from_trust: bool = False, _ignore_invalid_type: bool = False) -> "Base32Address":
         """
-        :param Union[Base32Address, HexAddress, str] address: a base32-or-hex format address
-        :param Optional[int] network_id: target address network_id. Optional if first argument is a base32 address, but required for hex address
+        :param Union[Base32Address,HexAddress,str] address: a base32-or-hex format address
+        :param Optional[int] network_id: target network_id of the address, defaults to :attr:`~default_network_id`. Can be None if first argument is a base32 address, which means don't change network id
         :param Optional[bool] verbose: whether the return value will be encoded in verbose mode, defaults to None (will be viewed as None)
         :param bool _from_trust: whether the value is a verified Base32Address, if true, network_id and verbose option should be None, and the verification and encoding process will be skipped. Not recommended to set unless preformance is critical. Defaults to False
+        :param bool _ignore_invalid_type: whether the address type is validated, defaults to False
         :raises InvalidAddress: address is neither base32 address nor hex address
         :raises InvalidNetworkId: network_id argument is not a positive integer or is None when address argument is a hex address
         :return Base32Address: an encoded base32 object, which can be trivially used as python str, specially, if from_trusted_source is true, the input value will be directly used as the encoded value
         
         :examples:
         
         >>> address = Base32Address("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1)
@@ -107,210 +162,264 @@
         'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
         >>> address_ = Base32Address(address, network_id=1029, verbose=True)
         >>> address_
         'CFX:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE7GGP3VPU'
         >>> isinstance(address_, str)
         True
         """
+        if network_id is default:
+            # if network_id is not specified (default),
+            # # network_id will be cls.default_network_id, which defaults to None
+            network_id = cls.default_network_id
+        # if _from_trust is True, 
+        # it requires network_id is None and verbose is None
+        # the new Base32Address will be initialized without validating, which means you can do
+        # Base32Address("hello world", network_id=None, verbose=None, _from_trust=True)
+        # so this API should be used carefully 
         if _from_trust:
-            if network_id is not None or verbose is not None:
-                raise ArgumentError("wrong argument: network_id and verbose should be None if from_trusted_source is True")
-            return str.__new__(cls, address)
-        if verbose is None:
-            verbose = False
+            if network_id is None and verbose is None:
+                return str.__new__(cls, address)
+            else:
+                raise ValueError("Invalid argument: `network_id` and `verbose` should be None if from_trusted_source is True")
+        
         try:
-            parts = cls.decode(address)
+            parts = cls.decode(address) # this line might raise exception if the address is not valid
+            if verbose is None:
+                # if verbose is None, the new address verbose is determined by the original address
+                verbose = (address[0] == "N" or address[0] == "C")
             if network_id is None:
-                val = cls._encode(parts["hex_address"], parts["network_id"], verbose)
-            else:
-                validate_network_id(network_id)    
-                val = cls._encode(parts["hex_address"], network_id, verbose)
+                # if network_id is None, the new address verbose is determined by the original address
+                network_id = parts["network_id"]
+
+            validate_network_id(network_id)  
+            val = cls._encode(parts["hex_address"], network_id, verbose, _ignore_invalid_type=_ignore_invalid_type)
         except InvalidBase32Address:
+            if verbose is None:
+                verbose = False
             if is_hex_address(address):
                 validate_network_id(network_id)
-                val = cls._encode(address, network_id, verbose) # type: ignore
+                val = cls._encode(address, network_id, verbose, _ignore_invalid_type=_ignore_invalid_type) # type: ignore
             else:
                 raise InvalidAddress("Address should be either base32 or hex, "
                                 f"receives {address}")
         
         return str.__new__(cls, val)
     
-    def __eq__(self, _address: str) -> bool:
+    def __eq__(self, _address: object) -> bool:
         """
-        invoked when a base32 address is compared to another string (or Base32Address typed object),
+        invoked when a base32 address is compared to another object (or Base32Address typed object),
         
-        :param str __address: value compared to 
+        :param str _address: value compared to, which is supposed to be encoded in Base32 format (else return false)
         :return bool: True if self and _address are of same hex_address and network_id
-        :raises InvalidBase32Address: _address is not encoded in base32 format
         :examples:
         
         >>> address = Base32Address("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
         >>> assert address == "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4"
         >>> assert "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4" == address
         >>> assert "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4" == address
         """
-        parts = self.__class__.decode(_address)
-        return self.hex_address == parts["hex_address"] and self.network_id == parts["network_id"]
+        try:
+            parts = self.__class__.decode(_address) # type: ignore
+            return self.hex_address == parts["hex_address"] and self.network_id == parts["network_id"]
+        except:
+            return False
+        
+    def __ne__(self, _address: object) -> bool:
+        return not (self == _address)
 
     def __hash__(self) -> int:
         return super().__hash__()
 
     @classmethod
     def from_public_key(
         cls, 
         public_key: Union[str, bytes],
-        network_id: int,
+        network_id: int = cast(int, default),
         verbose: bool = False
     ) -> "Base32Address":
         """
         create a Base32Address from public key
 
-        :param Union[str, bytes] public_key: str or bytes representation of public key
-        :param int network_id: network id of the return Base32Address, defaults to None
+        :param Union[str,bytes] public_key: str or bytes representation of public key
+        :param int network_id: network id of the return Base32Address, defaults to class variable :attr:`~default_network_id`
         :param bool verbose: whether the address will be represented in verbose mode, defaults to False
         :return Base32Address: Base32 representation of the address
+        
+        >>> Base32Address.from_public_key("0xdacdaeba8e391e7649d3ac4b5329ca0e202d38facd928d88b5f729b89a497e43cc4ad3816fcfdb241497b3b43862afb4c899bc284bf60feca4ee66ff868d1feb", 1)
+        'cfxtest:aamw4kj6g41pgedw1efjnsm59fbz0b9r1awbp8k2p2'
         """
         hex_address = public_key_to_cfx_hex(public_key)
         return cls(hex_address, network_id, verbose)
 
-    @functools.cached_property
+    @cached_property
     def network_id(self) -> int:
         """
         :return int: network_id of the address
         :examples:
         
         >>> address = Base32Address("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
         >>> address.network_id
         1
         """        
         return self.__class__._decode_network_id(self)
 
-    @functools.cached_property
-    def hex_address(self) -> HexAddress:
+    @cached_property
+    def hex_address(self) -> ChecksumAddress:
         """
-        :return HexAddress: hex address of the address.
+        :return ChecksumAddress: hex address of the address, will be encoded in ethereum checksum format
         
         >>> address = Base32Address("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
         >>> address.hex_address
-        '0x1ecde7223747601823f7535d7968ba98b4881e09'
+        '0x1ECdE7223747601823f7535d7968Ba98b4881E09'
         """        
         return self.__class__._decode_hex_address(self)
 
-    @functools.cached_property
+    @cached_property
     def address_type(self) -> AddressType:
         """
         :return Literal["null", "builtin", "user", "contract", "invalid"]: address type of an address. 
         
         :examples:
         
         >>> address = Base32Address("cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu")
         >>> address.address_type
         'user'
         """      
         return self.__class__._detect_address_type(HexBytes(self.hex_address))
 
-    @functools.cached_property
+    @cached_property
     def eth_checksum_address(self) -> ChecksumAddress:
         """
-        :return ChecksumAddress: self.hex_address in ethereum checksum address format
+        :return ChecksumAddress: alias for :attr:`~hex_address`. This API will be deprecated in a future version
         
         >>> address = Base32Address("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
-        >>> address.hex_address
-        '0x1ecde7223747601823f7535d7968ba98b4881e09'
         >>> address.eth_checksum_address
         '0x1ECdE7223747601823f7535d7968Ba98b4881E09'
         """        
-        return to_checksum_address(self.hex_address)
+        warnings.warn("eth_checksum_address will be deprecated in a future version. use hex_address instead", DeprecationWarning)
+        return self.hex_address
 
-    @functools.cached_property
+    @cached_property
     def verbose_address(self) -> "Base32Address":
         """
         :return Base32Address: self presented in verbose mode
         
         >>> address = Base32Address("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
         >>> address.verbose_address
         'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4'
         """        
-        return self.__class__.encode(self.hex_address, self.network_id, True)
+        return self.encode_base32(self.hex_address, self.network_id, True)
     
-    @functools.cached_property
+    @cached_property
     def abbr(self) -> str:
         """
         :return str: abbreviation of the address, as mentioned in https://forum.conflux.fun/t/voting-results-for-new-address-abbreviation-standard/7131
         
         :examples:
         
         >>> Base32Address("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4").abbr
         'cfxtest:aat...95j4'
         >>> Base32Address("cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu").abbr
         'cfx:aat...7ggp3vpu'
         """        
         return self.__class__._shorten_base32_address(self)
     
-    @functools.cached_property
+    @cached_property
     def compressed_abbr(self) -> str:
         """
-        :return str: compressed abbreviation of the address, same as property "abbr" except for mainnet address
+        :return str: compressed abbreviation of the address, as mentioned in https://forum.conflux.fun/t/voting-results-for-new-address-abbreviation-standard/7131
              
         :examples:
         
         >>> address = Base32Address("cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu")
         >>> address.abbr
         'cfx:aat...7ggp3vpu'
         >>> address.compressed_abbr
         'cfx:aat...3vpu'
         """ 
         return self.__class__._shorten_base32_address(self, True)
     
-    @functools.cached_property
-    def mapped_evm_space_address(self) -> HexAddress:
+    @cached_property
+    def mapped_evm_space_address(self) -> ChecksumAddress:
         """
-        :return HexAddress: the address of mapped account for EVM space as defined in https://github.com/Conflux-Chain/CIPs/blob/master/CIPs/cip-90.md#mapped-account
+        :return ChecksumAddress: the address of mapped account for EVM space as defined in https://github.com/Conflux-Chain/CIPs/blob/master/CIPs/cip-90.md#mapped-account
         
         >>> address = Base32Address("cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu")
         >>> address.mapped_evm_space_address
         '0x349f086998cF4a0C5a00b853a0E93239D81A97f6'
         """
         return self.__class__._mapped_evm_address_from_hex(self.hex_address)
 
     @classmethod
-    def encode(
-        cls, hex_address: str, network_id: int, verbose: bool=False
+    def encode_base32( # type: ignore
+        cls, hex_address: str, network_id: int=cast(int, default), verbose: bool=False, *, _ignore_invalid_type: bool=False
     ) -> "Base32Address":
         """
-        encode hex address to base32 address
+        Encode hex address to base32 address
 
         :param str hex_address: hex address begins with 0x
-        :param int network_id: address network id, e.g., 1 for testnet and 1029 for mainnet
+        :param int network_id: address network id, e.g., 1 for testnet and 1029 for mainnet, defaults to class variable :attr:`~default_network_id`
         :param bool verbose: whether the address will be presented in verbose mode, defaults to False
+        :param bool _ignore_invalid_type: whether the address type is validated, defaults to False
         :return Base32Address: an encoded base32 object, which can be trivially used as python str
         
         :examples:
         
-        >>> Base32Address.encode("0x1ecde7223747601823f7535d7968ba98b4881e09", 1)
+        >>> Base32Address.encode_base32("0x1ecde7223747601823f7535d7968ba98b4881e09", 1)
         'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
-        >>> Base32Address.encode("0x1ecde7223747601823f7535d7968ba98b4881e09", 1029, verbose=True)
+        >>> Base32Address.encode_base32("0x1ecde7223747601823f7535d7968ba98b4881e09", 1029, verbose=True)
         'CFX:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE7GGP3VPU'
         """ 
+        if network_id is default:
+            network_id = cast(int, cls.default_network_id)
         validate_hex_address(hex_address)
         validate_network_id(network_id)
-        return cls(hex_address, network_id, verbose)
+        return cls(hex_address, network_id, verbose, _ignore_invalid_type=_ignore_invalid_type)
+
+    @classmethod
+    def encode( # type: ignore
+        cls, hex_address: str, network_id: int=cast(int, default), verbose: bool=False, *, _ignore_invalid_type: bool=False
+    ) -> "Base32Address":
+        """
+        ## This method is deprecated and will be removed in future versions. Use encode_base32 method instead. ##
+        Encode hex address to base32 address.
+
+        :param str hex_address: hex address begins with 0x
+        :param int network_id: address network id, e.g., 1 for testnet and 1029 for mainnet, defaults to class variable :attr:`~default_network_id`
+        :param bool verbose: whether the address will be presented in verbose mode, defaults to False
+        :param bool _ignore_invalid_type: whether the address type is validated, defaults to False
+        :return Base32Address: an encoded base32 object, which can be trivially used as python str
+        
+        :examples:
+        
+        >>> Base32Address.encode("0x1ecde7223747601823f7535d7968ba98b4881e09", 1)
+        'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
+        >>> Base32Address.encode("0x1ecde7223747601823f7535d7968ba98b4881e09", 1029, verbose=True)
+        'CFX:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE7GGP3VPU'
+        """ 
+        warnings.warn(
+            "Base32Address.encode is deprecated and will be removed in future versions. "
+            "Use Base32Address.encode_base32 instead.", 
+            DeprecationWarning
+        )
+        return cls.encode_base32(hex_address, network_id, verbose, _ignore_invalid_type=_ignore_invalid_type)
 
     @classmethod
     def _encode(
-        cls, hex_address: str, network_id: int, verbose: bool=False
+        cls, hex_address: str, network_id: int, verbose: bool, *, _ignore_invalid_type: bool=False
     ) -> str:
         network_prefix = cls._encode_network_prefix(network_id)
         address_bytes = HexBytes(hex_address)
         payload = base32.encode(VERSION_BYTE + address_bytes)
         checksum = cls._create_checksum(network_prefix, payload)
         parts = [network_prefix]
         address_type = cls._detect_address_type(address_bytes)
-        if address_type == TYPE_INVALID:
-            raise InvalidConfluxHexAddress
+        if address_type == TYPE_INVALID and not _ignore_invalid_type:
+            raise InvalidConfluxHexAddress(f"The hex address should start with 0x0, 0x1 or 0x8, received {hex_address}."
+                                        "Check your code logic or set _ignore_invalid_type=True")
         if verbose:
             parts.append(f"{TYPE}.{address_type}")
         parts.append(payload + checksum)
         address = DELIMITER.join(parts)
         if verbose:
             return address.upper()
         return address
@@ -318,38 +427,38 @@
     @classmethod
     def _decode_network_id(cls, base32_address: str) -> int:
         base32_address = base32_address.lower()
         parts = base32_address.split(DELIMITER)
         return cls._network_prefix_to_id(parts[0])
 
     @classmethod
-    def _decode_hex_address(cls, base32_address: str) -> HexAddress:
+    def _decode_hex_address(cls, base32_address: str) -> ChecksumAddress:
         base32_address = base32_address.lower()
         parts = base32_address.split(DELIMITER)
         return cls._payload_to_hex(parts[-1])
 
     @classmethod
-    def _payload_to_hex(cls, payload: str) -> HexAddress:
+    def _payload_to_hex(cls, payload: str) -> ChecksumAddress:
         address_buf = base32.decode(payload)
         hex_buf = address_buf[1:21]
-        return HEX_PREFIX + hex_buf.hex() # type: ignore
+        return to_checksum_address(HEX_PREFIX + hex_buf.hex()) # type: ignore
     
     @classmethod
     def decode(cls, base32_address: str) -> Base32AddressParts:
         """
         Decode a base32 address string and get its hex_address, address_type, and network_id
 
         :param str base32_address: address encoded in base32 format
-        :raises InvalidBase32Address:
+        :raises InvalidBase32Address: the parameter is not a valid CIP-37 address
         :return Base32AddressParts: a dict object with field "hex_address", "address_type" and "network_id"
         
         :examples:
         
         >>> Base32Address.decode("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
-        {'network_id': 1, 'hex_address': '0x1ecde7223747601823f7535d7968ba98b4881e09', 'address_type': 'user'}
+        {'network_id': 1, 'hex_address': '0x1ECdE7223747601823f7535d7968Ba98b4881E09', 'address_type': 'user'}
         """        
         try:
             if not isinstance(base32_address, str):
                 raise InvalidBase32Address(f"Receives an argument of type {type(base32_address)}, expected a string")
             if not any([
                 str(base32_address) == base32_address.upper(), 
                 str(base32_address) == base32_address.lower(), 
@@ -358,25 +467,26 @@
                                         f"Receives {base32_address}")
             
             base32_address = base32_address.lower()
 
             splits = base32_address.split(DELIMITER)
             if len(splits) != 2 and len(splits) != 3:
                 raise InvalidBase32Address(
-                    "Address needs to be encode in Base32 format, such as cfx:aaejuaaaaaaaaaaaaaaaaaaaaaaaaaaaajrwuc9jnb\n"
+                    "Address needs to be encode in Base32 format, such as cfx:aaejuaaaaaaaaaaaaaaaaaaaaaaaaaaaajrwuc9jnb. "
                     "Received: {}".format(base32_address))
 
             # if exception occurs, outer try-except will handle
             address_parts = cls._decode(base32_address)
 
             # check address type
             address_type = address_parts["address_type"]
-            if address_type == TYPE_INVALID:
-                raise InvalidBase32Address(f"Invalid address type: the hex address of the provided address is {address_parts['hex_address']}, "
-                                        "while valid conflux address is supposed to start with 0x0, 0x1 or 0x8")
+            # it is ok to decode an address whose type is invalid
+            # if address_type == TYPE_INVALID:
+            #     raise InvalidBase32Address(f"Invalid address type: the hex address of the provided address is {address_parts['hex_address']}, "
+            #                             "while valid conflux address is supposed to start with 0x0, 0x1 or 0x8")
             
             """
             cip-37 #Decoding
             6.Verify optional fields:
 
             If the optional fields contain type.*: Verify the address-type according to the specification above.
             Unknown options (options other than type.*) should be ignored.
@@ -438,55 +548,58 @@
             return True
         except:
             return False
 
     @classmethod
     def validate(cls, value: Any) -> Literal[True]:
         """
-        validate if a value is a valid string-typed base32_address, raises an exception if not
+        Validate if a value is a valid string-typed base32_address, raises an exception if not
 
-        :param str base32_address: address to validate 
+        :param str value: value to validate 
         :raises InvalidBase32Address: raises an exception if the address is not a valid base32 address
         :return Literal[True]: returns True only if address is valid
         """
         # an exception will be raised if decode failure
         cls.decode(value)
         return True
   
     @classmethod
     def equals(cls, address1: str, address2: str) -> bool:
         """
-        check if two addresses share same hex_address and network_id
+        | Check if two addresses share same hex_address and network_id
+        | It will throw an error if any param is not in CIP-37 format while :meth:`~__eq__` doesn't
 
         :param str address1: base32 address to compare
         :param str address2: base32 address to compare
         :raises InvalidBase32Address: either address is not a valid base32 address
         :return bool: whether two addresses share same hex_address and network_id
         """
-        return cls(address1) == address2
+        return cls(address1) == cls(address2)
     
     @classmethod
-    def zero_address(cls, network_id: int, verbose: bool = False) -> "Base32Address":    
+    def zero_address(cls, network_id: int=cast(int, default), verbose: bool = False) -> "Base32Address":    
         """
         Get zero address of the target network.
 
-        :param int network_id: target network_id
+        :param int network_id: target network_id, defaults to `Base32Address.default_network_id`
         :param bool verbose: whether the zero address is presented in verbose mode, defaults to False
         :return Base32Address: base32 format zero address of the target network 
         :examples:
         
         >>> Base32Address.zero_address(network_id=1)
         'cfxtest:aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa6f0vrcsw'
         """        
-        return cls.encode("0x0000000000000000000000000000000000000000", network_id, verbose)
+        if network_id is default:
+            network_id = cast(int, cls.default_network_id)
+        return cls.encode_base32("0x0000000000000000000000000000000000000000", network_id, verbose)
     
     @classmethod
-    def shorten_base32_address(cls, base32_address: str, compressed=False) -> str:
+    def shorten_base32_address(cls, base32_address: str, compressed: bool=False) -> str:
         """
-        returns the abbreviation of the address
+        Returns the abbreviation of the address
 
         :param str base32_address: address to shorten
         :raises InvalidBase32Address: raised if address is invalid
         :param bool compressed: whether the abbreviation will be presented in compressed form,\
             which only affects mainnet addresses, defaults to False
         :return str: the abbreviation string
         
@@ -495,44 +608,44 @@
         >>> Base32Address.shorten_base32_address("cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu", compressed=True)
         'cfx:aat...3vpu'
         """        
         cls.validate(base32_address)
         return cls._shorten_base32_address(base32_address, compressed)
     
     @classmethod
-    def _shorten_base32_address(cls, base32_address: str, compressed=False) -> str:
+    def _shorten_base32_address(cls, base32_address: str, compressed: bool=False) -> str:
         lowcase = base32_address.lower()
         splits = lowcase.split(DELIMITER)
         prefix = splits[0]
         payload = splits[-1]
         if splits[0] != MAINNET_PREFIX or compressed:
             return f"{prefix}{DELIMITER}{payload[:3]}...{payload[-4:]}"
         else:
             return f"{prefix}{DELIMITER}{payload[:3]}...{payload[-8:]}"
     
     @classmethod
-    def calculate_mapped_evm_space_address(cls, base32_address: str) -> HexAddress:
+    def calculate_mapped_evm_space_address(cls, base32_address: str) -> ChecksumAddress:
         """
-        calculate the address of mapped account for EVM space as defined in https://github.com/Conflux-Chain/CIPs/blob/master/CIPs/cip-90.md#mapped-account
+        Calculate the address of mapped account for EVM space as defined in https://github.com/Conflux-Chain/CIPs/blob/master/CIPs/cip-90.md#mapped-account
 
         :raises InvalidBase32Address: raised when address is not a valid base32 address
         :examples:
         
         >>> Base32Address.calculate_mapped_evm_space_address("CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4")
         '0x349f086998cF4a0C5a00b853a0E93239D81A97f6'
         """        
         hex_address = cls.decode(base32_address)["hex_address"]
         return cls._mapped_evm_address_from_hex(hex_address)
 
     @classmethod
-    def _mapped_evm_address_from_hex(cls, hex_address: HexAddress) -> HexAddress:
+    def _mapped_evm_address_from_hex(cls, hex_address: str) -> ChecksumAddress:
         # do not check hex_address validity here
         mapped_hash = keccak(HexBytes(hex_address)).hex()
         mapped_evm_space_address = to_checksum_address(HEX_PREFIX + mapped_hash[-40:])
-        return cast(HexAddress, mapped_evm_space_address)
+        return mapped_evm_space_address
 
     @classmethod
     def _encode_network_prefix(cls, network_id: int) -> NetworkPrefix:
         if network_id == MAINNET_NETWORK_ID:
             return MAINNET_PREFIX
         elif network_id == TESTNET_NETWORK_ID:
             return TESTNET_PREFIX
@@ -551,51 +664,49 @@
                 raise InvalidBase32Address(f"The network prefix {network_prefix} is invalid")
             try:
                 return int(network_prefix[3:])
             except:
                 raise InvalidBase32Address(f"The network prefix {network_prefix} is invalid")
 
     @classmethod
-    def _create_checksum(cls, prefix, payload) -> str:
+    def _create_checksum(cls, prefix: NetworkPrefix, payload: str) -> str:
         """
         create checksum from prefix and payload
         :param prefix: network prefix (string)
         :param payload: bytes
         :return: string
         """
-        prefix = cls._prefix_to_words(prefix)
         delimiter = VERSION_BYTE
-        payload = base32.decode_to_words(payload)
         template = CHECKSUM_TEMPLATE
-        mod = cls._poly_mod(prefix + delimiter + payload + template)
+        mod = cls._poly_mod(cls._prefix_to_words(prefix) + delimiter + base32.decode_to_words(payload) + template)
         return base32.encode(cls._checksum_to_bytes(mod))
 
     @classmethod
-    def _detect_address_type(cls, hex_address_buf) -> AddressType:
+    def _detect_address_type(cls, hex_address_buf: bytes) -> AddressType:
         if hex_address_buf == bytes(20):
             return TYPE_NULL
         first_byte = hex_address_buf[0] & 0xf0
         if first_byte == 0x00:
             return TYPE_BUILTIN
         elif first_byte == 0x10:
             return TYPE_USER
         elif first_byte == 0x80:
             return TYPE_CONTRACT
         else:
             return TYPE_INVALID
 
     @classmethod
-    def _prefix_to_words(cls, prefix) -> bytearray:
+    def _prefix_to_words(cls, prefix: NetworkPrefix) -> bytearray:
         words = bytearray()
         for v in bytes(prefix, 'ascii'):
             words.append(v & 0x1f)
         return words
 
     @classmethod
-    def _checksum_to_bytes(cls, data) -> bytearray:
+    def _checksum_to_bytes(cls, data: int) -> bytearray:
         result = bytearray(0)
         result.append((data >> 32) & 0xff)
         result.append((data >> 24) & 0xff)
         result.append((data >> 16) & 0xff)
         result.append((data >> 8) & 0xff)
         result.append((data) & 0xff)
         return result
@@ -619,7 +730,27 @@
                 c ^= 0xf33e5fb3c4
             if c0 & 0x08:
                 c ^= 0xae2eabe2a8
             if c0 & 0x10:
                 c ^= 0x1e4f43e470
 
         return c ^ 1
+
+def get_base32_address_factory(default_network_id: int) -> Type[Base32Address]:
+    """
+    Generate a new :class:`~Base32Address` class object with `default_network_id` 
+    so the class variable will not influence the global :attr:`~Base32Address.default_network_id` setting
+    
+    >>> base32_address_factory = get_base32_address_factory(default_network_id=1)
+    >>> base32_address_factory.zero_address()
+    'cfxtest:aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa6f0vrcsw'
+
+    :param int default_network_id: default network 
+    :return Type[Base32Address]: a Class object of Base32Address with default_network_id
+    """
+    return type(
+        "Base32Address",
+        (Base32Address,),
+        {
+            "_default_network_id": default_network_id
+        }
+    )
```

### Comparing `cfx-address-1.0.0b9/cfx_address/base32.py` & `cfx-address-1.0.1/cfx_address/base32.py`

 * *Files identical despite different names*

### Comparing `cfx-address-1.0.0b9/cfx_address/utils.py` & `cfx-address-1.0.1/cfx_address/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,87 @@
 from typing import (
     Optional,
     Union,
-    cast,
-    Literal,
+    overload,
+)
+from typing_extensions import (
+    Literal
 )
 
 from eth_utils.address import (
     is_hex_address,
+    to_checksum_address,
 )
 
 from cfx_address._utils import (
     validate_hex_address,
     validate_network_id,
     eth_eoa_address_to_cfx_hex,
     public_key_to_cfx_hex,
 )
-from cfx_address.address import (
-    Base32Address
-)
+from cfx_address.address import Base32Address
 
 from cfx_utils.exceptions import (
     Base32AddressNotMatch,
     AddressNotMatch,
 )
 from cfx_utils.types import (
-    HexAddress,
+    ChecksumAddress,
 )
 
 validate_base32 = Base32Address.validate
 is_valid_base32 = Base32Address.is_valid_base32
 
+
+@overload
+def normalize_to(address: str, network_id: None, verbose: bool = False) -> ChecksumAddress:
+    ...
+
+
+@overload
+def normalize_to(address: str, network_id: int, verbose: bool = False) -> Base32Address:
+    ...
+
+
 def normalize_to(
-    address: str, network_id:Union[int, None], verbose=False
-) -> Union[Base32Address, HexAddress]:  
+    address: str, network_id: Union[int, None], verbose: bool = False
+) -> Union[Base32Address, ChecksumAddress]:
     """
     normalize a hex or base32 address to target network or hex address
 
     :param str address: a base32 address or hex address
-    :param Union[int, None] network_id: target network id. None will return hex address
-    :return Union[Base32Address, HexAddress]: a normalized base32 address or hex address, depending on network id
-    """    
+    :param Union[int, None] network_id: target network id. None will return hex checksum address
+    :return Union[Base32Address, HexAddress]: a normalized base32 address or hex checksum address, depending on network id
+    """
     if network_id is not None:
         return Base32Address(address, network_id, verbose)
     else:
         if is_hex_address(address):
-            return cast(HexAddress, address)
+            return to_checksum_address(address)
         # error will be raised if address is not a Base32Address
         return Base32Address(address).hex_address
 
-def validate_address_agaist_network_id(address: str, network_id: Union[int, None], accept_hex: Optional[bool]=False) -> Literal[True]:
+
+def validate_address_agaist_network_id(
+    address: str, network_id: Union[int, None], accept_hex: Optional[bool] = False
+) -> Literal[True]:
     """
     Validate address in specific network context. Error will be raised only if:
-        1. address validity checking: 
+        1. address validity checking:
             address is a base32 address or hex / base32 address if accept_hex
-        2. network id validity checking: 
+        2. network id validity checking:
             the network id of the address should be same as network_id, this step will be skipped if address is hex address or network_id is None
 
     :param str address: address to validate
     :param Union[int, None] network_id: if is None, then network id checking will be skipped
     :param Optional[bool] accept_hex: whether a hex address is accepted, if. Defaults to False
     :raises AddressNotMatch: hex address is received when accept_hex is not True
     :raises Base32AddressNotMatch: the network id of address does not equal to network_id
     :return Literal[True]: returns True if no exceptions are raised
-    
+
     >>> from cfx_address.utils import validate_address_agaist_network_id
     >>> address = Base32Address.zero_address(1)
     >>> validate_address_agaist_network_id(address, 1)
     True
     >>> validate_address_agaist_network_id(address.hex_address, 1, True)
     True
     >>> validate_address_agaist_network_id(address, None)
@@ -75,31 +90,33 @@
     Traceback (most recent call last):
         ...
     cfx_utils.exceptions.AddressNotMatch: hex address is not accepted
     >>> validate_address_agaist_network_id(address, 1029)
     Traceback (most recent call last):
         ...
     cfx_utils.exceptions.Base32AddressNotMatch: expects address of network id 1029, receives address of network id 1
-    
-    """    
+
+    """
     if is_hex_address(address):
         if accept_hex:
             return True
         raise AddressNotMatch("hex address is not accepted")
     else:
         # the address is Base32Address (or invalid)
         address_network_id = Base32Address.decode(address)["network_id"]
         if address_network_id == network_id or network_id is None:
             return True
-        raise Base32AddressNotMatch(f"expects address of network id {network_id}, "
-                                    f"receives address of network id {address_network_id}")
+        raise Base32AddressNotMatch(
+            f"expects address of network id {network_id}, "
+            f"receives address of network id {address_network_id}"
+        )
 
 
 __all__ = [
     "validate_hex_address",
     "validate_network_id",
     "eth_eoa_address_to_cfx_hex",
     "validate_base32",
     "is_valid_base32",
     "validate_address_agaist_network_id",
-    # "is_hex_address"
+    "public_key_to_cfx_hex",
 ]
```

### Comparing `cfx-address-1.0.0b9/cfx_address.egg-info/PKG-INFO` & `cfx-address-1.0.1/cfx_address.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,133 +1,127 @@
-Metadata-Version: 2.1
-Name: cfx-address
-Version: 1.0.0b9
-Summary: UNKNOWN
-Home-page: UNKNOWN
-Author: The Conflux foundation
-Author-email: wangpan@conflux-chain.org
-License: UNKNOWN
-Keywords: Conflux,base32,address
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-Provides-Extra: tester
-Provides-Extra: linter
-Provides-Extra: docs
-Provides-Extra: dev
-
-# cfx-address
-
-Conflux base32 address utilities
-
-Full documentation -> https://conflux-fans.github.io/cfx-address/cfx_address.html#module-cfx_address
-
-## installation
-
-```bash
-pip install cfx-address
-```
-
-### use Base32Address class methods
-
-```python
-from cfx_address import Base32Address
-```
-
-#### validate a base32 address
-``` python
-Base32Address.is_valid_base32("0x1ecde7223747601823f7535d7968ba98b4881e09") 
-# False
-Base32Address.validate("0x1ecde7223747601823f7535d7968ba98b4881e09")
-# will raise an exception
-```
-
-#### encode and decode
-
-``` python
-# encode hex address to base32
-Base32Address.encode("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1)
-#'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
-
-# decode base32 address
-Base32Address.decode("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
-# result:
-# {'network_id': 1,
-# 'hex_address': '0x1ecde7223747601823f7535d7968ba98b4881e09',
-# 'address_type': 'user'}
-```
-
-#### utilities
-
-```python
-address_str = "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4"
-address_verbose_str = "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4"
-assert Base32Address.equals(address_str, address_verbose_str)
-
-Base32Address.calculate_mapped_evm_space_address(address_str)
-Base32Address.zero_address(network_id=1)
-Base32Address.shorten_base32_address(address_str)
-```
-
-### Base32Address instances
-
-#### instance initialization
-
-```python
-address = Base32Address("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
-# 'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
-
-# Base32Address inherits from str
-assert isinstance(address, str)
-
-# init from hex address, in which case network_id is required
-Base32Address("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1029)
-# 'cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu'
-
-# change a base32 address to other network
-Base32Address(address, network_id=1029)
-# 'cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu'
-
-# verbose option defaults to False
-Base32Address(address, verbose=True)
-# 'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4'
-```
-
-#### __eq__ and properties
-
-```python
-# __eq__ is implemented, address in same network is treated equal
-assert address == "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4"
-assert address == "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4"
-assert "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4" == address
-assert "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4" == address
-
-# address in different network is not equal
-mainnet_address = Base32Address(address, 1029)
-assert mainnet_address == "cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu"
-assert not address == mainnet_address
-
-# properties
-[
-    address.address_type,
-    address.network_id,
-    address.hex_address,
-    address.verbose_address,
-    address.short,
-    address.mapped_evm_space_address
-    address.eth_checksum_address
-]
-# ['user',
-#  1,
-#  '0x1ecde7223747601823f7535d7968ba98b4881e09',
-#  'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4',
-#  'cfxtest:aat...95j4',
-#  '0x349f086998cF4a0C5a00b853a0E93239D81A97f6',
-#  '0x1ECdE7223747601823f7535d7968Ba98b4881E09']
-```
-
-
+Metadata-Version: 2.1
+Name: cfx-address
+Version: 1.0.1
+Author: The Conflux foundation
+Author-email: wangpan@conflux-chain.org
+Keywords: Conflux,base32,address
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Education
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: tester
+Provides-Extra: linter
+Provides-Extra: docs
+Provides-Extra: dev
+
+# cfx-address
+
+Conflux base32 address utilities
+
+Full documentation -> https://conflux-fans.github.io/cfx-address/cfx_address.html#module-cfx_address
+
+## installation
+
+```bash
+pip install cfx-address
+```
+
+### use Base32Address class methods
+
+```python
+from cfx_address import Base32Address
+```
+
+#### validate a base32 address
+``` python
+Base32Address.is_valid_base32("0x1ecde7223747601823f7535d7968ba98b4881e09") 
+# False
+Base32Address.validate("0x1ecde7223747601823f7535d7968ba98b4881e09")
+# will raise an exception
+```
+
+#### encode and decode
+
+``` python
+# encode hex address to base32
+Base32Address.encode_base32("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1)
+#'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
+
+# decode base32 address
+Base32Address.decode("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
+# result:
+# {'network_id': 1,
+# 'hex_address': '0x1ecde7223747601823f7535d7968ba98b4881e09',
+# 'address_type': 'user'}
+```
+
+#### utilities
+
+```python
+address_str = "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4"
+address_verbose_str = "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4"
+assert Base32Address.equals(address_str, address_verbose_str)
+
+Base32Address.calculate_mapped_evm_space_address(address_str)
+Base32Address.zero_address(network_id=1)
+Base32Address.shorten_base32_address(address_str)
+```
+
+### Base32Address instances
+
+#### instance initialization
+
+```python
+address = Base32Address("cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4")
+# 'cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4'
+
+# Base32Address inherits from str
+assert isinstance(address, str)
+
+# init from hex address, in which case network_id is required
+Base32Address("0x1ecde7223747601823f7535d7968ba98b4881e09", network_id=1029)
+# 'cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu'
+
+# change a base32 address to other network
+Base32Address(address, network_id=1029)
+# 'cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu'
+
+# verbose option defaults to False
+Base32Address(address, verbose=True)
+# 'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4'
+```
+
+#### __eq__ and properties
+
+```python
+# __eq__ is implemented, address in same network is treated equal
+assert address == "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4"
+assert address == "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4"
+assert "CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4" == address
+assert "cfxtest:aatp533cg7d0agbd87kz48nj1mpnkca8be1rz695j4" == address
+
+# address in different network is not equal
+mainnet_address = Base32Address(address, 1029)
+assert mainnet_address == "cfx:aatp533cg7d0agbd87kz48nj1mpnkca8be7ggp3vpu"
+assert not address == mainnet_address
+
+# properties
+[
+    address.address_type,
+    address.network_id,
+    address.hex_address,
+    address.verbose_address,
+    address.short,
+    address.mapped_evm_space_address
+]
+# ['user',
+#  1,
+#  '0x1ECdE7223747601823f7535d7968Ba98b4881E09',
+#  'CFXTEST:TYPE.USER:AATP533CG7D0AGBD87KZ48NJ1MPNKCA8BE1RZ695J4',
+#  'cfxtest:aat...95j4',
+#  '0x349f086998cF4a0C5a00b853a0E93239D81A97f6',
+#  ]
+```
```

### Comparing `cfx-address-1.0.0b9/setup.py` & `cfx-address-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,37 +51,41 @@
         # "twine>=1.13,<2",
         # "pluggy==0.13.1",
         # "when-changed>=0.3.0,<0.4"
     ]
 }
 
 extras_require['dev'] = (
-    extras_require['tester']
+    extras_require['tester'] # type: ignore
     + extras_require['linter']
     + extras_require['docs']
     + extras_require['dev']
 )
 
 with open('./README.md') as readme:
     long_description = readme.read()
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="cfx-address",
-    version="1.0.0-beta.9", # edit using bumpversion
+    version="1.0.1", # edit using bumpversion
     author="The Conflux foundation",
     author_email="wangpan@conflux-chain.org",
     long_description_content_type='text/markdown',
     long_description=long_description,
     packages=find_packages(),
+    python_requires='>=3.7',
+    package_data={'cfx_address': ['py.typed']},
     install_requires=[
-        "eth-utils>=2.0.0,<3.0.0",
+        "eth-utils>=1.9.5",
         "hexbytes>=0.1.0,<1.0.0",
-        "cfx-utils>=1.0.0b3",
+        "cfx-utils>=1.0.0",
+        "typing_extensions",
+        "cached_property==1.5.2;python_version<'3.8'"
     ],  # add any additional packages that
     # needs to be installed along with your package. Eg: 'caer'
     extras_require=extras_require,
     keywords=['Conflux', 'base32', 'address'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
```

