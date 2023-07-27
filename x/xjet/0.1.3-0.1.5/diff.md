# Comparing `tmp/xjet-0.1.3.tar.gz` & `tmp/xjet-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xjet-0.1.3.tar", max compression
+gzip compressed data, was "xjet-0.1.5.tar", max compression
```

## Comparing `xjet-0.1.3.tar` & `xjet-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-01-15 16:26:30.059724 xjet-0.1.3/LICENSE
--rw-r--r--   0        0        0     3596 2023-07-26 17:16:04.984537 xjet-0.1.3/README.md
--rw-r--r--   0        0        0      798 2023-07-26 17:41:01.639637 xjet-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3048 2023-07-26 17:39:13.325732 xjet-0.1.3/xjet/__init__.py
--rw-r--r--   0        0        0     7480 2023-07-26 17:24:20.211970 xjet-0.1.3/xjet/api.py
--rw-r--r--   0        0        0     1228 2023-07-26 17:41:18.063263 xjet-0.1.3/xjet/sync.py
--rw-r--r--   0        0        0     4514 1970-01-01 00:00:00.000000 xjet-0.1.3/setup.py
--rw-r--r--   0        0        0     4565 1970-01-01 00:00:00.000000 xjet-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-15 16:26:30.059724 xjet-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3596 2023-07-26 17:16:04.984537 xjet-0.1.5/README.md
+-rw-r--r--   0        0        0      686 2023-07-27 06:15:12.884440 xjet-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3048 2023-07-26 17:39:13.325732 xjet-0.1.5/xjet/__init__.py
+-rw-r--r--   0        0        0     7516 2023-07-27 06:06:48.670514 xjet-0.1.5/xjet/api.py
+-rw-r--r--   0        0        0     1228 2023-07-26 17:41:18.063263 xjet-0.1.5/xjet/sync.py
+-rw-r--r--   0        0        0     4500 1970-01-01 00:00:00.000000 xjet-0.1.5/setup.py
+-rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 xjet-0.1.5/PKG-INFO
```

### Comparing `xjet-0.1.3/LICENSE` & `xjet-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xjet-0.1.3/README.md` & `xjet-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `xjet-0.1.3/xjet/__init__.py` & `xjet-0.1.5/xjet/__init__.py`

 * *Files identical despite different names*

### Comparing `xjet-0.1.3/xjet/api.py` & `xjet-0.1.5/xjet/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,34 +212,34 @@
     * pairs()
     * estimate()
     * create_order()
     * order_status()
 
     """
 
-    async def pairs(self):
+    async def exchange_pairs(self):
         """ Get list of pairs """
         return await self.request(method = 'exchanges.pairs', request_method = 'GET')
 
-    async def estimate(self, pair: list, action_type: str, amount: Union[int, float]):
+    async def exchange_estimate(self, pair: list, action_type: str, amount: Union[int, float]):
         """ Estimate
 
         :param `pair` [list]: Pair
         :param `type` [str]: Type
         :param `amount` Union[int, float]: Amount
         
         """
         return await self.request(
             method = 'exchanges.estimate', 
             json = {
                 'pair': pair, 'type': action_type, 'amount': amount
             }
         )
 
-    async def create_order(self, pair: list, action_type: str, amount: Union[int, float], min_excepted_amount: Union[int, float]):
+    async def exchange_create_order(self, pair: list, action_type: str, amount: Union[int, float], min_excepted_amount: Union[int, float]):
         """ Create order
 
         :param `pair` [list]: Pair
         :param `action_type` [str]: Action type
         :param `amount` Union[int, float]: Amount
         :param `min_excepted_amount` Union[int, float]: Min excepted amount
         
@@ -247,13 +247,13 @@
         return await self.request(
             method = 'exchanges.createOrder', 
             json = self.sign_message({
                 'pair': pair, 'type': action_type, 'amount': amount, 'min_expected_amount': min_excepted_amount
             })
         )
 
-    async def order_status(self, order_id: str):
+    async def exchange_order_status(self, order_id: str):
         """ Get order status
         
         :param `order_id` [str]: Order id
         """
         return await self.request(method = 'exchanges.orderStatus', params = {'id': order_id})
