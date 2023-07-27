# Comparing `tmp/harmony_toolbox-1.1.0.tar.gz` & `tmp/harmony_toolbox-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmony_toolbox-1.1.0.tar", last modified: Wed Jul 26 01:12:31 2023, max compression
+gzip compressed data, was "harmony_toolbox-1.1.1.tar", last modified: Thu Jul 27 19:40:36 2023, max compression
```

## Comparing `harmony_toolbox-1.1.0.tar` & `harmony_toolbox-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-26 01:12:31.138245 harmony_toolbox-1.1.0/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1066 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.0/LICENSE
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      146 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.0/MANIFEST.in
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-07-26 01:12:31.139245 harmony_toolbox-1.1.0/PKG-INFO
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1058 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.0/README.md
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      121 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.0/pyproject.toml
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      141 2023-06-30 15:28:08.000000 harmony_toolbox-1.1.0/requirements.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      736 2023-07-26 01:12:31.146247 harmony_toolbox-1.1.0/setup.cfg
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)       37 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.0/setup.py
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-26 01:12:30.732547 harmony_toolbox-1.1.0/src/
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-26 01:12:30.987246 harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-07-26 01:12:30.000000 harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/PKG-INFO
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      344 2023-07-26 01:12:30.000000 harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/SOURCES.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        1 2023-07-26 01:12:30.000000 harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/dependency_links.txt
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        8 2023-07-26 01:12:30.000000 harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/top_level.txt
-drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-26 01:12:31.107245 harmony_toolbox-1.1.0/src/toolbox/
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-03-24 16:13:56.000000 harmony_toolbox-1.1.0/src/toolbox/__init__.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     2297 2023-07-19 18:56:52.000000 harmony_toolbox-1.1.0/src/toolbox/config.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    48485 2023-07-20 20:30:13.000000 harmony_toolbox-1.1.0/src/toolbox/library.py
--rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    30860 2023-07-26 00:27:49.000000 harmony_toolbox-1.1.0/src/toolbox/toolbox.py
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-27 19:40:36.075226 harmony_toolbox-1.1.1/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1066 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.1/LICENSE
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      146 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.1/MANIFEST.in
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-07-27 19:40:36.076226 harmony_toolbox-1.1.1/PKG-INFO
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1058 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.1/README.md
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      121 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.1/pyproject.toml
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      141 2023-06-30 15:28:08.000000 harmony_toolbox-1.1.1/requirements.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      736 2023-07-27 19:40:36.084222 harmony_toolbox-1.1.1/setup.cfg
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)       37 2023-04-04 17:13:12.000000 harmony_toolbox-1.1.1/setup.py
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-27 19:40:35.566121 harmony_toolbox-1.1.1/src/
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-27 19:40:35.872225 harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     1680 2023-07-27 19:40:35.000000 harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/PKG-INFO
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)      344 2023-07-27 19:40:35.000000 harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/SOURCES.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        1 2023-07-27 19:40:35.000000 harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/dependency_links.txt
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        8 2023-07-27 19:40:35.000000 harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-07-27 19:40:36.034226 harmony_toolbox-1.1.1/src/toolbox/
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)        0 2023-03-24 16:13:56.000000 harmony_toolbox-1.1.1/src/toolbox/__init__.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)     2297 2023-07-27 19:37:57.000000 harmony_toolbox-1.1.1/src/toolbox/config.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    49984 2023-07-27 18:03:40.000000 harmony_toolbox-1.1.1/src/toolbox/library.py
+-rwxrwxrwx   0 serviceuser  (1000) serviceuser  (1000)    31224 2023-07-27 17:44:47.000000 harmony_toolbox-1.1.1/src/toolbox/toolbox.py
```

### Comparing `harmony_toolbox-1.1.0/LICENSE` & `harmony_toolbox-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `harmony_toolbox-1.1.0/PKG-INFO` & `harmony_toolbox-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony_toolbox
-Version: 1.1.0
+Version: 1.1.1
 Summary: Harmony ONE Validator Node Toolbox and Easy Setup
 Home-page: https://github.com/easy-node-pro/harmony-toolbox
 Author: EasyNode.PRO
 Author-email: support@easynode.pro
 Project-URL: Bug Tracker, https://github.com/easy-node-pro/harmony-toolbox/issues
 Project-URL: repository, https://github.com/easy-node-pro/harmony-toolbox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harmony_toolbox-1.1.0/README.md` & `harmony_toolbox-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `harmony_toolbox-1.1.0/setup.cfg` & `harmony_toolbox-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = harmony_toolbox
-version = 1.1.0
+version = 1.1.1
 author = EasyNode.PRO
 author_email = support@easynode.pro
 description = Harmony ONE Validator Node Toolbox and Easy Setup
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/easy-node-pro/harmony-toolbox
 project_urls =
