# Comparing `tmp/qcloud_setup-1.0.3.tar.gz` & `tmp/qcloud_setup-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_setup-1.0.3.tar", last modified: Mon Jul 17 02:55:23 2023, max compression
+gzip compressed data, was "qcloud_setup-1.0.4.tar", last modified: Thu Jul 27 12:14:08 2023, max compression
```

## Comparing `qcloud_setup-1.0.3.tar` & `qcloud_setup-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-17 02:55:23.091042 qcloud_setup-1.0.3/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.3/LICENSE.txt
--rw-r-----   0 agilbert   (501) staff       (20)    16573 2023-07-17 02:55:23.090812 qcloud_setup-1.0.3/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)    15546 2023-07-17 02:45:41.000000 qcloud_setup-1.0.3/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      747 2023-07-17 02:52:37.000000 qcloud_setup-1.0.3/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-17 02:55:23.088929 qcloud_setup-1.0.3/qcloud_setup.egg-info/
--rw-r-----   0 agilbert   (501) staff       (20)    16573 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      422 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       51 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      151 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       13 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2023-07-17 02:55:23.091089 qcloud_setup-1.0.3/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      914 2023-07-17 02:52:44.000000 qcloud_setup-1.0.3/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-17 02:55:23.087565 qcloud_setup-1.0.3/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-17 02:55:23.090563 qcloud_setup-1.0.3/src/qcloud_setup/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.3/src/qcloud_setup/__init__.py
--rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.3/src/qcloud_setup/api-gateway.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.3/src/qcloud_setup/cognito.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     5729 2023-07-17 02:00:33.000000 qcloud_setup-1.0.3/src/qcloud_setup/iam-policy.yaml
--rwxr-x---   0 agilbert   (501) staff       (20)    56143 2023-07-17 02:42:47.000000 qcloud_setup-1.0.3/src/qcloud_setup/qcloud_admin.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:14:08.692882 qcloud_setup-1.0.4/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.4/LICENSE.txt
+-rw-r-----   0 agilbert   (501) staff       (20)    16593 2023-07-27 12:14:08.692666 qcloud_setup-1.0.4/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)    15566 2023-07-17 03:57:00.000000 qcloud_setup-1.0.4/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      747 2023-07-27 12:13:37.000000 qcloud_setup-1.0.4/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:14:08.690435 qcloud_setup-1.0.4/qcloud_setup.egg-info/
+-rw-r-----   0 agilbert   (501) staff       (20)    16593 2023-07-27 12:14:08.000000 qcloud_setup-1.0.4/qcloud_setup.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      422 2023-07-27 12:14:08.000000 qcloud_setup-1.0.4/qcloud_setup.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2023-07-27 12:14:08.000000 qcloud_setup-1.0.4/qcloud_setup.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       51 2023-07-27 12:14:08.000000 qcloud_setup-1.0.4/qcloud_setup.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      151 2023-07-27 12:14:08.000000 qcloud_setup-1.0.4/qcloud_setup.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       13 2023-07-27 12:14:08.000000 qcloud_setup-1.0.4/qcloud_setup.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2023-07-27 12:14:08.692931 qcloud_setup-1.0.4/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      914 2023-07-27 12:14:02.000000 qcloud_setup-1.0.4/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:14:08.689179 qcloud_setup-1.0.4/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:14:08.691948 qcloud_setup-1.0.4/src/qcloud_setup/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.4/src/qcloud_setup/__init__.py
+-rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.4/src/qcloud_setup/api-gateway.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.4/src/qcloud_setup/cognito.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     5829 2023-07-25 11:18:10.000000 qcloud_setup-1.0.4/src/qcloud_setup/iam-policy.yaml
+-rwxr-x---   0 agilbert   (501) staff       (20)    56432 2023-07-27 10:36:11.000000 qcloud_setup-1.0.4/src/qcloud_setup/qcloud_admin.py
```

### Comparing `qcloud_setup-1.0.3/LICENSE.txt` & `qcloud_setup-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.3/PKG-INFO` & `qcloud_setup-1.0.4/qcloud_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qcloud_setup
-Version: 1.0.3
+Name: qcloud-setup
+Version: 1.0.4
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -308,17 +308,17 @@
 validated administrator email.
 
 The cluster administrator will need to provide the server details to each 
 user which can be obtained by running the command:
 ```
 qcloud_setup --userinfo
 AwsRegion                        us-east-1
-CognitoUserPoolId                us-east-1_KbkatQIpW
-CognitoAppClientId               2mgcn0o6fk7kboq7jnqs6bd6ee
-ApiGatewayId                     fkkfolduo4
+CognitoUserPoolId                us-east-1_KbkdtpKpW
+CognitoAppClientId               2mgcn0o8fkakboq7jnqs6bd6ee
+ApiGatewayId                     fkkxolpuo4
 ```
 Cluster users will need to install and configure the command line interface (CLI):
 ```
 python3 -m pip install qcloud_user
 ```
 this will install the qcloud command into their python environment and this can be configured
 by running the following command and entering the appropriate values:
