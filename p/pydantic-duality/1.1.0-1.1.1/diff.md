# Comparing `tmp/pydantic_duality-1.1.0.tar.gz` & `tmp/pydantic_duality-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_duality-1.1.0.tar", max compression
+gzip compressed data, was "pydantic_duality-1.1.1.tar", max compression
```

## Comparing `pydantic_duality-1.1.0.tar` & `pydantic_duality-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-02-23 13:56:20.496071 pydantic_duality-1.1.0/LICENSE
--rw-r--r--   0        0        0     3258 2023-03-12 10:41:12.573209 pydantic_duality-1.1.0/README.md
--rw-r--r--   0        0        0     9908 2023-03-11 14:27:52.366299 pydantic_duality-1.1.0/pydantic_duality/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 13:49:04.753350 pydantic_duality-1.1.0/pydantic_duality/py.typed
--rw-r--r--   0        0        0     1627 2023-03-16 19:05:48.210039 pydantic_duality-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4168 1970-01-01 00:00:00.000000 pydantic_duality-1.1.0/setup.py
--rw-r--r--   0        0        0     4033 1970-01-01 00:00:00.000000 pydantic_duality-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-23 13:56:20.496071 pydantic_duality-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3258 2023-03-12 10:41:12.573209 pydantic_duality-1.1.1/README.md
+-rw-r--r--   0        0        0     9908 2023-07-27 18:58:36.207041 pydantic_duality-1.1.1/pydantic_duality/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 13:49:04.753350 pydantic_duality-1.1.1/pydantic_duality/py.typed
+-rw-r--r--   0        0        0     1624 2023-07-27 18:58:46.577041 pydantic_duality-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 pydantic_duality-1.1.1/setup.py
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 pydantic_duality-1.1.1/PKG-INFO
```

### Comparing `pydantic_duality-1.1.0/LICENSE` & `pydantic_duality-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_duality-1.1.0/README.md` & `pydantic_duality-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_duality-1.1.0/pydantic_duality/__init__.py` & `pydantic_duality-1.1.1/pydantic_duality/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_duality-1.1.0/pyproject.toml` & `pydantic_duality-1.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "pydantic-duality"
-version = "1.1.0"
+version = "1.1.1"
 description = "Automatically generate two versions of your pydantic models: one with Extra.forbid and one with Extra.ignore"
 repository = "https://github.com/Ovsyanka83/pydantic-duality"
 readme = "README.md"
-authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
+authors = ["Stanislav Zmiev <zmievsa@gmail.com>"]
 license = "MIT"
 
 [tool.coverage.report]
 fail_under = 100
 skip_covered = true
 skip_empty = true
 omit = ["tests/*"]
