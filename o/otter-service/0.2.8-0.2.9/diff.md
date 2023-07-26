# Comparing `tmp/otter_service-0.2.8.tar.gz` & `tmp/otter_service-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter_service-0.2.8.tar", last modified: Wed Jul 26 21:35:09 2023, max compression
+gzip compressed data, was "otter_service-0.2.9.tar", last modified: Wed Jul 26 22:17:54 2023, max compression
```

## Comparing `otter_service-0.2.8.tar` & `otter_service-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.915081 otter_service-0.2.8/
--rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.8/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)     9235 2023-07-26 21:35:09.915382 otter_service-0.2.8/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     8776 2023-07-26 18:31:30.000000 otter_service-0.2.8/README.md
--rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.8/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-26 21:35:09.917242 otter_service-0.2.8/setup.cfg
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.895963 otter_service-0.2.8/src/
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.905963 otter_service-0.2.8/src/otter_service/
--rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-26 21:34:48.000000 otter_service-0.2.8/src/otter_service/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     2149 2023-07-26 15:52:24.000000 otter_service-0.2.8/src/otter_service/access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1025 2023-07-21 21:37:40.000000 otter_service-0.2.8/src/otter_service/firestore-test.py
--rw-r--r--   0 sean       (501) staff       (20)     5320 2023-07-26 20:22:54.000000 otter_service-0.2.8/src/otter_service/grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)    19559 2023-07-26 21:23:52.000000 otter_service-0.2.8/src/otter_service/otter_nb.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.911740 otter_service-0.2.8/src/otter_service/secrets/
--rw-r--r--   0 sean       (501) staff       (20)     1043 2023-07-26 01:06:26.000000 otter_service-0.2.8/src/otter_service/secrets/gh_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.8/src/otter_service/secrets/gke_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)      516 2023-07-25 18:59:31.000000 otter_service-0.2.8/src/otter_service/util.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.909418 otter_service-0.2.8/src/otter_service.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     9235 2023-07-26 21:35:09.000000 otter_service-0.2.8/src/otter_service.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      610 2023-07-26 21:35:09.000000 otter_service-0.2.8/src/otter_service.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-26 21:35:09.000000 otter_service-0.2.8/src/otter_service.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-26 21:35:09.000000 otter_service-0.2.8/src/otter_service.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-26 21:35:09.000000 otter_service-0.2.8/src/otter_service.egg-info/top_level.txt
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.914527 otter_service-0.2.8/tests/
--rw-r--r--   0 sean       (501) staff       (20)      913 2023-07-26 00:57:35.000000 otter_service-0.2.8/tests/test_access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1187 2023-07-26 21:32:16.000000 otter_service-0.2.8/tests/test_grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)     2140 2023-07-21 23:00:39.000000 otter_service-0.2.8/tests/test_otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 22:17:54.128820 otter_service-0.2.9/
+-rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.9/LICENSE
+-rw-r--r--   0 sean       (501) staff       (20)     9235 2023-07-26 22:17:54.129001 otter_service-0.2.9/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)     8776 2023-07-26 18:31:30.000000 otter_service-0.2.9/README.md
+-rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.9/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-26 22:17:54.129727 otter_service-0.2.9/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 22:17:54.113955 otter_service-0.2.9/src/
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 22:17:54.121222 otter_service-0.2.9/src/otter_service/
+-rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-26 22:17:39.000000 otter_service-0.2.9/src/otter_service/__init__.py
+-rw-r--r--   0 sean       (501) staff       (20)     2149 2023-07-26 15:52:24.000000 otter_service-0.2.9/src/otter_service/access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1025 2023-07-21 21:37:40.000000 otter_service-0.2.9/src/otter_service/firestore-test.py
+-rw-r--r--   0 sean       (501) staff       (20)     5320 2023-07-26 20:22:54.000000 otter_service-0.2.9/src/otter_service/grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)    19692 2023-07-26 22:17:27.000000 otter_service-0.2.9/src/otter_service/otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 22:17:54.125425 otter_service-0.2.9/src/otter_service/secrets/
+-rw-r--r--   0 sean       (501) staff       (20)     1043 2023-07-26 01:06:26.000000 otter_service-0.2.9/src/otter_service/secrets/gh_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.9/src/otter_service/secrets/gke_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)      516 2023-07-25 18:59:31.000000 otter_service-0.2.9/src/otter_service/util.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 22:17:54.124130 otter_service-0.2.9/src/otter_service.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     9235 2023-07-26 22:17:54.000000 otter_service-0.2.9/src/otter_service.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      610 2023-07-26 22:17:54.000000 otter_service-0.2.9/src/otter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-26 22:17:54.000000 otter_service-0.2.9/src/otter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-26 22:17:54.000000 otter_service-0.2.9/src/otter_service.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-26 22:17:54.000000 otter_service-0.2.9/src/otter_service.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 22:17:54.128094 otter_service-0.2.9/tests/
+-rw-r--r--   0 sean       (501) staff       (20)      913 2023-07-26 00:57:35.000000 otter_service-0.2.9/tests/test_access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1187 2023-07-26 21:32:16.000000 otter_service-0.2.9/tests/test_grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)     2140 2023-07-21 23:00:39.000000 otter_service-0.2.9/tests/test_otter_nb.py
```

### Comparing `otter_service-0.2.8/LICENSE` & `otter_service-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/PKG-INFO` & `otter_service-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter_service
-Version: 0.2.8
+Version: 0.2.9
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.2.8/README.md` & `otter_service-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/setup.cfg` & `otter_service-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/src/otter_service/access_sops_keys.py` & `otter_service-0.2.9/src/otter_service/access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/src/otter_service/firestore-test.py` & `otter_service-0.2.9/src/otter_service/firestore-test.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/src/otter_service/grade_assignment.py` & `otter_service-0.2.9/src/otter_service/grade_assignment.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/src/otter_service/otter_nb.py` & `otter_service-0.2.9/src/otter_service/otter_nb.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,40 +98,40 @@
     :param course_id: the course id for this notebook
     :param assignment_id:  the assignment id for this notebook
     :return: formatted string
     """
     return f"course-v1%3A{course_id}:{os.environ['EDX_URL']}-{assignment_id}"
 
 
-async def post_grade(solutions_base_path, args):
+async def post_grade(solutions_base_path, metadata):
     """
     This posts the grade to the LTI server
     :paraem solutions_base_path: where the config file is to find the assignment id