```

### Comparing `harmony_toolbox-1.1.0/src/harmony_toolbox.egg-info/PKG-INFO` & `harmony_toolbox-1.1.1/src/harmony_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmony-toolbox
-Version: 1.1.0
+Version: 1.1.1
 Summary: Harmony ONE Validator Node Toolbox and Easy Setup
 Home-page: https://github.com/easy-node-pro/harmony-toolbox
 Author: EasyNode.PRO
 Author-email: support@easynode.pro
 Project-URL: Bug Tracker, https://github.com/easy-node-pro/harmony-toolbox/issues
 Project-URL: repository, https://github.com/easy-node-pro/harmony-toolbox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harmony_toolbox-1.1.0/src/toolbox/config.py` & `harmony_toolbox-1.1.1/src/toolbox/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     except requests.exceptions.RequestException as x:
         print(type(x), x)
         result = "0.0.0.0"
     return result
 
 
 class EnvironmentVariables:
-    easy_version = "1.1.0"
+    easy_version = "1.1.1"
     server_host_name = socket.gethostname()
     user_home_dir = path.expanduser("~")
     dotenv_file = f"{user_home_dir}/.easynode.env"
     active_user = path.split(user_home_dir)[-1]
     harmony_dir = environ.get("HARMONY_DIR") or f"{user_home_dir}/harmony"
     bls_key_file = path.join(harmony_dir, "blskey.pass")
     hmy_app = path.join(harmony_dir, "hmy")
```

### Comparing `harmony_toolbox-1.1.0/src/toolbox/library.py` & `harmony_toolbox-1.1.1/src/toolbox/library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import psutil, platform, dotenv, os, subprocess, requests, pyhmy, shutil, hashlib, re, json, subprocess
+import psutil, platform, dotenv, os, subprocess, requests, pyhmy, shutil, hashlib, re, json, subprocess, getpass
 from os import environ
 from dotenv import load_dotenv
 from simple_term_menu import TerminalMenu
 from colorama import Fore, Style, Back
 from pathlib import Path
 from pyhmy import account, staking, validator, numbers
 from json import load, dump
@@ -117,33 +117,33 @@
         f"* If you would like to import a wallet for manual wallet actions, and for using our claim and send functions, answer yes.\n* If you only want to load your validator address for stats answer no.\n* Would you like to add your wallet to this server? (YES/NO) "
     )
     # if yes, find recovery type
     if question:
         recovery_type()
         load_var_file(EnvironmentVariables.dotenv_file)
         print(
-            f'\n* Verify the address above matches the address below:\n* Detected Wallet: {Fore.YELLOW}{environ.get("VALIDATOR_WALLET")}{Fore.GREEN}\n* If a different wallet is showing you can remove it and retry it after installation.\n*\n* .{EnvironmentVariables.hmy_app} keys remove {EnvironmentVariables.active_user}\n*\n* To restore a wallet once again, run the following:\n*\n* .{EnvironmentVariables.hmy_app} keys recover-from-mnemonic {EnvironmentVariables.active_user} {environ.get("PASS_SWITCH")}\n*'
+            f'\n* Verify the address above matches the address below:\n* Detected Wallet: {Fore.YELLOW}{environ.get("VALIDATOR_WALLET")}{Fore.GREEN}\n* If a different wallet is showing you can remove it and retry it after installation.\n*\n* .{environ.get("HARMONY_DIR")}/hmy keys remove {EnvironmentVariables.active_user}\n*\n* To restore a wallet once again, run the following:\n*\n* .{environ.get("HARMONY_DIR")}/hmy keys recover-from-mnemonic {EnvironmentVariables.active_user} {environ.get("PASS_SWITCH")}\n*'
         )
         print_stars()
         input("* Verify your wallet information above.\n* Press ENTER to continue Installation.")
     else:
         while True:
             wallet = input(
-                f"* If you'd like to use the management menu, we need a one1 address, please input your address now: "
+                f"* If you'd like to use the management menu, we need a one1 or 0x address, please input your address now: "
             )
-            if wallet.startswith("one1"):
+            if wallet.startswith("one1") or wallet.startswith("0x"):
                 # Re-enter the wallet to verify
                 verify_wallet = input(f"* Please re-enter your wallet address for verification: ")
                 if wallet == verify_wallet:
                     set_var(EnvironmentVariables.dotenv_file, "VALIDATOR_WALLET", wallet)
-                    return
+                    break
                 else:
                     print("The entered wallets do not match. Please try again.")
             else:
-                print("Invalid wallet address. It should start with 'one1'. Please try again.")
+                print("Invalid wallet address. It should start with one1 or 0x. Please try again.")
     return
 
 
 def pull_harmony_update(harmony_dir, harmony_conf):
     arch = os.uname().machine
     os.chdir(f"{harmony_dir}")
     if environ.get("NETWORK") == "testnet":
