# Comparing `tmp/caselockerapi-0.0.9.tar.gz` & `tmp/caselockerapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caselockerapi-0.0.9.tar", last modified: Wed Jan 12 15:27:02 2022, max compression
+gzip compressed data, was "caselockerapi-0.1.1.tar", last modified: Thu Jul 27 17:04:44 2023, max compression
```

## Comparing `caselockerapi-0.0.9.tar` & `caselockerapi-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,33 @@
-drwxrwxr-x   0 skorux    (1000) skorux    (1000)        0 2022-01-12 15:27:02.262598 caselockerapi-0.0.9/
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)    33040 2020-10-19 19:23:19.000000 caselockerapi-0.0.9/COPYING
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)     7815 2020-10-19 19:23:19.000000 caselockerapi-0.0.9/COPYING.LESSER
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)      743 2020-10-19 19:23:19.000000 caselockerapi-0.0.9/LICENSE
--rw-rw-r--   0 skorux    (1000) skorux    (1000)      596 2022-01-12 15:27:02.262598 caselockerapi-0.0.9/PKG-INFO
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)        0 2020-10-19 19:23:19.000000 caselockerapi-0.0.9/README.md
-drwxrwxr-x   0 skorux    (1000) skorux    (1000)        0 2022-01-12 15:27:02.262598 caselockerapi-0.0.9/caselockerapi/
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)        0 2020-10-19 19:23:19.000000 caselockerapi-0.0.9/caselockerapi/__init__.py
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)     3161 2021-02-01 21:42:42.000000 caselockerapi-0.0.9/caselockerapi/auth.py
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)    36562 2022-01-12 03:38:00.000000 caselockerapi-0.0.9/caselockerapi/client.py
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)      330 2021-08-04 19:13:14.000000 caselockerapi-0.0.9/caselockerapi/utils.py
-drwxrwxr-x   0 skorux    (1000) skorux    (1000)        0 2022-01-12 15:27:02.262598 caselockerapi-0.0.9/caselockerapi.egg-info/
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)      596 2022-01-12 15:27:02.000000 caselockerapi-0.0.9/caselockerapi.egg-info/PKG-INFO
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)      328 2022-01-12 15:27:02.000000 caselockerapi-0.0.9/caselockerapi.egg-info/SOURCES.txt
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)        1 2022-01-12 15:27:02.000000 caselockerapi-0.0.9/caselockerapi.egg-info/dependency_links.txt
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)        9 2022-01-12 15:27:02.000000 caselockerapi-0.0.9/caselockerapi.egg-info/requires.txt
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)       14 2022-01-12 15:27:02.000000 caselockerapi-0.0.9/caselockerapi.egg-info/top_level.txt
--rw-rw-r--   0 skorux    (1000) skorux    (1000)       38 2022-01-12 15:27:02.262598 caselockerapi-0.0.9/setup.cfg
--rwxrwxrwx   0 skorux    (1000) skorux    (1000)      792 2022-01-12 15:22:49.000000 caselockerapi-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:44.222261 caselockerapi-0.1.1/
+-rw-rw-rw-   0        0        0    33040 2022-03-12 00:45:31.000000 caselockerapi-0.1.1/COPYING
+-rw-rw-rw-   0        0        0     7815 2022-03-12 00:45:31.000000 caselockerapi-0.1.1/COPYING.LESSER
+-rw-rw-rw-   0        0        0      743 2022-03-12 00:45:31.000000 caselockerapi-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-07-27 17:04:44.221761 caselockerapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-03-12 00:45:31.000000 caselockerapi-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:44.184142 caselockerapi-0.1.1/caselockerapi/
+-rw-rw-rw-   0        0        0        0 2023-05-12 16:47:33.000000 caselockerapi-0.1.1/caselockerapi/__init__.py
+-rw-rw-rw-   0        0        0     3161 2023-05-12 16:47:33.000000 caselockerapi-0.1.1/caselockerapi/auth.py
+-rw-rw-rw-   0        0        0    38889 2023-05-12 16:47:33.000000 caselockerapi-0.1.1/caselockerapi/client.py
+-rw-rw-rw-   0        0        0      330 2023-05-12 16:47:33.000000 caselockerapi-0.1.1/caselockerapi/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:44.193154 caselockerapi-0.1.1/caselockerapi.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-07-27 17:04:44.000000 caselockerapi-0.1.1/caselockerapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2023-07-27 17:04:44.000000 caselockerapi-0.1.1/caselockerapi.egg-info/SOURCES.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:44.170133 caselockerapi-0.1.1/caselockerapi.egg-info/build/
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:44.170634 caselockerapi-0.1.1/caselockerapi.egg-info/build/lib/
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:44.207167 caselockerapi-0.1.1/caselockerapi.egg-info/build/lib/caselockerapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 00:45:32.000000 caselockerapi-0.1.1/caselockerapi.egg-info/build/lib/caselockerapi/__init__.py
+-rw-rw-rw-   0        0        0     3161 2022-03-12 00:45:32.000000 caselockerapi-0.1.1/caselockerapi.egg-info/build/lib/caselockerapi/auth.py
+-rw-rw-rw-   0        0        0    38470 2023-01-12 19:02:20.000000 caselockerapi-0.1.1/caselockerapi.egg-info/build/lib/caselockerapi/client.py
+-rw-rw-rw-   0        0        0      330 2022-03-12 00:45:32.000000 caselockerapi-0.1.1/caselockerapi.egg-info/build/lib/caselockerapi/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:44.219759 caselockerapi-0.1.1/caselockerapi.egg-info/caselockerapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 00:45:32.000000 caselockerapi-0.1.1/caselockerapi.egg-info/caselockerapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:44.220759 caselockerapi-0.1.1/caselockerapi.egg-info/caselockerapi/__pycache__/
+-rw-rw-rw-   0        0        0      152 2022-03-12 00:45:32.000000 caselockerapi-0.1.1/caselockerapi.egg-info/caselockerapi/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3161 2022-03-12 00:45:32.000000 caselockerapi-0.1.1/caselockerapi.egg-info/caselockerapi/auth.py
+-rw-rw-rw-   0        0        0    38551 2023-02-24 01:22:00.000000 caselockerapi-0.1.1/caselockerapi.egg-info/caselockerapi/client.py
+-rw-rw-rw-   0        0        0      330 2022-03-12 00:45:32.000000 caselockerapi-0.1.1/caselockerapi.egg-info/caselockerapi/utils.py
+-rw-rw-rw-   0        0        0        1 2023-07-27 17:04:44.000000 caselockerapi-0.1.1/caselockerapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 17:04:44.000000 caselockerapi-0.1.1/caselockerapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-27 17:04:44.000000 caselockerapi-0.1.1/caselockerapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 17:04:44.222760 caselockerapi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-07-27 16:56:08.000000 caselockerapi-0.1.1/setup.py
```

### Comparing `caselockerapi-0.0.9/COPYING` & `caselockerapi-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `caselockerapi-0.0.9/COPYING.LESSER` & `caselockerapi-0.1.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `caselockerapi-0.0.9/LICENSE` & `caselockerapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caselockerapi-0.0.9/caselockerapi/auth.py` & `caselockerapi-0.1.1/caselockerapi/auth.py`

 * *Files identical despite different names*

### Comparing `caselockerapi-0.0.9/caselockerapi/client.py` & `caselockerapi-0.1.1/caselockerapi.egg-info/build/lib/caselockerapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dataclasses import field
 import datetime
 import shutil
 import os
 import sys
 import getpass
 import argparse
 import logging
