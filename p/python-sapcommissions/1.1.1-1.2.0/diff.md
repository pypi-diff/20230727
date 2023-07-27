# Comparing `tmp/python-sapcommissions-1.1.1.tar.gz` & `tmp/python-sapcommissions-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sapcommissions-1.1.1.tar", last modified: Tue Jul  4 19:49:24 2023, max compression
+gzip compressed data, was "python-sapcommissions-1.2.0.tar", last modified: Thu Jul 27 12:24:39 2023, max compression
```

## Comparing `python-sapcommissions-1.1.1.tar` & `python-sapcommissions-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:49:24.046342 python-sapcommissions-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:49:24.042342 python-sapcommissions-1.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:49:24.042342 python-sapcommissions-1.1.1/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:49:24.046342 python-sapcommissions-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/.github/workflows/pr-labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:49:24.046342 python-sapcommissions-1.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-04 19:49:24.046342 python-sapcommissions-1.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:49:24.046342 python-sapcommissions-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/docs/ENDPOINTS.md
--rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/docs/METHODS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:49:24.046342 python-sapcommissions-1.1.1/python_sapcommissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-04 19:49:24.000000 python-sapcommissions-1.1.1/python_sapcommissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-04 19:49:24.000000 python-sapcommissions-1.1.1/python_sapcommissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:49:24.000000 python-sapcommissions-1.1.1/python_sapcommissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 19:49:24.000000 python-sapcommissions-1.1.1/python_sapcommissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-04 19:49:24.000000 python-sapcommissions-1.1.1/python_sapcommissions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:49:24.046342 python-sapcommissions-1.1.1/sapcommissions/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/sapcommissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58524 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/sapcommissions/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/sapcommissions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   114107 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/sapcommissions/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:49:24.046342 python-sapcommissions-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:49:24.046342 python-sapcommissions-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-04 19:49:14.000000 python-sapcommissions-1.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/workflows/pr-labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    57710 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/docs/ENDPOINTS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/docs/METHODS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-27 12:24:39.000000 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-27 12:24:39.000000 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:24:39.000000 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 12:24:39.000000 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 12:24:39.000000 python-sapcommissions-1.2.0/python_sapcommissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/sapcommissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/sapcommissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58524 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/sapcommissions/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/sapcommissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114107 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/sapcommissions/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:24:39.608487 python-sapcommissions-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 12:24:29.000000 python-sapcommissions-1.2.0/tox.ini
```

### Comparing `python-sapcommissions-1.1.1/.github/scripts/release.py` & `python-sapcommissions-1.2.0/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/.github/workflows/lint.yml` & `python-sapcommissions-1.2.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/.github/workflows/publish.yml` & `python-sapcommissions-1.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/.pre-commit-config.yaml` & `python-sapcommissions-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/LICENSE` & `python-sapcommissions-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/PKG-INFO` & `python-sapcommissions-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sapcommissions
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Python wrapper for the SAP Commissions API
 Author-email: Niels Perfors <niels.perfors1987@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
@@ -38,16 +38,16 @@
 ```text
 pip install python-sapcommissions
 ```
 
 ### REST API
 
 This project mimics the usage of the SAP Commissions REST API. Visit
-`https://{CALD}-{ENV}.callidusondemand.com/APIDocument` to read the full specification, replacing `CALD` with your
-tenant name, and `ENV` with your environment name.
+`https://{TENANT}.callidusondemand.com/APIDocument` to read the full specification, replacing `TENANT` with your
+tenant-id.
 
 ### Terminology
 
 Things to keep in mind while reading the documentation.
 
 | Keyword  | Description                                                                       |
 | -------- | --------------------------------------------------------------------------------- |
@@ -60,19 +60,19 @@
 To get started, import `Connection` and an endpoint of your choosing. In this example, we'll use `Participants`.
 
 ```py
 from sapcommissions import Connection
 from sapcommissions.endpoints import Participants
 ```
 
-Initialize a Connection by providing the tenant, environment, username, and password. Optionally, you can disable ssl
-verification, if you are having problems connecting to the API from your network.
+Initialize a Connection by providing the tenant, username, and password. Optionally, you can disable ssl verification,
+if you are having problems connecting to the API from your network.
 
 ```python
-prod = Connection("CALD", "PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=True)
+prod = Connection("CALD-PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=True)
 ```
 
 In this example we will use the `Participants` endpoint to get a list of all participants from the system. The `list()`
 method returns a `generator` object, to retrieve all `Participants`, you can convert the generator to a `list`,
 processes the `Participants` one-by-one in a `for-loop` or use a list comprehension to extract neccecery properties.
 
 ```py
```

### Comparing `python-sapcommissions-1.1.1/docs/ENDPOINTS.md` & `python-sapcommissions-1.2.0/docs/ENDPOINTS.md`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/docs/METHODS.md` & `python-sapcommissions-1.2.0/docs/METHODS.md`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/docs/README.md` & `python-sapcommissions-1.2.0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 ```text
 pip install python-sapcommissions
 ```
 
 ### REST API
 
 This project mimics the usage of the SAP Commissions REST API. Visit
-`https://{CALD}-{ENV}.callidusondemand.com/APIDocument` to read the full specification, replacing `CALD` with your
-tenant name, and `ENV` with your environment name.
+`https://{TENANT}.callidusondemand.com/APIDocument` to read the full specification, replacing `TENANT` with your
+tenant-id.
 
 ### Terminology
 
 Things to keep in mind while reading the documentation.
 
 | Keyword  | Description                                                                       |
 | -------- | --------------------------------------------------------------------------------- |
