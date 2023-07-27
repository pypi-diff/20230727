# Comparing `tmp/related_mltoolbox-1.0.2.tar.gz` & `tmp/related_mltoolbox-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "related_mltoolbox-1.0.2.tar", max compression
+gzip compressed data, was "related_mltoolbox-1.1.0.tar", max compression
```

## Comparing `related_mltoolbox-1.0.2.tar` & `related_mltoolbox-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1135 2023-02-03 08:20:37.096469 related_mltoolbox-1.0.2/LICENSE
--rw-r--r--   0        0        0    11702 2023-02-03 08:20:37.096469 related_mltoolbox-1.0.2/README.md
--rw-r--r--   0        0        0     2724 2023-02-03 08:52:55.638843 related_mltoolbox-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1720 2023-02-03 08:22:27.612140 related_mltoolbox-1.0.2/src/related/__init__.py
--rw-r--r--   0        0        0     1263 2023-02-03 08:20:37.096469 related_mltoolbox-1.0.2/src/related/_init_fields.py
--rw-r--r--   0        0        0     7194 2023-02-03 08:20:37.096469 related_mltoolbox-1.0.2/src/related/converters.py
--rw-r--r--   0        0        0     1594 2023-02-03 08:20:37.096469 related_mltoolbox-1.0.2/src/related/decorators.py
--rw-r--r--   0        0        0     2899 2023-02-03 08:20:37.096469 related_mltoolbox-1.0.2/src/related/dispatchers.py
--rw-r--r--   0        0        0    13235 2023-02-03 08:20:37.096469 related_mltoolbox-1.0.2/src/related/fields.py
--rw-r--r--   0        0        0     6684 2023-02-03 08:20:37.096469 related_mltoolbox-1.0.2/src/related/functions.py
--rw-r--r--   0        0        0     4699 2023-02-03 08:20:37.096469 related_mltoolbox-1.0.2/src/related/types.py
--rw-r--r--   0        0        0     1195 2023-02-03 08:20:37.096469 related_mltoolbox-1.0.2/src/related/validators.py
--rw-r--r--   0        0        0    12894 1970-01-01 00:00:00.000000 related_mltoolbox-1.0.2/setup.py
--rw-r--r--   0        0        0    13006 1970-01-01 00:00:00.000000 related_mltoolbox-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-07-26 18:06:10.703910 related_mltoolbox-1.1.0/LICENSE
+-rw-r--r--   0        0        0    11702 2023-07-26 18:06:10.703910 related_mltoolbox-1.1.0/README.md
+-rw-r--r--   0        0        0     2674 2023-07-27 06:53:29.807298 related_mltoolbox-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1691 2023-07-27 06:53:29.807298 related_mltoolbox-1.1.0/src/related/__init__.py
+-rw-r--r--   0        0        0     1264 2023-07-26 18:06:10.703910 related_mltoolbox-1.1.0/src/related/_init_fields.py
+-rw-r--r--   0        0        0     7288 2023-07-26 18:06:10.703910 related_mltoolbox-1.1.0/src/related/converters.py
+-rw-r--r--   0        0        0     1589 2023-07-26 18:06:10.703910 related_mltoolbox-1.1.0/src/related/decorators.py
+-rw-r--r--   0        0        0     2853 2023-07-26 18:06:10.703910 related_mltoolbox-1.1.0/src/related/dispatchers.py
+-rw-r--r--   0        0        0    13375 2023-07-26 18:06:10.703910 related_mltoolbox-1.1.0/src/related/fields.py
+-rw-r--r--   0        0        0     6487 2023-07-26 18:06:10.703910 related_mltoolbox-1.1.0/src/related/functions.py
+-rw-r--r--   0        0        0     4591 2023-07-26 18:06:10.703910 related_mltoolbox-1.1.0/src/related/types.py
+-rw-r--r--   0        0        0     1200 2023-07-26 18:06:10.703910 related_mltoolbox-1.1.0/src/related/validators.py
+-rw-r--r--   0        0        0    12894 1970-01-01 00:00:00.000000 related_mltoolbox-1.1.0/setup.py
+-rw-r--r--   0        0        0    13006 1970-01-01 00:00:00.000000 related_mltoolbox-1.1.0/PKG-INFO
```

### Comparing `related_mltoolbox-1.0.2/LICENSE` & `related_mltoolbox-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `related_mltoolbox-1.0.2/README.md` & `related_mltoolbox-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `related_mltoolbox-1.0.2/pyproject.toml` & `related_mltoolbox-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "related-mltoolbox"
-version = "1.0.2"
+version = "1.1.0"
 license = "MIT license"
 description = "(Fork from related) Related: Straightforward nested object models in Python"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/related-mltoolbox"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/related-mltoolbox"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/related-mltoolbox/-/blob/main/README.md"
 authors = [
@@ -17,18 +17,14 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
 ]
 packages = [
     { include = "related", from="src" },
 ]
 
-[[tool.poetry.source]]
-name = "nexus-cache"
-url = "https://nexus.apps.sele.iml.fraunhofer.de/repository/pypi-group/simple/"
-
 [tool.poetry.dependencies]
 python = "^3.6.2"
 attrs = { version = "*" }
 PyYAML = { version = "*" }
 future = { version = "*" }
 python-dateutil = { version = "*" }
 
@@ -37,14 +33,16 @@
 pytest-cov = { version = "*" }
 pytest-mccabe = { version = "*" }
 pytest-pep8 = { version = "*" }
 pytest-pythonpath = { version = "*" }
 pytest-sugar = { version = "*" }
 coverage = {version = "*" }
 black = { version = "*" }