@@ -16,14 +17,18 @@
 
 class Client(object):
     def __init__(self, token=False):
         self.session = Session()
         if token:
             self.token = token
 
+    def keep_alive(self):
+        if self.token.expires + datetime.timedelta(minutes=1) < datetime.datetime.now():
+            self.token.refresh()
+
     def _auth_headers(self):
         if self.token.expires + datetime.timedelta(minutes=1) < datetime.datetime.now():
             self.token.refresh()
         return {
             'Authorization': 'Bearer {}'.format(self.token),
         }
 
@@ -270,38 +275,48 @@
                                 index = int(clean_key.split("-")[2])
                                 new_id = conversion_table['{}-{}'.format(question_id, fieldtype_id)]
                                 nqn = new_id.split('-')[0]
                                 answers = self.get_answers(pk)
                                 answer_list = answers['answerlists']
                                 lid_array = answer_list[nqn]
                                 list_id = lid_array[index - 1]
+                                print(list_id)
                         if "key:{}".format(clean_key.split("-")[2]) in map_list:
                             list_uuid = map_list["key:{}".format(clean_key.split("-")[2])]
                         else:
                             import uuid
                             map_list["key:{}".format(clean_key.split("-")[2])] = uuid.uuid4()
                             list_uuid = map_list["key:{}".format(clean_key.split("-")[2])]
                 if "D:" in key:
                     if "/" in answer_key[key]:
