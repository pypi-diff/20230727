# Comparing `tmp/sphinx_lfs_content-1.1.2.tar.gz` & `tmp/sphinx_lfs_content-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_lfs_content-1.1.2.tar", last modified: Thu Nov 24 11:52:50 2022, max compression
+gzip compressed data, was "sphinx_lfs_content-1.1.3.tar", last modified: Fri Dec 16 15:06:29 2022, max compression
```

## Comparing `sphinx_lfs_content-1.1.2.tar` & `sphinx_lfs_content-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:52:50.937813 sphinx_lfs_content-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2022-11-24 11:52:46.000000 sphinx_lfs_content-1.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     2253 2022-11-24 11:52:50.937813 sphinx_lfs_content-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1811 2022-11-24 11:52:46.000000 sphinx_lfs_content-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 11:52:50.937813 sphinx_lfs_content-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      848 2022-11-24 11:52:46.000000 sphinx_lfs_content-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:52:50.933813 sphinx_lfs_content-1.1.2/sphinx_lfs_content/
--rw-r--r--   0 runner    (1001) docker     (122)     2211 2022-11-24 11:52:46.000000 sphinx_lfs_content-1.1.2/sphinx_lfs_content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:52:50.937813 sphinx_lfs_content-1.1.2/sphinx_lfs_content.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2253 2022-11-24 11:52:50.000000 sphinx_lfs_content-1.1.2/sphinx_lfs_content.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      269 2022-11-24 11:52:50.000000 sphinx_lfs_content-1.1.2/sphinx_lfs_content.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 11:52:50.000000 sphinx_lfs_content-1.1.2/sphinx_lfs_content.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-24 11:52:50.000000 sphinx_lfs_content-1.1.2/sphinx_lfs_content.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-11-24 11:52:50.000000 sphinx_lfs_content-1.1.2/sphinx_lfs_content.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 15:06:29.609329 sphinx_lfs_content-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2022-12-16 15:06:29.609329 sphinx_lfs_content-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1811 2022-12-16 15:06:28.000000 sphinx_lfs_content-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 15:06:29.609329 sphinx_lfs_content-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      848 2022-12-16 15:06:28.000000 sphinx_lfs_content-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 15:06:29.605328 sphinx_lfs_content-1.1.3/sphinx_lfs_content/
+-rw-r--r--   0 runner    (1001) docker     (122)     2211 2022-12-16 15:06:28.000000 sphinx_lfs_content-1.1.3/sphinx_lfs_content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 15:06:29.605328 sphinx_lfs_content-1.1.3/sphinx_lfs_content.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2022-12-16 15:06:29.000000 sphinx_lfs_content-1.1.3/sphinx_lfs_content.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2022-12-16 15:06:29.000000 sphinx_lfs_content-1.1.3/sphinx_lfs_content.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-16 15:06:29.000000 sphinx_lfs_content-1.1.3/sphinx_lfs_content.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2022-12-16 15:06:29.000000 sphinx_lfs_content-1.1.3/sphinx_lfs_content.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2022-12-16 15:06:29.000000 sphinx_lfs_content-1.1.3/sphinx_lfs_content.egg-info/top_level.txt
```

### Comparing `sphinx_lfs_content-1.1.2/PKG-INFO` & `sphinx_lfs_content-1.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: sphinx_lfs_content
-Version: 1.1.2
-Summary: Ensure existence of LFS content in your LFS builds
-Author: Dominic Kempf
-Author-email: dominic.kempf@iwr.uni-heidelberg.de
-Classifier: Framework :: Sphinx :: Extension
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix 
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # sphinx_lfs_content
 
 [![PyPI version](https://badge.fury.io/py/sphinx-lfs-content.svg)](https://badge.fury.io/py/sphinx-lfs-content)
 [![Documentation Status](https://readthedocs.org/projects/sphinx-lfs-content/badge/?version=latest)](https://sphinx-lfs-content.readthedocs.io/en/latest/?badge=latest)
 
 Git LFS is a popular method to store large files like e.g. documentation assets in git repositories.
 Building such documentation on a system without Git LFS will typically result in broken documentation.
```

### Comparing `sphinx_lfs_content-1.1.2/README.md` & `sphinx_lfs_content-1.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,57 @@
-# sphinx_lfs_content
-
-[![PyPI version](https://badge.fury.io/py/sphinx-lfs-content.svg)](https://badge.fury.io/py/sphinx-lfs-content)
-[![Documentation Status](https://readthedocs.org/projects/sphinx-lfs-content/badge/?version=latest)](https://sphinx-lfs-content.readthedocs.io/en/latest/?badge=latest)
-
-Git LFS is a popular method to store large files like e.g. documentation assets in git repositories.
-Building such documentation on a system without Git LFS will typically result in broken documentation. 
-`sphinx_lfs_content` is a minimalistic Sphinx extension that ensures that `git-lfs` is installed and otherwise installs it and fetches LFS content.
-It is motivated by the [lack of LFS support on readthedocs.org](https://github.com/readthedocs/readthedocs.org/issues/1846).
-
-## Installation
-
-The extension can be installed from PyPI using `pip`:
-
-```python
-python -m pip install sphinx_lfs_content
-```
-
-If you use a requirements file to describe the dependencies of your documentation build, simply add `sphinx_lfs_content` to it.
-
-## How to use it
-
-Add the following lines to your `conf.py`:
-
-```python
-# The list of enabled extensions
-extensions = [
-    "sphinx_lfs_content",
-]
-```
-
-That's all. The extension will check whether the system has `git-lfs` and download a version
-from the [`git-lfs` GitHub page](https://github.com/git-lfs/git-lfs), verify its checksum
-and checkout any LFS content.
-
-Additionally, a configuration value `lfs_content_post_commands` is available. It accepts a list
-of strings with commands that will be executed after the git-lfs checkout was performed.
-This can be used to resolve chicken-egg situations with other setup code.
-
-## Restrictions
-
-The extension is very likely to only work on Linux right now, as it does not properly select the `git-lfs` archive to download.
+Metadata-Version: 2.1
+Name: sphinx_lfs_content
+Version: 1.1.3
+Summary: Ensure existence of LFS content in your LFS builds
+Home-page: UNKNOWN
+Author: Dominic Kempf
+Author-email: dominic.kempf@iwr.uni-heidelberg.de
+License: UNKNOWN
+Description: # sphinx_lfs_content
+        
+        [![PyPI version](https://badge.fury.io/py/sphinx-lfs-content.svg)](https://badge.fury.io/py/sphinx-lfs-content)
+        [![Documentation Status](https://readthedocs.org/projects/sphinx-lfs-content/badge/?version=latest)](https://sphinx-lfs-content.readthedocs.io/en/latest/?badge=latest)
+        
+        Git LFS is a popular method to store large files like e.g. documentation assets in git repositories.
+        Building such documentation on a system without Git LFS will typically result in broken documentation. 
+        `sphinx_lfs_content` is a minimalistic Sphinx extension that ensures that `git-lfs` is installed and otherwise installs it and fetches LFS content.
+        It is motivated by the [lack of LFS support on readthedocs.org](https://github.com/readthedocs/readthedocs.org/issues/1846).
+        
+        ## Installation
+        
+        The extension can be installed from PyPI using `pip`:
+        
+        ```python
+        python -m pip install sphinx_lfs_content
+        ```
+        
+        If you use a requirements file to describe the dependencies of your documentation build, simply add `sphinx_lfs_content` to it.
+        
+        ## How to use it
+        
+        Add the following lines to your `conf.py`:
+        
+        ```python
+        # The list of enabled extensions
+        extensions = [
+            "sphinx_lfs_content",
+        ]
+        ```
+        
+        That's all. The extension will check whether the system has `git-lfs` and download a version
+        from the [`git-lfs` GitHub page](https://github.com/git-lfs/git-lfs), verify its checksum
+        and checkout any LFS content.
+        
+        Additionally, a configuration value `lfs_content_post_commands` is available. It accepts a list
+        of strings with commands that will be executed after the git-lfs checkout was performed.
+        This can be used to resolve chicken-egg situations with other setup code.
+        
+        ## Restrictions
+        
+        The extension is very likely to only work on Linux right now, as it does not properly select the `git-lfs` archive to download.
+        
+Platform: UNKNOWN
+Classifier: Framework :: Sphinx :: Extension
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix 
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
```

### Comparing `sphinx_lfs_content-1.1.2/setup.py` & `sphinx_lfs_content-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="sphinx_lfs_content",
-    version="1.1.2",
+    version="1.1.3",
     author="Dominic Kempf",
     author_email="dominic.kempf@iwr.uni-heidelberg.de",
     description="Ensure existence of LFS content in your LFS builds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
```

### Comparing `sphinx_lfs_content-1.1.2/sphinx_lfs_content/__init__.py` & `sphinx_lfs_content-1.1.3/sphinx_lfs_content/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import shutil
 import sphinx
 import subprocess
 import tarfile
 import tempfile
 
 
-GIT_LFS_FILE = "https://github.com/git-lfs/git-lfs/releases/download/v3.2.0/git-lfs-linux-amd64-v3.2.0.tar.gz"
-GIT_LFS_CHECKSUM = "d6730b8036d9d99f872752489a331995930fec17b61c87c7af1945c65a482a50"
+GIT_LFS_FILE = "https://github.com/git-lfs/git-lfs/releases/download/v3.3.0/git-lfs-linux-amd64-v3.3.0.tar.gz"
+GIT_LFS_CHECKSUM = "6a4e6bd7d06d5c024bc70c8ee8c9da143ffc37d2646e252a17a6126d30cdebc1"
 
 
 def lfs_setup(_, config):
     # If we already have git-lfs, we do not need to set it up
     if shutil.which("git-lfs") is None:
         # Download the latest git-lfs tarball and check its checksum
         git_lfs_content = requests.get(GIT_LFS_FILE).content
@@ -31,15 +31,15 @@
             with tarfile.open(os.path.join(tmp_dir, "git-lfs.tar.gz"), "r:gz") as tar:
                 tar.extractall(path=tmp_dir)
 
             # Setup a modified environment that has the temporary directory in PATH
             # This works around a bug in git-lfs where git-lfs is called recursively,
             # but the inner calls rely on git-lfs being in PATH.
             env = os.environ
-            env["PATH"] = os.environ["PATH"] + os.path.pathsep + os.path.join(tmp_dir, "git-lfs-3.2.0")
+            env["PATH"] = os.environ["PATH"] + os.path.pathsep + os.path.join(tmp_dir, "git-lfs-3.3.0")
 
             # Fetch the LFS content of the repository
             subprocess.check_call("git-lfs install".split(), env=env)
             subprocess.check_call("git-lfs fetch".split(), env=env)
             subprocess.check_call("git-lfs checkout".split(), env=env)
 
     # Execute all of the given post commands
@@ -47,8 +47,8 @@
         subprocess.check_call(cmd, shell=True)
 
 
 def setup(app):
     app.add_config_value("lfs_content_post_commands", [], rebuild="")
     app.connect("config-inited", lfs_setup)
 
-    return {"version": "1.1.1", "parallel_read_safe": True}
+    return {"version": "1.1.3", "parallel_read_safe": True}
```

### Comparing `sphinx_lfs_content-1.1.2/sphinx_lfs_content.egg-info/PKG-INFO` & `sphinx_lfs_content-1.1.3/sphinx_lfs_content.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 Metadata-Version: 2.1
 Name: sphinx-lfs-content
-Version: 1.1.2
+Version: 1.1.3
 Summary: Ensure existence of LFS content in your LFS builds
+Home-page: UNKNOWN
 Author: Dominic Kempf
 Author-email: dominic.kempf@iwr.uni-heidelberg.de
+License: UNKNOWN
+Description: # sphinx_lfs_content
+        
+        [![PyPI version](https://badge.fury.io/py/sphinx-lfs-content.svg)](https://badge.fury.io/py/sphinx-lfs-content)
+        [![Documentation Status](https://readthedocs.org/projects/sphinx-lfs-content/badge/?version=latest)](https://sphinx-lfs-content.readthedocs.io/en/latest/?badge=latest)
+        
+        Git LFS is a popular method to store large files like e.g. documentation assets in git repositories.
+        Building such documentation on a system without Git LFS will typically result in broken documentation. 
+        `sphinx_lfs_content` is a minimalistic Sphinx extension that ensures that `git-lfs` is installed and otherwise installs it and fetches LFS content.
+        It is motivated by the [lack of LFS support on readthedocs.org](https://github.com/readthedocs/readthedocs.org/issues/1846).
+        
+        ## Installation
+        
+        The extension can be installed from PyPI using `pip`:
+        
+        ```python
+        python -m pip install sphinx_lfs_content
+        ```
+        
+        If you use a requirements file to describe the dependencies of your documentation build, simply add `sphinx_lfs_content` to it.
+        
+        ## How to use it
+        
+        Add the following lines to your `conf.py`:
+        
+        ```python
+        # The list of enabled extensions
+        extensions = [
+            "sphinx_lfs_content",
+        ]
+        ```
+        
+        That's all. The extension will check whether the system has `git-lfs` and download a version
+        from the [`git-lfs` GitHub page](https://github.com/git-lfs/git-lfs), verify its checksum
+        and checkout any LFS content.
+        
+        Additionally, a configuration value `lfs_content_post_commands` is available. It accepts a list
+        of strings with commands that will be executed after the git-lfs checkout was performed.
+        This can be used to resolve chicken-egg situations with other setup code.
+        
+        ## Restrictions
+        
+        The extension is very likely to only work on Linux right now, as it does not properly select the `git-lfs` archive to download.
+        
+Platform: UNKNOWN
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix 
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# sphinx_lfs_content
-
-[![PyPI version](https://badge.fury.io/py/sphinx-lfs-content.svg)](https://badge.fury.io/py/sphinx-lfs-content)
-[![Documentation Status](https://readthedocs.org/projects/sphinx-lfs-content/badge/?version=latest)](https://sphinx-lfs-content.readthedocs.io/en/latest/?badge=latest)
-
-Git LFS is a popular method to store large files like e.g. documentation assets in git repositories.
-Building such documentation on a system without Git LFS will typically result in broken documentation. 
-`sphinx_lfs_content` is a minimalistic Sphinx extension that ensures that `git-lfs` is installed and otherwise installs it and fetches LFS content.
-It is motivated by the [lack of LFS support on readthedocs.org](https://github.com/readthedocs/readthedocs.org/issues/1846).
-
-## Installation
-
-The extension can be installed from PyPI using `pip`:
-
-```python
-python -m pip install sphinx_lfs_content
-```
-
-If you use a requirements file to describe the dependencies of your documentation build, simply add `sphinx_lfs_content` to it.
-
-## How to use it
-
-Add the following lines to your `conf.py`:
-
-```python
-# The list of enabled extensions
-extensions = [
-    "sphinx_lfs_content",
-]
-```
-
-That's all. The extension will check whether the system has `git-lfs` and download a version
-from the [`git-lfs` GitHub page](https://github.com/git-lfs/git-lfs), verify its checksum
-and checkout any LFS content.
-
-Additionally, a configuration value `lfs_content_post_commands` is available. It accepts a list
-of strings with commands that will be executed after the git-lfs checkout was performed.
-This can be used to resolve chicken-egg situations with other setup code.
-
-## Restrictions
-
-The extension is very likely to only work on Linux right now, as it does not properly select the `git-lfs` archive to download.
```

