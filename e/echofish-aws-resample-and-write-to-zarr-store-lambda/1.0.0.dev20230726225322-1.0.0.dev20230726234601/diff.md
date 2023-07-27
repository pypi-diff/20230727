# Comparing `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322.tar.gz` & `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322.tar", last modified: Wed Jul 26 22:54:17 2023, max compression
+gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601.tar", last modified: Wed Jul 26 23:46:54 2023, max compression
```

## Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322.tar` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 22:54:17.302560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 22:54:17.302560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 22:54:17.302560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-07-26 22:54:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 22:54:17.298560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 22:54:17.302560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    24355 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1455 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 22:54:17.302560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 22:54:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      948 2023-07-26 22:54:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 22:54:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-26 22:54:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-26 22:54:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:46:54.471152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 23:46:54.471152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 23:46:54.471152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-07-26 23:46:51.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:46:54.467152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:46:54.471152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    24602 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-26 23:45:56.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 23:46:54.471152 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 23:46:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      948 2023-07-26 23:46:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 23:46:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-26 23:46:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-26 23:46:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/LICENSE` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230726225322
+Version: 1.0.0.dev20230726234601
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/README.md` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/setup.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-resample-and-write-to-zarr-store-lambda",
-  version="1.0.0.dev20230726225322",
+  version="1.0.0.dev20230726234601",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,7 +33,12 @@
             UpdateExpression=expression,
             ExpressionAttributeNames=attribute_names,
             ExpressionAttributeValues=attribute_values
         )
         status_code = response['ResponseMetadata']['HTTPStatusCode']
         assert(status_code == 200), "Problem, unable to update dynamodb table."
 
+    def get_table(self, table_name):
+        print(f"opening table: {table_name}")
+        session = boto3.Session()
+        dynamodb = session.resource(service_name='dynamodb')
+        return dynamodb.Table(table_name)
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,26 +276,23 @@
     #                 secret_access_key=self.__output_bucket_secret_access_key
     #             )
     #     # print('Done uploading files')
 
     ############################################################################
     #####################################################################
 
-    def __get_table_as_dataframe(
-            self,
-            ship_name: str,
-            cruise_name: str,
-            sensor_name: str,
-    ) -> pd.DataFrame:
+    def __get_table_as_dataframe(self) -> pd.DataFrame:
         print('get table as dataframe')
         session = boto3.Session()
-        dynamodb = session.resource(service_name='dynamodb')
         try:
             print(self.__table_name)
-            table = dynamodb.Table(self.__table_name)
+            #
+            # table = self.__dynamo.Table(self.__table_name)
+            table = self.__dynamo.get_table(table_name=self.__table_name)
+            #
             # Note: table.scan() has 1 MB limit on results so pagination is used.
             response = table.scan()
             data = response['Items']
             while 'LastEvaluatedKey' in response:
                 response = table.scan(ExclusiveStartKey=response['LastEvaluatedKey'])
                 data.extend(response['Items'])
         except ClientError as err:
@@ -332,15 +329,15 @@
         #     secret=os.getenv('SECRET_ACCESS_KEY'),
         # )
         # store = s3fs.S3Map(root=f's3://{self.__output_bucket}/{zarr_path}', s3=s3_fs, check=True)
         ### UPDATE 2 ###
         store = self.__s3fs.s3_map(
             s3_zarr_store_path=zarr_path,
             access_key_id=self.__output_bucket_access_key,
-            secret_access_key=self.__output_bucket_secret_access_key
+            secret_access_key=self.__output_bucket_secret_access_key,
         )
         # You are already using dask, this is assumed by open_zarr, not the same as open_dataset(engine=“zarr”)
         import fsspec
         return xr.open_zarr(store=store, consolidated=None)  # synchronizer=SYNCHRONIZER
 
     ############################################################################
     def __interpolate_data(
@@ -456,35 +453,37 @@
     def __publish_done_message(self, message):
         print("Sending done message")
         self.__sns_operations.publish(self.__done_topic_arn, json.dumps(message))
 
 
     ############################################################################
     def execute(self, message):
+        # {"shipName":"Henry_B._Bigelow","cruiseName":"HB0707","sensorName":"EK60","fileName":"D20070711-T210709.raw"}
         ship_name = message['shipName']  # 'Henry_B._Bigelow'
         cruise_name = message['cruiseName']  # 'HB0707'
         sensor_name = message['sensorName']  # 'EK60'
-        #input_file_name = message['fileName']  # TODO: what message parameters are passed in?
-        input_zarr_path = message['zarrPath']  # 'level_1/Henry_B._Bigelow/HB0707/EK60/D20070712-T152416.zarr',
+        input_file_name = message['fileName']  # TODO: what message parameters are passed in?
+        # input_zarr_path = message['zarrPath']  # 'level_1/Henry_B._Bigelow/HB0707/EK60/D20070712-T152416.zarr',
+        #
+        input_file_name = "D20070711-T210709.raw"
+        file_stem = os.path.splitext(input_file_name)[0]
+        # input_zarr_path = 'level_1/Henry_B._Bigelow/HB0707/EK60/D20070712-T152416.zarr'
+        input_zarr_path = f"level_1/{ship_name}/{cruise_name}/{sensor_name}/{file_stem}.zarr"
         #
         # store_name = f"{os.path.splitext(input_file_name)[0]}.zarr"
         # print(store_name)
         # output_zarr_prefix = f"level_1/{ship_name}/{cruise_name}/{sensor_name}"
         # bucket_key = f"data/raw/{ship_name}/{cruise_name}/{sensor_name}/{input_file_name}"
         # print(bucket_key)
         #
         os.chdir(TEMPDIR)
         #
         ### COPY N PASTED IN BELOW #######################################################
         # [0] get dynamoDB table info
-        df = self.__get_table_as_dataframe(
-            ship_name=ship_name,
-            cruise_name=cruise_name,
-            sensor_name=sensor_name,
-        )
+        df = self.__get_table_as_dataframe()
         # Zarr path is derived from DynamoDB
         ### ZARR_PATH ###
         # input_zarr_path = 'level_1/Henry_B._Bigelow/HB0707/EK60/D20070712-T061745.zarr'
         assert(input_zarr_path in list(df['ZARR_PATH'])), "The Zarr path is not found in the database."
         #
         index = df.index[df['ZARR_PATH'] == input_zarr_path][0]  # index among all cruise files
         print(index)
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,23 +17,20 @@
 executor = LambdaExecutor(
     s3_operations=S3Operations(),
     s3fs_operations=S3FSOperations(),
     dynamo_operations=DynamoOperations(),
     sns_operations=SnsOperations(),
     output_bucket=output_bucket,
     table_name=table_name,
-    output_bucket_access_key=os.getenv('OUTPUT_BUCKET_ACCESS_KEY'),
-    output_bucket_secret_access_key=os.getenv('OUTPUT_BUCKET_SECRET_ACCESS_KEY'),
+    output_bucket_access_key=output_bucket_access_key,
+    output_bucket_secret_access_key=output_bucket_secret_access_key,
     done_topic_arn=done_topic_arn
 )
 
 def handler(sns_event, context):
-    print(f"table name: {os.environ['TABLE_NAME']}")
-    print(f"output bucket: {os.environ['OUTPUT_BUCKET']}")
-    #
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
         print("Start Message : " + str(message))
         executor.execute(message)
         print("Done Message : " + str(message))
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,15 @@
     def __get_s3_fs(
             self,
             access_key_id=None,
             secret_access_key=None
     ):
         if access_key_id:
             s3_fs = s3fs.S3FileSystem(
-                # key=os.getenv('ACCESS_KEY_ID'),
                 key=access_key_id,
-                # secret=os.getenv('SECRET_ACCESS_KEY'),
                 secret=secret_access_key
             )
             print('NODD Authenticated w passed credentials')
         else:
             s3_fs = s3fs.S3FileSystem()
             print('NODD Authenticated wo passed credentials')
         return s3_fs
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230726225322
+Version: 1.0.0.dev20230726234601
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726234601/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