+# Isort guarantees formatting results for 5.X
+isort = { version = "^5.0" }
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `related_mltoolbox-1.0.2/src/related/__init__.py` & `related_mltoolbox-1.1.0/src/related/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,49 @@
 # -*- coding: utf-8 -*-
 
-from .decorators import (
-    mutable,
-    immutable,
-    serializer,
-)
-
-from .types import (
-    ImmutableDict,
-    TypedSequence,
-    TypedMapping,
-    TypedSet,
-)
-
+from . import dispatchers  # noqa F401
+from .decorators import immutable, mutable, serializer
 from .fields import (
     BooleanField,
     ChildField,
     DateField,
     DateTimeField,
-    TimeField,
+    DecimalField,
     FloatField,
     IntegerField,
     MappingField,
     RegexField,
     SequenceField,
     SetField,
     StringField,
+    TimeField,
     URLField,
     UUIDField,
-    DecimalField,
 )
-
 from .functions import (
     from_json,
     from_yaml,
     is_model,
     to_dict,
     to_json,
     to_model,
     to_yaml,
 )
-
-from . import dispatchers  # noqa F401
+from .types import ImmutableDict, TypedMapping, TypedSequence, TypedSet
 
 __all__ = [
     # decorators.py
     "mutable",
     "immutable",
     "serializer",
-
     # types.py
     "ImmutableDict",
     "TypedSequence",
     "TypedMapping",
     "TypedSet",
-
     # fields.py
     "BooleanField",
     "ChildField",
     "DateField",
     "DateTimeField",
     "TimeField",
     "FloatField",
@@ -67,29 +52,32 @@
     "RegexField",
     "SetField",
     "StringField",
     "SequenceField",
     "URLField",
     "UUIDField",
     "DecimalField",
-
     # functions.py
     "from_json",
     "from_yaml",
     "is_model",
     "to_dict",
     "to_json",
     "to_model",
     "to_yaml",
 ]
 
 
-__version__ = '1.0.2'
+__version__ = "1.1.0"
 __title__ = "related-mltoolbox"
 
 __author__ = """Ian Maurer, Maximilian Otten, Christian Hoppe"""
 
 __uri__ = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/related-mltoolbox"
-__copyright__ = "Copyright (c) Open Logistics Foundation, Copyright (c) 2017 genomoncology.com, "
-__description__ = "(Fork of related) Related: Straightforward nested object models in Python"
+__copyright__ = (
+    "Copyright (c) Open Logistics Foundation, Copyright (c) 2017 genomoncology.com, "
+)
+__description__ = (
+    "(Fork of related) Related: Straightforward nested object models in Python"
+)
 __doc__ = __description__ + " <" + __uri__ + ">"
 __license__ = "MIT"
```

### Comparing `related_mltoolbox-1.0.2/src/related/_init_fields.py` & `related_mltoolbox-1.1.0/src/related/_init_fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from attr import validators, NOTHING
+from attr import NOTHING, validators
+
 from .validators import composite
 
 
 def init_default(required, default, optional_default):
     """
     Returns optional default if field is not required and
     default was not provided.
```

### Comparing `related_mltoolbox-1.0.2/src/related/converters.py` & `related_mltoolbox-1.1.0/src/related/converters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-from collections import OrderedDict
-from uuid import UUID
-from future.moves.urllib.parse import urlparse
-from six import string_types, callable
 from datetime import datetime
+from importlib import import_module
 from inspect import isfunction
+from uuid import UUID
+
 from dateutil import parser
-from importlib import import_module
+from future.moves.urllib.parse import urlparse
+from six import callable, string_types
 
-from .types import TypedSequence, TypedMapping, TypedSet
 from .functions import to_model
+from .types import TypedMapping, TypedSequence, TypedSet
 
-CHILD_ERROR_MSG = "Failed to convert value ({}) to child object class ({}). " \
-                  + "... [Original error message: {}]"
+CHILD_ERROR_MSG = (
+    "Failed to convert value ({}) to child object class ({}). "
+    + "... [Original error message: {}]"
+)
 
 
 def to_child_field(cls):
     """
     Returns an callable instance that will convert a value to a Child object.
 
     :param cls: Valid class type of the Child.
     :return: instance of ChildConverter.
     """
 
     class ChildConverter(object):
-
         def __init__(self, cls):
             self._cls = cls
 
         @property
         def cls(self):
             return resolve_class(self._cls)
 
         def __call__(self, value):
             try:
                 # Issue #33: if value is the class and callable, then invoke
-                if (value == self._cls or isinstance(value, self._cls)) and callable(value):
-                    value = value()
-
+                try:
+                    if (
+                        value == self._cls or isinstance(value, self._cls)
+                    ) and callable(value):
+                        value = value()
+                except TypeError as te:
+                    print("HERE")
                 return to_model(self.cls, value)
             except ValueError as e:
                 error_msg = CHILD_ERROR_MSG.format(value, self.cls, str(e))
                 raise ValueError(error_msg)
 
     return ChildConverter(cls)
 
@@ -48,16 +53,16 @@
 def to_sequence_field(cls):
     """
     Returns a callable instance that will convert a value to a Sequence.
 
     :param cls: Valid class type of the items in the Sequence.
     :return: instance of the SequenceConverter.
     """
-    class SequenceConverter(object):
 
+    class SequenceConverter(object):
         def __init__(self, cls):
             self._cls = cls
 
         @property
         def cls(self):
             return resolve_class(self._cls)
 
@@ -72,16 +77,16 @@
 def to_set_field(cls):
     """
     Returns a callable instance that will convert a value to a Sequence.
 
     :param cls: Valid class type of the items in the Sequence.
     :return: instance of the SequenceConverter.
     """
-    class SetConverter(object):
 
+    class SetConverter(object):
         def __init__(self, cls):
             self._cls = cls
 
         @property
         def cls(self):
             return resolve_class(self._cls)
 
@@ -97,26 +102,26 @@
     """
     Returns a callable instance that will convert a value to a Mapping.
 
     :param cls: Valid class type of the items in the Sequence.
     :param key: Attribute name of the key value in each item of cls instance.
     :return: instance of the MappingConverter.
     """
-    class MappingConverter(object):
 
+    class MappingConverter(object):
         def __init__(self, cls, key):
             self._cls = cls
             self.key = key
 
         @property
         def cls(self):
             return resolve_class(self._cls)
 
         def __call__(self, values):
-            kwargs = OrderedDict()
+            kwargs = {}
 
             if isinstance(values, TypedMapping):
                 return values
 
             if not isinstance(values, (type({}), type(None))):
                 raise TypeError("Invalid type : {}".format(type(values)))
 
@@ -135,15 +140,15 @@
 def str_if_not_none(value):
     """
     Returns an str(value) if the value is not None.
 
     :param value: None or a value that can be converted to a str.
     :return: None or str(value)
     """
-    if not(value is None or isinstance(value, string_types)):
+    if not (value is None or isinstance(value, string_types)):
         value = str(value)
 
     return value
 
 
 def int_if_not_none(value):
     """
@@ -191,16 +196,16 @@
 def to_date_field(formatter):
     """
     Returns a callable instance that will convert a string to a Date.
 
     :param formatter: String that represents data format for parsing.
     :return: instance of the DateConverter.
     """
-    class DateConverter(object):
 
+    class DateConverter(object):
         def __init__(self, formatter):
             self.formatter = formatter
 
         def __call__(self, value):
             if isinstance(value, string_types):
                 value = datetime.strptime(value, self.formatter).date()
 
@@ -215,16 +220,16 @@
 def to_datetime_field(formatter):
     """
     Returns a callable instance that will convert a string to a DateTime.
 
     :param formatter: String that represents data format for parsing.
     :return: instance of the DateTimeConverter.
     """
-    class DateTimeConverter(object):
 
+    class DateTimeConverter(object):
         def __init__(self, formatter):
             self.formatter = formatter
 
         def __call__(self, value):
             if isinstance(value, string_types):
                 value = parser.parse(value)
 
