# Comparing `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831.tar.gz` & `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831.tar", last modified: Thu Jul 27 00:09:25 2023, max compression
+gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630.tar", last modified: Thu Jul 27 00:47:23 2023, max compression
```

## Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831.tar` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:09:25.304296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 00:09:25.304296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 00:09:25.304296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-07-27 00:09:22.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:09:25.300296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:09:25.300296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    24604 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-27 00:08:26.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:09:25.304296 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 00:09:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      948 2023-07-27 00:09:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 00:09:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-27 00:09:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-27 00:09:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:47:23.322649 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-27 00:46:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 00:47:23.322649 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-27 00:46:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 00:47:23.322649 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-07-27 00:47:20.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:47:23.318649 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:47:23.322649 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 00:46:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-07-27 00:46:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    22735 2023-07-27 00:46:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 00:46:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2023-07-27 00:46:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-27 00:46:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-27 00:46:25.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 00:47:23.322649 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-27 00:47:23.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      948 2023-07-27 00:47:23.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 00:47:23.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-27 00:47:23.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-27 00:47:23.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/LICENSE` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230727000831
+Version: 1.0.0.dev20230727004630
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/README.md` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/setup.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-resample-and-write-to-zarr-store-lambda",
-  version="1.0.0.dev20230727000831",
+  version="1.0.0.dev20230727004630",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,35 +9,22 @@
 import geopandas
 from datetime import datetime
 import boto3
 from botocore.exceptions import ClientError
 import numpy as np
 import xarray as xr
 import pandas as pd
-from enum import Enum
 
 TEMPDIR = "/tmp"
 
 MAX_POOL_CONNECTIONS = 64
 MAX_CONCURRENCY = 100
 TILE_SIZE = 512
 
-SYNCHRONIZER = None  # TODO: this will need to be shared between parallel lambdas will need to mount an EFS
-
-#####################################################################
-class PIPELINE_STATUS(Enum):
-    """
-    Keywords used to denote processing status in DynamoDB
-    """
-    PROCESSING = 'PROCESSING'
-    SUCCESS = 'SUCCESS'
-    FAILURE = 'FAILURE'
-
-#####################################################################
-
+SYNCHRONIZER = None  # TODO
 
 class LambdaExecutor:
 
     ############################################################################
     def __init__(
             self,
             s3_operations,
@@ -313,27 +300,14 @@
     ############################################################################
     # TODO: need to pass in key/secret as optionals
     def __get_s3_zarr_as_xr(
             self,
             zarr_path: str
     ) -> xr.core.dataset.Dataset:
         print('getting s3 zarr as xr')
-        ### ORIGINAL ###
-        # s3_fs = s3fs.S3FileSystem(
-        #     key=os.getenv('ACCESS_KEY_ID'),  # optional parameter
-        #     secret=os.getenv('SECRET_ACCESS_KEY'),
-        # )
-        # store = s3fs.S3Map(root=s3_zarr_store_path, s3=s3_fs, check=True)
-        ### UPDATE 1 ###
-        # s3_fs = self.__s3fs(
-        #     key=os.getenv('ACCESS_KEY_ID'),  # optional parameter
-        #     secret=os.getenv('SECRET_ACCESS_KEY'),
-        # )
-        # store = s3fs.S3Map(root=f's3://{self.__output_bucket}/{zarr_path}', s3=s3_fs, check=True)
-        ### UPDATE 2 ###
         store = self.__s3fs.s3_map(
             s3_zarr_store_path=zarr_path,
             access_key_id=self.__output_bucket_access_key,
             secret_access_key=self.__output_bucket_secret_access_key,
         )
         # You are already using dask, this is assumed by open_zarr, not the same as open_dataset(engine=“zarr”)
         import fsspec
@@ -457,53 +431,39 @@
 
     ############################################################################
     def execute(self, message):
         # {"shipName":"Henry_B._Bigelow","cruiseName":"HB0707","sensorName":"EK60","fileName":"D20070711-T210709.raw"}
         ship_name = message['shipName']  # 'Henry_B._Bigelow'
         cruise_name = message['cruiseName']  # 'HB0707'
         sensor_name = message['sensorName']  # 'EK60'
-        input_file_name = message['fileName']  # TODO: what message parameters are passed in?
-        # input_zarr_path = message['zarrPath']  # 'level_1/Henry_B._Bigelow/HB0707/EK60/D20070712-T152416.zarr',
+        input_file_name = message['fileName']
         #
-        # input_file_name = "D20070711-T210709.raw"
         file_stem = os.path.splitext(input_file_name)[0]
-        # input_zarr_path = 'level_1/Henry_B._Bigelow/HB0707/EK60/D20070712-T152416.zarr'
         input_zarr_path = f"level_1/{ship_name}/{cruise_name}/{sensor_name}/{file_stem}.zarr"
         #
-        # store_name = f"{os.path.splitext(input_file_name)[0]}.zarr"
-        # print(store_name)
-        # output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}"
-        # bucket_key = f"data/raw/{ship_name}/{cruise_name}/{sensor_name}/{input_file_name}"
-        # print(bucket_key)
-        #
         os.chdir(TEMPDIR)
         #
         ### COPY N PASTED IN BELOW #######################################################
         # [0] get dynamoDB table info
         df = self.__get_table_as_dataframe()
         # Zarr path is derived from DynamoDB
         ### ZARR_PATH ###
-        # input_zarr_path = 'level_1/Henry_B._Bigelow/HB0707/EK60/D20070712-T061745.zarr'
         assert(input_zarr_path in list(df['ZARR_PATH'])), "The Zarr path is not found in the database."
         #
         index = df.index[df['ZARR_PATH'] == input_zarr_path][0]  # index among all cruise files
         print(index)
         #
         file_info = df.iloc[index].to_dict()
         input_zarr_bucket = file_info['ZARR_BUCKET']
         input_zarr_path = file_info['ZARR_PATH']
         output_zarr_bucket = file_info['ZARR_BUCKET']
         #
         #################################################################
         # [1] read file-level Zarr store using xarray
-        file_xr = self.__get_s3_zarr_as_xr(
-            # already have bucket, pass in the path
-            # s3_zarr_store_path=f's3://{input_zarr_bucket}/{input_zarr_path}'
-            zarr_path=input_zarr_path
-        )
+        file_xr = self.__get_s3_zarr_as_xr(zarr_path=input_zarr_path)
         geo_json = self.__read_s3_geo_json(
             s3_geo_json_path=f's3://{input_zarr_bucket}/{input_zarr_path}/geo.json',
             access_key_id=os.getenv('ACCESS_KEY_ID'),
             secret_access_key=os.getenv('SECRET_ACCESS_KEY'),
         )
         #geo_json['features'][0]
         # {'id': '2007-07-12T15:24:16.032000000', 'type': 'Feature', 'properties': {'latitude': None, 'longitude': None}, 'geometry': None}
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,10 +28,10 @@
             access_key_id=None,
             secret_access_key=None,
     ):
         s3_fs = self.__get_s3_fs(
             access_key_id=access_key_id,
             secret_access_key=secret_access_key
         )
-        return s3fs.s3Map(root=s3_zarr_store_path, s3=s3_fs, check=True)
+        return s3fs.S3Map(root=s3_zarr_store_path, s3=s3_fs, check=True)
 
     #####################################################################
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230727000831
+Version: 1.0.0.dev20230727004630
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727000831/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230727004630/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

