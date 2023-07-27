# Comparing `tmp/dodevops-0.1.8.tar.gz` & `tmp/dodevops-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodevops-0.1.8.tar", max compression
+gzip compressed data, was "dodevops-0.1.9.tar", max compression
```

## Comparing `dodevops-0.1.8.tar` & `dodevops-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4751 2023-06-29 17:27:54.783038 dodevops-0.1.8/README.md
--rw-r--r--   0        0        0    78456 2023-07-26 04:10:47.084330 dodevops-0.1.8/dodevops.py
--rw-r--r--   0        0        0      646 2023-07-26 05:53:25.522647 dodevops-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5798 1970-01-01 00:00:00.000000 dodevops-0.1.8/setup.py
--rw-r--r--   0        0        0     5714 1970-01-01 00:00:00.000000 dodevops-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     5516 2023-07-27 03:08:28.878990 dodevops-0.1.9/README.md
+-rw-r--r--   0        0        0    82475 2023-07-27 02:29:37.802127 dodevops-0.1.9/dodevops.py
+-rw-r--r--   0        0        0      670 2023-07-27 02:01:45.613813 dodevops-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6616 1970-01-01 00:00:00.000000 dodevops-0.1.9/setup.py
+-rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dodevops-0.1.9/PKG-INFO
```

### Comparing `dodevops-0.1.8/README.md` & `dodevops-0.1.9/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,72 @@
-# TLDR
+# **DoDevOps**
 
-This is a tool to take github repos for Django projects and put them on DigitalOcean App Spaces with managed database and DO Spaces S3 storage.
+DoDevOps is a tool for creating and managing Django apps on DigitalOcean's App Platform. 
+It accesses DigitalOcean through the API, so it requires a DigitalOcean API token,
+and it requires a DigitalOcean Spaces key for storing media uploads.
+Additionally, you must authorize DigitalOcean to pull your GitHub repos.
 
-You will need:
+## Prerequisites:
 
-1) Poetry installed locally to run this tool
+1) Python 3.9 on Linux or Mac
 2) DigitalOcean account https://www.digitalocean.com/?refcode=9ef6f738fd8a
 3) DigitalOcean API token: https://cloud.digitalocean.com/account/api/tokens
 4) DigitalOcean S3 keys: https://cloud.digitalocean.com/account/api/spaces
 5) Authorize DigitalOcean to pull your github repos: https://cloud.digitalocean.com/apps/github/install
-6) A DigitalOcean S3 bucket: https://cloud.digitalocean.com/spaces/new
-7) A DigitalOcean PostgreSQL database cluster: https://cloud.digitalocean.com/databases
-8) A database and user and connection pool configured on the database cluster
-9) Manually add the app as a trusted source on the database
 
-There are plans to integrate items 6-9 into this tool, we just haven't gotten that far yet.
+# Installation
+
+This tool can be installed with pip. 
+If installed in a Django project, it will try to detect some settings from the project such as repo and branch,
+as well as enable migration of db.json files and media uploads.
+
+```shell
+pip install dodevops
+```
 
 To run the tool:
 
 ```shell
-poetry run start
+dodevops
 ```
 
-# What is this
+# Quickstart
 
-This is essentially an experiment/prototype that got a little too big and had some potential. So it's being turned into a project.
+## Migrate an existing Django project to DigitalOcean App Platform
 
-proto.py is the original prototype.
+1) Create clean temporary directory for your project
+2) Create a virtual environment in the directory (python 3.9 or higher) 
+   ```mkvirtualenv tempenv```
+3) git clone your project into the directory
+4) install requirements for your project
+   ```pip install -r requirements.txt```
+5) If you are migrating media uploads, copy your media folder into your project directory
+6) If you are migrating db.json files, copy or generate your db.json files into your project directory
+7) Run any project specific migration tasks
+8) Make sure pip is up to date
+   ```pip install --upgrade pip```
+9) Install dodevops
+   ```pip install dodevops```
+10) Export environment variables
+    ```
+    export DIGITALOCEAN_API_TOKEN=dop_v1_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    export AWS_ACCESS_KEY_ID=xxxxxxxxxxxxxxxxxxx
+    export AWS_SECRET_ACCESS_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    ```
+11) Run dodevops
+    ```dodevops```
 
-This project uses inquirer to get user input. As far as I know it only works on linux and mac. 
-When debugging in pycharm, you may need to set the run/debug settings to use the terminal emulation.
-You can find a link with more info here: https://intellij-support.jetbrains.com/hc/en-us/community/posts/360003383619-Pycharm-2019-termios-error-25-Inappropriate-ioctl-for-device-?page=1#community_comment_6589796593042 and here https://github.com/magmax/python-readchar/issues/11
 
 # Details
 
 ## Generating DO API token
 
 In order for this app to work it needs a valid DigitalOcean Personal Access Token. 
 The token is not required after this is run, so it is okay to recyle the token when finished. 
-The token can either be stored in a .env file, or it can be pasted into the app at run time. 
+The token can either be stored in a .env file or env variable, or it can be pasted into the app at run time. 
 
 ### To generating a new token
 
 Go here: https://cloud.digitalocean.com/account/api/tokens
 
 Pick whatever name you want for the token, it doesn't matter. 
 Pick whatever token expiration you want depending on your personal paranoia level. 
@@ -50,62 +74,62 @@
 
 Once the token is generated copy it and paste it somewhere safe like a password manager such as 1password. 
 The token won't be displayed again, so if you don't get it saved somewhere safe you'll have to regenerate it.
 
 Protect your token well. 
 Anyone with access to your token has the ability to create and destroy things and incur you costs, so be careful with it. 
 This is opensource so that you can read the code if you want and verify how the token is used. 
-Storing the token in the .env file is convenient but it is not the most secure, so if you feel paranoid don't do that or delete the token after. 
+Storing the token in the .env file is convenient, but it is not the most secure, so if you feel paranoid don't do that. 
 
 If you want more info about DO tokens, see here: https://docs.digitalocean.com/reference/api/create-personal-access-token/
 
 ## Generating DO Spaces Key
 
 A DO Spaces key is required for storing a media upload folder, as app platform doesn't have storage. 
 
