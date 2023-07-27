# Comparing `tmp/bstk_datatables-0.2.0.tar.gz` & `tmp/bstk_datatables-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_datatables-0.2.0.tar", max compression
+gzip compressed data, was "bstk_datatables-0.2.1.tar", max compression
```

## Comparing `bstk_datatables-0.2.0.tar` & `bstk_datatables-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4244 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/README.md
--rw-r--r--   0        0        0     2358 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/__init__.py
--rw-r--r--   0        0        0     2311 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/entry.py
--rw-r--r--   0        0        0      560 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/enum.py
--rw-r--r--   0        0        0     3248 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/merge.py
--rw-r--r--   0        0        0     8118 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/schema.py
--rw-r--r--   0        0        0     1565 2023-07-25 05:46:21.109636 bstk_datatables-0.2.0/bstk_datatables/table.py
--rw-r--r--   0        0        0      669 2023-07-25 05:46:45.349943 bstk_datatables-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4244 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/README.md
+-rw-r--r--   0        0        0     2358 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/__init__.py
+-rw-r--r--   0        0        0     2311 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/entry.py
+-rw-r--r--   0        0        0      560 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/enum.py
+-rw-r--r--   0        0        0     3522 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/merge.py
+-rw-r--r--   0        0        0     9455 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/schema.py
+-rw-r--r--   0        0        0     1565 2023-07-27 11:20:18.916744 bstk_datatables-0.2.1/bstk_datatables/table.py
+-rw-r--r--   0        0        0      669 2023-07-27 11:20:42.281086 bstk_datatables-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.2.1/PKG-INFO
```

### Comparing `bstk_datatables-0.2.0/README.md` & `bstk_datatables-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.0/bstk_datatables/__init__.py` & `bstk_datatables-0.2.1/bstk_datatables/__init__.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.0/bstk_datatables/entry.py` & `bstk_datatables-0.2.1/bstk_datatables/entry.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.0/bstk_datatables/enum.py` & `bstk_datatables-0.2.1/bstk_datatables/enum.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.0/bstk_datatables/schema.py` & `bstk_datatables-0.2.1/bstk_datatables/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -111,14 +111,22 @@
         _schema: MarshmallowSchema = self._schema()
         failures = _schema.validate(data=values)
         if not failures:
             return
 
         raise SchemaValuesError(errors=failures)
 
+    def get_defaults(self) -> typing.Dict:
+        _schema: MarshmallowSchema = self._schema()
+        return _schema.dump({})
+
+    def merge_defaults(self, values: typing.Dict) -> typing.Dict:
+        _defaults = self.get_defaults()
+        return {**_defaults, **values}
+
     def export(self) -> typing.Dict[typing.AnyStr, typing.Any]:
         _fields = ["uuid", "name", "code", "references"]
         rtn = {}
         for _exportfield in _fields:
             rtn[_exportfield] = self.__dict__[_exportfield]
         rtn["fields"] = [_field.export() for _field in self.fields]
         return rtn
@@ -169,14 +177,15 @@
         return _rtn
 
 
 @dataclass
 class SchemaFieldFormat:
     type: typing.Optional[typing.AnyStr]
     values: typing.Optional[typing.Any] = None
+    default_value: typing.Optional[typing.Any] = None
     lookup: typing.Optional[typing.Any] = None
     required: typing.Optional[bool] = field(default=False)
     readonly: typing.Optional[bool] = field(default=False)
     many: typing.Optional[bool] = field(default=False)
     markup: typing.Optional[typing.Dict] = field(default=None)
     _field: marshmallow_fields.Field = field(init=False, default=None)
     _missing_lookup: bool = field(init=False, default=False)
@@ -187,15 +196,24 @@
     def attach_lookup(
         self, lookup_value: typing.Union[typing.List[typing.AnyStr], PyEnum]
     ):
         self.lookup = lookup_value
         self._generate_marshmallow_field()
 
     def export(self) -> typing.Dict[typing.AnyStr, typing.Any]:
-        _fields = ["type", "values", "lookup", "required", "readonly", "many", "markup"]
+        _fields = [
+            "type",
+            "values",
+            "default_value",
+            "lookup",
+            "required",
+            "readonly",
+            "many",
+            "markup",
+        ]
         rtn = {}
         for _exportfield in _fields:
             if _exportfield == "lookup" and isinstance(
                 self.__dict__[_exportfield], Enum
             ):
                 rtn[_exportfield] = self.__dict__[_exportfield].code
                 continue
@@ -207,37 +225,66 @@
         if self.type in SCHEMAFIELD_MAP:
             return SCHEMAFIELD_MAP[self.type]
 
         raise ValueError(f"Field format type `{self.type}` is invalid")
 
     def _get_field_params(self) -> typing.Union[None, typing.Dict]:
         _field_params = {}
+
         if self.required is not None:
             _field_params["required"] = self.required
+
         if self.readonly is True:
             _field_params["dump_only"] = True
+
         if self.type == "enum":
             self._missing_lookup = False
             if self.values:
                 _field_params["enum"] = PyEnum("enum", self.values)
             elif self.lookup and isinstance(self.lookup, Enum):
                 _field_params["enum"] = self.lookup.values
             else:
                 self._missing_lookup = True
                 return None
 
+            if self.default_value:
+                _field_params["dump_default"] = self._process_enum_default(
+                    _field_params["enum"]
+                )
+
+        if self.type != "enum":
+            if self.default_value is not None:
+                _field_params["dump_default"] = self.default_value
+
         if self.type not in SCHEMAFIELD_EXTATTR:
             return _field_params
 
         return {**_field_params, **SCHEMAFIELD_EXTATTR[self.type]}
 
+    def _process_enum_default(self, enum_data: Enum):
+        if not self.default_value:
+            return None
+
+        for _member in enum_data:
+            if _member.name == self.default_value:
+                return _member
+
+        # TODO : Check for this much earlier
+        raise ValueError("Invalid default value")
+
     def _generate_marshmallow_field(self):
         _field_params = self._get_field_params()
         if _field_params is None:
             return
 
-        if self.many:
-            self._field = marshmallow_fields.List(
-                self._get_mapped_fieldclass()(**_field_params)
-            )
+        _field_class = self._get_mapped_fieldclass()
+        if issubclass(_field_class, marshmallow_fields.Enum) and self.many:
+            mapped_field = _field_class(enum=_field_params.get("enum"))
+            del _field_params["enum"]
         else:
-            self._field = self._get_mapped_fieldclass()(**_field_params)
+            mapped_field = _field_class(**_field_params)
+
+        if not self.many:
+            self._field = mapped_field
+            return
+
+        self._field = marshmallow_fields.List(mapped_field, **_field_params)
```

### Comparing `bstk_datatables-0.2.0/bstk_datatables/table.py` & `bstk_datatables-0.2.1/bstk_datatables/table.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.0/pyproject.toml` & `bstk_datatables-0.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk-datatables"
-version = "0.2.0"
+version = "0.2.1"
 description = "A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!"
 authors = ["colin <colin@broadstack.com.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bstk_datatables" }]
 
 [tool.poetry.dependencies]
```

### Comparing `bstk_datatables-0.2.0/PKG-INFO` & `bstk_datatables-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk-datatables
-Version: 0.2.0
+Version: 0.2.1
 Summary: A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!
 License: MIT
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

