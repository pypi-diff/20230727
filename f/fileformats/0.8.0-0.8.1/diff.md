# Comparing `tmp/fileformats-0.8.0.tar.gz` & `tmp/fileformats-0.8.1.tar.gz`

## Comparing `fileformats-0.8.0.tar` & `fileformats-0.8.1.tar`

### file list

```diff
@@ -1,50 +1,49 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/archive/__init__.py
--rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/_version.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/converter.py
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/datatype.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/field.py
--rw-r--r--   0        0        0    45604 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/fileset.py
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/mark.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/mixin.py
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/utils.py
--rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_subpackages.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_test_extras.py
--rw-r--r--   0        0        0    11540 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/document/__init__.py
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/base.py
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/notclassifiedyet.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/vector.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/misc/medical.py
--rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/misc/unclassified.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/model/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/testing/basic.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/testing/classifiers.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/testing/headers.py
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/text/__init__.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.0/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.0/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.0/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.0/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.8.0/README.rst
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 fileformats-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    22348 2020-02-02 00:00:00.000000 fileformats-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/converter.py
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/datatype.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/field.py
+-rw-r--r--   0        0        0    46110 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/mark.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/mixin.py
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/utils.py
+-rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_subpackages.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_test_extras.py
+-rw-r--r--   0        0        0    11504 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/base.py
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/notclassifiedyet.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/vector.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/misc/medical.py
+-rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/misc/unclassified.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/model/__init__.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/testing/basic.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/testing/classifiers.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/testing/headers.py
+-rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/text/__init__.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.1/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.1/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.1/LICENSE
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 fileformats-0.8.1/README.rst
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fileformats-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    23194 2020-02-02 00:00:00.000000 fileformats-0.8.1/PKG-INFO
```

### Comparing `fileformats-0.8.0/fileformats/archive/__init__.py` & `fileformats-0.8.1/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/audio/__init__.py` & `fileformats-0.8.1/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/converter.py` & `fileformats-0.8.1/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/datatype.py` & `fileformats-0.8.1/fileformats/core/datatype.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                 class_name = from_mime_format_name(format_name)
                 raise FormatRecognitionError(
                     f"Did not find class matching extension the class name '{class_name}' "
                     f"corresponding to MIME type '{mime_string}' "
                     f"in any of the installed namespaces: {namespace_names}"
                 )
             elif len(matching_name) > 1:
-                namespace_names = [f.__module__.__name__ for f in matching_name]
+                namespace_names = [f.__module__ for f in matching_name]
                 raise FormatRecognitionError(
                     f"Ambiguous extended MIME type '{mime_string}', could refer to "
                     f"{', '.join(repr(f) for f in matching_name)} installed types. "
                     f"Explicitly set the 'iana_mime' attribute on one or all of these types "
                     f"to disambiguate, or uninstall all but one of the following "
                     "namespaces: "
                 )
```

### Comparing `fileformats-0.8.0/fileformats/core/exceptions.py` & `fileformats-0.8.1/fileformats/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/field.py` & `fileformats-0.8.1/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/fileset.py` & `fileformats-0.8.1/fileformats/core/fileset.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     fspaths: ty.FrozenSet[Path] = attrs.field(default=None, converter=fspaths_converter)
 
     # Explicitly set the Internet Assigned Numbers Authority (https://iana_mime.org) MIME
     # type to None for any base classes that should not correspond to a MIME or MIME-like
     # type.
     iana_mime = None
     ext = None
+    alternate_exts = ()
 
     # Store converters registered by @converter decorator that convert to FileSet
     # NB: each class will have its own version of this dictionary
     converters = {}
 
     is_fileset = True
 
@@ -179,14 +180,23 @@
 
     @classproperty
     def unconstrained(cls) -> bool:
         """Whether the file-format is unconstrained by extension, magic number or another
         constraint"""
         return not list(cls.required_properties())
 
