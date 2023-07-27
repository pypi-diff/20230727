# Comparing `tmp/baca2-package-manager-0.2.tar.gz` & `tmp/baca2-package-manager-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baca2-package-manager-0.2.tar", last modified: Wed Jul 26 19:20:05 2023, max compression
+gzip compressed data, was "baca2-package-manager-0.2.1.tar", last modified: Thu Jul 27 14:00:35 2023, max compression
```

## Comparing `baca2-package-manager-0.2.tar` & `baca2-package-manager-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 19:20:05.836725 baca2-package-manager-0.2/
--rw-rw-rw-   0        0        0    35823 2023-07-26 17:19:31.000000 baca2-package-manager-0.2/LICENSE
--rw-rw-rw-   0        0        0      758 2023-07-26 19:20:05.835726 baca2-package-manager-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-07-26 18:31:13.000000 baca2-package-manager-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 19:20:05.817469 baca2-package-manager-0.2/baca2PackageManager/
--rw-rw-rw-   0        0        0      748 2023-07-26 18:26:18.000000 baca2-package-manager-0.2/baca2PackageManager/__init__.py
--rw-rw-rw-   0        0        0       83 2023-07-26 17:55:56.000000 baca2-package-manager-0.2/baca2PackageManager/consts.py
--rw-rw-rw-   0        0        0    23329 2023-07-26 18:25:59.000000 baca2-package-manager-0.2/baca2PackageManager/manager.py
--rw-rw-rw-   0        0        0      133 2023-07-26 17:58:18.000000 baca2-package-manager-0.2/baca2PackageManager/manager_exceptions.py
--rw-rw-rw-   0        0        0     5940 2023-07-26 18:08:03.000000 baca2-package-manager-0.2/baca2PackageManager/validators.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:20:05.832725 baca2-package-manager-0.2/baca2_package_manager.egg-info/
--rw-rw-rw-   0        0        0      758 2023-07-26 19:20:05.000000 baca2-package-manager-0.2/baca2_package_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-07-26 19:20:05.000000 baca2-package-manager-0.2/baca2_package_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 19:20:05.000000 baca2-package-manager-0.2/baca2_package_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 19:20:05.000000 baca2-package-manager-0.2/baca2_package_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-26 19:20:05.000000 baca2-package-manager-0.2/baca2_package_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 19:20:05.836725 baca2-package-manager-0.2/setup.cfg
--rw-rw-rw-   0        0        0      720 2023-07-26 18:31:12.000000 baca2-package-manager-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:20:05.834724 baca2-package-manager-0.2/tests/
--rw-rw-rw-   0        0        0    23736 2023-07-26 18:27:41.000000 baca2-package-manager-0.2/tests/tests.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:00:35.969170 baca2-package-manager-0.2.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-26 17:19:31.000000 baca2-package-manager-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      760 2023-07-27 14:00:35.969170 baca2-package-manager-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-07-26 18:31:13.000000 baca2-package-manager-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 14:00:35.945813 baca2-package-manager-0.2.1/baca2PackageManager/
+-rw-rw-rw-   0        0        0      748 2023-07-26 18:26:18.000000 baca2-package-manager-0.2.1/baca2PackageManager/__init__.py
+-rw-rw-rw-   0        0        0       83 2023-07-26 17:55:56.000000 baca2-package-manager-0.2.1/baca2PackageManager/consts.py
+-rw-rw-rw-   0        0        0    24181 2023-07-27 13:53:59.000000 baca2-package-manager-0.2.1/baca2PackageManager/manager.py
+-rw-rw-rw-   0        0        0      133 2023-07-26 17:58:18.000000 baca2-package-manager-0.2.1/baca2PackageManager/manager_exceptions.py
+-rw-rw-rw-   0        0        0     5940 2023-07-26 18:08:03.000000 baca2-package-manager-0.2.1/baca2PackageManager/validators.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:00:35.965670 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/
+-rw-rw-rw-   0        0        0      760 2023-07-27 14:00:35.000000 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-27 14:00:35.000000 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 14:00:35.000000 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 14:00:35.000000 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-27 14:00:35.000000 baca2-package-manager-0.2.1/baca2_package_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 14:00:35.969170 baca2-package-manager-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-07-27 13:59:24.000000 baca2-package-manager-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:00:35.967754 baca2-package-manager-0.2.1/tests/
+-rw-rw-rw-   0        0        0    24517 2023-07-27 13:54:21.000000 baca2-package-manager-0.2.1/tests/tests.py
```

### Comparing `baca2-package-manager-0.2/LICENSE` & `baca2-package-manager-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.2/PKG-INFO` & `baca2-package-manager-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baca2-package-manager
-Version: 0.2
+Version: 0.2.1
 Summary: A package manager for Baca2 project
 Home-page: https://github.com/BaCa2-project/BaCa2-package-manager
 Author: Baca2 Team
 Author-email: bartosz.deptula@student.uj.edu.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `baca2-package-manager-0.2/baca2PackageManager/__init__.py` & `baca2-package-manager-0.2.1/baca2PackageManager/__init__.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.2/baca2PackageManager/manager.py` & `baca2-package-manager-0.2.1/baca2PackageManager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,39 @@
         sets_path = self.commit_path / 'tests'
         super().__init__(path, config_path, Package.DEFAULT_SETTINGS)
         print(sets_path)
         self._sets = []
         for i in [x[0].replace(str(sets_path) + '\\', '') for x in walk(sets_path)][1:]:
             self._sets.append(TSet(sets_path / i))
 
+    def prepare_build(self, build_name: str):
+        """
+        It prepares the build
+
+        :param build_name: The name of the build
+        :type build_name: str
+        """
+        if not (self.commit_path / '.build').is_dir():
+            mkdir(self.commit_path / '.build')
+
+        if not (self.commit_path / '.build' / build_name).is_dir():
+            mkdir(self.commit_path / '.build' / build_name)
+
+    def delete_build(self, build_name: str = None):
+        """
+        Deletes the build. If build_name is None, it deletes all builds.
+
+        :param build_name: The name of the build, if None, it clears all builds
+        :type build_name: str
+        """
+        if build_name is None:
+            rmtree(self.commit_path / '.build')
+        else:
+            rmtree(self.commit_path / '.build' / build_name)
+
     @property
     def commit_path(self) -> Path:
         """
         It returns the path to the commit
         TODO: After implementing internal git system, this should be changed
 
         :return: The path to the commit
```

