# Comparing `tmp/aws-cdk-code-builder-1.2.3.tar.gz` & `tmp/aws-cdk-code-builder-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk-code-builder-1.2.3.tar", last modified: Mon May  1 19:30:06 2023, max compression
+gzip compressed data, was "aws-cdk-code-builder-1.2.4.tar", last modified: Thu Jul 27 13:08:08 2023, max compression
```

## Comparing `aws-cdk-code-builder-1.2.3.tar` & `aws-cdk-code-builder-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:30:06.184984 aws-cdk-code-builder-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-01 19:30:06.184984 aws-cdk-code-builder-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:30:06.180984 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:30:06.184984 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-01 19:30:06.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-01 19:30:06.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:30:06.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 19:30:06.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 19:30:06.000000 aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:30:06.184984 aws-cdk-code-builder-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:30:06.184984 aws-cdk-code-builder-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-01 19:29:50.000000 aws-cdk-code-builder-1.2.3/tests/test_build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:08:08.886946 aws-cdk-code-builder-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 13:07:48.000000 aws-cdk-code-builder-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-27 13:08:08.886946 aws-cdk-code-builder-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-27 13:07:48.000000 aws-cdk-code-builder-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:08:08.886946 aws-cdk-code-builder-1.2.4/aws_cdk_code_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-27 13:07:48.000000 aws-cdk-code-builder-1.2.4/aws_cdk_code_builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:08:08.886946 aws-cdk-code-builder-1.2.4/aws_cdk_code_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-27 13:08:08.000000 aws-cdk-code-builder-1.2.4/aws_cdk_code_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-27 13:08:08.000000 aws-cdk-code-builder-1.2.4/aws_cdk_code_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:08:08.000000 aws-cdk-code-builder-1.2.4/aws_cdk_code_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 13:08:08.000000 aws-cdk-code-builder-1.2.4/aws_cdk_code_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 13:08:08.000000 aws-cdk-code-builder-1.2.4/aws_cdk_code_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:08:08.886946 aws-cdk-code-builder-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-27 13:07:48.000000 aws-cdk-code-builder-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:08:08.886946 aws-cdk-code-builder-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-27 13:07:48.000000 aws-cdk-code-builder-1.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-27 13:07:48.000000 aws-cdk-code-builder-1.2.4/tests/test_build.py
```

### Comparing `aws-cdk-code-builder-1.2.3/LICENSE` & `aws-cdk-code-builder-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk-code-builder-1.2.3/PKG-INFO` & `aws-cdk-code-builder-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-code-builder
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Library that extends the aws_lambda.Code.from_asset and allows for auto packaging of the project
 Home-page: https://github.com/DEADSEC-SECURITY/aws-cdk-code-builder
 Author: DeadSec-Security
 Author-email: amng835@gmail.com
 Keywords: aws_cdk,aws_cdk_build,aws_cdk_packaging
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `aws-cdk-code-builder-1.2.3/README.md` & `aws-cdk-code-builder-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk-code-builder-1.2.3/aws_cdk_code_builder/__init__.py` & `aws-cdk-code-builder-1.2.4/aws_cdk_code_builder/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,18 @@
         self.ignore_folders = ignore_folders
 
         if not self.work_dir.is_dir():
             raise ValueError('Work dir needs to be a directory')
         if not self.project_path.is_dir():
             raise ValueError('Project path needs to be a directory')
 
+        # Use function folder and parent folder names to avoid same function folder name colisions
         project_name = self.project_path.parts[-1]
+        if base_path := self.project_path.parts[-2]:
+            project_name = f"{base_path}-{project_name}"
 
         self._build_dir = self.work_dir.joinpath('.build')
         self._project_build_dir = self._build_dir.joinpath(project_name)
 
         if not self._build_dir.exists():
             self._build_dir.mkdir()
```

### Comparing `aws-cdk-code-builder-1.2.3/aws_cdk_code_builder.egg-info/PKG-INFO` & `aws-cdk-code-builder-1.2.4/aws_cdk_code_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-code-builder
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Library that extends the aws_lambda.Code.from_asset and allows for auto packaging of the project
 Home-page: https://github.com/DEADSEC-SECURITY/aws-cdk-code-builder
 Author: DeadSec-Security
 Author-email: amng835@gmail.com
 Keywords: aws_cdk,aws_cdk_build,aws_cdk_packaging
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `aws-cdk-code-builder-1.2.3/setup.py` & `aws-cdk-code-builder-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Local Imports
 
 README = (pathlib.Path(__file__).parent / "README.md").read_text(encoding='utf8')
 
 setup(
     name='aws-cdk-code-builder',
     packages=find_packages(),
-    version='1.2.3',
+    version='1.2.4',
     description='A Library that extends the aws_lambda.Code.from_asset and allows for auto '
                 'packaging of the project',
     long_description=README,
     long_description_content_type='text/markdown',
     author='DeadSec-Security',
     author_email='amng835@gmail.com',
     url='https://github.com/DEADSEC-SECURITY/aws-cdk-code-builder',
```

### Comparing `aws-cdk-code-builder-1.2.3/tests/test_build.py` & `aws-cdk-code-builder-1.2.4/tests/test_build.py`

 * *Files identical despite different names*