+    @classproperty
+    def possible_exts(cls):
+        possible = [cls.ext]
+        try:
+            possible.extend(cls.alternate_exts)
+        except AttributeError:
+            pass
+        return possible
+
     @classmethod
     def required_properties(cls):
         """Find all properties required to treat file-set as being in the format specified
         by the class
 
         Returns
         -------
@@ -314,34 +324,43 @@
             matches_str = ", ".join(str(p) for p in matches)
             raise FormatMismatchError(
                 f"Multiple files with {exts} extensions found in : {matches_str}"
             )
         return matches[0]
 
     @classmethod
-    def matching_exts(cls, fspaths: ty.Set[Path], exts: ty.List[str]) -> ty.List[Path]:
+    def matching_exts(
+        cls, fspaths: ty.Set[Path], exts: ty.Optional[ty.List[str]] = None
+    ) -> ty.List[Path]:
         """Returns the paths out of the candidates provided that matches the
         given extension (by default the extension of the class)
 
         Parameters
         ----------
         fspaths: list[Path]
             The paths to select from
-        ext: list[str]
-            the extensions to match
+        ext: list[str], optional
+            the extensions to match, by default the primary and alternate extensions of
+            the class
 
         Returns
         -------
         list[Path]
             the matching paths
 
         Raises
         ------
         FileFormatError
             When no paths match or more than one path matches the given extension"""
+        if isinstance(fspaths, (str, Path)):
+            fspaths = [fspaths]
+        if exts is None:
+            if cls.ext is None:
+                return True
+            exts = cls.possible_exts
         return [
             p for p in fspaths if any(e is None or str(p).endswith(e) for e in exts)
         ]
 
     @classmethod
     def convert(cls, fileset, plugin="serial", task_name=None, **kwargs):
         """Convert a given file-set into the format specified by the class
@@ -772,18 +791,16 @@
             a file-set that will pass type-checking as an instance of the given
             fileset class but which doesn't actually point to any FS objects.
         """
         mock_cls = type(cls.__name__ + "Mock", (MockMixin, cls), {})
         if not fspaths:
             fspaths = []
             fspath = f"/mock/{cls.__name__.lower()}"
-            try:
+            if cls.ext:
                 fspath += cls.ext
-            except AttributeError:
-                pass
             fspaths.append(fspath)
         return mock_cls(fspaths=fspaths)
 
     @classmethod
     def sample(cls, dest_dir: ty.Optional[Path] = None) -> Self:
         """Return an sample instance of the file-set type for classes where the
         `test_data` extra has been implemented
@@ -799,18 +816,18 @@
             an instance of the given file-set class
         """
         if not dest_dir:
             dest_dir = Path(tempfile.mkdtemp())
         # Need to use mock to get an instance in order to use the singledispatch-based
         # mark.extra decorator
         mock = cls.mock()
-        return cls(mock.generate_test_data(dest_dir))
+        return cls(mock.generate_sample_data(dest_dir))
 
     @mark.extra
-    def generate_test_data(self, dest_dir: Path) -> ty.Iterable[Path]:
+    def generate_sample_data(self, dest_dir: Path) -> ty.Iterable[Path]:
         """Generate test data at the fspaths of the file-set
 
         Parameters
         ----------
         dest_dir : Path
             the directory to generate the test data within
```

### Comparing `fileformats-0.8.0/fileformats/core/mark.py` & `fileformats-0.8.1/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/mixin.py` & `fileformats-0.8.1/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/utils.py` & `fileformats-0.8.1/fileformats/core/utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/tests/test_classifiers.py` & `fileformats-0.8.1/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/tests/test_converter.py` & `fileformats-0.8.1/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/tests/test_detection.py` & `fileformats-0.8.1/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/tests/test_general.py` & `fileformats-0.8.1/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/tests/test_mime.py` & `fileformats-0.8.1/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/tests/test_mixin.py` & `fileformats-0.8.1/fileformats/core/tests/test_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,28 @@
     write_test_file(fspath, b"NOMAGIC some contents\n\n", binary=True)
     assert not FileWithMagicNumber.matches(fspath)
 
 
 class Header(File):
 
     ext = ".hdr"