@@ -236,16 +241,16 @@
 def to_time_field(formatter):
     """
     Returns a callable instance that will convert a string to a Time.
 
     :param formatter: String that represents data format for parsing.
     :return: instance of the TimeConverter.
     """
-    class TimeConverter(object):
 
+    class TimeConverter(object):
         def __init__(self, formatter):
             self.formatter = formatter
 
         def __call__(self, value):
             if isinstance(value, string_types):
                 value = datetime.strptime(value, self.formatter).time()
```

### Comparing `related_mltoolbox-1.0.2/src/related/decorators.py` & `related_mltoolbox-1.1.0/src/related/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import inspect
 
 from attr import attrs
 
-from .functions import to_model, to_dict, is_model
+from .functions import is_model, to_dict, to_model
 
 
 def mutable(maybe_cls=None, strict=False):
-
     def wrap(cls):
         wrapped = attrs(cls)
         wrapped.__related_strict__ = strict
         return wrapped
 
     return wrap(maybe_cls) if maybe_cls is not None else wrap
 
 
 def immutable(maybe_cls=None, strict=False):
-
     def wrap(cls):
         wrapped = attrs(cls, frozen=True, slots=True)
         wrapped.__related_strict__ = strict
         return wrapped
 
     return wrap(maybe_cls) if maybe_cls is not None else wrap
 
@@ -36,22 +34,21 @@
     except AttributeError:
         pass
 
     return annotation_map
 
 
 def serializer(func=None, **kwargs):
-
     def _serializer(func):
         # collect map of related models by name (currently not arg index)
         annotation_map = _get_annotation_map(func, **kwargs)
 
         def wrapper(*args, **kwargs):
             # iterate keys that intersect
-            for key in (set(kwargs.keys()) & set(annotation_map.keys())):
+            for key in set(kwargs.keys()) & set(annotation_map.keys()):
                 kwargs[key] = to_model(annotation_map[key], kwargs[key])
 
             # run function getting result
             result = func(*args, **kwargs)
 
             # return
             return to_dict(result)
```

### Comparing `related_mltoolbox-1.0.2/src/related/dispatchers.py` & `related_mltoolbox-1.1.0/src/related/dispatchers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+from datetime import date, datetime, time
 from decimal import Decimal
-from future.moves.urllib.parse import ParseResult
-from collections import OrderedDict
 from enum import Enum
 from uuid import UUID
-from datetime import date, datetime, time
+
+from future.moves.urllib.parse import ParseResult
 
 from .functions import to_dict
 from .types import (
-    TypedSequence, TypedMapping, TypedSet, DEFAULT_DATE_FORMAT,
-    DEFAULT_DATETIME_FORMAT, DEFAULT_TIME_FORMAT
+    DEFAULT_DATE_FORMAT,
+    DEFAULT_DATETIME_FORMAT,
+    DEFAULT_TIME_FORMAT,
+    TypedMapping,
+    TypedSequence,
+    TypedSet,
 )
 
 
 @to_dict.register(list)  # noqa F811
 @to_dict.register(set)
 @to_dict.register(tuple)
 def _(obj, **kwargs):
@@ -23,15 +27,15 @@
         cf = obj.__class__ if retain_collection_types else list
         return cf([to_dict(i, **kwargs) for i in obj])
 
 
 @to_dict.register(dict)  # noqa F811
 def _(obj, **kwargs):
     suppress_empty_values = kwargs.get("suppress_empty_values", False)
-    dict_factory = kwargs.get("dict_factory", OrderedDict)
+    dict_factory = kwargs.get("dict_factory", dict)
 
     items = []
     for kk, vv in obj.items():
         vv = to_dict(vv, **kwargs)
         if (not suppress_empty_values) or (vv is not None):
             items.append((to_dict(kk, **kwargs), vv))
 
@@ -49,15 +53,15 @@
     return to_dict(obj.set, **kwargs)
 
 
 @to_dict.register(TypedMapping)  # noqa F811
 def _(obj, **kwargs):
     suppress_map_key_values = kwargs.get("suppress_map_key_values", False)
     suppress_empty_values = kwargs.get("suppress_empty_values", False)
-    rv = kwargs.get("dict_factory", OrderedDict)()
+    rv = kwargs.get("dict_factory", dict)()
 
     items = obj.items()
 
     for key_value, item in items:
         sub_dict = to_dict(item, **kwargs)
         if suppress_map_key_values:
             sub_dict.pop(obj.key)
@@ -80,27 +84,26 @@
 @to_dict.register(ParseResult)  # noqa F811
 def _(obj, **kwargs):
     return obj.geturl()
 
 
 @to_dict.register(date)  # noqa F811
 def _(obj, **kwargs):
-    formatter = kwargs.get('formatter') or DEFAULT_DATE_FORMAT
+    formatter = kwargs.get("formatter") or DEFAULT_DATE_FORMAT
     return obj.strftime(formatter)
 
 
 @to_dict.register(datetime)  # noqa F811
 def _(obj, **kwargs):
-    formatter = kwargs.get('formatter') or DEFAULT_DATETIME_FORMAT
-    return (obj.isoformat() if formatter == "ISO_FORMAT"
-            else obj.strftime(formatter))
+    formatter = kwargs.get("formatter") or DEFAULT_DATETIME_FORMAT
+    return obj.isoformat() if formatter == "ISO_FORMAT" else obj.strftime(formatter)
 
 
 @to_dict.register(time)  # noqa F811
 def _(obj, **kwargs):
-    formatter = kwargs.get('formatter') or DEFAULT_TIME_FORMAT
+    formatter = kwargs.get("formatter") or DEFAULT_TIME_FORMAT
     return obj.strftime(formatter)
 
 
 @to_dict.register(Decimal)  # noqa F811
 def _(obj, **kwargs):
     return str(obj)
```

### Comparing `related_mltoolbox-1.0.2/src/related/fields.py` & `related_mltoolbox-1.1.0/src/related/fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # -*- coding: utf-8 -*-
+from datetime import date, datetime, time
 from decimal import Decimal
+from uuid import UUID, uuid4
+
+from attr import NOTHING, attrib
 from future.moves.urllib.parse import ParseResult
-from attr import attrib, NOTHING
-from collections import OrderedDict
-from uuid import uuid4, UUID
-from datetime import date, datetime, time
 from six import string_types
 
