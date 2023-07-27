# Comparing `tmp/visier-connector-0.9.7.tar.gz` & `tmp/visier-connector-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visier-connector-0.9.7.tar", last modified: Tue Jun  6 23:32:22 2023, max compression
+gzip compressed data, was "visier-connector-0.9.8.tar", last modified: Thu Jul 27 20:01:47 2023, max compression
```

## Comparing `visier-connector-0.9.7.tar` & `visier-connector-0.9.8.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:32:22.780756 visier-connector-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 23:32:11.000000 visier-connector-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26297 2023-06-06 23:32:22.780756 visier-connector-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-06-06 23:32:11.000000 visier-connector-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 23:32:11.000000 visier-connector-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 23:32:22.780756 visier-connector-0.9.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:32:22.776756 visier-connector-0.9.7/visier/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:32:22.780756 visier-connector-0.9.7/visier/api/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/api/direct_intake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/api/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:32:22.780756 visier-connector-0.9.7/visier/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/connector/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/connector/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-06 23:32:11.000000 visier-connector-0.9.7/visier/connector/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 23:32:22.780756 visier-connector-0.9.7/visier_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26297 2023-06-06 23:32:22.000000 visier-connector-0.9.7/visier_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-06 23:32:22.000000 visier-connector-0.9.7/visier_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 23:32:22.000000 visier-connector-0.9.7/visier_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-06 23:32:22.000000 visier-connector-0.9.7/visier_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 23:32:22.000000 visier-connector-0.9.7/visier_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:47.153149 visier-connector-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 20:01:35.000000 visier-connector-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28774 2023-07-27 20:01:47.153149 visier-connector-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-07-27 20:01:35.000000 visier-connector-0.9.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-27 20:01:35.000000 visier-connector-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:01:47.153149 visier-connector-0.9.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:47.149149 visier-connector-0.9.8/visier/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:47.149149 visier-connector-0.9.8/visier/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/api/direct_intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/api/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:47.149149 visier-connector-0.9.8/visier/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-27 20:01:35.000000 visier-connector-0.9.8/visier/connector/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:01:47.149149 visier-connector-0.9.8/visier_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28774 2023-07-27 20:01:47.000000 visier-connector-0.9.8/visier_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-27 20:01:47.000000 visier-connector-0.9.8/visier_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:01:47.000000 visier-connector-0.9.8/visier_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 20:01:47.000000 visier-connector-0.9.8/visier_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 20:01:47.000000 visier-connector-0.9.8/visier_connector.egg-info/top_level.txt
```

### Comparing `visier-connector-0.9.7/LICENSE` & `visier-connector-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.7/PKG-INFO` & `visier-connector-0.9.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.7
+Version: 0.9.8
 Summary: Visier People Data connector
 Author-email: Visier Research & Development <info@visier.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,36 +220,67 @@
 The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
 * A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
 * That user's password
 
 ## Authentication Environment
-In order to avoid passing authentication credentials in via command line arguments, Visier recommends that basic authentication credentials such as username and password are provided via environment variables. 
+As of version `0.9.8`, the Visier Python Connector supports two means of authentication:
+1. OAuth2.0: The connector supports the so called three-legged authentication flow. This means that authentication (and consent) have to be provided through the authorization server. In accordance with the OAuth2.0 protocol, no user credentials are provided directly to Visier. This is the preferred authentication method.
+1. Basic Authentication: This is a traditional authentication mechanism where Visier username and password are provided directly to Visier for authentication.
+
+In order to avoid passing authentication credentials in via command line arguments, Visier recommends that at least basic authentication credentials such as username and password are provided via environment variables. However, using a new function, `make_auth()`, the appropriate authentication configuration object will be created from `VISIER_`-prefixed environment variables, as outlined  below.
+
+### OAuth2.0
+Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the OAuth2.0 authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
+* `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant as well as to initiate the OAuth2.0 authentication process
+* `VISIER_APIKEY`: The API key granted by Visier
+* `VISIER_CLIENT_ID`: The identifier of the pre-registered application
+* `VISIER_REDIRECT_URI`: The URI the `authorize` call will ultimately redirect to upon a successful authorization code generation. By default, this will be `http://localhost:5000/oauth2/callback` however note that it must match the `redirect_uri` in the client application definition exactly. If the client application setting is different, it is essential that that exact value is provided to the connector.
+* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations
+
+On Linux-like systems, with an X-display available, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
+```sh
+export VISIER_HOST=https://customer-specific.api.visier.io
+export VISIER_CLIENT_ID=client-id
+export VISIER_APIKEY=the-api-key-issued-by-visier
+export VISIER_REDIRECT_URI=
+# export VISIER_REDIRECT_URI=http://localhost:5000/oauth2/callback
+export VISIER_TARGET_TENANT_ID=
+export VISIER_USERNAME=
+export VISIER_PASSWORD=
+```
 
-Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the various authentication parameters
+Source this file in and the environment is ready for using the connector with OAuth2.0 authentication:
+```sh
+$ source .env
+```
+
+### Basic Authentication
+Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the basic authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
 * `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant
 * `VISIER_USERNAME`: The user name with sufficient API capabilities
 * `VISIER_PASSWORD`: The password of that user
 * `VISIER_APIKEY`: The API key granted by Visier
 * `VISIER_VANITY`: The readable name of the customer organization
-* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations.
+* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations
 
 To illustrate this process, consider the following example approach suitable in a non-production environment:
 
 On Linux-like systems, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
 ```sh
 echo -n "Enter the password for the Visier API User: "
 read -s vpwd
-export VISIER_VANITY=example
+export VISIER_VANITY=customer-specific
 export VISIER_HOST=https://$VISIER_VANITY.api.visier.io
 export VISIER_USERNAME=apiuser@example.com
 export VISIER_PASSWORD=$vpwd
 export VISIER_TARGET_TENANT_ID=tenant-code
 export VISIER_APIKEY=the-api-key-issued-by-visier
+export VISIER_CLIENT_ID=
 ```
 
 Source this environment in and provide the password when prompted:
 ```sh
 $ source .env
 ```
 
@@ -279,31 +310,25 @@
  
 A small set of example queries have been provided. Generally, Visier Query API queries fall into one of two categories:
 1. **Detail query** - These queries produce tabular results from underlying individual analytic objects. The shape of the result is inherently tabular with each table attribute represented as a column in the result set. Detail queries are often referred to as `list` or even `drill-through` queries. This query provides a detailed, non-aggregated view of the underlying analytical objects.
 1. **Aggregate query** - These queries aggregate metric values. They do so along the axes defined for the query and they produce multi-dimensional cell sets by default However, by providing an `Accept` header whose first value is either `application/jsonlines` or `text/csv`, the server will flatten the cell set into a tabular format when building the response.
 
 Visier also offers an experimental alternative to the JSON-based query definitions: SQL-like. This allows you to make queries using a language that comes close to SQL, which is generally more compact and intuitive. SQL-like allows definition of both aggregate and detail queries.
 
-:warning: **SQL-like is in alpha stage and not yet suitable for production use**.
-
 Example queries are provided through individual _files_. This is merely for convenience. SQL-like, being simple strings, can easily be provided to the call itself.
 
-In order to reduce duplication, each provided sample below should be preceded by the necessary `import` statements as well as authentication credential definition:
+In order to reduce duplication, each provided sample below should be preceded by the necessary `import` statements as well as authentication credential definition (note the use of pandas here is only demo purposes. The Visier Python Connector does not depend on pandas):
 ```python
 import os
-from visier.connector import Authentication, VisierSession
+from visier.connector import VisierSession, make_auth
 from visier.api import QueryApiClient
 from examples import load_json, load_str
 import pandas as pd
 
