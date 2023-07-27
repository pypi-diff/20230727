# Comparing `tmp/saritasa_invocations-0.2.0.tar.gz` & `tmp/saritasa_invocations-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saritasa_invocations-0.2.0.tar", max compression
+gzip compressed data, was "saritasa_invocations-0.3.0.tar", max compression
```

## Comparing `saritasa_invocations-0.2.0.tar` & `saritasa_invocations-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1092 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/LICENSE
--rw-r--r--   0        0        0     7828 2023-07-25 10:22:05.388138 saritasa_invocations-0.2.0/README.md
--rw-r--r--   0        0        0     3893 2023-07-26 08:34:07.864855 saritasa_invocations-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      284 2023-07-25 10:21:50.404906 saritasa_invocations-0.2.0/saritasa_invocations/__init__.py
--rw-r--r--   0        0        0      900 2023-07-25 09:59:23.448672 saritasa_invocations-0.2.0/saritasa_invocations/celery.py
--rw-r--r--   0        0        0     6032 2023-07-26 08:00:52.721937 saritasa_invocations-0.2.0/saritasa_invocations/django.py
--rw-r--r--   0        0        0     5491 2023-07-25 09:59:23.448672 saritasa_invocations-0.2.0/saritasa_invocations/docker.py
--rw-r--r--   0        0        0      823 2023-07-25 09:59:23.448672 saritasa_invocations-0.2.0/saritasa_invocations/fastapi.py
--rw-r--r--   0        0        0      712 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/saritasa_invocations/git.py
--rw-r--r--   0        0        0      688 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/saritasa_invocations/github_actions.py
--rw-r--r--   0        0        0      457 2023-07-25 09:59:23.448672 saritasa_invocations-0.2.0/saritasa_invocations/open_api.py
--rw-r--r--   0        0        0      749 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/saritasa_invocations/pre_commit.py
--rw-r--r--   0        0        0      753 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/saritasa_invocations/printing.py
--rw-r--r--   0        0        0     2856 2023-07-25 10:22:05.388138 saritasa_invocations-0.2.0/saritasa_invocations/python.py
--rw-r--r--   0        0        0     1905 2023-07-13 03:53:10.395007 saritasa_invocations-0.2.0/saritasa_invocations/system.py
--rw-r--r--   0        0        0     8835 1970-01-01 00:00:00.000000 saritasa_invocations-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-13 03:53:10.395007 saritasa_invocations-0.3.0/LICENSE
+-rw-r--r--   0        0        0    10690 2023-07-27 03:17:28.077765 saritasa_invocations-0.3.0/README.md
+-rw-r--r--   0        0        0     3893 2023-07-27 03:15:01.906540 saritasa_invocations-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      297 2023-07-27 03:12:16.447282 saritasa_invocations-0.3.0/saritasa_invocations/__init__.py
+-rw-r--r--   0        0        0     3961 2023-07-27 03:12:16.447282 saritasa_invocations-0.3.0/saritasa_invocations/alembic.py
+-rw-r--r--   0        0        0      900 2023-07-25 09:59:23.448672 saritasa_invocations-0.3.0/saritasa_invocations/celery.py
+-rw-r--r--   0        0        0     6018 2023-07-27 03:04:21.552337 saritasa_invocations-0.3.0/saritasa_invocations/django.py
+-rw-r--r--   0        0        0     5491 2023-07-25 09:59:23.448672 saritasa_invocations-0.3.0/saritasa_invocations/docker.py
+-rw-r--r--   0        0        0      816 2023-07-27 03:04:21.552337 saritasa_invocations-0.3.0/saritasa_invocations/fastapi.py
+-rw-r--r--   0        0        0      712 2023-07-13 03:53:10.395007 saritasa_invocations-0.3.0/saritasa_invocations/git.py
+-rw-r--r--   0        0        0      688 2023-07-13 03:53:10.395007 saritasa_invocations-0.3.0/saritasa_invocations/github_actions.py
+-rw-r--r--   0        0        0      457 2023-07-25 09:59:23.448672 saritasa_invocations-0.3.0/saritasa_invocations/open_api.py
+-rw-r--r--   0        0        0      749 2023-07-13 03:53:10.395007 saritasa_invocations-0.3.0/saritasa_invocations/pre_commit.py
+-rw-r--r--   0        0        0      753 2023-07-13 03:53:10.395007 saritasa_invocations-0.3.0/saritasa_invocations/printing.py
+-rw-r--r--   0        0        0     2849 2023-07-27 03:04:21.552337 saritasa_invocations-0.3.0/saritasa_invocations/python.py
+-rw-r--r--   0        0        0     1905 2023-07-13 03:53:10.395007 saritasa_invocations-0.3.0/saritasa_invocations/system.py
+-rw-r--r--   0        0        0    11697 1970-01-01 00:00:00.000000 saritasa_invocations-0.3.0/PKG-INFO
```

### Comparing `saritasa_invocations-0.2.0/LICENSE` & `saritasa_invocations-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.2.0/README.md` & `saritasa_invocations-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,64 @@
 ![PyPI - License](https://img.shields.io/pypi/l/saritasa-invocations)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/saritasa-invocations)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 Collection of [invoke](https://www.pyinvoke.org/) commands used by Saritasa
 
+## Table of contents
+
+* [Installation](#installation)
+* [Configuration](#configuration)
+* [Modules](#modules)
+  * [system](#system)
+    * [system.copy-local-settings](#systemcopy-local-settings)
+    * [system.copy-vscode-settings](#systemcopy-vscode-settings)
+    * [system.chown](#systemchown)
+    * [system.create-tmp-folder](#systemcreate-tmp-folder)
+  * [git](#git)
+    * [git.set-git-setting](#gitset-git-setting)
+    * [git.setup](#gitsetup)
+  * [pre-commit](#pre-commit)
+    * [pre-commit.install](#pre-commitinstall)
+    * [pre-commit.run-hooks](#pre-commitrun-hooks)
+  * [docker](#docker)
+    * [docker.build-service](#dockerbuild-service)
+    * [docker.buildpack](#dockerbuildpack)
+    * [docker.stop-all-containers](#dockerstop-all-containers)
+    * [docker.up](#dockerup)
+    * [docker.stop](#dockerstop)
+    * [docker.clear](#dockerclear)
+  * [github-actions](#github-actions)
+    * [github-actions.set-up-hosts](#github-actionsset-up-hosts)
+  * [python](#python)
+    * [run](#pythonrun)
+  * [django](#django)
+    * [django.manage](#djangomanage)
+    * [django.makemigrations](#djangomakemigrations)
+    * [django.migrate](#djangomigrate)
+    * [django.resetdb](#djangoresetdb)
+    * [django.createsuperuser](#djangocreatesuperuser)
+    * [django.run](#djangorun)
+    * [django.shell](#djangoshell)
+    * [django.dbshell](#djangodbshell)
+  * [fastapi](#fastapi)
+    * [fastapi.run](#fastapirun)
+  * [alembic](#alembic)
+    * [alembic.run](#alembicrun)
+    * [alembic.autogenerate](#alembicautogenerate)
+    * [alembic.upgrade](#alembicupgrade)
+    * [alembic.downgrade](#alembicdowngrade)
+    * [alembic.check-for-migrations](#alembiccheck-for-migrations)
+    * [alembic.check-for-adjust-messages](#alembiccheck-for-adjust-messages)
+  * [celery](#celery)
+    * [celery.run](#celeryrun)
+  * [open-api](#open-api)
+    * [open-api.validate-swagger](#open-apivalidate-swagger)
+
 ## Installation
 
 ```bash
 pip install saritasa-invocations
 ```
 
 or if you are using [poetry](https://python-poetry.org/)
@@ -75,120 +125,124 @@
 )
 ```
 
 ## Modules
 
 ### system
 
-#### copy-local-settings
+#### system.copy-local-settings
 
 Copies local template for settings into specified file
 
 Settings:
+
 * `settings_template` path to settings template (Default: `config/settings/local.template.py`)
 * `save_settings_from_template_to` path to where save settings (Default: `config/settings/local.py`)
 
-#### copy-local-settings
+#### system.copy-vscode-settings
 
 Copies local template for vscode settings into `.vscode` folder
 
 Settings:
+
 * `vs_code_settings_template` path to settings template (Default: `.vscode/recommended_settings.json`)
 
-#### chown
+#### system.chown
 
 Change owner ship of project files to current user.
 
 Shortcut for owning apps dir by current user after some files were
 generated using docker-compose (migrations, new app, etc).
 
-#### create-tmp-folder
+#### system.create-tmp-folder
 
 Create folder for temporary files(`.tmp`).
 
 ### git
 
-#### set-git-setting
+#### git.set-git-setting
 
 Set git setting in config
 
-#### setup
+#### git.setup
 
 Preform setup of git:
 
 * Install pre-commit hooks
 * Set merge.ff
 * Set pull.ff
 
 Settings:
+
 * `merge_ff` setting value for `merge.ff` (Default: `false`)
 * `pull_ff` setting value for `pull.ff` (Default: `only`)
 
 ### pre-commit
 
-#### install
+#### pre-commit.install
 
 Install git hooks via pre-commit.
 
 Settings:
+
 * `pre_commit_hooks` list of hooks to install (Default: `["pre-commit", "pre-push", "commit-msg"]`)
 
-#### run-hooks
+#### pre-commit.run-hooks
 
 Run all hooks against all files
 
 ### docker
 
-#### build-service
+#### docker.build-service
 
 Build service image from docker compose
 
-#### buildpack
+#### docker.buildpack
 
 Build project via [pack-cli](https://buildpacks.io/docs/tools/pack/)
 
 Settings:
+
 * `buildpack_builder` image tag of builder (Default: `paketobuildpacks/builder:base`)
 * `buildpack_runner` image tag of runner (Default: `paketobuildpacks/run:base`)
 * `build_image_tag` image tag of builder (Default: Name of project from `project_name`)
 * `buildpack_requirements_path` path to folder with requirements (Default: `requirements`)
 
-#### stop-all-containers
+#### docker.stop-all-containers
 
 Shortcut for stopping ALL running docker containers
 
-#### up
+#### docker.up
 
 Bring up main containers and start them.
 
 Settings:
+
 * `docker_main_containers` image tag of builder (Default: `["postgres", "redis"]`)
 
-#### stop
+#### docker.stop
 
 Stop main containers.
 
 Settings:
+
 * `docker_main_containers` image tag of builder (Default: `["postgres", "redis"]`)
 
-#### clear
+#### docker.clear
 
 Stop and remove all containers defined in docker-compose. Also remove images.
 
 ### github-actions
 
-#### set-up-host
-
-Set up host in `/etc/hosts`
-
-#### set-up-hosts
+#### github-actions.set-up-hosts
 
 Add hosts to `/etc/hosts`.
 
 Settings:
+
 * `github_action_hosts` image tag of builder (Default: see `docker-main-containers`)
 
 ### python
 
 As of now we support two environments for python `local` and `docker`.
 
 * `local` is a python that is located in your current virtualenv
@@ -198,112 +252,156 @@
 
 Example of usage
 
 ```bash
 PYTHON_ENV=docker inv python.run-python --command="--version"
 ```
 
-#### run_python
+#### python.run
 
 Run python command depending on `PYTHON_ENV` variable(`docker` or `local`).
 
 Settings:
+
 * `python_entry` python entry command (Default: `python`)
 * `python_docker_service` python service name (Default: `web`)
 * `python_docker_service_params` params for docker (Default: `--rm`)
 
 ### django
 
-#### manage
+#### django.manage
 
 Run `manage.py` with specified command.
 
 This command also handle starting of required services and waiting DB to
 be ready.
 
 Requires [django_probes](https://github.com/painless-software/django-probes#basic-usage)
 
-#### makemigrations
+#### django.makemigrations
 
 Run `makemigrations` command and chown created migrations (only for docker env).
 
-#### check_new_migrations
+#### django.check_new_migrations
 
 Check if there is new migrations or not. Result should be check via exit code.
 
-#### migrate
+#### django.migrate
 
 Run `migrate` command.
 
 Settings:
+
 * `django_migrate_command` migrate command (Default: `migrate`)
 
-#### resetdb
+#### django.resetdb
 
 Reset database to initial state (including test DB).
 
 Requires [django-extensions](https://django-extensions.readthedocs.io/en/latest/installation_instructions.html)
 
-
-#### createsuperuser
+#### django.createsuperuser
 
 Create superuser.
 
 Settings:
+
 * `default_superuser_email` default email of superuser (Default: `root@localhost`)
 * `default_superuser_username` default username of superuser (Default: `root`)
 * `default_superuser_password` default password of superuser (Default: `root`)
 
-#### run
+#### django.run
 
 Run development web-server.
 
 Settings:
+
 * `runserver_docker_params` params for docker (Default: `--rm --service-ports`)
 * `runserver_command` runserver command (Default: `runserver_plus`)
 * `runserver_host` host of server (Default: `0.0.0.0`)
 * `runserver_port` port of server (Default: `8000`)
 * `runserver_params` params for runserver command (Default: `""`)
 
-#### shell
+#### django.shell
 
 Shortcut for manage.py shell command.
 
 Settings:
+
 * `shell_command` command to start python shell (Default: `shell_plus --ipython`)
 
-#### dbshell
+#### django.dbshell
 
 Open database shell with credentials from current django settings.
 
 ### fastapi
 
-#### run
+#### fastapi.run
 
 Run development web-server.
 
 Settings:
+
 * `fastapi_docker_params` params for docker (Default: `--rm --service-ports`)
 * `fastapi_uvicorn_command` uvicorn command (Default: `-m uvicorn`)
 * `fastapi_app` path to fastapi app (Default: `config:fastapi_app`)
 * `fastapi_host` host of server (Default: `0.0.0.0`)
 * `fastapi_port` port of server (Default: `8000`)
 * `fastapi_params` params for uvicorn (Default: `--reload`)
 
+### alembic
+
+#### alembic.run
+
+Run alembic command
+
+Settings:
+
+* `alembic_command` alembic command (Default: `-m alembic`)
+
+#### alembic.autogenerate
+
+Generate migrations
+
+Settings:
+
+* `alembic_migrations_folder` migrations files location (Default: `db/migrations/versions`)
+
+#### alembic.upgrade
+
+Upgrade database
+
+#### alembic.downgrade
+
+Downgrade database
+
+#### alembic.check-for-migrations
+
+Check if there any missing migrations to be generated
+
+#### alembic.check-for-adjust-messages
+
+Check migration files for adjust messages
+
+Settings:
+
+* `alembic_migrations_folder` migrations files location (Default: `db/migrations/versions`)
+* `alembic_adjust_messages` list of alembic adjust messages (Default: `# ### commands auto generated by Alembic - please adjust! ###`, `# ### end Alembic commands ###`)
 
 ### celery
 
-#### run
+#### celery.run
 
 Start celery worker.
 
 Settings:
+
 * `celery_local_cmd` command for celery (Default: `celery --app config.celery:app worker --beat --scheduler=django --loglevel=info`)
 * `celery_service_name` name of celery service (Default: `celery`)
 
 ### open-api
 
-#### validate-swagger
+#### open-api.validate-swagger
 
 Check that generated open_api spec is valid. This command uses
 [drf-spectacular](https://github.com/tfranzel/drf-spectacular) and
 it's default validator. It creates spec file in ./tmp folder and then validates it.
```

### Comparing `saritasa_invocations-0.2.0/pyproject.toml` & `saritasa_invocations-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saritasa-invocations"
-version = "0.2.0"
+version = "0.3.0"
 description = "Collection of invoke commands used by Saritasa"
 authors = [
   "Saritasa <pypi@saritasa.com>",
 ]
 maintainers = [
     "Stanislav Khlud <stanislav.khlud@saritasa.com>",
 ]
```

### Comparing `saritasa_invocations-0.2.0/saritasa_invocations/celery.py` & `saritasa_invocations-0.3.0/saritasa_invocations/celery.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.2.0/saritasa_invocations/django.py` & `saritasa_invocations-0.3.0/saritasa_invocations/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         https://github.com/painless-software/django-probes#basic-usage
 
     """
     if hasattr(wait_for_database, "_called"):
         return
     docker.up(context)
     # Not using manage to avoid infinite loop
-    python.run_python(
+    python.run(
         context,
         command="manage.py wait_for_database --stable 0",
     )
     wait_for_database._called = True
 
 
 @invoke.task
@@ -41,15 +41,15 @@
         context: Invoke context
         command: Manage command
         docker_params: Params for docker run
         watchers: Automated responders to command
 
     """
     wait_for_database(context)
-    python.run_python(
+    python.run(
         context,
         docker_params=docker_params,
         command=f"manage.py {command}",
         watchers=watchers,
     )
```

### Comparing `saritasa_invocations-0.2.0/saritasa_invocations/docker.py` & `saritasa_invocations-0.3.0/saritasa_invocations/docker.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.2.0/saritasa_invocations/fastapi.py` & `saritasa_invocations-0.3.0/saritasa_invocations/fastapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,12 +14,12 @@
     uvicorn_command = config.get("fastapi_uvicorn_command", "-m uvicorn")
     app = config.get("fastapi_app", "config:fastapi_app")
     host = config.get("fastapi_host", "0.0.0.0")
     port = config.get("fastapi_port", "8000")
     params = config.get("fastapi_params", "--reload")
 
     command = f"{uvicorn_command} {app} --host {host} --port {port} {params}"
-    python.run_python(
+    python.run(
         context,
         docker_params=docker_params,
         command=command,
     )
```

### Comparing `saritasa_invocations-0.2.0/saritasa_invocations/git.py` & `saritasa_invocations-0.3.0/saritasa_invocations/git.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.2.0/saritasa_invocations/github_actions.py` & `saritasa_invocations-0.3.0/saritasa_invocations/github_actions.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.2.0/saritasa_invocations/pre_commit.py` & `saritasa_invocations-0.3.0/saritasa_invocations/pre_commit.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.2.0/saritasa_invocations/printing.py` & `saritasa_invocations-0.3.0/saritasa_invocations/printing.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.2.0/saritasa_invocations/python.py` & `saritasa_invocations-0.3.0/saritasa_invocations/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     context.run(
         command=f"{python_entry} {command}",
         watchers=watchers,
     )
 
 
 @invoke.task
-def run_python(
+def run(
     context: invoke.Context,
     command: str,
     docker_params: str | None = None,
     watchers: typing.Iterable[invoke.StreamWatcher] = (),
 ) -> None:
     """Execute python command."""
     match get_python_env():
```

### Comparing `saritasa_invocations-0.2.0/saritasa_invocations/system.py` & `saritasa_invocations-0.3.0/saritasa_invocations/system.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-0.2.0/PKG-INFO` & `saritasa_invocations-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saritasa-invocations
-Version: 0.2.0
+Version: 0.3.0
 Summary: Collection of invoke commands used by Saritasa
 Home-page: https://pypi.org/project/saritasa-invocations/
 License: MIT
 Keywords: python,invoke
 Author: Saritasa
 Author-email: pypi@saritasa.com
 Maintainer: Stanislav Khlud
@@ -33,14 +33,64 @@
 ![PyPI - License](https://img.shields.io/pypi/l/saritasa-invocations)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/saritasa-invocations)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 Collection of [invoke](https://www.pyinvoke.org/) commands used by Saritasa
 
+## Table of contents
+
+* [Installation](#installation)
+* [Configuration](#configuration)
+* [Modules](#modules)
+  * [system](#system)
+    * [system.copy-local-settings](#systemcopy-local-settings)
+    * [system.copy-vscode-settings](#systemcopy-vscode-settings)
+    * [system.chown](#systemchown)
+    * [system.create-tmp-folder](#systemcreate-tmp-folder)
+  * [git](#git)
+    * [git.set-git-setting](#gitset-git-setting)
+    * [git.setup](#gitsetup)
+  * [pre-commit](#pre-commit)
+    * [pre-commit.install](#pre-commitinstall)
+    * [pre-commit.run-hooks](#pre-commitrun-hooks)
+  * [docker](#docker)
+    * [docker.build-service](#dockerbuild-service)
+    * [docker.buildpack](#dockerbuildpack)
+    * [docker.stop-all-containers](#dockerstop-all-containers)
+    * [docker.up](#dockerup)
+    * [docker.stop](#dockerstop)
+    * [docker.clear](#dockerclear)
+  * [github-actions](#github-actions)
+    * [github-actions.set-up-hosts](#github-actionsset-up-hosts)
+  * [python](#python)
+    * [run](#pythonrun)
+  * [django](#django)
+    * [django.manage](#djangomanage)
+    * [django.makemigrations](#djangomakemigrations)
+    * [django.migrate](#djangomigrate)
+    * [django.resetdb](#djangoresetdb)
+    * [django.createsuperuser](#djangocreatesuperuser)
+    * [django.run](#djangorun)
+    * [django.shell](#djangoshell)
+    * [django.dbshell](#djangodbshell)
+  * [fastapi](#fastapi)
+    * [fastapi.run](#fastapirun)
+  * [alembic](#alembic)
+    * [alembic.run](#alembicrun)
+    * [alembic.autogenerate](#alembicautogenerate)
+    * [alembic.upgrade](#alembicupgrade)
+    * [alembic.downgrade](#alembicdowngrade)
+    * [alembic.check-for-migrations](#alembiccheck-for-migrations)
+    * [alembic.check-for-adjust-messages](#alembiccheck-for-adjust-messages)
+  * [celery](#celery)
+    * [celery.run](#celeryrun)
+  * [open-api](#open-api)
+    * [open-api.validate-swagger](#open-apivalidate-swagger)
+
 ## Installation
 
 ```bash
 pip install saritasa-invocations
 ```
 
 or if you are using [poetry](https://python-poetry.org/)
@@ -101,120 +151,124 @@
 )
 ```
 
 ## Modules
 
 ### system
 
-#### copy-local-settings
+#### system.copy-local-settings
 
 Copies local template for settings into specified file
 
 Settings:
+
 * `settings_template` path to settings template (Default: `config/settings/local.template.py`)
 * `save_settings_from_template_to` path to where save settings (Default: `config/settings/local.py`)
 
-#### copy-local-settings
+#### system.copy-vscode-settings
 
 Copies local template for vscode settings into `.vscode` folder
 
 Settings:
+
 * `vs_code_settings_template` path to settings template (Default: `.vscode/recommended_settings.json`)
 
-#### chown
+#### system.chown
 
 Change owner ship of project files to current user.
 
 Shortcut for owning apps dir by current user after some files were
 generated using docker-compose (migrations, new app, etc).
 
-#### create-tmp-folder
+#### system.create-tmp-folder
 
 Create folder for temporary files(`.tmp`).
 
 ### git
 
-#### set-git-setting
+#### git.set-git-setting
 
 Set git setting in config
 
-#### setup
+#### git.setup
 
 Preform setup of git:
 
 * Install pre-commit hooks
 * Set merge.ff
 * Set pull.ff
 
 Settings:
+
 * `merge_ff` setting value for `merge.ff` (Default: `false`)
 * `pull_ff` setting value for `pull.ff` (Default: `only`)
 
 ### pre-commit
 
-#### install
+#### pre-commit.install
 
 Install git hooks via pre-commit.
 
 Settings:
+
 * `pre_commit_hooks` list of hooks to install (Default: `["pre-commit", "pre-push", "commit-msg"]`)
 
-#### run-hooks
+#### pre-commit.run-hooks
 
 Run all hooks against all files
 
 ### docker
 
-#### build-service
+#### docker.build-service
 
 Build service image from docker compose
 
-#### buildpack
+#### docker.buildpack
 
 Build project via [pack-cli](https://buildpacks.io/docs/tools/pack/)
 
 Settings:
+
 * `buildpack_builder` image tag of builder (Default: `paketobuildpacks/builder:base`)
 * `buildpack_runner` image tag of runner (Default: `paketobuildpacks/run:base`)
 * `build_image_tag` image tag of builder (Default: Name of project from `project_name`)
 * `buildpack_requirements_path` path to folder with requirements (Default: `requirements`)
 
-#### stop-all-containers
+#### docker.stop-all-containers
 
 Shortcut for stopping ALL running docker containers
 
-#### up
+#### docker.up
 
 Bring up main containers and start them.
 
 Settings:
+
 * `docker_main_containers` image tag of builder (Default: `["postgres", "redis"]`)
 
-#### stop
+#### docker.stop
 
 Stop main containers.
 
 Settings:
+
 * `docker_main_containers` image tag of builder (Default: `["postgres", "redis"]`)
 
-#### clear
+#### docker.clear
 
 Stop and remove all containers defined in docker-compose. Also remove images.
 
 ### github-actions
 
-#### set-up-host
-
-Set up host in `/etc/hosts`
-
-#### set-up-hosts
+#### github-actions.set-up-hosts
 
 Add hosts to `/etc/hosts`.
 
 Settings:
+
 * `github_action_hosts` image tag of builder (Default: see `docker-main-containers`)
 
 ### python
 
 As of now we support two environments for python `local` and `docker`.
 
 * `local` is a python that is located in your current virtualenv
@@ -224,113 +278,157 @@
 
 Example of usage
 
 ```bash
 PYTHON_ENV=docker inv python.run-python --command="--version"
 ```
 
-#### run_python
+#### python.run
 
 Run python command depending on `PYTHON_ENV` variable(`docker` or `local`).
 
 Settings:
+
 * `python_entry` python entry command (Default: `python`)
 * `python_docker_service` python service name (Default: `web`)
 * `python_docker_service_params` params for docker (Default: `--rm`)
 
 ### django
 
-#### manage
+#### django.manage
 
 Run `manage.py` with specified command.
 
 This command also handle starting of required services and waiting DB to
 be ready.
 
 Requires [django_probes](https://github.com/painless-software/django-probes#basic-usage)
 
-#### makemigrations
+#### django.makemigrations
 
 Run `makemigrations` command and chown created migrations (only for docker env).
 
-#### check_new_migrations
+#### django.check_new_migrations
 
 Check if there is new migrations or not. Result should be check via exit code.
 
-#### migrate
+#### django.migrate
 
 Run `migrate` command.
 
 Settings:
+
 * `django_migrate_command` migrate command (Default: `migrate`)
 
-#### resetdb
+#### django.resetdb
 
 Reset database to initial state (including test DB).
 
 Requires [django-extensions](https://django-extensions.readthedocs.io/en/latest/installation_instructions.html)
 
-
-#### createsuperuser
+#### django.createsuperuser
 
 Create superuser.
 
 Settings:
+
 * `default_superuser_email` default email of superuser (Default: `root@localhost`)
 * `default_superuser_username` default username of superuser (Default: `root`)
 * `default_superuser_password` default password of superuser (Default: `root`)
 
-#### run
+#### django.run
 
 Run development web-server.
 
 Settings:
+
 * `runserver_docker_params` params for docker (Default: `--rm --service-ports`)
 * `runserver_command` runserver command (Default: `runserver_plus`)
 * `runserver_host` host of server (Default: `0.0.0.0`)
 * `runserver_port` port of server (Default: `8000`)
 * `runserver_params` params for runserver command (Default: `""`)
 
-#### shell
+#### django.shell
 
 Shortcut for manage.py shell command.
 
 Settings:
+
 * `shell_command` command to start python shell (Default: `shell_plus --ipython`)
 
-#### dbshell
+#### django.dbshell
 
 Open database shell with credentials from current django settings.
 
 ### fastapi
 
-#### run
+#### fastapi.run
 
 Run development web-server.
 
 Settings:
+
 * `fastapi_docker_params` params for docker (Default: `--rm --service-ports`)
 * `fastapi_uvicorn_command` uvicorn command (Default: `-m uvicorn`)
 * `fastapi_app` path to fastapi app (Default: `config:fastapi_app`)
 * `fastapi_host` host of server (Default: `0.0.0.0`)
 * `fastapi_port` port of server (Default: `8000`)
 * `fastapi_params` params for uvicorn (Default: `--reload`)
 
+### alembic
+
+#### alembic.run
+
+Run alembic command
+
+Settings:
+
+* `alembic_command` alembic command (Default: `-m alembic`)
+
+#### alembic.autogenerate
+
+Generate migrations
+
+Settings:
+
+* `alembic_migrations_folder` migrations files location (Default: `db/migrations/versions`)
+
+#### alembic.upgrade
+
+Upgrade database
+
+#### alembic.downgrade
+
+Downgrade database
+
+#### alembic.check-for-migrations
+
+Check if there any missing migrations to be generated
+
+#### alembic.check-for-adjust-messages
+
+Check migration files for adjust messages
+
+Settings:
+
+* `alembic_migrations_folder` migrations files location (Default: `db/migrations/versions`)
+* `alembic_adjust_messages` list of alembic adjust messages (Default: `# ### commands auto generated by Alembic - please adjust! ###`, `# ### end Alembic commands ###`)
 
 ### celery
 
-#### run
+#### celery.run
 
 Start celery worker.
 
 Settings:
+
 * `celery_local_cmd` command for celery (Default: `celery --app config.celery:app worker --beat --scheduler=django --loglevel=info`)
 * `celery_service_name` name of celery service (Default: `celery`)
 
 ### open-api
 
-#### validate-swagger
+#### open-api.validate-swagger
 
 Check that generated open_api spec is valid. This command uses
 [drf-spectacular](https://github.com/tfranzel/drf-spectacular) and
 it's default validator. It creates spec file in ./tmp folder and then validates it.
```