-### To generating an app spaces key 
+### To generate an app spaces key 
 
 Go here: https://cloud.digitalocean.com/account/api/spaces 
 
 You can use whatever name you want for the key, it doesn't matter. 
 It will display two values, a key ID and a longer access key, save both somewhere safe like a password manager. 
 It won't display the access key again, so if you don't save it you'll have to regenerate it. 
 
 You can put the values in an .env file, or enter it at runtime.
 
 Protect the token well.
 
 To learn more about DO spaces keys, go here: https://docs.digitalocean.com/products/spaces/how-to/manage-access/#access-keys
 
-## Create a DO Spaces S3 bucket
-
-You must create an S3 bucket on DO's web interface:
-
-https://cloud.digitalocean.com/spaces/new
-
 ## Filling out .env file
 
-A .env file isn't required, but if you store values in it then it will save effort. 
+A .env file isn't required, but if you store values in it then it will save effort.
 But if you feel storing values in the .env file isn't secure enough for your personal paranoia levels you can instead enter things at runtime.
 
 The format of the env file is:
 
 ```
 DIGITALOCEAN_TOKEN=dop_v1_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 AWS_ACCESS_KEY_ID=DOxxxxxxxxxxxxxxxxxxx
 AWS_SECRET_ACCESS_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 # AWS_REGION=ams3
 # APP_NAME=example-rest-app
 # COMPONENT_NAME=example-rest
 # APP_PREFIX=example
-GH_REPO=xusernamex/xrepox
+# GH_REPO=xusernamex/xrepox
 # GH_BRANCH=main
 # DJANGO_ROOT_MODULE=example
 # DJANGO_USER_MODULE=core
 # SECRET_KEY_ENV_KEY=SECRET_KEY
 # SECRET_KEY=change_me
 # ALLOWED_HOSTS_ENV_KEY=ALLOWED_HOSTS
 # DEBUG=1
 # DOMAIN=rest.example.com
 # PARENT_DOMAIN=example.com
 # OIDC="\"-----BEGIN RSA PRIVATE KEY-----\\n_xxx_\\n-----END RSA PRIVATE KEY-----\\n\""
 ```
+
+## Linux and Mac
+
+This project uses inquirer to get user input. As far as I know it only works on linux and mac. 
+When debugging in pycharm, you may need to set the run/debug settings to use the terminal emulation.
+You can find a link with more info here: https://intellij-support.jetbrains.com/hc/en-us/community/posts/360003383619-Pycharm-2019-termios-error-25-Inappropriate-ioctl-for-device-?page=1#community_comment_6589796593042 and here https://github.com/magmax/python-readchar/issues/11
```

### Comparing `dodevops-0.1.8/dodevops.py` & `dodevops-0.1.9/dodevops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import configparser
 import json
 import logging
 import secrets
 import time
 
 import psycopg2
 from psycopg2 import sql
@@ -14,19 +15,26 @@
 import getpass
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.backends import default_backend as crypto_default_backend
 from cryptography.hazmat.primitives import serialization as crypto_serialization
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
-ch = logging.StreamHandler()
-ch.setLevel(logging.DEBUG)
 formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-ch.setFormatter(formatter)
-logger.addHandler(ch)
+
+file_handler = logging.FileHandler('debug.log')
+file_handler.setLevel(logging.DEBUG)
+file_handler.setFormatter(formatter)
+
+console_handler = logging.StreamHandler()
+console_handler.setLevel(logging.WARNING)
+console_handler.setFormatter(formatter)
+
+logger.addHandler(file_handler)
+logger.addHandler(console_handler)
 
 load_dotenv()
 
 
 def _get_env_var_from_list_or_keep_original(env_var_list, original_value=None,
                                             override=True):
     if original_value and not override:
@@ -127,15 +135,15 @@
             "scope": "BUILD_TIME"
         }
         env_list.append(temp_obj)
 
     return env_list
 
 
-def start_app_spec_file(appname, region="ams"):
+def start_app_spec_file(appname, region="sfo"):
     app_spec = {
         "name": appname,
         "services": [],
         "databases": [],
         "domains": [],
         "region": region,
         "alerts": [],
@@ -236,15 +244,16 @@
         "http_port": port
     }
     app_spec["services"].append(services_json)
     return app_spec
 
 
 def populate_app_spec_jobs(app_spec, gh_repo, gh_branch, env_list,
-                           django_user_module, deploy_on_push=True):
+                           django_user_module, import_json, deploy_on_push=True, bonuscommand1=None,
+                           bonuscommand2=None):
     lines = []
 
     python_lines = ("from custom_storages import MediaStorage;"
                     "FileStorage = MediaStorage;"
                     "fs = FileStorage();"
                     "test = fs.open('db.json');"
                     "temp = test.read();"
@@ -256,20 +265,26 @@
                     "f.close()")
 
     lines.append("python manage.py makemigrations\n")
     lines.append("python manage.py makemigrations {}\n".format(
         django_user_module))
     lines.append("python manage.py migrate\n")
 
+    if bonuscommand1:
+        lines.append(bonuscommand1)
+    if bonuscommand2:
+        lines.append(bonuscommand2)
+
     # get json file from somewhere to here
 
     lines.append("python manage.py shell -c \"{}\"\n".format(python_lines))
 
