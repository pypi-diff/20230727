# Comparing `tmp/heaserver-trash-aws-s3-1.0.0a5.tar.gz` & `tmp/heaserver-trash-aws-s3-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a5.tar", last modified: Fri May  5 23:28:48 2023, max compression
+gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a6.tar", last modified: Thu Jul 27 02:23:54 2023, max compression
```

## Comparing `heaserver-trash-aws-s3-1.0.0a5.tar` & `heaserver-trash-aws-s3-1.0.0a6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.351024 heaserver-trash-aws-s3-1.0.0a5/
--rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a5/LICENSE
--rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a5/MANIFEST.in
--rw-rw-rw-   0        0        0     4352 2023-05-05 23:28:48.350023 heaserver-trash-aws-s3-1.0.0a5/PKG-INFO
--rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 23:28:48.351024 heaserver-trash-aws-s3-1.0.0a5/setup.cfg
--rw-rw-rw-   0        0        0     1869 2023-05-05 23:28:04.000000 heaserver-trash-aws-s3-1.0.0a5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/
-drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/__init__.py
--rw-rw-rw-   0        0        0    48660 2023-05-05 23:05:37.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/service.py
-drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/wstl/
--rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.345024 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     4352 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/tests/
-drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.349023 heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/__init__.py
--rw-rw-rw-   0        0        0    69298 2023-04-26 23:41:02.000000 heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/test_all.py
--rw-rw-rw-   0        0        0     6276 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/testcase.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.556165 heaserver-trash-aws-s3-1.0.0a6/
+-rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a6/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4352 2023-07-27 02:23:54.555167 heaserver-trash-aws-s3-1.0.0a6/PKG-INFO
+-rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 02:23:54.556165 heaserver-trash-aws-s3-1.0.0a6/setup.cfg
+-rw-rw-rw-   0        0        0     1869 2023-07-27 02:23:18.000000 heaserver-trash-aws-s3-1.0.0a6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.514853 heaserver-trash-aws-s3-1.0.0a6/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.513858 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/
+drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.522856 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/__init__.py
+-rw-rw-rw-   0        0        0    48660 2023-05-20 05:24:56.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/service.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.524853 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/wstl/
+-rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.550165 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     4352 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 02:23:54.000000 heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.515853 heaserver-trash-aws-s3-1.0.0a6/tests/
+drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.515853 heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-07-27 02:23:54.554169 heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/__init__.py
+-rw-rw-rw-   0        0        0    68605 2023-07-27 02:15:49.000000 heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/test_all.py
+-rw-rw-rw-   0        0        0     6281 2023-07-27 02:05:15.000000 heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/testcase.py
```

### Comparing `heaserver-trash-aws-s3-1.0.0a5/LICENSE` & `heaserver-trash-aws-s3-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a5/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a5/README.md` & `heaserver-trash-aws-s3-1.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a5/setup.py` & `heaserver-trash-aws-s3-1.0.0a6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-trash-aws-s3',
-    version='1.0.0a5',
+    version='1.0.0a6',
     description="deleted file management",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
       package_dir={'': 'src'},
       packages=['heaserver.trashawss3'],
       package_data={'heaserver.trashawss3': ['wstl/*.json']},
       install_requires=[
-          'heaserver>=1.0.0a117, <1.0.0a118'
+          'heaserver>=1.0.0a158, <1.0.0a159'
       ],
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Environment :: Console',
           'Intended Audience :: Developers',
           'Natural Language :: English',
           'License :: OSI Approved :: Apache Software License',
```

### Comparing `heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/service.py` & `heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/wstl/all.json` & `heaserver-trash-aws-s3-1.0.0a6/src/heaserver/trashawss3/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt` & `heaserver-trash-aws-s3-1.0.0a6/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/test_all.py` & `heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/test_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from heaobject.awss3key import decode_key
 from heaserver.service.testcase.mixin import _ordered
 import boto3
 from heaserver.service.testcase.collection import query_fixtures
 from heaserver.trashawss3.service import TRASHAWSS3_COLLECTION
 from heaserver.trashawss3 import service
 from heaserver.service.testcase.aiohttptestcase import HEAAioHTTPTestCase
