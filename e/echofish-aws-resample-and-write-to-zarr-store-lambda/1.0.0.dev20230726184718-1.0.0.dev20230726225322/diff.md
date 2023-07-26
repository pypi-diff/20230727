# Comparing `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718.tar.gz` & `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718.tar", last modified: Wed Jul 26 18:48:14 2023, max compression
+gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322.tar", last modified: Wed Jul 26 22:54:17 2023, max compression
```

## Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718.tar` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:48:14.325727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 18:48:14.325727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 18:48:14.325727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-07-26 18:48:11.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:48:14.321727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:48:14.321727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    24145 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:48:14.325727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 18:48:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      948 2023-07-26 18:48:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 18:48:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-26 18:48:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-26 18:48:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 22:54:17.302560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 22:54:17.302560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 22:54:17.302560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-07-26 22:54:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 22:54:17.298560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 22:54:17.302560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    24355 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-26 22:53:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 22:54:17.302560 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 22:54:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      948 2023-07-26 22:54:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 22:54:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-26 22:54:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-26 22:54:17.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/LICENSE` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230726184718
+Version: 1.0.0.dev20230726225322
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/README.md` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/setup.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-resample-and-write-to-zarr-store-lambda",
-  version="1.0.0.dev20230726184718",
+  version="1.0.0.dev20230726225322",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 
 TEMPDIR = "/tmp"
 
 MAX_POOL_CONNECTIONS = 64
 MAX_CONCURRENCY = 100
 TILE_SIZE = 512
 
-SYNCHRONIZER = None  # TODO: this will need to be shared between parallel lambdas
-                     #  will need to mount an elastic file system
-
+SYNCHRONIZER = None  # TODO: this will need to be shared between parallel lambdas will need to mount an EFS
 
 #####################################################################
 class PIPELINE_STATUS(Enum):
     """
     Keywords used to denote processing status in DynamoDB
     """
     PROCESSING = 'PROCESSING'
@@ -59,78 +57,78 @@
         self.__output_bucket = output_bucket
         self.__table_name = table_name
         self.__output_bucket_access_key = output_bucket_access_key
         self.__output_bucket_secret_access_key = output_bucket_secret_access_key
         self.__done_topic_arn = done_topic_arn
 
     ############################################################################