-from . import _init_fields, types, converters, validators
+from . import _init_fields, converters, types, validators
 
 
-def BooleanField(default=NOTHING, required=True, repr=True, cmp=True,
-                 key=None):
+def BooleanField(default=NOTHING, required=True, repr=True, cmp=True, key=None):
     """
     Create new bool field on a model.
 
     :param default: any boolean value
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, None)
     validator = _init_fields.init_validator(required, bool)
-    return attrib(default=default, validator=validator, repr=repr, cmp=cmp,
-                  metadata=dict(key=key))
+    return attrib(
+        default=default, validator=validator, repr=repr, cmp=cmp, metadata=dict(key=key)
+    )
 
 
-def ChildField(cls, default=NOTHING, required=True, repr=True, cmp=True,
-               key=None):
+def ChildField(cls, default=NOTHING, required=True, repr=True, cmp=True, key=None):
     """
     Create new child field on a model.
 
     :param cls: class (or name) of the model to be related.
     :param default: any object value of type cls
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
@@ -40,152 +39,208 @@
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, None)
     converter = converters.to_child_field(cls)
     validator = _init_fields.init_validator(
         required, object if isinstance(cls, str) else cls
     )
-    return attrib(default=default, converter=converter, validator=validator,
-                  repr=repr, cmp=cmp, metadata=dict(key=key))
+    return attrib(
+        default=default,
+        converter=converter,
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(key=key),
+    )
 
 
-def DateField(formatter=types.DEFAULT_DATE_FORMAT, default=NOTHING,
-              required=True, repr=True, cmp=True, key=None):
+def DateField(
+    formatter=types.DEFAULT_DATE_FORMAT,
+    default=NOTHING,
+    required=True,
+    repr=True,
+    cmp=True,
+    key=None,
+):
     """
     Create new date field on a model.
 
     :param formatter: date formatter string (default: "%Y-%m-%d")
     :param default: any date or string that can be converted to a date value
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, None)
     validator = _init_fields.init_validator(required, date)
     converter = converters.to_date_field(formatter)
-    return attrib(default=default, converter=converter, validator=validator,
-                  repr=repr, cmp=cmp,
-                  metadata=dict(formatter=formatter, key=key))
+    return attrib(
+        default=default,
+        converter=converter,
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(formatter=formatter, key=key),
+    )
 
 
-def DateTimeField(formatter=types.DEFAULT_DATETIME_FORMAT, default=NOTHING,
-                  required=True, repr=True, cmp=True, key=None):
+def DateTimeField(
+    formatter=types.DEFAULT_DATETIME_FORMAT,
+    default=NOTHING,
+    required=True,
+    repr=True,
+    cmp=True,
+    key=None,
+):
     """
     Create new datetime field on a model.
 
     :param formatter: datetime formatter string (default: "ISO_FORMAT")
     :param default: any datetime or string that can be converted to a datetime
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, None)
     validator = _init_fields.init_validator(required, datetime)
     converter = converters.to_datetime_field(formatter)
-    return attrib(default=default, converter=converter, validator=validator,
-                  repr=repr, cmp=cmp,
-                  metadata=dict(formatter=formatter, key=key))
+    return attrib(
+        default=default,
+        converter=converter,
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(formatter=formatter, key=key),
+    )
 
 
-def TimeField(formatter=types.DEFAULT_TIME_FORMAT, default=NOTHING,
-              required=True, repr=True, cmp=True, key=None):
+def TimeField(
+    formatter=types.DEFAULT_TIME_FORMAT,
+    default=NOTHING,
+    required=True,
+    repr=True,
+    cmp=True,
+    key=None,
+):
     """
     Create new time field on a model.
 
     :param formatter: time formatter string (default: "%H:%M:%S")
     :param default: any time or string that can be converted to a time value
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, None)
     validator = _init_fields.init_validator(required, time)
     converter = converters.to_time_field(formatter)
-    return attrib(default=default, converter=converter, validator=validator,
-                  repr=repr, cmp=cmp,
-                  metadata=dict(formatter=formatter, key=key))
+    return attrib(
+        default=default,
+        converter=converter,
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(formatter=formatter, key=key),
+    )
 
 
-def FloatField(default=NOTHING, required=True, repr=True, cmp=True,
-               key=None):
+def FloatField(default=NOTHING, required=True, repr=True, cmp=True, key=None):
     """
     Create new float field on a model.
 
     :param default: any float value
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, None)
     validator = _init_fields.init_validator(required, float)
-    return attrib(default=default, converter=converters.float_if_not_none,
-                  validator=validator, repr=repr, cmp=cmp,
-                  metadata=dict(key=key))
+    return attrib(
+        default=default,
+        converter=converters.float_if_not_none,
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(key=key),
+    )
 
 
-def IntegerField(default=NOTHING, required=True, repr=True, cmp=True,
-                 key=None):
+def IntegerField(default=NOTHING, required=True, repr=True, cmp=True, key=None):
     """
     Create new int field on a model.
 
     :param default: any integer value
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, None)
     validator = _init_fields.init_validator(required, int)
-    return attrib(default=default, converter=converters.int_if_not_none,
-                  validator=validator, repr=repr, cmp=cmp,
-                  metadata=dict(key=key))
+    return attrib(
+        default=default,
+        converter=converters.int_if_not_none,
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(key=key),
+    )
 
 
-def MappingField(cls, child_key, default=NOTHING, required=True, repr=False,
-                 key=None):
+def MappingField(cls, child_key, default=NOTHING, required=True, repr=False, key=None):
     """
     Create new mapping field on a model.
 
     :param cls: class (or name) of the model to be related in Sequence.
     :param child_key: key field on the child object to be used as the map key.
     :param default: any mapping type
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
-    default = _init_fields.init_default(required, default, OrderedDict())
+    default = _init_fields.init_default(required, default, {})
     converter = converters.to_mapping_field(cls, child_key)
     validator = _init_fields.init_validator(required, types.TypedMapping)
-    return attrib(default=default, converter=converter, validator=validator,
-                  repr=repr, metadata=dict(key=key))
+    return attrib(
+        default=default,
+        converter=converter,
+        validator=validator,
+        repr=repr,
+        metadata=dict(key=key),
+    )
 
 
-def RegexField(regex, default=NOTHING, required=True, repr=True, cmp=True,
-               key=None):
+def RegexField(regex, default=NOTHING, required=True, repr=True, cmp=True, key=None):
     """
     Create new str field on a model.
 
     :param regex: regex validation string (e.g. "[^@]+@[^@]+" for email)
     :param default: any string value
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, None)
-    validator = _init_fields.init_validator(required, string_types,
-                                            validators.regex(regex))
-    return attrib(default=default, converter=converters.str_if_not_none,
-                  validator=validator, repr=repr, cmp=cmp,
-                  metadata=dict(key=key))
+    validator = _init_fields.init_validator(
+        required, string_types, validators.regex(regex)
+    )
+    return attrib(
+        default=default,
+        converter=converters.str_if_not_none,
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(key=key),
+    )
 
 
 def SequenceField(cls, default=NOTHING, required=True, repr=False, key=None):
     """
     Create new sequence field on a model.
 
     :param cls: class (or name) of the model to be related in Sequence.