```

### Comparing `pydantic_duality-1.1.0/setup.py` & `pydantic_duality-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 {'': ['*']}
 
 install_requires = \
 ['cached-classproperty>=0.1.0', 'pydantic>=1.9.2', 'typing-extensions>=4.4.0']
 
 setup_kwargs = {
     'name': 'pydantic-duality',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'Automatically generate two versions of your pydantic models: one with Extra.forbid and one with Extra.ignore',
     'long_description': '\n<p align="center">\n  <a href="https://ovsyanka83.github.io/pydantic-duality/"><img src="https://raw.githubusercontent.com/Ovsyanka83/pydantic-duality/main/docs/_media/logo_with_text.svg" alt="Pydantic Duality"></a>\n</p>\n<p align="center">\n  <b>Automatically and lazily generate three versions of your pydantic models: one with Extra.forbid, one with Extra.ignore, and one with all fields optional</b>\n</p>\n\n---\n\n<p align="center">\n<a href="https://github.com/ovsyanka83/pydantic-duality/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/Ovsyanka83/pydantic-duality/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://codecov.io/gh/ovsyanka83/pydantic-duality" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/pydantic-duality?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/pydantic-duality/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/pydantic-duality?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/pydantic-duality/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/pydantic-duality?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Installation\n\n```bash\npip install pydantic-duality\n```\n\n## Quickstart\n\nGiven the following models:\n\n```python\n\nfrom pydantic_duality import DualBaseModel\n\n\nclass User(DualBaseModel):\n    id: UUID\n    name: str\n\nclass Auth(DualBaseModel):\n    some_field: str\n    user: User\n```\n\nUsing pydantic-duality is roughly equivalent to making all of the following models by hand:\n\n```python\n\nfrom pydantic import BaseModel\n\n# Equivalent to User and User.__request__\nclass UserRequest(BaseModel, extra=Extra.forbid):\n    id: UUID\n    name: str\n\n# Rougly equivalent to Auth and Auth.__request__\nclass AuthRequest(BaseModel, extra=Extra.forbid):\n    some_field: str\n    user: UserRequest\n\n\n# Rougly equivalent to User.__response__\nclass UserResponse(BaseModel, extra=Extra.ignore):\n    id: UUID\n    name: str\n\n# Rougly equivalent to Auth.__response__\nclass AuthResponse(BaseModel, extra=Extra.ignore):\n    some_field: str\n    user: UserResponse\n\n\n# Rougly equivalent to User.__patch_request__\nclass UserPatchRequest(BaseModel, extra=Extra.forbid):\n    id: UUID | None\n    name: str | None\n\n# Rougly equivalent to Auth.__patch_request__\nclass AuthPatchRequest(BaseModel, extra=Extra.forbid):\n    some_field: str | None\n    user: UserPatchRequest | None\n\n```\n\nSo it takes you up to 3 times less code to write the same thing. Note also that pydantic-duality does everything lazily so you will not notice any significant performance or memory usage difference when using it instead of writing everything by hand. Think of it as using all the customized models as cached properties.\n\nInheritance, inner models, custom configs, [custom names](https://ovsyanka83.github.io/pydantic-duality/#/?id=customizing-schema-names), config kwargs, isinstance and subclass checks work intuitively and in the same manner as they would work if you were not using pydantic-duality.\n\n## Help\n\nSee [documentation](https://ovsyanka83.github.io/pydantic-duality/#/) for more details\n',
     'author': 'Stanislav Zmiev',
-    'author_email': 'szmiev2000@gmail.com',
+    'author_email': 'zmievsa@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Ovsyanka83/pydantic-duality',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['pydantic_duality'] package_data = \ {'': ['*']} install_requires = \
 ['cached-classproperty>=0.1.0', 'pydantic>=1.9.2', 'typing-extensions>=4.4.0']
-setup_kwargs = { 'name': 'pydantic-duality', 'version': '1.1.0', 'description':
+setup_kwargs = { 'name': 'pydantic-duality', 'version': '1.1.1', 'description':
 'Automatically generate two versions of your pydantic models: one with
 Extra.forbid and one with Extra.ignore', 'long_description': '\n
                             \n [Pydantic_Duality]\n
 \n
  \n Automatically and lazily generate three versions of your pydantic models:
      one with Extra.forbid, one with Extra.ignore, and one with all fields
                                   optional\n
@@ -33,12 +33,12 @@
 performance or memory usage difference when using it instead of writing
 everything by hand. Think of it as using all the customized models as cached
 properties.\n\nInheritance, inner models, custom configs, [custom names](https:
 //ovsyanka83.github.io/pydantic-duality/#/?id=customizing-schema-names), config
 kwargs, isinstance and subclass checks work intuitively and in the same manner
 as they would work if you were not using pydantic-duality.\n\n## Help\n\nSee
 [documentation](https://ovsyanka83.github.io/pydantic-duality/#/) for more
-details\n', 'author': 'Stanislav Zmiev', 'author_email':
-'szmiev2000@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'https://github.com/Ovsyanka83/pydantic-duality', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
+details\n', 'author': 'Stanislav Zmiev', 'author_email': 'zmievsa@gmail.com',
+'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
+Ovsyanka83/pydantic-duality', 'packages': packages, 'package_data':
+package_data, 'install_requires': install_requires, 'python_requires':
+'>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `pydantic_duality-1.1.0/PKG-INFO` & `pydantic_duality-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pydantic-duality
-Version: 1.1.0
+Version: 1.1.1
 Summary: Automatically generate two versions of your pydantic models: one with Extra.forbid and one with Extra.ignore
 Home-page: https://github.com/Ovsyanka83/pydantic-duality
 License: MIT
 Author: Stanislav Zmiev
-Author-email: szmiev2000@gmail.com
+Author-email: zmievsa@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cached-classproperty (>=0.1.0)
 Requires-Dist: pydantic (>=1.9.2)
```

