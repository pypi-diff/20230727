# Comparing `tmp/qcloud_user-1.0.3.tar.gz` & `tmp/qcloud_user-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_user-1.0.3.tar", last modified: Sun Jul 16 12:31:12 2023, max compression
+gzip compressed data, was "qcloud_user-1.0.4.tar", last modified: Thu Jul 27 12:15:53 2023, max compression
```

## Comparing `qcloud_user-1.0.3.tar` & `qcloud_user-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-16 12:31:12.339903 qcloud_user-1.0.3/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:49:28.000000 qcloud_user-1.0.3/LICENSE.txt
--rw-r-----   0 agilbert   (501) staff       (20)     4472 2023-07-16 12:31:12.339780 qcloud_user-1.0.3/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)     3473 2023-07-12 22:23:41.000000 qcloud_user-1.0.3/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      721 2023-07-16 12:28:49.000000 qcloud_user-1.0.3/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-16 12:31:12.339383 qcloud_user-1.0.3/qcloud_user.egg-info/
--rw-r-----   0 agilbert   (501) staff       (20)     4472 2023-07-16 12:31:12.000000 qcloud_user-1.0.3/qcloud_user.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      316 2023-07-16 12:31:12.000000 qcloud_user-1.0.3/qcloud_user.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2023-07-16 12:31:12.000000 qcloud_user-1.0.3/qcloud_user.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       44 2023-07-16 12:31:12.000000 qcloud_user-1.0.3/qcloud_user.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      153 2023-07-16 12:31:12.000000 qcloud_user-1.0.3/qcloud_user.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       12 2023-07-16 12:31:12.000000 qcloud_user-1.0.3/qcloud_user.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2023-07-16 12:31:12.339944 qcloud_user-1.0.3/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      793 2023-07-16 12:29:01.000000 qcloud_user-1.0.3/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-16 12:31:12.338219 qcloud_user-1.0.3/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-16 12:31:12.339606 qcloud_user-1.0.3/src/qcloud_user/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-27 02:16:27.000000 qcloud_user-1.0.3/src/qcloud_user/__init__.py
--rwxr-x---   0 agilbert   (501) staff       (20)    22671 2023-07-16 12:28:28.000000 qcloud_user-1.0.3/src/qcloud_user/qcloud_user.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:15:53.320183 qcloud_user-1.0.4/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:49:28.000000 qcloud_user-1.0.4/LICENSE.txt
+-rw-r-----   0 agilbert   (501) staff       (20)     4472 2023-07-27 12:15:53.320062 qcloud_user-1.0.4/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)     3473 2023-07-12 22:23:41.000000 qcloud_user-1.0.4/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      721 2023-07-27 12:15:04.000000 qcloud_user-1.0.4/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:15:53.319684 qcloud_user-1.0.4/qcloud_user.egg-info/
+-rw-r-----   0 agilbert   (501) staff       (20)     4472 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      316 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       44 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      153 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       12 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2023-07-27 12:15:53.320219 qcloud_user-1.0.4/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      793 2023-07-27 12:15:22.000000 qcloud_user-1.0.4/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:15:53.318510 qcloud_user-1.0.4/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:15:53.319890 qcloud_user-1.0.4/src/qcloud_user/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-27 02:16:27.000000 qcloud_user-1.0.4/src/qcloud_user/__init__.py
+-rwxr-x---   0 agilbert   (501) staff       (20)    22893 2023-07-27 11:01:31.000000 qcloud_user-1.0.4/src/qcloud_user/qcloud_user.py
```

### Comparing `qcloud_user-1.0.3/LICENSE.txt` & `qcloud_user-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_user-1.0.3/PKG-INFO` & `qcloud_user-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud_user
-Version: 1.0.3
+Version: 1.0.4
 Summary: Q-Cloud CLI for users
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
```

### Comparing `qcloud_user-1.0.3/README.md` & `qcloud_user-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qcloud_user-1.0.3/pyproject.toml` & `qcloud_user-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_user"
-version = "1.0.3"
+version = "1.0.4"
 description = "Q-Cloud CLI for users" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
@@ -12,15 +12,15 @@
 
 dependencies = [ 
    "boto3==1.21.33",
    "botocore==1.24.33",
    "demjson3==3.0.6",
    "paramiko==3.1.0",
    "pick>=2.2.0",
-   "PyYAML>=5.3",
+   "PyYAML==5.3",
    "python-jose>=3.3.0",
    "pyopenssl>=22.1.0",
    "jose>=1.0",
    "Requests==2.31.0",
 ]
 
 [project.urls]