-    :param args:
+    :param metadata:
         - userid: the user to post the grade for
         - grade: the grade as a float
         - course: the course this notebook is in
         - section: the section this notebook is in
         - assignment:  the assignment name for this notebook
     """
     body_hash = ""
     consumer_key = ""
     try:
         # post grade to EdX
         course_config = util.get_course_config(solutions_base_path)
-        course = args["course"]
-        section = args["section"]
-        assignment = args["assignment"]
-        user_id = args["userid"]
-        grade = args["grade"]
+        course = metadata["course"]
+        section = metadata["section"]
+        assignment = metadata["assignment"]
+        user_id = metadata["userid"]
+        grade = metadata["grade"]
 
         course_id = course_config[course][section]["course_id"]
         assignment_id = course_config[course][section]["assignments"][assignment]
 
-        log_info_csv(user_id, args, f"Edx Course Config Loaded: Course Id: {course_id}, Assignment_id: {assignment_id}")
+        log_info_csv(user_id, metadata, f"Edx Course Config Loaded: Course Id: {course_id}, Assignment_id: {assignment_id}")
 
         sourced_id = create_sourced_id(course_id, assignment_id)
         outcomes_url = create_post_url(course_id, assignment_id)
 
         # TODO: extract this into a real library with real XML parsing
         # WARNING: You can use this only with data you trust! Beware, etc.
         post_xml = r"""
@@ -203,15 +203,15 @@
         response_tree = etree.fromstring(resp_text.encode('utf-8'))
 
         # XML and its namespaces. UBOOF!
         status = response_tree.find('.//{http://www.imsglobal.org/services/ltiv1p1/xsd/imsoms_v1p0}imsx_statusInfo')
         code_major = status.find('{http://www.imsglobal.org/services/ltiv1p1/xsd/imsoms_v1p0}imsx_codeMajor').text
         desc = status.find('{http://www.imsglobal.org/services/ltiv1p1/xsd/imsoms_v1p0}imsx_description').text
 
-        log_info_csv(user_id, args, f"Posted to Edx: code: {code_major}, desc: {desc}")
+        log_info_csv(user_id, metadata, f"Posted to Edx: code: {code_major}, desc: {desc}")
 
         if code_major != 'success':
             raise GradePostException(desc)
 
     except GradePostException as grade_post_exception:
         raise grade_post_exception
     except Exception as ex:
@@ -304,15 +304,16 @@
                 if metadata["section"] is None:
                     metadata["section"] = "Section: problem getting section - not in notebook?"
                 if metadata["assignment"] is None:
                     metadata["assignment"] = "Assignment: problem getting assignment - not in notebook?"
 
             log_error_csv(user['name'], metadata, str(grade_submission_exception))
         except Exception as ex:  # pylint: disable=broad-except
-            log_error_csv(user, metadata, str(ex))
+            msg = ''.join(traceback.format_exception(etype=type(ex), value=ex, tb=ex.__traceback__))
+            log_error_csv(user, metadata, msg)
 
     async def _grade_and_post(self, args):
         """
         This is called by spawn_callback method on the IOLoop to move the actual grading and
         posting of the grade out of the main thread.
 
         :param args
```

### Comparing `otter_service-0.2.8/src/otter_service/secrets/gh_key.yaml` & `otter_service-0.2.9/src/otter_service/secrets/gh_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/src/otter_service/secrets/gke_key.yaml` & `otter_service-0.2.9/src/otter_service/secrets/gke_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/src/otter_service/util.py` & `otter_service-0.2.9/src/otter_service/util.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/src/otter_service.egg-info/PKG-INFO` & `otter_service-0.2.9/src/otter_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-service
-Version: 0.2.8
+Version: 0.2.9
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.2.8/src/otter_service.egg-info/SOURCES.txt` & `otter_service-0.2.9/src/otter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/tests/test_access_sops_keys.py` & `otter_service-0.2.9/tests/test_access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/tests/test_grade_assignment.py` & `otter_service-0.2.9/tests/test_grade_assignment.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.8/tests/test_otter_nb.py` & `otter_service-0.2.9/tests/test_otter_nb.py`

 * *Files identical despite different names*