@@ -194,16 +249,21 @@
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, [])
     converter = converters.to_sequence_field(cls)
     validator = _init_fields.init_validator(required, types.TypedSequence)
-    return attrib(default=default, converter=converter, validator=validator,
-                  repr=repr, metadata=dict(key=key))
+    return attrib(
+        default=default,
+        converter=converter,
+        validator=validator,
+        repr=repr,
+        metadata=dict(key=key),
+    )
 
 
 def SetField(cls, default=NOTHING, required=True, repr=False, key=None):
     """
     Create new set field on a model.
 
     :param cls: class (or name) of the model to be related in Set.
@@ -212,34 +272,43 @@
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, set())
     converter = converters.to_set_field(cls)
     validator = _init_fields.init_validator(required, types.TypedSet)
-    return attrib(default=default, converter=converter, validator=validator,
-                  repr=repr, metadata=dict(key=key))
+    return attrib(
+        default=default,
+        converter=converter,
+        validator=validator,
+        repr=repr,
+        metadata=dict(key=key),
+    )
 
 
-def StringField(default=NOTHING, required=True, repr=True, cmp=True,
-                key=None):
+def StringField(default=NOTHING, required=True, repr=True, cmp=True, key=None):
     """
     Create new str field on a model.
 
     :param default: any string value
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, None)
     validator = _init_fields.init_validator(required, string_types)
-    return attrib(default=default, converter=converters.str_if_not_none,
-                  validator=validator, repr=repr, cmp=cmp,
-                  metadata=dict(key=key))
+    return attrib(
+        default=default,
+        converter=converters.str_if_not_none,
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(key=key),
+    )
 
 
 def URLField(default=NOTHING, required=True, repr=True, cmp=True, key=None):
     """
     Create new UUID field on a model.
 
     :param default: any value
@@ -247,17 +316,22 @@
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     cls = ParseResult
     default = _init_fields.init_default(required, default, None)
     validator = _init_fields.init_validator(required, cls)
-    return attrib(default=default, converter=converters.str_to_url,
-                  validator=validator, repr=repr, cmp=cmp,
-                  metadata=dict(key=key))
+    return attrib(
+        default=default,
+        converter=converters.str_to_url,
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(key=key),
+    )
 
 
 def UUIDField(default=NOTHING, required=False, repr=True, cmp=True, key=None):
     """
     Create new UUID field on a model.
 
     :param default: any value
@@ -265,28 +339,37 @@
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     cls = UUID
     default = _init_fields.init_default(required, default, uuid4)
     validator = _init_fields.init_validator(required, cls)
-    return attrib(default=default, converter=converters.str_to_uuid,
-                  validator=validator, repr=repr, cmp=cmp,
-                  metadata=dict(key=key))
+    return attrib(
+        default=default,
+        converter=converters.str_to_uuid,
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(key=key),
+    )
 
 
-def DecimalField(default=NOTHING, required=True, repr=True, cmp=True,
-                 key=None):
+def DecimalField(default=NOTHING, required=True, repr=True, cmp=True, key=None):
     """
     Create new decimal field on a model.
 
     :param default: any decimal value
     :param bool required: whether or not the object is invalid if not provided.
     :param bool repr: include this field should appear in object's repr.
     :param bool cmp: include this field in generated comparison.
     :param string key: override name of the value when converted to dict.
     """
     default = _init_fields.init_default(required, default, None)
     validator = _init_fields.init_validator(required, Decimal)
-    return attrib(default=default, converter=lambda x: Decimal(x),
-                  validator=validator, repr=repr, cmp=cmp,
-                  metadata=dict(key=key))
+    return attrib(
+        default=default,
+        converter=lambda x: Decimal(x),
+        validator=validator,
+        repr=repr,
+        cmp=cmp,
+        metadata=dict(key=key),
+    )
```

### Comparing `related_mltoolbox-1.0.2/src/related/functions.py` & `related_mltoolbox-1.1.0/src/related/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from __future__ import absolute_import, division, print_function
 
-from collections import OrderedDict
-from enum import Enum
-from typing import Type
-
 import json
+from enum import Enum
 
 from attr._make import fields
 
 try:
     from functools import singledispatch
 except ImportError:
     from singledispatch import singledispatch
@@ -35,53 +32,53 @@
     # else, return obj directly. register a custom to_dict if you need to!
     #   reference: https://pypi.python.org/pypi/singledispatch
     else:
         return obj
 
 
 def related_obj_to_dict(obj, **kwargs):
-    """ Covert a known related object to a dictionary. """
+    """Covert a known related object to a dictionary."""
 
     # Explicitly discard formatter kwarg, should not be cascaded down.
-    kwargs.pop('formatter', None)
+    kwargs.pop("formatter", None)
 
     # If True, remove fields that start with an underscore (e.g. _secret)
     suppress_private_attr = kwargs.get("suppress_private_attr", False)
 
     # if True, don't store fields with None values into dictionary.
     suppress_empty_values = kwargs.get("suppress_empty_values", False)
 
     # get list of attrs fields
     attrs = fields(obj.__class__)
 
-    # instantiate return dict, use OrderedDict type by default
-    return_dict = kwargs.get("dict_factory", OrderedDict)()
+    # instantiate return dict, use dict type by default
+    return_dict = kwargs.get("dict_factory", dict)()
 
     for a in attrs:
 
         # skip if private attr and flag tells you to skip
         if suppress_private_attr and a.name.startswith("_"):
             continue
 
         metadata = a.metadata or {}
 
         # formatter is a related-specific `attrs` meta field
         #   see fields.DateField
-        formatter = metadata.get('formatter')
+        formatter = metadata.get("formatter")
 
         # get value and call to_dict on it, passing the kwargs/formatter
         value = getattr(obj, a.name)
         value = to_dict(value, formatter=formatter, **kwargs)
 
         # check flag, skip None values
         if suppress_empty_values and value is None:
             continue
 
         # field name can be overridden by the metadata field
-        key_name = a.metadata.get('key') or a.name
+        key_name = a.metadata.get("key") or a.name
 
         # store converted / formatted value into return dictionary
         return_dict[key_name] = value
 
     return return_dict
 
 
@@ -105,26 +102,26 @@
     else:
         value = cls(value)
 
     return value
 
 
 def convert_key_to_attr_names(cls, original):
-    """ convert key names to their corresponding attribute names """
+    """convert key names to their corresponding attribute names"""
     attrs = fields(cls)
     updated = {}
     keys_pulled = set()
 
     for a in attrs:
-        key_name = a.metadata.get('key') or a.name
+        key_name = a.metadata.get("key") or a.name
         if key_name in original:
             updated[a.name] = original.get(key_name)
             keys_pulled.add(key_name)
 