-from heaserver.service.testcase.mockaws import MockS3ManagerWithMockMongo
+from heaserver.service.testcase.mockaws import MockS3WithMockMongoManager
 from heaserver.service.representor import nvpjson
 from heaserver.service.appproperty import HEA_DB
 from moto import mock_s3, mock_organizations, mock_sts
 from freezegun import freeze_time
 from aiohttp.web import Application
 from aiohttp import hdrs
 from heaserver.service import runner
 from heaserver.service import wstl
 from contextlib import ExitStack, closing
 import logging
 
 
 class TestTrash(HEAAioHTTPTestCase):
     def run(self, result=None):
-        with self._caplog.at_level(logging.DEBUG), mock_s3(), mock_organizations(), mock_sts(), closing(MockS3ManagerWithMockMongo()) as db, ExitStack() as es, freeze_time("2022-05-17"):
+        with self._caplog.at_level(logging.DEBUG), mock_s3(), mock_organizations(), mock_sts(), closing(MockS3WithMockMongoManager()) as db, ExitStack() as es, freeze_time("2022-05-17"):
             self.__db = db
             self.__db.start_database(es)
             self.__db.insert_desktop_objects(query_fixtures(
                 fixtures=db_store, db_manager=self.__db, name='volumes'))
             self.__db.insert_desktop_objects(query_fixtures(
                 fixtures=db_store, db_manager=self.__db, name='buckets'))
             self.__db.insert_desktop_objects(query_fixtures(
@@ -97,36 +97,36 @@
                                             {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                             {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                             {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
-                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
-                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
-                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'},
-                                            {'prompt': 'View volume', 'rel': 'hea-volume', 'href': 'http://localhost:8080/volumes/666f6f2d6261722d71757578'},
-                                            {'prompt': 'View account', 'rel': 'hea-account', 'href': 'http://localhost:8080/volumes/666f6f2d6261722d71757578/awsaccounts/me'}]}],
+                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
+                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
+                                            {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'},
+                                            {'prompt': 'View volume', 'rel': 'hea-volume', 'href': '/volumes/666f6f2d6261722d71757578'},
+                                            {'prompt': 'View account', 'rel': 'hea-account', 'href': '/volumes/666f6f2d6261722d71757578/awsaccounts/me'}]}],
                                       'template': {'prompt': 'Properties', 'rel': 'hea-properties hea-context-menu',
                                                    'data': [
                                                         {'name': 'id', 'value': f'VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', 'prompt': 'Id', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'display_name', 'value': 'TextFileUTF8.txt', 'prompt': 'Name', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'original_location', 'value': '/arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'Original location', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'Type', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'description', 'value': None, 'prompt': 'Description', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'textarea'},
                                                         {'name': 'size', 'value': 0, 'prompt': 'Size in bytes', 'required': False, 'readOnly': False, 'pattern': None, 'display': False},
                                                         {'name': 'human_readable_size', 'value': '0 Bytes', 'prompt': 'Size', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'Storage class', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/TextFileUTF8.txt', 'prompt': 'S3 URI', 'required': False, 'readOnly': True, 'pattern': None},
                                                         {'name': 'mime_type', 'value': None, 'prompt': 'MIME Type', 'required': False, 'readOnly': True, 'pattern': None},
-                                                        {'name': 'owner', 'value': 'system|none', 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
+                                                        {'name': 'owner', 'value': 'system|none', 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                                         {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'Created', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                                         {'name': 'modified', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                                         {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
-                                                        {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
+                                                        {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                                         {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(_ordered(actual), _ordered(await resp.json()))
 
     async def test_get_deleted_item_nvpjson(self):
         async with self.client.get(f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA==,{self.__version1}', headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
             actual = [{'actual_object_id': 'VGV4dEZpbGVVVEY4LnR4dA==',
                        'actual_object_type_name':
@@ -246,17 +246,17 @@
                                               {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                               {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                               {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                               {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                               {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                               {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                            'links': [
-                                              {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
-                                              {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
-                                              {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
+                                              {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
+                                              {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
+                                              {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
                                             {'data': [
                                               {'name': 'actual_object_id', 'value': 'YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU=', 'prompt': 'actual_object_id', 'display': True},
                                               {'name': 'actual_object_type_name', 'value': 'heaobject.data.AWSS3FileObject', 'prompt': 'actual_object_type_name',  'display': True},
                                               {'name': 'actual_object_uri', 'value': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3files/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU=', 'prompt': 'actual_object_uri', 'display': True},
                                               {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                               {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
                                               {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
@@ -275,36 +275,36 @@
                                               {'name': 's3_uri', 'value': 's3://arp-scale-2-cloud-bucket-with-tags11/afolder/anotherfolder/BinaryFile', 'prompt': 's3_uri', 'display': True},
                                               {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True}, {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                               {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True}, {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                               {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                               {'name': 'version', 'value': self.__version2, 'prompt': 'version', 'display': True},
                                               {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                             'links': [
-                                              {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}/restorer'},
-                                              {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}/deleter'},
-                                              {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}'}]}],
+                                              {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}/restorer'},
+                                              {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}/deleter'},
+                                              {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci9hbm90aGVyZm9sZGVyL0JpbmFyeUZpbGU%3D%2C{self.__version2}'}]}],
                                       'template': {
                                         'prompt': 'Properties',
                                         'rel': 'hea-properties hea-context-menu',
                                         'data': [
                                             {'name': 'id', 'value': None, 'prompt': 'Id', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'display_name', 'value': None, 'prompt': 'Name', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'original_location', 'value': None, 'prompt': 'Original location', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'type', 'value': None, 'prompt': 'Type', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'description', 'value': None, 'prompt': 'Description', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'textarea'},
                                             {'name': 'size', 'value': None, 'prompt': 'Size in bytes', 'required': False, 'readOnly': False, 'pattern': None, 'display': False},
                                             {'name': 'human_readable_size', 'value': None, 'prompt': 'Size', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'Storage class', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 's3_uri', 'value': None, 'prompt': 'S3 URI', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'mime_type', 'value': None, 'prompt': 'MIME Type', 'required': False, 'readOnly': True, 'pattern': None},
-                                            {'name': 'owner', 'value': None, 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
+                                            {'name': 'owner', 'value': None, 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'name': 'created', 'value': None, 'prompt': 'Created', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'modified', 'value': None, 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'source', 'value': None, 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
-                                            {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
+                                            {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(_ordered(actual), _ordered(await resp.json()))
 
     async def test_get_deleted_items_invalid_folder_id(self):
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/toor/awss3trash') as resp:
             self.assertEqual(404, resp.status)
 
@@ -347,17 +347,17 @@
                                             {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True}, {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                             {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                             {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
-                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
-                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
-                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
+                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
+                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
+                                            {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
                                         {'data': [
                                             {'name': 'actual_object_id', 'value': 'YWZvbGRlci8=', 'prompt': 'actual_object_id', 'display': True},
                                             {'name': 'actual_object_type_name', 'value': 'heaobject.folder.AWSS3Folder', 'prompt': 'actual_object_type_name', 'display': True},
                                             {'name': 'actual_object_uri', 'value': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/YWZvbGRlci8=', 'prompt': 'actual_object_uri', 'display': True},
                                             {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                             {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
                                             {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
@@ -378,35 +378,35 @@
                                             {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                             {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                             {'name': 'version', 'value': self.__version2, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
-                                            {'prompt': 'Open', 'rel': 'hea-opener-choices hea-context-menu', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/opener'},
-                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/restorer'},
-                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/deleter'},
-                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}'}]}],
+                                            {'prompt': 'Open', 'rel': 'hea-opener-choices hea-context-menu', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/opener'},
+                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/restorer'},
+                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/deleter'},
+                                            {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}'}]}],
                                         'template': {'prompt': 'Properties', 'rel': 'hea-properties hea-context-menu',
                                           'data': [
                                             {'name': 'id', 'value': None, 'prompt': 'Id', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'display_name', 'value': None, 'prompt': 'Name', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'original_location', 'value': None, 'prompt': 'Original location', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'type', 'value': None, 'prompt': 'Type', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'description', 'value': None, 'prompt': 'Description', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'textarea'},
                                             {'name': 'size', 'value': None, 'prompt': 'Size in bytes', 'required': False, 'readOnly': False, 'pattern': None, 'display': False},
                                             {'name': 'human_readable_size', 'value': None, 'prompt': 'Size', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'Storage class', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 's3_uri', 'value': None, 'prompt': 'S3 URI', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'mime_type', 'value': None, 'prompt': 'MIME Type', 'required': False, 'readOnly': True, 'pattern': None},
-                                            {'name': 'owner', 'value': None, 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
+                                            {'name': 'owner', 'value': None, 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'name': 'created', 'value': None, 'prompt': 'Created', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'modified', 'value': None, 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'source', 'value': None, 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
-                                            {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
+                                            {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(actual, await resp.json())
 
     async def test_get_deleted_items_invalid_trash_folder(self):
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashfolders/toor/items') as resp:
             self.assertEqual(404, resp.status)
 
@@ -445,17 +445,17 @@
                                             {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True}, {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                             {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                             {'name': 'version', 'value': self.__version1, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
-                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
-                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
-                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
+                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/restorer'},
+                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}/deleter'},
+                                            {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/VGV4dEZpbGVVVEY4LnR4dA%3D%3D%2C{self.__version1}'}]},
                                         {'data': [
                                             {'name': 'actual_object_id', 'value': 'YWZvbGRlci8=', 'prompt': 'actual_object_id', 'display': True},
                                             {'name': 'actual_object_type_name', 'value': 'heaobject.folder.AWSS3Folder', 'prompt': 'actual_object_type_name', 'display': True},
                                             {'name': 'actual_object_uri', 'value': '/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/YWZvbGRlci8=', 'prompt': 'actual_object_uri', 'display': True},
                                             {'name': 'bucket_id', 'value': 'arp-scale-2-cloud-bucket-with-tags11', 'prompt': 'bucket_id', 'display': True},
                                             {'name': 'created', 'value': '2022-05-17T00:00:00+00:00', 'prompt': 'created', 'display': True},
                                             {'name': 'derived_by', 'value': None, 'prompt': 'derived_by', 'display': True},
@@ -476,35 +476,35 @@
                                             {'name': 'size', 'value': 0, 'prompt': 'size', 'display': True},
                                             {'name': 'source', 'value': 'AWS Simple Cloud Storage (S3)', 'prompt': 'source', 'display': True},
                                             {'name': 'storage_class', 'value': 'STANDARD', 'prompt': 'storage_class', 'display': True},
                                             {'name': 'type', 'value': 'heaobject.trash.AWSS3FolderFileTrashItem', 'prompt': 'type', 'display': True},
                                             {'name': 'version', 'value': self.__version2, 'prompt': 'version', 'display': True},
                                             {'name': 'volume_id', 'value': '666f6f2d6261722d71757578', 'prompt': 'volume_id', 'display': True}],
                                           'links': [
-                                            {'prompt': 'Open', 'rel': 'hea-opener-choices hea-context-menu', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/opener'},
-                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/restorer'},
-                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/deleter'},
-                                            {'prompt': 'View', 'rel': 'self', 'href': f'http://localhost:8080/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}'}]}],
+                                            {'prompt': 'Open', 'rel': 'hea-opener-choices hea-context-menu', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/opener'},
+                                            {'prompt': 'Restore', 'rel': 'hea-trash-restore-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/restorer'},
+                                            {'prompt': 'Permanently delete', 'rel': 'hea-trash-delete-confirmer hea-context-menu hea-confirm-prompt', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}/deleter'},
+                                            {'prompt': 'View', 'rel': 'self', 'href': f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trash/YWZvbGRlci8%3D%2C{self.__version2}'}]}],
                                         'template': {'prompt': 'Properties', 'rel': 'hea-properties hea-context-menu',
                                           'data': [
                                             {'name': 'id', 'value': None, 'prompt': 'Id', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'display_name', 'value': None, 'prompt': 'Name', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'original_location', 'value': None, 'prompt': 'Original location', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'type', 'value': None, 'prompt': 'Type', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'description', 'value': None, 'prompt': 'Description', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'textarea'},
                                             {'name': 'size', 'value': None, 'prompt': 'Size in bytes', 'required': False, 'readOnly': False, 'pattern': None, 'display': False},
                                             {'name': 'human_readable_size', 'value': None, 'prompt': 'Size', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'storage_class', 'value': None, 'prompt': 'Storage class', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 's3_uri', 'value': None, 'prompt': 'S3 URI', 'required': False, 'readOnly': True, 'pattern': None},
                                             {'name': 'mime_type', 'value': None, 'prompt': 'MIME Type', 'required': False, 'readOnly': True, 'pattern': None},
-                                            {'name': 'owner', 'value': None, 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
+                                            {'name': 'owner', 'value': None, 'prompt': 'Owner', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'name': 'created', 'value': None, 'prompt': 'Created', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'modified', 'value': None, 'prompt': 'Modified', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'datetime'},
                                             {'name': 'source', 'value': None, 'prompt': 'Source', 'required': False, 'readOnly': True, 'pattern': None},
-                                            {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': 'http://localhost:8080/people/', 'text': 'display_name', 'value': 'id'}},
+                                            {'section': 'shares', 'index': -1, 'sectionPrompt': 'Shares', 'name': 'user', 'value': None, 'prompt': 'User', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'options': {'href': '/people/', 'text': 'display_name', 'value': 'id'}},
                                             {'section': 'shares', 'index': -1, 'name': 'permissions', 'value': None, 'prompt': 'Permissions', 'required': False, 'readOnly': True, 'pattern': None, 'type': 'select', 'cardinality': 'multiple', 'options': [{'value': 'COOWNER', 'text': 'Co-owner'}, {'value': 'CREATOR', 'text': 'Creator'}, {'value': 'DELETER', 'text': 'Deleter'}, {'value': 'EDITOR', 'text': 'Editor'}, {'value': 'SHARER', 'text': 'Sharer'}, {'value': 'VIEWER', 'text': 'Viewer'}]}]}}}]
             self.assertEqual(actual, await resp.json())
 
     async def test_do_empty_trash_status(self):
         async with self.client.get('/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3trashemptier') as resp:
             self.assertEqual(204, resp.status)
```

### Comparing `heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/testcase.py` & `heaserver-trash-aws-s3-1.0.0a6/tests/heaserver/trashawss3test/testcase.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 """
 
 from heaserver.service.testcase.microservicetestcase import get_test_case_cls_default
 from heaserver.service.testcase import expectedvalues
 from heaserver.trashawss3 import service
 from heaobject.user import NONE_USER
 from heaobject.data import AWSS3FileObject
-from heaserver.service.testcase.mockaws import MockS3ManagerWithMockMongo
+from heaserver.service.testcase.mockmongo import MockMongoManager
+from heaserver.service.testcase.mockaws import MockS3Manager
 from heaserver.service.testcase.collection import CollectionKey
 
 
 db_store = {
-    CollectionKey(name='volumes', db_manager_cls=MockS3ManagerWithMockMongo): [{
+    CollectionKey(name='volumes', db_manager_cls=MockMongoManager): [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'My Amazon Web Services',
         'invited': [],
@@ -27,15 +28,15 @@
         'source': None,
         'type': 'heaobject.volume.Volume',
         'version': None,
         'file_system_name': 'amazon_web_services',
         'file_system_type': 'heaobject.volume.AWSFileSystem',
         'credential_id': None  # Let boto3 try to find the user's credentials.
     }],
-    CollectionKey(name='buckets', db_manager_cls=MockS3ManagerWithMockMongo): [{
+    CollectionKey(name='buckets', db_manager_cls=MockS3Manager): [{
         "arn": None,
         "created": '2022-05-17T00:00:00+00:00',
         "derived_by": None,
         "derived_from": [],
         "description": None,
         "display_name": "arp-scale-2-cloud-bucket-with-tags11",
         "encrypted": True,
@@ -55,15 +56,15 @@
         "size": None,
         "source": None,
         "tags": [],
         "type": "heaobject.bucket.AWSBucket",
         "version": None,
         "versioned": False
     }],
-    CollectionKey(name='awss3files', db_manager_cls=MockS3ManagerWithMockMongo): [{
+    CollectionKey(name='awss3files', db_manager_cls=MockS3Manager): [{
         'created': '2022-05-17T00:00:00+00:00',
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'TextFileUTF8.txt',
         'id': 'VGV4dEZpbGVVVEY4LnR4dA==',
         'invites': [],
@@ -106,15 +107,15 @@
             'mime_type': 'application/octet-stream',
             'size': 8673123,
             'human_readable_size': '8.7 MB',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
             'key': 'afolder/anotherfolder/BinaryFile'
     }
     ],
-    CollectionKey(name=service.TRASHAWSS3_COLLECTION, db_manager_cls=MockS3ManagerWithMockMongo): [{
+    CollectionKey(name=service.TRASHAWSS3_COLLECTION, db_manager_cls=MockS3Manager): [{
         'id': 'VGV4dEZpbGVVVEY4LnR4dA==,',
         'created': '2022-05-17T00:00:00+00:00',
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'TextFileUTF8.txt',
         'invited': [],
```