-                        answer = {
-                            'month': int(answer_key[key].split('/')[0]),
-                            'day': int(answer_key[key].split('/')[1]),
-                            'year': int(answer_key[key].split('/')[2])
-                        }
+                        if len(answer_key[key].split('/')) == 3:
+                            answer = {
+                                'month': int(answer_key[key].split('/')[0]),
+                                'day': int(answer_key[key].split('/')[1]),
+                                'year': int(answer_key[key].split('/')[2])
+                            }
+                        else:
+                            answer = {
+                                'month': int(answer_key[key].split('/')[0]),
+                                'day': None,
+                                'year': int(answer_key[key].split('/')[1])
+                            }
                     else:
                         answer = {
                             'month': None,
                             'day': None,
                             'year': int(answer_key[key])
                         }
                 elif "O:" in key:
                     if fieldtype_id in options:
                         option_list = options[fieldtype_id]
                         for option in option_list['options']:
-                            if option['text'] == answer_key[key]:
+                            if answer_key[key].lower() == "mi" and option['text'] == "Michigan":
+                                answer = option['id']
+                            if option['text'].lower() == answer_key[key].lower():
                                 answer = option['id']
                     else:
                         raise Exception("Can't lookup answer for option")
                 elif "S:" in key:
                     p1_name = answer_key[key].split(";")[0]
                     p1_email = answer_key[key].split(";")[1]
                     answer = {
@@ -340,20 +355,24 @@
                     "fieldtype_clid": fieldtype_id,
                     "question_clid": question_id,
                     "list_id": list_id,
                     "client_id": str(list_uuid) if list_uuid and list_id == None else None,
                     "answer": answer
                 }
                 self.save_answer(pk, ans_obj)
-            except:
+            except Exception as e:
+                print(e)
                 print("Error: Failed to save an answer; Skipping {} - {}".format(answer_key[key], key))
 
     def save_file_answer(self, pk, file, **kwargs):
         return self.client.request('PUT', format_url(self.BASE_URL) + '{}/answer/'.format(pk), files=file, **kwargs).json()
 