-    if getattr(cls, '__related_strict__', False):
+    if getattr(cls, "__related_strict__", False):
         extra = set(original.keys()) - keys_pulled
         if len(extra):
             raise ValueError("Extra keys (strict mode): {}".format(extra))
 
     return updated
 
 
@@ -136,64 +133,66 @@
     :raise TypeError: If *cls* is not a class.
 
     :rtype: :class:`bool`
     """
     return getattr(cls, "__attrs_attrs__", None) is not None
 
 
-def to_yaml(obj, yaml_package, dumper_cls, stream=None, default_flow_style=False,
-            **kwargs):
+def to_yaml(
+    obj, yaml_package, dumper_cls, stream=None, default_flow_style=False, **kwargs
+):
     """
-    Serialize a Python object into a YAML stream with OrderedDict and
+    Serialize a Python object into a YAML stream with dict and
     default_flow_style defaulted to False.
 
     If stream is None, return the produced string instead.
 
-    OrderedDict reference: http://stackoverflow.com/a/21912744
     default_flow_style reference: http://stackoverflow.com/a/18210750
 
     :param data: python object to be serialized
     :param stream: to be serialized to
     :param Dumper: base Dumper class to extend.
     :param kwargs: arguments to pass to to_dict
     :return: stream if provided, string if stream is None
     """
 
     class OrderedDumper(dumper_cls):
         pass
 
     def dict_representer(dumper, data):
         return dumper.represent_mapping(
-            yaml_package.resolver.BaseResolver.DEFAULT_MAPPING_TAG,
-            data.items())
+            yaml_package.resolver.BaseResolver.DEFAULT_MAPPING_TAG, data.items()
+        )
 
-    OrderedDumper.add_representer(OrderedDict, dict_representer)
+    OrderedDumper.add_representer(dict, dict_representer)
 
     obj_dict = to_dict(obj, **kwargs)
 
-    return yaml_package.dump(obj_dict, stream, OrderedDumper,
-                     default_flow_style=default_flow_style)
+    return yaml_package.dump(
+        obj_dict, stream, OrderedDumper, default_flow_style=default_flow_style
+    )
 
 
-def from_yaml(stream, yaml_package, loader_cls, cls=None,
-              object_pairs_hook=OrderedDict, **extras):
+def from_yaml(
+    stream, yaml_package, loader_cls, cls=None, object_pairs_hook=dict, **extras
+):
     """
     Convert a YAML stream into a class via the OrderedLoader class.
     """
 
     class OrderedLoader(loader_cls):
         pass
 
     def construct_mapping(loader, node):
         loader.flatten_mapping(node)
         return object_pairs_hook(loader.construct_pairs(node))
 
     OrderedLoader.add_constructor(
-        yaml_package.resolver.BaseResolver.DEFAULT_MAPPING_TAG,
-        construct_mapping)
+        yaml_package.resolver.BaseResolver.DEFAULT_MAPPING_TAG, construct_mapping
+    )
 
     yaml_dict = yaml_package.load(stream, OrderedLoader) or {}
     yaml_dict.update(extras)
     return cls(**yaml_dict) if cls else yaml_dict
 
 
 def to_json(obj, indent=4, sort_keys=True, **kwargs):
@@ -204,16 +203,16 @@
     :param kwargs: arguments to pass to to_dict
     :return: json string
     """
     obj_dict = to_dict(obj, **kwargs)
     return json.dumps(obj_dict, indent=indent, sort_keys=sort_keys)
 
 
-def from_json(stream, cls=None, object_pairs_hook=OrderedDict, **extras):
+def from_json(stream, cls=None, object_pairs_hook=dict, **extras):
     """
     Convert a JSON string or stream into specified class.
     """
-    stream = stream.read() if hasattr(stream, 'read') else stream
+    stream = stream.read() if hasattr(stream, "read") else stream
     json_dict = json.loads(stream, object_pairs_hook=object_pairs_hook)
     if extras:
         json_dict.update(extras)  # pragma: no cover
     return to_model(cls, json_dict) if cls else json_dict
```

### Comparing `related_mltoolbox-1.0.2/src/related/types.py` & `related_mltoolbox-1.1.0/src/related/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # -*- coding: utf-8 -*-
 from attr.exceptions import FrozenInstanceError
-from collections import OrderedDict
 
 try:
-    from collections.abc import (MutableSequence, MutableMapping, MutableSet)
+    from collections.abc import MutableMapping, MutableSequence, MutableSet
 except ImportError:
-    from collections import (MutableSequence, MutableMapping, MutableSet)
+    from collections import MutableMapping, MutableSequence, MutableSet
 
 
 DEFAULT_DATE_FORMAT = "%Y-%m-%d"
 DEFAULT_DATETIME_FORMAT = "ISO_FORMAT"
 DEFAULT_TIME_FORMAT = "%H:%M:%S"
 
 
 class ImmutableDict(dict):
-
     def __setitem__(self, key, value):
         raise FrozenInstanceError()
 
     def __delitem__(self, key):
         raise FrozenInstanceError()
 
     def __setattr__(self, name, value):
@@ -75,31 +73,30 @@
 
     def insert(self, i, v):
         self._check(v)
         self.list.insert(i, v)
 
     def _check(self, v):
         if not isinstance(v, self.allowed_types):
-            raise TypeError("Invalid value %s (%s != %s)" %
-                            (v, type(v), self.cls))
+            raise TypeError("Invalid value %s (%s != %s)" % (v, type(v), self.cls))
 
 
 class TypedMapping(MutableMapping):
     """
     Custom dict type that checks the instance type of new values.
 
     reference:
     http://stackoverflow.com/a/3488283
     """
 
     def __init__(self, cls, kwargs, key=None, allow_none=True):
         self.cls = cls
         self.allowed_types = (cls, type(None)) if allow_none else cls
         self.key = key
-        self.dict = OrderedDict()
+        self.dict = {}
         self.update(kwargs)
 
     def __str__(self):
         return str(self.dict)
 
     def __repr__(self):
         return repr(self.dict)
@@ -182,9 +179,8 @@
         self.set.add(v)
 
     def discard(self, value):
         self.set.discard(value)
 
     def _check(self, v):
         if not isinstance(v, self.allowed_types):
-            raise TypeError("Invalid value %s (%s != %s)" %
-                            (v, type(v), self.cls))
+            raise TypeError("Invalid value %s (%s != %s)" % (v, type(v), self.cls))
```

### Comparing `related_mltoolbox-1.0.2/src/related/validators.py` & `related_mltoolbox-1.1.0/src/related/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-from attr import attr, attributes
 import re
 
+from attr import attr, attributes
+
 
 @attributes(repr=False, slots=True)
 class _CompositeValidator(object):
     validators = attr()
 
     def __call__(self, inst, attr, value):
         for validator in self.validators:
             validator(inst, attr, value)
 
     def __repr__(self):