### Comparing `baca2-package-manager-0.2/baca2PackageManager/validators.py` & `baca2-package-manager-0.2.1/baca2PackageManager/validators.py`

 * *Files identical despite different names*

### Comparing `baca2-package-manager-0.2/baca2_package_manager.egg-info/PKG-INFO` & `baca2-package-manager-0.2.1/baca2_package_manager.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baca2-package-manager
-Version: 0.2
+Version: 0.2.1
 Summary: A package manager for Baca2 project
 Home-page: https://github.com/BaCa2-project/BaCa2-package-manager
 Author: Baca2 Team
 Author-email: bartosz.deptula@student.uj.edu.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `baca2-package-manager-0.2/setup.py` & `baca2-package-manager-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='baca2-package-manager',
-    version='0.2',
+    version='0.2.1',
     author='Baca2 Team',
     author_email='bartosz.deptula@student.uj.edu.pl',
     description='A package manager for Baca2 project',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/BaCa2-project/BaCa2-package-manager',
     packages=setuptools.find_packages(),
```

### Comparing `baca2-package-manager-0.2/tests/tests.py` & `baca2-package-manager-0.2.1/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -610,7 +610,26 @@
         """
         new_comm = self.package.make_commit('3')
         self.assertIsInstance(new_comm, Package)
         self.assertEqual(new_comm._commit, '3')
         path_to_comm = new_comm.commit_path
         new_comm.delete()
         self.assertFalse(path_to_comm.exists())
+
+    def test_prepare_build(self):
+        """
+        It tests if the function prepare_build() works.
+        """
+        self.package.prepare_build('test')
+        self.assertTrue((self.package.commit_path / '.build' / 'test').is_dir())
+        self.package.delete_build('test')
+        self.assertFalse((self.package.commit_path / '.build' / 'test').is_dir())
+
+    def test_prepare_build_multiple(self):
+        """
+        It tests if the function prepare_build() works.
+        """
+        self.package.prepare_build('test')
+        self.package.prepare_build('test2')
+        self.assertTrue((self.package.commit_path / '.build' / 'test').is_dir())
+        self.package.delete_build()
+        self.assertFalse((self.package.commit_path / '.build').is_dir())
```

