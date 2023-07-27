# Comparing `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601.tar.gz` & `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601.tar", last modified: Wed Jul 26 23:46:54 2023, max compression
+gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831.tar", last modified: Thu Jul 27 00:09:25 2023, max compression
```

## Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601.tar` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:46:54.471152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 23:46:54.471152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 23:46:54.471152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-07-26 23:46:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:46:54.467152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:46:54.471152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    24602 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:46:54.471152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 23:46:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      948 2023-07-26 23:46:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 23:46:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-26 23:46:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-26 23:46:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:09:25.304296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 00:09:25.304296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 00:09:25.304296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-07-27 00:09:22.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:09:25.300296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:09:25.300296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    24604 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:09:25.304296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 00:09:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      948 2023-07-27 00:09:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 00:09:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-27 00:09:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-27 00:09:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/LICENSE` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230726234601
+Version: 1.0.0.dev20230727000831
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/README.md` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/setup.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-resample-and-write-to-zarr-store-lambda",
-  version="1.0.0.dev20230726234601",
+  version="1.0.0.dev20230727000831",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
         # {"shipName":"Henry_B._Bigelow","cruiseName":"HB0707","sensorName":"EK60","fileName":"D20070711-T210709.raw"}
         ship_name = message['shipName']  # 'Henry_B._Bigelow'
         cruise_name = message['cruiseName']  # 'HB0707'
         sensor_name = message['sensorName']  # 'EK60'
         input_file_name = message['fileName']  # TODO: what message parameters are passed in?
         # input_zarr_path = message['zarrPath']  # 'level_1/Henry_B._Bigelow/HB0707/EK60/D20070712-T152416.zarr',
         #
-        input_file_name = "D20070711-T210709.raw"
+        # input_file_name = "D20070711-T210709.raw"
         file_stem = os.path.splitext(input_file_name)[0]
         # input_zarr_path = 'level_1/Henry_B._Bigelow/HB0707/EK60/D20070712-T152416.zarr'
         input_zarr_path = f"level_1/{ship_name}/{cruise_name}/{sensor_name}/{file_stem}.zarr"
         #
         # store_name = f"{os.path.splitext(input_file_name)[0]}.zarr"
         # print(store_name)
         # output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}"
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230726234601
+Version: 1.0.0.dev20230727000831
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