@@ -334,15 +334,16 @@
 
 
 
 ## Suspending a Cluster
 
 It is possible to shut down the cluster head node and restart it at a later
 time in order to minimise the running costs.  If you plan to restart the
-cluster, make sure you keep a copy of the configuration file and activation key.
+cluster, make sure to keep copies of the configuration file, ssh key (.pem
+file) and activation key.
 
 Use the `--suspend` option to delete only the cluster stack.  You will be prompted
 if you want to delete the stack, type 'y' to confirm.
 
 ```
 qcloud_setup --suspend
 Delete stack qcloud-cluster? [y/N] y
```

### Comparing `qcloud_setup-1.0.3/README.md` & `qcloud_setup-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -283,17 +283,17 @@
 validated administrator email.
 
 The cluster administrator will need to provide the server details to each 
 user which can be obtained by running the command:
 ```
 qcloud_setup --userinfo
 AwsRegion                        us-east-1
-CognitoUserPoolId                us-east-1_KbkatQIpW
-CognitoAppClientId               2mgcn0o6fk7kboq7jnqs6bd6ee
-ApiGatewayId                     fkkfolduo4
+CognitoUserPoolId                us-east-1_KbkdtpKpW
+CognitoAppClientId               2mgcn0o8fkakboq7jnqs6bd6ee
+ApiGatewayId                     fkkxolpuo4
 ```
 Cluster users will need to install and configure the command line interface (CLI):
 ```
 python3 -m pip install qcloud_user
 ```
 this will install the qcloud command into their python environment and this can be configured
 by running the following command and entering the appropriate values:
@@ -309,15 +309,16 @@
 
 
 
 ## Suspending a Cluster
 
 It is possible to shut down the cluster head node and restart it at a later
 time in order to minimise the running costs.  If you plan to restart the
-cluster, make sure you keep a copy of the configuration file and activation key.
+cluster, make sure to keep copies of the configuration file, ssh key (.pem
+file) and activation key.
 
 Use the `--suspend` option to delete only the cluster stack.  You will be prompted
 if you want to delete the stack, type 'y' to confirm.
 
 ```
 qcloud_setup --suspend
 Delete stack qcloud-cluster? [y/N] y
```

### Comparing `qcloud_setup-1.0.3/pyproject.toml` & `qcloud_setup-1.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_setup"
-version = "1.0.3"
+version = "1.0.4"
 description = "Q-Cloud setup utility for cluster administrators" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
@@ -12,18 +12,18 @@
 
 dependencies = [ 
    "boto3==1.21.33",
    "botocore==1.24.33",
    "demjson3==3.0.6",
    "paramiko==3.1.0",
    "pick>=2.2.0",
-   "PyYAML>=5.3",
+   "PyYAML==5.3",
    "pyopenssl>=22.1.0",
    "Requests>=2.27.1",
-   "aws-parallelcluster>=3.1.5"
+   "aws-parallelcluster==3.1.5"
 ]
 
 [project.urls]
 "Homepage" = "https://q-chem.com"
 
 [project.scripts]
 qcloud_setup = "qcloud_admin:main"
```

### Comparing `qcloud_setup-1.0.3/qcloud_setup.egg-info/PKG-INFO` & `qcloud_setup-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qcloud-setup
-Version: 1.0.3
+Name: qcloud_setup
+Version: 1.0.4
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -308,17 +308,17 @@
 validated administrator email.
 
 The cluster administrator will need to provide the server details to each 
 user which can be obtained by running the command:
 ```
 qcloud_setup --userinfo
 AwsRegion                        us-east-1
-CognitoUserPoolId                us-east-1_KbkatQIpW
-CognitoAppClientId               2mgcn0o6fk7kboq7jnqs6bd6ee
-ApiGatewayId                     fkkfolduo4
+CognitoUserPoolId                us-east-1_KbkdtpKpW
+CognitoAppClientId               2mgcn0o8fkakboq7jnqs6bd6ee
+ApiGatewayId                     fkkxolpuo4
 ```
 Cluster users will need to install and configure the command line interface (CLI):
 ```
 python3 -m pip install qcloud_user
 ```
 this will install the qcloud command into their python environment and this can be configured
 by running the following command and entering the appropriate values:
@@ -334,15 +334,16 @@
 
 
 
 ## Suspending a Cluster
 
 It is possible to shut down the cluster head node and restart it at a later
 time in order to minimise the running costs.  If you plan to restart the
-cluster, make sure you keep a copy of the configuration file and activation key.
+cluster, make sure to keep copies of the configuration file, ssh key (.pem
+file) and activation key.
 
 Use the `--suspend` option to delete only the cluster stack.  You will be prompted
 if you want to delete the stack, type 'y' to confirm.
 
 ```
 qcloud_setup --suspend
 Delete stack qcloud-cluster? [y/N] y
```

### Comparing `qcloud_setup-1.0.3/setup.py` & `qcloud_setup-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="qcloud_setup",
     python_requires='>=3.7',
-    version="1.0.3",
+    version="1.0.4",
     url="https://q-chem.com",
     author="Andrew Gilbert",
     author_email="support@q-chem.com",
     description="Utility for setting up Q-Cloud administrators",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(where="src"), 
