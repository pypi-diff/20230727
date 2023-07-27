# Comparing `tmp/pysh-3.3.0.tar.gz` & `tmp/pysh-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysh-3.3.0.tar", max compression
+gzip compressed data, was "pysh-3.3.1.tar", max compression
```

## Comparing `pysh-3.3.0.tar` & `pysh-3.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      870 2023-01-15 14:39:07.400013 pysh-3.3.0/README.md
--rw-r--r--   0        0        0      751 2023-01-15 15:48:31.393445 pysh-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     4001 2023-01-15 15:48:13.446778 pysh-3.3.0/pysh/__init__.py
--rw-r--r--   0        0        0        0 2022-09-25 11:27:23.499921 pysh-3.3.0/pysh/py.typed
--rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 pysh-3.3.0/setup.py
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 pysh-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0      870 2023-01-15 14:39:07.400013 pysh-3.3.1/README.md
+-rw-r--r--   0        0        0      748 2023-07-27 19:00:21.963709 pysh-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4001 2023-01-15 15:48:13.446778 pysh-3.3.1/pysh/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-25 11:27:23.499921 pysh-3.3.1/pysh/py.typed
+-rw-r--r--   0        0        0     1519 1970-01-01 00:00:00.000000 pysh-3.3.1/setup.py
+-rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 pysh-3.3.1/PKG-INFO
```

### Comparing `pysh-3.3.0/README.md` & `pysh-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pysh-3.3.0/pyproject.toml` & `pysh-3.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "pysh"
-version = "3.3.0"
+version = "3.3.1"
 description = "A library of small functions that simplify scripting in python"
-authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
+authors = ["Stanislav Zmiev <zmievsa@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Ovsyanka83/pysh"
 keywords = ["python", "shell", "bash", "script", "scripting", "pysh"]
 classifiers = [
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `pysh-3.3.0/pysh/__init__.py` & `pysh-3.3.1/pysh/__init__.py`

 * *Files identical despite different names*

### Comparing `pysh-3.3.0/setup.py` & `pysh-3.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 ['pysh']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pysh',
-    'version': '3.3.0',
+    'version': '3.3.1',
     'description': 'A library of small functions that simplify scripting in python',
     'long_description': '# pysh\n\nA library of small functions that simplify scripting in python\n\n## Installation\n\n```bash\npip install pysh\n```\n\n## Usage\n\n### sh\n\nRun a shell command and display the output:\n\n```python\nsh("git status")\n```\n\nCapture the output of a shell command:\n\n```python\nres = sh("git status", capture=True)\nprint(res.stdout)\n```\n\n### cd\n\nChange the current working directory:\n\n```python\ncd("path/to/dir")\n```\n\nChange the current working directory temporarily:\n\n```python\nwith cd("path/to/dir"):\n    sh("git status")\n```\n\n### env\n\nSet an environment variable:\n\n```python\nenv(var="value")\n```\n\nSet an environment variable temporarily:\n\n```python\nwith env(PGPASSWORD="MyPassword", PGUSER="postgres"):\n    sh("createdb -h localhost -p 5432 -O postgres mydb")\n```\n\n### which\n\nChecks whether an executable/script/builtin is available:\n\n```python\ngit_is_installed = which("git")\n```\n',
     'author': 'Stanislav Zmiev',
-    'author_email': 'szmiev2000@gmail.com',
+    'author_email': 'zmievsa@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Ovsyanka83/pysh',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `pysh-3.3.0/PKG-INFO` & `pysh-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pysh
-Version: 3.3.0
+Version: 3.3.1
 Summary: A library of small functions that simplify scripting in python
 Home-page: https://github.com/Ovsyanka83/pysh
 License: MIT
 Keywords: python,shell,bash,script,scripting,pysh
 Author: Stanislav Zmiev
-Author-email: szmiev2000@gmail.com
+Author-email: zmievsa@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