-    # Load json file
-    lines.append("python manage.py loaddata \"db.json\"\n")
+    if import_json:
+        # Load json file
+        lines.append("python manage.py loaddata \"db.json\"\n")
 
     run_command = "".join(lines)
 
     services_json = {
         "name": "migrate",
         "kind": "PRE_DEPLOY",
         "github": {
@@ -282,15 +297,15 @@
         "envs": env_list,
     }
     app_spec["jobs"] = []
     app_spec["jobs"].append(services_json)
     return app_spec
 
 
-def build_app_spec_file(env_obj, job_lines=None):
+def build_app_spec_file(env_obj, import_json, migrate_task):
     env_list = build_env_list(env_obj["envvars"],
                               secret_key_env_key=env_obj["secret_key_env_key"],
                               allowed_hosts_env_key=env_obj["allowed_hosts_env_key"])
     region = env_obj["region"]
     appname = env_obj["appname"]
     component_name = env_obj["component_name"]
     domain = env_obj["domain"]
@@ -316,23 +331,22 @@
                                            database_name=database_name,
                                            database_user=database_user)
     app_spec = populate_app_spec_services(app_spec, component_name=component_name,
                                           gh_repo=gh_repo,
                                           gh_branch=gh_branch,
                                           django_user_module=django_user_module,
                                           env_list=env_list,
-                                          django_root_module=django_root_module,
-                                          bonuscommand1=bonuscommand1,
-                                          bonuscommand2=bonuscommand2)
-    if job_lines:
+                                          django_root_module=django_root_module)
+    if import_json or migrate_task:
         app_spec = populate_app_spec_jobs(app_spec,
                                           gh_repo=gh_repo,
                                           gh_branch=gh_branch,
                                           django_user_module=django_user_module,
-                                          env_list=env_list)
+                                          env_list=env_list, import_json=import_json, bonuscommand1=bonuscommand1,
+                                          bonuscommand2=bonuscommand2)
         # populate_app_spec_jobs(app_spec, gh_repo, gh_branch, env_list,
         #                            django_user_module, deploy_on_push=True)
     return app_spec
 
 
 def get_app(client, app_name="app"):
     app_resp = client.apps.list()
@@ -398,15 +412,15 @@
     else:
         appname = inquirer.text("What is the name of your app?", default=appname)
     return appname
 
 
 def get_region(client, region_slug=None):
     if region_slug is None:
-        region_slug = "ams3"
+        region_slug = "sfo3"
     print("Getting regions")
     reg_resp = client.regions.list()
     regioncount = len(reg_resp["regions"])
     if regioncount > 0:
         options = []
         for r in reg_resp["regions"]:
             if r["available"] and "storage" in r["features"]:
@@ -421,16 +435,16 @@
                           ),
         ]
         answers = inquirer.prompt(questions)
         pickedoption = answers['region']
         logger.debug("Using region {}".format(pickedoption))
         return pickedoption
     else:
-        print("No regions found, defaulting to ams3")
-        return "ams3"
+        print("No regions found, defaulting to sfo3")
+        return "sfo3"
 
 
 def get_spaces(s3client, appname):
     pickedoption = None
     while not pickedoption:
         space_resp = s3client.list_buckets()
         spacecount = len(space_resp['Buckets'])
@@ -944,49 +958,106 @@
     if not allowed_hosts_env_key:
         allowed_hosts_env_key = inquirer.text(
             "What environment variable holds your allowed hosts?",
             default="ALLOWED_HOSTS")
     return allowed_hosts_env_key
 
 
+def find_git_config_file_and_repo(base_path):
+
+    git_config_files = []
+    for root, dirs, files in os.walk(base_path):
+        for d in dirs:
+            if d == ".git":
+                git_config_files.append(os.path.join(root, d, "config"))
+
+    if len(git_config_files) == 0:
+        return None
+    else:
+        config = configparser.ConfigParser()
+        config.read(git_config_files[0])
+
+        try:
+            remote_url = config.get('remote "origin"', 'url')
+            relative_path = remote_url.split("github.com/")[1]
+            relative_path = relative_path.split(".git")[0]
+            return git_config_files[0], remote_url, relative_path
+        except (configparser.NoSectionError, configparser.NoOptionError):
+            return None
+
+
+def get_active_branch_from_head(head_file_path):
+    try:
+        with open(head_file_path, 'r') as head_file:
+            ref = head_file.read().strip()
+            if ref.startswith("ref: refs/heads/"):
+                branch_name = ref.split("ref: refs/heads/")[1]
+                print("Found branch {}".format(branch_name))
+                return branch_name
+    except FileNotFoundError:
+        return None
+
+
 def get_gh_repo(existing_app=None, app_name=None, repo=None, branch=None):
     logger.debug("Getting github repo")
 
+    default_repo = None
+    default_branch = "main"
+
     if existing_app is not None and existing_app["spec"]["services"]:
         services = existing_app["spec"]["services"]
         for service in services:
             if service["name"] == app_name:
                 repo = repo or service["github"]["repo"]
                 branch = branch or service["github"]["branch"]
     if repo is None or branch is None:
-        repo = repo or inquirer.text("What is the github repo for your app?")
+        current_directory = os.getcwd()
+        config_path, git_repo, relative_path = find_git_config_file_and_repo(current_directory)
+        if relative_path:
+            default_repo = relative_path
+            print("GitHub repository found:")
+            print(config_path)
+
+            head_file = os.path.join(os.path.dirname(config_path), "HEAD")
+            if head_file:
+                default_branch = get_active_branch_from_head(head_file)
+
+        else:
+            print(
+                "No GitHub repositories found in the current directory or its subdirectories.")
+
+        repo = repo or inquirer.text("What is the github repo for your app?", default=default_repo)
         branch = branch or inquirer.text("What branch should we build from?",
-                                         default="main")
+                                         default=default_branch)
     return {"repo": repo, "branch": branch}
 
 
 def get_aws_access_key_id():
     if os.getenv("$AWS_ACCESS_KEY_ID"):
         return os.getenv("$AWS_ACCESS_KEY_ID")
     else:
         print("No AWS_ACCESS_KEY_ID found")
+        print("This tool uses DigitalOcean's s3 Spaces API to create and manage resources")
+        print("You can create a new access key here:")
         print("https://cloud.digitalocean.com/account/api/spaces")