@@ -155,63 +155,59 @@
         if arch == "x86_64":
             os.system("curl -LO https://harmony.one/binary && mv binary harmony && chmod +x harmony")
         os.system("./harmony config dump harmony.conf")
     update_text_file(harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
     update_text_file(harmony_conf, " DisablePrivateIPScan = false", " DisablePrivateIPScan = true")
     print_stars()
     print("* harmony.conf MaxKeys modified to 13 & DisablePrivateIPScan set to true.")
-    if os.path.isdir(f"{os.environ.get('HARMONY_DIR')}/blskey.pass"):
+    if os.path.isfile(f"{os.environ.get('HARMONY_DIR')}/blskey.pass"):
         update_text_file(harmony_conf, 'PassFile = ""', f'PassFile = "blskey.pass"')
         print("* blskey.pass found, updated harmony.conf")
     print_stars()
     print(f"* Harmony {environ.get('NETWORK')} application installed & ~/harmony/harmony.conf created. ")
     return
 
 
 # Search harmony.conf for the proper port to hit
 def find_port(folder):
-    with open(f"{EnvironmentVariables.user_home_dir}/{folder}/harmony.conf") as f:
+    with open(f"{folder}/harmony.conf") as f:
         data_file = f.readlines()
     count = 0
     for line in data_file:
         line = line.rstrip()
         if "Port =" in line:
             if count == 3:
                 return line[9:]
             count += 1
 
 
 # build list of installs
 def get_folders():
     folders = {}
-    if os.path.exists(f"{os.environ.get('HARMONY_DIR')}/harmony.conf"):
-        port = find_port(f"harmony")
+    if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony/harmony.conf"):
+        port = find_port(f"{EnvironmentVariables.user_home_dir}/harmony")
         folders["harmony"] = port
         print(f"* Found ~/harmony folder, on port {port}")
-        print_stars()
-    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony0/harmony.conf"):
-        port = find_port(f"harmony0")
+    if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony0/harmony.conf"):
+        port = find_port(f"{EnvironmentVariables.user_home_dir}/harmony0")
         folders["harmony0"] = port
         print(f"* Found ~/harmony1 folder, on port {port}")
-        print_stars()
-    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony1/harmony.conf"):
-        port = find_port(f"harmony1")
+    if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony1/harmony.conf"):
+        port = find_port(f"{EnvironmentVariables.user_home_dir}/harmony1")
         folders["harmony1"] = port
         print(f"* Found ~/harmony1 folder, on port {port}")
-        print_stars()
-    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony2/harmony.conf"):
-        port = find_port(f"harmony2")
+    if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony2/harmony.conf"):
+        port = find_port(f"{EnvironmentVariables.user_home_dir}/harmony2")
         folders["harmony2"] = port
         print(f"* Found ~/harmony2 folder, on port {port}")
-        print_stars()
-    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony3/harmony.conf"):
-        port = find_port(f"harmony3")
+    if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony3/harmony.conf"):
+        port = find_port(f"{EnvironmentVariables.user_home_dir}/harmony3")
         folders["harmony3"] = port
         print(f"* Found ~/harmony3 folder, on port {port}")
-        print_stars()
+    print_stars()
     return folders
 
 
 def validator_stats_output(folders) -> None:
     # Get server stats & wallet balances
     load_1, load_5, load_15 = os.getloadavg()
     sign_percentage = get_sign_pct()
@@ -255,30 +251,42 @@
         local_server = [
             f"{EnvironmentVariables.user_home_dir}/{folder}/hmy",
             "utility",
             "metadata",
             f"--node=http://localhost:{folders[folder]}",
         ]
         result_local_server = run(local_server, stdout=PIPE, stderr=PIPE, universal_newlines=True)
-        local_data = json.loads(result_local_server.stdout)
-        remote_server = [
-            f"{EnvironmentVariables.user_home_dir}/{folder}/hmy",
-            "utility",
-            "metadata",
-            f"--node=https://api.s{local_data['result']['shard-id']}.t.hmny.io",
-        ]
-        result_remote_server = run(remote_server, stdout=PIPE, stderr=PIPE, universal_newlines=True)
-        remote_data = json.loads(result_remote_server.stdout)
-        print(
-            f"* Remote Shard {local_data['result']['shard-id']} Epoch: {remote_data['result']['current-epoch']}, Current Block: {remote_data['result']['current-block-number']}"
-        )
-        print(
-            f"*  Local Shard {local_data['result']['shard-id']} Epoch: {local_data['result']['current-epoch']}, Current Block: {(local_data['result']['current-block-number'])}\n*   Local Shard 0 Size: {get_db_size(f'{current_full_path}', '0')}\n*   Local Shard {local_data['result']['shard-id']} Size: {get_db_size(f'{current_full_path}', local_data['result']['shard-id'])}"
-        )
-        print_stars()
+        try:
+            local_data = json.loads(result_local_server.stdout)
+            remote_server = [
+                f"{EnvironmentVariables.user_home_dir}/{folder}/hmy",
+                "utility",
+                "metadata",
+                f"--node=https://api.s{local_data['result']['shard-id']}.t.hmny.io",
+            ]
+            result_remote_server = run(remote_server, stdout=PIPE, stderr=PIPE, universal_newlines=True)
+            remote_data = json.loads(result_remote_server.stdout)
+            print(
+                f"* Remote Shard {local_data['result']['shard-id']} Epoch: {remote_data['result']['current-epoch']}, Current Block: {remote_data['result']['current-block-number']}"
+            )
+            if local_data["result"]["shard-id"] == 0:
+                print(
+                    f"*  Local Shard {local_data['result']['shard-id']} Epoch: {local_data['result']['current-epoch']}, Current Block: {(local_data['result']['current-block-number'])}"
+                    + f"\n*   Local Shard {local_data['result']['shard-id']} Size: {get_db_size(f'{current_full_path}', local_data['result']['shard-id'])}"
+                )
+            else:
+                print(
+                    f"*  Local Shard {local_data['result']['shard-id']} Epoch: {local_data['result']['current-epoch']}, Current Block: {(local_data['result']['current-block-number'])}"
+                    + f"\n*   Local Shard 0 Size: {get_db_size(f'{current_full_path}', '0')}\n*   Local Shard {local_data['result']['shard-id']} Size: {get_db_size(f'{current_full_path}', local_data['result']['shard-id'])}"
+                )
+
+            print_stars()
+        except Exception as e:
+            print(f"* Error, Service Offline or Unresponsive: {e}")
+            print_stars()
 
 
 def harmony_service_status(service="harmony") -> None:
     status = subprocess.call(["systemctl", "is-active", "--quiet", service])
     if status == 0:
         if service == "harmony":
             print(
@@ -309,15 +317,15 @@
         )
 
 
 def set_wallet_env():
     load_var_file(EnvironmentVariables.dotenv_file)
     if os.path.exists(EnvironmentVariables.hmy_wallet_store):
         output = subprocess.getoutput(
-            f"{EnvironmentVariables.hmy_app} keys list | grep {EnvironmentVariables.active_user}"
+            f"{environ.get('HARMONY_DIR')}/hmy keys list | grep {EnvironmentVariables.active_user}"
         )
         output_stripped = output.lstrip(EnvironmentVariables.active_user)
         output_stripped = output_stripped.strip()
         set_var(EnvironmentVariables.dotenv_file, "VALIDATOR_WALLET", output_stripped)
         return output_stripped
     else:
         validator_wallet = environ.get("VALIDATOR_WALLET")
@@ -342,29 +350,28 @@
         "[0] - Mnemonic Phrase Recovery",
         "[1] - Private Key Recovery",
     ]
     terminal_menu = TerminalMenu(
         menu_options, title="* Which type of restore method would you like to use for your validator wallet?"
     )
     results = terminal_menu.show()
