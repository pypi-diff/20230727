# Comparing `tmp/Tyf-1.4.3.tar.gz` & `tmp/Tyf-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Tyf-1.4.3.tar", last modified: Sun Dec 27 18:59:15 2020, max compression
+gzip compressed data, was "Tyf-1.5.0.tar", last modified: Thu Jul 27 16:54:39 2023, max compression
```

## Comparing `Tyf-1.4.3.tar` & `Tyf-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2020-12-27 18:59:15.051420 Tyf-1.4.3/
--rw-rw-rw-   0        0        0       17 2020-12-27 18:58:19.000000 Tyf-1.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9111 2020-12-27 18:59:14.972604 Tyf-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     6797 2020-12-22 16:30:11.000000 Tyf-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2020-12-27 18:59:14.770109 Tyf-1.4.3/Tyf/
--rw-rw-rw-   0        0        0    20322 2020-12-22 20:46:28.000000 Tyf-1.4.3/Tyf/__init__.py
--rw-rw-rw-   0        0        0     2033 2020-12-22 21:06:24.000000 Tyf-1.4.3/Tyf/decoders.py
--rw-rw-rw-   0        0        0     6320 2020-12-05 23:05:45.000000 Tyf-1.4.3/Tyf/encoders.py
--rw-rw-rw-   0        0        0     7477 2020-12-22 14:23:13.000000 Tyf-1.4.3/Tyf/gkd.py
--rw-rw-rw-   0        0        0    22362 2020-12-22 21:17:02.000000 Tyf-1.4.3/Tyf/ifd.py
--rw-rw-rw-   0        0        0    28646 2020-12-05 21:54:14.000000 Tyf-1.4.3/Tyf/tags.py
--rw-rw-rw-   0        0        0   295954 2020-12-05 22:49:05.000000 Tyf-1.4.3/Tyf/values.py
-drwxrwxrwx   0        0        0        0 2020-12-27 18:59:14.938695 Tyf-1.4.3/Tyf.egg-info/
--rw-rw-rw-   0        0        0     9111 2020-12-27 18:59:13.000000 Tyf-1.4.3/Tyf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2020-12-27 18:59:13.000000 Tyf-1.4.3/Tyf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-27 18:59:13.000000 Tyf-1.4.3/Tyf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2020-12-27 18:59:13.000000 Tyf-1.4.3/Tyf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        5 2020-12-05 10:43:07.000000 Tyf-1.4.3/VERSION
--rw-rw-rw-   0        0        0       42 2020-12-27 18:59:15.052390 Tyf-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1503 2020-12-27 18:58:19.000000 Tyf-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:54:39.912367 Tyf-1.5.0/
+-rw-rw-rw-   0        0        0       42 2023-07-26 20:11:53.000000 Tyf-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7907 2023-07-27 16:54:39.910372 Tyf-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6926 2023-07-27 15:37:47.000000 Tyf-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 16:54:39.890478 Tyf-1.5.0/Tyf/
+-rw-rw-rw-   0        0        0    23420 2023-07-27 15:45:46.000000 Tyf-1.5.0/Tyf/__init__.py
+-rw-rw-rw-   0        0        0     2112 2023-07-26 08:57:13.000000 Tyf-1.5.0/Tyf/decoders.py
+-rw-rw-rw-   0        0        0     6393 2023-07-26 11:03:24.000000 Tyf-1.5.0/Tyf/encoders.py
+-rw-rw-rw-   0        0        0     7764 2023-07-27 15:14:03.000000 Tyf-1.5.0/Tyf/gkd.py
+-rw-rw-rw-   0        0        0    23698 2023-07-27 15:31:15.000000 Tyf-1.5.0/Tyf/ifd.py
+-rw-rw-rw-   0        0        0     1324 2023-07-27 15:31:58.000000 Tyf-1.5.0/Tyf/tags.py
+-rw-rw-rw-   0        0        0    53248 2023-07-26 12:58:03.000000 Tyf-1.5.0/Tyf/tags.sqlite
+-rw-rw-rw-   0        0        0   295954 2020-12-05 22:49:05.000000 Tyf-1.5.0/Tyf/values.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:54:39.907380 Tyf-1.5.0/Tyf.egg-info/
+-rw-rw-rw-   0        0        0     7907 2023-07-27 16:54:39.000000 Tyf-1.5.0/Tyf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-27 16:54:39.000000 Tyf-1.5.0/Tyf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 16:54:39.000000 Tyf-1.5.0/Tyf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-27 16:54:39.000000 Tyf-1.5.0/Tyf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        5 2023-07-23 18:46:34.000000 Tyf-1.5.0/VERSION
+-rw-rw-rw-   0        0        0       42 2023-07-27 16:54:39.913363 Tyf-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1538 2020-12-28 19:47:26.000000 Tyf-1.5.0/setup.py
```

### Comparing `Tyf-1.4.3/README.md` & `Tyf-1.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,63 +5,81 @@
 ## Distribution
 [![pypi](https://img.shields.io/pypi/pyversions/Tyf.svg)](https://pypi.python.org/pypi/Tyf)
 [![pypi](https://img.shields.io/pypi/v/Tyf.svg)](https://pypi.python.org/pypi/Tyf)
 [![pypi](https://img.shields.io/badge/wheel-yes-brightgreen.svg)](https://pypi.python.org/pypi/Tyf)
 [![Downloads](https://pepy.tech/badge/Tyf/week)](https://pepy.tech/project/tyf)
 
 ## Support this project
+[![Liberapay receiving](https://img.shields.io/liberapay/goal/Toons?logo=liberapay)](https://liberapay.com/Toons/donate)
+
 [Buy &#1126;](https://bittrex.com/Account/Register?referralCode=NW5-DQO-QMT) and:
 
  + [X] Send &#1126; to `AUahWfkfr5J4tYakugRbfow7RWVTK35GPW`
- + [X] Vote `arky` on [Ark blockchain](https://explorer.ark.io) and [earn &#1126; weekly](http://arky-delegate.info/arky)
+ + [X] Vote `arky` on [Ark blockchain](https://explorer.ark.io) and [earn &#1126; weekly](http://dpos.arky-delegate.info/arky)
 
 ## Why this package ?
 Tyf package provides pythonic way to work with embeded data in TIFF and JPEG images.
 
 ## Documentation
 [The Tyf Project [WIP]](https://moustikitos.github.io/tyf/)
 
 ### Read / write EXIF and IFD data
  + read / edit EXIF data from JPEG images
  + read / edit IFD data from TIFF images
  + read / edit GEOTIFF data from IFD
- + read / edit XMP data from IFD
+ + read / edit XMP data from IFD and JPEG images
  + work directly with python numbers, string and datetime
  + interpolate map coordinates using GEOTIFF ModelTransformation
 
 ### Do more with JPEG and TIFF files
  + extract TIFF or JPEG thumbnails from JPEG files
- + strip EXIF data from JPEG File
  + dump EXIF data from JPEG into file
  + dump location thumbnail using any map provider API
 
 ## Quick view
 ```python
 >>> import Tyf
 >>> jpg = Tyf.open("test/IMG_20150730_210115.jpg")
 >>> jpg.__class__
 <class 'Tyf.JpegFile'>
 >>> print(Tyf.xmp.tostring(jpg.xmp).decode()) 
-<ns0:xmpmeta xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:ns0="adobe:ns:meta/" xmlns:ns3="http://ns.adobe.com/xap/1.0/" xmlns:ns4="http://ns.microsoft.com/photo/1.0/" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"><rdf:RDF><rdf:Description rdf:about="uuid:faf5bdd5-ba3d-11da-ad31-d33d75182f1b"><dc:title><rdf:Alt><rdf:li xml:lang="x-default">Beautifull Rainbow</rdf:li></rdf:Alt>
-  </dc:title><dc:description><rdf:Alt><rdf:li xml:lang="x-default">Beautifull Rainbow</rdf:li></rdf:Alt>
-  </dc:description><dc:creator><rdf:Seq><rdf:li>THOORENS Bruno</rdf:li></rdf:Seq>
-  </dc:creator><dc:rights><rdf:Alt><rdf:li xml:lang="x-default">THOORENS Bruno</rdf:li></rdf:Alt>
-  </dc:rights></rdf:Description><rdf:Description rdf:about="uuid:faf5bdd5-ba3d-11da-ad31-d33d75182f1b" /><rdf:Description rdf:about="uuid:faf5bdd5-ba3d-11da-ad31-d33d75182f1b"><ns3:Rating>4</ns3:Rating></rdf:Description><rdf:Description rdf:about="uuid:faf5bdd5-ba3d-11da-ad31-d33d75182f1b"><ns4:Rating>75</ns4:Rating><ns4:LastKeywordXMP><rdf:Bag><rdf:li>Rainbow</rdf:li><rdf:li>Belgium</rdf:li></rdf:Bag>
-  </ns4:LastKeywordXMP></rdf:Description><rdf:Description rdf:about="uuid:faf5bdd5-ba3d-11da-ad31-d33d75182f1b"><dc:subject><rdf:Bag><rdf:li>Rainbow</rdf:li><rdf:li>Belgium</rdf:li></rdf:Bag>
-  </dc:subject></rdf:Description></rdf:RDF></ns0:xmpmeta>
+<ns0:xmpmeta
+ xmlns:dc="http://purl.org/dc/elements/1.1/"
+ xmlns:ns0="adobe:ns:meta/" xmlns:ns3="http://ns.adobe.com/xap/1.0/"
+ xmlns:ns4="http://ns.microsoft.com/photo/1.0/"
+ xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"><rdf:RDF>
+<rdf:Description rdf:about="uuid:faf5bdd5-ba3d-11da-ad31-d33d75182f1b">
+<dc:title><rdf:Alt><rdf:li xml:lang="x-default">Beautifull Rainbow</rdf:li>
+</rdf:Alt></dc:title><dc:description><rdf:Alt>
+<rdf:li xml:lang="x-default">Beautifull Rainbow</rdf:li></rdf:Alt>
+</dc:description><dc:creator><rdf:Seq><rdf:li>THOORENS Bruno</rdf:li>
+</rdf:Seq></dc:creator><dc:rights><rdf:Alt>
+<rdf:li xml:lang="x-default">THOORENS Bruno</rdf:li></rdf:Alt></dc:rights>
+</rdf:Description>
+<rdf:Description rdf:about="uuid:faf5bdd5-ba3d-11da-ad31-d33d75182f1b" />
+<rdf:Description rdf:about="uuid:faf5bdd5-ba3d-11da-ad31-d33d75182f1b">
+<ns3:Rating>4</ns3:Rating></rdf:Description>
+<rdf:Description rdf:about="uuid:faf5bdd5-ba3d-11da-ad31-d33d75182f1b">
+<ns4:Rating>75</ns4:Rating><ns4:LastKeywordXMP><rdf:Bag>
+<rdf:li>Rainbow</rdf:li><rdf:li>Belgium</rdf:li></rdf:Bag>
+</ns4:LastKeywordXMP></rdf:Description>
+<rdf:Description rdf:about="uuid:faf5bdd5-ba3d-11da-ad31-d33d75182f1b">
+<dc:subject><rdf:Bag><rdf:li>Rainbow</rdf:li><rdf:li>Belgium</rdf:li></rdf:Bag>
+</dc:subject></rdf:Description>
+</rdf:RDF></ns0:xmpmeta>
 >>> jpg.save_thumbnail("test/test_thumb") # extension automatically added
 ```
 
 ![EXIF thumbnail](https://raw.githubusercontent.com/Moustikitos/tyf/master/test/test_thumb.jpg)
 
 There are 3 attributes to access data within `Tyf.JpegFile` :
 
- + ``ifd0`` containing picture IFD, EXIF and eventually GPS data 
- + ``ifd1`` containing thubnail data
- + ``xmp`` containing XMP data
++ ``ifd0`` containing picture IFD, EXIF and eventually GPS data 
++ ``ifd1`` containing thubnail data
++ ``xmp`` containing XMP data
 
 `ifd0` and `ifd1` are shortcut to the first and second IFD in `ifd` attribute which is itself a `Tyf.TiffFile`.
 
 ```python
 >>> jpg.ifd[0] == jpg.ifd0
 True
 >>> jpg.ifd[1] == jpg.ifd1
```

### Comparing `Tyf-1.4.3/Tyf/__init__.py` & `Tyf-1.5.0/Tyf/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- encoding:utf-8 -*-
 """
 # Bibliography
  + [Tiff 6.0 spec](https://www.itu.int/itudoc/itu-t/com16/tiff-fx/docs/tiff6.pdf)
  + [GeoTiFF 1.8.1 spec](https://htmlpreview.github.io/?https://github.com/OSGeo/libgeotiff/blob/master/geotiff/html/spec/geotiff2.6.html)
- + [JPEG FIF 1.02](https://www.w3.org/Graphics/JPEG/jfif3.pdf)
+ + [JPEG FIF 1.02 spec](https://www.w3.org/Graphics/JPEG/jfif3.pdf)
+ + [XMP spec](https://developer.adobe.com/xmp/docs/XMPSpecifications/)
 
 Tyf package aims to provide pythonic way to interact with metadata in TIFF and
 JPEG files.
 
 ```python
 >>> import Tyf
 ```
 """
 
-__copyright__ = """Copyright © 2015-2020 - BSD Licence"""
+__copyright__ = "Copyright © 2015-2023 - BSD Licence"
 __author__ = "THOORENS Bruno"
 __tiff__ = (6, 0)
 __geotiff__ = (1, 8, 1)
 
 import io
 import os
 import sys
@@ -25,14 +26,40 @@
 import operator
 
 import xml.etree.ElementTree as xmp
 
 __PY3__ = sys.version_info[0] >= 3
 __XMP__ = True
 
+#: Adobe namespaces mapping related to TIFF and JPEG File
+XmpNamespace = dict(
+    RDF="http://www.w3.org/1999/02/22-rdf-syntax-ns#",
+    TIFF="http://ns.adobe.com/tiff/1.0/",
+    ADOBE="http://ns.adobe.com/xap/1.0/",
+    PHOTOSHOP="http://ns.adobe.com/photoshop/1.0/",
+    EXIF="http://ns.adobe.com/exif/1.0/",
+    MICROSOFT="http://ns.microsoft.com/photo/1.0",
+    CAMERA_RAW_SETTINGS="http://ns.adobe.com/camera-raw-settings/1.0/",
+    IPTC="http://iptc.org/std/Iptc4xmpCore/1.0/xmlns/"
+)
+
+
+class InvalidFileError(Exception):
+    """
+    Raise when the input file is not valid, e.g. not a tiff or jpeg, or is a
+    bigtiff.
+    """
+    pass
+
+
+class XmpDataNotFound(Exception):
+    "Raise when no xmp data found in JPEG file"
+    pass
+
+
 #: Type definition linking tag type value to python `struct` format
 TYPES = {
     1:  ("B",  "UCHAR or USHORT"),
     2:  ("s",  "ASCII"),
     3:  ("H",  "UBYTE"),
     4:  ("L",  "ULONG"),
     5:  ("LL", "URATIONAL"),
@@ -54,56 +81,47 @@
 else:
     TYPES[2] = ("c", "ASCII")
     TYPES[7] = ("c", "UDEFINED")
     from cStringIO import StringIO
     reduce = __builtins__["reduce"]
 
 # here to avoid circular import
-from Tyf import ifd, gkd, tags
+from Tyf import ifd, gkd
 
 
 def unpack(fmt, fileobj):
     return struct.unpack(fmt, fileobj.read(struct.calcsize(fmt)))
 
 
 def pack(fmt, fileobj, value):
     return fileobj.write(struct.pack(fmt, *value))
 
 
-def _read_IFD(obj, fileobj, offset, byteorder="<", db=None):
+def _read_IFD(obj, fileobj, offset, byteorder="<"):
     "Read IFD from file object and return next IFD offset."
     # fileobj seek must be on the start offset
     fileobj.seek(offset)
     # get number of entry
     nb_entry, = unpack(byteorder+"H", fileobj)
     next_ifd_offset = offset + struct.calcsize("=H" + nb_entry*"HHLL")
     # for each entry
     for i in range(nb_entry):
-        obj.append(ifd.Tag.read(fileobj, byteorder, db=db))
+        obj.append(ifd.Tag.read(fileobj, byteorder))
     # return next ifd offset, if =0 then end of TIFF
     return next_ifd_offset
 
 
 def _from_buffer(obj, fileobj, offset, byteorder="<"):
     "Read IFD and sub IFD from file object and return next IFD offset."
     # read data from offset and get next ifd offset
     next_ifd_offset = _read_IFD(obj, fileobj, offset, byteorder)
     # read sub IFD if any
     for key in set(["GPS IFD", "Exif IFD", "Interoperability IFD"]) \
             & set(obj.keys()):
-        dic = getattr(
-            tags,
-            "gpsT" if "GPS" in key else
-            "exfT" if "Exif" in key else
-            "itrT"
-        )
-        _read_IFD(
-            obj, fileobj, obj[key], byteorder,
-            db=dict([(i[0], i[-1][0]) for i in dic.items()])
-        )
+        _read_IFD(obj, fileobj, obj[key], byteorder)
     fileobj.seek(next_ifd_offset)
     next_ifd, = unpack(byteorder+"L", fileobj)
     return next_ifd
 
 
 def _write_IFD(obj, fileobj, offset, byteorder="<", ifd1=None):
     "Write IFD in file object and return next ifd offset."
@@ -119,47 +137,44 @@
     ifds = obj.pack(byteorder)
     if isinstance(ifd1, ifd.Ifd):
         ifds.update(ifd1=ifd1.pack(byteorder)["root"])
 
     # compute exif, gps and interoperability offsets
     ifd_size = ifds["root"]["size"]
     ifd_values = ifds["root"]["data"]
-
     # where to put ifd values
     ifd_offset_values = offset + ifd_size
     # where to put the sub ifds
     sub_ifd_offset = ifd_offset_values + len(ifd_values)
 
     # compute all possible sub ifd offsets
-    for name in [n for n in ["exfT", "gpsT", "itrT"] if n in ifds]:
+    for name in set(["exfT", "gpsT", "itrT"]) & set(ifds.keys()):
         i = ifds[name]
-        tag = \
-            "Exif IFD" if name == "exfT" else \
-            "GPS IFD" if name == "gpsT" else \
+        obj[
+            "Exif IFD" if name == "exfT" else
+            "GPS IFD" if name == "gpsT" else
             "Interoperability IFD"
-        obj[tag] = sub_ifd_offset
+        ] = sub_ifd_offset
         # increment the next sub ifd offset
         sub_ifd_offset += i["size"] + len(i["data"])
 
     # if ifd1 given (thumbnail jor Jpeg), reserve needed space before raster
     # data
     if "ifd1" in ifds:
         raster_offset = \
             sub_ifd_offset + ifds["ifd1"]["size"] + \
             len(ifds["ifd1"]["data"]) + ifds["ifd1"]["raster"]
     # else raster data can follow the last sub ifd
     else:
         raster_offset = sub_ifd_offset
 
     # compute raster positions
-    for tag in [
-        t for t in
+    for tag in set(
         ["StripOffsets", "TileOffsets", "FreeOffsets", "JPEGInterchangeFormat"]
-        if t in dict.keys(obj)
-    ]:
+    ) & set(dict.keys(obj)):
         if "Offset" in tag:  # StripOffsets, TileOffsets or FreeOffsets
             raster_offsets = (raster_offset,)
             tagname = tag.replace("Offsets", "ByteCounts")
             bytecounts = obj[tagname]
             if isinstance(bytecounts, tuple):
                 for bytecount in obj[tagname]:
                     raster_offsets += (raster_offsets[-1] + bytecount, )
@@ -171,56 +186,52 @@
     ifds = obj.pack(byteorder)
     if isinstance(ifd1, ifd.Ifd):
         ifds.update(ifd1=ifd1.pack(byteorder)["root"])
     # adjust raser offset with diff between first computation and second one
     raster_offset += len(ifds["root"]["data"]) - len(ifd_values)
 
     # write IFDs
-    for key in [
-        k for k in ["root", "exfT", "gpsT", "itrT"]
-        if k in ifds
-    ]:
+    for key in set(["root", "exfT", "gpsT", "itrT"]) & set(ifds.keys()):
         packed = ifds[key]
         # go to according [SUB]IFD offset and determine associated data offset
         if key == "root":
             fileobj.seek(offset)
             data_offset = ifd_offset_values
         else:
             sub_ifd_offset = obj[
                 "Exif IFD" if key == "exfT" else
                 "GPS IFD" if key == "gpsT" else
                 "Interoperability IFD"
             ]
             fileobj.seek(sub_ifd_offset)
-            data_offset = \
-                sub_ifd_offset + packed["size"]
+            data_offset = sub_ifd_offset + packed["size"]
 
         tags = packed["tags"]
         # write number of entries
-        pack(byteorder+"H", fileobj, (len(tags),))
+        pack(byteorder + "H", fileobj, (len(tags),))
         # write all ifd entries and data
         for entry, data, is_offset in tags:
             fileobj.write(entry)
             if not is_offset:
                 fileobj.write(data)
             else:
                 # put offset and shift it by len(data) for next offset value
-                pack(byteorder+"L", fileobj, (data_offset, ))
+                pack(byteorder + "L", fileobj, (data_offset, ))
                 data_offset += len(data)
 
         if key == "root":
             next_ifd_offset = fileobj.tell()
-        pack(byteorder+"L", fileobj, (0, ))
+        pack(byteorder + "L", fileobj, (0, ))
         fileobj.write(packed["data"])
 
     # write IFD1 (this should only be used with Jpeg exif thumbnail)
     if "ifd1" in ifds:
         ifd1_offset = fileobj.tell()
         fileobj.seek(next_ifd_offset)
-        pack(byteorder+"L", fileobj, (ifd1_offset, ))
+        pack(byteorder + "L", fileobj, (ifd1_offset, ))
         _write_IFD(ifd1, fileobj, ifd1_offset, byteorder="<", ifd1=None)
 
     # write raster data
     if obj.raster_loaded:
         fileobj.seek(raster_offset)
         if hasattr(obj, "jpegIF"):
             fileobj.write(getattr(obj, "jpegIF"))
@@ -233,61 +244,62 @@
             ):
                 fileobj.write(data)
 
     return next_ifd_offset
 
 
 def _fileobj(f, mode):
+    #: returns fileobj from a path or a stringIO
     if hasattr(f, "close"):
         fileobj = f
         _close = False
     else:
         fileobj = io.open(f, mode)
         _close = True
     return fileobj, _close
 
 
 def open(f):
     """
-    Return JpegFile or TiffFile according to `f`. If it is a file object,
-    it is not closed.
+    Return `JpegFile` or `TiffFile` instance according to argument.
+
+    Args:
+        f (buffer or string): a valid file path or a python file object.
 
-    Arguments:
-        f (buffer or string): a valid file path or a python file object
+    Returns:
+        Tyf.JpegFile|Tyf.TiffFile: JPEG or TIFF instance.
     """
     fileobj, _close = _fileobj(f, "rb")
 
     first, = unpack(">H", fileobj)
     fileobj.seek(0)
 
     if first == 0xffd8:
         obj = JpegFile(fileobj)
     elif first in [0x4d4d, 0x4949]:
         obj = TiffFile(fileobj)
+    else:
+        obj = None
 
     if _close:
         fileobj.close()
 
-    try:
+    if obj is None:
+        raise InvalidFileError("file is not a valid JPEG nor TIFF image")
+    else:
         return obj
-    except Exception:
-        raise Exception("file is not a valid JPEG nor TIFF image")
-
-
-def getGeokeyDirectories(cls):
-    if not hasattr(cls, "_geokey_directories"):
-        setattr(cls, "_geokey_directories", [
-            gkd.Gkd.from_ifd(ifd) for ifd in cls
-        ])
-    return getattr(cls, "_geokey_directories")
 
 
 class TiffFile(list):
     """
-    List of IFD found in TIFF file.
+    This class is is a list of all Image File Directories defining the TIFF
+    file.
+
+    Args:
+        fileobj (buffer): a python file object.
 
     ```python
     >>> tif = Tyf.open("test/CEA.tif")
     >>> tif[0]["BitsPerSample"]
     <IFD tag BitsPerSample:8>
     >>> tif[0]["ModelTiepointTag"].value
     (0.0, 0.0, 0.0, -28493.166784412522, 4255884.5438021915, 0.0)
@@ -297,15 +309,15 @@
     >>> tr(tif[0]["ImageWidth"], tif[0]["ImageLength"])
     (2358.211624949061, 4224973.143255847, 0.0, 1.0)
     ```
     """
 
     #: shortcut to geokey directories
     gkd = property(
-        lambda obj: getGeokeyDirectories(obj),
+        lambda obj: gkd.getGeokeyDirectories(obj),
         None, None, "Geotiff IFD"
     )
 
     #: `True` if raster data loaded
     raster_loaded = property(
         lambda obj: reduce(
             operator.__and__, [ifd.raster_loaded for ifd in obj]
@@ -318,22 +330,24 @@
         first, = unpack(">H", fileobj)
         byteorder = "<" if first == 0x4949 else ">"
         # manage according to magic number found
         magic_number, = unpack(byteorder+"H", fileobj)
         if magic_number not in [0x732E, 0x2A]:  # 29486, 42
             fileobj.close()
             if magic_number == 0x2B:  # 43
-                raise IOError("BigTIFF file not supported")
+                raise InvalidFileError("BigTIFF file not supported")
             else:
-                raise IOError("Bad magic number. Not a valid TIFF file")
+                raise InvalidFileError(
+                    "Bad magic number. Not a valid TIFF file"
+                )
 
         ifds = []
         next_ifd, = unpack(byteorder+"L", fileobj)
         while next_ifd != 0:
-            i = ifd.Ifd(tag_family=[tags.bTT, tags.pTT, tags.xTT])
+            i = ifd.Ifd(tag_family=["bTT", "pTT", "xTT"])
             next_ifd = _from_buffer(i, fileobj, next_ifd, byteorder)
             ifds.append(i)
 
         # keep filename source to load raster when needed
         if hasattr(fileobj, "name"):
             self._filename = fileobj.name
         # load raster if initializing from fileobj
@@ -349,23 +363,22 @@
             for item in iter(self) if idx is None else [self[idx]]:
                 if not item.raster_loaded:
                     ifd._load_raster(item, in_)
             in_.close()
 
     def save(self, f, byteorder="<", idx=None, ifd1=None):
         """
-        Save object as a TIFF file. If `f` is a file object, it is not
-        closed.
+        Save object into a TIFF file.
 
         Arguments:
-            f (buffer or string): a valid file path or a python file object
+            f (buffer|string): a valid file path or a python file object
             byteorder (string): `">"` if big-endian used else `"<"`
             idx (int): IFD index to save
             ifd1 (Tyf.ifd.Ifd): IFD to be used as thumbnail (only needed with
-                                JPEG saving)
+                JPEG saving)
         """
         self.load_raster()
         fileobj, _close = _fileobj(f, "wb")
 
         pack(
             byteorder+"HH", fileobj,
             (0x4949 if byteorder == "<" else 0x4d4d, 0x2A, )
@@ -380,18 +393,21 @@
             fileobj.close()
             del fileobj
 
 
 class JpegFile(list):
     """
     List of JPEG segment tuple (marker, segment) defining the JPEG file. Tyf
-    manage to extract xmd data as python `ElementTree` object and EXIF data
+    manage to extract xmp data as python `ElementTree` object and EXIF data
     as IFD. `ifd0` is a shortcut to JPEF Exif, `ifd1` is a shortcut to JPEG
     Thumbnail and `xmp` is a shortcut to XMP data.
 
+    Args:
+        fileobj (buffer): a python file object.
+
     ```python
     >>> jpg = Tyf.open("test/IMG_20150730_210115.jpg")
     >>> jpg.ifd0["GPS IFD"]
     <IFD tag GPS IFD:794>
     >>> jpg.ifd0.get_location()
     (5.1872093, 51.2095416, 0.0)
     >>> jpg.xmp
@@ -407,43 +423,50 @@
 
     #: shortcut to JPEG thumbnail
     ifd1 = property(
         lambda obj: getattr(obj, "ifd", [{}, {}])[1],
         None, None, "readonly thumbnail IFD attribute"
     )
 
+    @property
+    def xmp(obj):
+        "readonly XMP attribute"
+        if not hasattr(obj, "_JpegFile__xmp_ns"):
+            raise XmpDataNotFound("no XMP segment found")
+        return list.__getitem__(obj, obj.__xmp_idx)[-1]
+
     def __init__(self, fileobj):
-        """
-        Arguments:
-            fileobj: a python file object
-        """
         sgmt = []
 
         fileobj.seek(0)
         marker, = unpack(">H", fileobj)
         if marker != 0xffd8:
-            raise Exception("not a valid jpeg file")
+            raise InvalidFileError("not a valid jpeg file")
 
         while marker != 0xffd9:  # EOI (End Of Image) Marker
             marker, count = unpack(">HH", fileobj)
             # if JPEG raw data
             if marker == 0xffda:
                 fileobj.seek(-2, 1)
                 sgmt.append((0xffda, fileobj.read()[:-2]))
                 marker = 0xffd9
             elif marker == 0xffe1:
                 data = fileobj.read(count-2)
                 if data[:6] == b"Exif\x00\x00":
                     string = StringIO(data[6:])
                     self.ifd = TiffFile(string)
                     string.close()
-                    sgmt.append((0xffe1, self.ifd))
+                    sgmt.append((marker, self.ifd))
                 elif b"ns.adobe.com" in data[:30]:
-                    self.xmp = xmp.fromstring(data[data.find(b"\x00")+1:])
-                    sgmt.append((0xffe1, self.xmp))
+                    xmp_data_idx = data.find(b"\x00")
+                    self.__xmp_idx = len(sgmt)
+                    self.__xmp_ns = data[:xmp_data_idx]
+                    sgmt.append(
+                        (marker, xmp.fromstring(data[xmp_data_idx+1:]))
+                    )
             else:
                 sgmt.append((marker, fileobj.read(count-2)))
 
         list.__init__(self, sgmt)
 
     def __getitem__(self, item):
         """
@@ -463,19 +486,69 @@
         ```python
         >>> jpg.get("ImageWidth")
         <IFD tag ImageWidth:320>
         ```
         """
         return self.ifd1.get(item, default)
 
+    def set_xmp(self, tag, value, **attributes):
+        """
+        Set xmp tag value. Custom namespace can be used.
+
+        Args:
+            tag (str): tag.
+            value (str): tag value.
+            **attributes: all elements to be set using `attributes` arg on
+                `xml.etree.ElementTree.Element` creation.
+
+        Returns:
+            xml.etree.ElementTree.Element: tag element.
+        """
+        # create the xmp segment if no one found
+        if not hasattr(self, "_JpegFile__xmp_ns"):
+            self.__xmp_ns = b"http://ns.adobe.com/xap/1.0/"
+            self.__xmp_idx = 2
+            elem = xmp.Element("{adobe:ns:meta/}xmpmeta")
+            xmp.SubElement(elem, "{%s}RDF" % XmpNamespace["RDF"])
+            list.insert(self, self.__xmp_idx, (65505, elem))
+        # get namespace
+        ns = attributes.pop("ns", "http://ns.adobe.com/exif/1.0/")
+        ns = XmpNamespace.get(ns, ns)
+        # try to get a parent node containing at least one tag with the
+        # according namespace
+        parent = self.xmp.find(".//{%s}*/..." % ns)
+        if parent is None:
+            # create a 'Description' node in root element with rdf namespace
+            parent = xmp.SubElement(
+                self.xmp[0], "{%s}Description" % XmpNamespace["RDF"]
+            )
+        # add element with the appropriate namespace
+        elem = xmp.SubElement(parent, "{%s}%s" % (ns, tag), **attributes)
+        elem.text = "%s" % value
+        parent.append(elem)
+        return elem
+
+    def get_xmp(self, tag, ns="http://ns.adobe.com/exif/1.0/"):
+        """
+        Get xmp tag value. Custom namespace can be used.
+
+        Args:
+            tag (str): tag name.
+            ns (url): xml namespace url (default to
+                http://ns.adobe.com/exif/1.0/).
+
+        Returns:
+            xml.etree.ElementTree.Element: tag element.
+        """
+        return self.xmp.find(".//{%s}%s" % (XmpNamespace.get(ns, ns), tag))
+
     def save(self, f):
         """
         Save object as a JPEG file. All segmet are writed in current order,
-        only `ifd0`, `ifd1` and `xmp` are recomputed. If `f` is a file
-        object, it is not closed.
+        only `ifd0`, `ifd1` and `xmp` are recomputed.
 
         Arguments:
             f (buffer or string): a valid file path or a python file object
         """
         fileobj, _close = _fileobj(f, "wb")
         pack(">H", fileobj, (0xffd8,))
 
@@ -494,15 +567,15 @@
                     value = b"Exif\x00\x00" + (
                         data if isinstance(data, bytes)
                         else data.encode("utf-8")
                     )
                     string.close()
                 elif isinstance(value, xmp.Element):
                     data = xmp.tostring(self.xmp)
-                    value = b"http://ns.adobe.com/xap/1.0/\x00" + (
+                    value = self.__xmp_ns + b"\x00" + (
                         data if isinstance(data, bytes)
                         else data.encode("utf-8")
                     )
                 else:
                     value = b""
                 pack(">HH", fileobj, (marker, len(value) + 2))
 
@@ -516,15 +589,15 @@
         if _close:
             fileobj.close()
             del fileobj
 
     def save_thumbnail(self, f):
         """
         Save JPEG thumbnail in a separated TIFF or JPEG file, file extention
-        automatically appended. If `f` is a file object, it is not closed.
+        automatically appended.
 
         Arguments:
             f (buffer or string): a valid file path or a python file object
         """
         try:
             ifd = self.ifd1
         except Exception as error:
@@ -561,76 +634,81 @@
         """
         fileobj, _close = _fileobj(f, "wb")
         self.ifd.save(fileobj)
         if _close:
             fileobj.close()
             del fileobj
 
-    def strip_exif(self):
-        """
-        Remove EXIF from JPEG, keeping XMP segment untouched.
-        """
-        ifd = self.ifd
-        ifd0 = self.ifd0
-        while len(ifd) > 1:
-            ifd.pop(-1)
-        for key in list(k for k in dict.__iter__(ifd0) if k not in tags.bTT):
-            ifd0.pop(key)
-
 
 # if PIL exists do some overridings
 try:
     from PIL import Image as _Image
 except ImportError:
     pass
 else:
+
+    def _getmeta(im):
+        for _, data in im.applist:
+            if data[:6] == b'Exif\x00\x00':
+                fileobj = io.BytesIO(data[6:])
+                setattr(im, "ifd", TiffFile(fileobj))
+                fileobj.close()
+            elif data[:29] == b'http://ns.adobe.com/xap/1.0/\x00':
+                setattr(im, "xmp", xmp.fromstring(data[29:]))
+
     def _getexif(im):
-        try:
-            data = im.info["exif"]
-        except KeyError:
-            return None
-        # b'Exif\x00\x00' -> 6 bytes
-        fileobj = io.BytesIO(data[6:])
-        exif = TiffFile(fileobj)
-        fileobj.close()
-        del fileobj
-        return exif
+        if not hasattr(im, "ifd"):
+            try:
+                data = im.info["exif"]
+            except KeyError:
+                return None
+            # b'Exif\x00\x00' -> 6 bytes
+            fileobj = io.BytesIO(data[6:])
+            setattr(im, "ifd", TiffFile(fileobj))
+            fileobj.close()
+            del fileobj
+        return im.ifd
 
     class Image(_Image.Image):
         """
         Pillow Image class override.
         """
 
         # keep a reference of original PIL Image object
         _image_ = _Image.Image
 
         @staticmethod
         def open(*args, **kwargs):
-            return _Image.open(*args, **kwargs)
+            img = _Image.open(*args, **kwargs)
+            img._getmeta()
+            return img
 
         def save(self, fp, format=None, **params):
             if (
                 isinstance(fp, str) and
                 os.path.splitext(fp)[-1].lower() in [".jpg", ".jpeg"]
                 or
                 isinstance(format, str) and
                 format.lower() == "jpeg"
             ) and not params.pop("strip_exif", False):
+                self._getexif()
                 stringio = StringIO()
-                ifd = self._getexif()
-                ifd.save(stringio, idx=0, ifd1=ifd[1])
+                self.ifd.save(stringio, idx=0, ifd1=self.ifd[1])
                 data = stringio.getvalue()
                 params["exif"] = b'Exif\x00\x00' + (
                     data if isinstance(data, bytes) else
                     data.encode("utf-8")
                 )
                 stringio.close()
                 del stringio, data
+            if hasattr(self, "xmp"):
+                params["xmp"] = b'http://ns.adobe.com/xap/1.0/\x00' + \
+                    xmp.tostring(self.xmp)
             return Image._image_.save(self, fp, format, **params)
 
     #: Pillow override
     _Image.Image = Image
 
     from PIL import JpegImagePlugin
-    JpegImagePlugin._getexif_ = JpegImagePlugin._getexif
     JpegImagePlugin._getexif = _getexif
-    del _getexif
+    JpegImagePlugin.JpegImageFile._getmeta = _getmeta
+    del _getexif, _getmeta
```

### Comparing `Tyf-1.4.3/Tyf/decoders.py` & `Tyf-1.5.0/Tyf/decoders.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,7 +111,13 @@
 def GPSTimeStamp(value):
     return datetime.time(*[int(e) for e in _5(value)])
 
 
 def GPSDateStamp(value):
     dt = datetime.datetime.strptime(_2(value), "%Y:%m:%d")
     return datetime.date(dt.year, dt.month, dt.day)
+
+
+# XMP tag
+
+def XMP(value):
+    return bytearray(value).decode("utf-8")
```

### Comparing `Tyf-1.4.3/Tyf/encoders.py` & `Tyf-1.5.0/Tyf/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,7 +253,11 @@
 def GPSDateStamp(value):
     try:
         return _2(value.strftime("%Y:%m:%d"))
     except Exception:
         raise EncodingException(
             "%s is not a valide time object" % (value, )
         )
+
+
+def XMP(value):
+    return tuple(bytearray(value.encode("utf-8")))
```

### Comparing `Tyf-1.4.3/Tyf/gkd.py` & `Tyf-1.5.0/Tyf/gkd.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,24 +58,30 @@
     4099: ("VerticalUnitsGeoKey", [3], None, None),
 }
 
 _2TAG = dict((v[0], t) for t, v in _TAGS.items())
 _2KEY = dict((v, k) for k, v in _2TAG.items())
 
 
+def getGeokeyDirectories(cls):
+    #: create _geokey_directories or return it
+    if not hasattr(cls, "_geokey_directories"):
+        setattr(cls, "_geokey_directories", [
+            Gkd.from_ifd(ifd) for ifd in cls
+        ])
+    return getattr(cls, "_geokey_directories")
+
+
 class GkdTag:
     strict = True
-
     info = property(
         lambda cls: getattr(
             values, _2KEY.get(cls.tag, cls.key), {}
         ).get(cls._decode(), None),
-        None,
-        None,
-        ""
+        None, None, ""
     )
 
     def __init__(self, tag, value=None):
         self.key, types, default, self.comment = _TAGS.get(
             tag, ("Unknown", [0], None, "Undefined tag")
         )
         value = default if value is None else value
@@ -182,7 +188,8 @@
                 t.count = count
                 dict.__setitem__(cls, tag, t)
         return cls
 
     def tags(self):
         for v in sorted(dict.values(self), key=lambda e: e.tag):
             yield v
+    __iter__ = tags
```

### Comparing `Tyf-1.4.3/Tyf/ifd.py` & `Tyf-1.5.0/Tyf/ifd.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 import collections
 
 from Tyf import TYPES, reduce
 from Tyf import tags, encoders, decoders, values
 
 try:
     from urllib.request import urlopen
-    from io import BytesIO as StringIO
 except ImportError:
     from urllib import urlopen
-    from cStringIO import StringIO
 
 
 #: Mapping of named tuple to be used with geotiff `ModelPixelScaleTag`,
 #: `ModelTiepointTag` and `ModelTransformationTag`.
 #: ```python
 #: >>> import tyf
 #: >>> from Tyf import ifd
@@ -54,40 +52,44 @@
     ...     0., 0.,  Sz, Z - K * Sz,
     ...     0., 0.,  0., 1.
     ... )
     >>> ifd.Transform(matrix, 10, 10)
     (-27892.945414580587, 4255284.32243236, 0.0)
     ```
 
-    Arguments:
-        obj (GeoKeyModel["ModelTransformationTag"]): transformation matrix
-        x (float): pixel column index from left
-        y (float): pixel row index from top
-        z (float): altitude value
+    Args:
+        obj (GeoKeyModel["ModelTransformationTag"]): transformation matrix.
+        x (float): pixel column index from left.
+        y (float): pixel row index from top.
+        z (float): altitude value.
+
     Returns:
-        projeted coordinates X, Y, Z
+        tuple: projeted coordinates X, Y, Z.
     """
     return (
         obj[0] * x + obj[1] * y + obj[2] * z + obj[3] * 1.,
         obj[4] * x + obj[5] * y + obj[6] * z + obj[7] * 1.,
         obj[8] * x + obj[9] * y + obj[10] * z + obj[11] * 1.
     )
 
 
 class Tag(object):
-    #: Encode and decode on the fly the `_v` attribute (see `Tyf.encoders` and
-    #: `Tyf.decoders` modules).
-    #: ```python
-    #: >>> tag = ifd.Tag("GPSLongitude")
-    #: >>> tag.value = 5.62347
-    #: >>> tag._v
-    #: (5, 1, 37, 1, 6123, 250)  # 5/1 deg + 37/1 min + 6123/250 sec
-    #: >>> tag.value
-    #: 5.62347
-    #: ```
+    """
+    Encode and decode on the fly the `_v` attribute (see `Tyf.encoders` and
+    `Tyf.decoders` modules).
+
+    ```python
+    >>> tag = ifd.Tag("GPSLongitude")
+    >>> tag.value = 5.62347
+    >>> tag._v
+    (5, 1, 37, 1, 6123, 250)  # 5/1 deg + 37/1 min + 6123/250 sec
+    >>> tag.value
+    5.62347
+    ```
+    """
     value = property(
         lambda cls: cls._getvalue(),
         lambda cls, v: cls._setvalue(v),
         None,
         ""
     )
     count = property(
@@ -137,52 +139,50 @@
         self._v = self._encode(value)
         self._is_offset = self.count * struct.calcsize(
             "=" + TYPES[self.type][0]
         ) > 4
 
     def __init__(self, tag_or_key, value=None):
         """
-        Arguments:
-            tag_or_key (int or string): tag value or keyword
+        Args:
+            tag_or_key (int or string): tag value or keyword.
             value (any): value of the tag. If `None` is given, it is set to
-                         default value if anyone is defined else `_v` attribute
-                         is not created.
+                default value if anyone is defined.
         """
         self.tag, (self.key, self._types, default, self.comment) = \
             tags.get(tag_or_key)
         self.type = self._types[-1]
         if value or default:
             self.value = value or default
 
     def __repr__(self):
         if self.info:
             return "<IFD tag %s:%r - %s>" % (self.key, self.value, self.info)
         else:
             return "<IFD tag %s:%r>" % (self.key, self.value)
 
     @staticmethod
-    def read(fileobj, byteorder, db=None):
+    def read(fileobj, byteorder):
         """
         Extract an IFD tag from buffer current position. Buffer position is
         adjusted to the end of IFD entry before returning the value.
 
-        Arguments:
-            fileobj (buffer): a python file object
-            byteorder (string): `">"` if big-endian used else `"<"`
-            db (dict): authorized tag database
+        Args:
+            fileobj (buffer): a python file object.
+            byteorder (string): `">"` if big-endian used else `"<"`.
+
         Returns:
-            `Tyf.ifd.Tag`
+            `Tyf.ifd.Tag`: tag instance.
         """
         # read tag, type and count
         fmt = byteorder + "HHL"
         tag, typ, cnt = struct.unpack(
             fmt, fileobj.read(struct.calcsize(fmt))
         )
         cls = Tag(tag)
-        cls.key, cls._types, cls.default, cls.comment = tags.get(tag)[-1]
         cls.type = typ
         # extract value_or_offset
         value_or_offset = fileobj.read(struct.calcsize("=L"))
         if not isinstance(value_or_offset, bytes):
             value_or_offset = value_or_offset.encode("utf-8")
         # prepare structure value
         _typ = TYPES[typ][0]
@@ -206,14 +206,16 @@
             # python 3.x
             if len(value) == 1:
                 value = value[0]
             # python 2.x
             else:
                 value = b"".join(value)
         cls._v = value
+        if cls.tag is False:
+            print(f"unknown tag {tag} type {cls._types}: {cls} ignored")
         return cls
 
     def calcsize(self):
         """
         Return tag value size in `bytes` when packed.
         """
         return struct.calcsize("=" + TYPES[self.type][0] * self.count)
@@ -232,18 +234,19 @@
         '00000005000000010000002500000001000017eb000000fa'
         >>> #   5,      1,     37,      1,   6123,    250
         >>> # 5/1 deg   + 37/1 min         + 6123/250 sec
         >>> ofs
         True
         ```
 
-        Arguments:
-            byteorder (string): `">"` if big-endian used else `"<"`
+        Args:
+            byteorder (string): `">"` if big-endian used else `"<"`.
+
         Returns:
-            (packed ifd entry - packed value - is offset boolean)
+            tuple: packed ifd entry, packed value, is offset boolean
         """
         tag, typ, cnt = self.tag, self.type, self.count
         info = struct.pack(byteorder + "HHL", tag, typ, cnt)
         typ_ = TYPES[typ][0]
         fmt = \
             byteorder + ("%ds" % cnt if typ_ == "s" else cnt * typ_)
         packed = \
@@ -299,29 +302,24 @@
     if "JPEGInterchangeFormat" in obj:
         fileobj.seek(obj["JPEGInterchangeFormat"])
         obj.jpegIF = fileobj.read(obj["JPEGInterchangeFormatLength"])
 
 
 def getModelTiePoints(cls):
     """
-    Return tiepoint list found in `ModelTiepointTag` tags. This function sets
-    a list of all points in private attribute `_model_tiepoints` on first
-    call.
+    Return tiepoint list found in `ModelTiepointTag` tags.
 
-    ```
-    ModelTiepointTag = (I1, J1, K1, X1, Y1, Z1, ...In, Jn, Kn, Xn, Yn, Zn)
-    _model_tiepoints = [(I1, J1, K1, X1, Y1, Z1), ...(In, Jn, Kn, Xn, Yn, Zn)]
-    ```
+    Args:
+        cls (dict or Tyf.ifd.Ifd): image file directory.
 
-    Arguments:
-        cls (dict or Tyf.ifd.Ifd): image file directory
     Returns:
-        Tiepoint `list`
+        list: Tiepoint.
+
     Raises:
-        KeyError if no `ModelTiepointTag` defined
+        KeyError: if no `ModelTiepointTag` defined.
     """
     if not hasattr(cls, "_model_tiepoints"):
         setattr(cls, "_model_tiepoints", [
             cls["ModelTiepointTag"][i:i+6]
             for i in range(0, len(cls["ModelTiepointTag"]), 6)
         ])
     return getattr(cls, "_model_tiepoints")
@@ -366,15 +364,15 @@
         lambda cls: getModelTiePoints(cls),
         None, None, ""
     )
 
     def __init__(self, **kwargs):
         dict.__init__(self)
         self.tag_family = kwargs.pop(
-            "tag_family", [tags.bTT, tags.xTT, tags.pTT]
+            "tag_family", ["bTT", "xTT", "pTT"]
         )
 
     def __delattr__(self, attr):
         if attr == "gpsT":
             dict.pop(self, "GPS IFD", False)
         elif attr == "exfT":
             dict.pop(self, "Exif IFD", False)
@@ -440,23 +438,22 @@
                     result = dict.pop(dic, key)
                     if len(dic) == 0:
                         delattr(self, name)
                     return result
         return default
 
     def append(self, tag):
-        for dic in self.tag_family:
-            if tag.tag in dic:
+        for family in self.tag_family:
+            if tags.in_family(tag.key, family):
                 return dict.__setitem__(self, tag.key, tag)
-        for name in ["exfT", "gpsT", "itrT"]:
-            dic = getattr(tags, "_" + name, {})
-            if tag.key in dic:
-                if not hasattr(self, name):
-                    setattr(self, name, Ifd(tag_family=[getattr(tags, name)]))
-                return dict.__setitem__(getattr(self, name), tag.key, tag)
+        for family in ["exfT", "gpsT", "itrT"]:
+            if tags.in_family(tag.key, family):
+                if not hasattr(self, family):
+                    setattr(self, family, Ifd(tag_family=[family]))
+                return dict.__setitem__(getattr(self, family), tag.key, tag)
 
     def tags(self):
         """
         Return iterator over all IFD values including sub IFD ones in the
         order: `exfT` - `gpsT` - `itrT`.
         """
         for v in sorted(dict.values(self), key=lambda e: e.tag):
@@ -519,21 +516,21 @@
         <IFD tag GPSLatitude:45.21345>
         <IFD tag GPSLongitudeRef:'E'>
         <IFD tag GPSLongitude:5.62347>
         <IFD tag GPSAltitudeRef:0 - Above sea level>
         <IFD tag GPSAltitude:12.0>
         ```
 
-        Arguments:
+        Args:
             lon (float): longitude in decimal degrees
             lat (float): latitude in decimal degrees
             alt (float): altitude in meters
         """
         if not hasattr(self, "gpsT"):
-            setattr(self, "gpsT", Ifd(tag_family=[tags.gpsT]))
+            setattr(self, "gpsT", Ifd(tag_family=["gpsT"]))
         if "GPSVersionID" not in self:
             dict.__setitem__(self.gpsT, "GPSVersionID", Tag("GPSVersionID"))
         self["GPSLatitudeRef"] = "n" if lat >= 0 else "s"
         self["GPSLatitude"] = lat
         self["GPSLongitudeRef"] = "e" if lon >= 0 else "w"
         self["GPSLongitude"] = lon
         self["GPSAltitudeRef"] = alt >= 0
@@ -551,17 +548,18 @@
         Exception: No location data found
         >>> i.set_location(5.62347, 45.21345, 12)
         >>> i.get_location()
         (5.62347, 45.21345, 12.0)
         ```
 
         Returns:
-            longitude - latitude - altitude tuple
+            tuple: longitude, latitude and altitude.
+
         Raises:
-            Exception if no GPS IFD found
+            Exception: if no GPS IFD found.
         """
         ifd = getattr(self, "gpsT", {})
         if set([
             "GPSLatitudeRef", "GPSLatitude",
             "GPSLongitudeRef", "GPSLongitude",
             "GPSAltitudeRef", "GPSAltitude"
         ]) <= set(ifd.keys()):
@@ -574,37 +572,67 @@
                 ifd["GPSAltitude"]
             )
         else:
             raise Exception("No location data found")
 
     def url_load_location(self, url, **kwargs):
         """
+        Return a static map image data from map provider.
+
+        ```python
+        >>> from Tyf import ifd
+        >>> i = ifd.Ifd()
+        >>> i.set_location(5.62347, 45.21345, 12)
+        >>> # below a mapbox-static-map url centered on [lon, lat] with a red
+        >>> # pin, width, height and zoom to be specified on call
+        >>> url = "https://api.mapbox.com/styles/v1/mapbox/outdoors-v11/static"
+        ... "/pin-s+f74e4e(%(lon)f,%(lat)f)/%(lon)f,%(lat)f,%(zoom)d,0"
+        ... "/%(width)dx%(height)d?access_token=%(token)s"
+        >>> data = i.url_load_location(
+        ...    url, zoom=15, width=600, height=400, token="xx-xxxxxx-xx"
+        ... )
+        >>> with io.open("dump.png", "wb") as f:
+        ...    f.write(data)
+        ```
+
+        Args:
+            url (str): map provider url containing `%(lon)f` and `%(lat)f`
+                format expression to be replaced by longitude and latitude
+                found in GPS data.
+            **kwargs (dict): key-value pairs to match entries in url according
+                to python string formatting.
+
+        Returns:
+            bytes|str: Image data.
         """
         lon, lat, alt = self.get_location()
         kwargs.update(lon=lon, lat=lat, alt=alt)
         try:
             opener = urlopen(url % kwargs)
         except Exception as error:
             print("%r" % error)
         else:
-            return StringIO(opener.read())
+            return opener.read()
 
-    def dump_location(self, name, *args, **kwargs):
+    def dump_location(self, name, url, **kwargs):
         """
+        Dump a static map image from map provider into filesystem.
+
+        Arguments:
+            name (str): a valid filepath.
+            url (str): map provider url containing `%(lon)f` and `%(lat)f`
+                format expression to be replaced by longitude and latitude
+                found in GPS data.
+            **kwargs (dict): key-value pairs to match entries in url according
+                to python string formatting.
         """
-        fileobj = io.open(name, "wb")
-        stringio = self.url_load_location(*args, **kwargs)
-        fileobj.write(stringio.getvalue())
-        fileobj.close()
-        stringio.close()
-        del fileobj, stringio
+        with io.open(name, "wb") as fileobj:
+            fileobj.write(self.url_load_location(url, **kwargs))
 
     def getModelTransformation(self, tie_idx=0):
-        """
-        """
         if "ModelTransformationTag" in self:
             matrix = GeoKeyModel["ModelTransformationTag"](
                *self["ModelTransformationTag"]
             )
         elif "ModelTiepointTag" in self and "ModelPixelScaleTag" in self:
             Sx, Sy, Sz = self["ModelPixelScaleTag"]
             I, J, K, X, Y, Z = self["ModelTiepointTag"][
@@ -622,21 +650,29 @@
                 0., -1., 0., 0.,
                 0., 0.,  1., 0.,
                 0., 0.,  0., 1.
             )
         return lambda x, y, z=0., m=matrix: Transform(m, x, y, z)
 
 
-def dump_mapbox_location(
-    cls, name, zoom=15, width=400, height=300,
-    token="pk.eyJ1IjoibW91c2lraXRvcyIsImEiOiJja2k2bGw2bnkzMXZ2MnJtcHlyejFrNXd4"
-          "In0.JIyrV6sWjehsRHKVMBDFaw",
-):
+def dump_mapbox_location(cls, name, zoom=15, width=400, height=300, token=""):
     """
+    Free `Tyf.ifd.Ifd.url_load_location` use case.
+    [Use your own Mapbox token]
+        https://docs.mapbox.com/api/overview/#access-tokens-and-token-scopes
+    ).
+
+    Arguments:
+        cls (dict or Tyf.ifd.Ifd): IFD containing GPS data.
+        name (str): filename to use.
+        zoom (int): map zoom level.
+        width (int): image width in pixel.
+        height (int): image height in pixel.
+        token (str): a valid Mapbox API token.
     """
     return cls.dump_location(
         name,
         "https://api.mapbox.com/styles/v1/mapbox/outdoors-v11/static/"
-        "pin-s+f74e4e(%(lon)s,%(lat)s)/%(lon)s,%(lat)s,%(zoom)s,0/"
-        "%(width)sx%(height)s?access_token=%(token)s",
-        zoom=15, width=400, height=300, token=token
+        "pin-s+f74e4e(%(lon)f,%(lat)f)/%(lon)f,%(lat)f,%(zoom)d,0/"
+        "%(width)dx%(height)d?access_token=%(token)s",
+        zoom=zoom, width=width, height=height, token=token
     )
```

### Comparing `Tyf-1.4.3/Tyf/values.py` & `Tyf-1.5.0/Tyf/values.py`

 * *Files identical despite different names*

### Comparing `Tyf-1.4.3/setup.py` & `Tyf-1.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 kw = {}
 
 f = open("VERSION", "r")
 long_description = open("README.md", "r")
 kw.update(**{
     "version": f.read().strip(),
     "name": "Tyf",
-    "keywords": ["ifd", "tiff", "jpeg", "exif", "gps", "geotiff", "PIL", "Pillow"],
+    "keywords": [
+        "ifd", "tiff", "jpeg", "exif", "gps", "geotiff", "PIL", "Pillow"
+    ],
     "author": "Bruno THOORENS",
     "author_email": "moustikitos@gmail.com",
     "maintainer": "Bruno THOORENS",
     "maintainer_email": "moustikitos@gmail.com",
     "url": "https://Moustikitos.github.io/tyf/",
-    "download_url": "https://github.com/Moustikitos/tyf",
+    "download_url": "https://github.com/Moustikitos/tyf/archive/master.zip",
     "description": "Pythonic way to read and edit IFD and EXIF tags.",
     "long_description": long_description.read(),
     "long_description_content_type": "text/markdown",
     "include_package_data": True,
     "packages": ["Tyf"],
     "license": "Copyright 2015-2020, THOORENS Bruno, BSD licence",
     "classifiers": [
```