-        promptentry = input(
-            "Please enter your AWS_ACCESS_KEY_ID and press enter to continue: ")
+        print("You can save effort when running this tool by setting the key id in the environment variable AWS_ACCESS_KEY_ID")
+        promptentry = input("Please enter your AWS_ACCESS_KEY_ID and press enter to continue: ")
         return promptentry
 
 
 def get_aws_secret_access_key():
     if os.getenv("$AWS_SECRET_ACCESS_KEY"):
         return os.getenv("$AWS_SECRET_ACCESS_KEY")
     else:
         print("No AWS_SECRET_ACCESS_KEY found")
+        print("This tool uses DigitalOcean's s3 Spaces API to create and manage resources")
+        print("You can create a new access key here:")
         print("https://cloud.digitalocean.com/account/api/spaces")
-        promptentry = inquirer.password(
-            message="Please enter your AWS_SECRET_ACCESS_KEY and press enter to continue: ")
+        print("You can save effort when running this tool by setting the key in the environment variable AWS_SECRET_ACCESS_KEY")
+        promptentry = inquirer.password(message="Please enter your AWS_SECRET_ACCESS_KEY and press enter to continue: ")
         return promptentry
 
 
 def check_cluster_status(cluster_id, client):
     # Get the current status of the cluster
     cluster = client.databases.get_cluster(cluster_id)
     print(cluster)
@@ -1263,14 +1334,20 @@
         logger.debug("Space {} exists".format(space_name))
         return True
     except client.exceptions.NoSuchBucket:
         logger.debug("Space {} does not exist yet".format(space_name))
         return False
 
 
+def get_secret_key_env_key_from_env(env_var_list):
+    for var_name in env_var_list:
+        if os.getenv(var_name):
+            return var_name
+
+
 class Helper:
     # DigitalOcean's connection info
     _DIGITALOCEAN_TOKEN = None
     _AWS_ACCESS_KEY_ID = None
     _AWS_SECRET_ACCESS_KEY = None
     _AWS_REGION = None
     _do_client = None
@@ -1305,15 +1382,18 @@
         self._AWS_SECRET_ACCESS_KEY = aws_secret_access_key
         self.load_env(override=True)
 
     @property
     def _digitalocean_token(self):
         while not self._DIGITALOCEAN_TOKEN:
             print("No DIGITALOCEAN_TOKEN found")
+            print("This tool uses DigitalOcean's API to create and manage resources")
+            print("You can create a token here: ")
             print("https://cloud.digitalocean.com/account/api/tokens")
+            print("You can save effort when running this tool by setting the token in the environment variable DIGITALOCEAN_API_TOKEN")
             self._DIGITALOCEAN_TOKEN = getpass.getpass("Enter your DigitalOcean token: ")
         return self._DIGITALOCEAN_TOKEN
 
     @property
     def do_client(self):
         while not self._do_client:
             self._do_client = Client(token=self._digitalocean_token)
@@ -1364,15 +1444,15 @@
         print(self.allowed_hosts_env_key)
         print(self.debug)
 
     def load_env(self, override=False):
 
         # DigitalOcean's connection info
         potential_var_names = ["$DIGITALOCEAN_TOKEN", "DIGITALOCEAN_TOKEN",
-                               "digitalocean_token"]
+                               "digitalocean_token", "DIGITALOCEAN_API_TOKEN"]
         self._DIGITALOCEAN_TOKEN = _get_env_var_from_list_or_keep_original(
             potential_var_names, self._DIGITALOCEAN_TOKEN, override)
 
         potential_var_names = ["$AWS_ACCESS_KEY_ID", "AWS_ACCESS_KEY_ID",
                                "aws_access_key_id"]
         self._AWS_ACCESS_KEY_ID = _get_env_var_from_list_or_keep_original(
             potential_var_names, self._AWS_ACCESS_KEY_ID, override)
@@ -1426,14 +1506,16 @@
         self.secret_key_env_key = _get_env_var_from_list_or_keep_original(
             potential_var_names, self.secret_key_env_key, override)
 
         potential_var_names = ["secret_key", "SECRET_KEY", "DJANGO_SECRET_KEY",
                                "django_secret_key"]
         self._secret_key = _get_env_var_from_list_or_keep_original(
             potential_var_names, self._secret_key, override)
+        if not self.secret_key_env_key:
+            self.secret_key_env_key = get_secret_key_env_key_from_env(potential_var_names)
 
         potential_var_names = ["allowed_hosts_env_key", "allowed_hosts", "ALLOWED_HOSTS",
                                "ALLOWED_HOSTS_ENV_KEY"]
         self.allowed_hosts_env_key = _get_env_var_from_list_or_keep_original(
             potential_var_names, self.allowed_hosts_env_key, override)
 
         potential_var_names = ["debug", "DEBUG"]
@@ -1465,14 +1547,20 @@
             json.dump(self._app_spec, f, indent=4)
 
     def load_app_spec_from_json_file(self, filename=None):
         with open("appspecs/" + filename, "r") as f:
             self._app_spec = json.load(f)
 
     def main_menu(self):
+        while not self._digitalocean_token:
+            print("No DIGITALOCEAN_TOKEN found")
+        if not self._AWS_ACCESS_KEY_ID:
+            self._AWS_ACCESS_KEY_ID = get_aws_access_key_id()
+        if not self._AWS_SECRET_ACCESS_KEY:
+            self._AWS_SECRET_ACCESS_KEY = get_aws_secret_access_key()
         while True:
             options = [
                 ("$$$ Create Full Stack Django App $$$", "create_full_stack_django_app"),
                 (" - Submenu Manage Apps", "submenu_manage_apps"),
                 (" - Submenu Manage Spaces", "submenu_manage_spaces"),
                 (" - Submenu Manage Databases", "submenu_manage_db"), ("Exit", "exit")]
 
@@ -1716,18 +1804,20 @@
         confirmed_app_name = get_app_name(appname=possible_appname)
 
         if not self._oidc or inquirer.confirm(
                 "Do you want to generate a new OIDC RSA key?", default=True):
             self._oidc = get_oidc_rsa_key()
         oidc_rsa_private_key = self._oidc
 