@@ -17,14 +17,14 @@
 
     install_requires=[
         "boto3==1.21.33",
         "botocore==1.24.33",
         "demjson3==3.0.6",
         "paramiko==3.1.0",
         "pick>=2.2.0",
-        "PyYAML>=5.3",
+        "PyYAML==5.3",
         "pyopenssl>=22.1.0",
         "Requests>=2.27.0",
-        "aws-parallelcluster>=3.1.5"
+        "aws-parallelcluster==3.1.5"
     ],
     scripts=['src/qcloud_setup/qcloud_admin.py'],
 )
```

### Comparing `qcloud_setup-1.0.3/src/qcloud_setup/api-gateway.yaml` & `qcloud_setup-1.0.4/src/qcloud_setup/api-gateway.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.3/src/qcloud_setup/cognito.yaml` & `qcloud_setup-1.0.4/src/qcloud_setup/cognito.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.3/src/qcloud_setup/iam-policy.yaml` & `qcloud_setup-1.0.4/src/qcloud_setup/iam-policy.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -148,14 +148,17 @@
       - acm:ListCertificates
       - apigateway:*
       - cloudformation:*
       - cloudwatch:PutDashboard
       - cloudwatch:ListDashboards
       - cloudwatch:DeleteDashboards
       - cloudwatch:GetDashboard
+      - cloudwatch:PutMetricAlarm
+      - cloudwatch:DeleteAlarms
+      - cloudwatch:DescribeAlarms
       - cognito-identity:*
       - cognito-sync:*
       - cognito-idp:*
       - iam:ListSAMLProviders
       - iam:ListOpenIDConnectProviders
       - iam:GetSAMLProvider
       - iam:GetRole
```

### Comparing `qcloud_setup-1.0.3/src/qcloud_setup/qcloud_admin.py` & `qcloud_setup-1.0.4/src/qcloud_setup/qcloud_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1074,14 +1074,15 @@
 
 
 def gen_iam():
     template = load_template("iam-policy")
     fname = "iam-policy.yaml"
     with open(fname, "w") as file:
          file.write(template)
+    print("IAM policy written to {}".format(fname))
 
 
 def launch_cognito(session, stack_name, admin_email):
     if stack_exists(session,stack_name):
        print_stack_status(session,stack_name)
        return
 
@@ -1234,15 +1235,15 @@
     with open(fname) as file:
          text = file.read()
 
     ip = re.search("ElasticIp:\s*(.+)", text)
     if ip:
        checklist("Retrieving elastic IP address", ip.group(1), True)
     else:
-        print("[x] Failed to determine elastic IP, check config file")
+       print("[x] Failed to determine elastic IP, check config file")
 
 
 def update_lambda(session, cluster_stack, api_stack):
     instance_id = get_resource_id(session, cluster_stack, 'HeadNode')
     checklist("Updating config file with instance ID")
     lambda_qcloud = get_resource_id(session, api_stack, 'LambdaFunctionQCloud')
     lambda_s3submit = get_resource_id(session, api_stack, 'LambdaFunctionS3Submit')
@@ -1356,14 +1357,18 @@
                 UserPoolId = pool_id,
                 Username = username,
                 UserAttributes=[
                     {
                         'Name': 'email',
                         'Value': email
                     },
+                    {
+                        'Name':  'email_verified',
+                        'Value': 'true' 
+                    },
                 ],
                 ForceAliasCreation = False,
                 DesiredDeliveryMediums = [ 'EMAIL' ]
             )
             checklist("Added user:", username, True)
 
         except botocore.exceptions.ClientError as e:
@@ -1622,23 +1627,23 @@
 
         parser.add_argument("--list", dest="list", action='store_true',
             help="list all cloudformation stacks")
 
         parser.add_argument("--adduser", dest="adduser",
             help="add user to the cognito user pool")
 
+        parser.add_argument("--addusers", dest="users_file", 
+            help="add multiple users to the cognito user pool")
+
         parser.add_argument("--listusers", dest="listusers", action='store_true',
             help="list all users in the cognito user pool")
 
         parser.add_argument("--email", dest="email",
             help="specify the user's email address")
 
-        parser.add_argument("--addusers", dest="users_file", 
-            help="add multiple users to the cognito user pool")
-
         parser.add_argument("--suspend", dest="suspend", action='store_true',
             help="suspend the compute stack")
 
         parser.add_argument("--delete", dest="delete", action='store_true',
             help="delete stack(s)")
 
         parser.add_argument("--debug", dest="debug", action='store_true',
@@ -1682,14 +1687,16 @@
         if args.config:
             configure_cluster(session, name, interactive)
             if args.launch:
                launch(session, name, args.nocognito, args.email)
 
         elif args.launch:
             launch(session, name, args.nocognito, args.email)
+            if args.license_key:
+               install_license_key(session, name, args.license_key)
 
         elif args.status:
             print_all_stack_status(session, name)
 
         elif args.delete:
             if extra_args:
                delete_stacks(session, extra_args)
```