+    passphrase_set()
     if results == 0:
-        passphrase_set()
         # Mnemonic Recovery Here
         os.system(
-            f"{EnvironmentVariables.hmy_app} keys recover-from-mnemonic {EnvironmentVariables.active_user} --passphrase-file passphrase.txt"
+            f"{environ.get('HARMONY_DIR')}/hmy keys recover-from-mnemonic {EnvironmentVariables.active_user} --passphrase-file passphrase.txt"
         )
         print_stars()
         set_wallet_env()
     elif results == 1:
-        passphrase_set()
         # Private Key Recovery Here
         print("* Private key recovery requires your private information in the command itself.")
         private = input("* Please enter your private key to restore your wallet: ")
         os.system(
-            f"{EnvironmentVariables.hmy_app} keys import-private-key {private} {EnvironmentVariables.active_user} --passphrase"
+            f"{environ.get('HARMONY_DIR')}/hmy keys import-private-key {private} {EnvironmentVariables.active_user} --passphrase-file passphrase.txt"
         )
         print_stars()
         set_wallet_env()
 
 
 def passphrase_status():
     load_var_file(EnvironmentVariables.dotenv_file)
@@ -377,15 +384,15 @@
         )
     else:
         set_var(EnvironmentVariables.dotenv_file, "PASS_SWITCH", "--passphrase")
     load_var_file(EnvironmentVariables.dotenv_file)
 
 
 def passphrase_set():
-    if os.path.exists(EnvironmentVariables.password_path):
+    if os.path.exists(f"{environ.get('HARMONY_DIR')}/passphrase.txt"):
         return
     import getpass
 
     print(f"* Setup {os.environ.get('HARMONY_DIR')}/passphrase.txt file for use with autobidder & harmony-toolbox.")
     print_stars()
     # take input
     while True:
@@ -396,15 +403,15 @@
         password_2 = getpass.getpass(prompt="* Re-enter your password: ", stream=None)
         if not password_1 == password_2:
             print("* Passwords do NOT match, Please try again..")
         else:
             print("* Passwords Match!")
             break
     # Save file, we won't encrypt because if someone has access to the file, they will also have the salt and decrypt code at their disposal.