-    def __delete_all_local_raw_and_zarr_files(self):  # good
-        """Used to clean up any residual files from warm lambdas
-        to keep the storage footprint below the 512 MB allocation.
-
-        Returns
-        -------
-        None : None
-            No return value.
-        """
-        print('Deleting all local raw and zarr files')
-        for i in ['*.raw*', '*.zarr']:
-            for j in glob.glob(i):
-                # print(f'Deleting {j}')
-                if os.path.isdir(j):
-                    shutil.rmtree(j, ignore_errors=True)
-                elif os.path.isfile(j):
-                    os.remove(j)
-
-    ############################################################################
-    def __set_processing_status(
-            self,
-            ship_name: str,
-            cruise_name: str,
-            sensor_name: str,
-            file_name: str,
-            new_status: str
-    ):
-        # Updates PIPELINE_STATUS via new_status value
-        # HASH: FILE_NAME, RANGE: SENSOR_NAME
-        self.__dynamo.put_item(
-            table_name=self.__table_name,
-            item={
-                'FILE_NAME': {'S': file_name},  # HASH
-                'SHIP_NAME': {'S': ship_name},
-                'CRUISE_NAME': {'S': cruise_name},
-                'SENSOR_NAME': {'S': sensor_name},  # RANGE
-                'PIPELINE_TIME': {'S': datetime.now().isoformat(timespec="seconds") + "Z"},
-                'PIPELINE_STATUS': {'S': new_status},
-            }
-        )
-
-    ############################################################################
-    def __update_processing_status(
-            self,
-            cruise_name,
-            file_name,
-            new_status
-    ):
-        self.__dynamo.update_item(
-            table_name=self.__table_name,
-            key={
-                'FILE_NAME': {'S': file_name},  # Partition Key
-                'CRUISE_NAME': {'S': cruise_name},  # Sort Key
-            },
-            expression='SET #PS = :ps',
-            attribute_names={
-                '#PS': 'PIPELINE_STATUS'
-            },
-            attribute_values={
-                ':ps': {
-                    'S': new_status
-                }
-            }
-        )
+    # def __delete_all_local_raw_and_zarr_files(self):  # good
+    #     """Used to clean up any residual files from warm lambdas
+    #     to keep the storage footprint below the 512 MB allocation.
+    #
+    #     Returns
+    #     -------
+    #     None : None
+    #         No return value.
+    #     """
+    #     print('Deleting all local raw and zarr files')
+    #     for i in ['*.raw*', '*.zarr']:
+    #         for j in glob.glob(i):
+    #             # print(f'Deleting {j}')
+    #             if os.path.isdir(j):
+    #                 shutil.rmtree(j, ignore_errors=True)
+    #             elif os.path.isfile(j):
+    #                 os.remove(j)
+
+    ############################################################################
+    # def __set_processing_status(
+    #         self,
+    #         ship_name: str,
+    #         cruise_name: str,
+    #         sensor_name: str,
+    #         file_name: str,
+    #         new_status: str
+    # ):
+    #     # Updates PIPELINE_STATUS via new_status value
+    #     # HASH: FILE_NAME, RANGE: SENSOR_NAME
+    #     self.__dynamo.put_item(
+    #         table_name=self.__table_name,
+    #         item={
+    #             'FILE_NAME': {'S': file_name},  # HASH
+    #             'SHIP_NAME': {'S': ship_name},
+    #             'CRUISE_NAME': {'S': cruise_name},
+    #             'SENSOR_NAME': {'S': sensor_name},  # RANGE
+    #             'PIPELINE_TIME': {'S': datetime.now().isoformat(timespec="seconds") + "Z"},
+    #             'PIPELINE_STATUS': {'S': new_status},
+    #         }
+    #     )
+
+    ############################################################################
+    # def __update_processing_status(
+    #         self,
+    #         cruise_name,
+    #         file_name,
+    #         new_status
+    # ):
+    #     self.__dynamo.update_item(
+    #         table_name=self.__table_name,
+    #         key={
+    #             'FILE_NAME': {'S': file_name},  # Partition Key
+    #             'CRUISE_NAME': {'S': cruise_name},  # Sort Key
+    #         },
+    #         expression='SET #PS = :ps',
+    #         attribute_names={
+    #             '#PS': 'PIPELINE_STATUS'
+    #         },
+    #         attribute_values={
+    #             ':ps': {
+    #                 'S': new_status
+    #             }
+    #         }
+    #     )
 
     ############################################################################
     def __get_processing_status(
             self,
             file_name,
             cruise_name
     ):
@@ -208,80 +206,80 @@
                     'L': [{'S': i} for i in channels]
                 }
             }
         )
 
     ############################################################################
     ############################################################################
