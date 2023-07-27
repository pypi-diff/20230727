# Comparing `tmp/yaml_config_builder-8.1.1.tar.gz` & `tmp/yaml_config_builder-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_config_builder-8.1.1.tar", max compression
+gzip compressed data, was "yaml_config_builder-8.2.0.tar", max compression
```

## Comparing `yaml_config_builder-8.1.1.tar` & `yaml_config_builder-8.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11412 2023-06-23 09:54:30.687889 yaml_config_builder-8.1.1/LICENSE
--rw-r--r--   0        0        0      950 2023-06-23 09:54:30.687889 yaml_config_builder-8.1.1/README.md
--rw-r--r--   0        0        0     2739 2023-06-23 10:53:19.629307 yaml_config_builder-8.1.1/pyproject.toml
--rw-r--r--   0        0        0      452 2023-06-23 09:54:30.691889 yaml_config_builder-8.1.1/src/config_builder/__init__.py
--rw-r--r--   0        0        0    18716 2023-06-23 09:54:30.691889 yaml_config_builder-8.1.1/src/config_builder/base_config_class.py
--rw-r--r--   0        0        0    13656 2023-06-23 09:54:30.691889 yaml_config_builder-8.1.1/src/config_builder/config_builder.py
--rw-r--r--   0        0        0        0 2023-06-23 11:39:45.057131 yaml_config_builder-8.1.1/src/config_builder/py.typed
--rw-r--r--   0        0        0     3913 2023-06-23 09:54:30.691889 yaml_config_builder-8.1.1/src/config_builder/replacement_map.py
--rw-r--r--   0        0        0     2702 2023-06-23 10:33:05.439045 yaml_config_builder-8.1.1/src/config_builder/utils.py
--rw-r--r--   0        0        0    10568 2023-06-23 09:54:30.691889 yaml_config_builder-8.1.1/src/config_builder/yaml_constructors.py
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 yaml_config_builder-8.1.1/setup.py
--rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 yaml_config_builder-8.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-07-26 18:40:16.254257 yaml_config_builder-8.2.0/LICENSE
+-rw-r--r--   0        0        0      950 2023-07-26 18:40:16.254257 yaml_config_builder-8.2.0/README.md
+-rw-r--r--   0        0        0     2739 2023-07-26 18:40:16.258257 yaml_config_builder-8.2.0/pyproject.toml
+-rw-r--r--   0        0        0      452 2023-07-26 18:40:16.258257 yaml_config_builder-8.2.0/src/config_builder/__init__.py
+-rw-r--r--   0        0        0    18764 2023-07-26 18:40:16.258257 yaml_config_builder-8.2.0/src/config_builder/base_config_class.py
+-rw-r--r--   0        0        0    13693 2023-07-27 08:40:00.192575 yaml_config_builder-8.2.0/src/config_builder/config_builder.py
+-rw-r--r--   0        0        0     1800 2023-07-26 18:40:16.258257 yaml_config_builder-8.2.0/src/config_builder/json_encoding.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:34:38.694087 yaml_config_builder-8.2.0/src/config_builder/py.typed
+-rw-r--r--   0        0        0     3913 2023-07-26 18:40:16.258257 yaml_config_builder-8.2.0/src/config_builder/replacement_map.py
+-rw-r--r--   0        0        0     2702 2023-07-26 18:40:16.258257 yaml_config_builder-8.2.0/src/config_builder/utils.py
+-rw-r--r--   0        0        0    10334 2023-07-27 12:21:07.899871 yaml_config_builder-8.2.0/src/config_builder/yaml_constructors.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 yaml_config_builder-8.2.0/setup.py
+-rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 yaml_config_builder-8.2.0/PKG-INFO
```

### Comparing `yaml_config_builder-8.1.1/LICENSE` & `yaml_config_builder-8.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.1.1/README.md` & `yaml_config_builder-8.2.0/README.md`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.1.1/pyproject.toml` & `yaml_config_builder-8.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "yaml-config-builder"
 description = "Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files"
-version = "8.1.1"
+version = "8.2.0"
 license = "Open Logistics Foundation License 1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `yaml_config_builder-8.1.1/src/config_builder/base_config_class.py` & `yaml_config_builder-8.2.0/src/config_builder/base_config_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 """
 Definition of the BaseConfigClass that should be used as superclass for any configuration
 class that should be built with the ConfigBuilder.
 """
 from __future__ import annotations
 
 import copy