-auth = Authentication(
-    username = os.getenv("SOME_USERNAME"),
-    password = os.getenv("SOME_PASSWORD"),
-    host = os.getenv("SOME_HOST"),
-    api_key = os.getenv("SOME_APIKEY"))
+auth = make_auth()
 ```
 
 ### Detail Query
 This is an example of a snippet that may be added to something that loads detailed data such as a Jupyter Notebook. Detailed data is essentially granular, non-aggregated data from Visier entities. For example, subjects such as `Employee` or events such as `Compensation_Payout`.
 ```python
 with VisierSession(auth) as s:
     client = QueryApiClient(s)
```

### Comparing `visier-connector-0.9.7/README.md` & `visier-connector-0.9.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -8,36 +8,67 @@
 The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
 * A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
 * That user's password
 
 ## Authentication Environment
-In order to avoid passing authentication credentials in via command line arguments, Visier recommends that basic authentication credentials such as username and password are provided via environment variables. 
+As of version `0.9.8`, the Visier Python Connector supports two means of authentication:
+1. OAuth2.0: The connector supports the so called three-legged authentication flow. This means that authentication (and consent) have to be provided through the authorization server. In accordance with the OAuth2.0 protocol, no user credentials are provided directly to Visier. This is the preferred authentication method.
+1. Basic Authentication: This is a traditional authentication mechanism where Visier username and password are provided directly to Visier for authentication.
+
+In order to avoid passing authentication credentials in via command line arguments, Visier recommends that at least basic authentication credentials such as username and password are provided via environment variables. However, using a new function, `make_auth()`, the appropriate authentication configuration object will be created from `VISIER_`-prefixed environment variables, as outlined  below.
+
+### OAuth2.0
+Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the OAuth2.0 authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
+* `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant as well as to initiate the OAuth2.0 authentication process
+* `VISIER_APIKEY`: The API key granted by Visier
+* `VISIER_CLIENT_ID`: The identifier of the pre-registered application
+* `VISIER_REDIRECT_URI`: The URI the `authorize` call will ultimately redirect to upon a successful authorization code generation. By default, this will be `http://localhost:5000/oauth2/callback` however note that it must match the `redirect_uri` in the client application definition exactly. If the client application setting is different, it is essential that that exact value is provided to the connector.
+* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations
+
+On Linux-like systems, with an X-display available, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
+```sh
+export VISIER_HOST=https://customer-specific.api.visier.io
+export VISIER_CLIENT_ID=client-id
+export VISIER_APIKEY=the-api-key-issued-by-visier
+export VISIER_REDIRECT_URI=
+# export VISIER_REDIRECT_URI=http://localhost:5000/oauth2/callback
+export VISIER_TARGET_TENANT_ID=
+export VISIER_USERNAME=
+export VISIER_PASSWORD=
+```
 
-Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the various authentication parameters
+Source this file in and the environment is ready for using the connector with OAuth2.0 authentication:
+```sh
+$ source .env
+```
+
+### Basic Authentication
+Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the basic authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
 * `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant
 * `VISIER_USERNAME`: The user name with sufficient API capabilities
 * `VISIER_PASSWORD`: The password of that user
 * `VISIER_APIKEY`: The API key granted by Visier
 * `VISIER_VANITY`: The readable name of the customer organization
-* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations.
+* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations
 
 To illustrate this process, consider the following example approach suitable in a non-production environment:
 
 On Linux-like systems, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
 ```sh
 echo -n "Enter the password for the Visier API User: "
 read -s vpwd
-export VISIER_VANITY=example
+export VISIER_VANITY=customer-specific
 export VISIER_HOST=https://$VISIER_VANITY.api.visier.io
 export VISIER_USERNAME=apiuser@example.com
 export VISIER_PASSWORD=$vpwd
 export VISIER_TARGET_TENANT_ID=tenant-code
 export VISIER_APIKEY=the-api-key-issued-by-visier
