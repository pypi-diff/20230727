# Comparing `tmp/dataclass_binder-0.3.1.tar.gz` & `tmp/dataclass_binder-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_binder-0.3.1.tar", max compression
+gzip compressed data, was "dataclass_binder-0.3.2.tar", max compression
```

## Comparing `dataclass_binder-0.3.1.tar` & `dataclass_binder-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-07-17 14:22:04.480950 dataclass_binder-0.3.1/LICENSE
--rw-r--r--   0        0        0    17748 2023-07-17 14:22:04.480950 dataclass_binder-0.3.1/README.md
--rw-r--r--   0        0        0     2550 2023-07-17 14:22:31.493489 dataclass_binder-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      172 2023-07-17 14:22:04.480950 dataclass_binder-0.3.1/src/dataclass_binder/__init__.py
--rw-r--r--   0        0        0    33930 2023-07-17 14:22:04.480950 dataclass_binder-0.3.1/src/dataclass_binder/_impl.py
--rw-r--r--   0        0        0        0 2023-07-17 14:22:04.480950 dataclass_binder-0.3.1/src/dataclass_binder/py.typed
--rw-r--r--   0        0        0    19137 1970-01-01 00:00:00.000000 dataclass_binder-0.3.1/setup.py
--rw-r--r--   0        0        0    18664 1970-01-01 00:00:00.000000 dataclass_binder-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-27 01:34:05.108884 dataclass_binder-0.3.2/LICENSE
+-rw-r--r--   0        0        0    18141 2023-07-27 01:34:05.108884 dataclass_binder-0.3.2/README.md
+-rw-r--r--   0        0        0     2550 2023-07-27 01:34:28.332758 dataclass_binder-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-07-27 01:34:05.108884 dataclass_binder-0.3.2/src/dataclass_binder/__init__.py
+-rw-r--r--   0        0        0    35105 2023-07-27 01:34:05.108884 dataclass_binder-0.3.2/src/dataclass_binder/_impl.py
+-rw-r--r--   0        0        0        0 2023-07-27 01:34:05.108884 dataclass_binder-0.3.2/src/dataclass_binder/py.typed
+-rw-r--r--   0        0        0    19536 1970-01-01 00:00:00.000000 dataclass_binder-0.3.2/setup.py
+-rw-r--r--   0        0        0    19057 1970-01-01 00:00:00.000000 dataclass_binder-0.3.2/PKG-INFO
```

### Comparing `dataclass_binder-0.3.1/LICENSE` & `dataclass_binder-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_binder-0.3.1/README.md` & `dataclass_binder-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -527,7 +527,13 @@
 - Fix formatting of `init=False` field in nested dataclasses ([#22](https://github.com/ProtixIT/dataclass-binder/pull/22))
 - Fix annotation evaluation on inherited dataclasses ([#21](https://github.com/ProtixIT/dataclass-binder/pull/21))
 
 ### 0.3.1 - 2023-07-17:
 
 - Generate template in depth-first order ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))
 - Fix binder creation and formatting for recursive dataclasses ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))