@@ -44,19 +44,19 @@
 To get started, import `Connection` and an endpoint of your choosing. In this example, we'll use `Participants`.
 
 ```py
 from sapcommissions import Connection
 from sapcommissions.endpoints import Participants
 ```
 
-Initialize a Connection by providing the tenant, environment, username, and password. Optionally, you can disable ssl
-verification, if you are having problems connecting to the API from your network.
+Initialize a Connection by providing the tenant, username, and password. Optionally, you can disable ssl verification,
+if you are having problems connecting to the API from your network.
 
 ```python
-prod = Connection("CALD", "PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=True)
+prod = Connection("CALD-PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=True)
 ```
 
 In this example we will use the `Participants` endpoint to get a list of all participants from the system. The `list()`
 method returns a `generator` object, to retrieve all `Participants`, you can convert the generator to a `list`,
 processes the `Participants` one-by-one in a `for-loop` or use a list comprehension to extract neccecery properties.
 
 ```py
```

### Comparing `python-sapcommissions-1.1.1/pyproject.toml` & `python-sapcommissions-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/python_sapcommissions.egg-info/PKG-INFO` & `python-sapcommissions-1.2.0/python_sapcommissions.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sapcommissions
-Version: 1.1.1
+Version: 1.2.0
 Summary: A Python wrapper for the SAP Commissions API
 Author-email: Niels Perfors <niels.perfors1987@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/niro1987/python-sapcommissions
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
@@ -38,16 +38,16 @@
 ```text
 pip install python-sapcommissions
 ```
 
 ### REST API
 
 This project mimics the usage of the SAP Commissions REST API. Visit
-`https://{CALD}-{ENV}.callidusondemand.com/APIDocument` to read the full specification, replacing `CALD` with your
-tenant name, and `ENV` with your environment name.
+`https://{TENANT}.callidusondemand.com/APIDocument` to read the full specification, replacing `TENANT` with your
+tenant-id.
 
 ### Terminology
 
 Things to keep in mind while reading the documentation.
 
 | Keyword  | Description                                                                       |
 | -------- | --------------------------------------------------------------------------------- |
@@ -60,19 +60,19 @@
 To get started, import `Connection` and an endpoint of your choosing. In this example, we'll use `Participants`.
 
 ```py
 from sapcommissions import Connection
 from sapcommissions.endpoints import Participants
 ```
 
-Initialize a Connection by providing the tenant, environment, username, and password. Optionally, you can disable ssl
-verification, if you are having problems connecting to the API from your network.
+Initialize a Connection by providing the tenant, username, and password. Optionally, you can disable ssl verification,
+if you are having problems connecting to the API from your network.
 
 ```python
-prod = Connection("CALD", "PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=True)
+prod = Connection("CALD-PRD", "MyUserName", "MySuperSecretPassword", verify_ssl=True)
 ```
 
 In this example we will use the `Participants` endpoint to get a list of all participants from the system. The `list()`
 method returns a `generator` object, to retrieve all `Participants`, you can convert the generator to a `list`,
 processes the `Participants` one-by-one in a `for-loop` or use a list comprehension to extract neccecery properties.
 
 ```py
```

### Comparing `python-sapcommissions-1.1.1/python_sapcommissions.egg-info/SOURCES.txt` & `python-sapcommissions-1.2.0/python_sapcommissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/sapcommissions/__init__.py` & `python-sapcommissions-1.2.0/sapcommissions/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 @dataclass(frozen=True)
 class Connection:
     """
     Connection variables used to connect with SAP Commissions.
     """
 
     tenant: str = field(repr=True)
-    environment: str = field(repr=True)
     username: str = field(repr=True)
     password: str = field(repr=False)
     verifySsl: bool = field(default=True, repr=False)
 
     @property
     def url(self) -> str:
         """Return the Commissions URL."""
-        return f"https://{self.tenant}-{self.environment}.callidusondemand.com"
+        return f"https://{self.tenant}.callidusondemand.com"
 
     @property
     def apiUrl(self) -> str:
         """Returns the base url for the Commissions REST API."""
         return self.url + "/api"
 
     @property
```

### Comparing `python-sapcommissions-1.1.1/sapcommissions/endpoints.py` & `python-sapcommissions-1.2.0/sapcommissions/endpoints.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/sapcommissions/resources.py` & `python-sapcommissions-1.2.0/sapcommissions/resources.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/tests/test_base.py` & `python-sapcommissions-1.2.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/tests/test_endpoints.py` & `python-sapcommissions-1.2.0/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `python-sapcommissions-1.1.1/tests/test_resources.py` & `python-sapcommissions-1.2.0/tests/test_resources.py`

 * *Files identical despite different names*