-        return (
-            "<composite validator for validators {!r}>".format(self.validators)
-        )
+        return "<composite validator for validators {!r}>".format(self.validators)
 
 
 def composite(*validators):
-    """A validator that executes each validator passed as arguments.
-    """
+    """A validator that executes each validator passed as arguments."""
     return _CompositeValidator(validators)
 
 
 @attributes(repr=False, slots=True)
 class _RegexValidator(object):
     regex = attr()
 
     def __call__(self, inst, attr, value):
         if not re.match(self.regex, value):
             raise TypeError(
                 "'{name}' must match {regex!r} (got {value!r}).".format(
-                    name=attr.name, regex=self.regex, value=value), attr,
-                self.regex, value)
+                    name=attr.name, regex=self.regex, value=value
+                ),
+                attr,
+                self.regex,
+                value,
+            )
 
     def __repr__(self):
-        return (
-            "<regex validator for {!r}>".format(self.regex)
-        )
+        return "<regex validator for {!r}>".format(self.regex)
 
 
 def regex(match_string):
-    """A validator that executes each validator passed as arguments.
-
-    """
+    """A validator that executes each validator passed as arguments."""
     return _RegexValidator(match_string)
```

### Comparing `related_mltoolbox-1.0.2/setup.py` & `related_mltoolbox-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['PyYAML', 'attrs', 'future', 'python-dateutil']
 
 setup_kwargs = {
     'name': 'related-mltoolbox',
-    'version': '1.0.2',
+    'version': '1.1.0',
     'description': '(Fork from related) Related: Straightforward nested object models in Python',
     'long_description': '# related-mltoolbox\n(fork from) https://github.com/genomoncology/related\n\n`Related` is a Python library for creating nested object models\nthat can be serialized to and de-serialized from\nnested python dictionaries.\nWhen paired with other libraries (e.g. [PyYAML]),\n`Related` object models can be used to convert to and from\nnested data formats (e.g. JSON, YAML).\n\nExample use cases for `related` object models include:\n\n* Configuration file reading and writing\n* REST API message response generation and request processing\n* Object-Document Mapping for a document store (e.g. MongoDB, elasticsearch)\n* Data import parsing or export generation\n\n<br/><br/>\n\n<img src=\'./.images/flow.png\' width=\'750\' align="center" />\n\n\n# Installation\n\nInstall using `pip`...\n\n    pip install related-mltoolbox\n\n\n# First Example\n\n```python\nimport related\nimport yaml\n\n@related.immutable\nclass Person(object):\n    first_name = related.StringField()\n    last_name = related.StringField()\n\n@related.immutable\nclass RoleModels(object):\n    scientists = related.SetField(Person)\n\npeople = [Person(first_name="Grace", last_name="Hopper"),\n          Person(first_name="Katherine", last_name="Johnson"),\n          Person(first_name="Katherine", last_name="Johnson")]\n\nprint(related.to_yaml(obj=RoleModels(scientists=people), yaml_package=yaml, dumper_cls=yaml.yaml.Dumper))\n```\n\nYields:\n\n```yaml\nscientists:\n- first_name: Grace\n  last_name: Hopper\n- first_name: Katherine\n  last_name: Johnson\n```\n\n\n# Second Example\n\nThe below example is based off of this [Docker Compose example].\nIt shows how a YAML file can be loaded into an object model, tested, and\nthen generated back into a string that matches the original YAML.\n\n```yaml\nversion: \'2\'\nservices:\n  web:\n    build: .\n    ports:\n    - 5000:5000\n    volumes:\n    - .:/code\n  redis:\n    image: redis\n```\n\nBelow is the `related` object model that represents the above configuration.\nNotice how the name-based mapping of services (i.e. web, redis) are\nrepresented by the model.\n\n\n```python\nimport related\n\n\n@related.immutable\nclass Service(object):\n    name = related.StringField()\n    image = related.StringField(required=False)\n    build = related.StringField(required=False)\n    ports = related.SequenceField(str, required=False)\n    volumes = related.SequenceField(str, required=False)\n    command = related.StringField(required=False)\n\n\n@related.immutable\nclass Compose(object):\n    version = related.StringField(required=False, default=None)\n    services = related.MappingField(Service, "name", required=False)\n```\n\nThe above yaml can then be loaded by using one of the convenience\nmethod and then round-tripped back to yaml to check that the format\nhas been maintained. The `related` module uses `OrderedDict` objects\nin order to maintain sort order by default.\n\n```python\nfrom os.path import join, dirname\n\nimport yaml\nfrom model import Compose\nfrom related import to_yaml, from_yaml, to_model\n\nYML_FILE = join(dirname(__file__), "docker-compose.yml")\n\n\ndef test_compose_from_yml():\n    original_yaml = open(YML_FILE).read().strip()\n    yml_dict = from_yaml(stream=original_yaml, yaml_package=yaml, loader_cls=yaml.Loader)\n    compose = to_model(Compose, yml_dict)\n\n    assert compose.version == \'2\'\n    assert compose.services[\'web\'].ports == ["5000:5000"]\n    assert compose.services[\'redis\'].image == "redis"\n\n    generated_yaml = to_yaml(compose,\n                             suppress_empty_values=True,\n                             suppress_map_key_values=True).strip()\n\n    assert original_yaml == generated_yaml\n```\n\n\n# More Examples\n\nMore examples can be found by reviewing the [tests/] folder of this project.\nBelow are links and descriptions of the tests provided so far.\n\n| Example        | description                                                        |\n| -------------- | ------------------------------------------------------------------ |\n| [Example 00]   | First example above that shows how SetFields work.                 |\n| [Example 01]   | Second example above that demonstrates YAML (de)serialization.     |\n| [Example 02]   | Compose v3 with long-form ports and singledispatch to_dict         |\n| [Example 03]   | A single class (Company) with a bunch of value fields.             |\n| [Example 04]   | A multi-class object model with Enum class value field.            |\n| [Example 05]   | Handling of renaming of attributes including Python keywords.      |\n| [Example 06]   | Basic JSON (de)serialization with TimeField, DateTimeField and DecimalField.     |\n| [Example 07]   | Function decorator that converts inputs to obj and outputs to dict |\n| [Example 08]   | Handle self-referencing and out-of-order references using strings. |\n\n\n# Documentation\n\nBelow is a quick version of documentation until more time can be dedicated.\n\n\n## Overview\n\nThe [attrs] library is the underlying engine for `related`.\nAs explained in [this article by Glyph],\n`attrs` cleanly and cleverly\neliminates a lot of the boilerplate\nrequired when creating Python classes\nwithout using inheritance.\nSome core functionality provided by attrs:\n\n* Generated initializer method\n    (``__init__``)\n* Generated comparison methods\n    (``__eq__``, ``__ne__``, ``__lt__``, ``__le__``, ``__gt__``, ``__ge__`` )\n* Human-readable representation method\n    (``__repr__``)\n* Attribute converter and validator framework\n\n\nThe `related` project is an opinionated layer\nbuilt on top of the `attrs` library\nthat provides the following:\n\n* Value fields that handle both validation and conversion\n  to and from basic data types like\n  ``str``, ``float``, and ``bool``.\n* Nested fields that support relationships such as\n  Child, Sequences, Mappings, and Sets of objects.\n* ``to_dict`` function that converts nested object graphs\n  to python dictionaries.\n  Made customizable (without resorting to [monkey-patching])\n  by the [singledispatch library].\n* ``to_model`` function that instantiated classes\n  used by the de-serialization process going from\n  python dictionaries to the related model.\n* Conversion helper functions\n  (``to_yaml``, ``from_yaml``, ``to_json``, ``from_json``)\n  for easily going between\n  related models and data formats.\n* ``@mutable`` and ``@immutable`` for decorating classes\n  as related models without the need for inheritance increasing\n  maintainability and flexibility.\n\n\n## Class Decorators\n\n| decorator             | description                                                      |\n| --------------        | ---------------------------------------------------------------- |\n| @mutable              | Activate a related class that instantiates changeable objects.   |\n| @immutable            | Activate a related class that instantiates unchangeable objects. |\n\nSee the [decorators.py] file to view the source code until proper\ndocumentation is generated.\n\n\n## Field Types\n\n| field type            | description                                                      |\n| --------------        | ---------------------------------------------------------------- |\n| BooleanField          | `bool` value field.                                              |\n| ChildField            | Child object of a specified type `cls`.                          |\n| DateField             | `date` field formatted using `formatter`.                        |\n| DateTimeField         | `datetime` field formatted using `formatter`.                    |\n| TimeField             | `time` field formatted using `formatter`.                    |\n| FloatField            | `float` value field.                                             |\n| IntegerField          | `int` value field.                                               |\n| MappingField(cls,key) | Dictionary of objects of type `cls` index by `key` field values. |\n| RegexField(regex)     | `str` value field that is validated by re.match(`regex`).        |\n| SequenceField(cls)    | List of objects all of specified type `cls`.                     |\n| SetField              | Set of objects all of a specified type `cls`.                    |\n| StringField           | `str` value field.                                               |\n| URLField              | [ParseResult] object.                                            |\n| UUIDField             | [UUID] object, will create [uuid4] by default if not specified.  |\n\n\nAdding your own field types is fairly straightforward\ndue to the power of the underlying `attrs` project.\nSee the [fields.py] file to see how the above are constructed.\n\n\n## Functions\n\n| function                        | description                                           |\n| ------------------------------- | ----------------------------------------------------- |\n| from_json(s,cls)                | Convert a JSON string or stream into specified class. |\n| from_yaml(s, yaml, loader, cls) | Convert a YAML string or stream into specified class. |\n| is_related(obj)                 | Returns True if object is @mutable or @immutable.     |\n| to_dict(obj)                    | Singledispatch function for converting to a dict.     |\n| to_json(obj)                    | Convert object to a (pretty) JSON string via to_dict. |\n| to_model(cls,value)             | Convert a value to a `cls` instance.                  |\n| to_yaml(obj, yaml, dumper)      | Convert object to a YAML string via to_dict.          |\n\n\nSee the [functions.py] file to view the source code until proper\ndocumentation is generated.\n\n\n# Credits/Prior Art\n\nThe `related` project has been heavily influenced by the following\nprojects that might be worth looking at if `related` doesn\'t meet your needs.\n\n* [attrs] - The engine that powers `related` functionality.\n* [Django ORM] - Object-relational mapping for Django that inspired `related\'s` design.\n* [cattrs] - Alternative take for handling nested-objects using `attrs`.\n* [addict] and [box] - Python dictionary wrappers that do not require a model.\n* [Jackson] - Java-based technology for serializing and de-serializing objects.\n\n\n# License\n\nThe MIT License (MIT)\n\nCopyright (c) [Open Logistics Foundation]\n\nCopyright (c) 2017 [Ian Maurer], [Genomoncology LLC]\n\n\n\n\n[flow-image]: ./.images/flow.png\n[decorators.py]: ./src/related/decorators.py\n[fields.py]: ./src/related/fields.py\n[functions.py]: ./src/related/functions.py\n[attrs]: http://attrs.readthedocs.io/en/stable/\n[this article by Glyph]: https://glyph.twistedmatrix.com/2016/08/attrs.html\n[Genomoncology LLC]: http://genomoncology.com\n[Ian Maurer]: https://github.com/imaurer\n[Open Logistics Foundation]: https://www.openlogisticsfoundation.org/\n[singledispatch library]: https://pypi.python.org/pypi/singledispatch\n[monkey-patching]: http://stackoverflow.com/questions/5626193/what-is-a-monkey-patch\n[Django ORM]: https://docs.djangoproject.com/en/1.11/topics/db/models/\n[UUID]: https://docs.python.org/3/library/uuid.html#uuid.UUID\n[uuid4]: https://docs.python.org/3/library/uuid.html#uuid.uuid4\n[ParseResult]: https://docs.python.org/2/library/urlparse.html#urlparse.ParseResult\n[cattrs]: http://cattrs.readthedocs.io/en/latest/readme.html\n[addict]: https://github.com/mewwts/addict\n[box]: https://pypi.python.org/pypi/python-box\n[Jackson]: https://github.com/FasterXML/jackson\n[Docker Compose example]: https://docs.docker.com/compose/gettingstarted/#step-3-define-services-in-a-compose-file\n[PyYAML]: https://pypi.python.org/pypi/PyYAML\n\n[tests/]: ./tests/\n[Example 00]: ./tests/ex00_sets_hashes\n[Example 01]: ./tests/ex01_compose_v2\n[Example 02]: ./tests/ex02_compose_v3.2\n[Example 03]: ./tests/ex03_company\n[Example 04]: ./tests/ex04_contact\n[Example 05]: ./tests/ex05_field_names\n[Example 06]: ./tests/ex06_json\n[Example 07]: ./tests/ex07_serializer\n[Example 08]: ./tests/ex08_self_reference\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/related-mltoolbox',
```

### Comparing `related_mltoolbox-1.0.2/PKG-INFO` & `related_mltoolbox-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: related-mltoolbox
-Version: 1.0.2
+Version: 1.1.0
 Summary: (Fork from related) Related: Straightforward nested object models in Python
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/related-mltoolbox
 License: MIT
 Keywords: related,object,models,yaml,json,dict,nested
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.6.2,<4.0.0
```

