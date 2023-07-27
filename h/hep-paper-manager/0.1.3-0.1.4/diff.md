# Comparing `tmp/hep_paper_manager-0.1.3.tar.gz` & `tmp/hep_paper_manager-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hep_paper_manager-0.1.3.tar", max compression
+gzip compressed data, was "hep_paper_manager-0.1.4.tar", max compression
```

## Comparing `hep_paper_manager-0.1.3.tar` & `hep_paper_manager-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1064 2023-06-22 07:10:17.667054 hep_paper_manager-0.1.3/LICENSE
--rw-r--r--   0        0        0     3770 2023-06-23 10:34:03.963586 hep_paper_manager-0.1.3/README.md
--rw-r--r--   0        0        0      366 2023-06-23 10:34:03.964059 hep_paper_manager-0.1.3/hpm/__init__.py
--rw-r--r--   0        0        0     5864 2023-06-23 10:33:43.459023 hep_paper_manager-0.1.3/hpm/cli.py
--rw-r--r--   0        0        0       29 2023-06-13 04:12:40.062240 hep_paper_manager-0.1.3/hpm/engines/__init__.py
--rw-r--r--   0        0        0     3648 2023-06-22 07:01:11.908415 hep_paper_manager-0.1.3/hpm/engines/inspire.py
--rw-r--r--   0        0        0       27 2023-06-13 04:13:59.907266 hep_paper_manager-0.1.3/hpm/notion/__init__.py
--rw-r--r--   0        0        0     3427 2023-06-18 11:18:06.400535 hep_paper_manager-0.1.3/hpm/notion/client.py
--rw-r--r--   0        0        0       54 2023-06-13 04:13:42.598101 hep_paper_manager-0.1.3/hpm/notion/objects/__init__.py
--rw-r--r--   0        0        0      962 2023-06-13 04:13:47.941688 hep_paper_manager-0.1.3/hpm/notion/objects/database.py
--rw-r--r--   0        0        0     3682 2023-06-23 10:04:15.831479 hep_paper_manager-0.1.3/hpm/notion/objects/page.py
--rw-r--r--   0        0        0     5470 2023-06-23 10:33:43.460062 hep_paper_manager-0.1.3/hpm/notion/properties.py
--rw-r--r--   0        0        0      215 2023-06-22 07:01:11.909628 hep_paper_manager-0.1.3/hpm/templates/paper.yml
--rw-r--r--   0        0        0      698 2023-06-23 10:34:03.964999 hep_paper_manager-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 hep_paper_manager-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-22 07:10:17.000000 hep_paper_manager-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3873 2023-07-27 13:23:13.543527 hep_paper_manager-0.1.4/README.md
+-rw-r--r--   0        0        0      366 2023-07-27 13:55:59.615072 hep_paper_manager-0.1.4/hpm/__init__.py
+-rw-r--r--   0        0        0     7179 2023-07-27 13:22:36.023359 hep_paper_manager-0.1.4/hpm/cli.py
+-rw-r--r--   0        0        0       29 2023-06-13 04:12:40.000000 hep_paper_manager-0.1.4/hpm/engines/__init__.py
+-rw-r--r--   0        0        0     3648 2023-06-22 07:01:11.000000 hep_paper_manager-0.1.4/hpm/engines/inspire.py
+-rw-r--r--   0        0        0       27 2023-06-13 04:13:59.000000 hep_paper_manager-0.1.4/hpm/notion/__init__.py
+-rw-r--r--   0        0        0     3427 2023-07-27 13:47:52.607583 hep_paper_manager-0.1.4/hpm/notion/client.py
+-rw-r--r--   0        0        0       54 2023-06-13 04:13:42.000000 hep_paper_manager-0.1.4/hpm/notion/objects/__init__.py
+-rw-r--r--   0        0        0      962 2023-06-13 04:13:47.000000 hep_paper_manager-0.1.4/hpm/notion/objects/database.py
+-rw-r--r--   0        0        0     3682 2023-06-23 10:04:15.000000 hep_paper_manager-0.1.4/hpm/notion/objects/page.py
+-rw-r--r--   0        0        0     5470 2023-06-23 10:33:43.000000 hep_paper_manager-0.1.4/hpm/notion/properties.py
+-rw-r--r--   0        0        0      215 2023-06-22 07:01:11.000000 hep_paper_manager-0.1.4/hpm/templates/paper.yml
+-rw-r--r--   0        0        0      720 2023-07-27 13:55:59.615249 hep_paper_manager-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 hep_paper_manager-0.1.4/PKG-INFO
```

### Comparing `hep_paper_manager-0.1.3/LICENSE` & `hep_paper_manager-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.3/README.md` & `hep_paper_manager-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,17 @@
     abstract: Abstract
     url: URL
     bibtex: Bibtex
     source: Source
   ```
 
 ## Updates
+### v0.1.4
+- Update print style.
+- Add friendly error message when the `database_id` is not specified.
 ### v0.1.3
 - Update `hpm add` to check if the paper already exists in the database.
 - You can now create a database with more properties then the template.
 ### v0.1.2
 - Update paper from Inspire engine to include url, bibtex, and source. 
 ### v0.1.1
 - Add `hpm init` for interactive setup.
```