```

### Comparing `qcloud_user-1.0.3/qcloud_user.egg-info/PKG-INFO` & `qcloud_user-1.0.4/qcloud_user.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud-user
-Version: 1.0.3
+Version: 1.0.4
 Summary: Q-Cloud CLI for users
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
```

### Comparing `qcloud_user-1.0.3/setup.py` & `qcloud_user-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name="qcloud_user",
     python_requires='>=3.7',
-    version="1.0.3",
+    version="1.0.4",
     url="https://q-chem.com",
     author="Andrew Gilbert",
     author_email="suppor@q-chem.com",
     description="CLI for interacting with Q-Cloud clusters",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=['qcloud_user'],
@@ -15,15 +15,15 @@
 
     install_requires=[
         "boto3==1.21.33",
         "botocore==1.24.33",
         "demjson3==3.0.6",
         "paramiko==3.1.0",
         "pick>=2.2.0",
-        "PyYAML>=5.3",
+        "PyYAML==5.3",
         "python-jose>=3.3.0",
         "pyopenssl>=22.1.0",
         "jose>=1.0",
         "Requests==2.31.0",
     ],
     scripts=['src/qcloud_user/qcloud_user.py'],
 )
```

### Comparing `qcloud_user-1.0.3/src/qcloud_user/qcloud_user.py` & `qcloud_user-1.0.4/src/qcloud_user/qcloud_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,32 +161,40 @@
         ChallengeName = 'NEW_PASSWORD_REQUIRED',
         ClientId = client_id,
         ChallengeResponses = {
             'USERNAME': username,
             'NEW_PASSWORD': password
          },
          Session = session_key,
-    );
+    )
 
     token = update_tokens(config, response)
     return token
 
 
 
 def forgot_password(session, config):
     cognito   = session.client('cognito-idp')
     username  = config.get("USER", "username")
     client_id = config.get("AWS", "appclientid")
 
-    code = input("Reset code {}: ".format(username))
+    response = cognito.forgot_password(
+        ClientId = client_id,
+        Username = username,
+    )
+
+    dest = response['CodeDeliveryDetails']['Destination']
+    print("A password reset code has been sent to {}".format(dest))
+
+    code = input("Enter code: ".format(username))
 
     password = None
     while (password == None):
-        pw1 = getpass.getpass("Enter new password: ")
-        pw2 = getpass.getpass("Confirm password: ")
+        pw1 = getpass.getpass("Enter new password for {}: ".format(username))
+        pw2 = getpass.getpass("Confirm password for {}: ".format(username))
         if (pw1 == pw2):
            password = pw1
         else:
            print("Passwords do not match")
  
     response = cognito.confirm_forgot_password(
         ClientId = client_id,
@@ -377,18 +385,17 @@
            body = json.dumps({ "input_file": inp })
 
         response = requests.post(url, headers=headers, data=body)
         if "Submitted job id" in response.text: 
            job_id   = response.text.replace("Submitted job id ","")
            job_name = pathlib.Path(filename).stem
            db.set_job(job_id, job_name)
-           #print("{}:  {}".format(response.text, job_name))
            checklist("{}: ".format(response.text), job_name, True)
         else:
-           print("[x] Problem submitting job: {}".format(repsonse))
+           print("[x] Problem submitting job: {}".format(response.text))
 
 
 
 def tail(token, job_ids, config, db):
     if not job_ids: return ""
     headers = {'Authorization': token}
     job_id = ",".join(job_ids)
@@ -649,21 +656,22 @@
     try:
         parser = MyParser();
 
         parser.add_argument("--configure", dest="config", action='store_true',
             help="configure qcloud settings")
 
         parser.add_argument("--pwreset", dest="pwreset", action='store_true',
-            help="password reset using a code")
+            help="request password reset code")
 
         parser.add_argument("--submit", dest="submit", action='store_true',
             help="submit job(s)")
 
         parser.add_argument("--ncpu", dest="ncpu", default = 1,
             help="specify the number of openmp threads to use.")
+
         parser.add_argument("--ncpus", dest="ncpu", default = 1,
             help="specify the number of openmp threads to use.")
 
         parser.add_argument("--cancel", dest="cancel", action='store_true',
             help="cancel queued or running job(s)")
 
         parser.add_argument("--info", dest="info", action='store_true',
```

