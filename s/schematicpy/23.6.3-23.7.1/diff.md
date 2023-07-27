# Comparing `tmp/schematicpy-23.6.3.tar.gz` & `tmp/schematicpy-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schematicpy-23.6.3.tar", max compression
+gzip compressed data, was "schematicpy-23.7.1.tar", max compression
```

## Comparing `schematicpy-23.6.3.tar` & `schematicpy-23.7.1.tar`

### file list

```diff
@@ -1,51 +1,53 @@
--rw-r--r--   0        0        0     1073 2023-06-23 16:44:42.610783 schematicpy-23.6.3/LICENSE
--rw-r--r--   0        0        0    16389 2023-06-23 16:44:42.610783 schematicpy-23.6.3/README.md
--rw-r--r--   0        0        0     3356 2023-06-23 16:45:16.994212 schematicpy-23.6.3/pyproject.toml
--rw-r--r--   0        0        0     1411 2023-06-23 16:44:42.614781 schematicpy-23.6.3/schematic/__init__.py
--rw-r--r--   0        0        0     1421 2023-06-23 16:44:42.614781 schematicpy-23.6.3/schematic/__main__.py
--rw-r--r--   0        0        0     4843 2023-06-23 16:44:42.614781 schematicpy-23.6.3/schematic/configuration.py
--rw-r--r--   0        0        0      663 2023-06-23 16:44:42.614781 schematicpy-23.6.3/schematic/etc/README.md
--rw-r--r--   0        0        0    76063 2023-06-23 16:44:42.614781 schematicpy-23.6.3/schematic/etc/data_models/biothings.model.jsonld
--rw-r--r--   0        0        0  1387510 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/etc/data_models/schema_org.model.jsonld
--rw-r--r--   0        0        0     4414 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/etc/validation_schemas/class.schema.json
--rw-r--r--   0        0        0     9914 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/etc/validation_schemas/model.schema.json
--rw-r--r--   0        0        0     5021 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/etc/validation_schemas/property.schema.json
--rw-r--r--   0        0        0     3129 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/exceptions.py
--rw-r--r--   0        0        0    10598 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/help.py
--rw-r--r--   0        0        0     3415 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/loader.py
--rw-r--r--   0        0        0       59 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/manifest/__init__.py
--rw-r--r--   0        0        0     9375 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/manifest/commands.py
--rw-r--r--   0        0        0    74507 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/manifest/generator.py
--rw-r--r--   0        0        0    22894 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/models/GE_Helpers.py
--rw-r--r--   0        0        0       52 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/models/__init__.py
--rw-r--r--   0        0        0     6912 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/models/commands.py
--rw-r--r--   0        0        0    16680 2023-06-23 16:44:42.618780 schematicpy-23.6.3/schematic/models/metadata.py
--rw-r--r--   0        0        0    44816 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/models/validate_attribute.py
--rw-r--r--   0        0        0    11604 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/models/validate_manifest.py
--rw-r--r--   0        0        0      166 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/schemas/__init__.py
--rw-r--r--   0        0        0     2470 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/schemas/commands.py
--rw-r--r--   0        0        0     4291 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/schemas/curie.py
--rw-r--r--   0        0        0    34388 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/schemas/df_parser.py
--rw-r--r--   0        0        0    46753 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/schemas/explorer.py
--rw-r--r--   0        0        0    30347 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/schemas/generator.py
--rw-r--r--   0        0        0     7100 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/schemas/validator.py
--rw-r--r--   0        0        0       96 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/store/__init__.py
--rw-r--r--   0        0        0      218 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/store/base.py
--rw-r--r--   0        0        0   113572 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/store/synapse.py
--rw-r--r--   0        0        0      787 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/__init__.py
--rw-r--r--   0        0        0     4765 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/cli_utils.py
--rw-r--r--   0        0        0     2785 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/curie_utils.py
--rw-r--r--   0        0        0     8086 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/df_utils.py
--rw-r--r--   0        0        0     6338 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/general.py
--rw-r--r--   0        0        0     8197 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/google_api_utils.py
--rw-r--r--   0        0        0     1148 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/io_utils.py
--rw-r--r--   0        0        0     9804 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/schema_utils.py
--rw-r--r--   0        0        0     9565 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/validate_rules_utils.py
--rw-r--r--   0        0        0     2629 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/validate_utils.py
--rw-r--r--   0        0        0      236 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/utils/viz_utils.py
--rw-r--r--   0        0        0      119 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/version.py
--rw-r--r--   0        0        0      135 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/visualization/__init__.py
--rw-r--r--   0        0        0    10207 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/visualization/attributes_explorer.py
--rw-r--r--   0        0        0     3480 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/visualization/commands.py
--rw-r--r--   0        0        0    37113 2023-06-23 16:44:42.622778 schematicpy-23.6.3/schematic/visualization/tangled_tree.py
--rw-r--r--   0        0        0    18820 1970-01-01 00:00:00.000000 schematicpy-23.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-27 16:28:02.621153 schematicpy-23.7.1/LICENSE
+-rw-r--r--   0        0        0    17198 2023-07-27 16:28:02.621153 schematicpy-23.7.1/README.md
+-rw-r--r--   0        0        0     3356 2023-07-27 16:28:37.349772 schematicpy-23.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1424 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/__init__.py
+-rw-r--r--   0        0        0     1421 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/configuration/__init__.py
+-rw-r--r--   0        0        0     6996 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/configuration/configuration.py
+-rw-r--r--   0        0        0     5034 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/configuration/dataclasses.py
+-rw-r--r--   0        0        0      663 2023-07-27 16:28:02.621153 schematicpy-23.7.1/schematic/etc/README.md
+-rw-r--r--   0        0        0    76063 2023-07-27 16:28:02.625153 schematicpy-23.7.1/schematic/etc/data_models/biothings.model.jsonld
+-rw-r--r--   0        0        0  1387510 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/etc/data_models/schema_org.model.jsonld
+-rw-r--r--   0        0        0     4414 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/etc/validation_schemas/class.schema.json
+-rw-r--r--   0        0        0     9914 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/etc/validation_schemas/model.schema.json
+-rw-r--r--   0        0        0     5021 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/etc/validation_schemas/property.schema.json
+-rw-r--r--   0        0        0     3193 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/exceptions.py
+-rw-r--r--   0        0        0    10581 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/help.py
+-rw-r--r--   0        0        0     3415 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/loader.py
+-rw-r--r--   0        0        0       59 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/manifest/__init__.py
+-rw-r--r--   0        0        0     9339 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/manifest/commands.py
+-rw-r--r--   0        0        0    77864 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/manifest/generator.py
+-rw-r--r--   0        0        0    22894 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/GE_Helpers.py
+-rw-r--r--   0        0        0       52 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/__init__.py
+-rw-r--r--   0        0        0     6616 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/commands.py
+-rw-r--r--   0        0        0    16680 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/metadata.py
+-rw-r--r--   0        0        0    44816 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/validate_attribute.py
+-rw-r--r--   0        0        0    11604 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/models/validate_manifest.py
+-rw-r--r--   0        0        0      166 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/__init__.py
+-rw-r--r--   0        0        0     2470 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/commands.py
+-rw-r--r--   0        0        0     4291 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/curie.py
+-rw-r--r--   0        0        0    34388 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/df_parser.py
+-rw-r--r--   0        0        0    46753 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/explorer.py
+-rw-r--r--   0        0        0    29741 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/generator.py
+-rw-r--r--   0        0        0     7070 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/schemas/validator.py
+-rw-r--r--   0        0        0       96 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/store/__init__.py
+-rw-r--r--   0        0        0      218 2023-07-27 16:28:02.629153 schematicpy-23.7.1/schematic/store/base.py
+-rw-r--r--   0        0        0   110877 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/store/synapse.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/__init__.py
+-rw-r--r--   0        0        0     2524 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/cli_utils.py
+-rw-r--r--   0        0        0     2785 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/curie_utils.py
+-rw-r--r--   0        0        0     8182 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/df_utils.py
+-rw-r--r--   0        0        0     6806 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/general.py
+-rw-r--r--   0        0        0     7338 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/google_api_utils.py
+-rw-r--r--   0        0        0     1140 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/io_utils.py
+-rw-r--r--   0        0        0     9804 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/schema_utils.py
+-rw-r--r--   0        0        0     9565 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/validate_rules_utils.py
+-rw-r--r--   0        0        0     2621 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/validate_utils.py
+-rw-r--r--   0        0        0      236 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/utils/viz_utils.py
+-rw-r--r--   0        0        0      119 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/version.py
+-rw-r--r--   0        0        0      135 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/visualization/__init__.py
+-rw-r--r--   0        0        0    10207 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/visualization/attributes_explorer.py
+-rw-r--r--   0        0        0     3548 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/visualization/commands.py
+-rw-r--r--   0        0        0    37113 2023-07-27 16:28:02.633153 schematicpy-23.7.1/schematic/visualization/tangled_tree.py
+-rw-r--r--   0        0        0    19629 1970-01-01 00:00:00.000000 schematicpy-23.7.1/PKG-INFO
```

### Comparing `schematicpy-23.6.3/LICENSE` & `schematicpy-23.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/README.md` & `schematicpy-23.7.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -84,53 +84,77 @@
 editor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section 
 
 *Note*: You could also visit [configparser](https://docs.python.org/3/library/configparser.html#module-configparser>) doc to see the format that `.synapseConfig` must have. For instance:
 >[authentication]<br> username = ABC <br> authtoken = abc
 
 <strong>Configure config.yml File</strong>
 
-*Note*: Below is only a brief explanation of some attributes in `config.yml`. <strong>Please use the link [here](https://github.com/Sage-Bionetworks/schematic/blob/develop/config.yml) to get the latest version of `config.yml` in `develop` branch</strong>.
+There are some defaults in schematic that can be configured. These fields are in ``config_example.yml``:
 
-Description of `config.yml` attributes
+```text
 
-    definitions:
-        synapse_config: "~/path/to/.synapseConfig"
-        service_acct_creds: "~/path/to/service_account_creds.json"
-
-    synapse:
-        master_fileview: "syn23643253" # fileview of project with datasets on Synapse
-        manifest_folder: "~/path/to/manifest_folder/" # manifests will be downloaded to this folder
-        manifest_basename: "filename" # base name of the manifest file in the project dataset, without extension
-        service_acct_creds: "syn25171627" # synapse ID of service_account_creds.json file
-
-    manifest:
-        title: "example" # title of metadata manifest file
-        # to make all manifests enter only 'all manifests'
-        data_type: 
-          - "Biospecimen"
-          - "Patient"
-
-    model:
-        input:
-            location: "data/schema_org_schemas/example.jsonld" # path to JSON-LD data model
-            file_type: "local" # only type "local" is supported currently
-    style: # configuration of google sheet
-        google_manifest:
-          req_bg_color:
-            red: 0.9215
-            green: 0.9725
-            blue: 0.9803
-          opt_bg_color:
-            red: 1.0
-            green: 1.0
-            blue: 0.9019
-          master_template_id: '1LYS5qE4nV9jzcYw5sXwCza25slDfRA1CIg3cs-hCdpU'
-          strict_validation: true
+# This is an example config for Schematic.
+# All listed values are those that are the default if a config is not used.
+# Save this as config.yml, this will be gitignored.
+# Remove any fields in the config you don't want to change
+# Change the values of any fields you do want to change
+
+
+# This describes where assets such as manifests are stored
+asset_store:
+  # This is when assets are stored in a synapse project
+  synapse:
+    # Synapse ID of the file view listing all project data assets.
+    master_fileview_id: "syn23643253"
+    # Path to the synapse config file, either absolute or relative to this file
+    config: ".synapseConfig"
+    # Base name that manifest files will be saved as
+    manifest_basename: "synapse_storage_manifest"
+
+# This describes information about manifests as it relates to generation and validation
+manifest:
+  # Location where manifests will saved to
+  manifest_folder: "manifests"
+  # Title or title prefix given to generated manifest(s)
+  title: "example"
+  # Data types of manifests to be generated or data type (singular) to validate manifest against
+  data_type:
+    - "Biospecimen"
+    - "Patient"
+
+# Describes the location of your schema
+model:
+  # Location of your schema jsonld, it must be a path relative to this file or absolute
+  location: "tests/data/example.model.jsonld"
+
+# This section is for using google sheets with Schematic
+google_sheets:
+  # The Synapse id of the Google service account credentials.
+  service_acct_creds_synapse_id: "syn25171627"
+  # Path to the synapse config file, either absolute or relative to this file
+  service_acct_creds: "schematic_service_account_creds.json"
+  # When doing google sheet validation (regex match) with the validation rules.
+  #   true is alerting the user and not allowing entry of bad values.
+  #   false is warning but allowing the entry on to the sheet.
+  strict_validation: true
+```
+
+If you want to change any of these copy ``config_example.yml`` to ``config.yml``, change any fields you want to, and remove any fields you don't.
+
+For example if you wanted to change the folder where manifests are downloaded your config should look like:
+
+```text
 
-*Note*: Paths can be specified relative to the `config.yml` file or as absolute paths.
+manifest:
+  manifest_folder: "my_manifest_folder_path"
+```
+
+_Note_: `config.yml` is ignored by git.
+
+_Note_: Paths can be specified relative to the `config.yml` file or as absolute paths.
 
 6. Login to Synapse by using the command line
 On the CLI in your virtual environment, run the following command: 
 ```
 synapse login -u <synapse username> -p <synapse password> --rememberMe
 ```
 Please make sure that you run the command before running `schematic init` below
@@ -260,15 +284,15 @@
 1. [Getting started with Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)
 2. [Installing Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)
 
 ## Update toml file and lock file
 If you install external libraries by using `poetry add <name of library>`, please make sure that you include `pyproject.toml` and `poetry.lock` file in your commit.
 
 ## Reporting bugs or feature requests
-You can use the [`Issues`](https://github.com/Sage-Bionetworks/schematic/issues) tab to **create bug and feature requests**. Providing enough details to the developers to verify and troubleshoot your issue is paramount:
+You can **create bug and feature requests** through [Sage Bionetwork's FAIR Data service desk](https://sagebionetworks.jira.com/servicedesk/customer/portal/5/group/8). Providing enough details to the developers to verify and troubleshoot your issue is paramount:
 - **Provide a clear and descriptive title as well as a concise summary** of the issue to identify the problem.
 - **Describe the exact steps which reproduce the problem** in as many details as possible.
 - **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.
 - **Explain which behavior you expected to see** instead and why.
 - **Provide screenshots of the expected or actual behaviour** where applicable.
 
 # Command Line Usage
```

### Comparing `schematicpy-23.6.3/pyproject.toml` & `schematicpy-23.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "schematicpy"
-version = "v23.6.3"
+version = "v23.7.1"
 description = "Package for biomedical data model and metadata ingress management"
 authors = [ "Milen Nikolov <milen.nikolov@sagebase.org>", "Lingling Peng <lingling.peng@sagebase.org>", "Mialy Defelice <mialy.defelice@sagebase.org>", "Gianna Jordan <gianna.jordan@sagebase.org>", "Bruno Grande <bruno.grande@sagebase.org>", "Robert Allaway <robert.allaway@sagebionetworks.org>",]
 readme = "README.md"
 homepage = "https://github.com/Sage-Bionetworks/schematic"
 repository = "https://github.com/Sage-Bionetworks/schematic"
 documentation = "https://github.com/Sage-Bionetworks/schematic"
 keywords = [ "schema", "metadata", "validation", "data model", "linked data",]
@@ -61,16 +61,16 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.5.1"
 flake8 = "^6.0.0"
 python-dotenv = "^0.21.0"
-black = "^22.6.0"
-mypy = "^0.982"
+black = "^23.7.0"
+mypy = "^1.4.1"
 pylint = "^2.16.1"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--verbose"
 testpaths = [ "tests",]
 filterwarnings = [ "ignore::DeprecationWarning",]
@@ -81,15 +81,15 @@
 version = "^2.8.0"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 markers = "python_version < \"3.9\""
 version = "^0.2.1"
 
 [tool.poetry.dependencies.schematic-db]
-version = "^0.0.20"
+version = "^0.0.29"
 extras = [ "synapse",]
 
 [tool.poetry.group.aws]
 optional = true
 
 [tool.poetry.group.aws.dependencies]
 uWSGI = "^2.0.21"
```

### Comparing `schematicpy-23.6.3/schematic/__init__.py` & `schematicpy-23.7.1/schematic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import logging
 
 import click
 import click_log
 
-from schematic.configuration import CONFIG
+from schematic.configuration.configuration import CONFIG
 from schematic.loader import LOADER
 from schematic.utils.google_api_utils import download_creds_file
 from schematic.utils.cli_utils import query_dict
 from schematic.help import init_command
 
 logging.basicConfig(
     format=("%(levelname)s: [%(asctime)s] %(name)s" " - %(message)s"),
@@ -31,15 +31,15 @@
 @click.option(
     "-c", "--config", required=True, help=query_dict(init_command, ("init", "config"))
 )
 def init(config):
     """Initialize authentication for schematic."""
     try:
         logger.debug(f"Loading config file contents in '{config}'")
-        obj = CONFIG.load_config(config)
-    except ValueError as e:
+        CONFIG.load_config(config)
+    except ValueError as exc:
         logger.error("'--config' not provided or environment variable not set.")
-        logger.exception(e)
+        logger.exception(exc)
         sys.exit(1)
 
-    # download crdentials file based on selected mode of authentication
+    # download credentials file based on selected mode of authentication
     download_creds_file()
```

### Comparing `schematicpy-23.6.3/schematic/__main__.py` & `schematicpy-23.7.1/schematic/__main__.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/etc/README.md` & `schematicpy-23.7.1/schematic/etc/README.md`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/etc/data_models/biothings.model.jsonld` & `schematicpy-23.7.1/schematic/etc/data_models/biothings.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/etc/data_models/schema_org.model.jsonld` & `schematicpy-23.7.1/schematic/etc/data_models/schema_org.model.jsonld`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/etc/validation_schemas/class.schema.json` & `schematicpy-23.7.1/schematic/etc/validation_schemas/class.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/etc/validation_schemas/model.schema.json` & `schematicpy-23.7.1/schematic/etc/validation_schemas/model.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/etc/validation_schemas/property.schema.json` & `schematicpy-23.7.1/schematic/etc/validation_schemas/property.schema.json`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/exceptions.py` & `schematicpy-23.7.1/schematic/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Schematic Exceptions"""
-from typing import Any, Sequence
+from typing import Optional, Any, Sequence
 
 
 class MissingConfigValueError(Exception):
     """Exception raised when configuration value not provided in config file.
 
     Args:
         config_keys: tuple of keys as present in config file.
         message: custom/pre-defined error message to be returned.
 
     Returns:
         message.
     """
 
-    def __init__(self, config_keys: Sequence[Any], message: str = None) -> None:
+    def __init__(
+        self, config_keys: Sequence[Any], message: Optional[str] = None
+    ) -> None:
         config_keys_str = " > ".join(config_keys)
         self.message = (
             "The configuration value corresponding to the argument "
             f"({config_keys_str}) doesn't exist. "
             "Please provide a value in the configuration file."
         )
 
@@ -37,15 +39,15 @@
         entity id: For synapse, thi
         message: custom/pre-defined error message to be returned.
 
     Returns:
         message.
     """
 
-    def __init__(self, syn_id: str, message: str = None) -> None:
+    def __init__(self, syn_id: str, message: Optional[str] = None) -> None:
         self.message = (
             f"'{syn_id}'' is not a desired entity type"
             "Please ensure that you put in the right syn_id"
         )
 
         if message:
             self.message = message
@@ -65,15 +67,15 @@
         message: custom/pre-defined error message to be returned.
 
     Returns:
         message.
     """
 
     def __init__(
-        self, arg_name: str, config_keys: Sequence[Any], message: str = None
+        self, arg_name: str, config_keys: Sequence[Any], message: Optional[str] = None
     ) -> None:
         config_keys_str = " > ".join(config_keys)
         self.message = (
             f"The value corresponding to the CLI argument '--{arg_name}'"
             " doesn't exist. "
             "Please provide a value for either the CLI argument or "
             f"({config_keys_str}) in the configuration file."
@@ -95,15 +97,15 @@
         project: Platform/project (e.g., synID of a project)
         message: custom/pre-defined error message to be returned.
 
     Returns:
         message.
     """
 
-    def __init__(self, project: str, message: str = None) -> None:
+    def __init__(self, project: str, message: Optional[str] = None) -> None:
         self.message = (
             f"Your access to '{project}'' could not be resolved. "
             "Please check your credentials and try again."
         )
 
         if message:
             self.message = message
```

### Comparing `schematicpy-23.6.3/schematic/help.py` & `schematicpy-23.7.1/schematic/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             "use_annotations": (
                 "This is a boolean flag. If flag is provided when command line utility is executed, it will prepopulate template "
                 "with existing annotations from Synapse."
             ),
             "json_schema": (
                 "Specify the path to the JSON Validation Schema for this argument. "
                 "You can either explicitly pass the `.json` file here or provide it in the `config.yml` file "
-                "as a value for the `(model > input > validation_schema)` key."
+                "as a value for the `(model > location)` key."
             ),
             "alphabetize_valid_values": (
                 "Specify to alphabetize valid attribute values either ascending (a) or descending (d)."
                 "Optional"
             ),
         },
         "migrate": {
```

### Comparing `schematicpy-23.6.3/schematic/loader.py` & `schematicpy-23.7.1/schematic/loader.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/manifest/commands.py` & `schematicpy-23.7.1/schematic/manifest/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import os
 import logging
 from pathlib import Path
-import click
-import click_log
-import logging
 import sys
 from typing import List
+import click
+import click_log
 
 from schematic.manifest.generator import ManifestGenerator
-from schematic.utils.cli_utils import fill_in_from_config, query_dict, parse_synIDs
+from schematic.utils.cli_utils import log_value_from_config, query_dict, parse_synIDs
 from schematic.help import manifest_commands
-from schematic import CONFIG
 from schematic.schemas.generator import SchemaGenerator
-from schematic.utils.google_api_utils import export_manifest_csv, export_manifest_excel, export_manifest_drive_service
+from schematic.utils.google_api_utils import export_manifest_csv
 from schematic.store.synapse import SynapseStorage
+from schematic.configuration.configuration import CONFIG
 
 logger = logging.getLogger('schematic')
 click_log.basic_config(logger)
 
 CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
 
-
 # invoke_without_command=True -> forces the application not to show aids before losing them with a --h
 @click.group(context_settings=CONTEXT_SETTINGS, invoke_without_command=True)
 @click_log.simple_verbosity_option(logger)
 @click.option(
     "-c",
     "--config",
     envvar="SCHEMATIC_CONFIG",
@@ -33,15 +31,16 @@
 @click.pass_context
 def manifest(ctx, config):  # use as `schematic manifest ...`
     """
     Sub-commands with Manifest Generation utilities/methods.
     """
     try:
         logger.debug(f"Loading config file contents in '{config}'")
-        ctx.obj = CONFIG.load_config(config)
+        CONFIG.load_config(config)
+        ctx.obj = CONFIG
     except ValueError as e:
         logger.error("'--config' not provided or environment variable not set.")
         logger.exception(e)
         sys.exit(1)
 
 
 # prototype based on getModelManifest() and get_manifest()
@@ -113,25 +112,26 @@
     json_schema,
     output_xlsx,
     alphabetize_valid_values,
 ):
     """
     Running CLI with manifest generation options.
     """
-    # optional parameters that need to be passed to ManifestGenerator()
-    # can be read from config.yml as well
-    data_type = fill_in_from_config("data_type", data_type, ("manifest", "data_type"))
-    jsonld = fill_in_from_config("jsonld", jsonld, ("model", "input", "location"))
-    title = fill_in_from_config("title", title, ("manifest", "title"), allow_none=True)
-    json_schema = fill_in_from_config(
-        "json_schema",
-        json_schema,
-        ("model", "input", "validation_schema"),
-        allow_none=True,
-    )
+    # Optional parameters that need to be passed to ManifestGenerator()
+    # If CLI parameters are None they are gotten from the CONFIG object and logged
+    if data_type is None:
+        data_type =  CONFIG.manifest_data_type
+        log_value_from_config("data_type", data_type)
+    if jsonld is None:
+        jsonld =  CONFIG.model_location
+        log_value_from_config("jsonld", jsonld)
+    if title is None:
+        title =  CONFIG.manifest_title
+        log_value_from_config("title", title)
+
     def create_single_manifest(data_type, output_csv=None, output_xlsx=None):
         # create object of type ManifestGenerator
         manifest_generator = ManifestGenerator(
             path_to_json_ld=jsonld,
             title=t,
             root=data_type,
             use_annotations=use_annotations,
@@ -258,17 +258,18 @@
     jsonld: str,
     return_entities: bool,
     dry_run: bool,
 ):
     """
     Running CLI with manifest migration options.
     """
-    jsonld = fill_in_from_config("jsonld", jsonld, ("model", "input", "location"))
+    if jsonld is None:
+        jsonld =  CONFIG.model_location
+        log_value_from_config("jsonld", jsonld)
 
-    
     full_scope = project_scope + [archive_project]
     synStore = SynapseStorage(project_scope = full_scope)  
 
     for project in project_scope:
         if not return_entities:
             logging.info("Re-uploading manifests as tables")
             synStore.upload_annotated_project_manifests_to_synapse(project, jsonld, dry_run)
```

### Comparing `schematicpy-23.6.3/schematic/manifest/generator.py` & `schematicpy-23.7.1/schematic/manifest/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from openpyxl import load_workbook
 from openpyxl.utils.dataframe import dataframe_to_rows
 import os
 import pandas as pd
 from pathlib import Path
 import pygsheets as ps
 from tempfile import NamedTemporaryFile
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 from schematic.schemas.generator import SchemaGenerator
 from schematic.utils.google_api_utils import (
     execute_google_api_requests,
     build_service_account_creds,
 )
 from schematic.utils.df_utils import update_df, load_df
 from schematic.utils.validate_utils import rule_in_rule_list
 
 #TODO: This module should only be aware of the store interface
 # we shouldn't need to expose Synapse functionality explicitly
 from schematic.store.synapse import SynapseStorage
 
-from schematic import CONFIG
+from schematic.configuration.configuration import CONFIG
 from schematic.utils.google_api_utils import export_manifest_drive_service
 
 
 logger = logging.getLogger(__name__)
 
 
 
@@ -125,21 +125,17 @@
 
         'if a cell in column idx is equal to condition argument, then set specified formatting'
         """
 
         col_letter = self._column_to_letter(column_idx)
 
         if not required:
-            bg_color = CONFIG["style"]["google_manifest"].get(
-                "opt_bg_color", {"red": 1.0, "green": 1.0, "blue": 0.9019,},
-            )
+            bg_color = CONFIG.google_optional_background_color
         else:
-            bg_color = CONFIG["style"]["google_manifest"].get(
-                "req_bg_color", {"red": 0.9215, "green": 0.9725, "blue": 0.9803,},
-            )
+            bg_color = CONFIG.google_required_background_color
 
         boolean_rule = {
             "condition": {
                 "type": "CUSTOM_FORMULA",
                 "values": [
                     {
                         "userEnteredValue": "=$"
@@ -170,30 +166,41 @@
         # return new copy sheet ID
         return (
             self.drive_service.files()
             .copy(fileId=origin_file_id, body=copied_file)
             .execute()["id"]
         )
 
-    def _create_empty_manifest_spreadsheet(self, title):
-        if CONFIG["style"]["google_manifest"]["master_template_id"]:
+    def _create_empty_manifest_spreadsheet(self, title:str) -> str:
+        """
+        Creates an empty google spreadsheet returning the id.
+        If the configuration has a template id it will be used
 
-            # if provided with a template manifest google sheet, use it
-            spreadsheet_id = self._gdrive_copy_file(
-                CONFIG["style"]["google_manifest"]["master_template_id"], title
-            )
+        Args:
+            title (str): The title of the spreadsheet
+
+        Returns:
+            str: The id of the created spreadsheet
+        """
+        template_id = CONFIG.google_sheets_master_template_id
+
+        if template_id:
+            spreadsheet_id = self._gdrive_copy_file(template_id, title)
 
         else:
             spreadsheet_body = {
-            'properties': {
-                'title': title
-            }}
+                'properties': {
+                    'title': title
+                }
+            }
 
-            # if no template, create an empty spreadsheet
-            spreadsheet_id = self.sheet_service.spreadsheets().create(body=spreadsheet_body, fields="spreadsheetId").execute().get("spreadsheetId")
+            spreadsheet_id = self.sheet_service.spreadsheets().create(
+                body=spreadsheet_body,
+                fields="spreadsheetId").execute().get("spreadsheetId"
+            )
 
         return spreadsheet_id
 
     def _get_cell_borders(self, cell_range):
 
         # set border style request
         color = {
@@ -277,24 +284,23 @@
         return valid_values
 
     def _get_column_data_validation_values(
         self,
         spreadsheet_id,
         valid_values,
         column_id,
-        strict,
+        strict:Optional[bool],
         validation_type="ONE_OF_LIST",
         custom_ui=True,
         input_message="Choose one from dropdown",
     ):
 
         # set validation strictness to config file default if None indicated.
         if strict == None:
-            strict = CONFIG["style"]["google_manifest"].get("strict_validation", True)
-        
+            strict = CONFIG.google_sheets_strict_validation
         #store valid values explicitly in workbook at the provided range to use as validation values
         if validation_type == "ONE_OF_RANGE":
             valid_values=self._store_valid_values_as_data_dictionary(column_id, valid_values, spreadsheet_id)
 
         # setup validation data request body
         validation_body = {
             "requests": [
@@ -696,15 +702,15 @@
                     }
                 }
             ]
         }
         return requests_vr
 
     def _request_regex_match_vr_formatting(self, validation_rules: List[str], i: int,
-        spreadsheet_id: str, requests_body: dict,
+        spreadsheet_id: str, requests_body: dict, strict: Optional[bool],
         ):
         """
         Purpose:
             - Apply regular expression validaiton rules to google sheets.
             - Will only be run if the regex module specified in the validation
             rules is 'match'.
                 - This is because of the limitations of google sheets regex.
@@ -736,15 +742,14 @@
                 {
                     "userEnteredValue": '=REGEXMATCH(INDIRECT("RC",FALSE), "{}")'.format(
                         regular_expression
                     )
                 }
             ]
             ## Set validaiton strictness based on user specifications.
-            strict = None
             if split_rules[-1].lower() == "strict":
                 strict = True
 
             ## Create error message for users if they enter value with incorrect formatting
             input_message = (
                 f"Values in this column are being validated "
                 f"against the following regular expression ({regular_expression}) "
@@ -891,22 +896,15 @@
                 'type', 'properties', 'required'
         Returns:
             req_format_body["requests"] (dict): specifing the format updating for
                 required attributes/columns
         """
         # check if attribute is required and set a corresponding color
         if req in json_schema["required"]:
-            bg_color = CONFIG["style"]["google_manifest"].get(
-                "req_bg_color",
-                {
-                    "red": 0.9215,
-                    "green": 0.9725,
-                    "blue": 0.9803,
-                },
-            )
+            bg_color = CONFIG.google_required_background_color
 
             req_format_body = {
                 "requests": [
                     {
                         "repeatCell": {
                             "range": {
                                 "startColumnIndex": i,
@@ -1077,42 +1075,47 @@
 
     def _create_requests_body(
         self,
         required_metadata_fields,
         ordered_metadata_fields,
         json_schema,
         spreadsheet_id,
+        sheet_url,
+        strict: Optional[bool],
     ):
         """Create and store all formatting changes for the google sheet to
         execute at once.
         Args:
             required_metadata_fields(dict):
                 keys: of all the fields/attributes that need to be added
                     to the manifest
                 values(list[str]): valid values
             ordered_metadata_fields: List[list], contining all the attributes to
                 add as columns, ordered
             json_schema: dict, representing a handful of values
                 representing the data model, including: '$schema', '$id', 'title',
                 'type', 'properties', 'required'
             spreadsheet_id: str, of the id for the google sheet
+            sheet_url (Will be deprecated): a boolean ; determine if a pandas dataframe or a google sheet url gets return
+            strict (Optional Bool): strictness with which to apply validation rules to google sheets. True, blocks incorrect entries, False, raises a warning
         Return:
             requests_body(dict):
                 containing all the update requests to add to the gs
         """
         # store all requests to execute at once
         requests_body = {}
         requests_body["requests"] = []
         for i, req in enumerate(ordered_metadata_fields[0]):
-            # Gather validation rules and valid values for attribute
+            # Gather validation rules and valid values for attribute.
             validation_rules = self.sg.get_node_validation_rules(req)
-
-            if validation_rules:
+            
+            # Add regex match validaiton rule to Google Sheets.
+            if validation_rules and sheet_url:
                 requests_body =self._request_regex_match_vr_formatting(
-                        validation_rules, i, spreadsheet_id, requests_body
+                        validation_rules, i, spreadsheet_id, requests_body, strict
                         )
 
             if req in json_schema["properties"].keys():
                 valid_values = self._get_valid_values_from_jsonschema_property(
                     json_schema["properties"][req]
                 )
             else:
@@ -1160,25 +1163,27 @@
            
         # Set borders formatting
         borders_formatting = self._request_cell_borders()
         if borders_formatting:
             requests_body["requests"].append(borders_formatting)
         return requests_body
 
-    def _create_empty_gs(self, required_metadata_fields, json_schema, spreadsheet_id):
+    def _create_empty_gs(self, required_metadata_fields, json_schema, spreadsheet_id, sheet_url, strict: Optional[bool]):
         """Generate requests to add columns and format the google sheet.
         Args:
             required_metadata_fields(dict):
                 keys: of all the fields/attributes that need to be added
                     to the manifest
                 values(list[str]): valid values
             json_schema: dict, representing a handful of values
                 representing the data model, including: '$schema', '$id', 'title',
                 'type', 'properties', 'required'
             spreadsheet_id: str, of the id for the google sheet
+            sheet_url (str): google sheet url of template manifest
+            strict (Optional Bool): strictness with which to apply validation rules to google sheets. True, blocks incorrect entries, False, raises a warning
         Returns:
             manifest_url (str): url of the google sheet manifest.
         """
         # adding columns to manifest sheet
         response, ordered_metadata_fields = self._gs_add_and_format_columns(
             required_metadata_fields, spreadsheet_id
         )
@@ -1190,14 +1195,16 @@
 
         # Create requests body to add additional formatting to the sheets
         requests_body = self._create_requests_body(
             required_metadata_fields,
             ordered_metadata_fields,
             json_schema,
             spreadsheet_id,
+            sheet_url,
+            strict,
         )
 
         # Execute requests
         execute_google_api_requests(
             self.sheet_service,
             requests_body,
             service_type="batch_update",
@@ -1232,33 +1239,36 @@
 
         # Add additional metadata as entries to columns
         required_metadata_fields = self._get_additional_metadata(
             required_metadata_fields
         )
         return required_metadata_fields
 
-    def get_empty_manifest(self, json_schema_filepath=None):
+    def get_empty_manifest(self, strict: Optional[bool], json_schema_filepath: str=None, sheet_url: Optional[bool]=None):
         """Create an empty manifest using specifications from the
         json schema.
         Args:
+            strict (bool): strictness with which to apply validation rules to google sheets. If true, blocks incorrect entries; if false, raises a warning
             json_schema_filepath (str): path to json schema file
+            sheet_url (Will be deprecated): a boolean ; determine if a pandas dataframe or a google sheet url gets return
+            strict (Optional Bool): strictness with which to apply validation rules to google sheets. True, blocks incorrect entries, False, raises a warning
         Returns:
             manifest_url (str): url of the google sheet manifest.
         TODO:
             Refactor to not be dependent on GS.
         """
         spreadsheet_id = self._create_empty_manifest_spreadsheet(self.title)
-        json_schema = self._get_json_schema(json_schema_filepath)
+        json_schema = self._get_json_schema(json_schema_filepath=json_schema_filepath)
 
         required_metadata_fields = self._gather_all_fields(
             json_schema["properties"].keys(), json_schema
         )
 
         manifest_url = self._create_empty_gs(
-            required_metadata_fields, json_schema, spreadsheet_id
+            required_metadata_fields, json_schema, spreadsheet_id, sheet_url=sheet_url, strict=strict,
         )
         return manifest_url
 
     def _get_missing_columns(self, headers_1:list , headers_2:list) -> list:
         """Compare two colunm sets and get cols that are in headers_1, but not headers_2
         Args:
             headers_1 (list): list of column headers
@@ -1294,14 +1304,16 @@
         # update validation rules (i.e. no validation rules) for out of schema columns, if any
         # TODO: similarly clear formatting for out of schema columns, if any
         if out_of_schema_columns:
             num_out_of_schema_columns = len(out_of_schema_columns)
             start_col = self._column_to_letter(len(manifest_df.columns) - num_out_of_schema_columns) # find start of out of schema columns
             end_col = self._column_to_letter(len(manifest_df.columns) + 1) # find end of out of schema columns
             wb.set_data_validation(start = start_col, end = end_col, condition_type = None)
+        
+
         # set permissions so that anyone with the link can edit
         sh.share("", role="writer", type="anyone")
 
         return sh
 
     def get_dataframe_by_url(self, manifest_url: str) -> pd.DataFrame:
         """Retrieve pandas DataFrame from table in Google Sheets.
@@ -1349,21 +1361,22 @@
         # Generate a dictionary mapping labels to display names
         label_map = {l: model_nodes[l]["displayName"] for l in labels}
 
         # Use the above dictionary to rename columns in question
         return annotations.rename(columns=label_map)
 
     def get_manifest_with_annotations(
-        self, annotations: pd.DataFrame
+        self, annotations: pd.DataFrame, sheet_url:bool=None, strict: Optional[bool]=None,
     ) -> Tuple[ps.Spreadsheet, pd.DataFrame]:
         """Generate manifest, optionally with annotations (if requested).
 
         Args:
             annotations (pd.DataFrame): Annotations table (can be empty).
-
+            strict (Optional Bool): strictness with which to apply validation rules to google sheets. True, blocks incorrect entries, False, raises a warning
+            sheet_url (Will be deprecated): a boolean ; determine if a pandas dataframe or a google sheet url gets return
         Returns:
             Tuple[ps.Spreadsheet, pd.DataFrame]: Both the Google Sheet
             URL and the corresponding data frame is returned.
         """
 
         # Map annotation labels to display names to match manifest columns
         annotations = self.map_annotation_names_to_display_names(annotations)
@@ -1374,16 +1387,16 @@
             (k, list(v.values())) for k, v in annotations_dict_raw.items()
         )
 
         # Needs to happen before get_empty_manifest() gets called
         self.additional_metadata = annotations_dict
 
         # Generate empty manifest using `additional_metadata`
-        manifest_url = self.get_empty_manifest()
-        manifest_df = self.get_dataframe_by_url(manifest_url)
+        manifest_url = self.get_empty_manifest(sheet_url=sheet_url, strict=strict)
+        manifest_df = self.get_dataframe_by_url(manifest_url=manifest_url)
 
         # Annotations clashing with manifest attributes are skipped
         # during empty manifest generation. For more info, search
         # for `additional_metadata` in `self.get_empty_manifest`.
         # Hence, the shared columns need to be updated separately.
         if self.is_file_based and self.use_annotations:
             # This approach assumes that `update_df` returns
@@ -1458,42 +1471,42 @@
 
             # populate an excel spreadsheet with the existing dataframe
             self.populate_existing_excel_spreadsheet(output_file_path, dataframe)
 
             return output_file_path
         
         # Return google sheet if sheet_url flag is raised.
-        elif sheet_url: 
+        elif sheet_url:
             manifest_sh = self.set_dataframe_by_url(manifest_url=empty_manifest_url, manifest_df=dataframe, out_of_schema_columns=out_of_schema_columns)
             return manifest_sh.url
         
         # Default return a DataFrame
         else:
             return dataframe
 
     def get_manifest(
-        self, dataset_id: str = None, sheet_url: bool = None, json_schema: str = None, output_format: str = None, output_path: str = None, access_token: str = None
+        self, dataset_id: str = None, sheet_url: bool = None, json_schema: str = None, output_format: str = None, output_path: str = None, access_token: str = None, strict: Optional[bool]=None,
     ) -> Union[str, pd.DataFrame]:
         """Gets manifest for a given dataset on Synapse.
            TODO: move this function to class MetadatModel (after MetadataModel is refactored)
 
         Args:
             dataset_id: Synapse ID of the "dataset" entity on Synapse (for a given center/project).
-            sheet_url: Determines if googlesheet URL or pandas dataframe should be returned.
+            sheet_url (Will be deprecated): a boolean ; determine if a pandas dataframe or a google sheet url gets return
             output_format: Determines if Google sheet URL, pandas dataframe, or Excel spreadsheet gets returned.
             output_path: Determines the output path of the exported manifest
             access_token: Token in .synapseConfig. Since we could not pre-load access_token as an environment variable on AWS, we have to add this variable. 
 
         Returns:
             Googlesheet URL, pandas dataframe, or an Excel spreadsheet 
         """
 
         # Handle case when no dataset ID is provided
         if not dataset_id:
-            manifest_url = self.get_empty_manifest(json_schema_filepath=json_schema)
+            manifest_url = self.get_empty_manifest(json_schema_filepath=json_schema, strict=strict, sheet_url=sheet_url)
 
             # if output_form parameter is set to "excel", return an excel spreadsheet
             if output_format == "excel": 
                 output_file_path = self.export_sheet_to_excel(title = self.title, manifest_url = manifest_url, output_location = output_path)
                 return output_file_path
             # since we are not going to return an empty dataframe for an empty manifest, here we will just return a google sheet url for all other cases
             else: 
@@ -1510,21 +1523,20 @@
             store = SynapseStorage()
 
         # Get manifest file associated with given dataset (if applicable)
         # populate manifest with set of new files (if applicable)
         manifest_record = store.updateDatasetManifestFiles(self.sg, datasetId = dataset_id, store = False)
 
         # get URL of an empty manifest file created based on schema component
-        empty_manifest_url = self.get_empty_manifest()
+        empty_manifest_url = self.get_empty_manifest(strict=strict, sheet_url=sheet_url)
 
         # Populate empty template with existing manifest
         if manifest_record:
             # TODO: Update or remove the warning in self.__init__() if
             # you change the behavior here based on self.use_annotations
-
             # Update df with existing manifest. Agnostic to output format
             updated_df, out_of_schema_columns = self._update_dataframe_with_existing_df(empty_manifest_url=empty_manifest_url, existing_df=manifest_record[1])
 
             # determine the format of manifest
             result = self._handle_output_format_logic(output_format = output_format,
                                                       output_path = output_path,
                                                       sheet_url = sheet_url,
@@ -1541,36 +1553,61 @@
 
             annotations = pd.DataFrame()
             if self.is_file_based:
                 annotations = store.getDatasetAnnotations(dataset_id)
 
             # if there are no files with annotations just generate an empty manifest
             if annotations.empty:
-                manifest_url = self.get_empty_manifest()
+                manifest_url = self.get_empty_manifest(strict=strict)
                 manifest_df = self.get_dataframe_by_url(manifest_url)
             else:
                 # Subset columns if no interested in user-defined annotations and there are files present
                 if self.is_file_based and not self.use_annotations:
                     annotations = annotations[["Filename", "eTag", "entityId"]]
 
                 # Update `additional_metadata` and generate manifest
-                manifest_url, manifest_df = self.get_manifest_with_annotations(annotations)
-            
+                manifest_url, manifest_df = self.get_manifest_with_annotations(annotations, sheet_url=sheet_url, strict=strict)
+
             # Update df with existing manifest. Agnostic to output format
             updated_df, out_of_schema_columns = self._update_dataframe_with_existing_df(empty_manifest_url=empty_manifest_url, existing_df=manifest_df)
 
             # determine the format of manifest that gets return 
             result = self._handle_output_format_logic(output_format = output_format,
                                                       output_path = output_path,
                                                       sheet_url = sheet_url,
                                                       empty_manifest_url=empty_manifest_url,
-                                                      dataframe = manifest_df,
+                                                      dataframe = updated_df,
+                                                      out_of_schema_columns = out_of_schema_columns,
                                                       )
             return result
 
+    def _get_end_columns(self, current_schema_headers, existing_manifest_headers, out_of_schema_columns):
+        """
+        Gather columns to be added to the end of the manifest, and ensure entityId is at the end.
+        Args:
+            current_schema_headers: list, columns in the current manifest schema
+            existing_manifest_headers: list, columns in the existing manifest
+            out_of_schema_columns: set, columns that are in the existing manifest, but not the current schema
+        Returns:
+            end_columns: list of columns to be added to the end of the manifest.
+        """
+        # Identify columns to add to the end of the manifest
+        end_columns = list(out_of_schema_columns)
+        
+        # Make sure want Ids are placed at end of manifest, in given order.
+        for id_name in ['Uuid', 'Id', 'entityId']:
+            if id_name in end_columns:
+                end_columns.remove(id_name)
+                end_columns.append(id_name)
+        
+        # Add entity_id to the end columns if it should be there but isn't
+        if 'entityId' in (current_schema_headers or existing_manfiest_headers) and 'entityId' not in end_columns:
+            end_columns.append('entityId')
+        return end_columns
+
     def _update_dataframe_with_existing_df(self, empty_manifest_url: str, existing_df: pd.DataFrame) -> pd.DataFrame:
         """
         Handle scenario when existing manifest does not match new manifest template due to changes in the data model:
             the sheet column header reflect the latest schema the existing manifest column-set may be outdated
             ensure that, if missing, attributes from the latest schema are added to the column-set of the existing manifest so that the user can modify their data if needed
             to comply with the latest schema.
         Args:
@@ -1579,22 +1616,22 @@
 
         Returns:
             updated_df (Pd.DataFrame): existing_df with new_columns added.
             out_of_schema_columns (set): Columns that are in downloaded manifest, but not in current schema.
         """
 
         # Get headers for the current schema and existing manifest df.
-        current_schema_headers = list(self.get_dataframe_by_url(empty_manifest_url).columns)
+        current_schema_headers = list(self.get_dataframe_by_url(manifest_url=empty_manifest_url).columns)
         existing_manfiest_headers = list(existing_df.columns)
 
         # Find columns that exist in the current schema, but are not in the manifest being downloaded.
-        new_columns = self._get_missing_columns(current_schema_headers, existing_manfiest_headers)
+        new_columns = self._get_missing_columns(current_schema_headers, existing_manifest_headers)
 
         # Find columns that exist in the manifest being downloaded, but not in the current schema.
-        out_of_schema_columns = self._get_missing_columns(existing_manfiest_headers, current_schema_headers)
+        out_of_schema_columns = self._get_missing_columns(existing_manifest_headers, current_schema_headers)
 
         # clean empty columns if any are present (there should be none)
         # TODO: Remove this line once we start preventing empty column names
         if '' in new_columns:
             new_columns = new_columns.remove('')
 
         # Copy the df for updating.
@@ -1602,20 +1639,25 @@
         
         # update existing manifest w/ missing columns, if any
         if new_columns:
             updated_df = updated_df.assign(
                 **dict(zip(new_columns, len(new_columns) * [""]))
             )
 
+        end_columns = self._get_end_columns(current_schema_headers=current_schema_headers,
+                                           existing_manifest_headers=existing_manifest_headers,
+                                           out_of_schema_columns=out_of_schema_columns)
+        
         # sort columns in the updated manifest:
         # match latest schema order
         # move obsolete columns at the end
         updated_df = updated_df[self.sort_manifest_fields(updated_df.columns)]
-        updated_df = updated_df[[c for c in updated_df if c not in out_of_schema_columns] + list(out_of_schema_columns)]
 
+        # move obsolete columns at the end with entityId at the very end
+        updated_df = updated_df[[c for c in updated_df if c not in end_columns] + list(end_columns)]
         return updated_df, out_of_schema_columns
 
     def _format_new_excel_column(self, worksheet, new_column_index: int, col: str):
         """Add new column to an openpyxl worksheet and format header.
         Args:
             worksheet: openpyxl worksheet
             new_column_index, int: index to add new column
```

### Comparing `schematicpy-23.6.3/schematic/models/GE_Helpers.py` & `schematicpy-23.7.1/schematic/models/GE_Helpers.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/models/commands.py` & `schematicpy-23.7.1/schematic/models/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 import click
 import click_log
 
 from jsonschema import ValidationError
 
 from schematic.models.metadata import MetadataModel
-from schematic.utils.cli_utils import get_from_config, fill_in_from_config, query_dict, parse_synIDs, parse_comma_str_to_list
+from schematic.utils.cli_utils import log_value_from_config, query_dict, parse_synIDs, parse_comma_str_to_list
 from schematic.help import model_commands
 from schematic.exceptions import MissingConfigValueError
-from schematic import CONFIG
+from schematic.configuration.configuration import CONFIG
 
 logger = logging.getLogger('schematic')
 click_log.basic_config(logger)
 
 CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
 
 # invoke_without_command=True -> forces the application not to show aids before losing them with a --h
@@ -34,15 +34,16 @@
 @click.pass_context
 def model(ctx, config):  # use as `schematic model ...`
     """
     Sub-commands for Metadata Model related utilities/methods.
     """
     try:
         logger.debug(f"Loading config file contents in '{config}'")
-        ctx.obj = CONFIG.load_config(config)
+        CONFIG.load_config(config)
+        ctx.obj =  CONFIG
     except ValueError as e:
         logger.error("'--config' not provided or environment variable not set.")
         logger.exception(e)
         sys.exit(1)
 
 
 # prototype based on submit_metadata_manifest()
@@ -106,20 +107,19 @@
 def submit_manifest(
     ctx, manifest_path, dataset_id, validate_component, manifest_record_type, use_schema_label, hide_blanks, restrict_rules, project_scope, table_manipulation,
 ):
     """
     Running CLI with manifest validation (optional) and submission options.
     """
     
-    jsonld = get_from_config(CONFIG.DATA, ("model", "input", "location"))
-
-    model_file_type = get_from_config(CONFIG.DATA, ("model", "input", "file_type"))
+    jsonld =  CONFIG.model_location
+    log_value_from_config("jsonld", jsonld)
 
     metadata_model = MetadataModel(
-        inputMModelLocation=jsonld, inputMModelLocationType=model_file_type
+        inputMModelLocation=jsonld, inputMModelLocationType="local"
     )
 
 
     manifest_id = metadata_model.submit_metadata_manifest(
         path_to_json_ld = jsonld,
         manifest_path=manifest_path,
         dataset_id=dataset_id,
@@ -177,39 +177,34 @@
     help=query_dict(model_commands, ("model", "validate", "project_scope")),
 )
 @click.pass_obj
 def validate_manifest(ctx, manifest_path, data_type, json_schema, restrict_rules,project_scope):
     """
     Running CLI for manifest validation.
     """
-    if not data_type:
-        data_type = fill_in_from_config("data_type", data_type, ("manifest", "data_type"))
-    
+    if data_type is None:
+        data_type =  CONFIG.manifest_data_type
+        log_value_from_config("data_type", data_type)
+ 
     try:
         len(data_type) == 1
     except:
         logger.error(
             f"Can only validate a single data_type at a time. Please provide a single data_type"
         )
 
     data_type = data_type[0]
 
-    json_schema = fill_in_from_config(
-        "json_schema",
-        json_schema,
-        ("model", "input", "validation_schema"),
-        allow_none=True,
-    )
     t_validate = perf_counter()
-    jsonld = get_from_config(CONFIG.DATA, ("model", "input", "location"))
 
-    model_file_type = get_from_config(CONFIG.DATA, ("model", "input", "file_type"))
+    jsonld =  CONFIG.model_location
+    log_value_from_config("jsonld", jsonld)
 
     metadata_model = MetadataModel(
-        inputMModelLocation=jsonld, inputMModelLocationType=model_file_type
+        inputMModelLocation=jsonld, inputMModelLocationType="local"
     )
 
     errors, warnings = metadata_model.validateModelManifest(
         manifestPath=manifest_path, rootNode=data_type, jsonSchema=json_schema, restrict_rules=restrict_rules, project_scope=project_scope,
     )
 
     if not errors:
```

### Comparing `schematicpy-23.6.3/schematic/models/metadata.py` & `schematicpy-23.7.1/schematic/models/metadata.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/models/validate_attribute.py` & `schematicpy-23.7.1/schematic/models/validate_attribute.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/models/validate_manifest.py` & `schematicpy-23.7.1/schematic/models/validate_manifest.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/schemas/commands.py` & `schematicpy-23.7.1/schematic/schemas/commands.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/schemas/curie.py` & `schematicpy-23.7.1/schematic/schemas/curie.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/schemas/df_parser.py` & `schematicpy-23.7.1/schematic/schemas/df_parser.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/schemas/explorer.py` & `schematicpy-23.7.1/schematic/schemas/explorer.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/schemas/generator.py` & `schematicpy-23.7.1/schematic/schemas/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from schematic.schemas.explorer import SchemaExplorer
 from schematic.utils.io_utils import load_json
 from schematic.utils.cli_utils import query_dict
 from schematic.utils.schema_utils import load_schema_into_networkx
 from schematic.utils.validate_utils import validate_schema, rule_in_rule_list
 
-from schematic import CONFIG
 
 logger = logging.getLogger(__name__)
 
 
 class SchemaGenerator(object):
     def __init__(
         self,
@@ -685,36 +684,24 @@
 
         logger.info("JSON schema successfully generated from schema.org schema!")
 
         # if no conditional dependencies were added we can't have an empty 'AllOf' block in the schema, so remove it
         if not json_schema["allOf"]:
             del json_schema["allOf"]
 
-        # Check if config value is provided; otherwise, set to None
-        json_schema_log_file = query_dict(
-            CONFIG.DATA, ("model", "input", "log_location")
-        )
-
         # If no config value and SchemaGenerator was initialized with
         # a JSON-LD path, construct
-        if json_schema_log_file is None and self.jsonld_path is not None:
+        if self.jsonld_path is not None:
             prefix = self.jsonld_path_root
             prefix_root, prefix_ext = os.path.splitext(prefix)
             if prefix_ext == ".model":
                 prefix = prefix_root
             json_schema_log_file = f"{prefix}.{source_node}.schema.json"
 
-        if json_schema_log_file is None:
-            logger.info(
-                "The JSON schema file can be inspected by setting the following "
-                "nested key in the configuration: (model > input > log_location)."
-            )
-        else:
-            json_schema_dirname = os.path.dirname(json_schema_log_file)
-            if json_schema_dirname != '':
-                os.makedirs(json_schema_dirname, exist_ok=True)
-            with open(json_schema_log_file, "w") as js_f:
-                json.dump(json_schema, js_f, indent=2)
+        logger.info(
+            "The JSON schema file can be inspected by setting the following "
+            "nested key in the configuration: (model > input > log_location)."
+        )
 
         logger.info(f"JSON schema file log stored as {json_schema_log_file}")
 
         return json_schema
```

### Comparing `schematicpy-23.6.3/schematic/schemas/validator.py` & `schematicpy-23.7.1/schematic/schemas/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 )
 from schematic.utils.validate_utils import (
     validate_class_schema,
     validate_property_schema,
     validate_schema,
 )
 
-from schematic import CONFIG
-
 
 class SchemaValidator:
     """Validate Schema against SchemaOrg standard
 
     Validation Criterias:
     1. Data Structure wise:
       > "@id", "@context", "@graph"
```

### Comparing `schematicpy-23.6.3/schematic/store/synapse.py` & `schematicpy-23.7.1/schematic/store/synapse.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,27 +36,28 @@
 from synapseclient.annotations import from_synapse_annotations
 from synapseclient.core.exceptions import SynapseHTTPError, SynapseAuthenticationError, SynapseUnmetAccessRestrictions
 from synapseutils import walk
 from synapseutils.copy_functions import changeFileMetaData
 
 import uuid
 
-from schematic_db.synapse.synapse import SynapseConfig
 from schematic_db.rdb.synapse_database import SynapseDatabase
 
 
 from schematic.utils.df_utils import update_df, load_df, col_in_dataframe, populate_df_col_with_another_col
 from schematic.utils.validate_utils import comma_separated_list_regex, rule_in_rule_list
 from schematic.utils.general import entity_type_mapping, get_dir_size, convert_size, convert_gb_to_bytes, create_temp_folder
 from schematic.schemas.explorer import SchemaExplorer
 from schematic.schemas.generator import SchemaGenerator
 from schematic.store.base import BaseStorage
 from schematic.exceptions import MissingConfigValueError, AccessCredentialsError
 
-from schematic import CONFIG
+from schematic.configuration.configuration import CONFIG
+
+from schematic.utils.general import profile
 
 logger = logging.getLogger("Synapse storage")
 
 @dataclass
 class ManifestDownload(object):
     """
     syn: an object of type synapseclient.
@@ -65,43 +66,31 @@
     syn: synapseclient.Synapse
     manifest_id: str
 
     def _download_manifest_to_folder(self) -> File:
         """
         try downloading a manifest to local cache or a given folder
         manifest
-        Return: 
+        Return:
             manifest_data: A Synapse file entity of the downloaded manifest
         """
-        # TO DO: potentially deprecate the if else statement because "manifest_folder" key always exist in config (See issue FDS-349 in Jira)
-        # on AWS, to avoid overriding manifest, we download the manifest to a temporary folder
         if "SECRETS_MANAGER_SECRETS" in os.environ:
             temporary_manifest_storage = "/var/tmp/temp_manifest_download"
             if not os.path.exists(temporary_manifest_storage):
                 os.mkdir("/var/tmp/temp_manifest_download")
             download_location = create_temp_folder(temporary_manifest_storage)
-
-        elif CONFIG["synapse"]["manifest_folder"]:
-            download_location=CONFIG["synapse"]["manifest_folder"]
-
         else:
-            download_location=None
-        
-        if not download_location:
-            manifest_data = self.syn.get(
-                        self.manifest_id,
-                    )
-        # if download_location is provided and it is not an empty string
-        else:
-            manifest_data = self.syn.get(
-                    self.manifest_id,
-                    downloadLocation=download_location,
-                    ifcollision="overwrite.local",
-                )
-        return manifest_data 
+            download_location=CONFIG.manifest_folder
+
+        manifest_data = self.syn.get(
+                self.manifest_id,
+                downloadLocation=download_location,
+                ifcollision="overwrite.local",
+            )
+        return manifest_data
 
     def _entity_type_checking(self) -> str:
         """
         check the entity type of the id that needs to be downloaded
         Return: 
              if the entity type is wrong, raise an error
         """
@@ -187,28 +176,16 @@
             ValueError: when Admin fileview cannot be found (describe further).
         Typical usage example:
             syn_store = SynapseStorage()
         """
 
         self.syn = self.login(token, access_token)
         self.project_scope = project_scope
-
-
-        # check if "master_fileview" has been set
-        try: 
-            self.storageFileview = CONFIG["synapse"]["master_fileview"]
-        except KeyError: 
-            raise MissingConfigValueError(("synapse", "master_fileview"))
-
-        # check if "manifest_basename" has been set
-        try: 
-            self.manifest = CONFIG["synapse"]["manifest_basename"]
-        except KeyError: 
-            raise MissingConfigValueError(("synapse", "manifest_basename"))
-
+        self.storageFileview = CONFIG.synapse_master_fileview_id
+        self.manifest = CONFIG.synapse_manifest_basename
         self._query_fileview()
 
     def _purge_synapse_cache(self, root_dir: str = "/var/www/.synapseCache/", maximum_storage_allowed_cache_gb=7):
         """
         Purge synapse cache if it exceeds 7GB
         Args:
             root_dir: directory of the .synapseCache function
@@ -235,28 +212,25 @@
                 remaining_space = total_ephemeral_storage_bytes - nbytes
                 converted_space = convert_size(remaining_space)
                 logger.info(f'Estimated {remaining_space} bytes (which is approximately {converted_space}) remained in ephemeral storage after calculating size of .synapseCache excluding OS')
 
     def _query_fileview(self):
         self._purge_synapse_cache()
         try:
-            self.storageFileview = CONFIG["synapse"]["master_fileview"]
-            self.manifest = CONFIG["synapse"]["manifest_basename"]
+            self.storageFileview = CONFIG.synapse_master_fileview_id
+            self.manifest = CONFIG.synapse_manifest_basename
             if self.project_scope:
                 self.storageFileviewTable = self.syn.tableQuery(
                     f"SELECT * FROM {self.storageFileview} WHERE projectId IN {tuple(self.project_scope + [''])}"
                     ).asDataFrame()
             else:
                 # get data in administrative fileview for this pipeline
                 self.storageFileviewTable = self.syn.tableQuery(
                     "SELECT * FROM " + self.storageFileview
                 ).asDataFrame()
-
-        except AttributeError:
-            raise AttributeError("storageFileview attribute has not been set.")
         except SynapseHTTPError:
             raise AccessCredentialsError(self.storageFileview)    
 
     @staticmethod
     def login(token=None, access_token=None):
         # If no token is provided, try retrieving access token from environment
         if not token and not access_token:
@@ -274,17 +248,16 @@
             try:
                 syn = synapseclient.Synapse()
                 syn.default_headers["Authorization"] = f"Bearer {access_token}"
             except synapseclient.core.exceptions.SynapseHTTPError:
                 raise ValueError("No access to resources. Please make sure that your token is correct")
         else:
             # login using synapse credentials provided by user in .synapseConfig (default) file
-            syn = synapseclient.Synapse(configPath=CONFIG.SYNAPSE_CONFIG_PATH)
+            syn = synapseclient.Synapse(configPath=CONFIG.synapse_configuration_path)
             syn.login(silent=True)
-            
         return syn
 
     def missing_entity_handler(method):
         def wrapper(*args, **kwargs):
             try:
                 return method(*args, **kwargs)
             except(SynapseHTTPError) as ex:
@@ -292,15 +265,14 @@
                 if 'trash' in str_message or 'does not exist' in str_message:
                     logging.warning(str_message)
                     return None
                 else:
                     raise ex
         return wrapper
 
-
     def getStorageFileviewTable(self):
         """ Returns the storageFileviewTable obtained during initialization.
         """
         return self.storageFileviewTable
 
     def getPaginatedRestResults(self, currentUserId: str) -> Dict[str, str]:
         """Gets the paginated results of the REST call to Synapse to check what projects the current user has access to.
@@ -597,21 +569,15 @@
         dataset_files = self.getFilesInStorageDataset(datasetId)
 
         # update manifest with additional filenames, if any
         # note that if there is an existing manifest and there are files in the dataset
         # the columns Filename and entityId are assumed to be present in manifest schema
         # TODO: use idiomatic panda syntax
         if dataset_files:
-            new_files = {"Filename": [], "entityId": []}
-
-            # find new files if any
-            for file_id, file_name in dataset_files:
-                if not file_id in manifest["entityId"].values:
-                    new_files["Filename"].append(file_name)
-                    new_files["entityId"].append(file_id)
+            new_files = self._get_file_entityIds(dataset_files=dataset_files, only_new_files=True, manifest=manifest)
 
             # update manifest so that it contain new files
             new_files = pd.DataFrame(new_files)
             manifest = (
                 pd.concat([manifest, new_files], sort=False)
                 .reset_index()
                 .drop("index", axis=1)
@@ -623,14 +589,46 @@
 
                 # store manifest and update associated metadata with manifest on Synapse
                 manifest_id = self.associateMetadataWithFiles(sg, manifest_filepath, datasetId)
 
         manifest = manifest.fillna("") 
         
         return manifest_id, manifest
+    
+    def _get_file_entityIds(self, dataset_files: List,  only_new_files: bool = False, manifest: pd.DataFrame = None):
+        """
+        Get a dictionary of files in a dataset. Either files that are not in the current manifest or all files
+        
+        Args:
+            manifest: metadata manifest
+            dataset_file: List of all files in a dataset
+            only_new_files: boolean to control whether only new files are returned or all files in the dataset
+        Returns:
+            files: dictionary of file names and entityIDs, with scope as specified by `only_new_files`
+        """
+        files = {"Filename": [], "entityId": []}
+
+        if only_new_files:
+            if manifest is None:
+                raise UnboundLocalError(
+                    "No manifest was passed in, a manifest is required when `only_new_files` is True."
+                )
+            
+            # find new files (that are not in the current manifest) if any
+            for file_id, file_name in dataset_files:
+                if not file_id in manifest["entityId"].values:
+                    files["Filename"].append(file_name)
+                    files["entityId"].append(file_id)
+        else:
+            # get all files
+            for file_id, file_name in dataset_files:
+                files["Filename"].append(file_name)
+                files["entityId"].append(file_id)
+
+        return files
 
     def getProjectManifests(self, projectId: str) -> List[str]:
         """Gets all metadata manifest files across all datasets in a specified project.
 
         Returns: A list of datasets per project; metadata manifest Synapse ID for each dataset; and the corresponding schema component of the manifest
                  as a list of tuples, one for each manifest:
                     [
@@ -991,25 +989,39 @@
             manifest_table_id: synID of the uploaded table
         
         """
         table_info = self.get_table_info(datasetId = datasetId)
         # Put table manifest onto synapse
         schema = Schema(name=table_name, columns=col_schema, parent=self.getDatasetProject(datasetId))
 
-        
+        if table_name in table_info:
+            existingTableId = table_info[table_name]
+        else:
+            existingTableId = None
+
+
+        tableOps = TableOperations(
+            synStore = self,  
+            tableToLoad = table_manifest,
+            tableName = table_name,
+            datasetId = datasetId, 
+            existingTableId = existingTableId,
+            restrict = restrict,
+            )
+
         if not table_manipulation or table_name not in table_info.keys():
-            manifest_table_id = TableOperations.createTable(self, tableToLoad=table_manifest, tableName=table_name, datasetId=datasetId, columnTypeDict=col_schema, specifySchema=True, restrict=restrict)
+            manifest_table_id = tableOps.createTable(columnTypeDict=col_schema, specifySchema=True,)
         elif table_name in table_info.keys() and table_info[table_name]:
 
             if table_manipulation.lower() == 'replace':
-                manifest_table_id = TableOperations.replaceTable(self, tableToLoad=table_manifest, tableName=table_name, existingTableId=table_info[table_name], specifySchema = True, datasetId = datasetId, columnTypeDict=col_schema, restrict=restrict)
+                manifest_table_id = tableOps.replaceTable(specifySchema = True, columnTypeDict=col_schema,)
             elif table_manipulation.lower() == 'upsert':
-                manifest_table_id = TableOperations.upsertTable(self, sg=sg, tableToLoad = table_manifest, tableName=table_name, existingTableId=table_info[table_name], datasetId=datasetId)
+                manifest_table_id = tableOps.upsertTable(sg=sg,)
             elif table_manipulation.lower() == 'update':
-                manifest_table_id = TableOperations.updateTable(self, tableToLoad=table_manifest, existingTableId=table_info[table_name], restrict=restrict)
+                manifest_table_id = tableOps.updateTable()
 
 
 
         if table_manipulation and table_manipulation.lower() == 'upsert':
             existing_tables=self.get_table_info(datasetId=datasetId)
             tableId=existing_tables[table_name]
             annos = self.syn.get_annotations(tableId)
@@ -1026,45 +1038,42 @@
         # store manifest to Synapse as a CSV
         # update file name
         file_name_full = metadataManifestPath.split('/')[-1]
         file_extension = file_name_full.split('.')[-1]
 
         # Differentiate "censored" and "uncensored" manifest
         if "censored" in file_name_full: 
-            file_name_new = os.path.basename(CONFIG["synapse"]["manifest_basename"]) + "_" + component_name + "_censored" + '.' + file_extension
+            file_name_new = os.path.basename(CONFIG.synapse_manifest_basename) + "_" + component_name + "_censored" + '.' + file_extension
         else: 
-            file_name_new = os.path.basename(CONFIG["synapse"]["manifest_basename"]) + "_" + component_name + '.' + file_extension
+            file_name_new = os.path.basename(CONFIG.synapse_manifest_basename) + "_" + component_name + '.' + file_extension
 
         manifestSynapseFile = File(
             metadataManifestPath,
             description="Manifest for dataset " + datasetId,
             parent=datasetId,
             name=file_name_new
         )
 
         manifest_synapse_file_id = self.syn.store(manifestSynapseFile, isRestricted = restrict_manifest).id
         changeFileMetaData(syn = self.syn, entity = manifest_synapse_file_id, downloadAs = file_name_new)
         
         return manifest_synapse_file_id
 
     @missing_entity_handler
-    def format_row_annotations(self, se, sg, row, entityId, useSchemaLabel, hideBlanks):
+    def format_row_annotations(self, se, sg, row, entityId, hideBlanks):
         # prepare metadata for Synapse storage (resolve display name into a name that Synapse annotations support (e.g no spaces, parenthesis)
         # note: the removal of special characters, will apply only to annotation keys; we are not altering the manifest
         # this could create a divergence between manifest column and annotations. this should be ok for most use cases.
         # columns with special characters are outside of the schema
         metadataSyn = {}
         blacklist_chars = ['(', ')', '.', ' ', '-']
         
         for k, v in row.to_dict().items():
 
-            if useSchemaLabel:
-                keySyn = se.get_class_label_from_display_name(str(k)).translate({ord(x): '' for x in blacklist_chars})
-            else:
-                keySyn = str(k)
+            keySyn = se.get_class_label_from_display_name(str(k)).translate({ord(x): '' for x in blacklist_chars})
 
             # Skip `Filename` and `ETag` columns when setting annotations
             if keySyn in ["Filename", "ETag", "eTag"]:
                 continue
 
             # truncate annotation values to 500 characters if the
             # size of values is greater than equal to 500 characters
@@ -1288,28 +1297,27 @@
             component_name = manifest['Component'][0].lower()
             table_name = component_name + '_synapse_storage_manifest_table'
         else:
             component_name = ''
             table_name = 'synapse_storage_manifest_table'
         return table_name, component_name
 
-    def _add_annotations(self, se, schemaGenerator, row, entityId, useSchemaLabel, hideBlanks):
+    def _add_annotations(self, se, schemaGenerator, row, entityId, hideBlanks):
         """Helper function to format and add annotations to entities in Synapse.
         Args:
             se: schemaExplorer object,
             schemaGenerator: schemaGenerator Object.
             row: current row of manifest being processed
             entityId (str): synapseId of entity to add annotations to
-            useSchemaLabel (bool): Flag to use schema label instead of display name
             hideBlanks: Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
         Returns:
             Annotations are added to entities in Synapse, no return.
         """
         # Format annotations for Synapse
-        annos = self.format_row_annotations(se, schemaGenerator, row, entityId, useSchemaLabel, hideBlanks)
+        annos = self.format_row_annotations(se, schemaGenerator, row, entityId, hideBlanks)
 
         if annos:
         # Store annotations for an entity folder
             self.syn.set_annotations(annos)
         return
 
     def _create_entity_id(self, idx, row, manifest, datasetId):
@@ -1334,32 +1342,42 @@
     def add_entities(
                     self,
                     se,
                     schemaGenerator,
                     manifest,
                     manifest_record_type,
                     datasetId,
-                    useSchemaLabel,
                     hideBlanks,
                     manifest_synapse_table_id=''
                     ):
         '''Depending on upload type add Ids to entityId row. Add anotations to connected files.
         Args:
             se: Schema Explorer Object
             schemaGenerator: SchemaGenerator object
             manifest (pd.DataFrame): loaded df containing user supplied data.
             manifest_record_type: valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
             datasetId (str): synapse ID of folder containing the dataset
-            useSchemaLabel (bool): Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
             hideBlanks (bool): Default is false -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
             manifest_synapse_table_id (str): Default is an empty string ''.
         Returns:
             manifest (pd.DataFrame): modified to add entitiyId as appropriate.
 
         '''
+
+        # Expected behavior is to annotate files if `Filename` is present regardless of `-mrt` setting
+        if 'filename' in [col.lower() for col in manifest.columns]:
+            # get current list of files and store as dataframe
+            dataset_files = self.getFilesInStorageDataset(datasetId)
+            files_and_entityIds = self._get_file_entityIds(dataset_files=dataset_files, only_new_files=False)
+            file_df = pd.DataFrame(files_and_entityIds)
+            
+            # Merge dataframes to add entityIds
+            manifest = manifest.merge(file_df, how = 'left', on='Filename', suffixes=['_x',None]).drop('entityId_x',axis=1)
+
+        # Fill `entityId` for each row if missing and annotate entity as appropriate
         for idx, row in manifest.iterrows():
             if not row["entityId"] and (manifest_record_type == 'file_and_entities' or 
                 manifest_record_type == 'table_file_and_entities'):
                 manifest, entityId = self._create_entity_id(idx, row, manifest, datasetId)
             elif not row["entityId"] and manifest_record_type == 'table_and_file':
                 # If not using entityIds, fill with manifest_table_id so 
                 row["entityId"] = manifest_synapse_table_id
@@ -1367,15 +1385,15 @@
                 entityId = ''
             else:
                 # get the entity id corresponding to this row
                 entityId = row["entityId"]
 
             # Adding annotations to connected files.
             if entityId:
-                self._add_annotations(se, schemaGenerator, row, entityId, useSchemaLabel, hideBlanks)
+                self._add_annotations(se, schemaGenerator, row, entityId, hideBlanks)
         return manifest
 
     def upload_manifest_as_table(
                             self,
                             se,
                             schemaGenerator,
                             manifest,
@@ -1396,15 +1414,14 @@
             manifest (pd.DataFrame): loaded df containing user supplied data.
             metadataManifestPath: path to csv containing a validated metadata manifest.
             datasetId (str): synapse ID of folder containing the dataset
             table_name (str): Generated to name the table being uploaded.
             component_name (str): Name of the component manifest that is currently being uploaded.
             restrict (bool): Flag for censored data.
             manifest_record_type (str): valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
-            useSchemaLabel(bool): Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
             hideBlanks (bool): Default is False -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
             table_malnipulation (str): Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
         Return:
             manifest_synapse_file_id: SynID of manifest csv uploaded to synapse.
         """      
         # Upload manifest as a table, get the ID and updated manifest.
         manifest_synapse_table_id, manifest, table_manifest = self.uploadDB(
@@ -1412,15 +1429,15 @@
                                                     manifest,
                                                     datasetId,
                                                     table_name,
                                                     restrict,
                                                     useSchemaLabel,
                                                     table_manipulation)
 
-        manifest = self.add_entities(se, schemaGenerator, manifest, manifest_record_type, datasetId, useSchemaLabel, hideBlanks, manifest_synapse_table_id)
+        manifest = self.add_entities(se, schemaGenerator, manifest, manifest_record_type, datasetId, hideBlanks, manifest_synapse_table_id)
         # Load manifest to synapse as a CSV File
         manifest_synapse_file_id = self.upload_manifest_file(manifest, metadataManifestPath, datasetId, restrict, component_name = component_name)
         
         # Set annotations for the file manifest.
         manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_file_id)
         self.syn.set_annotations(manifest_annotations)
         logger.info("Associated manifest file with dataset on Synapse.")
@@ -1445,36 +1462,34 @@
                             se,
                             schemaGenerator,
                             manifest,
                             metadataManifestPath,
                             datasetId,
                             restrict,
                             manifest_record_type,
-                            useSchemaLabel,
                             hideBlanks,
                             component_name,
                             with_entities = False,):
         """Upload manifest to Synapse as a csv only.
         Args:
             se: SchemaExplorer object
             schemaGenerator: SchemaGenerator Object
             manifest (pd.DataFrame): loaded df containing user supplied data.
             metadataManifestPath: path to csv containing a validated metadata manifest.
             datasetId (str): synapse ID of folder containing the dataset
             restrict (bool): Flag for censored data.
             manifest_record_type: valid values are 'entity', 'table' or 'both'. Specifies whether to create entity ids and folders for each row in a manifest, a Synapse table to house the entire manifest or do both.
-            useSchemaLabel (bool): Default is True - use the schema label. If False, uses the display label from the schema. Attribute display names in the schema must not only include characters that are not accepted by Synapse. Annotation names may only contain: letters, numbers, '_' and '.'.
             hideBlanks (bool): Default is False -Boolean flag that does not upload annotation keys with blank values when true. Uploads Annotation keys with empty string values when false.
             table_malnipulation (str): Specify the way the manifest tables should be store as on Synapse when one with the same name already exists. Options are 'replace' and 'upsert'.
             with_entities (bool): Default is False - Flag to indicate whether to create entityIds and add annotations.
         Return:
             manifest_synapse_file_id (str): SynID of manifest csv uploaded to synapse.
         """
         if with_entities:
-            manifest = self.add_entities(se, schemaGenerator, manifest, manifest_record_type, datasetId, useSchemaLabel, hideBlanks)
+            manifest = self.add_entities(se, schemaGenerator, manifest, manifest_record_type, datasetId, hideBlanks)
 
         # Load manifest to synapse as a CSV File
         manifest_synapse_file_id = self.upload_manifest_file(manifest,
                 metadataManifestPath, datasetId, restrict, component_name = component_name)
         
         # Set annotations for the file manifest.
         manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_file_id)
@@ -1521,15 +1536,15 @@
                                                     manifest,
                                                     datasetId,
                                                     table_name,
                                                     restrict,
                                                     useSchemaLabel=useSchemaLabel,
                                                     table_manipulation=table_manipulation,)
 
-        manifest = self.add_entities(se, schemaGenerator, manifest, manifest_record_type, datasetId, useSchemaLabel, hideBlanks, manifest_synapse_table_id)
+        manifest = self.add_entities(se, schemaGenerator, manifest, manifest_record_type, datasetId, hideBlanks, manifest_synapse_table_id)
         
         # Load manifest to synapse as a CSV File
         manifest_synapse_file_id = self.upload_manifest_file(manifest, metadataManifestPath, datasetId, restrict, component_name)
         
         # Set annotations for the file manifest.
         manifest_annotations = self.format_manifest_annotations(manifest, manifest_synapse_file_id)
         self.syn.set_annotations(manifest_annotations)
@@ -1595,15 +1610,14 @@
             manifest_synapse_file_id = self.upload_manifest_as_csv(
                                         se,
                                         schemaGenerator,
                                         manifest,
                                         metadataManifestPath,
                                         datasetId=datasetId,
                                         restrict=restrict_manifest,
-                                        useSchemaLabel=useSchemaLabel,
                                         hideBlanks=hideBlanks,
                                         manifest_record_type=manifest_record_type,
                                         component_name = component_name,
                                         with_entities = False,
                                         )
         elif manifest_record_type == "table_and_file":
             manifest_synapse_file_id = self.upload_manifest_as_table(
@@ -1624,15 +1638,14 @@
             manifest_synapse_file_id = self.upload_manifest_as_csv( 
                                         se,
                                         schemaGenerator,
                                         manifest,
                                         metadataManifestPath,
                                         datasetId=datasetId,
                                         restrict=restrict_manifest,
-                                        useSchemaLabel=useSchemaLabel,
                                         hideBlanks=hideBlanks,
                                         manifest_record_type=manifest_record_type,
                                         component_name = component_name,
                                         with_entities=True,
                                         )
         elif manifest_record_type == "table_file_and_entities":
             manifest_synapse_file_id = self.upload_manifest_combo(
@@ -1924,46 +1937,66 @@
     createTable: upload a manifest as a new table when none exist
     replaceTable: replace a metadata in a table from one manifest with metadata from another manifest
     updateTable: add a column to a table that already exists on synapse
 
     Operations currently in development are:
     upsertTable: add metadata from a manifest to an existing table that contains metadata from another manifest
     """
+    def __init__(self, 
+                 synStore: SynapseStorage, 
+                 tableToLoad: pd.DataFrame = None, 
+                 tableName: str = None, 
+                 datasetId: str = None, 
+                 existingTableId: str = None,
+                 restrict: bool = False
+                 ):
+        
+        """
+        Class governing table operations (creation, replacement, upserts, updates) in schematic
+
+        tableToLoad: manifest formatted appropriately for the table
+        tableName: name of the table to be uploaded
+        datasetId: synID of the dataset for the manifest
+        existingTableId: synId of the table currently exising on synapse (if there is one)
+        restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
+
+        """
+        self.synStore = synStore
+        self.tableToLoad = tableToLoad
+        self.tableName = tableName
+        self.datasetId = datasetId
+        self.existingTableId = existingTableId
+        self.restrict = restrict
 
 
-    def createTable(synStore: SynapseStorage, tableToLoad: pd.DataFrame = None, tableName: str = None, datasetId: str = None, columnTypeDict: dict = None, specifySchema: bool = True, restrict: bool = False):
+    def createTable(self, columnTypeDict: dict = None, specifySchema: bool = True,):
         """
         Method to create a table from a metadata manifest and upload it to synapse
         
         Args:
-            tableToLoad: manifest formatted appropriately for the table
-            tableName: name of the table to be uploaded
-            datasetId: synID of the dataset for the manifest
             columnTypeDict: dictionary schema for table columns: type, size, etc
-            specifySchema: to specify a specific schema for the table format          
-            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
-            
+            specifySchema: to specify a specific schema for the table format                      
 
         Returns:
             table.schema.id: synID of the newly created table
         """
 
-        datasetEntity = synStore.syn.get(datasetId, downloadFile = False)
+        datasetEntity = self.synStore.syn.get(self.datasetId, downloadFile = False)
         datasetName = datasetEntity.name
-        table_schema_by_cname = synStore._get_table_schema_by_cname(columnTypeDict) 
+        table_schema_by_cname = self.synStore._get_table_schema_by_cname(columnTypeDict) 
 
-        if not tableName:
-            tableName = datasetName + 'table'
-        datasetParentProject = synStore.getDatasetProject(datasetId)
+        if not self.tableName:
+            self.tableName = datasetName + 'table'
+        datasetParentProject = self.synStore.getDatasetProject(self.datasetId)
         if specifySchema:
             if columnTypeDict == {}:
                 logger.error("Did not provide a columnTypeDict.")
             #create list of columns:
             cols = []
-            for col in tableToLoad.columns:
+            for col in self.tableToLoad.columns:
                 if col in table_schema_by_cname:
                     col_type = table_schema_by_cname[col]['columnType']
                     max_size = table_schema_by_cname[col]['maximumSize'] if 'maximumSize' in table_schema_by_cname[col].keys() else 100
                     max_list_len = 250
                     if max_size and max_list_len:
                         cols.append(Column(name=col, columnType=col_type, 
                             maximumSize=max_size, maximumListLength=max_list_len))
@@ -1971,70 +2004,64 @@
                         cols.append(Column(name=col, columnType=col_type, 
                             maximumSize=max_size))
                     else:
                         cols.append(Column(name=col, columnType=col_type))
                 else:
                     #TODO add warning that the given col was not found and it's max size is set to 100
                     cols.append(Column(name=col, columnType='STRING', maximumSize=100))
-            schema = Schema(name=tableName, columns=cols, parent=datasetParentProject)
-            table = Table(schema, tableToLoad)
-            table = synStore.syn.store(table, isRestricted = restrict)
+            schema = Schema(name=self.tableName, columns=cols, parent=datasetParentProject)
+            table = Table(schema, self.tableToLoad)
+            table = self.synStore.syn.store(table, isRestricted = self.restrict)
             return table.schema.id
         else:
             # For just uploading the tables to synapse using default
             # column types.
-            table = build_table(tableName, datasetParentProject, tableToLoad)
-            table = synStore.syn.store(table, isRestricted = restrict)
+            table = build_table(self.tableName, datasetParentProject, self.tableToLoad)
+            table = self.synStore.syn.store(table, isRestricted = self.restrict)
             return table.schema.id
 
-    def replaceTable(synStore: SynapseStorage, tableToLoad: pd.DataFrame = None, tableName: str = None, existingTableId: str = None, specifySchema: bool = True, datasetId: str = None, columnTypeDict: dict = None, restrict: bool = False):
+    def replaceTable(self, specifySchema: bool = True, columnTypeDict: dict = None,):
         """
         Method to replace an existing table on synapse with metadata from a new manifest
         
         Args:
-            tableToLoad: manifest formatted appropriately for the table
-            tableName: name of the table to be uploaded
-            existingTableId: synId of the existing table to be replaced
             specifySchema: to infer a schema for the table format      
-            datasetId: synID of the dataset for the manifest    
-            columnTypeDict: dictionary schema for table columns: type, size, etc
-            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
-            
+            columnTypeDict: dictionary schema for table columns: type, size, etc            
 
         Returns:
            existingTableId: synID of the already existing table that had its metadata replaced
         """
-        datasetEntity = synStore.syn.get(datasetId, downloadFile = False)
+        datasetEntity = self.synStore.syn.get(self.datasetId, downloadFile = False)
         datasetName = datasetEntity.name
-        table_schema_by_cname = synStore._get_table_schema_by_cname(columnTypeDict) 
-        existing_table, existing_results = synStore.get_synapse_table(existingTableId)
+        table_schema_by_cname = self.synStore._get_table_schema_by_cname(columnTypeDict) 
+        existing_table, existing_results = self.synStore.get_synapse_table(self.existingTableId)
         # remove rows
-        synStore.syn.delete(existing_results)
+        self.synStore.syn.delete(existing_results)
         # wait for row deletion to finish on synapse before getting empty table
         sleep(10)
         
         # removes all current columns
-        current_table = synStore.syn.get(existingTableId)
-        current_columns = synStore.syn.getTableColumns(current_table)
+        current_table = self.synStore.syn.get(self.existingTableId)
+        current_columns = self.synStore.syn.getTableColumns(current_table)
         for col in current_columns:
             current_table.removeColumn(col)
 
-        if not tableName:
-            tableName = datasetName + 'table'
+        if not self.tableName:
+            self.tableName = datasetName + 'table'
         
         # Process columns according to manifest entries
-        table_schema_by_cname = synStore._get_table_schema_by_cname(columnTypeDict) 
-        datasetParentProject = synStore.getDatasetProject(datasetId)
+        table_schema_by_cname = self.synStore._get_table_schema_by_cname(columnTypeDict) 
+        datasetParentProject = self.synStore.getDatasetProject(self.datasetId)
         if specifySchema:
             if columnTypeDict == {}:
                 logger.error("Did not provide a columnTypeDict.")
             #create list of columns:
             cols = []
             
-            for col in tableToLoad.columns:
+            for col in self.tableToLoad.columns:
                 
                 if col in table_schema_by_cname:
                     col_type = table_schema_by_cname[col]['columnType']
                     max_size = table_schema_by_cname[col]['maximumSize'] if 'maximumSize' in table_schema_by_cname[col].keys() else 100
                     max_list_len = 250
                     if max_size and max_list_len:
                         cols.append(Column(name=col, columnType=col_type, 
@@ -2048,214 +2075,175 @@
                     
                     #TODO add warning that the given col was not found and it's max size is set to 100
                     cols.append(Column(name=col, columnType='STRING', maximumSize=100))
             
             # adds new columns to schema
             for col in cols:
                 current_table.addColumn(col)
-            synStore.syn.store(current_table, isRestricted = restrict)
+            self.synStore.syn.store(current_table, isRestricted = self.restrict)
 
             # wait for synapse store to finish
             sleep(1)
 
             # build schema and table from columns and store with necessary restrictions
-            schema = Schema(name=tableName, columns=cols, parent=datasetParentProject)
-            schema.id = existingTableId
-            table = Table(schema, tableToLoad, etag = existing_results.etag)
-            table = synStore.syn.store(table, isRestricted = restrict)
+            schema = Schema(name=self.tableName, columns=cols, parent=datasetParentProject)
+            schema.id = self.existingTableId
+            table = Table(schema, self.tableToLoad, etag = existing_results.etag)
+            table = self.synStore.syn.store(table, isRestricted = self.restrict)
         else:
             logging.error("Must specify a schema for table replacements")
 
         # remove system metadata from manifest
         existing_table.drop(columns = ['ROW_ID', 'ROW_VERSION'], inplace = True)
-        return existingTableId
+        return self.existingTableId
     
 
-    def _get_schematic_db_creds(synStore: SynapseStorage):
-        username = None
+    def _get_auth_token(self,):
         authtoken = None
 
-
         # Get access token from environment variable if available
         # Primarily useful for testing environments, with other possible usefulness for containers
         env_access_token = os.getenv("SYNAPSE_ACCESS_TOKEN")
         if env_access_token:
             authtoken = env_access_token
-            return username, authtoken
+            return authtoken
 
         # Get token from authorization header
         # Primarily useful for API endpoint functionality
-        if 'Authorization' in synStore.syn.default_headers:
-            authtoken = synStore.syn.default_headers['Authorization'].split('Bearer ')[-1]
-            return username, authtoken
+        if 'Authorization' in self.synStore.syn.default_headers:
+            authtoken = self.synStore.syn.default_headers['Authorization'].split('Bearer ')[-1]
+            return authtoken
 
         # retrive credentials from synapse object
         # Primarily useful for local users, could only be stored here when a .synapseConfig file is used, but including to be safe
-        synapse_object_creds = synStore.syn.credentials
-        if hasattr(synapse_object_creds, 'username'):
-            username = synapse_object_creds.username
+        synapse_object_creds = self.synStore.syn.credentials
         if hasattr(synapse_object_creds, '_token'):
             authtoken = synapse_object_creds.secret
 
         # Try getting creds from .synapseConfig file if it exists
         # Primarily useful for local users. Seems to correlate with credentials stored in synaspe object when logged in
-        if os.path.exists(CONFIG.SYNAPSE_CONFIG_PATH):
-            config = synStore.syn.getConfigFile(CONFIG.SYNAPSE_CONFIG_PATH)
+        if os.path.exists(CONFIG.synapse_configuration_path):
+            config = self.synStore.syn.getConfigFile(CONFIG.synapse_configuration_path)
 
             # check which credentials are provided in file
-            if config.has_option('authentication', 'username'):
-                username = config.get('authentication', 'username')
             if config.has_option('authentication', 'authtoken'):
                 authtoken = config.get('authentication', 'authtoken')
         
         # raise error if required credentials are not found
-        # providing an authtoken without a username did not prohibit upsert functionality, 
-        # but including username gathering for completeness for schematic_db
-        if not username and not authtoken:
-            raise NameError(
-                "Username and authtoken credentials could not be found in the environment, synapse object, or the .synapseConfig file"
-            )
         if not authtoken:
             raise NameError(
                 "authtoken credentials could not be found in the environment, synapse object, or the .synapseConfig file"
             )
         
-        return username, authtoken
+        return authtoken
 
-    def upsertTable(synStore: SynapseStorage, sg: SchemaGenerator, tableToLoad: pd.DataFrame = None, tableName: str = None, existingTableId: str = None,  datasetId: str = None):
+    def upsertTable(self, sg: SchemaGenerator,):
         """
         Method to upsert rows from a new manifest into an existing table on synapse
         For upsert functionality to work, primary keys must follow the naming convention of <componenet>_id        
         `-tm upsert` should be used for initial table uploads if users intend to upsert into them at a later time; using 'upsert' at creation will generate the metadata necessary for upsert functionality.
         Currently it is required to use -dl/--use_display_label with table upserts.
         
 
         Args:
-            tableToLoad: manifest formatted appropriately for the table
-            tableName: name of the table to be uploaded
-            existingTableId: synId of the existing table to be replaced     
-            datasetId: synID of the dataset for the manifest    
-            columnTypeDict: dictionary schema for table columns: type, size, etc
+            sg: SchemaGenerator instance
             
-
         Returns:
            existingTableId: synID of the already existing table that had its metadata replaced
         """            
 
-        username, authtoken = TableOperations._get_schematic_db_creds(synStore)
+        authtoken = self._get_auth_token()
 
-        synConfig = SynapseConfig(username, authtoken, synStore.getDatasetProject(datasetId))
-        synapseDB = SynapseDatabase(synConfig)
+        synapseDB = SynapseDatabase(auth_token=authtoken, project_id=self.synStore.getDatasetProject(self.datasetId))
 
         try:
             # Try performing upsert
-            synapseDB.upsert_table_rows(table_name=tableName, data=tableToLoad)
+            synapseDB.upsert_table_rows(table_name=self.tableName, data=self.tableToLoad)
         except(SynapseHTTPError) as ex:
             # If error is raised because Table has old `Uuid` column and not new `Id` column, then handle and re-attempt upload
             if 'Id is not a valid column name or id' in str(ex):
-                TableOperations._update_table_uuid_column(synStore, existingTableId, sg)
-                synapseDB.upsert_table_rows(table_name=tableName, data=tableToLoad)
+                self._update_table_uuid_column(sg)
+                synapseDB.upsert_table_rows(table_name=self.tableName, data=self.tableToLoad)
             # Raise if other error
             else:
                 raise ex
 
-        return existingTableId
-
-    def _update_table_uuid_column(synStore: SynapseStorage, table_id: str, sg: SchemaGenerator,) -> None:
+        return self.existingTableId
+    
+    def _update_table_uuid_column(self, sg: SchemaGenerator,) -> None:
         """Removes the `Uuid` column when present, and relpaces with an `Id` column
         Used to enable backwards compatability for manifests using the old `Uuid` convention
 
         Args:
-            table_id (str): The Synapse id of the table to be upserted into, that needs columns updated
+            sg: SchemaGenerator instance
 
         Returns:
             None
         """
 
         # Get the columns of the schema
-        schema = synStore.syn.get(table_id)
-        cols = synStore.syn.getTableColumns(schema)
+        schema = self.synStore.syn.get(self.existingTableId)
+        cols = self.synStore.syn.getTableColumns(schema)
         
         # Iterate through columns until `Uuid` column is found
         for col in cols:
             if col.name.lower() == 'uuid':
                 # See if schema has `Uuid` column specified
                 try:
                     uuid_col_in_schema = sg.se.is_class_in_schema(col.name)      
                 except (KeyError):
                     uuid_col_in_schema = False
 
                 # If there is, then create a new `Id` column from scratch
                 if uuid_col_in_schema:
                     new_col = Column(columnType = "STRING", maximumSize = 64, name = "Id")
                     schema.addColumn(new_col)
-                    schema = synStore.syn.store(schema)
+                    schema = self.synStore.syn.store(schema)
                 # If there is not, then use the old `Uuid` column as a basis for the new `Id` column
                 else:
-                    # Create a new `Id` column based off of the old `Uuid` column, and store (column is empty)
-                    new_col = deepcopy(col)
-                    new_col['name'] = 'Id'
-                    schema.addColumn(new_col)
-                    schema = synStore.syn.store(schema)
-                
-                
-                    # Recently stored column is empty, so populated with uuid values
-                    TableOperations._populate_new_id_column(synStore, table_id, schema)
-
-                    # get the up-to-date table, remove old `Uuid` column, and store
-                    sleep(1)
-                    schema = synStore.syn.get(table_id)
-                    schema.removeColumn(col)
-                    schema = synStore.syn.store(schema)
+                    
+                    # Build ColumnModel that will be used for new column
+                    id_column = Column(name='Id', columnType='STRING', maximumSize=64, defaultValue=None, maximumListLength=1)
+                    new_col_response = self.synStore.syn.store(id_column)
+
+
+                    # Define columnChange body
+                    columnChangeDict = {
+                        "concreteType": "org.sagebionetworks.repo.model.table.TableSchemaChangeRequest",
+                        "entityId": self.existingTableId,
+                        "changes": [
+                            {                        
+                                "oldColumnId": col['id'],
+                                "newColumnId": new_col_response['id'],
+                            }
+                        ]
+                    }
 
-                    # Exit iteration; only concerned with `Uuid` column
+                    self.synStore.syn._async_table_update(table=self.existingTableId, changes=[columnChangeDict], wait=False)
                 break
 
         return
 
-    def _populate_new_id_column(synStore: SynapseStorage, table_id: str, schema: Schema) -> None:
-        """Copies the uuid values that were present in the column named `Uuid` to the new column named `Id`
-
-        Args:
-            table_id (str): The Synapse id of the table to be upserted into, that needs columns updated
-            schema (synapseclient.table.Schema): Schema of the table columns
-
-        Returns:
-            None
-        """
-        # Query the table for the old `Uuid` column and new `Id` column
-        results = synStore.syn.tableQuery(f"select Uuid,Id from {table_id}")
-        results_df = results.asDataFrame()
-
-        # Copy uuid values to new column, and store in table
-        results_df = populate_df_col_with_another_col(results_df, 'Uuid', 'Id')
-        table = synStore.syn.store(Table(schema, results_df, etag=results.etag))
-        return
-
-    def updateTable(synStore: SynapseStorage, tableToLoad: pd.DataFrame = None, existingTableId: str = None,  update_col: str = 'Id',  restrict: bool = False):
+    def updateTable(self, update_col: str = 'Id',):
         """
         Method to update an existing table with a new column
         
         Args:
-            tableToLoad: manifest formatted appropriately for the table, that contains the new column
-            existingTableId: synId of the existing table to be replaced
-            updateCol: column to index the old and new tables on
-            restrict: bool, whether or not the manifest contains sensitive data that will need additional access restrictions 
-            
+            updateCol: column to index the old and new tables on            
 
         Returns:
            existingTableId: synID of the already existing table that had its metadata replaced
         """
-        existing_table, existing_results = synStore.get_synapse_table(existingTableId)
+        existing_table, existing_results = self.synStore.get_synapse_table(self.existingTableId)
         
-        tableToLoad = update_df(existing_table, tableToLoad, update_col)
+        self.tableToLoad = update_df(existing_table, self.tableToLoad, update_col)
         # store table with existing etag data and impose restrictions as appropriate
-        synStore.syn.store(Table(existingTableId, tableToLoad, etag = existing_results.etag), isRestricted = restrict)
+        self.synStore.syn.store(Table(self.existingTableId, self.tableToLoad, etag = existing_results.etag), isRestricted = self.restrict)
 
-        return existingTableId
+        return self.existingTableId
 
 
 class DatasetFileView:
     """Helper class to create temporary dataset file views.
     This class can be used in conjunction with a 'with' statement.
     This will ensure that the file view is deleted automatically.
     See SynapseStorage.getDatasetAnnotationsBatch for example usage.
```

### Comparing `schematicpy-23.6.3/schematic/utils/curie_utils.py` & `schematicpy-23.7.1/schematic/utils/curie_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/utils/df_utils.py` & `schematicpy-23.7.1/schematic/utils/df_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,25 +56,28 @@
         if org_df.size < large_manifest_cutoff_size:  # If small manifest, iterate as normal for improved performance
             ints = org_df.applymap(lambda x: np.int64(x) if str.isdigit(x) else False, na_action='ignore').fillna(False)
 
         else:   # parallelize iterations for large manfiests
             pandarallel.initialize(verbose = 1)
             ints = org_df.parallel_applymap(lambda x: np.int64(x) if str.isdigit(x) else False, na_action='ignore').fillna(False)
 
+        # Identify cells converted to intergers
+        ints_tf_df = ints.applymap(pd.api.types.is_integer)
+
         # convert strings to numerical dtype (float) if possible, preserve non-numerical strings
         for col in org_df.columns:
             float_df[col]=pd.to_numeric(float_df[col], errors='coerce')
             # replace values that couldn't be converted to float with the original str values
             float_df[col].fillna(org_df[col][float_df[col].isna()],inplace=True)
         
         # Trim nans and empty rows and columns
         processed_df = trim_commas_df(float_df)
-        
+
         # Store values that were converted to type int in the final dataframe
-        processed_df=processed_df.mask(ints != False, other = ints)  
+        processed_df=processed_df.mask(ints_tf_df, other = ints)
         
         # log manifest load and processing time
         logger.debug(f"Load Elapsed time {perf_counter()-t_load_df}")
         return processed_df
 
 
 def _parse_dates(date_string):
```

### Comparing `schematicpy-23.6.3/schematic/utils/general.py` & `schematicpy-23.7.1/schematic/utils/general.py`

 * *Files 14% similar despite different names*

```diff
@@ -179,7 +179,23 @@
                         ps.sort_stats(sort_by)
                     ps.print_stats(lines_to_print)
             return retval
 
         return wrapper
 
     return inner
+
+def normalize_path(path: str, parent_folder: str) -> str:
+    """
+    Normalizes a path.
+    If the path is relative, the parent_folder is added to make it an absolute path.
+
+    Args:
+        path (str): The path to the file to normalize.
+        parent_folder (str): The folder the file is in.
+
+    Returns:
+        str: The normalized path.
+    """
+    if not os.path.isabs(path):
+        path = os.path.join(parent_folder, path)
+    return os.path.normpath(path)
```

### Comparing `schematicpy-23.6.3/schematic/utils/google_api_utils.py` & `schematicpy-23.7.1/schematic/utils/google_api_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,51 +7,27 @@
 from typing import Dict, Any
 
 from googleapiclient.discovery import build
 from google_auth_oauthlib.flow import InstalledAppFlow
 from google.auth.transport.requests import Request
 from google.oauth2 import service_account
 from google.oauth2.credentials import Credentials
-from schematic import CONFIG
+from schematic.configuration.configuration import CONFIG
 from schematic.store.synapse import SynapseStorage
 import pandas as pd
 
 logger = logging.getLogger(__name__)
 
 
 # If modifying these scopes, delete the file token.pickle.
 SCOPES = [
     "https://www.googleapis.com/auth/spreadsheets",
     "https://www.googleapis.com/auth/drive",
 ]
 
-
-# it will create 'token.pickle' based on credentials.json
-def generate_token() -> Credentials:
-    creds = None
-    # The file token.pickle stores the user's access and refresh tokens,
-    # and is created automatically when the authorization flow completes for the first time.
-    if os.path.exists(CONFIG.TOKEN_PICKLE):
-        with open(CONFIG.TOKEN_PICKLE, "rb") as token:
-            creds = pickle.load(token)
-
-    # If there are no (valid) credentials available, let the user log in.
-    if not creds or not creds.valid:
-        if creds and creds.expired and creds.refresh_token:
-            creds.refresh(Request())
-        else:
-            flow = InstalledAppFlow.from_client_secrets_file(CONFIG.CREDS_PATH, SCOPES)
-            creds = flow.run_console()  ### don't have to deal with ports
-        # Save the credentials for the next run
-        with open(CONFIG.TOKEN_PICKLE, "wb") as token:
-            pickle.dump(creds, token)
-
-    return creds
-
-
 # TODO: replace by pygsheets calls?
 def build_credentials() -> Dict[str, Any]:
     creds = generate_token()
 
     # get a Google Sheet API service
     sheet_service = build("sheets", "v4", credentials=creds)
     # get a Google Drive API service
@@ -72,15 +48,15 @@
     # for AWS deployment
     elif "SECRETS_MANAGER_SECRETS" in os.environ:
         all_secrets_dict =json.loads(os.environ["SECRETS_MANAGER_SECRETS"])
         dict_creds=json.loads(all_secrets_dict["SERVICE_ACCOUNT_CREDS"])
         credentials = service_account.Credentials.from_service_account_info(dict_creds, scopes=SCOPES)
     else:
         credentials = service_account.Credentials.from_service_account_file(
-            CONFIG.SERVICE_ACCT_CREDS, scopes=SCOPES
+            CONFIG.service_account_credentials_path, scopes=SCOPES
         )
 
     # get a Google Sheet API service
     sheet_service = build("sheets", "v4", credentials=credentials)
     # get a Google Drive API service
     drive_service = build("drive", "v3", credentials=credentials)
 
@@ -93,29 +69,29 @@
 
 def download_creds_file() -> None:
     syn = SynapseStorage.login()
 
     # if file path of service_account does not exist
     # and if an environment variable related to service account is not found
     # regenerate service_account credentials
-    if not os.path.exists(CONFIG.SERVICE_ACCT_CREDS) and "SERVICE_ACCOUNT_CREDS" not in os.environ:
+    if not os.path.exists(CONFIG.service_account_credentials_path) and "SERVICE_ACCOUNT_CREDS" not in os.environ:
 
         # synapse ID of the 'schematic_service_account_creds.json' file
-        API_CREDS = CONFIG["synapse"]["service_acct_creds"]
+        API_CREDS = CONFIG.service_account_credentials_synapse_id
 
         # Download in parent directory of SERVICE_ACCT_CREDS to
         # ensure same file system for os.rename()
-        creds_dir = os.path.dirname(CONFIG.SERVICE_ACCT_CREDS)
+        creds_dir = os.path.dirname(CONFIG.service_account_credentials_path)
 
         creds_file = syn.get(API_CREDS, downloadLocation=creds_dir)
-        os.rename(creds_file.path, CONFIG.SERVICE_ACCT_CREDS)
+        os.rename(creds_file.path, CONFIG.service_account_credentials_path)
 
         logger.info(
             "The credentials file has been downloaded "
-            f"to '{CONFIG.SERVICE_ACCT_CREDS}'"
+            f"to '{CONFIG.service_account_credentials_path}'"
         )
 
     elif "SERVICE_ACCOUNT_CREDS" in os.environ:
         # remind users that "SERVICE_ACCOUNT_CREDS" as an environment variable is being used
         logger.info(
             "Using environment variable SERVICE_ACCOUNT_CREDS as the credential file."
         )
```

### Comparing `schematicpy-23.6.3/schematic/utils/io_utils.py` & `schematicpy-23.7.1/schematic/utils/io_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import json
 import urllib.request
 
-from schematic import CONFIG, LOADER
+from schematic import LOADER
 
 
 def load_json(file_path):
     """Load json document from file path or url
 
     :arg str file_path: The path of the url doc, could be url or file path
     """
```

### Comparing `schematicpy-23.6.3/schematic/utils/schema_utils.py` & `schematicpy-23.7.1/schematic/utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/utils/validate_rules_utils.py` & `schematicpy-23.7.1/schematic/utils/validate_rules_utils.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/utils/validate_utils.py` & `schematicpy-23.7.1/schematic/utils/validate_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import pandas as pd
 from jsonschema import validate
 from re import compile, search, IGNORECASE
 from schematic.utils.io_utils import load_json
-from schematic import CONFIG, LOADER
+from schematic import LOADER
 from typing import List
 import numpy as np
 
 def validate_schema(schema):
     """Validate schema against schema.org standard"""
     data_path = "validation_schemas/model.schema.json"
     json_schema_path = LOADER.filename(data_path)
```

### Comparing `schematicpy-23.6.3/schematic/visualization/attributes_explorer.py` & `schematicpy-23.7.1/schematic/visualization/attributes_explorer.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/schematic/visualization/commands.py` & `schematicpy-23.7.1/schematic/visualization/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import sys
 
 import click
 import click_log
 
 from schematic.visualization.attributes_explorer import AttributesExplorer
 from schematic.visualization.tangled_tree import TangledTree
-from schematic.utils.cli_utils import get_from_config, fill_in_from_config, query_dict
+from schematic.utils.cli_utils import log_value_from_config, query_dict
 from schematic.help import viz_commands
 from schematic.help import model_commands
-from schematic import CONFIG
+from schematic.configuration.configuration import CONFIG
 
 logger = logging.getLogger(__name__)
 click_log.basic_config(logger)
 
 CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])  # help options
 
 # invoke_without_command=True -> forces the application not to show aids before losing them with a --h
@@ -31,15 +31,16 @@
 @click.pass_context
 def viz(ctx, config):  # use as `schematic model ...`
     """
     Sub-commands for Visualization methods.
     """
     try:
         logger.debug(f"Loading config file contents in '{config}'")
-        ctx.obj = CONFIG.load_config(config)
+        CONFIG.load_config(config)
+        ctx.obj =  CONFIG
     except ValueError as e:
         logger.error("'--config' not provided or environment variable not set.")
         logger.exception(e)
         sys.exit(1)
 
 @viz.command(
     "attributes",
@@ -48,15 +49,16 @@
 
 @click.pass_obj
 def get_attributes(ctx):
     """
     
     """
     # Get JSONLD file path
-    path_to_jsonld = get_from_config(CONFIG.DATA, ("model", "input", "location"))
+    path_to_jsonld = CONFIG.model_location
+    log_value_from_config("jsonld", path_to_jsonld)
     # Run attributes explorer
     AttributesExplorer(path_to_jsonld).parse_attributes(save_file=True)
     return
 
 @viz.command(
     "tangled_tree_text"
 )
@@ -75,15 +77,16 @@
 )
 
 @click.pass_obj
 def get_tangled_tree_text(ctx, figure_type, text_format):
     """ Get text to be placed on the tangled tree visualization.
     """
     # Get JSONLD file path
-    path_to_jsonld = get_from_config(CONFIG.DATA, ("model", "input", "location"))
+    path_to_jsonld = CONFIG.model_location
+    log_value_from_config("jsonld", path_to_jsonld)
     
     # Initialize TangledTree
     tangled_tree = TangledTree(path_to_jsonld, figure_type)
 
     # Get text for tangled tree.
     text_df = tangled_tree.get_text_for_tangled_tree(text_format, save_file=True)
     return
@@ -100,15 +103,16 @@
 )
 
 @click.pass_obj
 def get_tangled_tree_component_layers(ctx, figure_type):
     ''' Get the components that belong in each layer of the tangled tree visualization.
     '''
     # Get JSONLD file path