-        if not self.secret_key_env_key:
-            self.secret_key_env_key = inquirer.text(
-                message="What is the name of the environment variable that contains the Django secret key?",
-                default="SECRET_KEY")
+        default_secret_env_key = "SECRET_KEY"
+        if self.secret_key_env_key:
+            default_secret_env_key = self.secret_key_env_key
+        self.secret_key_env_key = inquirer.text(
+            message="What is the name of the environment variable that contains the Django secret key?",
+            default=default_secret_env_key)
         if not self._secret_key or inquirer.confirm(
                 "Do you want to generate a new Django secret key?", default=False):
             self._secret_key = secrets.token_urlsafe()
 
         if self._AWS_REGION:
             region_guess = self._AWS_REGION
         elif self._target_app and self._target_app["region"]["data_centers"][0]:
@@ -1768,25 +1858,31 @@
 
         mediafolder = get_media_folder(s3client=s3client, space=spacename,
                                        root_folder=rootfolder)
 
         aws_s3_endpoint_url = "https://{}.{}.digitaloceanspaces.com".format(spacename,
                                                                             confirmed_region)
 
-        job_lines = inquirer.confirm(
-            "Do you want to include a migration job to import db.json?", default=True)
-        if job_lines:
-            if not self._AWS_REGION:
-                self._AWS_REGION = get_region(client=self.do_client)
-            upload_db_json_to_s3_space(aws_access_key_id=self._AWS_ACCESS_KEY_ID,
-                                       aws_secret_access_key=self._AWS_SECRET_ACCESS_KEY,
-                                       aws_region=confirmed_region,
-                                       appname=confirmed_app_name, space_name=spacename, rootfolder=rootfolder, mediafolder=mediafolder)
+        migrate_task = inquirer.confirm(
+            "Do you want to include a migration job?", default=True)
+        import_json = False
+        if migrate_task:
             self._wait_for_migrate = True
 
+            import_json = inquirer.confirm("Do you want to import db.json?", default=True)
+
+            if import_json:
+
+                if not self._AWS_REGION:
+                    self._AWS_REGION = get_region(client=self.do_client)
+                upload_db_json_to_s3_space(aws_access_key_id=self._AWS_ACCESS_KEY_ID,
+                                           aws_secret_access_key=self._AWS_SECRET_ACCESS_KEY,
+                                           aws_region=confirmed_region,
+                                           appname=confirmed_app_name, space_name=spacename, rootfolder=rootfolder, mediafolder=mediafolder)
+
         aws_storage_bucket_name = rootfolder
         aws_location = rootfolder
         disable_collectstatic = "1"
 
         cluster_guess = self._target_app["spec"]["databases"][0]["cluster_name"] if \
             self._target_app and self._target_app["spec"][
                 "databases"] else "db-postgresql"
@@ -1849,15 +1945,15 @@
             "django_user_module": self.django_user_module,
             "django_root_module": django_root_module,
             "secret_key_env_key": self.secret_key_env_key,
             "allowed_hosts_env_key": self.allowed_hosts_env_key,
             "bonuscommand1": self.bonuscommand1,
             "bonuscommand2": self.bonuscommand2,
         }