-    save_text(EnvironmentVariables.password_path, password_1)
+    save_text(f"{environ.get('HARMONY_DIR')}/passphrase.txt", password_1)
     load_var_file(EnvironmentVariables.dotenv_file)
     passphrase_status()
 
 
 def process_command(command: str) -> None:
     process = subprocess.Popen(command, shell=True)
     output, error = process.communicate()
@@ -612,15 +619,15 @@
         totalRewards = totalRewards + i["reward"]
     totalRewards = "{:,}".format(round(totalRewards * 0.000000000000000001, 2))
     return totalRewards
 
 
 def get_sign_pct() -> str:
     config = EnvironmentVariables()
-    hmy_external_rpc = f"{EnvironmentVariables.hmy_app} --node='{config.working_rpc_endpoint}'"
+    hmy_external_rpc = f"{environ.get('HARMONY_DIR')}/hmy --node='{config.working_rpc_endpoint}'"
     output = subprocess.getoutput(
         f"{hmy_external_rpc} blockchain validator information {environ.get('VALIDATOR_WALLET')} | grep signing-percentage"
     )
     output_stripped = output.lstrip('        "current-epoch-signing-percentage": "').rstrip('",')
     try:
         math = float(output_stripped)
         signPerc = math * 100
@@ -667,14 +674,15 @@
     return output_harmony_version.group(1)[:-2], hmy_ver
 
 
 def first_env_check(env_file) -> None:
     first_time = load_var_file(env_file)
     return first_time
 
+
 def version_checks(harmony_folder):
     software_versions = {}
     software_versions["harmony_version"], software_versions["hmy_version"] = get_local_version(f"{harmony_folder}")
     software_versions["online_harmony_version"], software_versions["online_hmy_version"] = check_online_version()
     # Check versions, if matching False (No Upgrade Required), non-match True (Upgrade Required)
     if (
         software_versions["harmony_version"] == software_versions["online_harmony_version"]
@@ -702,15 +710,15 @@
     check_for_install()
     print_stars()
     return
 
 
 # looks for ~/harmony or installs it if it's not there. Asks to overwrite if it finds it, run at your own risk.
 def check_for_install() -> str:
-    if os.path.exists(f'{EnvironmentVariables.user_home_dir}/harmony'):
+    if os.path.exists(f"{EnvironmentVariables.user_home_dir}/harmony"):
         question = ask_yes_no(
             "* You already have a harmony folder on this system, would you like to re-run installation and rclone on this server? (YES/NO)"
         )
         if question:
             install_harmony()
             print_stars()
             # Wallet Setup
@@ -720,18 +728,22 @@
             passphrase_status()
             print_stars()
             print("* All harmony files now installed. Database download starting now...")
             print_stars()
             clone_shards()
             finish_node_install()
         else:
-            if os.path.isdir(f'{EnvironmentVariables.user_home_dir}/harmony'):
-                print("* Exiting Harmony Validator Toolbox\n* You already have a folder at ~/harmony.\n* Contact Easy Node for help setting up if this is an existing Harmony server.")
-            if os.path.isfile(f'{EnvironmentVariables.user_home_dir}/harmony'):
-                print("* Exiting Harmony Validator Toolbox\n* You already have a file at ~/harmony.\n* Contact Easy Node for help setting up if this is an existing Harmony server with a custom configuration.")
+            if os.path.isdir(f"{EnvironmentVariables.user_home_dir}/harmony"):
+                print(
+                    "* Exiting Harmony Validator Toolbox\n* You already have a folder at ~/harmony.\n* Contact Easy Node for help setting up if this is an existing Harmony server."
+                )
+            if os.path.isfile(f"{EnvironmentVariables.user_home_dir}/harmony"):
+                print(
+                    "* Exiting Harmony Validator Toolbox\n* You already have a file at ~/harmony.\n* Contact Easy Node for help setting up if this is an existing Harmony server with a custom configuration."
+                )
             raise SystemExit(0)
     else:
         print(f"* You selected Shard: {environ.get('SHARD')}. ")
         install_harmony()
         print_stars()
         # Wallet Setup
         recover_wallet()
@@ -748,36 +760,45 @@
 
 # Installer Module
 def install_harmony() -> None:
     # Checks Passed at this point, only 1 folder in /mnt and it's probably our volume (can scope this down further later)
     print_stars()
     print("* Install Location")
     print_stars()
-    question = ask_yes_no(f"* Would you like to install Harmony in the folder ~/harmony on your main disk? (YES/NO)")
+    question = ask_yes_no(
+        f"* Answer yes if you'd like to setup harmony in the default location\n* {EnvironmentVariables.user_home_dir}/harmony\n* Or answer no to choose a custom folder (for a volume or 2nd disk setup): (YES/NO) "
+    )
     if question:
-        set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f'{EnvironmentVariables.user_home_dir}/harmony')
-        print_stars()
-        print("* Creating all Harmony Files & Folders")
-        os.system(f"mkdir -p {os.environ.get('HARMONY_DIR')}/.hmy/blskeys")
+        set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{EnvironmentVariables.user_home_dir}/harmony")
     else:
         answer = input(
-            "* If you'd like to use an alternative location or volume we can make a symlink.\n* What is the full path to your volume? (example: /mnt/mydisk) "
+            "\n* Please enter the full path to a location you'd like to install harmony into.\n* The folder should not exist yet for best results (example: /mnt/volume1/harmony): "
         )
         if not os.path.exists(answer):
