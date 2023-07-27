# Comparing `tmp/certbot_dns_godaddy-0.2.4.tar.gz` & `tmp/certbot_dns_godaddy-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot_dns_godaddy-0.2.4.tar", max compression
+gzip compressed data, was "certbot_dns_godaddy-2.6.0.tar", max compression
```

## Comparing `certbot_dns_godaddy-0.2.4.tar` & `certbot_dns_godaddy-2.6.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10786 2023-07-14 05:49:16.095575 certbot_dns_godaddy-0.2.4/LICENSE.txt
--rw-r--r--   0        0        0     5610 2023-07-14 05:49:16.095575 certbot_dns_godaddy-0.2.4/README.md
--rw-r--r--   0        0        0     4686 2023-07-14 05:49:16.095575 certbot_dns_godaddy-0.2.4/certbot_dns_godaddy.py
--rw-r--r--   0        0        0     1501 2023-07-14 05:49:16.099575 certbot_dns_godaddy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 certbot_dns_godaddy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    10786 2023-07-27 12:26:07.042586 certbot_dns_godaddy-2.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     5343 2023-07-27 12:26:07.042586 certbot_dns_godaddy-2.6.0/README.md
+-rw-r--r--   0        0        0     4686 2023-07-27 12:26:07.042586 certbot_dns_godaddy-2.6.0/certbot_dns_godaddy.py
+-rw-r--r--   0        0        0     1468 2023-07-27 12:26:07.042586 certbot_dns_godaddy-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6820 1970-01-01 00:00:00.000000 certbot_dns_godaddy-2.6.0/PKG-INFO
```

### Comparing `certbot_dns_godaddy-0.2.4/LICENSE.txt` & `certbot_dns_godaddy-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot_dns_godaddy-0.2.4/README.md` & `certbot_dns_godaddy-2.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,31 +3,39 @@
 
 [![Version](https://img.shields.io/pypi/v/certbot-dns-godaddy.svg)](https://pypi.python.org/pypi/certbot-dns-godaddy) [![License: Apache](https://img.shields.io/pypi/l/certbot-dns-godaddy.svg)](https://github.com/miigotu/certbot-dns-godaddy/blob/master/LICENSE.txt) [![Docker image size](https://img.shields.io/docker/image-size/miigotu/certbot-dns-godaddy)](https://hub.docker.com/repository/docker/miigotu/certbot-dns-godaddy)
 
 [godaddy](https://www.godaddy.com/) DNS Authenticator plugin for [certbot](https://certbot.eff.org/).
 
 This plugin automates the process of completing a `dns-01` challenge by creating, and subsequently removing, `TXT` records using the godaddy [API](https://developer.godaddy.com/doc/endpoint/domains) via [lexicon](https://github.com/AnalogJ/lexicon).
 
-**Note:** This manual assumes certbot ≥ v1.7, which has improved the naming scheme for external plugins. If you cannot upgrade, please also refer to the Old option naming scheme\_ section below.
+**Note:** This manual assumes certbot 2.6.0, which has improved the naming scheme for external plugins.
 
 Installation
 ------------
 
-    pip install certbot-dns-godaddy
+    # create a virtual environment, to avoid conflicts
+    python3 -m venv /some/path
+
+    # use the pip in the virtual environment to install or update
+    /some/path/bin/pip install -U certbot-dns-godaddy
+
+    # yse the cerbot from the virtualenv, to avoid accidentally
+    # using one from a different environment that does not have this library
+    /some/path/bin/certbot
 
 Named Arguments
 ---------------
 
 To start using DNS authentication for godaddy, pass the following arguments on certbot's command line:
 
-Option|Description|
----|---|
-`--authenticator dns-godaddy`|select the authenticator plugin (Required)|
-`--dns-godaddy-credentials FILE`|godaddy credentials INI file. (Required)|
-`--dns-godaddy-propagation-seconds NUM`|waiting time for DNS to propagate before asking the ACME server to verify the DNS record. (Default: 30, Recommended: \>= 600)|
+| Option                                  | Description                                                                           |
+|-----------------------------------------|---------------------------------------------------------------------------------------|
+| `--authenticator dns-godaddy`           | select the authenticator plugin (Required)                                            |
+| `--dns-godaddy-credentials FILE`        | godaddy credentials INI file. (Required)                                              |
+| `--dns-godaddy-propagation-seconds NUM` | how long to wait before ACME tries to verify DNS. (Default: 30, Recommended: \>= 600) |
 
 You may need to set an unexpectedly high propagation time (≥ 900 seconds) to give the godaddy DNS time to propagate the entries! This may be annoying when calling certbot manually but should not be a problem in automated setups.
 
 Credentials
 -----------
 
 Use of this plugin requires a configuration file containing godaddy API credentials, obtained from your [developer.godaddy.com](https://developer.godaddy.com/).
@@ -78,25 +86,7 @@
         --dns-godaddy-credentials /var/lib/letsencrypt/godaddy_credentials.ini \
         --keep-until-expiring --non-interactive --expand \
         --server https://acme-v02.api.letsencrypt.org/directory \
         --agree-tos --email "webmaster@example.com" \
         -d example.com -d '*.example.com'
 
 You may want to change the volumes `/var/lib/letsencrypt` and `/etc/letsencrypt` to local directories where the certificates and configuration should be stored.
-
-Old option naming scheme
-------------------------
-
-It is recommended to use the newest certbot version, at least `v1.7`.
-
-If you're using a certbot version below `v1.7` all options related to external plugins (such as this one) must be prefixed by the name of the plugin. This means that every occurence of `dns-godaddy` in the command line options must be replaced by `certbot-dns-godaddy:dns-godaddy`, i.e.:
-
-    --authenticator certbot-dns-godaddy:dns-godaddy
-    --certbot-dns-godaddy:dns-godaddy-credentials
-    --certbot-dns-godaddy:dns-godaddy-propagation-seconds
-
-Further, every occurence of `dns_godaddy` in the config file must be prefixed by `certbot_dns_godaddy:`, resulting in a file like this:
-
-``` {.sourceCode .ini}
-certbot_dns_godaddy:dns_godaddy_key      = ...
-certbot_dns_godaddy:dns_godaddy_secret = ...
-```
```

### Comparing `certbot_dns_godaddy-0.2.4/certbot_dns_godaddy.py` & `certbot_dns_godaddy-2.6.0/certbot_dns_godaddy.py`

 * *Files identical despite different names*

### Comparing `certbot_dns_godaddy-0.2.4/pyproject.toml` & `certbot_dns_godaddy-2.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "certbot-dns-godaddy"
-version = "0.2.4"
+version = "2.6.0"
 description = "A certbot plugin that implements letsencrypt dns wildcard support for godaddy using lexicon"
 authors = ["Dustyn Gibson <miigotu@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/miigotu/certbot-dns-godaddy"
 
 packages = [{include = "certbot_dns_godaddy.py"}]
@@ -26,20 +26,19 @@
     "Topic :: System :: Installation/Setup",
     "Topic :: System :: Networking",
     "Topic :: System :: Systems Administration",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6,<4.0"
-acme = ">=0.31.0"
-certbot = ">=0.31.0,<2.0.0"
+python = ">=3.7,<4.0"
+acme = "2.6.0"
+certbot = "2.6.0"
 dns-lexicon = ">=3.2.3"
 "zope.interface" = ">=5.4.0"
-urllib3 = "^1.26.4"
 
 [tool.poetry.dev-dependencies]
 isort = "^5.8.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `certbot_dns_godaddy-0.2.4/PKG-INFO` & `certbot_dns_godaddy-2.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 Metadata-Version: 2.1
 Name: certbot-dns-godaddy
-Version: 0.2.4
+Version: 2.6.0
 Summary: A certbot plugin that implements letsencrypt dns wildcard support for godaddy using lexicon
 Home-page: https://github.com/miigotu/certbot-dns-godaddy
 License: Apache-2.0
 Author: Dustyn Gibson
 Author-email: miigotu@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
-Requires-Dist: acme (>=0.31.0)
-Requires-Dist: certbot (>=0.31.0,<2.0.0)
+Requires-Dist: acme (==2.6.0)
+Requires-Dist: certbot (==2.6.0)
 Requires-Dist: dns-lexicon (>=3.2.3)
-Requires-Dist: urllib3 (>=1.26.4,<2.0.0)
 Requires-Dist: zope.interface (>=5.4.0)
 Project-URL: Repository, https://github.com/miigotu/certbot-dns-godaddy
 Description-Content-Type: text/markdown
 
 certbot-dns-godaddy
 ==================
 
 [![Version](https://img.shields.io/pypi/v/certbot-dns-godaddy.svg)](https://pypi.python.org/pypi/certbot-dns-godaddy) [![License: Apache](https://img.shields.io/pypi/l/certbot-dns-godaddy.svg)](https://github.com/miigotu/certbot-dns-godaddy/blob/master/LICENSE.txt) [![Docker image size](https://img.shields.io/docker/image-size/miigotu/certbot-dns-godaddy)](https://hub.docker.com/repository/docker/miigotu/certbot-dns-godaddy)
 
 [godaddy](https://www.godaddy.com/) DNS Authenticator plugin for [certbot](https://certbot.eff.org/).
 
 This plugin automates the process of completing a `dns-01` challenge by creating, and subsequently removing, `TXT` records using the godaddy [API](https://developer.godaddy.com/doc/endpoint/domains) via [lexicon](https://github.com/AnalogJ/lexicon).
 
-**Note:** This manual assumes certbot ≥ v1.7, which has improved the naming scheme for external plugins. If you cannot upgrade, please also refer to the Old option naming scheme\_ section below.
+**Note:** This manual assumes certbot 2.6.0, which has improved the naming scheme for external plugins.
 
 Installation
 ------------
 
-    pip install certbot-dns-godaddy
+    # create a virtual environment, to avoid conflicts
+    python3 -m venv /some/path
+
+    # use the pip in the virtual environment to install or update
+    /some/path/bin/pip install -U certbot-dns-godaddy
+
+    # yse the cerbot from the virtualenv, to avoid accidentally
+    # using one from a different environment that does not have this library
+    /some/path/bin/certbot
 
 Named Arguments
 ---------------
 
 To start using DNS authentication for godaddy, pass the following arguments on certbot's command line:
 
-Option|Description|
----|---|
-`--authenticator dns-godaddy`|select the authenticator plugin (Required)|
-`--dns-godaddy-credentials FILE`|godaddy credentials INI file. (Required)|
-`--dns-godaddy-propagation-seconds NUM`|waiting time for DNS to propagate before asking the ACME server to verify the DNS record. (Default: 30, Recommended: \>= 600)|
+| Option                                  | Description                                                                           |
+|-----------------------------------------|---------------------------------------------------------------------------------------|
+| `--authenticator dns-godaddy`           | select the authenticator plugin (Required)                                            |
+| `--dns-godaddy-credentials FILE`        | godaddy credentials INI file. (Required)                                              |
+| `--dns-godaddy-propagation-seconds NUM` | how long to wait before ACME tries to verify DNS. (Default: 30, Recommended: \>= 600) |
 
 You may need to set an unexpectedly high propagation time (≥ 900 seconds) to give the godaddy DNS time to propagate the entries! This may be annoying when calling certbot manually but should not be a problem in automated setups.
 
 Credentials
 -----------
 
 Use of this plugin requires a configuration file containing godaddy API credentials, obtained from your [developer.godaddy.com](https://developer.godaddy.com/).
@@ -115,25 +122,7 @@
         --keep-until-expiring --non-interactive --expand \
         --server https://acme-v02.api.letsencrypt.org/directory \
         --agree-tos --email "webmaster@example.com" \
         -d example.com -d '*.example.com'
 
 You may want to change the volumes `/var/lib/letsencrypt` and `/etc/letsencrypt` to local directories where the certificates and configuration should be stored.
 
-Old option naming scheme
-------------------------
-
-It is recommended to use the newest certbot version, at least `v1.7`.
-
-If you're using a certbot version below `v1.7` all options related to external plugins (such as this one) must be prefixed by the name of the plugin. This means that every occurence of `dns-godaddy` in the command line options must be replaced by `certbot-dns-godaddy:dns-godaddy`, i.e.:
-
-    --authenticator certbot-dns-godaddy:dns-godaddy
-    --certbot-dns-godaddy:dns-godaddy-credentials
-    --certbot-dns-godaddy:dns-godaddy-propagation-seconds
-
-Further, every occurence of `dns_godaddy` in the config file must be prefixed by `certbot_dns_godaddy:`, resulting in a file like this:
-
-``` {.sourceCode .ini}
-certbot_dns_godaddy:dns_godaddy_key      = ...
-certbot_dns_godaddy:dns_godaddy_secret = ...
-```
-
```