+
+### 0.3.2 - 2023-07-27:
+
+- Document fields with a `default_factory` as optional in template ([#35](https://github.com/ProtixIT/dataclass-binder/pull/35))
+- Omit values that are formatted equally to the default ([#36](https://github.com/ProtixIT/dataclass-binder/pull/36))
+- Require optional fields to have `None` as their default ([#37](https://github.com/ProtixIT/dataclass-binder/pull/37))
```

### Comparing `dataclass_binder-0.3.1/pyproject.toml` & `dataclass_binder-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-binder"
-version = "0.3.1"
+version = "0.3.2"
 description = "Library to bind TOML data to Python dataclasses in a type-safe way."
 authors = [
     "Maarten ter Huurne <maarten.terhuurne@protix.eu>",
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ProtixIT/dataclass-binder"
```

### Comparing `dataclass_binder-0.3.1/src/dataclass_binder/_impl.py` & `dataclass_binder-0.3.2/src/dataclass_binder/_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Iterator,
     Mapping,
     MutableMapping,
     MutableSequence,
     Sequence,
     Set,
 )
-from dataclasses import MISSING, asdict, dataclass, fields, is_dataclass, replace
+from dataclasses import MISSING, Field, asdict, dataclass, fields, is_dataclass, replace
 from datetime import date, datetime, time, timedelta
 from functools import reduce
 from importlib import import_module
 from inspect import cleandoc, get_annotations, getmodule, getsource, isabstract
 from pathlib import Path
 from textwrap import dedent
 from types import MappingProxyType, ModuleType, NoneType, UnionType
@@ -161,15 +161,15 @@
         raise KeyError(full_name) from None
     if name in field_names:
         return name, suffix
     else:
         raise KeyError(full_name)
 
 
-def _get_fields(cls: type) -> Iterator[tuple[str, type]]:
+def _get_fields(cls: type) -> Iterator[tuple[Field, type]]:
     """
     Iterates through all the fields in a dataclass.
 
     This includes fields inherited from superclasses.
     """
 
     fields_by_name = {field.name: field for field in fields(cls)}
@@ -184,15 +184,26 @@
             if not field.init:
                 continue
             if isinstance(annotation, str):
                 try:
                     annotation = eval(annotation, cls_globals, cls_locals)  # noqa: PGH001
                 except NameError as ex:
                     raise TypeError(f"Failed to parse annotation of field '{cls.__name__}.{name}': {ex}") from None
-            yield name, annotation
+            yield field, annotation
+
+
+def _check_field(field: Field, field_type: type, context: str) -> None:
+    """
+    Perform some checks on the validity of a field definition.
+
+    This does not do a full type check: there are better tools for that.
+    Instead, it checks specific limitations that our Binder imposes on dataclasses.
+    """
+    if get_origin(field_type) is UnionType and NoneType in get_args(field_type) and field.default is not None:
+        raise TypeError(f"Default for optional field '{context}' is not None")
 
 
 _TIMEDELTA_SUFFIXES = {"days", "seconds", "microseconds", "milliseconds", "minutes", "hours", "weeks"}
 
 T = TypeVar("T")
 
 
@@ -211,18 +222,19 @@
             return cls._cache[dataclass]
         except KeyError:
             # Populate field_types *after* adding new instance to the cache to make sure
             # _collect_type() will find the given dataclass if it's accessed recursively.
             field_types: dict[str, type | Binder[Any]] = {}
             info = cls(dataclass, field_types)
             cls._cache[dataclass] = info
-            field_types.update(
-                (field_name, _collect_type(field_type, f"{dataclass.__name__}.{field_name}"))
-                for field_name, field_type in _get_fields(dataclass)
-            )
+            for field, field_type in _get_fields(dataclass):
+                field_name = field.name
+                context = f"{dataclass.__name__}.{field_name}"
+                field_types[field_name] = _collect_type(field_type, context)
+                _check_field(field, field_type, context)
             return info
 
     @property
     def class_docstring(self) -> str | None:
         class_docstring = self.dataclass.__doc__
         if class_docstring is None:
             # No coverage because of the undocumented feature described below.
@@ -427,15 +439,15 @@
 
         If we are binding to an object, values from that object will be used to populate the template.
         If we are binding to a class, example values will be derived from the field types.
         """
 
         table = Table(self, "", self._instance, None)
         lines = table.format_table(set())
-        for line in lines:  # pragma: no cover
+        for line in lines:
             if line:
                 yield line
                 break
         yield from lines
 
     def _format_toml_table(self, instance: T | None, defer: Callable[[Table[Any]], None]) -> Iterator[str]:
         dataclass = self._dataclass
@@ -448,17 +460,27 @@
 
             key = field.name.replace("_", "-")
             # Most Python names are valid as bare keys, but not if they contain non-ASCII characters.
             key_fmt = "".join(_iter_format_key(key))
             value = None if instance is None else getattr(instance, field.name)
             docstring = docstrings.get(field.name)
 
+            default = field.default
+            if default is MISSING:
+                default_factory = field.default_factory
+                if default_factory is not MISSING:
+                    # We don't call the factory:
+                    # - to avoid listing a dynamic value as a default, like the current date
+                    # - to not trigger any unwanted side effects
+                    default = {list: [], dict: {}}.get(default_factory)  # type: ignore[call-overload]
+            optional = default is not MISSING
+
             field_type = field_types[field.name]
             if isinstance(field_type, Binder):
-                defer(Table(field_type, key_fmt, value, docstring, field.default is not MISSING))
+                defer(Table(field_type, key_fmt, value, docstring, optional))
                 continue
             origin = get_origin(field_type)
             if origin is not None:
                 if issubclass(origin, Mapping):
                     key_type, value_type = get_args(field_type)
                     if isinstance(value_type, Binder):
                         if value is None:
@@ -468,49 +490,49 @@
                                 f"{key_fmt}.{''.join(_iter_format_key(nested_key))}": nested_value
                                 for nested_key, nested_value in value.items()
                             }
                         for nested_key_fmt, nested_value in nested_map.items():
                             defer(Table(value_type, nested_key_fmt, nested_value, docstring))
                         continue
                     if value_type is object:  # Any
-                        defer(Table(None, key_fmt, value, docstring, field.default is not MISSING))
+                        defer(Table(None, key_fmt, value, docstring, optional))
                         continue
                 elif issubclass(origin, Sequence):
                     (value_type,) = get_args(field_type)
                     binder = value_type if isinstance(value_type, Binder) else None
                     if binder is not None or (
                         value_type is object  # Any
                         and (value is None or all(isinstance(item, Mapping) or is_dataclass(item) for item in value))
                     ):
                         nested_key_fmt = f"[{key_fmt}]"
-                        optional = field.default is not MISSING
                         for nested_value in [None] if value is None else value:
                             defer(Table(binder, nested_key_fmt, nested_value, docstring, optional))
                         continue
 
             yield ""
 
             comments = [docstring]
-            default = field.default
-            if value == default:
-                value = None
-            if default is MISSING or default is None:
+            if not optional or default is None:
+                fmt_default = None
                 comments.append("Optional." if default is None else "Mandatory.")
             else:
-                comments.append(f"Default:\n{format_toml_pair(key, default)}")
+                fmt_default = format_toml_pair(key, default)
+                comments.append(f"Default:\n{fmt_default}")
             yield from _format_comments(*comments)
 
             if value is None:
-                if default is MISSING or default is None:
+                if not optional or default is None:
                     comment = "# " if default is None else ""
                     key_fmt = "".join(_iter_format_key(key))
                     value_fmt = _format_value_for_type(field_type)
                     yield f"{comment}{key_fmt} = {value_fmt}"
             else:
-                yield f"{format_toml_pair(key, value)}"
+                fmt_value = format_toml_pair(key, value)
+                if fmt_value != fmt_default:
+                    yield fmt_value
 
     if TYPE_CHECKING:
         # These definitions exist to support the deprecated `Binder[DC]` syntax in mypy.
 
         @classmethod
         def bind(cls, data: Mapping[str, Any]) -> T:
             ...
@@ -549,28 +571,32 @@
         binder = self.binder
         return None if binder is None else binder._class_info.class_docstring
 
     def prefix_context(self, context: str) -> Table[T]:
         return replace(self, key_fmt=f"{context}.{self.key_fmt}" if context else self.key_fmt)
 
     def format_table(self, inside: Set[type]) -> Iterator[str]:
+        """
+        The `inside` parameter keeps track of which dataclasses we are currently outputting,
+        to prevent infinite recursion.
+        """
+
         child_tables: list[Table[Any]] = []
         context = self.key_fmt
         value = self.value
 
         if (binder := self.binder) is None:
             match value:
                 case Mapping() as mapping:
                     content = [format_toml_pair(k, v) for k, v in mapping.items()]
                 case dc if is_dataclass(dc):
                     content = [format_toml_pair(k, v) for k, v in asdict(dc).items()]  # type: ignore[arg-type]
                 case _:
                     content = []
         elif value is None and binder._dataclass in inside:
-            # Prevent infinite recursion.
             content = None
         else:
             inside |= {binder._dataclass}
             content = list(binder._format_toml_table(value, child_tables.append))
             if not content:
                 content = None
```

### Comparing `dataclass_binder-0.3.1/setup.py` & `dataclass_binder-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'dataclass-binder',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Library to bind TOML data to Python dataclasses in a type-safe way.',
-    'long_description': '# Dataclass Binder\n\nLibrary to bind TOML data to Python dataclasses in a type-safe way.\n\n\n## Features\n\nCurrently it has the following properties that might set it apart from other data binding libraries:\n\n- requires Python 3.10+\n- relies only on dataclasses from the Python standard library\n- detailed error messages which mention location, expected data and actual data\n- strict parsing which considers unknown keys to be errors\n- support for durations (`timedelta`)\n- support for immutable (frozen) dataclasses\n- can bind data from files, I/O streams or pre-parsed dictionaries\n- can generate configuration templates from dataclass definitions\n\nThis library was originally designed for parsing configuration files.\nAs TOML\'s data model is very similar to JSON\'s, adding support for JSON in the future would be an option and would make the library useful for binding HTTP API requests.\n\n\n## Maturity\n\nThis library is fully type-checked, has unit tests which provide 100% branch coverage and is used in production, so it should be reliable.\n\nThe API might still change in incompatible ways until the 1.0 release.\nIn particular the following aspects are subject to change:\n\n- use of key suffixes for `timedelta`: this mechanism doesn\'t work for arrays\n- the handling of separators in keys: currently `-` in TOML is mapped to `_` in Python and `_` is forbidden in TOML; most applications seem to accept both `-` and `_` in TOML instead\n\n\n## Why Dataclasses?\n\nA typical TOML, JSON or YAML parser returns the parse results as a nested dictionary.\nYou might wonder why you would want to use a data binding library rather than just getting the values directly from that dictionary.\n\nLet\'s take the following example code for a service that connects to a database using a connection URL configured in a TOML file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\n\n\ndef read_config() -> dict:\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n    return config\n\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    print("connect to database:", url)\n\nconfig = read_config()\n...\nhandle_request(config)\n```\n\nIf the configuration is missing a `database-url` key or its value is not a string, this service would start up without complaints and then fail when the first requests comes in.\nIt would be better to instead check the configuration on startup, so let\'s add code for that:\n\n```py\ndef read_config():\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n\n    url = config["database-url"]\n    if not isinstance(url, str):\n        raise TypeError(\n            f"Value for \'database-url\' has type \'{type(url).__name__}\', expected \'str\'"\n        )\n\n    return config\n```\n\nImagine you have 20 different configurable options: you\'d need this code 20 times.\n\nNow let\'s assume that you use a type checker like `mypy`.\nInside `read_config()`, the type checker will know that `url` is a `str`, but if you fetch the same value elsewhere in the code, that information is lost:\n\n```py\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    reveal_type(url)\n    print("connect to database:", url)\n```\n\nWhen you run `mypy` on this code, it will output \'Revealed type is "Any"\'.\nFalling back to `Any` means type checking will not be able to find type mismatches and autocomplete in an IDE will not work well either.\n\nDeclaring the desired type in a dataclass solves both these issues:\n- the type can be verified at runtime before instantiating the dataclass\n- tooling knows the type when you read the value from the dataclass\n\nHaving the dataclass as a central and formal place for defining the configuration format is also an advantage.\nFor example, it enables automatic generation of a documented configuration file template.\n\n\n## Usage\n\nThe `dataclass_binder` module contains the `Binder` class which makes it easy to bind TOML data, such as a configuration file, to Python [dataclasses](https://docs.python.org/3/library/dataclasses.html).\n\nThe binding is a two-step process:\n- instantiate the `Binder` class by passing your top-level dataclass as an argument\n- call the `parse_toml()` method, providing the path of the configuration file as its argument\n\nPut together, the code looks like this:\n\n```py\nimport logging\nimport sys\nfrom pathlib import Path\n\nfrom dataclass_binder import Binder\n\n\nlogger = logging.getLogger(__name__)\n\nif __name__ == "__main__":\n    config_file = Path("config.toml")\n    try:\n        config = Binder(Config).parse_toml(config_file)\n    except Exception as ex:\n        logger.critical("Error reading configuration file \'%s\': %s", config_file, ex)\n        sys.exit(1)\n```\n\n### Binding a Pre-parsed Dictionary\n\nIf you don\'t want to bind the contents of a full file, there is also the option to bind a pre-parsed dictionary instead.\nFor this, you can use the `bind()` method on the `Binder` object.\n\nFor example, the following service is configured by one table within a larger TOML configuration file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\nfrom dataclass_binder import Binder\n\n\nwith open("config.toml", "rb") as f:\n    config = tomllib.load(f)\nservice_config = Binder(ServiceConfig).bind(config["service"])\n```\n\nTo keep these examples short, from now on `import` statements will only be included the first time a particular imported name is used.\n\n### Basic Types\n\nDataclass fields correspond to TOML keys. In the dataclass, underscores are used as word separators, while dashes are used in the TOML file. Let\'s configure a service that listens on a TCP port for requests and stores its data in a database, using the following TOML fragment:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\nport = 8080\n```\n\nThis configuration can be bound to the following dataclass:\n\n```py\nfrom dataclasses import dataclass\n\n@dataclass\nclass Config:\n    database_url: str\n    port: int\n    verbose: bool\n```\n\nThe `float` type can be used to bind floating point numbers.\nSupport for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.\n\n### Defaults\n\nFields can be made optional by assigning a default value. Using `None` as a default value is allowed too:\n\n```py\n@dataclass\nclass Config:\n    verbose: bool = False\n    webhook_url: str | None = None\n```\n\nIf you want to mix fields with and without defaults in any order, mark the fields as keyword-only:\n\n```py\n@dataclass(kw_only=True)\nclass Config:\n    database_url: str\n    verbose: bool = False\n    port: int\n```\n\n### Dates and Times\n\nTOML handles dates and timestamps as first-class values.\nDate, time and date+time TOML values are bound to `datetime.date`, `datetime.time` and `datetime.datetime` Python objects respectively.\n\nThere is also support for time intervals using `datetime.timedelta`:\n\n```py\nfrom datetime import timedelta\n\n@dataclass\nclass Config:\n    retry_after: timedelta\n    delete_after: timedelta\n```\n\nIntervals shorter than a day can be specified using a TOML time value.\nLonger intervals are supported by adding an `-hours`, `-days`, or `-weeks` suffix.\nOther supported suffixes are `-minutes`, `-seconds`, `-milliseconds` and `-microseconds`, but these are there for completeness sake and less likely to be useful.\nHere is an example TOML fragment corresponding to the dataclass above:\n\n```toml\nretry-after = 00:02:30\ndelete-after-days = 30\n```\n\n### Collections\n\nLists and dictionaries can be used to bind TOML arrays and tables.\nIf you want to make a `list` or `dict` optional, you need to provide a default value via the `default_factory` mechanism as usual, see the [dataclasses documentation](https://docs.python.org/3/library/dataclasses.html#mutable-default-values) for details.\n\n```py\nfrom dataclasses import dataclass, field\n\n@dataclass\nclass Config:\n    tags: list[str] = field(default_factory=list)\n    limits: dict[str, int]\n```\n\nThe dataclass above can be used to bind the following TOML fragment:\n\n```toml\ntags = ["production", "development"]\nlimits = {ram-gb = 1, disk-gb = 100}\n```\n\nAn alternative to `default_factory` is to use a homogeneous (single element type) tuple:\n\n```py\n@dataclass\nclass Config:\n    tags: tuple[str, ...] = ()\n    limits: dict[str, int]\n```\n\nHeterogeneous tuples are supported too: for example `tuple[str, bool]` binds a TOML array that must always have a string as its first element and a Boolean as its second and last element.\nIt is generally clearer though to define a separate dataclass when you need more than one value to configure something:\n\n```py\n@dataclass\nclass Webhook:\n    url: str\n    token: str\n\n@dataclass\nclass Config:\n    webhooks: tuple[Webhook, ...] = ()\n```\n\nThe extra keys (`url` and `token` in this example) provide the clarity:\n\n```toml\nwebhooks = [\n    {url = "https://host1/notify", token = "12345"},\n    {url = "https://host2/hook", token = "frperg"}\n]\n```\n\nTOML\'s array-of-tables syntax can make this configuration a bit easier on the eyes:\n\n```toml\n[[webhooks]]\nurl = "https://host1/notify"\ntoken = "12345"\n\n[[webhooks]]\nurl = "https://host2/hook"\ntoken = "frperg"\n```\n\nAlways define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` constructor will not be able to find it.\n\n### Untyped Data\n\nSometimes the full structure of the data you want to bind is either too complex or too much in flux to be worth fully annotating.\nIn such a situation, you can use `typing.Any` as the annotation to simply capture the output of Python\'s TOML parser without type-checking it.\n\nIn the following example, a service uses the Python standard library logging implementation, configured using the [configuration dictionary schema](https://docs.python.org/3/library/logging.config.html#logging-config-dictschema):\n\n```py\nimport logging.config\nfrom dataclasses import dataclass\nfrom typing import Any\n\nfrom dataclass_binder import Binder\n\n\n@dataclass\nclass Config:\n    database_url: str\n    logging: Any\n\n\ndef run(url: str) -> None:\n    logging.info("Service starting")\n\n\nif __name__ == "__main__":\n    config = Binder[Config].parse_toml("service.toml")\n    logging.config.dictConfig(config.logging)\n    run(config.database_url)\n```\n\nThe `service.toml` configuration file for this service could look like this:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\n\n[logging]\nversion = 1\n\n[logging.root]\nlevel = \'INFO\'\nhandlers = [\'file\']\n\n[logging.handlers.file]\nclass = \'logging.handlers.RotatingFileHandler\'\nfilename = \'service.log\'\nformatter = \'simple\'\n\n[logging.formatters.simple]\nformat = \'%(asctime)s %(name)s %(levelname)s %(message)s\'\n```\n\n### Plugins\n\nTo select plugins to activate, you can bind Python classes or modules using `type[BaseClass]` and `types.ModuleType` annotations respectively:\n\n```py\nfrom dataclasses import dataclass, field\nfrom types import ModuleType\n\nfrom supertool.plugins import PostProcessor\n\n\n@dataclass\nclass PluginConfig:\n    postprocessors = tuple[type[PostProcessor], ...] = ()\n    modules: dict[str, ModuleType] = field(default_factory=dict)\n```\n\nIn the TOML, you specify Python classes or modules using their fully qualified names:\n\n```toml\npostprocessors = ["supertool_addons.reporters.JSONReport"]\nmodules = {lint = "supertool_addons.linter"}\n```\n\nThere is no mechanism yet to add configuration to be used by the plugins.\n\n### Immutable\n\nIf you prefer immutable configuration objects, you can achieve that using the `frozen` argument of the `dataclass` decorator and using abstract collection types in the annotations. For example, the following dataclass will be instantiated with a `tuple` object for `tags` and an immutable dictionary view for `limits`:\n\n```py\nfrom collections.abc import Mapping, Sequence\n\n\n@dataclass(frozen=True)\nclass Config:\n    tags: Sequence[str] = ()\n    limits: Mapping[str, int]\n```\n\n### Layered Binding\n\n`Binder` can be instantiated from a dataclass object rather than the dataclass itself.\nThe dataclass object will provide new default values when binding data to it.\nThis can be used to implement a layered configuration parsing mechanism, where there is a default configuration that can be customized using a system-wide configuration file and/or a per-user configuration file:\n\n```py\nconfig = Config()\nif system_config_path.exists():\n    config = Binder(config).parse_toml(system_config_path)\nif user_config_path.exists():\n    config = Binder(config).parse_toml(user_config_path)\n```\n\nLater layers can override individual fields in nested dataclasses, allowing fine-grained configuration merging, but collections are replaced whole instead of merged.\n\n### Generating a Configuration Template\n\nTo provide users with a starting point for configuring your application/service, you can automatically generate a configuration template from the information in the dataclass.\n\nFor example, when the following dataclass defines your configuration:\n\n```py\n@dataclass\nclass Config:\n    database_url: str\n    """The URL of the database to connect to."""\n\n    port: int = 12345\n    """TCP port on which to accept connections."""\n```\n\nYou can generate a template configuration file using:\n\n```py\nfrom dataclass_binder import Binder\n\n\nfor line in Binder(Config).format_toml_template():\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'???\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\n```\n\nIt is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_toml_template()`:\n\n```py\nTEMPLATE = Config(\n    database_url="postgresql://<username>:<password>@<hostname>/<database name>",\n    port=8080,\n)\n\nfor line in Binder(TEMPLATE).format_toml_template():\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'postgresql://<username>:<password>@<hostname>/<database name>\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\nport = 8080\n```\n\n### Troubleshooting\n\nFinally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.\nIf that fails, the problem is in the dataclass definitions.\nIf that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.\n\n\n## Development Environment\n\n[Poetry](https://python-poetry.org/) is used to set up a virtual environment with all the dependencies and development tools that you need:\n\n    $ cd dataclass-binder\n    $ poetry install\n\nYou can activate a shell which contains the development tools in its search path:\n\n    $ poetry shell\n\nWe recommend setting up pre-commit hooks for Git in the `dataclass-binder` work area.\nThese hooks automatically run a few simple checks and cleanups when you create a new commit.\nAfter you first set up your virtual environment with Poetry, run this command to install the pre-commit hooks:\n\n    $ pre-commit install\n\n\n## Release Procedure\n\n- Verify that CI passes on the branch that you want to release (typically `main`)\n- Create a release on the GitHub web interface; name the tag `v<major>.<minor>.<patchlevel>`\n- After publishing the release on GitHub, the package will be built and published on PyPI automatically via Actions\n\n\n## Deprecations\n\n### Binder Specialization\n\nPrior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.\n\n### Template Formatting\n\nIn version 0.3.0, the function `format_template()` has been replaced by the method `Binder.format_toml_template()`. The old function is still available for now.\n\n## Changelog\n\n### 0.1.0 - 2023-02-21:\n\n- First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible\n\n### 0.1.1 - 2023-02-22:\n\n- Relax `Binder.bind()` argument type to `Mapping` ([#3](https://github.com/ProtixIT/dataclass-binder/issues/3))\n\n### 0.1.2 - 2023-03-03:\n\n- Fix `get()` and `[]` on object bound to read-only mapping ([#6](https://github.com/ProtixIT/dataclass-binder/issues/6))\n\n### 0.1.3 - 2023-03-05:\n\n- Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))\n\n### 0.2.0 - 2023-06-26:\n\n- Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))\n- Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))\n- Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))\n\n### 0.3.0 - 2023-07-13:\n\n- Replace `format_template()` function by `Binder.format_toml_template()` method ([#23](https://github.com/ProtixIT/dataclass-binder/pull/23))\n- Format nested dataclasses as TOML tables ([#25](https://github.com/ProtixIT/dataclass-binder/pull/25))\n- Format untyped mappings and sequences as TOML tables ([#27](https://github.com/ProtixIT/dataclass-binder/pull/27))\n- Fix formatting of `init=False` field in nested dataclasses ([#22](https://github.com/ProtixIT/dataclass-binder/pull/22))\n- Fix annotation evaluation on inherited dataclasses ([#21](https://github.com/ProtixIT/dataclass-binder/pull/21))\n\n### 0.3.1 - 2023-07-17:\n\n- Generate template in depth-first order ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))\n- Fix binder creation and formatting for recursive dataclasses ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))\n',
+    'long_description': '# Dataclass Binder\n\nLibrary to bind TOML data to Python dataclasses in a type-safe way.\n\n\n## Features\n\nCurrently it has the following properties that might set it apart from other data binding libraries:\n\n- requires Python 3.10+\n- relies only on dataclasses from the Python standard library\n- detailed error messages which mention location, expected data and actual data\n- strict parsing which considers unknown keys to be errors\n- support for durations (`timedelta`)\n- support for immutable (frozen) dataclasses\n- can bind data from files, I/O streams or pre-parsed dictionaries\n- can generate configuration templates from dataclass definitions\n\nThis library was originally designed for parsing configuration files.\nAs TOML\'s data model is very similar to JSON\'s, adding support for JSON in the future would be an option and would make the library useful for binding HTTP API requests.\n\n\n## Maturity\n\nThis library is fully type-checked, has unit tests which provide 100% branch coverage and is used in production, so it should be reliable.\n\nThe API might still change in incompatible ways until the 1.0 release.\nIn particular the following aspects are subject to change:\n\n- use of key suffixes for `timedelta`: this mechanism doesn\'t work for arrays\n- the handling of separators in keys: currently `-` in TOML is mapped to `_` in Python and `_` is forbidden in TOML; most applications seem to accept both `-` and `_` in TOML instead\n\n\n## Why Dataclasses?\n\nA typical TOML, JSON or YAML parser returns the parse results as a nested dictionary.\nYou might wonder why you would want to use a data binding library rather than just getting the values directly from that dictionary.\n\nLet\'s take the following example code for a service that connects to a database using a connection URL configured in a TOML file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\n\n\ndef read_config() -> dict:\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n    return config\n\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    print("connect to database:", url)\n\nconfig = read_config()\n...\nhandle_request(config)\n```\n\nIf the configuration is missing a `database-url` key or its value is not a string, this service would start up without complaints and then fail when the first requests comes in.\nIt would be better to instead check the configuration on startup, so let\'s add code for that:\n\n```py\ndef read_config():\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n\n    url = config["database-url"]\n    if not isinstance(url, str):\n        raise TypeError(\n            f"Value for \'database-url\' has type \'{type(url).__name__}\', expected \'str\'"\n        )\n\n    return config\n```\n\nImagine you have 20 different configurable options: you\'d need this code 20 times.\n\nNow let\'s assume that you use a type checker like `mypy`.\nInside `read_config()`, the type checker will know that `url` is a `str`, but if you fetch the same value elsewhere in the code, that information is lost:\n\n```py\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    reveal_type(url)\n    print("connect to database:", url)\n```\n\nWhen you run `mypy` on this code, it will output \'Revealed type is "Any"\'.\nFalling back to `Any` means type checking will not be able to find type mismatches and autocomplete in an IDE will not work well either.\n\nDeclaring the desired type in a dataclass solves both these issues:\n- the type can be verified at runtime before instantiating the dataclass\n- tooling knows the type when you read the value from the dataclass\n\nHaving the dataclass as a central and formal place for defining the configuration format is also an advantage.\nFor example, it enables automatic generation of a documented configuration file template.\n\n\n## Usage\n\nThe `dataclass_binder` module contains the `Binder` class which makes it easy to bind TOML data, such as a configuration file, to Python [dataclasses](https://docs.python.org/3/library/dataclasses.html).\n\nThe binding is a two-step process:\n- instantiate the `Binder` class by passing your top-level dataclass as an argument\n- call the `parse_toml()` method, providing the path of the configuration file as its argument\n\nPut together, the code looks like this:\n\n```py\nimport logging\nimport sys\nfrom pathlib import Path\n\nfrom dataclass_binder import Binder\n\n\nlogger = logging.getLogger(__name__)\n\nif __name__ == "__main__":\n    config_file = Path("config.toml")\n    try:\n        config = Binder(Config).parse_toml(config_file)\n    except Exception as ex:\n        logger.critical("Error reading configuration file \'%s\': %s", config_file, ex)\n        sys.exit(1)\n```\n\n### Binding a Pre-parsed Dictionary\n\nIf you don\'t want to bind the contents of a full file, there is also the option to bind a pre-parsed dictionary instead.\nFor this, you can use the `bind()` method on the `Binder` object.\n\nFor example, the following service is configured by one table within a larger TOML configuration file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\nfrom dataclass_binder import Binder\n\n\nwith open("config.toml", "rb") as f:\n    config = tomllib.load(f)\nservice_config = Binder(ServiceConfig).bind(config["service"])\n```\n\nTo keep these examples short, from now on `import` statements will only be included the first time a particular imported name is used.\n\n### Basic Types\n\nDataclass fields correspond to TOML keys. In the dataclass, underscores are used as word separators, while dashes are used in the TOML file. Let\'s configure a service that listens on a TCP port for requests and stores its data in a database, using the following TOML fragment:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\nport = 8080\n```\n\nThis configuration can be bound to the following dataclass:\n\n```py\nfrom dataclasses import dataclass\n\n@dataclass\nclass Config:\n    database_url: str\n    port: int\n    verbose: bool\n```\n\nThe `float` type can be used to bind floating point numbers.\nSupport for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.\n\n### Defaults\n\nFields can be made optional by assigning a default value. Using `None` as a default value is allowed too:\n\n```py\n@dataclass\nclass Config:\n    verbose: bool = False\n    webhook_url: str | None = None\n```\n\nIf you want to mix fields with and without defaults in any order, mark the fields as keyword-only:\n\n```py\n@dataclass(kw_only=True)\nclass Config:\n    database_url: str\n    verbose: bool = False\n    port: int\n```\n\n### Dates and Times\n\nTOML handles dates and timestamps as first-class values.\nDate, time and date+time TOML values are bound to `datetime.date`, `datetime.time` and `datetime.datetime` Python objects respectively.\n\nThere is also support for time intervals using `datetime.timedelta`:\n\n```py\nfrom datetime import timedelta\n\n@dataclass\nclass Config:\n    retry_after: timedelta\n    delete_after: timedelta\n```\n\nIntervals shorter than a day can be specified using a TOML time value.\nLonger intervals are supported by adding an `-hours`, `-days`, or `-weeks` suffix.\nOther supported suffixes are `-minutes`, `-seconds`, `-milliseconds` and `-microseconds`, but these are there for completeness sake and less likely to be useful.\nHere is an example TOML fragment corresponding to the dataclass above:\n\n```toml\nretry-after = 00:02:30\ndelete-after-days = 30\n```\n\n### Collections\n\nLists and dictionaries can be used to bind TOML arrays and tables.\nIf you want to make a `list` or `dict` optional, you need to provide a default value via the `default_factory` mechanism as usual, see the [dataclasses documentation](https://docs.python.org/3/library/dataclasses.html#mutable-default-values) for details.\n\n```py\nfrom dataclasses import dataclass, field\n\n@dataclass\nclass Config:\n    tags: list[str] = field(default_factory=list)\n    limits: dict[str, int]\n```\n\nThe dataclass above can be used to bind the following TOML fragment:\n\n```toml\ntags = ["production", "development"]\nlimits = {ram-gb = 1, disk-gb = 100}\n```\n\nAn alternative to `default_factory` is to use a homogeneous (single element type) tuple:\n\n```py\n@dataclass\nclass Config:\n    tags: tuple[str, ...] = ()\n    limits: dict[str, int]\n```\n\nHeterogeneous tuples are supported too: for example `tuple[str, bool]` binds a TOML array that must always have a string as its first element and a Boolean as its second and last element.\nIt is generally clearer though to define a separate dataclass when you need more than one value to configure something:\n\n```py\n@dataclass\nclass Webhook:\n    url: str\n    token: str\n\n@dataclass\nclass Config:\n    webhooks: tuple[Webhook, ...] = ()\n```\n\nThe extra keys (`url` and `token` in this example) provide the clarity:\n\n```toml\nwebhooks = [\n    {url = "https://host1/notify", token = "12345"},\n    {url = "https://host2/hook", token = "frperg"}\n]\n```\n\nTOML\'s array-of-tables syntax can make this configuration a bit easier on the eyes:\n\n```toml\n[[webhooks]]\nurl = "https://host1/notify"\ntoken = "12345"\n\n[[webhooks]]\nurl = "https://host2/hook"\ntoken = "frperg"\n```\n\nAlways define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` constructor will not be able to find it.\n\n### Untyped Data\n\nSometimes the full structure of the data you want to bind is either too complex or too much in flux to be worth fully annotating.\nIn such a situation, you can use `typing.Any` as the annotation to simply capture the output of Python\'s TOML parser without type-checking it.\n\nIn the following example, a service uses the Python standard library logging implementation, configured using the [configuration dictionary schema](https://docs.python.org/3/library/logging.config.html#logging-config-dictschema):\n\n```py\nimport logging.config\nfrom dataclasses import dataclass\nfrom typing import Any\n\nfrom dataclass_binder import Binder\n\n\n@dataclass\nclass Config:\n    database_url: str\n    logging: Any\n\n\ndef run(url: str) -> None:\n    logging.info("Service starting")\n\n\nif __name__ == "__main__":\n    config = Binder[Config].parse_toml("service.toml")\n    logging.config.dictConfig(config.logging)\n    run(config.database_url)\n```\n\nThe `service.toml` configuration file for this service could look like this:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\n\n[logging]\nversion = 1\n\n[logging.root]\nlevel = \'INFO\'\nhandlers = [\'file\']\n\n[logging.handlers.file]\nclass = \'logging.handlers.RotatingFileHandler\'\nfilename = \'service.log\'\nformatter = \'simple\'\n\n[logging.formatters.simple]\nformat = \'%(asctime)s %(name)s %(levelname)s %(message)s\'\n```\n\n### Plugins\n\nTo select plugins to activate, you can bind Python classes or modules using `type[BaseClass]` and `types.ModuleType` annotations respectively:\n\n```py\nfrom dataclasses import dataclass, field\nfrom types import ModuleType\n\nfrom supertool.plugins import PostProcessor\n\n\n@dataclass\nclass PluginConfig:\n    postprocessors = tuple[type[PostProcessor], ...] = ()\n    modules: dict[str, ModuleType] = field(default_factory=dict)\n```\n\nIn the TOML, you specify Python classes or modules using their fully qualified names:\n\n```toml\npostprocessors = ["supertool_addons.reporters.JSONReport"]\nmodules = {lint = "supertool_addons.linter"}\n```\n\nThere is no mechanism yet to add configuration to be used by the plugins.\n\n### Immutable\n\nIf you prefer immutable configuration objects, you can achieve that using the `frozen` argument of the `dataclass` decorator and using abstract collection types in the annotations. For example, the following dataclass will be instantiated with a `tuple` object for `tags` and an immutable dictionary view for `limits`:\n\n```py\nfrom collections.abc import Mapping, Sequence\n\n\n@dataclass(frozen=True)\nclass Config:\n    tags: Sequence[str] = ()\n    limits: Mapping[str, int]\n```\n\n### Layered Binding\n\n`Binder` can be instantiated from a dataclass object rather than the dataclass itself.\nThe dataclass object will provide new default values when binding data to it.\nThis can be used to implement a layered configuration parsing mechanism, where there is a default configuration that can be customized using a system-wide configuration file and/or a per-user configuration file:\n\n```py\nconfig = Config()\nif system_config_path.exists():\n    config = Binder(config).parse_toml(system_config_path)\nif user_config_path.exists():\n    config = Binder(config).parse_toml(user_config_path)\n```\n\nLater layers can override individual fields in nested dataclasses, allowing fine-grained configuration merging, but collections are replaced whole instead of merged.\n\n### Generating a Configuration Template\n\nTo provide users with a starting point for configuring your application/service, you can automatically generate a configuration template from the information in the dataclass.\n\nFor example, when the following dataclass defines your configuration:\n\n```py\n@dataclass\nclass Config:\n    database_url: str\n    """The URL of the database to connect to."""\n\n    port: int = 12345\n    """TCP port on which to accept connections."""\n```\n\nYou can generate a template configuration file using:\n\n```py\nfrom dataclass_binder import Binder\n\n\nfor line in Binder(Config).format_toml_template():\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'???\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\n```\n\nIt is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_toml_template()`:\n\n```py\nTEMPLATE = Config(\n    database_url="postgresql://<username>:<password>@<hostname>/<database name>",\n    port=8080,\n)\n\nfor line in Binder(TEMPLATE).format_toml_template():\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'postgresql://<username>:<password>@<hostname>/<database name>\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\nport = 8080\n```\n\n### Troubleshooting\n\nFinally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.\nIf that fails, the problem is in the dataclass definitions.\nIf that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.\n\n\n## Development Environment\n\n[Poetry](https://python-poetry.org/) is used to set up a virtual environment with all the dependencies and development tools that you need:\n\n    $ cd dataclass-binder\n    $ poetry install\n\nYou can activate a shell which contains the development tools in its search path:\n\n    $ poetry shell\n\nWe recommend setting up pre-commit hooks for Git in the `dataclass-binder` work area.\nThese hooks automatically run a few simple checks and cleanups when you create a new commit.\nAfter you first set up your virtual environment with Poetry, run this command to install the pre-commit hooks:\n\n    $ pre-commit install\n\n\n## Release Procedure\n\n- Verify that CI passes on the branch that you want to release (typically `main`)\n- Create a release on the GitHub web interface; name the tag `v<major>.<minor>.<patchlevel>`\n- After publishing the release on GitHub, the package will be built and published on PyPI automatically via Actions\n\n\n## Deprecations\n\n### Binder Specialization\n\nPrior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.\n\n### Template Formatting\n\nIn version 0.3.0, the function `format_template()` has been replaced by the method `Binder.format_toml_template()`. The old function is still available for now.\n\n## Changelog\n\n### 0.1.0 - 2023-02-21:\n\n- First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible\n\n### 0.1.1 - 2023-02-22:\n\n- Relax `Binder.bind()` argument type to `Mapping` ([#3](https://github.com/ProtixIT/dataclass-binder/issues/3))\n\n### 0.1.2 - 2023-03-03:\n\n- Fix `get()` and `[]` on object bound to read-only mapping ([#6](https://github.com/ProtixIT/dataclass-binder/issues/6))\n\n### 0.1.3 - 2023-03-05:\n\n- Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))\n\n### 0.2.0 - 2023-06-26:\n\n- Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))\n- Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))\n- Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))\n\n### 0.3.0 - 2023-07-13:\n\n- Replace `format_template()` function by `Binder.format_toml_template()` method ([#23](https://github.com/ProtixIT/dataclass-binder/pull/23))\n- Format nested dataclasses as TOML tables ([#25](https://github.com/ProtixIT/dataclass-binder/pull/25))\n- Format untyped mappings and sequences as TOML tables ([#27](https://github.com/ProtixIT/dataclass-binder/pull/27))\n- Fix formatting of `init=False` field in nested dataclasses ([#22](https://github.com/ProtixIT/dataclass-binder/pull/22))\n- Fix annotation evaluation on inherited dataclasses ([#21](https://github.com/ProtixIT/dataclass-binder/pull/21))\n\n### 0.3.1 - 2023-07-17:\n\n- Generate template in depth-first order ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))\n- Fix binder creation and formatting for recursive dataclasses ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))\n\n### 0.3.2 - 2023-07-27:\n\n- Document fields with a `default_factory` as optional in template ([#35](https://github.com/ProtixIT/dataclass-binder/pull/35))\n- Omit values that are formatted equally to the default ([#36](https://github.com/ProtixIT/dataclass-binder/pull/36))\n- Require optional fields to have `None` as their default ([#37](https://github.com/ProtixIT/dataclass-binder/pull/37))\n',
     'author': 'Maarten ter Huurne',
     'author_email': 'maarten.terhuurne@protix.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ProtixIT/dataclass-binder',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `dataclass_binder-0.3.1/PKG-INFO` & `dataclass_binder-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-binder
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to bind TOML data to Python dataclasses in a type-safe way.
 Home-page: https://github.com/ProtixIT/dataclass-binder
 License: MIT
 Keywords: dataclass,toml,bind,binding
 Author: Maarten ter Huurne
 Author-email: maarten.terhuurne@protix.eu
 Requires-Python: >=3.10,<4.0
@@ -549,7 +549,13 @@
 - Fix annotation evaluation on inherited dataclasses ([#21](https://github.com/ProtixIT/dataclass-binder/pull/21))
 
 ### 0.3.1 - 2023-07-17:
 
 - Generate template in depth-first order ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))
 - Fix binder creation and formatting for recursive dataclasses ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))
 
+### 0.3.2 - 2023-07-27:
+
+- Document fields with a `default_factory` as optional in template ([#35](https://github.com/ProtixIT/dataclass-binder/pull/35))
+- Omit values that are formatted equally to the default ([#36](https://github.com/ProtixIT/dataclass-binder/pull/36))
+- Require optional fields to have `None` as their default ([#37](https://github.com/ProtixIT/dataclass-binder/pull/37))
+
```