### Comparing `hep_paper_manager-0.1.3/hpm/cli.py` & `hep_paper_manager-0.1.4/hpm/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import shutil
 from importlib import import_module
 from pathlib import Path
 from typing import Optional
 
 import typer
 import yaml
-from rich import print
+from rich.console import Console
+from rich.prompt import Confirm, Prompt
+from rich.theme import Theme
 from typing_extensions import Annotated
 
 from hpm import APP_DIR, CACHE_DIR, TEMPLATE_DIR
 from hpm.notion.client import Client
 from hpm.notion.objects import Database, Page
 from hpm.notion.properties import *
 
@@ -17,70 +19,102 @@
 
 # ---------------------------------------------------------------------------- #
 app = typer.Typer(
     context_settings={"help_option_names": ["-h", "--help"]},
     add_completion=False,
 )
 
+console = Console(
+    theme=Theme(
+        {
+            "sect": "bold white",  # section
+            "info": "bold blue",  # informatiom
+            "done": "bold green",  # done
+            "ques": "bold yellow",  # question
+            "error": "bold red",  # error
+            "warn": "yellow",  # warning
+            "path": "cyan underline",  # path
+            "number": "cyan",  # number
+        },
+        inherit=False,
+    )
+)
+
 
 @app.command(help="Initialize hpm with the Notion API token")
 def init():
-    print("Welcome to the HEP Paper Manager!\n")
-    print("Before we start, let's set up a few necessary configurations.\n")
-    token = typer.prompt("Enter your Notion API token", hide_input=True)
+    console.print("Welcome to the HEP Paper Manager!\n")
+    console.print("Before we start, let's set up a few necessary configurations.\n")
+    token = Prompt.ask("[ques]?[/ques] Enter your Notion API token", console=console, password=True)
     token_file = APP_DIR / "auth.yml"
     with open(token_file, "w") as f:
         yaml.dump({"token": token}, f)
-    print(f"[green]Your token has been saved in {token_file}\n")
+    console.print(f"[done]✔️[/done] Your token has been saved in {token_file}\n")
 
-    use_template = typer.confirm("Would you like to use the default paper template?", default=True)
+    use_template = Confirm.ask(
+        "[ques]?[/ques] Would you like to use the default paper template?",
+        console=console,
+        default=True,
+    )
     if use_template:
         paper_template = Path(__file__).parent / "templates/paper.yml"
         shutil.copy(paper_template, TEMPLATE_DIR)
-        print(f"[green]The default template has been saved in {TEMPLATE_DIR}/paper.yml")
-        print("[yellow]Remember to add a database id to the template before using hpm!\n")
-
-    print("Configuration complete! Here are directories that hpm will use:")
-    print(f"1. App directory: {APP_DIR}")
-    print(f"2. Template directory: {TEMPLATE_DIR}")
-    print(f"3. Cache directory: {CACHE_DIR}")
+        console.print(
+            f"[done]✔️[/done] The default template has been saved in {TEMPLATE_DIR}/paper.yml"
+        )
+        console.print("[warn]Remember to add a database id to the template before using hpm!\n")
+
+    console.print("Configuration complete! Here are directories that hpm will use:")
+    console.print(f"1. App directory: {APP_DIR}")
+    console.print(f"2. Template directory: {TEMPLATE_DIR}")
+    console.print(f"3. Cache directory: {CACHE_DIR}")
 
 
 @app.command(help="Add a new page to a database")
 def add(template: str, parameters: str):
     token_file = APP_DIR / "auth.yml"
     with open(token_file, "r") as f:
         token = yaml.safe_load(f)["token"]
 
     # Create a Notion client
     client = Client(token)
 
     # Resolve the template and parameters
     parameters = parameters.split(",")
-    template = TEMPLATE_DIR / f"{template}.yml"
+    template_path = TEMPLATE_DIR / f"{template}.yml"
 
     # Load the template
-    with open(template, "r") as f:
+    with open(template_path, "r") as f:
         template = yaml.safe_load(f)
 