-        self._app_spec = build_app_spec_file(env_obj=spec_vars, job_lines=job_lines)
+        self._app_spec = build_app_spec_file(env_obj=spec_vars, migrate_task=migrate_task, import_json=import_json)
 
     def create_full_stack_django_app(self):
         logger.debug("Starting building app spec from user input")
         self.build_app_spec_from_user_input()
 
         migrate_finished_too = create_app_from_app_spec(client=self.do_client,
                                                         potential_spec=self._app_spec,
```

### Comparing `dodevops-0.1.8/setup.py` & `dodevops-0.1.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 from setuptools import setup
 
 modules = \
 ['dodevops']
 install_requires = \
 ['boto3>=1.26.143,<2.0.0',
  'botocore>=1.29.145,<2.0.0',
+ 'configparser>=6.0.0,<7.0.0',
  'cryptography>=39.0.1,<40.0.0',
  'inquirer>=3.1.3,<4.0.0',
  'psycopg2-binary>=2.9.5,<3.0.0',
  'pydo>=0.1.4,<0.2.0',
  'python-dotenv>=0.21.1,<0.22.0']
 
 entry_points = \
 {'console_scripts': ['dodevops = dodevops:main']}
 
 setup_kwargs = {
     'name': 'dodevops',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Devops tool for deploying and managing resources on DigitalOcean',
-    'long_description': '# TLDR\n\nThis is a tool to take github repos for Django projects and put them on DigitalOcean App Spaces with managed database and DO Spaces S3 storage.\n\nYou will need:\n\n1) Poetry installed locally to run this tool\n2) DigitalOcean account https://www.digitalocean.com/?refcode=9ef6f738fd8a\n3) DigitalOcean API token: https://cloud.digitalocean.com/account/api/tokens\n4) DigitalOcean S3 keys: https://cloud.digitalocean.com/account/api/spaces\n5) Authorize DigitalOcean to pull your github repos: https://cloud.digitalocean.com/apps/github/install\n6) A DigitalOcean S3 bucket: https://cloud.digitalocean.com/spaces/new\n7) A DigitalOcean PostgreSQL database cluster: https://cloud.digitalocean.com/databases\n8) A database and user and connection pool configured on the database cluster\n9) Manually add the app as a trusted source on the database\n\nThere are plans to integrate items 6-9 into this tool, we just haven\'t gotten that far yet.\n\nTo run the tool:\n\n```shell\npoetry run start\n```\n\n# What is this\n\nThis is essentially an experiment/prototype that got a little too big and had some potential. So it\'s being turned into a project.\n\nproto.py is the original prototype.\n\nThis project uses inquirer to get user input. As far as I know it only works on linux and mac. \nWhen debugging in pycharm, you may need to set the run/debug settings to use the terminal emulation.\nYou can find a link with more info here: https://intellij-support.jetbrains.com/hc/en-us/community/posts/360003383619-Pycharm-2019-termios-error-25-Inappropriate-ioctl-for-device-?page=1#community_comment_6589796593042 and here https://github.com/magmax/python-readchar/issues/11\n\n# Details\n\n## Generating DO API token\n\nIn order for this app to work it needs a valid DigitalOcean Personal Access Token. \nThe token is not required after this is run, so it is okay to recyle the token when finished. \nThe token can either be stored in a .env file, or it can be pasted into the app at run time. \n\n### To generating a new token\n\nGo here: https://cloud.digitalocean.com/account/api/tokens\n\nPick whatever name you want for the token, it doesn\'t matter. \nPick whatever token expiration you want depending on your personal paranoia level. \nWrite permissions are required. \n\nOnce the token is generated copy it and paste it somewhere safe like a password manager such as 1password. \nThe token won\'t be displayed again, so if you don\'t get it saved somewhere safe you\'ll have to regenerate it.\n\nProtect your token well. \nAnyone with access to your token has the ability to create and destroy things and incur you costs, so be careful with it. \nThis is opensource so that you can read the code if you want and verify how the token is used. \nStoring the token in the .env file is convenient but it is not the most secure, so if you feel paranoid don\'t do that or delete the token after. \n\nIf you want more info about DO tokens, see here: https://docs.digitalocean.com/reference/api/create-personal-access-token/\n\n## Generating DO Spaces Key\n\nA DO Spaces key is required for storing a media upload folder, as app platform doesn\'t have storage. \n\n### To generating an app spaces key \n\nGo here: https://cloud.digitalocean.com/account/api/spaces \n\nYou can use whatever name you want for the key, it doesn\'t matter. \nIt will display two values, a key ID and a longer access key, save both somewhere safe like a password manager. \nIt won\'t display the access key again, so if you don\'t save it you\'ll have to regenerate it. \n\nYou can put the values in an .env file, or enter it at runtime.\n\nProtect the token well.\n\nTo learn more about DO spaces keys, go here: https://docs.digitalocean.com/products/spaces/how-to/manage-access/#access-keys\n\n## Create a DO Spaces S3 bucket\n\nYou must create an S3 bucket on DO\'s web interface:\n\nhttps://cloud.digitalocean.com/spaces/new\n\n## Filling out .env file\n\nA .env file isn\'t required, but if you store values in it then it will save effort. \nBut if you feel storing values in the .env file isn\'t secure enough for your personal paranoia levels you can instead enter things at runtime.\n\nThe format of the env file is:\n\n```\nDIGITALOCEAN_TOKEN=dop_v1_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\nAWS_ACCESS_KEY_ID=DOxxxxxxxxxxxxxxxxxxx\nAWS_SECRET_ACCESS_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\n# AWS_REGION=ams3\n# APP_NAME=example-rest-app\n# COMPONENT_NAME=example-rest\n# APP_PREFIX=example\nGH_REPO=xusernamex/xrepox\n# GH_BRANCH=main\n# DJANGO_ROOT_MODULE=example\n# DJANGO_USER_MODULE=core\n# SECRET_KEY_ENV_KEY=SECRET_KEY\n# SECRET_KEY=change_me\n# ALLOWED_HOSTS_ENV_KEY=ALLOWED_HOSTS\n# DEBUG=1\n# DOMAIN=rest.example.com\n# PARENT_DOMAIN=example.com\n# OIDC="\\"-----BEGIN RSA PRIVATE KEY-----\\\\n_xxx_\\\\n-----END RSA PRIVATE KEY-----\\\\n\\""\n```\n',
+    'long_description': '# **DoDevOps**\n\nDoDevOps is a tool for creating and managing Django apps on DigitalOcean\'s App Platform. \nIt accesses DigitalOcean through the API, so it requires a DigitalOcean API token,\nand it requires a DigitalOcean Spaces key for storing media uploads.\nAdditionally, you must authorize DigitalOcean to pull your GitHub repos.\n\n## Prerequisites:\n\n1) Python 3.9 on Linux or Mac\n2) DigitalOcean account https://www.digitalocean.com/?refcode=9ef6f738fd8a\n3) DigitalOcean API token: https://cloud.digitalocean.com/account/api/tokens\n4) DigitalOcean S3 keys: https://cloud.digitalocean.com/account/api/spaces\n5) Authorize DigitalOcean to pull your github repos: https://cloud.digitalocean.com/apps/github/install\n\n# Installation\n\nThis tool can be installed with pip. \nIf installed in a Django project, it will try to detect some settings from the project such as repo and branch,\nas well as enable migration of db.json files and media uploads.\n\n```shell\npip install dodevops\n```\n\nTo run the tool:\n\n```shell\ndodevops\n```\n\n# Quickstart\n\n## Migrate an existing Django project to DigitalOcean App Platform\n\n1) Create clean temporary directory for your project\n2) Create a virtual environment in the directory (python 3.9 or higher) \n   ```mkvirtualenv tempenv```\n3) git clone your project into the directory\n4) install requirements for your project\n   ```pip install -r requirements.txt```\n5) If you are migrating media uploads, copy your media folder into your project directory\n6) If you are migrating db.json files, copy or generate your db.json files into your project directory\n7) Run any project specific migration tasks\n8) Make sure pip is up to date\n   ```pip install --upgrade pip```\n9) Install dodevops\n   ```pip install dodevops```\n10) Export environment variables\n    ```\n    export DIGITALOCEAN_API_TOKEN=dop_v1_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\n    export AWS_ACCESS_KEY_ID=xxxxxxxxxxxxxxxxxxx\n    export AWS_SECRET_ACCESS_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\n    ```\n11) Run dodevops\n    ```dodevops```\n\n\n# Details\n\n## Generating DO API token\n\nIn order for this app to work it needs a valid DigitalOcean Personal Access Token. \nThe token is not required after this is run, so it is okay to recyle the token when finished. \nThe token can either be stored in a .env file or env variable, or it can be pasted into the app at run time. \n\n### To generating a new token\n\nGo here: https://cloud.digitalocean.com/account/api/tokens\n\nPick whatever name you want for the token, it doesn\'t matter. \nPick whatever token expiration you want depending on your personal paranoia level. \nWrite permissions are required. \n\nOnce the token is generated copy it and paste it somewhere safe like a password manager such as 1password. \nThe token won\'t be displayed again, so if you don\'t get it saved somewhere safe you\'ll have to regenerate it.\n\nProtect your token well. \nAnyone with access to your token has the ability to create and destroy things and incur you costs, so be careful with it. \nThis is opensource so that you can read the code if you want and verify how the token is used. \nStoring the token in the .env file is convenient, but it is not the most secure, so if you feel paranoid don\'t do that. \n\nIf you want more info about DO tokens, see here: https://docs.digitalocean.com/reference/api/create-personal-access-token/\n\n## Generating DO Spaces Key\n\nA DO Spaces key is required for storing a media upload folder, as app platform doesn\'t have storage. \n\n### To generate an app spaces key \n\nGo here: https://cloud.digitalocean.com/account/api/spaces \n\nYou can use whatever name you want for the key, it doesn\'t matter. \nIt will display two values, a key ID and a longer access key, save both somewhere safe like a password manager. \nIt won\'t display the access key again, so if you don\'t save it you\'ll have to regenerate it. \n\nYou can put the values in an .env file, or enter it at runtime.\n\nProtect the token well.\n\nTo learn more about DO spaces keys, go here: https://docs.digitalocean.com/products/spaces/how-to/manage-access/#access-keys\n\n## Filling out .env file\n\nA .env file isn\'t required, but if you store values in it then it will save effort.\nBut if you feel storing values in the .env file isn\'t secure enough for your personal paranoia levels you can instead enter things at runtime.\n\nThe format of the env file is:\n\n```\nDIGITALOCEAN_TOKEN=dop_v1_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\nAWS_ACCESS_KEY_ID=DOxxxxxxxxxxxxxxxxxxx\nAWS_SECRET_ACCESS_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx\n# AWS_REGION=ams3\n# APP_NAME=example-rest-app\n# COMPONENT_NAME=example-rest\n# APP_PREFIX=example\n# GH_REPO=xusernamex/xrepox\n# GH_BRANCH=main\n# DJANGO_ROOT_MODULE=example\n# DJANGO_USER_MODULE=core\n# SECRET_KEY_ENV_KEY=SECRET_KEY\n# SECRET_KEY=change_me\n# ALLOWED_HOSTS_ENV_KEY=ALLOWED_HOSTS\n# DEBUG=1\n# DOMAIN=rest.example.com\n# PARENT_DOMAIN=example.com\n# OIDC="\\"-----BEGIN RSA PRIVATE KEY-----\\\\n_xxx_\\\\n-----END RSA PRIVATE KEY-----\\\\n\\""\n```\n\n## Linux and Mac\n\nThis project uses inquirer to get user input. As far as I know it only works on linux and mac. \nWhen debugging in pycharm, you may need to set the run/debug settings to use the terminal emulation.\nYou can find a link with more info here: https://intellij-support.jetbrains.com/hc/en-us/community/posts/360003383619-Pycharm-2019-termios-error-25-Inappropriate-ioctl-for-device-?page=1#community_comment_6589796593042 and here https://github.com/magmax/python-readchar/issues/11\n',
     'author': 'Abby Oakwright',
     'author_email': 'abby.oakwright@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Oakwright/dodevops',
     'py_modules': modules,
     'install_requires': install_requires,
```

### Comparing `dodevops-0.1.8/PKG-INFO` & `dodevops-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,97 @@
 Metadata-Version: 2.1
 Name: dodevops
-Version: 0.1.8
+Version: 0.1.9
 Summary: Devops tool for deploying and managing resources on DigitalOcean
 Home-page: https://github.com/Oakwright/dodevops
 Keywords: devops,digitalocean,django
 Author: Abby Oakwright
 Author-email: abby.oakwright@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.143,<2.0.0)
 Requires-Dist: botocore (>=1.29.145,<2.0.0)
+Requires-Dist: configparser (>=6.0.0,<7.0.0)
 Requires-Dist: cryptography (>=39.0.1,<40.0.0)
 Requires-Dist: inquirer (>=3.1.3,<4.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pydo (>=0.1.4,<0.2.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Project-URL: Repository, https://github.com/Oakwright/dodevops
 Description-Content-Type: text/markdown
 
-# TLDR
+# **DoDevOps**
 
-This is a tool to take github repos for Django projects and put them on DigitalOcean App Spaces with managed database and DO Spaces S3 storage.
+DoDevOps is a tool for creating and managing Django apps on DigitalOcean's App Platform. 
+It accesses DigitalOcean through the API, so it requires a DigitalOcean API token,
+and it requires a DigitalOcean Spaces key for storing media uploads.
+Additionally, you must authorize DigitalOcean to pull your GitHub repos.
 
-You will need:
+## Prerequisites:
 
-1) Poetry installed locally to run this tool
+1) Python 3.9 on Linux or Mac
 2) DigitalOcean account https://www.digitalocean.com/?refcode=9ef6f738fd8a
 3) DigitalOcean API token: https://cloud.digitalocean.com/account/api/tokens
 4) DigitalOcean S3 keys: https://cloud.digitalocean.com/account/api/spaces
 5) Authorize DigitalOcean to pull your github repos: https://cloud.digitalocean.com/apps/github/install