-            print("* That path doesn't exist, please try again.")
-            install_harmony()
-        answer2 = input("* Re-enter the path to your volume: ")
-        if answer == answer2:
-            set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{answer}/harmony")
-            print_stars()
-            print("* Creating base folder, setting ownership & creating symlink.")
-            os.system(f"sudo mkdir -p {os.environ.get('HARMONY_DIR')}")
-            os.system(f"sudo chown {EnvironmentVariables.active_user} {os.environ.get('HARMONY_DIR')}")
-            os.system(f"mkdir -p {os.environ.get('HARMONY_DIR')}/.hmy/blskeys")
-            os.system(f"ln -s {os.environ.get('HARMONY_DIR')} {EnvironmentVariables.user_home_dir}/harmony")
+            question = ask_yes_no(
+                f"* That path {answer} doesn't exist yet.\n* Do you want to create the folder {answer} and install the harmony files here? (YES/NO) "
+            )
+            if question:
+                set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{answer}")
+            else:
+                install_harmony()
+        else:
+            question = ask_yes_no(
+                f"* Are you sure you want to isntall into the already existing folder {answer}? (YES/NO) "
+            )
+            if question:
+                set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{answer}")
+            else:
+                install_harmony()
+        set_var(EnvironmentVariables.dotenv_file, "HARMONY_DIR", f"{answer}")
+        os.system(f"sudo mkdir -p {os.environ.get('HARMONY_DIR')}")
+        os.system(f"sudo chown {EnvironmentVariables.active_user} {os.environ.get('HARMONY_DIR')}")
+    print_stars()
+    print("* Creating all Harmony Files & Folders")
+    os.system(f"mkdir -p {os.environ.get('HARMONY_DIR')}/.hmy/blskeys")
 
     # Setup folders now that symlink exists or we know we're using ~/harmony
     if not os.path.isdir(f"{EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/"):
         os.system(f"mkdir -p {EnvironmentVariables.user_home_dir}/.hmy_cli/account-keys/")
     if not os.path.isdir(f"{os.environ.get('HARMONY_DIR')}/.hmy/blskeys"):
         print("* Creating all Harmony Files & Folders")
         os.system(f"mkdir -p {os.environ.get('HARMONY_DIR')}/.hmy/blskeys")
@@ -805,22 +826,34 @@
 
     os.system(
         f"mkdir -p {EnvironmentVariables.user_home_dir}/.config/rclone && cp {EnvironmentVariables.toolbox_location}/src/bin/rclone.conf {EnvironmentVariables.user_home_dir}/.config/rclone/"
     )
     print_stars()
     # Setup the harmony service file
     print("* Customizing, Moving & Enabling your harmony.service systemd file")
-    if EnvironmentVariables.active_user == "root":
-        os.system(
-            f"sudo cp {EnvironmentVariables.toolbox_location}/src/bin/harmony.service . && sed -i 's/home\/serviceharmony/{EnvironmentVariables.active_user}/g' 'harmony.service' && sed -i 's/serviceharmony/{EnvironmentVariables.active_user}/g' 'harmony.service' && sudo mv harmony.service /etc/systemd/system/harmony.service && sudo chmod a-x /etc/systemd/system/harmony.service && sudo systemctl enable harmony.service"
-        )
-    else:
-        os.system(
-            f"sudo cp {EnvironmentVariables.toolbox_location}/src/bin/harmony.service . && sed -i 's/serviceharmony/{EnvironmentVariables.active_user}/g' 'harmony.service' && sudo mv harmony.service /etc/systemd/system/harmony.service && sudo chmod a-x /etc/systemd/system/harmony.service && sudo systemctl enable harmony.service"
-        )
+    service_file_path = f"{EnvironmentVariables.toolbox_location}/src/bin/harmony.service"
+    
+    # Read the service file
+    with open(service_file_path, 'r') as file:
+        filedata = file.read()
+
+    # Replace the paths with the value of HARMONY_DIR
+    harmony_dir = os.environ.get("HARMONY_DIR")
+    if harmony_dir:
+        filedata = filedata.replace('WorkingDirectory=/home/serviceharmony/harmony', f'WorkingDirectory={harmony_dir}')
+        filedata = filedata.replace('ExecStart=/home/serviceharmony/harmony/harmony -c harmony.conf', f'ExecStart={harmony_dir}/harmony -c harmony.conf')
+
+    # Write the file out again
+    with open('harmony.service', 'w') as file:
+        file.write(filedata)
+
+    # Move the modified service file into place, change the permissions and enable the service
+    subprocess.run(['sudo', 'mv', 'harmony.service', '/etc/systemd/system/harmony.service'], check=True)
+    subprocess.run(['sudo', 'chmod', 'a-x', '/etc/systemd/system/harmony.service'], check=True)
+    subprocess.run(['sudo', 'systemctl', 'enable', 'harmony.service'], check=True)
 
 
 # Database Downloader
 def clone_shards():
     # Move to ~/harmony
     os.chdir(f"{os.environ.get('HARMONY_DIR')}")
 