+import json
 import logging
+from collections import OrderedDict
 from typing import Any, Dict, List, Optional, cast
 
 import related
 from attr import define, field, fields_dict
 from related import TypedSequence
 
 from config_builder.replacement_map import (
```

### Comparing `yaml_config_builder-8.1.1/src/config_builder/config_builder.py` & `yaml_config_builder-8.2.0/src/config_builder/config_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """ Main class for building configuration classes """
 
 import argparse
 import logging
 import os
 from collections import OrderedDict
 from pathlib import Path
-from typing import Callable, Dict, Optional, Type, cast
+from typing import Any, Callable, Dict, Optional, Type, cast
 
 import yaml
 from related import from_yaml, to_model
 
 from config_builder import BaseConfigClass
 from config_builder.replacement_map import (
     clear_replacement_map,
@@ -338,24 +338,27 @@
                 and args_dict[os_replacement_key] is not None
             ):
                 set_replacement_map_value(
                     key=os_replacement_key, value=args_dict[os_replacement_key]
                 )
 
     @staticmethod
-    def __recursive_check_dict(yml_dict: OrderedDict) -> None:  # type: ignore
+    def __recursive_check_dict(yml_dict: Dict[Any, Any]) -> None:
         """
         Check the dictionary that has been parsed by a from_yaml(stream=original_yaml),
         whether there have been failures while reading configs
         from file-paths. This indicates either a real wrong configured
         path or that some OS replacements haven't been configured.
 
-        :param yml_dict: OrderedDict parsed from via "from_yaml(stream=original_yaml)"
-        :return: None
+        Args:
+            yml_dict: Dict parsed from via "from_yaml(stream=original_yaml)"
+
+        Returns:
+             None
         """
 
         for key, value in yml_dict.items():
-            if isinstance(value, OrderedDict):
+            if isinstance(value, OrderedDict) or isinstance(value, dict):
                 ConfigBuilder.__recursive_check_dict(yml_dict=value)
             else:
                 if "FileNotFoundError" in key:
                     raise FileNotFoundError(value)
```

### Comparing `yaml_config_builder-8.1.1/src/config_builder/replacement_map.py` & `yaml_config_builder-8.2.0/src/config_builder/replacement_map.py`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.1.1/src/config_builder/utils.py` & `yaml_config_builder-8.2.0/src/config_builder/utils.py`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.1.1/src/config_builder/yaml_constructors.py` & `yaml_config_builder-8.2.0/src/config_builder/yaml_constructors.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 Definition of constructors that can be added to the python yaml package
 """
 
 from __future__ import absolute_import, annotations, division, print_function
 
 import logging
 import os
-from collections import OrderedDict
 from pathlib import Path
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import yaml
 from yaml import FullLoader, Loader, Node, UnsafeLoader
 
 from config_builder.utils import prepare_config_path
 
 logger = logging.getLogger(__name__)
@@ -121,32 +120,32 @@
     - 2.: The path to the yaml file from which the content should be extracted
 
     Args:
         loader: a yaml loader needed to parse the content of the given node into
                 a sequence
         node: The node for which to apply this constructors
     Returns:
-        An OrderedDict containing the content of the given yaml file
+        A dictionary containing the content of the given yaml file
     """
 
     seq = loader.construct_sequence(node)  # type: ignore[arg-type]
 
     if len(seq) < 2:
         raise ValueError(
             "You have two provide two parameters when using !join_object:\n"
             " -1.: The first defines the name of the attribute whose content should be "
             " extracted from the given yaml file\n"
             " -2.: The path to the yaml file from which the content should be extracted\n"
         )
 
     class_type = str(seq[0])
 
-    transformed_data: Union[List[Any], OrderedDict[Any, Any]]
+    transformed_data: Union[List[Any], Dict[Any, Any]]
 
-    transformed_data_list: List[Union[List[Any], OrderedDict[Any, Any]]] = []
+    transformed_data_list: List[Union[List[Any], Dict[Any, Any]]] = []
 
     for index in range(1, len(seq)):
         config_path = str(Path(str(seq[index])))
         data, config_path = __get_config_data(config_path=config_path)
 
         if data is not None and class_type != "":
             logger.debug(
@@ -160,21 +159,19 @@
                 logger.debug(
                     f"Parsed configuration via !join_object "
                     f"with emtpy class-type from '{config_path}'"
                 )
 
                 _transformed_data = data
             else:
-                _transformed_data = OrderedDict(
-                    {
-                        "FileNotFoundError": f"Could not parse content from the "
-                        f"configuration file {config_path} "
-                        f"for class '{class_type}'!"
-                    }
-                )
+                _transformed_data = {
+                    "FileNotFoundError": f"Could not parse content from the "
+                    f"configuration file {config_path} "
+                    f"for class '{class_type}'!"
+                }
 
         transformed_data_list.append(_transformed_data)
 
     if len(transformed_data_list) > 1:
         # In case of multiple filepaths given by !join_object,
         # we assume that the respective attribute is of type list.
         # Therefore, we concatenate all the entries to one joined list.
@@ -183,15 +180,15 @@
             transformed_data.extend(_transformed_data)
     elif len(transformed_data_list) == 1:
         # In case of a single item, take the entry as is.
         transformed_data = transformed_data_list[0]
     else:
         # This is just a fallback. With checking 'len(seq) < 2' above,
         # we normally have at least one entry in the transformed_data_list
-        transformed_data = OrderedDict({})
+        transformed_data = {}
 
     return transformed_data
 
 
 def join_object_from_config_dir(
     loader: Union[Loader, FullLoader, UnsafeLoader], node: Node
 ) -> Any:
@@ -207,15 +204,15 @@
 
     Args:
         loader: a yaml loader needed to parse the content of the given node into
                 a sequence
         node: The node for which to apply this constructors
 
     Returns:
-         An OrderedDict containing the content of the given yaml file
+         An Dict containing the content of the given yaml file
     """
 
     sequences = loader.construct_sequence(node)  # type: ignore[arg-type]
 
     if len(sequences) < 3:
         raise ValueError(
             "For !join_object_from_config_dir at least 3 Arguments have to be provided!\n"
@@ -224,15 +221,15 @@
             " -3. to n: directories where to search for the config_file_name"
         )
 
     class_type = str(sequences[0])
     config_file_name = str(sequences[1])
     config_dirs = sequences[2:]
 
-    transformed_data: Optional[OrderedDict[Any, Any]] = None
+    transformed_data: Optional[Dict[Any, Any]] = None
 
     for _, config_dir in enumerate(config_dirs):
         if transformed_data is not None:
             break
 
         data, config_path = __get_config_data(
             config_path=str(Path(os.path.join(str(config_dir), config_file_name)))
@@ -251,51 +248,49 @@
                     f"Parsed configuration via !join_object_from_config_dir "
                     f"with emtpy class-type from '{config_path}'"
                 )
 
                 transformed_data = data
 
     if transformed_data is None:
-        transformed_data = OrderedDict(
-            {
-                "FileNotFoundError": f"Could not find a valid "
-                f"configuration file for class '{class_type}' "
-                f"while parsing for config_file_name '{config_file_name}' "
-                f"and config_dirs '{config_dirs}'!"
-            }
-        )
+        transformed_data = {
+            "FileNotFoundError": f"Could not find a valid "
+            f"configuration file for class '{class_type}' "
+            f"while parsing for config_file_name '{config_file_name}' "
+            f"and config_dirs '{config_dirs}'!"
+        }
 
     return transformed_data
 
 
 # register the tag handlers
 yaml.add_constructor("!join_string", join_string)
 yaml.add_constructor("!join_string_with_delimiter", join_string_with_delimiter)
 yaml.add_constructor("!join_path", join_path)
 yaml.add_constructor("!join_object", join_object)
 yaml.add_constructor("!join_object_from_config_dir", join_object_from_config_dir)
 
 
-def __parse_from_config_path(config_path: str) -> Optional[OrderedDict[Any, Any]]:
-    parsed_dict: Optional[OrderedDict[Any, Any]] = None
+def __parse_from_config_path(config_path: str) -> Optional[Dict[Any, Any]]:
+    parsed_dict: Optional[Dict[Any, Any]] = None
 
     if os.path.isfile(config_path):
         with open(config_path, encoding="utf8") as config_file:
-            parsed_dict = yaml.load(config_file, Loader) or OrderedDict()
+            parsed_dict = yaml.load(config_file, Loader) or {}
     else:
         logger.debug(
             "The given config-path does not exist! Can not parse any data. "
             f"config_path: {config_path}"
         )
 
     return parsed_dict
 
 
-def __get_config_data(config_path: str) -> Tuple[Optional[OrderedDict[Any, Any]], str]:
-    parsed_dict: Optional[OrderedDict[Any, Any]]
+def __get_config_data(config_path: str) -> Tuple[Optional[Dict[Any, Any]], str]:
+    parsed_dict: Optional[Dict[Any, Any]]
 
     parsed_dict = __parse_from_config_path(config_path=config_path)
 
     if parsed_dict is not None:
         return parsed_dict, config_path
     else:
         logger.debug(
```

### Comparing `yaml_config_builder-8.1.1/setup.py` & `yaml_config_builder-8.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'attrs>=20',
  'future>0.18',
  'python-dateutil>2.8',
  'related-mltoolbox>=1.0.1,<2']
 
 setup_kwargs = {
     'name': 'yaml-config-builder',
-    'version': '8.1.1',
+    'version': '8.2.0',
     'description': 'Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files',
     'long_description': '# Config Builder\n\nThe ConfigBuilder provides an SDK for building configuration classes on the basis of \ngiven content from YAML configuration files. Details about the ConfigBuilder can be\nfound in the [documentation](documentation/index.adoc).\n\n## Install\n\nThe installation and setup of the ConfigBuilder is described in [chapter 11](documentation/12_tutorial.adoc) \nof the documentation.\n\n# Technology stack\n\n- Python \n\n## License\nSee the license file in the top directory.\n\n## Contact information\n\n\nMaintainer: \n- Maximilian Otten <a href="mailto:maximilian.otten@iml.fraunhofer.de?">maximilian.otten@iml.fraunhofer.de</a>\n\nDevelopment Team: \n- Christian Hoppe <a href="mailto:christian.hoppe@iml.fraunhofer.de?">christian.hoppe@iml.fraunhofer.de</a>\n- Oliver Bredtmann <a href="mailto:oliver.bredtmann@dbschenker.com?">oliver.bredtmann@dbschenker.com</a>\n- Thilo Bauer <a href="mailto:thilo.bauer@dbschenker.com?">thilo.bauer@dbschenker.com</a>\n\n\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['config_builder'] package_data = \ {'': ['*']}
 install_requires = \ ['PyYAML>5.4', 'attrs>=20', 'future>0.18', 'python-
 dateutil>2.8', 'related-mltoolbox>=1.0.1,<2'] setup_kwargs = { 'name': 'yaml-
-config-builder', 'version': '8.1.1', 'description': 'Yaml-Config-Builder: SDK
+config-builder', 'version': '8.2.0', 'description': 'Yaml-Config-Builder: SDK
 for building configuration classes on the basis of given content from YAML
 configuration files', 'long_description': '# Config Builder\n\nThe
 ConfigBuilder provides an SDK for building configuration classes on the basis
 of \ngiven content from YAML configuration files. Details about the
 ConfigBuilder can be\nfound in the [documentation](documentation/
 index.adoc).\n\n## Install\n\nThe installation and setup of the ConfigBuilder
 is described in [chapter 11](documentation/12_tutorial.adoc) \nof the
```

### Comparing `yaml_config_builder-8.1.1/PKG-INFO` & `yaml_config_builder-8.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-config-builder
-Version: 8.1.1
+Version: 8.2.0
 Summary: Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder
 License: Open Logistics Foundation License 1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yaml-config-builder Version: 8.1.1 Summary: Yaml-
+Metadata-Version: 2.1 Name: yaml-config-builder Version: 8.2.0 Summary: Yaml-
 Config-Builder: SDK for building configuration classes on the basis of given
 content from YAML configuration files Home-page: https://
 git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder
 License: Open Logistics Foundation License 1.3 Author: Maximilian Otten Author-
 email: maximilian.otten@iml.fraunhofer.de Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: Other/Proprietary License
```

