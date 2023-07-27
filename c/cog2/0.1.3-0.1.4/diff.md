# Comparing `tmp/cog2-0.1.3.tar.gz` & `tmp/cog2-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cog2-0.1.3.tar", max compression
+gzip compressed data, was "cog2-0.1.4.tar", max compression
```

## Comparing `cog2-0.1.3.tar` & `cog2-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      471 2023-07-25 06:52:04.663746 cog2-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-24 00:37:04.090024 cog2-0.1.3/cog2/__init__.py
--rw-r--r--   0        0        0     2924 2023-07-25 06:50:39.421630 cog2-0.1.3/cog2/main.py
--rw-r--r--   0        0        0      427 2023-07-25 06:51:26.428115 cog2-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 cog2-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      471 2023-07-25 06:52:04.663746 cog2-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-24 00:37:04.090024 cog2-0.1.4/cog2/__init__.py
+-rw-r--r--   0        0        0     2916 2023-07-27 06:21:07.824353 cog2-0.1.4/cog2/main.py
+-rw-r--r--   0        0        0      427 2023-07-27 06:21:27.148232 cog2-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 cog2-0.1.4/PKG-INFO
```

### Comparing `cog2-0.1.3/cog2/main.py` & `cog2-0.1.4/cog2/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     )
     webbrowser.open("https://www.wizmodel.com/models")
     token = typer.prompt("Paste your token here and press Enter to login")
     data = {"token": token}
     response = requests.post(url="https://api.stagingwazs.online/cog/v1/verify-token", json=data).json()
     user_name = response['username']
     password = response['docker_token']
-    os.system("docker login -u {} -p {} registry.gpu-backend-prod.xyz".format(user_name, password))  # noqa: E501
+    os.system("docker login -u {} -p {} registry.wizmodel.com".format(user_name, password))  # noqa: E501
 
 
 @app.command()
 def build(
         tag: Annotated[str, typer.Option("--tag", "-t")] = "",
         no_cache: bool = typer.Option(False),
         separate_weights: bool = typer.Option(False),
```

### Comparing `cog2-0.1.3/PKG-INFO` & `cog2-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog2
-Version: 0.1.3
+Version: 0.1.4
 Summary: wizmodel.com cog2 sdk
 Author: incoming
 Author-email: 18320122+incomingflyingbrick@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