-6) A DigitalOcean S3 bucket: https://cloud.digitalocean.com/spaces/new
-7) A DigitalOcean PostgreSQL database cluster: https://cloud.digitalocean.com/databases
-8) A database and user and connection pool configured on the database cluster
-9) Manually add the app as a trusted source on the database
 
-There are plans to integrate items 6-9 into this tool, we just haven't gotten that far yet.
+# Installation
+
+This tool can be installed with pip. 
+If installed in a Django project, it will try to detect some settings from the project such as repo and branch,
+as well as enable migration of db.json files and media uploads.
+
+```shell
+pip install dodevops
+```
 
 To run the tool:
 
 ```shell
-poetry run start
+dodevops
 ```
 
-# What is this
+# Quickstart
 
-This is essentially an experiment/prototype that got a little too big and had some potential. So it's being turned into a project.
+## Migrate an existing Django project to DigitalOcean App Platform
 
-proto.py is the original prototype.
+1) Create clean temporary directory for your project
+2) Create a virtual environment in the directory (python 3.9 or higher) 
+   ```mkvirtualenv tempenv```
+3) git clone your project into the directory
+4) install requirements for your project
+   ```pip install -r requirements.txt```
+5) If you are migrating media uploads, copy your media folder into your project directory
+6) If you are migrating db.json files, copy or generate your db.json files into your project directory
+7) Run any project specific migration tasks
+8) Make sure pip is up to date
+   ```pip install --upgrade pip```
+9) Install dodevops
+   ```pip install dodevops```
+10) Export environment variables
+    ```
+    export DIGITALOCEAN_API_TOKEN=dop_v1_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    export AWS_ACCESS_KEY_ID=xxxxxxxxxxxxxxxxxxx
+    export AWS_SECRET_ACCESS_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    ```
+11) Run dodevops
+    ```dodevops```
 
