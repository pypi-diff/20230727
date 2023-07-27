# Comparing `tmp/pyprocessors_openai_completion-0.5.81.tar.gz` & `tmp/pyprocessors-openai_completion-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors_openai_completion-0.5.81.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprocessors-openai_completion-0.5.9.tar", last modified: Wed Feb 15 16:28:15 2023, max compression
```

## Comparing `pyprocessors_openai_completion-0.5.81.tar` & `pyprocessors-openai_completion-0.5.9.tar`

### file list

```diff
@@ -1,35 +1,14 @@
--rw-r--r--   0        0        0       97 2023-06-07 12:04:27.485906 pyprocessors_openai_completion-0.5.81/.dockerignore
--rw-r--r--   0        0        0      147 2023-06-07 12:04:27.486906 pyprocessors_openai_completion-0.5.81/.gitignore
--rw-r--r--   0        0        0      448 2023-06-07 12:04:27.487906 pyprocessors_openai_completion-0.5.81/Dockerfile
--rw-r--r--   0        0        0    10227 2023-06-07 12:04:27.488906 pyprocessors_openai_completion-0.5.81/Jenkinsfile
--rw-r--r--   0        0        0      380 2023-06-07 12:04:27.489906 pyprocessors_openai_completion-0.5.81/README.md
--rw-r--r--   0        0        0     1559 2023-06-07 12:04:27.490906 pyprocessors_openai_completion-0.5.81/bumpversion.py
--rw-r--r--   0        0        0       56 2023-07-27 14:44:19.359702 pyprocessors_openai_completion-0.5.81/pyprocessors_openai_completion/__init__.py
--rw-r--r--   0        0        0    17365 2023-07-27 14:42:06.619928 pyprocessors_openai_completion-0.5.81/pyprocessors_openai_completion/openai_completion.py
--rw-r--r--   0        0        0     1923 2023-06-07 12:04:27.493906 pyprocessors_openai_completion-0.5.81/pyprocessors_openai_completion/retry_limit.py
--rw-r--r--   0        0        0     2594 2023-07-27 10:11:40.494783 pyprocessors_openai_completion-0.5.81/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 12:04:27.494906 pyprocessors_openai_completion-0.5.81/tests/__init__.py
--rw-r--r--   0        0        0      674 2023-06-07 12:04:27.496906 pyprocessors_openai_completion-0.5.81/tests/data/complexdoc.json
--rw-r--r--   0        0        0     3992 2023-06-07 12:04:27.498906 pyprocessors_openai_completion-0.5.81/tests/data/en_davinci-instruct-beta.json
--rw-r--r--   0        0        0     4868 2023-06-07 12:04:27.498906 pyprocessors_openai_completion-0.5.81/tests/data/en_gpt-3.5-turbo.json
--rw-r--r--   0        0        0     4716 2023-06-07 12:04:27.499906 pyprocessors_openai_completion-0.5.81/tests/data/en_gpt-4.json
--rw-r--r--   0        0        0     4141 2023-06-07 12:04:27.500906 pyprocessors_openai_completion-0.5.81/tests/data/en_text-ada-001.json
--rw-r--r--   0        0        0     3914 2023-06-07 12:04:27.500906 pyprocessors_openai_completion-0.5.81/tests/data/en_text-babbage-001.json
--rw-r--r--   0        0        0     4187 2023-06-07 12:04:27.501906 pyprocessors_openai_completion-0.5.81/tests/data/en_text-curie-001.json
--rw-r--r--   0        0        0     4182 2023-06-07 12:04:27.502906 pyprocessors_openai_completion-0.5.81/tests/data/en_text-davinci-003.json
--rw-r--r--   0        0        0     2202 2023-06-07 12:04:27.502906 pyprocessors_openai_completion-0.5.81/tests/data/fr_davinci-instruct-beta.json
--rw-r--r--   0        0        0     3207 2023-06-07 12:04:27.503907 pyprocessors_openai_completion-0.5.81/tests/data/fr_gpt-3.5-turbo.json
--rw-r--r--   0        0        0     2560 2023-06-07 12:04:27.504907 pyprocessors_openai_completion-0.5.81/tests/data/fr_gpt-4.json
--rw-r--r--   0        0        0     2295 2023-06-07 12:04:27.505906 pyprocessors_openai_completion-0.5.81/tests/data/fr_text-ada-001.json
--rw-r--r--   0        0        0     1699 2023-06-07 12:04:27.506907 pyprocessors_openai_completion-0.5.81/tests/data/fr_text-babbage-001.json
--rw-r--r--   0        0        0     1823 2023-06-07 12:04:27.506907 pyprocessors_openai_completion-0.5.81/tests/data/fr_text-curie-001.json
--rw-r--r--   0        0        0     2366 2023-06-07 12:04:27.507907 pyprocessors_openai_completion-0.5.81/tests/data/fr_text-davinci-003.json
--rw-r--r--   0        0        0     8421 2023-06-07 12:04:27.508907 pyprocessors_openai_completion-0.5.81/tests/data/jinjadocs.json
--rw-r--r--   0        0        0    13529 2023-06-07 12:04:27.508907 pyprocessors_openai_completion-0.5.81/tests/data/jinjadocs_preserve_entities.json
--rw-r--r--   0        0        0    14427 2023-06-07 12:04:27.509907 pyprocessors_openai_completion-0.5.81/tests/data/jinjadocs_substitute_entities.json
--rw-r--r--   0        0        0     5070 2023-06-07 12:04:27.510907 pyprocessors_openai_completion-0.5.81/tests/data/question_segments.json
--rw-r--r--   0        0        0     1219 2023-06-07 12:04:27.510907 pyprocessors_openai_completion-0.5.81/tests/data/question_segments_answer.json
--rw-r--r--   0        0        0    13876 2023-07-27 14:42:06.620929 pyprocessors_openai_completion-0.5.81/tests/test_openai_completion.py
--rw-r--r--   0        0        0      951 2023-06-07 12:04:27.512907 pyprocessors_openai_completion-0.5.81/tox.ini
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 pyprocessors_openai_completion-0.5.81/setup.py
--rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 pyprocessors_openai_completion-0.5.81/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-02-15 15:56:35.737007 pyprocessors-openai_completion-0.5.9/.dockerignore
+-rw-r--r--   0        0        0      147 2023-02-15 15:56:35.738007 pyprocessors-openai_completion-0.5.9/.gitignore
+-rw-r--r--   0        0        0      448 2023-02-15 15:56:35.739007 pyprocessors-openai_completion-0.5.9/Dockerfile
+-rw-r--r--   0        0        0    10227 2023-02-15 16:21:10.683489 pyprocessors-openai_completion-0.5.9/Jenkinsfile
+-rw-r--r--   0        0        0      380 2023-02-15 15:56:35.741007 pyprocessors-openai_completion-0.5.9/README.md
+-rw-r--r--   0        0        0     1559 2023-02-15 15:56:35.742007 pyprocessors-openai_completion-0.5.9/bumpversion.py
+-rw-r--r--   0        0        0       55 2023-02-15 16:28:13.706505 pyprocessors-openai_completion-0.5.9/pyprocessors_openai_completion/__init__.py
+-rw-r--r--   0        0        0     8400 2023-02-15 16:25:55.699911 pyprocessors-openai_completion-0.5.9/pyprocessors_openai_completion/openai_completion.py
+-rw-r--r--   0        0        0     2556 2023-02-15 15:56:35.744007 pyprocessors-openai_completion-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-15 15:56:35.745007 pyprocessors-openai_completion-0.5.9/tests/__init__.py
+-rw-r--r--   0        0        0     5320 2023-02-15 16:15:56.148298 pyprocessors-openai_completion-0.5.9/tests/test_openai_completion.py
+-rw-r--r--   0        0        0      951 2023-02-15 16:25:55.699911 pyprocessors-openai_completion-0.5.9/tox.ini
+-rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 pyprocessors-openai_completion-0.5.9/setup.py
+-rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 pyprocessors-openai_completion-0.5.9/PKG-INFO
```

### Comparing `pyprocessors_openai_completion-0.5.81/Jenkinsfile` & `pyprocessors-openai_completion-0.5.9/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.81/bumpversion.py` & `pyprocessors-openai_completion-0.5.9/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.81/pyproject.toml` & `pyprocessors-openai_completion-0.5.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,17 +26,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 requires = [
     "pymultirole-plugins>=0.5.0,<0.6.0",
-    "openai>=0.27.8",
-    "Jinja2",
-    "tenacity"
+    "openai"
 ]
 dist-name = "pyprocessors-openai_completion"
 description-file = "README.md"
 requires-python = ">=3.8"
 
 [tool.flit.entrypoints."pyprocessors.plugins"]
 openai_completion = "pyprocessors_openai_completion.openai_completion:OpenAICompletionProcessor"
