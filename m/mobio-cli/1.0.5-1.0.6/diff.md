# Comparing `tmp/mobio-cli-1.0.5.tar.gz` & `tmp/mobio-cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-cli-1.0.5.tar", last modified: Tue Jun 20 04:57:42 2023, max compression
+gzip compressed data, was "mobio-cli-1.0.6.tar", last modified: Thu Jul 27 07:42:45 2023, max compression
```

## Comparing `mobio-cli-1.0.5.tar` & `mobio-cli-1.0.6.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/
--rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-05-04 11:47:35.000000 mobio-cli-1.0.5/MANIFEST.in
--rw-r--r--   0 ChungNT    (501) staff       (20)     1127 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/PKG-INFO
--rw-r--r--   0 ChungNT    (501) staff       (20)      743 2023-06-20 04:56:25.000000 mobio-cli-1.0.5/README.md
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/
--rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-04-26 18:02:24.000000 mobio-cli-1.0.5/mobio_cli/__init__.py
--rw-r--r--   0 ChungNT    (501) staff       (20)     5324 2023-02-15 09:44:10.000000 mobio-cli-1.0.5/mobio_cli/__main__.py
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/
--rw-r--r--   0 ChungNT    (501) staff       (20)     1187 2023-02-14 06:38:19.000000 mobio-cli-1.0.5/mobio_cli/templates/Dockerfile
--rw-r--r--   0 ChungNT    (501) staff       (20)     1496 2023-02-14 06:39:12.000000 mobio-cli-1.0.5/mobio_cli/templates/Dockerfile-release
--rw-r--r--   0 ChungNT    (501) staff       (20)       55 2021-05-04 19:20:07.000000 mobio-cli-1.0.5/mobio_cli/templates/README.md
--rw-r--r--   0 ChungNT    (501) staff       (20)      265 2021-10-07 09:50:11.000000 mobio-cli-1.0.5/mobio_cli/templates/app_{#PROJECT_NAME_SNAKE_LOWERCASE#}_api.{pymobio}
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/configs/
--rw-r--r--   0 ChungNT    (501) staff       (20)     1167 2023-02-15 08:52:06.000000 mobio-cli-1.0.5/mobio_cli/templates/configs/__init__.{pymobio}
--rw-r--r--   0 ChungNT    (501) staff       (20)     4745 2023-02-13 09:22:10.000000 mobio-cli-1.0.5/mobio_cli/templates/k8s-Jenkinsfile
--rw-r--r--   0 ChungNT    (501) staff       (20)      388 2021-08-17 17:39:15.000000 mobio-cli-1.0.5/mobio_cli/templates/prepare_env.sh
--rw-r--r--   0 ChungNT    (501) staff       (20)       66 2023-06-20 04:54:55.000000 mobio-cli-1.0.5/mobio_cli/templates/requirements.txt
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/configs/
--rw-r--r--   0 ChungNT    (501) staff       (20)      268 2021-04-13 11:49:20.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/configs/{#PROJECT_NAME_SNAKE_LOWERCASE#}.conf
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/lang/
--rw-r--r--   0 ChungNT    (501) staff       (20)     1008 2023-02-15 08:46:40.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/lang/message_en.json
--rw-r--r--   0 ChungNT    (501) staff       (20)     1158 2023-02-15 08:46:46.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/lang/message_vi.json
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/src/
--rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-03-12 07:01:14.000000 mobio-cli-1.0.5/mobio_cli/templates/src/__init__.{pymobio}
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/src/apis/
--rw-r--r--   0 ChungNT    (501) staff       (20)     3808 2023-02-15 09:11:58.000000 mobio-cli-1.0.5/mobio_cli/templates/src/apis/__init__.{pymobio}
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/src/apis/v1_0/
--rw-r--r--   0 ChungNT    (501) staff       (20)       43 2021-04-23 02:12:16.000000 mobio-cli-1.0.5/mobio_cli/templates/src/apis/v1_0/__init__.{pymobio}
--rw-r--r--   0 ChungNT    (501) staff       (20)      297 2021-07-22 04:38:08.000000 mobio-cli-1.0.5/mobio_cli/templates/src/apis/v1_0/blueprints_api.{pymobio}
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/src/common/
--rw-r--r--   0 ChungNT    (501) staff       (20)       47 2023-02-15 08:19:00.000000 mobio-cli-1.0.5/mobio_cli/templates/src/common/__init__.{pymobio}
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/src/controllers/
--rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-08-17 18:16:25.000000 mobio-cli-1.0.5/mobio_cli/templates/src/controllers/empty
--rw-r--r--   0 ChungNT    (501) staff       (20)      760 2021-07-18 18:03:26.000000 mobio-cli-1.0.5/mobio_cli/templates/startup.sh
--rw-r--r--   0 ChungNT    (501) staff       (20)      214 2021-10-11 09:16:05.000000 mobio-cli-1.0.5/mobio_cli/templates/test.env
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/yaml/
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/yaml/BASE/
--rw-r--r--   0 ChungNT    (501) staff       (20)     1932 2023-06-20 04:54:17.000000 mobio-cli-1.0.5/mobio_cli/templates/yaml/BASE/deploy_{#PROJECT_NAME_SNAKE_LOWERCASE#}_app_api.yaml
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/
--rw-r--r--   0 ChungNT    (501) staff       (20)     1127 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/PKG-INFO
--rw-r--r--   0 ChungNT    (501) staff       (20)     1184 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ChungNT    (501) staff       (20)        1 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ChungNT    (501) staff       (20)       55 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/entry_points.txt
--rw-r--r--   0 ChungNT    (501) staff       (20)       10 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/top_level.txt
--rw-r--r--   0 ChungNT    (501) staff       (20)       38 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/setup.cfg
--rw-r--r--   0 ChungNT    (501) staff       (20)     1211 2023-06-20 04:57:41.000000 mobio-cli-1.0.5/setup.py
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/
+-rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-05-04 11:47:35.000000 mobio-cli-1.0.6/MANIFEST.in
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1286 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/PKG-INFO
+-rw-r--r--   0 ChungNT    (501) staff       (20)      902 2023-07-27 07:41:48.000000 mobio-cli-1.0.6/README.md
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/
+-rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-04-26 18:02:24.000000 mobio-cli-1.0.6/mobio_cli/__init__.py
+-rw-r--r--   0 ChungNT    (501) staff       (20)     5692 2023-07-27 07:33:29.000000 mobio-cli-1.0.6/mobio_cli/__main__.py
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1187 2023-02-14 06:38:19.000000 mobio-cli-1.0.6/mobio_cli/templates/Dockerfile
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1496 2023-02-14 06:39:12.000000 mobio-cli-1.0.6/mobio_cli/templates/Dockerfile-release
+-rw-r--r--   0 ChungNT    (501) staff       (20)       55 2021-05-04 19:20:07.000000 mobio-cli-1.0.6/mobio_cli/templates/README.md
+-rw-r--r--   0 ChungNT    (501) staff       (20)      265 2021-10-07 09:50:11.000000 mobio-cli-1.0.6/mobio_cli/templates/app_{#PROJECT_NAME_SNAKE_LOWERCASE#}_api.{pymobio}
+-rw-r--r--   0 ChungNT    (501) staff       (20)      399 2023-07-26 06:54:56.000000 mobio-cli-1.0.6/mobio_cli/templates/check_image.sh
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/configs/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1167 2023-02-15 08:52:06.000000 mobio-cli-1.0.6/mobio_cli/templates/configs/__init__.{pymobio}
+-rw-r--r--   0 ChungNT    (501) staff       (20)     4859 2023-07-26 09:07:19.000000 mobio-cli-1.0.6/mobio_cli/templates/k8s-Jenkinsfile
+-rw-r--r--   0 ChungNT    (501) staff       (20)      388 2021-08-17 17:39:15.000000 mobio-cli-1.0.6/mobio_cli/templates/prepare_env.sh
+-rw-r--r--   0 ChungNT    (501) staff       (20)       67 2023-07-26 09:11:58.000000 mobio-cli-1.0.6/mobio_cli/templates/requirements.txt
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/resources/
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/resources/configs/
+-rw-r--r--   0 ChungNT    (501) staff       (20)      268 2021-04-13 11:49:20.000000 mobio-cli-1.0.6/mobio_cli/templates/resources/configs/{#PROJECT_NAME_SNAKE_LOWERCASE#}.conf
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/resources/lang/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1008 2023-02-15 08:46:40.000000 mobio-cli-1.0.6/mobio_cli/templates/resources/lang/message_en.json
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1158 2023-02-15 08:46:46.000000 mobio-cli-1.0.6/mobio_cli/templates/resources/lang/message_vi.json
+-rw-r--r--   0 ChungNT    (501) staff       (20)      550 2023-07-26 09:15:26.000000 mobio-cli-1.0.6/mobio_cli/templates/script-update-version.sh
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/src/
+-rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-03-12 07:01:14.000000 mobio-cli-1.0.6/mobio_cli/templates/src/__init__.{pymobio}
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/src/apis/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     4248 2023-07-27 07:12:32.000000 mobio-cli-1.0.6/mobio_cli/templates/src/apis/__init__.{pymobio}
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/src/apis/v1_0/
+-rw-r--r--   0 ChungNT    (501) staff       (20)       43 2021-04-23 02:12:16.000000 mobio-cli-1.0.6/mobio_cli/templates/src/apis/v1_0/__init__.{pymobio}
+-rw-r--r--   0 ChungNT    (501) staff       (20)      297 2021-07-22 04:38:08.000000 mobio-cli-1.0.6/mobio_cli/templates/src/apis/v1_0/blueprints_api.{pymobio}
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/src/common/
+-rw-r--r--   0 ChungNT    (501) staff       (20)       47 2023-02-15 08:19:00.000000 mobio-cli-1.0.6/mobio_cli/templates/src/common/__init__.{pymobio}
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/src/controllers/
+-rw-r--r--   0 ChungNT    (501) staff       (20)      831 2023-07-27 07:28:38.000000 mobio-cli-1.0.6/mobio_cli/templates/src/controllers/example_controller.{pymobio}
+-rw-r--r--   0 ChungNT    (501) staff       (20)      760 2021-07-18 18:03:26.000000 mobio-cli-1.0.6/mobio_cli/templates/startup.sh
+-rw-r--r--   0 ChungNT    (501) staff       (20)      268 2023-07-26 04:52:02.000000 mobio-cli-1.0.6/mobio_cli/templates/test.env
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/yaml/
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli/templates/yaml/BASE/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1547 2023-07-26 06:46:51.000000 mobio-cli-1.0.6/mobio_cli/templates/yaml/BASE/0_script_init_deploy.yaml
+-rw-r--r--   0 ChungNT    (501) staff       (20)     2504 2023-07-26 09:05:35.000000 mobio-cli-1.0.6/mobio_cli/templates/yaml/BASE/deploy_{#PROJECT_NAME_SNAKE_LOWERCASE#}_app_api.yaml
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli.egg-info/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1286 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1343 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ChungNT    (501) staff       (20)        1 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ChungNT    (501) staff       (20)       55 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ChungNT    (501) staff       (20)       10 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/mobio_cli.egg-info/top_level.txt
+-rw-r--r--   0 ChungNT    (501) staff       (20)       38 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/setup.cfg
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1211 2023-07-27 07:42:45.000000 mobio-cli-1.0.6/setup.py
```

### Comparing `mobio-cli-1.0.5/PKG-INFO` & `mobio-cli-1.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,37 @@
-Metadata-Version: 2.1
-Name: mobio-cli
-Version: 1.0.5
-Summary: Command line create Mobio's projects
-Home-page: UNKNOWN
-Author: MOBIO
-Author-email: contact@mobio.vn
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-
 ## Tool generate Mobio Python Project
 
 ## Copyright: MobioVN
 
 ## Version:
 
-Phiên bản hiện tại `1.0.5`. Xem [changelog](#Changlog)
+Phiên bản hiện tại `1.0.6`. Xem [changelog](#Changlog)
 
 ## Cài đặt:
 
 `pip3 install mobio-cli`
 
 ## Sử dụng:
 
 `mobio-cli`
 
 ## Changelog:
 
+#### v1.0.6:
+* Cập nhật theo quy định mới (thêm init-container).
+* Fix lỗi tạo auth.verify_token.
+* Thêm tham số generate ExampleController.
+
 #### v1.0.5:
 * Cập nhật file .yaml (Thêm secretRef).
 * Upgrade dependency mobio-base-sdk==1.0.13.
 
 #### v1.0.4:
 * Cập nhật lại version trong README.
 
 #### v1.0.3:
 * Tương thích với Mobio base SDK mới. [See](https://pypi.org/project/mobio-base-sdk/1.0.12/)
 * Sửa lại format các file sinh tự động theo thống nhất họp mới nhất.
 * Loại bỏ một số file (do đã được merge vào Base SDK): logging, lang_config, common/__init__,...
 
 #### v1.0.2:
-* Phiên bản đầu tiên.
-
+* Phiên bản đầu tiên.
```

### Comparing `mobio-cli-1.0.5/mobio_cli/__main__.py` & `mobio-cli-1.0.6/mobio_cli/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     input_ = raw_input  # Python2.7
 elif sys.version_info[0] < 4:
     input_ = input  # Python3.+
 
 
 __TEMPLATE_DIR__ = 'templates'
 RESOURCES_OF_TEMPLATE_PROJECT, _ = os.path.split(os.path.abspath(__file__))
-__REMOVED_FILES__ = ['empty']
+__REMOVED_FILES__ = ['empty', 'startup.sh']
 __IGNORE_FILES_TEMPLATE__ = ['.+\.json$', '^mobio_exception.+']
 __DEPENDENCIES_FILE__ = 'requirements.txt'
+__EXAMPLE_FILE__ = ['example_controller.py']
 
 
 def _camel_to_snake(name):
     name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
     return re.sub('([a-z0-9])([A-Z])', r'\1_\2', name).lower()
 
 
@@ -49,33 +50,35 @@
     return user_input
 
 
 def _get_user_inputs():
 
     name = _get_input('project_name(CapitalizeWord, ex: JourneyBuilder)')
     description = _get_input('project_description')
-    port = _get_input('project_port(default: 80)')
+    port = '80' # _get_input('project_port(default: 80)')
     if not port:
         port = '80'
+    generate_controller_example = _get_input('Generate example controller(y/n)')
 
     print('')
     print('Setup overview')
     print('--------------')
     print('Project name: %s' % name)
     print('Description: %s' % description)
     print('Port: %s' % port)
+    print('Generate example: %s' % generate_controller_example)
     print('')
     correct = _is_yes(_get_input('Is this correct?(y/n)'))
     if not correct:
         print()
         return _get_user_inputs()
-    return name, description, port
+    return name, description, port, generate_controller_example
 
 
-def _setup(name, description, port, args=argparse.Namespace()):
+def _setup(name, description, port, generate_example, args=argparse.Namespace()):
     project_name_camel = name
     project_name_snake_lowercase = _camel_to_snake(name)
     project_name_snake_uppercase = project_name_snake_lowercase.upper()
     project_name_kebab_lowercase = _camel_to_kebab(name)
     project_name_kebab_uppercase = project_name_kebab_lowercase.upper()
     date_created = datetime.now().strftime("%Y/%m/%d")
     project_path = os.path.join(os.getcwd(), project_name_camel)
@@ -101,26 +104,27 @@
     for (path, directories, filenames) in os.walk(source_dir):
         relative_path = path[len(source_dir + '/'):]
         os.makedirs(os.path.join(dest_dir, relative_path), exist_ok=True)
         for filename in filenames:
             source = os.path.join(path, filename)
             # print('-------------')
             # print(filename)
+            if filename in __EXAMPLE_FILE__ and generate_example.lower() == 'n':
+                continue
             _process_file(source, relative_path, filename, dest_dir, replace_options)
 
     python_path = sys.executable
     create_venv = _get_input("create venv?(y/n)")
     if create_venv == 'y' or create_venv == 'Y':
         venv_path = os.path.join(project_path, 'venv')
         subprocess.run([python_path, '-m', 'venv', venv_path])
         subprocess.run([os.path.join(venv_path, 'bin', 'pip'),
                         'install', '-r',
                         os.path.join(project_path, __DEPENDENCIES_FILE__)])
 
-
 def _process_file(source, relative_path, filename, dest_dir, replace_options):
     if filename in __REMOVED_FILES__:
         return
 
     with open(source, 'rt') as fin:
         source_code = fin.read()
 
@@ -152,14 +156,14 @@
     parser = argparse.ArgumentParser()
     parser.add_argument('-y', '--yes', action='store_true',
                         help="Say 'yes' to all prompts")
     parser.add_argument('-f', '--force', action='store_true',
                         help="Force remove exist directory")
     args = parser.parse_known_args()[0]
 
-    defaults = ('TestAbc', 'test %s' % format(datetime.utcnow()), '80')
+    defaults = ('TestAbc', 'test %s' % format(datetime.utcnow()), '80', 'n')
     inputs = defaults if args.yes else _get_user_inputs()
     _setup(*inputs, args=args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mobio-cli-1.0.5/mobio_cli/templates/Dockerfile` & `mobio-cli-1.0.6/mobio_cli/templates/Dockerfile`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.5/mobio_cli/templates/Dockerfile-release` & `mobio-cli-1.0.6/mobio_cli/templates/Dockerfile-release`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.5/mobio_cli/templates/configs/__init__.{pymobio}` & `mobio-cli-1.0.6/mobio_cli/templates/configs/__init__.{pymobio}`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.5/mobio_cli/templates/k8s-Jenkinsfile` & `mobio-cli-1.0.6/mobio_cli/templates/k8s-Jenkinsfile`

 * *Files 6% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     }
 
     stage ('Run') {
       steps {
         script {
           if (env.BRANCH_NAME.toUpperCase() == "DEVELOP") {
             // apply các file yaml
-            sh ("find ./yaml -name '*.yaml' -type f -exec sed -i 's#{image}#${tagToDeploy}#g' {} ';' -exec kubectl -n mobio apply -f {} ';'")
+            sh  ("find ./yaml -type f -name '*.yaml' -exec sed -i 's#{image}#${tagToDeploy}#g; s#{image-monstache}#docker-registry.mobio.vn/mobio_monstache:6-V2#g' {} ';' -printf '%f\t%p\n' | sort -k1 | awk '{system(\"kubectl apply -n mobio -f \" \$2)}'")
             def is_used = true
             def unused_pods = [
             ]
             if (is_used == false) {
               echo "Khong su dung"
               sh ("find ./yaml -name '*.yaml' -type f -exec kubectl scale --replicas=0 -f {} -n mobio ';'")
             }
```

### Comparing `mobio-cli-1.0.5/mobio_cli/templates/resources/lang/message_en.json` & `mobio-cli-1.0.6/mobio_cli/templates/resources/lang/message_en.json`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.5/mobio_cli/templates/resources/lang/message_vi.json` & `mobio-cli-1.0.6/mobio_cli/templates/resources/lang/message_vi.json`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.5/mobio_cli/templates/src/apis/__init__.{pymobio}` & `mobio-cli-1.0.6/mobio_cli/templates/src/apis/__init__.{pymobio}`

 * *Files 17% similar despite different names*

```diff
@@ -4,27 +4,33 @@
     Date created: {#DATE_CREATED#}
 """
 
 from functools import wraps
 
 from flask import jsonify, Flask
 from mobio.libs.logging import MobioLogging, LoggingConstant
+from mobio.sdks.admin import MobioAdminSDK
 from mobio.sdks.base.common import CONSTANTS
 from mobio.sdks.base.common.lang_config import LangError
 from mobio.sdks.base.common.mobio_exception import BaseMoError, DBLogicError, InputNotFoundError, LogicSystemError, \
     ParamInvalidError, CustomError, CustomUnauthorizeError
 from mobio.sdks.base.common.system_config import SystemConfig
-from mobio.sdks.admin.http_jwt_auth import HttpJwtAuth
-from mobio.sdks.admin.mobio_authorization import MobioAuthorization
 
-from configs import {#PROJECT_NAME_CAMEL#}ApplicationConfig
+from configs import {#PROJECT_NAME_CAMEL#}ApplicationConfig, RedisConfig
 
 sys_conf = SystemConfig()
 app = Flask({#PROJECT_NAME_CAMEL#}ApplicationConfig.NAME, static_folder=None)
-auth = HttpJwtAuth(MobioAuthorization())
+MobioAdminSDK().config(
+    admin_host={#PROJECT_NAME_CAMEL#}ApplicationConfig.ADMIN_HOST,  # admin host (VD:https://api-test1.mobio.vn/)
+    redis_uri=RedisConfig.REDIS_URI,  # redis uri (VD: redis://redis-server:6378/0)
+    module_use="{#PROJECT_NAME_SNAKE_UPPERCASE#}",  # liên hệ admin để khai báo tên của module
+    module_encrypt="encypt_{#PROJECT_NAME_SNAKE_UPPERCASE#}",  # liên hệ admin để lấy mã
+    api_admin_version="api/v2.1",  # ["v1.0", "api/v2.0", "api/v2.1"]
+)
+auth = MobioAdminSDK().create_mobio_verify_token()
 
 
 class HTTP:
     class METHOD:
         DELETE = 'delete'
         PATCH = 'patch'
         PUT = 'put'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mobio-cli-1.0.5/mobio_cli/templates/startup.sh` & `mobio-cli-1.0.6/mobio_cli/templates/startup.sh`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.5/mobio_cli/templates/yaml/BASE/deploy_{#PROJECT_NAME_SNAKE_LOWERCASE#}_app_api.yaml` & `mobio-cli-1.0.6/mobio_cli/templates/yaml/BASE/deploy_{#PROJECT_NAME_SNAKE_LOWERCASE#}_app_api.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
    matchLabels:
      app: {#PROJECT_NAME_KEBAB_LOWERCASE#}-app-api
  template:
    metadata:
      labels:
        app: {#PROJECT_NAME_KEBAB_LOWERCASE#}-app-api
    spec:
+     serviceAccountName: mobio
      containers:
        - name: {#PROJECT_NAME_KEBAB_LOWERCASE#}
          image: {image}
          imagePullPolicy: IfNotPresent
          command: ["/bin/sh", "-c"]
          args: ["cd ${#PROJECT_NAME_SNAKE_UPPERCASE#}_HOME; sh prepare_env.sh && uwsgi --http :{#PROJECT_PORT#} --wsgi-file app_{#PROJECT_NAME_SNAKE_LOWERCASE#}_api.py --callable app --master --processes 4 -b 65536 --lazy --enable-threads"]
          envFrom:
@@ -42,14 +43,28 @@
              port: {#PROJECT_PORT#}
              path: /api/v1.0/ping
            initialDelaySeconds: 120
            periodSeconds: 5
            timeoutSeconds: 4
            successThreshold: 1
            failureThreshold: 3
+     initContainers:
+       - name: init-data-out
+         image: { image }
+         command: [ '/bin/sh', '-c', "cd ${#PROJECT_NAME_SNAKE_UPPERCASE#}_HOME; sh prepare_env.sh && sh check_image.sh" ]
+         envFrom:
+           - configMapRef:
+               name: mobio-config
+           - secretRef:
+               name: mobio-secret
+         volumeMounts:
+           - name: mobio-shared-data
+             mountPath: /media/data/resources/
+           - name: mobio-public-shared-data
+             mountPath: /media/data/public_resources/
      imagePullSecrets:
        - name: registrypullsecret
      volumes:
        - name: mobio-shared-data
          persistentVolumeClaim:
            claimName: mobio-resources-pvc
 ---
```

### Comparing `mobio-cli-1.0.5/mobio_cli.egg-info/SOURCES.txt` & `mobio-cli-1.0.6/mobio_cli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,26 @@
 mobio_cli.egg-info/dependency_links.txt
 mobio_cli.egg-info/entry_points.txt
 mobio_cli.egg-info/top_level.txt
 mobio_cli/templates/Dockerfile
 mobio_cli/templates/Dockerfile-release
 mobio_cli/templates/README.md
 mobio_cli/templates/app_{#PROJECT_NAME_SNAKE_LOWERCASE#}_api.{pymobio}
+mobio_cli/templates/check_image.sh
 mobio_cli/templates/k8s-Jenkinsfile
 mobio_cli/templates/prepare_env.sh
 mobio_cli/templates/requirements.txt
+mobio_cli/templates/script-update-version.sh
 mobio_cli/templates/startup.sh
 mobio_cli/templates/test.env
 mobio_cli/templates/configs/__init__.{pymobio}
 mobio_cli/templates/resources/configs/{#PROJECT_NAME_SNAKE_LOWERCASE#}.conf
 mobio_cli/templates/resources/lang/message_en.json
 mobio_cli/templates/resources/lang/message_vi.json
 mobio_cli/templates/src/__init__.{pymobio}
 mobio_cli/templates/src/apis/__init__.{pymobio}
 mobio_cli/templates/src/apis/v1_0/__init__.{pymobio}
 mobio_cli/templates/src/apis/v1_0/blueprints_api.{pymobio}
 mobio_cli/templates/src/common/__init__.{pymobio}
-mobio_cli/templates/src/controllers/empty
+mobio_cli/templates/src/controllers/example_controller.{pymobio}
+mobio_cli/templates/yaml/BASE/0_script_init_deploy.yaml
 mobio_cli/templates/yaml/BASE/deploy_{#PROJECT_NAME_SNAKE_LOWERCASE#}_app_api.yaml
```

### Comparing `mobio-cli-1.0.5/setup.py` & `mobio-cli-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             paths.append(os.path.join(path, filename))
     return paths
 
 
 data_files = package_data_files(os.path.join(__PACKAGE_NAME__, __TEMPLATE_DIR__))
 
 setup(name='mobio-cli',
-      version='1.0.5',
+      version='1.0.6',
       author='MOBIO',
       author_email='contact@mobio.vn',
       description='Command line create Mobio\'s projects',
       long_description=long_description,
       long_description_content_type='text/markdown',
       entry_points={
           'console_scripts': [
```