+export VISIER_CLIENT_ID=
 ```
 
 Source this environment in and provide the password when prompted:
 ```sh
 $ source .env
 ```
 
@@ -67,31 +98,25 @@
  
 A small set of example queries have been provided. Generally, Visier Query API queries fall into one of two categories:
 1. **Detail query** - These queries produce tabular results from underlying individual analytic objects. The shape of the result is inherently tabular with each table attribute represented as a column in the result set. Detail queries are often referred to as `list` or even `drill-through` queries. This query provides a detailed, non-aggregated view of the underlying analytical objects.
 1. **Aggregate query** - These queries aggregate metric values. They do so along the axes defined for the query and they produce multi-dimensional cell sets by default However, by providing an `Accept` header whose first value is either `application/jsonlines` or `text/csv`, the server will flatten the cell set into a tabular format when building the response.
 
 Visier also offers an experimental alternative to the JSON-based query definitions: SQL-like. This allows you to make queries using a language that comes close to SQL, which is generally more compact and intuitive. SQL-like allows definition of both aggregate and detail queries.
 
-:warning: **SQL-like is in alpha stage and not yet suitable for production use**.
-
 Example queries are provided through individual _files_. This is merely for convenience. SQL-like, being simple strings, can easily be provided to the call itself.
 
-In order to reduce duplication, each provided sample below should be preceded by the necessary `import` statements as well as authentication credential definition:
+In order to reduce duplication, each provided sample below should be preceded by the necessary `import` statements as well as authentication credential definition (note the use of pandas here is only demo purposes. The Visier Python Connector does not depend on pandas):
 ```python
 import os
-from visier.connector import Authentication, VisierSession
+from visier.connector import VisierSession, make_auth
 from visier.api import QueryApiClient
 from examples import load_json, load_str
 import pandas as pd
 
-auth = Authentication(
-    username = os.getenv("SOME_USERNAME"),
-    password = os.getenv("SOME_PASSWORD"),
-    host = os.getenv("SOME_HOST"),
-    api_key = os.getenv("SOME_APIKEY"))
+auth = make_auth()
 ```
 
 ### Detail Query
 This is an example of a snippet that may be added to something that loads detailed data such as a Jupyter Notebook. Detailed data is essentially granular, non-aggregated data from Visier entities. For example, subjects such as `Employee` or events such as `Compensation_Payout`.
 ```python
 with VisierSession(auth) as s:
     client = QueryApiClient(s)
```

### Comparing `visier-connector-0.9.7/pyproject.toml` & `visier-connector-0.9.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 requires-python = ">=3.8"
 keywords = ["visier", "data", "query", "connector", "api"]
 license = {file = "LICENSE"}
 dynamic = ["version"]
 dependencies = [
     "requests >= 2.31",
     "deprecated",
+    "flask",
 ]
 
 [tool.poetry]
 readme = "README.md"
 
 [tool.setuptools.dynamic]
 version = {attr = "visier.__version__"}
```

### Comparing `visier-connector-0.9.7/visier/api/__init__.py` & `visier-connector-0.9.8/visier/api/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.7/visier/api/base.py` & `visier-connector-0.9.8/visier/api/base.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.7/visier/api/direct_intake.py` & `visier-connector-0.9.8/visier/api/direct_intake.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.7/visier/api/model.py` & `visier-connector-0.9.8/visier/api/model.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.7/visier/api/query.py` & `visier-connector-0.9.8/visier/api/query.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.7/visier/connector/__init__.py` & `visier-connector-0.9.8/visier/connector/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Public Python Connector
 """
 
-from .authentication import Authentication
+from .authentication import Authentication, Basic, OAuth2, add_auth_arguments, make_auth
 from .sessions import VisierSession, SessionContext, QueryExecutionError
 from .table import ResultTable
```

### Comparing `visier-connector-0.9.7/visier/connector/sessions.py` & `visier-connector-0.9.8/visier/connector/sessions.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Session object through which JSON as well as SQL-like queries are executed.
 """
 
+import os
 from typing import Callable
+import webbrowser
+from queue import Empty
+import urllib.parse
 import requests
 from requests import Session, Response
 from deprecated import deprecated
 from .table import ResultTable