+    def save_esign_upload(self, pk, file, **kwargs):
+        return self.client.request('POST', format_url(self.BASE_URL) + '{}/esign/'.format(pk), files=file, **kwargs).json()
+
     def downloadFileAnswer(self, pk, fieldtype, question, path, list_id=None, **kwargs):
         with self.client.request('GET',
                           format_url('userforms/userforms/{}/download/'.format(
                               pk
                           )),
                           params={
                               'fieldtype_id': question,
@@ -530,54 +549,58 @@
             return sec_id_array
 
         for root in template['root_parts']:
             if root['part_type'] == "s" and root['archived'] == False:
                 id_array.update(PARSE_SECTION(root))
         return id_array
 
-    def import_form(self, json):
+    def import_form(self, json, ignore_clid = False):
         fieldtype_dict = {}
         def CREATE_TEMPLATE(template):
             template_client = FormTemplate(self.client)
             createdTemplate = template_client.post({
                 'name': template['name'],
                 'header_text': template['header_text'],
                 'submission_fill_blank': template['submission_prop']['fill_blanks'],
                 'submission_min_rows': template['submission_prop']['hide_blank_rows']
             })
             for fieldtype in template['fieldtypes']:
                 fieldtype_obj = template['fieldtypes'][fieldtype]
                 if 'subfieldtypes' in fieldtype_obj:
                     pass
                 else:
-                    fieldtype_id = CREATE_FIELDTYPE(fieldtype_obj)
-                    fieldtype_dict[fieldtype] = fieldtype_id
+                    if fieldtype not in fieldtype_dict:
+                        fieldtype_id = CREATE_FIELDTYPE(fieldtype_obj, ignore_clid)
+                        fieldtype_dict[fieldtype] = fieldtype_id
             for fieldtype in template['fieldtypes']:
                 fieldtype_obj = template['fieldtypes'][fieldtype]
                 if 'subfieldtypes' in fieldtype_obj:
                     old_subfields = fieldtype_obj['subfieldtypes']
                     fieldtype_obj['subfieldtypes'] = []
                     for subfield in old_subfields:
                         fieldtype_obj['subfieldtypes'].append(fieldtype_dict[subfield])
-                    fieldtype_id = CREATE_FIELDTYPE(fieldtype_obj)
-                    fieldtype_dict[fieldtype] = fieldtype_id
+                    if fieldtype not in fieldtype_dict:
+                        fieldtype_id = CREATE_FIELDTYPE(fieldtype_obj, ignore_clid)
+                        fieldtype_dict[fieldtype] = fieldtype_id
                 
             CREATE_ROOT_PARTS(template['parts'], createdTemplate['id'])
 
-        def CREATE_FIELDTYPE(ftobj):
+        def CREATE_FIELDTYPE(ftobj, ignore_clid = False):
             fieldtype = {}
+            if ignore_clid:
+                ftobj['clid'] == None
             if 'atomic_type' in ftobj:
                 if ftobj['atomic_type'] in ["text", "textarea", "date", "harddate", "number", "currency", "file", "email", "ssn", "altesign"]:
-                    fieldtype = CREATE_BASIC_FIELDTYPE(ftobj['atomic_type'], ftobj['clid'], ftobj['required'] if 'required' in ftobj else False, ftobj)
+                    fieldtype = CREATE_BASIC_FIELDTYPE(ftobj['atomic_type'], None if ignore_clid else ftobj['clid'], ftobj['required'] if 'required' in ftobj else False, ftobj)
                 elif ftobj['atomic_type'] in ["regex"]:
-                    fieldtype = CREATE_REGEX_FIELDTYPE('regex', ftobj['clid'], ftobj['required'] if 'required' in ftobj else False, ftobj)
+                    fieldtype = CREATE_REGEX_FIELDTYPE('regex', None if ignore_clid else ftobj['clid'], ftobj['required'] if 'required' in ftobj else False, ftobj)
                 elif ftobj['atomic_type'] in ["radio", "checkbox", "dropdown"]:
-                    fieldtype = CREATE_OPTION_FIELDTYPE(ftobj['atomic_type'], ftobj['options'], ftobj['clid'], ftobj['required'] if 'required' in ftobj else False, ftobj)
+                    fieldtype = CREATE_OPTION_FIELDTYPE(ftobj['atomic_type'], ftobj['options'], None if ignore_clid else ftobj['clid'], ftobj['required'] if 'required' in ftobj else False, ftobj)
             elif 'subfieldtypes' in ftobj:
-                fieldtype = CREATE_COMPLEX_FIELDTYPE(ftobj['subfieldtypes'], ftobj['clid'])
+                fieldtype = CREATE_COMPLEX_FIELDTYPE(ftobj['subfieldtypes'], None if ignore_clid else ftobj['clid'])
             return fieldtype
 
         def CREATE_COMPLEX_FIELDTYPE(subFieldTypes, clid=None, required=False):
             fieldtype_client = FieldType(self.client)
             fieldtype_hold = fieldtype_client.post({
                 'atomic_type': None,
                 'option_list': None,
@@ -632,15 +655,15 @@
                 'part_type': 'q',
                 'section': sectionId,
                 'template': templateId,
                 'text': question['text'] if 'text' in question else None,
                 'read_only': question['read_only'] if 'read_only' in question else False,
                 'web_only': question['web_only'] if 'web_only' in question else False,
                 'archived': question['archived'] if 'archived' in question else False,
-                'clid': question['clid'] if 'clid' in question else None,
+                'clid': question['clid'] if 'clid' in question and ignore_clid is False else None,
                 'required': question['required'] if 'required' in question else False
             })
 
         def CREATE_BASIC_FIELDTYPE(fieldType, clid=None, required=False, ftobj={}):
             fieldtype_client = FieldType(self.client)
             return fieldtype_client.post({
                 'atomic_type': fieldType,
@@ -731,14 +754,27 @@
     BASE_URL = 'reports/reports/'
 
     #downloadReport
 
 class Users(CaseObject):
     BASE_URL = 'users/users/'
 
+    def create_user(self, fname, lname, password, email, username, admin, **kwargs):
+        obj = {
+            "email": email,
+            "username": username,
+            "first_name": fname,
+            "last_name": lname,
+            "password": password,
+            "contacttag_subscriptions": [],
+            "userformtag_subscriptions": [],
+            "is_org_admin": admin
+        }
+        return self.client.request('POST', format_url(self.BASE_URL), json=obj, **kwargs).json()
+
     #resetPassword
 
 class SuperOrgs(CaseObject):
     BASE_URL = 'users/admin-orgs/'
 
     def create_org(self, subdomain, name, **kwargs):
         obj = {
```

### Comparing `caselockerapi-0.0.9/setup.py` & `caselockerapi-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="caselockerapi",
-    version="0.0.9",
+    version="0.1.1",
     author="Litigation Locker",
     author_email="help@litigationlocker.com",
     description="Python API to interact with CaseLocker installation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://litigationlocker.com/",
     packages=setuptools.find_packages(),
```