+    binary = False
 
     def load(self):
         return dict(ln.split(":") for ln in self.contents.splitlines())
 
 
 class FileWithSeparateHeader(WithSeparateHeader, File):
 
     ext = ".img"
     header_type = Header
 
     image_type_key = "image-type"
     image_type = "sample-image-type"
+    binary = False
 
     @mark.check
     def check_image_type(self):
         if self.metadata[self.image_type_key] != self.image_type:
             raise FormatMismatchError(
                 f"Mismatch in '{self.image_type_key}', expected {self.image_type}, "
                 f"found {self.metadata[self.image_type_key]}"
```

### Comparing `fileformats-0.8.0/fileformats/core/tests/test_subpackages.py` & `fileformats-0.8.1/fileformats/core/tests/test_subpackages.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/core/tests/test_test_extras.py` & `fileformats-0.8.1/fileformats/core/tests/test_test_extras.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as ty
 from pathlib import Path
 from fileformats.core.fileset import FileSet, MockMixin
 from fileformats.testing import Foo
 
 
-@FileSet.generate_test_data.register
+@FileSet.generate_sample_data.register
 def generate_foo_data(file: Foo, dest_dir: Path) -> ty.List[Path]:
     foo_fspath = dest_dir / "test.foo"
     foo_fspath.write_text("foo")
     return [foo_fspath]
 
 
 def test_sample():
```

### Comparing `fileformats-0.8.0/fileformats/core/tests/test_utils.py` & `fileformats-0.8.1/fileformats/core/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from fileformats.core.mixin import WithSeparateHeader
 from fileformats.core.utils import (
     find_matching,
     MissingExtendedDependency,
 )
 from fileformats.core.exceptions import MissingExtendedDepenciesError, FileFormatsError
 import fileformats.text
-import fileformats.numeric
 from conftest import write_test_file
 
 
 class Bar(File):
     ext = ".bar"
 
 
@@ -288,15 +287,15 @@
     with open(text_file, "w") as f:
         f.write("sample text")
 
     detected = find_matching(text_file, standard_only=True)
     assert sorted(detected, key=lambda f: f.mime_like) == [
         fileformats.text.Prs_Fallenstein_Rst,
         fileformats.text.Prs_Prop_Logic,
-        fileformats.text.Unstructured,
+        fileformats.text.Txt,
     ]
 
 
 def test_missing_dependency():
     missing_dep = MissingExtendedDependency("missing_dep", "fileformats.image")
 
     with pytest.raises(MissingExtendedDepenciesError):
```

### Comparing `fileformats-0.8.0/fileformats/document/__init__.py` & `fileformats-0.8.1/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/field/__init__.py` & `fileformats-0.8.1/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/field/tests/test_fields.py` & `fileformats-0.8.1/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.8.1/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/generic/__init__.py` & `fileformats-0.8.1/fileformats/generic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,16 @@
         # file-sets as ones that have more constraints than simply existing
         return not (len(list(cls.required_properties())) - 1)
 
 
 class File(FsObject):
     """Generic file type"""
 
-    binary = False
+    binary = True
     is_dir = False
-    alternate_exts = ()
 
     @mark.required
     @property
     def fspath(self):
         fspath = self.select_by_ext()
         if fspath.is_dir():
             # fspath is guaranteed to exist
@@ -112,23 +111,14 @@
     def read_contents(self, size=None, offset=0):
         with open(self.fspath, "rb" if self.binary else "r") as f:
             if offset:
                 f.read(offset)
             contents = f.read(size)
         return contents
 
-    @classproperty
-    def possible_exts(cls):
-        possible = [cls.ext]
-        try:
-            possible.extend(cls.alternate_exts)
-        except AttributeError:
-            pass
-        return possible
-
     @property
     def actual_ext(self):
         "The actual file extension (out of the primary  and alternate extensions possible)"
         matching = [e for e in self.possible_exts if self.fspath.name.endswith(e)]
         if not matching:
             assert False, (
                 f"extension of fspath {self.fspath} is not in possible extensions for "
```

### Comparing `fileformats-0.8.0/fileformats/image/__init__.py` & `fileformats-0.8.1/fileformats/image/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/image/notclassifiedyet.py` & `fileformats-0.8.1/fileformats/image/notclassifiedyet.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/image/raster.py` & `fileformats-0.8.1/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/image/tests/test_image_raster.py` & `fileformats-0.8.1/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/misc/__init__.py` & `fileformats-0.8.1/fileformats/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/misc/unclassified.py` & `fileformats-0.8.1/fileformats/misc/unclassified.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/model/__init__.py` & `fileformats-0.8.1/fileformats/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/serialization/__init__.py` & `fileformats-0.8.1/fileformats/serialization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     # Classifiers class attrs
     classifiers_attr_name = "schema"
     schema = None
     multiple_classifiers = False
     allowed_classifiers = (Schema,)
     generically_qualifies = True
+    binary = False
 
     iana_mime = None
 
     @mark.extra
     def load(self):
         """Load the contents of the file into a dictionary"""
         raise NotImplementedError
```

### Comparing `fileformats-0.8.0/fileformats/testing/classifiers.py` & `fileformats-0.8.1/fileformats/testing/classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/fileformats/testing/headers.py` & `fileformats-0.8.1/fileformats/testing/headers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from fileformats.generic import File
 from fileformats.serialization import Json
 from fileformats.core.mixin import WithSideCars, WithSeparateHeader
 
 
 class Y(File):
     ext = ".y"
+    binary = False
 
 
 class Z(File):
     ext = ".z"
+    binary = False
 
 
 class Xyz(WithSideCars, File):
 
     ext = ".x"
+    binary = False
     side_car_types = (Y, Z)
 
 
 class MyFormat(File):
 
     ext = ".my"
+    binary = False
 
 
 class MyFormatGz(MyFormat):
 
     ext = ".my.gz"
 
 
@@ -31,31 +35,35 @@
 
     side_car_types = (Json,)
 
 
 class YourFormat(File):
 
     ext = ".yr"
+    binary = False
 
 
 class SeparateHeader(File):
 
     ext = ".hdr"
+    binary = False
 
 
 class ImageWithHeader(WithSeparateHeader, File):
 
     ext = ".img"
     header_type = SeparateHeader
+    binary = False
 
 
 class MyFormatGzX(MyFormatX, MyFormatGz):
 
     pass
 
 
 class EncodedText(File):
     """A text file where the characters ASCII codes are shifted on conversion
     from text
     """
 
     ext = ".enc"
+    binary = False
```

### Comparing `fileformats-0.8.0/fileformats/text/__init__.py` & `fileformats-0.8.1/fileformats/text/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,23 @@
     Xml,
     Yaml,
 )  # These are sometimes/historically considered part of the text registry so we import them here
 
 
 class Text(File):
     iana_mime = None
+    binary = False
 
 
 # General formats
 class Plain(Text):
     iana_mime = "text/plain"
 
 
-class Unstructured(Text):
+class Txt(Text):
     ext = ".txt"
 
 
 class Csv(Text):
     ext = ".csv"
     iana_mime = "text/csv"
```

### Comparing `fileformats-0.8.0/fileformats/video/__init__.py` & `fileformats-0.8.1/fileformats/video/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/LICENSE` & `fileformats-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.0/README.rst` & `fileformats-0.8.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -29,17 +29,28 @@
 formats that require inspection of headers to locate data files, directories containing
 certain file types, or to peek at metadata fields to define specific sub-types
 (e.g. functional MRI DICOM file set).
 
 See the `extension template <https://github.com/ArcanaFramework/fileformats-extension-template>`__
 for instructions on how to design *FileFormats* extensions modules to augment the
 standard file-types implemented in the main repository with custom domain/vendor-specific
-file-format types. Note that *FileFormats* is a new package, and only has limited support
-for standard formats at this stage, although the aim is to include all the official
-`IANA MIME types` (hopefully by scraping that site if anyone wants to have a go 😊).
+file-format types.
+
+Notes on MIME-type coverage
+---------------------------
+
+Support for all non-vendor standard MIME types (i.e. ones not matching ``*/vnd.*`` or ``*/x-*``) has been
+added to *FileFormats* by semi-automatically scraping the `IANA MIME types`_ website for file
+extensions and magic numbers. As such, many of the formats in the library have not been properly
+tested on real data and so should be treated with some caution. If you encounter any issues with an implemented file
+type, please raise an issue in the `GitHub tracker <https://github.com/ArcanaFramework/fileformats/issues>`__.
+
+Adding support for vendor formats will be relatively straightforward, it just requires someone to do the job
+of manually curating the scraped data (a days work or so). Please get in touch if you are interested in helping out
+with this.
 
 
 Installation
 ------------
 
 *FileFormats* can be installed for Python >= 3.7 from PyPI with
 
@@ -83,17 +94,18 @@
 for a boolean method that checks the validation use ``matches``
 
 .. code-block:: python
 
     if Png.matches(a_path_to_a_file):
         ... handle case ...
 
+Format Conversion
+-----------------
 
-There are a few selected converters between standard file-format types, perhaps most usefully
-between archive types and generic file/directories
+While not implemented in the main File-formats itself, file-formats provides hooks for other packages to implement extra behaviour such as format conversion. The `fileformats-extras <https://github.com/ArcanaFramework/fileformats-extras>`__ implements a number of converters between standard file-format types, e.g. archive types to/from generic file/directories, which if installed can be called using the `convert()` method.
 
 .. code-block:: python
 
     from fileformats.archive import Zip
     from fileformats.generic import Directory
 
     zip_file = Zip.convert(Directory("/path/to/a/directory"))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fileformats-0.8.0/pyproject.toml` & `fileformats-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dynamic = ["version"]
```

### Comparing `fileformats-0.8.0/PKG-INFO` & `fileformats-0.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.8.0
+Version: 0.8.1
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -102,15 +102,14 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: attrs>=22.1.0
@@ -169,17 +168,28 @@
 formats that require inspection of headers to locate data files, directories containing
 certain file types, or to peek at metadata fields to define specific sub-types
 (e.g. functional MRI DICOM file set).
 
 See the `extension template <https://github.com/ArcanaFramework/fileformats-extension-template>`__
 for instructions on how to design *FileFormats* extensions modules to augment the
 standard file-types implemented in the main repository with custom domain/vendor-specific
-file-format types. Note that *FileFormats* is a new package, and only has limited support
-for standard formats at this stage, although the aim is to include all the official
-`IANA MIME types` (hopefully by scraping that site if anyone wants to have a go 😊).
+file-format types.
+
+Notes on MIME-type coverage
+---------------------------
+
+Support for all non-vendor standard MIME types (i.e. ones not matching ``*/vnd.*`` or ``*/x-*``) has been
+added to *FileFormats* by semi-automatically scraping the `IANA MIME types`_ website for file
+extensions and magic numbers. As such, many of the formats in the library have not been properly
+tested on real data and so should be treated with some caution. If you encounter any issues with an implemented file
+type, please raise an issue in the `GitHub tracker <https://github.com/ArcanaFramework/fileformats/issues>`__.
+
+Adding support for vendor formats will be relatively straightforward, it just requires someone to do the job
+of manually curating the scraped data (a days work or so). Please get in touch if you are interested in helping out
+with this.
 
 
 Installation
 ------------
 
 *FileFormats* can be installed for Python >= 3.7 from PyPI with
 
@@ -223,17 +233,18 @@
 for a boolean method that checks the validation use ``matches``
 
 .. code-block:: python
 
     if Png.matches(a_path_to_a_file):
         ... handle case ...
 
+Format Conversion
+-----------------
 
-There are a few selected converters between standard file-format types, perhaps most usefully
-between archive types and generic file/directories
+While not implemented in the main File-formats itself, file-formats provides hooks for other packages to implement extra behaviour such as format conversion. The `fileformats-extras <https://github.com/ArcanaFramework/fileformats-extras>`__ implements a number of converters between standard file-format types, e.g. archive types to/from generic file/directories, which if installed can be called using the `convert()` method.
 
 .. code-block:: python
 
     from fileformats.archive import Zip
     from fileformats.generic import Directory
 
     zip_file = Zip.convert(Directory("/path/to/a/directory"))
```