@@ -968,15 +1001,15 @@
         pathname = os.path.dirname(pathname)
         if pathname == HARMONY_DIR:
             break
         parent_device = os.stat(pathname).st_dev
     return HARMONY_DIR
 
 
-def refresh_stats() -> str:
+def refreshing_stats_message() -> str:
     print(Fore.GREEN)
     print_stars()
     print(f"* Getting the latest local & blockchain information now, one moment while we load...")
     print_stars()
     return
```

### Comparing `harmony_toolbox-1.1.0/src/toolbox/toolbox.py` & `harmony_toolbox-1.1.1/src/toolbox/toolbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from toolbox.library import (
     process_command,
     print_stars,
     print_stars,
     print_whitespace,
     ask_yes_no,
     return_txt,
-    install_harmony,
+    find_port,
     install_hmy,
     get_sign_pct,
     load_var_file,
     get_wallet_balance,
     get_rewards_balance,
     string_stars,
     set_var,
@@ -37,15 +37,15 @@
     validator_stats_output,
     get_db_size,
     first_setup,
     update_text_file,
     get_shard_menu,
     set_main_or_test,
     recover_wallet,
-    refresh_stats,
+    refreshing_stats_message,
     passphrase_status
 )
 
 
 def parse_flags(parser):
     print_stars()
     # Add the arguments
@@ -104,15 +104,15 @@
 
     if args.collect_send:
         rewards_collector(EnvironmentVariables.hmy_app, True, True)
         finish_node()
 
 
 def run_multistats():
-    refresh_stats()
+    refreshing_stats_message()
     folders = get_folders()
     validator_stats_output(folders)
     return
 
 
 def collect_rewards(networkCall):
     os.system(
@@ -191,15 +191,15 @@
     print(
         f'{Fore.GREEN}* Validator Toolbox for {Fore.CYAN}Harmony ONE{Fore.GREEN} Validators by Easy Node   v{environ.get("EASY_VERSION")}{Fore.WHITE}   https://easynode.pro {Fore.GREEN}*'
     )
     print_stars()
     print(
         f'* Your validator wallet address is: {Fore.RED}{str(environ.get("VALIDATOR_WALLET"))}{Fore.GREEN}\n* Your $ONE balance is:             {Fore.CYAN}{str(round(total_balance, 2))}{Fore.GREEN}\n* Your pending $ONE rewards are:    {Fore.CYAN}{str(round(get_rewards_balance(EnvironmentVariables.rpc_endpoints, environ.get("VALIDATOR_WALLET")), 2))}{Fore.GREEN}\n* Server Hostname & IP:             {Fore.BLUE}{EnvironmentVariables.server_host_name}{Fore.GREEN} - {Fore.YELLOW}{EnvironmentVariables.external_ip}{Fore.GREEN}'
     )
-    harmony_service_status()
+    harmony_service_status(environ.get("SERVICE_NAME", "harmony"))
     print(
         f'* Epoch Signing Percentage:         {Style.BRIGHT}{Fore.GREEN}{Back.BLUE}{sign_percentage} %{Style.RESET_ALL}{Fore.GREEN}\n* Current disk space free: {Fore.CYAN}{free_space_check(os.environ.get("HARMONY_DIR")): >6}{Fore.GREEN}\n* Current harmony version: {Fore.YELLOW}{software_versions["harmony_version"]}{Fore.GREEN}, has upgrade available: {software_versions["harmony_upgrade"]}\n* Current hmy version: {Fore.YELLOW}{software_versions["hmy_version"]}{Fore.GREEN}, has upgrade available: {software_versions["hmy_upgrade"]}'
     )
     print_stars()
     if environ.get("SHARD") != "0":
         print(
             f"* Note: Running on shard {environ.get('SHARD')}, Shard 0 is no longer needed locally and should be under 300MB\n* Remote Shard 0 Epoch: {remote_data_shard_0['result']['shard-chain-header']['epoch']}, Current Block: {literal_eval(remote_data_shard_0['result']['shard-chain-header']['number'])}, Local Shard 0 Size: {get_db_size(os.environ.get('HARMONY_DIR'), '0')}"
@@ -369,14 +369,16 @@
                 )
                 raise SystemExit(0)
         else:
             first_setup()
     # always set conf to 13 keys, shard max
     if os.path.exists(EnvironmentVariables.harmony_conf):
         update_text_file(EnvironmentVariables.harmony_conf, "MaxKeys = 10", "MaxKeys = 13")
+    if os.path.isfile(f"{os.environ.get('HARMONY_DIR')}/blskey.pass"):
+        update_text_file(EnvironmentVariables.harmony_conf, 'PassFile = ""', f'PassFile = "blskey.pass"')
     passphrase_status()
     get_shard_menu()
     set_main_or_test()
     if environ.get("VALIDATOR_WALLET") is None:
         # Recover wallet or have them add address
         recover_wallet()
 
@@ -424,23 +426,23 @@
         )
     else:
         print(f"*  20 - Enable Auto update        - Enable Update Timer")
 
 
 def start_regular_node() -> None:
     # Check online versions of harmony & hmy and compare to our local copy.