-    path_to_jsonld = get_from_config(CONFIG.DATA, ("model", "input", "location"))
+    path_to_jsonld = CONFIG.model_location
+    log_value_from_config("jsonld", path_to_jsonld)
     
     # Initialize Tangled Tree
     tangled_tree = TangledTree(path_to_jsonld, figure_type)
     
     # Get tangled trees layers JSON.
     layers = tangled_tree.get_tangled_tree_layers(save_file=True)
```

### Comparing `schematicpy-23.6.3/schematic/visualization/tangled_tree.py` & `schematicpy-23.7.1/schematic/visualization/tangled_tree.py`

 * *Files identical despite different names*

### Comparing `schematicpy-23.6.3/PKG-INFO` & `schematicpy-23.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schematicpy
-Version: 23.6.3
+Version: 23.7.1
 Summary: Package for biomedical data model and metadata ingress management
 Home-page: https://github.com/Sage-Bionetworks/schematic
 Keywords: schema,metadata,validation,data model,linked data
 Author: Milen Nikolov
 Author-email: milen.nikolov@sagebase.org
 Requires-Python: >=3.9.0,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -38,15 +38,15 @@
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
 Requires-Dist: pandarallel (>=1.6.4,<2.0.0)
 Requires-Dist: pandas (>=1.3.1,<2.0.0)
 Requires-Dist: pdoc (>=12.2.0,<13.0.0)
 Requires-Dist: pygsheets (>=2.0.4,<3.0.0)
 Requires-Dist: pyopenssl (>=23.0.0,<24.0.0)
 Requires-Dist: rdflib (>=6.0.0,<7.0.0)