-    print(f"-> Launching {template['engine']}")
+    # Check if the database_id is specified in the template
+    database_id = template["database"]
+    if database_id == "<database_id>":
+        console.print(
+            f"[error]x[/error] Please specify a database id in [path]{template_path}[/path]"
+        )
+        raise typer.Exit(1)
+
+    console.print(f"[sect]>[/sect] Launching {template['engine']} engine")
     # Instantiate the engine
     engine = getattr(import_module("hpm.engines"), template["engine"])()
 
     # Unpack the parameters and pass them to the engine to get the results
     engine_results = engine.get(*parameters)
+    console.print(f"[done]✔️[/done] Engine launched\n")
 
-    print(f"-> Fetching database {template['database']}")
+    console.print(f"[sect]>[/sect] Fetching Notion database {template['database']}")
     # Get the database according to the template
     database_id = template["database"]
     retrieved_json = client.retrieve_database(database_id).json()
     queried_json = client.query_database(database_id).json()
     database = Database.from_dict(retrieved_json, queried_json)
+    console.print(f"[done]✔️[/done] Database fetched\n")
 
-    print(f"-> Creating page in database {database.title}")
+    console.print(f"[sect]>[/sect] Creating page in database {database.title}")
     # Loop over database properties
     # we need to get related database in DatabaseRelation, then extract its pages's title and id to a dictionary.
     # Then when creating a page with this property, we can find its id by its title.
     for name, prop in database.properties.items():
         if type(prop) == DatabaseRelation:
             related_database_id = prop.value
             retrieved_json = client.retrieve_database(related_database_id).json()
@@ -122,30 +156,30 @@
             if type(property) == Title:
                 page.title = getattr(engine_results, source)
             page.properties[target].value = getattr(engine_results, source)
 
     # Check if the page already exists
     for i in database.pages:
         if i.title == page.title:
-            print("[red]Page already exists!")
+            console.print("[error]![/error] Page already exists!")
             raise typer.Exit(code=1)
 
     # Create the page
     response = client.create_page(database_id, page.properties_to_dict())
     if response.status_code == 200:
-        print("[green]Page created successfully!")
+        console.print("[done]✔️[/done] Page created successfully!")
     else:
-        print("[red]Page creation failed!")
+        console.print("[error]x[/error] Page creation failed!")
         print(response.text)
         raise typer.Exit(code=1)
 
 
 def version_callback(value: bool):
     if value:
-        print(f"{__app_name__} v[yellow]{__app_version__}[/yellow]")
+        console.print(f"[bold]{__app_name__}[/bold] (version [number]{__app_version__}[/number])")
         raise typer.Exit()
 
 
 @app.callback()
 def main(
     version: Annotated[
         Optional[bool],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hep_paper_manager-0.1.3/hpm/engines/inspire.py` & `hep_paper_manager-0.1.4/hpm/engines/inspire.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.3/hpm/notion/client.py` & `hep_paper_manager-0.1.4/hpm/notion/client.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.3/hpm/notion/objects/database.py` & `hep_paper_manager-0.1.4/hpm/notion/objects/database.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.3/hpm/notion/objects/page.py` & `hep_paper_manager-0.1.4/hpm/notion/objects/page.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.3/hpm/notion/properties.py` & `hep_paper_manager-0.1.4/hpm/notion/properties.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.3/pyproject.toml` & `hep_paper_manager-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hep-paper-manager"
-version = "0.1.3"
+version = "0.1.4"
 description = "HPM is a command-line tool that adds High Energy Physics (HEP) papers to a Notion database."
 authors = ["Star9daisy <star9daisy@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "hpm" },
 ]
 
@@ -20,11 +20,12 @@
 pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
 python-dotenv = "^1.0.0"
 deptry = "^0.11.0"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hep_paper_manager-0.1.3/PKG-INFO` & `hep_paper_manager-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hep-paper-manager
-Version: 0.1.3
+Version: 0.1.4
 Summary: HPM is a command-line tool that adds High Energy Physics (HEP) papers to a Notion database.
 Author: Star9daisy
 Author-email: star9daisy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -93,14 +93,17 @@
     abstract: Abstract
     url: URL
     bibtex: Bibtex
     source: Source
   ```
 
 ## Updates
+### v0.1.4
+- Update print style.
+- Add friendly error message when the `database_id` is not specified.
 ### v0.1.3
 - Update `hpm add` to check if the paper already exists in the database.
 - You can now create a database with more properties then the template.
 ### v0.1.2
 - Update paper from Inspire engine to include url, bibtex, and source. 
 ### v0.1.1
 - Add `hpm init` for interactive setup.
```