-    def __write_geojson_to_file(
-            self,
-            store_name,
-            data
-    ) -> None:
-        """Write the GeoJSON file inside the Zarr store folder. Note that the
-        file is not a technical part of the store, this is more of a hack
-        to help pass the data along to the next processing step.
-
-        Parameters
-        ----------
-        path : str
-            The path to a local Zarr store where the file will be written.
-        data : str
-            A GeoJSON Feature Collection to be written to output file.
-
-        Returns
-        -------
-        None : None
-            No return value.
-        """
-        with open(os.path.join(store_name, 'geo.json'), "w") as outfile:
-            outfile.write(data)
-
-    ############################################################################
-    ############################################################################
-    def __remove_existing_s3_objects(
-            self,
-            prefix
-    ):
-        print(f'Removing existing s3 objects from: {self.__output_bucket} with prefix {prefix}')
-        keys = self.__s3.list_objects(
-            bucket_name=self.__output_bucket,
-            prefix=prefix,
-            access_key_id=self.__output_bucket_access_key,
-            secret_access_key=self.__output_bucket_secret_access_key
-        )
-        for key in keys:
-            self.__s3.delete_object(
-                bucket_name=self.__output_bucket,
-                key=key,
-                access_key_id=self.__output_bucket_access_key,
-                secret_access_key=self.__output_bucket_secret_access_key
-            )
-        print('Removing existing s3 objects done')
-
-    ############################################################################
-    def __upload_files(
-            self,
-            local_directory,
-            object_prefix
-    ):
-        print('Upload files')
-        for subdir, dirs, files in os.walk(local_directory):
-            for file in files:
-                local_path = os.path.join(subdir, file)
-                # print(local_path)
-                s3_key = os.path.join(object_prefix, local_path)
-                self.__s3.upload_file(
-                    file_name=local_path,
-                    bucket_name=self.__output_bucket,
-                    key=s3_key,
-                    access_key_id=self.__output_bucket_access_key,
-                    secret_access_key=self.__output_bucket_secret_access_key
-                )
-        # print('Done uploading files')
+    # def __write_geojson_to_file(
+    #         self,
+    #         store_name,
+    #         data
+    # ) -> None:
+    #     """Write the GeoJSON file inside the Zarr store folder. Note that the
+    #     file is not a technical part of the store, this is more of a hack
+    #     to help pass the data along to the next processing step.
+    #
+    #     Parameters
+    #     ----------
+    #     path : str
+    #         The path to a local Zarr store where the file will be written.
+    #     data : str
+    #         A GeoJSON Feature Collection to be written to output file.
+    #
+    #     Returns
+    #     -------
+    #     None : None
+    #         No return value.
+    #     """
+    #     with open(os.path.join(store_name, 'geo.json'), "w") as outfile:
+    #         outfile.write(data)
+
+    ############################################################################
+    ############################################################################
+    # def __remove_existing_s3_objects(
+    #         self,
+    #         prefix
+    # ):
+    #     print(f'Removing existing s3 objects from: {self.__output_bucket} with prefix {prefix}')
+    #     keys = self.__s3.list_objects(
+    #         bucket_name=self.__output_bucket,
+    #         prefix=prefix,
+    #         access_key_id=self.__output_bucket_access_key,
+    #         secret_access_key=self.__output_bucket_secret_access_key
+    #     )
+    #     for key in keys:
+    #         self.__s3.delete_object(
+    #             bucket_name=self.__output_bucket,
+    #             key=key,
+    #             access_key_id=self.__output_bucket_access_key,
+    #             secret_access_key=self.__output_bucket_secret_access_key
+    #         )
+    #     print('Removing existing s3 objects done')
+
+    ############################################################################
+    # def __upload_files(
+    #         self,
+    #         local_directory,
+    #         object_prefix
+    # ):
+    #     print('Upload files')
+    #     for subdir, dirs, files in os.walk(local_directory):
+    #         for file in files:
+    #             local_path = os.path.join(subdir, file)
+    #             # print(local_path)
+    #             s3_key = os.path.join(object_prefix, local_path)
+    #             self.__s3.upload_file(
+    #                 file_name=local_path,
+    #                 bucket_name=self.__output_bucket,
+    #                 key=s3_key,
+    #                 access_key_id=self.__output_bucket_access_key,
+    #                 secret_access_key=self.__output_bucket_secret_access_key
+    #             )
+    #     # print('Done uploading files')
 
     ############################################################################
     #####################################################################
 
     def __get_table_as_dataframe(
             self,
             ship_name: str,
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,41 +5,34 @@
 from .s3_operations import S3Operations
 from .s3fs_operations import S3FSOperations
 from .dynamo_operations import DynamoOperations
 from .sns_operations import SnsOperations
 
 
 table_name = os.environ['TABLE_NAME']
-# input_bucket = os.environ['INPUT_BUCKET']
 output_bucket = os.environ['OUTPUT_BUCKET']
 output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
 output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
 done_topic_arn = os.environ['TOPIC_ARN']
 
 executor = LambdaExecutor(
     s3_operations=S3Operations(),
     s3fs_operations=S3FSOperations(),
     dynamo_operations=DynamoOperations(),
     sns_operations=SnsOperations(),
-    # input_bucket=input_bucket,
     output_bucket=output_bucket,
     table_name=table_name,
     output_bucket_access_key=os.getenv('OUTPUT_BUCKET_ACCESS_KEY'),
     output_bucket_secret_access_key=os.getenv('OUTPUT_BUCKET_SECRET_ACCESS_KEY'),
     done_topic_arn=done_topic_arn
 )
 
 def handler(sns_event, context):
     print(f"table name: {os.environ['TABLE_NAME']}")
-    # print(f"input bucket: {os.environ['INPUT_BUCKET']}")
     print(f"output bucket: {os.environ['OUTPUT_BUCKET']}")
-    if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
-        print(os.environ['OUTPUT_BUCKET_ACCESS_KEY'])
-    if 'OUTPUT_BUCKET_SECRET_ACCESS_KEY' in os.environ:
-        print(os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY'])
     #
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
         print("Start Message : " + str(message))
         executor.execute(message)
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230726184718
+Version: 1.0.0.dev20230726225322
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726225322/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