```

### Comparing `xjet-0.1.3/xjet/sync.py` & `xjet-0.1.5/xjet/sync.py`

 * *Files identical despite different names*

### Comparing `xjet-0.1.3/setup.py` & `xjet-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['ecdsa>=0.18.0', 'httpx>=0.23.1']
 
 setup_kwargs = {
     'name': 'xjet',
-    'version': '0.1.3',
+    'version': '0.1.5',
     'description': 'Python SDK for t.me/xJetSwapBot',
     'long_description': '# Python SDK for xJet Connect API\n\n## Authors\n- [@xJetLabs](https://github.com/xJetLabs) (forked from)\n- [@nik-1x](https://www.github.com/nik-1x)\n \n## Installation\n```shell\npip install xjet\n```\nIf requires <b>nacl</b> package, install it <i>manually</i>:\n```shell\npip install pynacl\n```\n\n## Webhook analog\n```python\nwhile True:\n    res = httpx.get(\n        \'https://api.xjet.io/v1/account.events\',\n        params={\'timeout\': 10},\n        headers={\n            \'X-API-Key\': api_key,\n        },\n        timeout=11,\n    )\n    print(res.json)\n\n    time.sleep(3)\n```\n\n\n## Usage/Examples  \n[Live example](https://replit.com/@delpydoc/xJetAPI)\n\n### Initialization\n```python\nfrom xjet import JetAPI\n\n# api_key: str\n# private_key: str\napi = JetAPI(\n    api_key="API_KEY",\n    private_key="PRIVATE_KEY",\n    network=\'mainnet\'  # mainnet / testnet\n)\n```\n\n\n### Info\n```python\nawait xjet.currencies() # Shows all saved xJetSwap currencies\n```\n\n\n### Account\n```python\nawait api.me() # get API Application information.\n# {\'id\': <str>, \'name: <str>, \'service_wallet\': <str>}\n\nawait api.balance() # get balance\n# {\n#   \'balances\': [\n#       {\'currency\': <int>, \'amount\': <float>, \n#           \'values\': {\'byn\': 0.0, \'cny\': 0.0, \'eur\': 0.0, \'gbp\': 0.0, \'kzt\': 0.0, \'rub\': 0.0, \'uah\': 0.0, \'usd\': 0.0}}], \n#   \'timestamp\': <int>\n# }\n\nawait api.submit_deposit() # check for deposit\n# {\'success\': <bool>}\n\n# ton_address: str\n# currency: str\n# amount: float\nawait api.withdraw(ton_address, currency, amount) # check for deposit\n\n# limit: int\n# offset: int\nawait xjet.operations(limit, offset) # operations\n```\n\n### Cheque\n```python\n# currency: str\n# amount: float\n# expires: [int, None]\n# description: [str, None]\n# activates_count: [int, None]\n# groups_id: [int, None]\n# personal_id: [int, None]\n# password: [str, None]\n\nawait api.cheque_create(currency, amount, expires, description, activates_count, groups_id, personal_id, password) # create cheque\n# {\'cheque_id\': <str>, \'external_link\': \'https://t.me/xJetSwapBot?start=c_<cheque_id>\'}\n\nawait api.cheque_status(cheque_id) # get cheque status\n# {\n#   \'id\': <str>, \n#   \'issuer_id\': <str>, \n#   \'amount\': <float>, \n#   \'activates_count\': <int>, \n#   \'activates: <list[str]>, \n#   \'locked_value\': <float>, \n#   \'currency\': <Str>, \n#   \'expires\': <bool>, \n#   \'description\': <str>, \n#   \'status\': \'activated/canceled/expired/active\', \n#   \'password\': <str | None>, \n#   \'groups_id\': <list[str] | None>, \n#   \'personal_id\': <int | None>, \n#   \'is_for_premium\': <bool>\n# }\n\n\nawait api.cheque_list() # get cheques on account\n# list of cheque_status\n\nawait api.cheque_cancel(cheque_id) # delete cheque\n# returns cheque_status\n```\n\n\n### Invoice\n```python\n# currency: str\n# amount: float\n# description: [str, None]\n# max_payments: [int, None]\nawait api.invoice_create(currency, amount, description, max_payments) # create invoice\n# {\'invoice_id\': <str>, \'external_link\': \'https://t.me/xJetSwapBot?start=inv_<cheque_id>\'}\n\nawait api.invoice_status(invoice_status) # get invoice status\n# {\n#   \'id\': <str>, \n#   \'description\': <str>, \n#   \'currency\': <str>, \n#   \'amount\': <float>, \n#   \'max_amount\': None, \n#   \'min_amount\': None, \n#   \'payments\': [{\'telegram_id\': <int>, \'amount\': <float>, \'comment\': [str | None}, ... ], \n#   \'max_payments\': 1, \n#   \'after_pay\': [], \n#   \'created\': \'2023-04-20T22:55:24.313000\'\n# }\n\nawait api.invoice_list() # get invoices on account\n# list of invoice_status\n```\n\n```python\n# NFT methods\nawait api.nft_list()\nawait api.nft_transfer(nft_address, to_address)\n```\n\n## License\n[GNUv3](https://github.com/nik-1x/pyxJetAPI/blob/main/LICENSE)  \n',
     'author': 'delpydoc',
     'author_email': 'delpydoc@proton.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/xJetLabs/python-sdk',
+    'url': 'https://t.me/xJetSwapBot',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `xjet-0.1.3/PKG-INFO` & `xjet-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: xjet
-Version: 0.1.3
+Version: 0.1.5
 Summary: Python SDK for t.me/xJetSwapBot
-Home-page: https://github.com/xJetLabs/python-sdk
-Keywords: ton,the open network,xjet,xjetswap,sdk
+Home-page: https://t.me/xJetSwapBot
+Keywords: ton,xjet,xjetswap,sdk
 Author: delpydoc
 Author-email: delpydoc@proton.me
 Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