-Requires-Dist: schematic-db[synapse] (>=0.0.20,<0.0.21)
+Requires-Dist: schematic-db[synapse] (>=0.0.29,<0.0.30)
 Requires-Dist: setuptools (>=66.0.0,<67.0.0)
 Requires-Dist: sphinx-click (>=4.0.0,<5.0.0)
 Requires-Dist: synapseclient (>=2.7.0,<3.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typing-extensions (<4.6.0)
 Project-URL: Documentation, https://github.com/Sage-Bionetworks/schematic
@@ -139,53 +139,77 @@
 editor of your choice and edit the `username` and `authtoken` attribute under the `authentication` section 
 
 *Note*: You could also visit [configparser](https://docs.python.org/3/library/configparser.html#module-configparser>) doc to see the format that `.synapseConfig` must have. For instance:
 >[authentication]<br> username = ABC <br> authtoken = abc
 
 <strong>Configure config.yml File</strong>
 
-*Note*: Below is only a brief explanation of some attributes in `config.yml`. <strong>Please use the link [here](https://github.com/Sage-Bionetworks/schematic/blob/develop/config.yml) to get the latest version of `config.yml` in `develop` branch</strong>.
+There are some defaults in schematic that can be configured. These fields are in ``config_example.yml``:
 
-Description of `config.yml` attributes
+```text
 
-    definitions:
-        synapse_config: "~/path/to/.synapseConfig"
-        service_acct_creds: "~/path/to/service_account_creds.json"
-
-    synapse:
-        master_fileview: "syn23643253" # fileview of project with datasets on Synapse
-        manifest_folder: "~/path/to/manifest_folder/" # manifests will be downloaded to this folder
-        manifest_basename: "filename" # base name of the manifest file in the project dataset, without extension
-        service_acct_creds: "syn25171627" # synapse ID of service_account_creds.json file
-
-    manifest:
-        title: "example" # title of metadata manifest file
-        # to make all manifests enter only 'all manifests'
-        data_type: 
-          - "Biospecimen"
-          - "Patient"
-
-    model:
-        input:
-            location: "data/schema_org_schemas/example.jsonld" # path to JSON-LD data model
-            file_type: "local" # only type "local" is supported currently
-    style: # configuration of google sheet
-        google_manifest:
-          req_bg_color:
-            red: 0.9215
-            green: 0.9725
-            blue: 0.9803
-          opt_bg_color:
-            red: 1.0
-            green: 1.0
-            blue: 0.9019
-          master_template_id: '1LYS5qE4nV9jzcYw5sXwCza25slDfRA1CIg3cs-hCdpU'
-          strict_validation: true
+# This is an example config for Schematic.
+# All listed values are those that are the default if a config is not used.
+# Save this as config.yml, this will be gitignored.
+# Remove any fields in the config you don't want to change
+# Change the values of any fields you do want to change
+
+
+# This describes where assets such as manifests are stored
+asset_store:
+  # This is when assets are stored in a synapse project
+  synapse:
+    # Synapse ID of the file view listing all project data assets.
+    master_fileview_id: "syn23643253"
+    # Path to the synapse config file, either absolute or relative to this file
+    config: ".synapseConfig"
+    # Base name that manifest files will be saved as
+    manifest_basename: "synapse_storage_manifest"
+
+# This describes information about manifests as it relates to generation and validation
+manifest:
+  # Location where manifests will saved to
+  manifest_folder: "manifests"
+  # Title or title prefix given to generated manifest(s)
+  title: "example"
+  # Data types of manifests to be generated or data type (singular) to validate manifest against
+  data_type:
+    - "Biospecimen"
+    - "Patient"
+
+# Describes the location of your schema
+model:
+  # Location of your schema jsonld, it must be a path relative to this file or absolute
+  location: "tests/data/example.model.jsonld"
+
+# This section is for using google sheets with Schematic
+google_sheets:
+  # The Synapse id of the Google service account credentials.
+  service_acct_creds_synapse_id: "syn25171627"
+  # Path to the synapse config file, either absolute or relative to this file
+  service_acct_creds: "schematic_service_account_creds.json"
+  # When doing google sheet validation (regex match) with the validation rules.
+  #   true is alerting the user and not allowing entry of bad values.
+  #   false is warning but allowing the entry on to the sheet.
+  strict_validation: true
+```
+
+If you want to change any of these copy ``config_example.yml`` to ``config.yml``, change any fields you want to, and remove any fields you don't.
+
+For example if you wanted to change the folder where manifests are downloaded your config should look like:
+
+```text
 
-*Note*: Paths can be specified relative to the `config.yml` file or as absolute paths.
+manifest:
+  manifest_folder: "my_manifest_folder_path"
+```
+
+_Note_: `config.yml` is ignored by git.
+
+_Note_: Paths can be specified relative to the `config.yml` file or as absolute paths.
 
 6. Login to Synapse by using the command line
 On the CLI in your virtual environment, run the following command: 
 ```
 synapse login -u <synapse username> -p <synapse password> --rememberMe
 ```
 Please make sure that you run the command before running `schematic init` below
@@ -315,15 +339,15 @@
 1. [Getting started with Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)
 2. [Installing Sphinx](https://haha.readthedocs.io/en/latest/intro/getting-started-with-sphinx.html)
 
 ## Update toml file and lock file
 If you install external libraries by using `poetry add <name of library>`, please make sure that you include `pyproject.toml` and `poetry.lock` file in your commit.
 
 ## Reporting bugs or feature requests
-You can use the [`Issues`](https://github.com/Sage-Bionetworks/schematic/issues) tab to **create bug and feature requests**. Providing enough details to the developers to verify and troubleshoot your issue is paramount:
+You can **create bug and feature requests** through [Sage Bionetwork's FAIR Data service desk](https://sagebionetworks.jira.com/servicedesk/customer/portal/5/group/8). Providing enough details to the developers to verify and troubleshoot your issue is paramount:
 - **Provide a clear and descriptive title as well as a concise summary** of the issue to identify the problem.
 - **Describe the exact steps which reproduce the problem** in as many details as possible.
 - **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.
 - **Explain which behavior you expected to see** instead and why.
 - **Provide screenshots of the expected or actual behaviour** where applicable.
 
 # Command Line Usage
```