-    refresh_stats()
+    refreshing_stats_message()
     software_versions = version_checks(environ.get("HARMONY_DIR"))
     run_regular_node(software_versions)
 
 
 def run_regular_node(software_versions) -> None:
     menu_options = {
         0: finish_node,
-        1: refresh_stats,
+        1: refreshing_stats_message,
         2: menu_active_bls,
         3: coming_soon,
         4: run_rewards_collector,
         5: bingo_checker,
         6: coming_soon,
         7: set_rewards_wallet,
         8: menu_service_stop_start,
@@ -528,20 +530,20 @@
 
 def hmy_cli_upgrade():
     question = ask_yes_no(
         "* Are you sure you would like to proceed with updating the Harmony CLI file?\n\nType 'Yes' or 'No' to continue"
     )
     if question:
         folder_name = make_backup_dir()
-        os.system(f"cp {EnvironmentVariables.hmy_app} {folder_name}")
+        os.system(f"cp {environ.get('HARMONY_DIR')}/hmy {folder_name}")
         print_stars()
         install_hmy()
         print_stars()
         print("Harmony cli has been updated to: ")
-        os.system(f"{EnvironmentVariables.hmy_app} version")
+        os.system(f"{environ.get('HARMONY_DIR')}/hmy version")
         print_stars()
         set_var(EnvironmentVariables.dotenv_file, "HMY_UPGRADE_AVAILABLE", "False")
         input("* Update completed, press ENTER to return to the main menu. ")
 
 
 def update_harmony_app():
     os.chdir(f"{os.environ.get('HARMONY_DIR')}")
@@ -589,38 +591,39 @@
     set_var(EnvironmentVariables.dotenv_file, "HARMONY_UPGRADE_AVAILABLE", "False")
     time.sleep(10)
 
 
 def menu_validator_stats():
     load_var_file(EnvironmentVariables.dotenv_file)
     remote_shard_0 = [
-        f"{EnvironmentVariables.hmy_app}",
+        f"{environ.get('HARMONY_DIR')}/hmy",
         "blockchain",
         "latest-headers",
         f'--node=https://api.s0.{environ.get("NETWORK_SWITCH")}.hmny.io',
     ]
     try:
         result_remote_shard_0 = run(remote_shard_0, stdout=PIPE, stderr=PIPE, universal_newlines=True)
         remote_data_shard_0 = json.loads(result_remote_shard_0.stdout)
     except (ValueError, KeyError, TypeError) as e:
         print(f"* Remote Shard 0 Offline, Error {e}")
     try:
-        local_shard = [f"{EnvironmentVariables.hmy_app}", "blockchain", "latest-headers"]
+        http_port = find_port(environ.get('HARMONY_DIR'))
+        local_shard = [f"{environ.get('HARMONY_DIR')}/hmy", "blockchain", "latest-headers", "--node", f"http://localhost:{http_port}"]
         result_local_shard = run(local_shard, stdout=PIPE, stderr=PIPE, universal_newlines=True)
         local_data_shard = json.loads(result_local_shard.stdout)
     except (ValueError, KeyError, TypeError) as e:
         print(
             f"* Local Server Offline\n*\n* Run troubleshooting, See our documents site for info on how to manually troubleshoot:\n* https://docs.easynode.pro/harmony/post#validator-toolbox-troubleshooting\n*"
         )
         print_stars()
         finish_node()
 
     if environ.get("SHARD") != "0":
         remote_shard = [
-            f"{EnvironmentVariables.hmy_app}",
+            f"{environ.get('HARMONY_DIR')}/hmy",
             "blockchain",
             "latest-headers",
             f'--node=https://api.s{environ.get("SHARD")}.{environ.get("NETWORK_SWITCH")}.hmny.io',
         ]
         try:
             result_remote_shard = run(remote_shard, stdout=PIPE, stderr=PIPE, universal_newlines=True)
             remote_data_shard = json.loads(result_remote_shard.stdout)
```