-from .authentication import Authentication
-from .constants import TARGET_TENANT_ID
+from .authentication import Authentication, OAuth2, Basic
+from .constants import TARGET_TENANT_ID, ENV_VISIER_OAUTH_CALLBACK_URL
+from .callback import CallbackServer, CallbackBinding
 
 
 class QueryExecutionError(Exception):
     """Description of error from executing a query"""
     def __init__(self, status_code, message) -> None:
         self.args = (f"""The query execution failed with the following
         HTTP status code: {status_code}
@@ -39,14 +44,26 @@
         return self._status_code
 
     def message(self) -> str:
         """Returns the error message"""
         return self._message
 
 
+class OAuthConnectError(Exception):
+    """Raised when there is an error connecting to Visier using OAuth2"""
+    def __init__(self, message) -> None:
+        self.args = (f"""The OAuth2 connection failed with the following error:
+        {message}""", )
+        self._message = message
+
+    def message(self) -> str:
+        """Returns the error message"""
+        return self._message
+
+
 class SessionContext:
     """
     Context object passed to the user-defined function in the execute() method.
     """
     def __init__(self, session: Session, host: str, target_tenant_id: str = None) -> None:
         self._session = session
         self._host = host
@@ -76,14 +93,15 @@
     auth -- Authentication configuration
     """
     HEADER = {"Accept": "application/jsonlines, application/json"}
 
     def __init__(self, auth: Authentication) -> None:
         self._auth = auth
         self._session = None
+        self._timeout = 30
 
     @deprecated(version="0.9.5", reason="Use visier.api.QueryApiClient instead")
     def execute_aggregate(self, query_def: object):
         """Execute a Visier aggregate query and return a tabular result."""
         return self._execute_query_api("/v1/data/query/aggregate", query_def)
 
     @deprecated(version="0.9.5", reason="Use visier.api.QueryApiClient instead")
@@ -133,23 +151,85 @@
         principals to execute queries in the customer tenants."""
         result = self.execute(lambda s: s.session().post(url=s.mk_url(path),
                                                          json=body,
                                                          headers=self.HEADER))
         return ResultTable(result.iter_lines())
 
     def _connect(self):
-        url = self._auth.host + "/v1/admin/visierSecureToken"
-        body = {'username': self._auth.username, 'password': self._auth.password}
-        if self._auth.vanity:
-            body["vanityName"] = self._auth.vanity
-        result = requests.post(url=url, data=body, timeout=30)
+        """Connect to Visier using either OAuth or basic authentication."""
+        if isinstance(self._auth, OAuth2):
+            self.connect_oauth(self._auth)
+        else:
+            self.connect_basic(self._auth)
+
+    def connect_oauth(self, auth: OAuth2):
+        """Connect to Visier using (three-legged) OAuth2.
+        This method will attempt to open a browser for the authentication and consent screens.
+        It will also spin up a local web server to receive the OAuth2 authorization code."""
+        url_prefix = auth.host + "/v1/auth/oauth2"
+
+        def get_token(code: str) -> str:
+            url = url_prefix + "/token"
+            body = {
+                "grant_type": "authorization_code",
+                "client_id": auth.client_id,
+                "scope": "read",
+                "code": code
+            }
+            # if we have a redirect_uri when getting the auth code, we also must include it in the token
+            # request as part of the grant. https://datatracker.ietf.org/doc/html/rfc6749#section-4.1.3
+            if auth.redirect_uri:
+                body["redirect_uri"] = auth.redirect_uri
+            response = requests.post(url=url, data=body, headers={"apikey": auth.api_key}, timeout=self._timeout)
+            response.raise_for_status()
+            response = response.json()
+            # Currently not using refresh_token and id_token
+            # refresh_token = response['refresh_token']
+            # id_token = response['id_token']
+            return response['access_token']
+
+        def update_session(token: str) -> None:
+            headers = {
+                "Authorization": f"Bearer {token}",
+                "apikey": auth.api_key
+            }
+            self._session = Session()
+            self._session.headers.update(headers)
+
+        callback_url = os.getenv(ENV_VISIER_OAUTH_CALLBACK_URL)
+        binding = CallbackBinding(callback_url)
+        with CallbackServer(binding) as svr:
+            if auth.redirect_uri:
+                redirect_uri_arg = f"&redirect_uri={urllib.parse.quote(auth.redirect_uri, safe='')}"
+            else:
+                redirect_uri_arg = "" # Empty means use the redirect_uri registered with Visier
+            browser_url = f'{url_prefix}/authorize?apikey={auth.api_key}&response_type=code&client_id={auth.client_id}{redirect_uri_arg}'
+            # Launch the browser for authentication and consent screens
+            webbrowser.open(browser_url)
+            try:
+                # Wait up to 5 minutes for the user to complete the OAuth2 code flow
+                code = svr.queue.get(block=True, timeout=300)
+                update_session(get_token(code))
+            except Empty as empty:
+                raise OAuthConnectError("Timed out waiting for OAuth2 auth code") from empty
+
+    def connect_basic(self, auth: Basic):
+        """Connect to Visier using Basic Authentication."""
+        def update_session(asid_token: str):
+            self._session = Session()
+            self._session.cookies["VisierASIDToken"] = asid_token
+            self._session.headers.update({"apikey": auth.api_key})
+
+        url = auth.host + "/v1/admin/visierSecureToken"
+        body = {'username': auth.username, 'password': auth.password}
+        if auth.vanity:
+            body["vanityName"] = auth.vanity
+        result = requests.post(url=url, data=body, timeout=self._timeout)
         result.raise_for_status()
 
         # Only create a requests.Session once we have a Visier ASID Token
-        asid_token = result.text
-        self._session = Session()
-        self._session.cookies["VisierASIDToken"] = asid_token
-        self._session.headers.update({"apikey": self._auth.api_key})
+        update_session(result.text)
 
     def close(self):
         """Close the session."""
         self._session.close()
+        self._session = None
```

### Comparing `visier-connector-0.9.7/visier/connector/table.py` & `visier-connector-0.9.8/visier/connector/table.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.7/visier_connector.egg-info/PKG-INFO` & `visier-connector-0.9.8/visier_connector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.7
+Version: 0.9.8
 Summary: Visier People Data connector
 Author-email: Visier Research & Development <info@visier.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,36 +220,67 @@
 The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
 * A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
 * That user's password
 
 ## Authentication Environment
-In order to avoid passing authentication credentials in via command line arguments, Visier recommends that basic authentication credentials such as username and password are provided via environment variables. 
+As of version `0.9.8`, the Visier Python Connector supports two means of authentication:
+1. OAuth2.0: The connector supports the so called three-legged authentication flow. This means that authentication (and consent) have to be provided through the authorization server. In accordance with the OAuth2.0 protocol, no user credentials are provided directly to Visier. This is the preferred authentication method.
+1. Basic Authentication: This is a traditional authentication mechanism where Visier username and password are provided directly to Visier for authentication.
+
+In order to avoid passing authentication credentials in via command line arguments, Visier recommends that at least basic authentication credentials such as username and password are provided via environment variables. However, using a new function, `make_auth()`, the appropriate authentication configuration object will be created from `VISIER_`-prefixed environment variables, as outlined  below.
+
+### OAuth2.0
+Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the OAuth2.0 authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
+* `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant as well as to initiate the OAuth2.0 authentication process
+* `VISIER_APIKEY`: The API key granted by Visier
+* `VISIER_CLIENT_ID`: The identifier of the pre-registered application
+* `VISIER_REDIRECT_URI`: The URI the `authorize` call will ultimately redirect to upon a successful authorization code generation. By default, this will be `http://localhost:5000/oauth2/callback` however note that it must match the `redirect_uri` in the client application definition exactly. If the client application setting is different, it is essential that that exact value is provided to the connector.
+* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations
+
+On Linux-like systems, with an X-display available, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
+```sh
+export VISIER_HOST=https://customer-specific.api.visier.io
+export VISIER_CLIENT_ID=client-id
+export VISIER_APIKEY=the-api-key-issued-by-visier
+export VISIER_REDIRECT_URI=
+# export VISIER_REDIRECT_URI=http://localhost:5000/oauth2/callback
+export VISIER_TARGET_TENANT_ID=
+export VISIER_USERNAME=
+export VISIER_PASSWORD=
+```
 
-Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the various authentication parameters
+Source this file in and the environment is ready for using the connector with OAuth2.0 authentication:
+```sh
+$ source .env
+```
+
+### Basic Authentication
+Though the Visier Python Connector doesn't directly interact with the environment variables, the following list and example below illustrate the basic authentication parameters. These are also the environment variables the `make_auth()` utility function will use.
 * `VISIER_HOST`: The fully qualified domain name and protocol to access your Visier tenant
 * `VISIER_USERNAME`: The user name with sufficient API capabilities
 * `VISIER_PASSWORD`: The password of that user
 * `VISIER_APIKEY`: The API key granted by Visier
 * `VISIER_VANITY`: The readable name of the customer organization
-* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations.
+* `VISIER_TARGET_TENANT_ID`: The technical name of the tenant for the customer. This is only applicable in partner configurations
 
 To illustrate this process, consider the following example approach suitable in a non-production environment:
 
 On Linux-like systems, create a file named `.env` and populate it like the following example, substituting with actual values as appropriate:
 ```sh
 echo -n "Enter the password for the Visier API User: "
 read -s vpwd
-export VISIER_VANITY=example
+export VISIER_VANITY=customer-specific
 export VISIER_HOST=https://$VISIER_VANITY.api.visier.io
 export VISIER_USERNAME=apiuser@example.com
 export VISIER_PASSWORD=$vpwd
 export VISIER_TARGET_TENANT_ID=tenant-code
 export VISIER_APIKEY=the-api-key-issued-by-visier
+export VISIER_CLIENT_ID=
 ```
 
 Source this environment in and provide the password when prompted:
 ```sh
 $ source .env
 ```
 
@@ -279,31 +310,25 @@
  
 A small set of example queries have been provided. Generally, Visier Query API queries fall into one of two categories:
 1. **Detail query** - These queries produce tabular results from underlying individual analytic objects. The shape of the result is inherently tabular with each table attribute represented as a column in the result set. Detail queries are often referred to as `list` or even `drill-through` queries. This query provides a detailed, non-aggregated view of the underlying analytical objects.
 1. **Aggregate query** - These queries aggregate metric values. They do so along the axes defined for the query and they produce multi-dimensional cell sets by default However, by providing an `Accept` header whose first value is either `application/jsonlines` or `text/csv`, the server will flatten the cell set into a tabular format when building the response.
 
 Visier also offers an experimental alternative to the JSON-based query definitions: SQL-like. This allows you to make queries using a language that comes close to SQL, which is generally more compact and intuitive. SQL-like allows definition of both aggregate and detail queries.
 
-:warning: **SQL-like is in alpha stage and not yet suitable for production use**.
-
 Example queries are provided through individual _files_. This is merely for convenience. SQL-like, being simple strings, can easily be provided to the call itself.
 
-In order to reduce duplication, each provided sample below should be preceded by the necessary `import` statements as well as authentication credential definition:
+In order to reduce duplication, each provided sample below should be preceded by the necessary `import` statements as well as authentication credential definition (note the use of pandas here is only demo purposes. The Visier Python Connector does not depend on pandas):
 ```python
 import os
-from visier.connector import Authentication, VisierSession
+from visier.connector import VisierSession, make_auth
 from visier.api import QueryApiClient
 from examples import load_json, load_str
 import pandas as pd
 
-auth = Authentication(
-    username = os.getenv("SOME_USERNAME"),
-    password = os.getenv("SOME_PASSWORD"),
-    host = os.getenv("SOME_HOST"),
-    api_key = os.getenv("SOME_APIKEY"))
+auth = make_auth()
 ```
 
 ### Detail Query
 This is an example of a snippet that may be added to something that loads detailed data such as a Jupyter Notebook. Detailed data is essentially granular, non-aggregated data from Visier entities. For example, subjects such as `Employee` or events such as `Compensation_Payout`.
 ```python
 with VisierSession(auth) as s:
     client = QueryApiClient(s)
```

