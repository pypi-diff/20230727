# Comparing `tmp/spawn-lia-0.2.8.tar.gz` & `tmp/spawn-lia-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spawn-lia-0.2.8.tar", last modified: Wed Apr 19 19:36:45 2023, max compression
+gzip compressed data, was "spawn-lia-0.3.0.tar", last modified: Thu Jul 27 18:08:16 2023, max compression
```

## Comparing `spawn-lia-0.2.8.tar` & `spawn-lia-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,42 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/
--rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/LICENSE.txt
--rw-r--r--   0 developer  (1001) developer  (1001)     5125 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     4659 2023-04-19 19:34:22.000000 spawn-lia-0.2.8/README.md
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/__init__.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/bounty/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/bounty/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     4814 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/lia/bounty/heal.py
--rw-r--r--   0 developer  (1001) developer  (1001)      554 2023-04-15 20:42:23.000000 spawn-lia-0.2.8/lia/bounty/testing.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/conversation/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/conversation/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1028 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/lia/conversation/ask_to_proceed.py
--rw-r--r--   0 developer  (1001) developer  (1001)      103 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/conversation/decision.py
--rw-r--r--   0 developer  (1001) developer  (1001)      960 2023-04-15 20:42:23.000000 spawn-lia-0.2.8/lia/conversation/emojis.py
--rw-r--r--   0 developer  (1001) developer  (1001)      395 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/conversation/end_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)      506 2023-04-15 20:42:23.000000 spawn-lia-0.2.8/lia/conversation/get_input.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1015 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/conversation/start_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2218 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/conversation/virtualenv.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/git_operations/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/git_operations/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1546 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/lia/git_operations/push.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/lia/git_operations/verify_branch.py
--rw-r--r--   0 developer  (1001) developer  (1001)      608 2023-04-15 20:42:23.000000 spawn-lia-0.2.8/lia/main.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/simplify/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/simplify/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1768 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/lia/simplify/create_venv.py
--rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/simplify/verify_package.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/support/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/support/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1260 2023-04-15 19:23:40.000000 spawn-lia-0.2.8/lia/support/deploy.py
--rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/setup.cfg
--rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-19 19:36:35.000000 spawn-lia-0.2.8/setup.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/spawn_lia.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     5125 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)      894 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.8/tests/test_deploy.py
--rw-r--r--   0 developer  (1001) developer  (1001)     5114 2023-04-19 19:36:03.000000 spawn-lia-0.2.8/tests/test_git_operations.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1140 2023-04-12 17:06:07.000000 spawn-lia-0.2.8/tests/test_heal.py
--rw-r--r--   0 developer  (1001) developer  (1001)      885 2023-04-15 20:42:23.000000 spawn-lia-0.2.8/tests/test_venv.py
+drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/
+-rw-r--r--   0 dev       (1001) dev       (1001)    34693 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/LICENSE.txt
+-rw-r--r--   0 dev       (1001) dev       (1001)     5966 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/PKG-INFO
+-rw-r--r--   0 dev       (1001) dev       (1001)     5500 2023-07-27 17:55:35.000000 spawn-lia-0.3.0/README.md
+drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/lia/
+-rw-r--r--   0 dev       (1001) dev       (1001)        0 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/__init__.py
+drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/lia/bounty/
+-rw-r--r--   0 dev       (1001) dev       (1001)        0 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/bounty/__init__.py
+-rw-r--r--   0 dev       (1001) dev       (1001)     4814 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/bounty/heal.py
+-rw-r--r--   0 dev       (1001) dev       (1001)      554 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/bounty/testing.py
+drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/lia/conversation/
+-rw-r--r--   0 dev       (1001) dev       (1001)        0 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/conversation/__init__.py
+-rw-r--r--   0 dev       (1001) dev       (1001)     1028 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/conversation/ask_to_proceed.py
+-rw-r--r--   0 dev       (1001) dev       (1001)      103 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/conversation/decision.py
+-rw-r--r--   0 dev       (1001) dev       (1001)      960 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/conversation/emojis.py
+-rw-r--r--   0 dev       (1001) dev       (1001)      395 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/conversation/end_message.py
+-rw-r--r--   0 dev       (1001) dev       (1001)      506 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/conversation/get_input.py
+-rw-r--r--   0 dev       (1001) dev       (1001)     1020 2023-07-27 18:08:09.000000 spawn-lia-0.3.0/lia/conversation/start_message.py
+drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/lia/git_operations/
+-rw-r--r--   0 dev       (1001) dev       (1001)        0 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/git_operations/__init__.py
+-rw-r--r--   0 dev       (1001) dev       (1001)     1546 2023-07-26 21:19:00.000000 spawn-lia-0.3.0/lia/git_operations/push.py
+-rw-r--r--   0 dev       (1001) dev       (1001)     1486 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/git_operations/verify_branch.py
+-rw-r--r--   0 dev       (1001) dev       (1001)      527 2023-07-27 17:55:59.000000 spawn-lia-0.3.0/lia/main.py
+drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/lia/simplify/
+-rw-r--r--   0 dev       (1001) dev       (1001)        0 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/simplify/__init__.py
+-rw-r--r--   0 dev       (1001) dev       (1001)      246 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/simplify/verify_package.py
+drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/lia/support/
+-rw-r--r--   0 dev       (1001) dev       (1001)        0 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/support/__init__.py
+-rw-r--r--   0 dev       (1001) dev       (1001)     1260 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/lia/support/deploy.py
+-rw-r--r--   0 dev       (1001) dev       (1001)       38 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/setup.cfg
+-rw-r--r--   0 dev       (1001) dev       (1001)     1156 2023-07-27 18:07:48.000000 spawn-lia-0.3.0/setup.py
+drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/spawn_lia.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)     5966 2023-07-27 18:08:16.000000 spawn-lia-0.3.0/spawn_lia.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1001) dev       (1001)      816 2023-07-27 18:08:16.000000 spawn-lia-0.3.0/spawn_lia.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1001) dev       (1001)        1 2023-07-27 18:08:16.000000 spawn-lia-0.3.0/spawn_lia.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1001) dev       (1001)       40 2023-07-27 18:08:16.000000 spawn-lia-0.3.0/spawn_lia.egg-info/entry_points.txt
+-rw-r--r--   0 dev       (1001) dev       (1001)       96 2023-07-27 18:08:16.000000 spawn-lia-0.3.0/spawn_lia.egg-info/requires.txt
+-rw-r--r--   0 dev       (1001) dev       (1001)        4 2023-07-27 18:08:16.000000 spawn-lia-0.3.0/spawn_lia.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1001) dev       (1001)        0 2023-07-27 18:08:16.513582 spawn-lia-0.3.0/tests/
+-rw-r--r--   0 dev       (1001) dev       (1001)      626 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/tests/test_deploy.py
+-rw-r--r--   0 dev       (1001) dev       (1001)     5184 2023-07-27 17:58:52.000000 spawn-lia-0.3.0/tests/test_git_operations.py
+-rw-r--r--   0 dev       (1001) dev       (1001)     1140 2023-07-25 17:45:36.000000 spawn-lia-0.3.0/tests/test_heal.py
```

### Comparing `spawn-lia-0.2.8/LICENSE.txt` & `spawn-lia-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.8/PKG-INFO` & `spawn-lia-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,48 @@
-Metadata-Version: 2.1
-Name: spawn-lia
-Version: 0.2.8
-Summary: The most wanted support
-Home-page: https://codeberg.org/cap_jmk/lia
-Author: Julian M. Kleber
-Author-email: julian.kleber@sail.black
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# lia
+# 1. lia
 
 [![Downloads](https://static.pepy.tech/personalized-badge/spawn-lia?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/spawn-lia)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20-blue)
 ![Style Black](https://warehouse-camo.ingress.cmh1.psfhosted.org/fbfdc7754183ecf079bc71ddeabaf88f6cbc5c00/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667)
 [![PyPI - Version](https://img.shields.io/pypi/v/spawn-lia.svg)](https://pypi.org/project/spawn-lia)
 
-![Lia](lia.jpg)
+![Lia](lia_2_sunglasses.png)
 
 -----
-
 **Table of Contents**
+- [1. lia](#1-lia)
+  - [1.1. Why?](#11-why)
+  - [1.2. What?](#12-what)
+  - [1.3. Lia](#13-lia)
+  - [1.4. Installation](#14-installation)
+  - [1.5. Usage](#15-usage)
+    - [1.5.1. CI](#151-ci)
+    - [1.5.2. CI in container](#152-ci-in-container)
+    - [1.5.3. About Testing](#153-about-testing)
+    - [1.5.4. Deployments](#154-deployments)
+    - [1.5.5. Git operations](#155-git-operations)
+- [Successes](#successes)
+- [2. Support the Development](#2-support-the-development)
 
-<!-- TOC -->
-- [1. Why?](#1-why)
-- [2. What?](#2-what)
-- [3. Lia](#3-lia)
-- [4. Installation](#4-installation)
-- [5. Usage](#5-usage)
-- [6. # Deployments](#6--deployments)
-    - [6.1. Git operations](#61-git-operations)
-<!-- /TOC -->
 
-## 1. Why?
+
+## 1.1. Why?
 
 Remember code is poetry. And we write our own story. And for this, we need a support.
 
 Without a support, all your efforts will fail. A support takes care we do all the necessary things we would not find time during battles. We need a support. So we asked `lia` to join us.
 
 She protects us from malicious adversaries, and heals our organization by making our poetry better and thereby our story.
 
-## 2. What?
+## 1.2. What?
 
 `lia` is the best support you can hope for. She helps us to maintain our ship, fight enemies, and win customers.
 
-## 3. Lia
+## 1.3. Lia
 
 Why did we name the package `lia`?
 
 As a short form of Elisabeth, Lia means "God is fullness", "God is my oath" or "God swears". From Amilia Lia gets the meanings "the zealous", "the imitator" or "the competitor" and from Julia "from the family of the Julii" or "consecrated to Jupiter". Lia is also the Irish word for "healer".
 
 All other meanings do not matter in this context whatsoever.
 
@@ -64,15 +54,15 @@
 
 If you read through books about Agile Development, Refactoring and Clean Coding you maybe realize that security, value generation, and awesome products do have a lot to do with these books. `Thus, true developers have one common enemy: The Fel.` 
 
 We hope the tool brings you joy in winning your daily battles against the Fel. 
 
 We built for a better future. And we are excited what the future has prepared for us. ⛵
 
-## 4. Installation
+## 1.4. Installation
 
 ```bash
 pip install spawn-lia
 ```
 
 If you want to get really fancy (it really makes a lot more fun) create an alias for `pip install`
 
@@ -94,58 +84,68 @@
 
 Then finally,
 
 ```bash
 cast spawn-lia
 ```
 
-## 5. Usage
+## 1.5. Usage
 
 To get general information about the spells `lia` has to offer run the plain command
 
 ```bash
 lia
 ```
 
-### CI 
+### 1.5.1. CI 
 
 To improve the quality of your package and doing local CI do:
 
 ```bash
 lia heal package
 ```
 
 Do not be afraid you will probably see many errors. This behavior is intended and shall raise your attention to all sorts of errors, bugs, technical debt and antipatterns in your code.
 
 Getting rid of everything may be tedious but it is doable. We are going through the same process. It improved everything for us.
 
 If you need more information about typing, then the `mypy` [documentation](https://mypy.readthedocs.io/en/stable/getting_started.html) is a great place to start.
 
-### CI in container
+### 1.5.2. CI in container
 
 For all remote CI systems like Drone CI, Woodpecker, Actions, etc. 
 
 ```bash
 lia heal package
 ```
 
-### 5.1. Deployments
+### 1.5.3. About Testing
+
+We recommend to use `unittest` instead of `pytest`. There is a bug such that pytests are now running very slow. Lia is compatible with both
+
+### 1.5.4. Deployments
 
 To deploy you package do
 
 
 ```bash
 lia deploy package 
 ```
 
-### 5.2. Git operations 
+### 1.5.5. Git operations 
 
 ```bash
 lia push origin_name
 ```
 where origin name is the name of your remote, e.g. `origin`
 
-# Support the Development
+# Successes 
+
+Our now deprecated venv mechanics are implemented into Debian 12. Here we clearly demonstrated how our philosphy of free software accelerates businesses all around the world.
+
+It feels nice to have so many supporters and we thus continue with the project and are happy that the virtual environments are handled by someone else at the right point of the operating system.
+
+# 2. Support the Development
 
 To support the development you can
 
 <a href="https://www.buymeacoffee.com/capjmk" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
```

### Comparing `spawn-lia-0.2.8/README.md` & `spawn-lia-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,62 @@
-# lia
+Metadata-Version: 2.1
+Name: spawn-lia
+Version: 0.3.0
+Summary: The most wanted support
+Home-page: https://codeberg.org/cap_jmk/lia
+Author: Julian M. Kleber
+Author-email: julian.kleber@sail.black
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# 1. lia
 
 [![Downloads](https://static.pepy.tech/personalized-badge/spawn-lia?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/spawn-lia)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20-blue)
 ![Style Black](https://warehouse-camo.ingress.cmh1.psfhosted.org/fbfdc7754183ecf079bc71ddeabaf88f6cbc5c00/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667)
 [![PyPI - Version](https://img.shields.io/pypi/v/spawn-lia.svg)](https://pypi.org/project/spawn-lia)
 
-![Lia](lia.jpg)
+![Lia](lia_2_sunglasses.png)
 
 -----
-
 **Table of Contents**
+- [1. lia](#1-lia)
+  - [1.1. Why?](#11-why)
+  - [1.2. What?](#12-what)
+  - [1.3. Lia](#13-lia)
+  - [1.4. Installation](#14-installation)
+  - [1.5. Usage](#15-usage)
+    - [1.5.1. CI](#151-ci)
+    - [1.5.2. CI in container](#152-ci-in-container)
+    - [1.5.3. About Testing](#153-about-testing)
+    - [1.5.4. Deployments](#154-deployments)
+    - [1.5.5. Git operations](#155-git-operations)
+- [Successes](#successes)
+- [2. Support the Development](#2-support-the-development)
 
-<!-- TOC -->
-- [1. Why?](#1-why)
-- [2. What?](#2-what)
-- [3. Lia](#3-lia)
-- [4. Installation](#4-installation)
-- [5. Usage](#5-usage)
-- [6. # Deployments](#6--deployments)
-    - [6.1. Git operations](#61-git-operations)
-<!-- /TOC -->
 
-## 1. Why?
+
+## 1.1. Why?
 
 Remember code is poetry. And we write our own story. And for this, we need a support.
 
 Without a support, all your efforts will fail. A support takes care we do all the necessary things we would not find time during battles. We need a support. So we asked `lia` to join us.
 
 She protects us from malicious adversaries, and heals our organization by making our poetry better and thereby our story.
 
-## 2. What?
+## 1.2. What?
 
 `lia` is the best support you can hope for. She helps us to maintain our ship, fight enemies, and win customers.
 
-## 3. Lia
+## 1.3. Lia
 
 Why did we name the package `lia`?
 
 As a short form of Elisabeth, Lia means "God is fullness", "God is my oath" or "God swears". From Amilia Lia gets the meanings "the zealous", "the imitator" or "the competitor" and from Julia "from the family of the Julii" or "consecrated to Jupiter". Lia is also the Irish word for "healer".
 
 All other meanings do not matter in this context whatsoever.
 
@@ -50,15 +68,15 @@
 
 If you read through books about Agile Development, Refactoring and Clean Coding you maybe realize that security, value generation, and awesome products do have a lot to do with these books. `Thus, true developers have one common enemy: The Fel.` 
 
 We hope the tool brings you joy in winning your daily battles against the Fel. 
 
 We built for a better future. And we are excited what the future has prepared for us. ⛵
 
-## 4. Installation
+## 1.4. Installation
 
 ```bash
 pip install spawn-lia
 ```
 
 If you want to get really fancy (it really makes a lot more fun) create an alias for `pip install`
 
@@ -80,58 +98,68 @@
 
 Then finally,
 
 ```bash
 cast spawn-lia
 ```
 
-## 5. Usage
+## 1.5. Usage
 
 To get general information about the spells `lia` has to offer run the plain command
 
 ```bash
 lia
 ```
 
-### CI 
+### 1.5.1. CI 
 
 To improve the quality of your package and doing local CI do:
 
 ```bash
 lia heal package
 ```
 
 Do not be afraid you will probably see many errors. This behavior is intended and shall raise your attention to all sorts of errors, bugs, technical debt and antipatterns in your code.
 
 Getting rid of everything may be tedious but it is doable. We are going through the same process. It improved everything for us.
 
 If you need more information about typing, then the `mypy` [documentation](https://mypy.readthedocs.io/en/stable/getting_started.html) is a great place to start.
 
-### CI in container
+### 1.5.2. CI in container
 
 For all remote CI systems like Drone CI, Woodpecker, Actions, etc. 
 
 ```bash
 lia heal package
 ```
 
-### 5.1. Deployments
+### 1.5.3. About Testing
+
+We recommend to use `unittest` instead of `pytest`. There is a bug such that pytests are now running very slow. Lia is compatible with both
+
+### 1.5.4. Deployments
 
 To deploy you package do
 
 
 ```bash
 lia deploy package 
 ```
 
-### 5.2. Git operations 
+### 1.5.5. Git operations 
 
 ```bash
 lia push origin_name
 ```
 where origin name is the name of your remote, e.g. `origin`
 
-# Support the Development
+# Successes 
+
+Our now deprecated venv mechanics are implemented into Debian 12. Here we clearly demonstrated how our philosphy of free software accelerates businesses all around the world.
+
+It feels nice to have so many supporters and we thus continue with the project and are happy that the virtual environments are handled by someone else at the right point of the operating system.
+
+# 2. Support the Development
 
 To support the development you can
 
 <a href="https://www.buymeacoffee.com/capjmk" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
```

### Comparing `spawn-lia-0.2.8/lia/bounty/heal.py` & `spawn-lia-0.3.0/lia/bounty/heal.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.8/lia/bounty/testing.py` & `spawn-lia-0.3.0/lia/bounty/testing.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.8/lia/conversation/ask_to_proceed.py` & `spawn-lia-0.3.0/lia/conversation/ask_to_proceed.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.8/lia/conversation/emojis.py` & `spawn-lia-0.3.0/lia/conversation/emojis.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.8/lia/conversation/start_message.py` & `spawn-lia-0.3.0/lia/conversation/start_message.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,10 +35,11 @@
     :doc-author: Julian M. Kleber
     """
 
     message = (
         f"{anatomical_heart} Lia is an open-source CI/CD tool\n"
         f"that eliminates the Fel {mechanical_arm}\n"
         f"Copyright © 2023 Soul Twin Studios {call_me_hand}\n"
-        f"A subsidiary of SailBlack Inc. {sailing_ship}"
+        f"A brand of sail.black {sailing_ship}"
+        f"\n"
     )
     return message
```

### Comparing `spawn-lia-0.2.8/lia/git_operations/push.py` & `spawn-lia-0.3.0/lia/git_operations/push.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.8/lia/git_operations/verify_branch.py` & `spawn-lia-0.3.0/lia/git_operations/verify_branch.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.8/lia/main.py` & `spawn-lia-0.3.0/lia/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 import click
 
 
 # spells
 from lia.bounty.heal import heal, heal_file
 from lia.support.deploy import deploy
-from lia.simplify.create_venv import create_venv
 from lia.git_operations.push import push
 
 
 @click.group()
 def spells() -> None:
     """Collection for Lia's spells.
 
@@ -20,12 +19,11 @@
     """
     pass  # pragma: no cover
 
 
 spells.add_command(heal)
 spells.add_command(heal_file)
 spells.add_command(deploy)
-spells.add_command(create_venv)
 spells.add_command(push)
 
 if __name__ == "__main__":
     spells()
```

### Comparing `spawn-lia-0.2.8/lia/support/deploy.py` & `spawn-lia-0.3.0/lia/support/deploy.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.8/setup.py` & `spawn-lia-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="spawn-lia",
-    version="0.2.8",
+    version="0.3.0",
     packages=find_packages(include=["lia*"]),
     include_package_data=True,
     install_requires=[
         "Click",
         "black",
         "autopep8",
         "mypy",
```

### Comparing `spawn-lia-0.2.8/spawn_lia.egg-info/PKG-INFO` & `spawn-lia-0.3.0/spawn_lia.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 Metadata-Version: 2.1
 Name: spawn-lia
-Version: 0.2.8
+Version: 0.3.0
 Summary: The most wanted support
 Home-page: https://codeberg.org/cap_jmk/lia
 Author: Julian M. Kleber
 Author-email: julian.kleber@sail.black
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# lia
+# 1. lia
 
 [![Downloads](https://static.pepy.tech/personalized-badge/spawn-lia?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/spawn-lia)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20-blue)
 ![Style Black](https://warehouse-camo.ingress.cmh1.psfhosted.org/fbfdc7754183ecf079bc71ddeabaf88f6cbc5c00/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667)
 [![PyPI - Version](https://img.shields.io/pypi/v/spawn-lia.svg)](https://pypi.org/project/spawn-lia)
 
-![Lia](lia.jpg)
+![Lia](lia_2_sunglasses.png)
 
 -----
-
 **Table of Contents**
+- [1. lia](#1-lia)
+  - [1.1. Why?](#11-why)
+  - [1.2. What?](#12-what)
+  - [1.3. Lia](#13-lia)
+  - [1.4. Installation](#14-installation)
+  - [1.5. Usage](#15-usage)
+    - [1.5.1. CI](#151-ci)
+    - [1.5.2. CI in container](#152-ci-in-container)
+    - [1.5.3. About Testing](#153-about-testing)
+    - [1.5.4. Deployments](#154-deployments)
+    - [1.5.5. Git operations](#155-git-operations)
+- [Successes](#successes)
+- [2. Support the Development](#2-support-the-development)
+
 
-<!-- TOC -->
-- [1. Why?](#1-why)
-- [2. What?](#2-what)
-- [3. Lia](#3-lia)
-- [4. Installation](#4-installation)
-- [5. Usage](#5-usage)
-- [6. # Deployments](#6--deployments)
-    - [6.1. Git operations](#61-git-operations)
-<!-- /TOC -->
 
-## 1. Why?
+## 1.1. Why?
 
 Remember code is poetry. And we write our own story. And for this, we need a support.
 
 Without a support, all your efforts will fail. A support takes care we do all the necessary things we would not find time during battles. We need a support. So we asked `lia` to join us.
 
 She protects us from malicious adversaries, and heals our organization by making our poetry better and thereby our story.
 
-## 2. What?
+## 1.2. What?
 
 `lia` is the best support you can hope for. She helps us to maintain our ship, fight enemies, and win customers.
 
-## 3. Lia
+## 1.3. Lia
 
 Why did we name the package `lia`?
 
 As a short form of Elisabeth, Lia means "God is fullness", "God is my oath" or "God swears". From Amilia Lia gets the meanings "the zealous", "the imitator" or "the competitor" and from Julia "from the family of the Julii" or "consecrated to Jupiter". Lia is also the Irish word for "healer".
 
 All other meanings do not matter in this context whatsoever.
 
@@ -64,15 +68,15 @@
 
 If you read through books about Agile Development, Refactoring and Clean Coding you maybe realize that security, value generation, and awesome products do have a lot to do with these books. `Thus, true developers have one common enemy: The Fel.` 
 
 We hope the tool brings you joy in winning your daily battles against the Fel. 
 
 We built for a better future. And we are excited what the future has prepared for us. ⛵
 
-## 4. Installation
+## 1.4. Installation
 
 ```bash
 pip install spawn-lia
 ```
 
 If you want to get really fancy (it really makes a lot more fun) create an alias for `pip install`
 
@@ -94,58 +98,68 @@
 
 Then finally,
 
 ```bash
 cast spawn-lia
 ```
 
-## 5. Usage
+## 1.5. Usage
 
 To get general information about the spells `lia` has to offer run the plain command
 
 ```bash
 lia
 ```
 
-### CI 
+### 1.5.1. CI 
 
 To improve the quality of your package and doing local CI do:
 
 ```bash
 lia heal package
 ```
 
 Do not be afraid you will probably see many errors. This behavior is intended and shall raise your attention to all sorts of errors, bugs, technical debt and antipatterns in your code.
 
 Getting rid of everything may be tedious but it is doable. We are going through the same process. It improved everything for us.
 
 If you need more information about typing, then the `mypy` [documentation](https://mypy.readthedocs.io/en/stable/getting_started.html) is a great place to start.
 
-### CI in container
+### 1.5.2. CI in container
 
 For all remote CI systems like Drone CI, Woodpecker, Actions, etc. 
 
 ```bash
 lia heal package
 ```
 
-### 5.1. Deployments
+### 1.5.3. About Testing
+
+We recommend to use `unittest` instead of `pytest`. There is a bug such that pytests are now running very slow. Lia is compatible with both
+
+### 1.5.4. Deployments
 
 To deploy you package do
 
 
 ```bash
 lia deploy package 
 ```
 
-### 5.2. Git operations 
+### 1.5.5. Git operations 
 
 ```bash
 lia push origin_name
 ```
 where origin name is the name of your remote, e.g. `origin`
 
-# Support the Development
+# Successes 
+
+Our now deprecated venv mechanics are implemented into Debian 12. Here we clearly demonstrated how our philosphy of free software accelerates businesses all around the world.
+
+It feels nice to have so many supporters and we thus continue with the project and are happy that the virtual environments are handled by someone else at the right point of the operating system.
+
+# 2. Support the Development
 
 To support the development you can
 
 <a href="https://www.buymeacoffee.com/capjmk" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
```

### Comparing `spawn-lia-0.2.8/spawn_lia.egg-info/SOURCES.txt` & `spawn-lia-0.3.0/spawn_lia.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,23 @@
 lia/conversation/__init__.py
 lia/conversation/ask_to_proceed.py
 lia/conversation/decision.py
 lia/conversation/emojis.py
 lia/conversation/end_message.py
 lia/conversation/get_input.py
 lia/conversation/start_message.py
-lia/conversation/virtualenv.py
 lia/git_operations/__init__.py
 lia/git_operations/push.py
 lia/git_operations/verify_branch.py
 lia/simplify/__init__.py
-lia/simplify/create_venv.py
 lia/simplify/verify_package.py
 lia/support/__init__.py
 lia/support/deploy.py
 spawn_lia.egg-info/PKG-INFO
 spawn_lia.egg-info/SOURCES.txt
 spawn_lia.egg-info/dependency_links.txt
 spawn_lia.egg-info/entry_points.txt
 spawn_lia.egg-info/requires.txt
 spawn_lia.egg-info/top_level.txt
 tests/test_deploy.py
 tests/test_git_operations.py
-tests/test_heal.py
-tests/test_venv.py
+tests/test_heal.py
```

### Comparing `spawn-lia-0.2.8/tests/test_deploy.py` & `spawn-lia-0.3.0/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.8/tests/test_git_operations.py` & `spawn-lia-0.3.0/tests/test_git_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,16 +113,18 @@
     subprocess.run(["git checkout dev"], shell=True, check=True)
    """  # -> can only implement after merge
 
 def test_push(): 
 
     #switch to temporary branch to avoid contaminations
     subprocess.run(["git checkout dev"], check = True, shell=True)
-    subprocess.run(["git branch -D test_branch"], check = True, shell = True)
-
+    try:
+        subprocess.run(["git branch -D test_branch"], check = True, shell = True)
+    except: 
+        print("No branch test-branch found")
     out = subprocess.run(["git status"], check=True, shell=True, capture_output=True)
     out2 = subprocess.run(["git branch"], check=True, shell=True, capture_output=True)
     if b"On branch test_branch" not in out.stdout:
         if "test_branch" not in out2.stdout.decode("utf-8"):
             subprocess.run(["git checkout -b test_branch"], check=True, shell=True)
         else: 
             subprocess.run(["git checkout test_branch"], check=True, shell=True)
```

### Comparing `spawn-lia-0.2.8/tests/test_heal.py` & `spawn-lia-0.3.0/tests/test_heal.py`

 * *Files identical despite different names*