-This project uses inquirer to get user input. As far as I know it only works on linux and mac. 
-When debugging in pycharm, you may need to set the run/debug settings to use the terminal emulation.
-You can find a link with more info here: https://intellij-support.jetbrains.com/hc/en-us/community/posts/360003383619-Pycharm-2019-termios-error-25-Inappropriate-ioctl-for-device-?page=1#community_comment_6589796593042 and here https://github.com/magmax/python-readchar/issues/11
 
 # Details
 
 ## Generating DO API token
 
 In order for this app to work it needs a valid DigitalOcean Personal Access Token. 
 The token is not required after this is run, so it is okay to recyle the token when finished. 
-The token can either be stored in a .env file, or it can be pasted into the app at run time. 
+The token can either be stored in a .env file or env variable, or it can be pasted into the app at run time. 
 
 ### To generating a new token
 
 Go here: https://cloud.digitalocean.com/account/api/tokens
 
 Pick whatever name you want for the token, it doesn't matter. 
 Pick whatever token expiration you want depending on your personal paranoia level. 
@@ -74,63 +99,63 @@
 
 Once the token is generated copy it and paste it somewhere safe like a password manager such as 1password. 
 The token won't be displayed again, so if you don't get it saved somewhere safe you'll have to regenerate it.
 
 Protect your token well. 
 Anyone with access to your token has the ability to create and destroy things and incur you costs, so be careful with it. 
 This is opensource so that you can read the code if you want and verify how the token is used. 
-Storing the token in the .env file is convenient but it is not the most secure, so if you feel paranoid don't do that or delete the token after. 
+Storing the token in the .env file is convenient, but it is not the most secure, so if you feel paranoid don't do that. 
 
 If you want more info about DO tokens, see here: https://docs.digitalocean.com/reference/api/create-personal-access-token/
 
 ## Generating DO Spaces Key
 
 A DO Spaces key is required for storing a media upload folder, as app platform doesn't have storage. 
 
-### To generating an app spaces key 
+### To generate an app spaces key 
 
 Go here: https://cloud.digitalocean.com/account/api/spaces 
 
 You can use whatever name you want for the key, it doesn't matter. 
 It will display two values, a key ID and a longer access key, save both somewhere safe like a password manager. 
 It won't display the access key again, so if you don't save it you'll have to regenerate it. 
 
 You can put the values in an .env file, or enter it at runtime.
 
 Protect the token well.
 
 To learn more about DO spaces keys, go here: https://docs.digitalocean.com/products/spaces/how-to/manage-access/#access-keys
 
-## Create a DO Spaces S3 bucket
-
-You must create an S3 bucket on DO's web interface:
-
-https://cloud.digitalocean.com/spaces/new
-
 ## Filling out .env file
 
-A .env file isn't required, but if you store values in it then it will save effort. 
+A .env file isn't required, but if you store values in it then it will save effort.
 But if you feel storing values in the .env file isn't secure enough for your personal paranoia levels you can instead enter things at runtime.
 
 The format of the env file is:
 
 ```
 DIGITALOCEAN_TOKEN=dop_v1_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 AWS_ACCESS_KEY_ID=DOxxxxxxxxxxxxxxxxxxx
 AWS_SECRET_ACCESS_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 # AWS_REGION=ams3
 # APP_NAME=example-rest-app
 # COMPONENT_NAME=example-rest
 # APP_PREFIX=example
-GH_REPO=xusernamex/xrepox
+# GH_REPO=xusernamex/xrepox
 # GH_BRANCH=main
 # DJANGO_ROOT_MODULE=example
 # DJANGO_USER_MODULE=core
 # SECRET_KEY_ENV_KEY=SECRET_KEY
 # SECRET_KEY=change_me
 # ALLOWED_HOSTS_ENV_KEY=ALLOWED_HOSTS
 # DEBUG=1
 # DOMAIN=rest.example.com
 # PARENT_DOMAIN=example.com
 # OIDC="\"-----BEGIN RSA PRIVATE KEY-----\\n_xxx_\\n-----END RSA PRIVATE KEY-----\\n\""
 ```
 
+## Linux and Mac
+
+This project uses inquirer to get user input. As far as I know it only works on linux and mac. 
+When debugging in pycharm, you may need to set the run/debug settings to use the terminal emulation.
+You can find a link with more info here: https://intellij-support.jetbrains.com/hc/en-us/community/posts/360003383619-Pycharm-2019-termios-error-25-Inappropriate-ioctl-for-device-?page=1#community_comment_6589796593042 and here https://github.com/magmax/python-readchar/issues/11
+
```

