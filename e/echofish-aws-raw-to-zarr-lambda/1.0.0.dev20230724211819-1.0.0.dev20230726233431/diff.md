# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819.tar", last modified: Mon Jul 24 21:19:21 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431.tar", last modified: Wed Jul 26 23:35:33 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:19:21.945458 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-24 21:18:15.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-24 21:19:21.945458 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-24 21:18:15.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 21:19:21.945458 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-24 21:19:17.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:19:21.941458 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:19:21.945458 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 21:18:15.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-24 21:18:15.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15839 2023-07-24 21:18:15.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-07-24 21:18:15.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3398 2023-07-24 21:18:15.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-24 21:18:15.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/sns_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 21:19:21.945458 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-24 21:19:21.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      641 2023-07-24 21:19:21.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 21:19:21.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-24 21:19:21.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-24 21:19:21.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:35:33.640104 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-26 23:34:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-26 23:35:33.640104 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-26 23:34:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 23:35:33.640104 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-26 23:35:29.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:35:33.636104 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:35:33.640104 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 23:34:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-26 23:34:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15839 2023-07-26 23:34:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-07-26 23:34:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-07-26 23:34:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-26 23:34:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:35:33.640104 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-26 23:35:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-26 23:35:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 23:35:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-26 23:35:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-26 23:35:33.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230724211819
+Version: 1.0.0.dev20230726233431
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230724211819",
+  version="1.0.0.dev20230726233431",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             self,
             bucket_name,
             key,
             access_key_id=None,
             secret_access_key=None
     ):
         s3_client = self.__get_client(access_key_id=access_key_id, secret_access_key=secret_access_key)
-        print(f"Deleting item: Bucket={bucket_name}, Key={key}")
+        # print(f"Deleting item: Bucket={bucket_name}, Key={key}")
         s3_client.delete_object(Bucket=bucket_name, Key=key)
 
     #####################################################################
     def upload_file(
             self,
             file_name,
             bucket_name,
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230724211819
+Version: 1.0.0.dev20230726233431
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230724211819/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230726233431/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