```

### Comparing `pyprocessors_openai_completion-0.5.81/tox.ini` & `pyprocessors-openai_completion-0.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.81/setup.py` & `pyprocessors-openai_completion-0.5.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 packages = \
 ['pyprocessors_openai_completion']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pymultirole-plugins>=0.5.0,<0.6.0', 'openai>=0.27.8', 'Jinja2', 'tenacity']
+['pymultirole-plugins>=0.5.0,<0.6.0', 'openai']
 
 extras_require = \
 {'dev': ['flit', 'pre-commit', 'bump2version'],
  'docs': ['sphinx',
           'sphinx-rtd-theme',
           'm2r2',
           'sphinxcontrib.apidoc',
@@ -30,15 +30,15 @@
           'flask==2.1.3']}
 
 entry_points = \
 {'pyprocessors.plugins': ['openai_completion = '
                           'pyprocessors_openai_completion.openai_completion:OpenAICompletionProcessor']}
 
 setup(name='pyprocessors-openai_completion',
-      version='0.5.81',
+      version='0.5.9',
       description='OpenAICompletion processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyprocessors_openai_completion-0.5.81/PKG-INFO` & `pyprocessors-openai_completion-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-openai_completion
-Version: 0.5.81
+Version: 0.5.9
 Summary: OpenAICompletion processor
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -23,17 +23,15 @@
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: pymultirole-plugins>=0.5.0,<0.6.0
-Requires-Dist: openai>=0.27.8
-Requires-Dist: Jinja2
-Requires-Dist: tenacity
+Requires-Dist: openai
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Requires-Dist: m2r2 ; extra == "docs"
 Requires-Dist: sphinxcontrib.apidoc ; extra == "docs"
```

