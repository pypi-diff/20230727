# Comparing `tmp/icdutil-0.2.0.tar.gz` & `tmp/icdutil-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icdutil-0.2.0.tar", max compression
+gzip compressed data, was "icdutil-0.3.0.tar", max compression
```

## Comparing `icdutil-0.2.0.tar` & `icdutil-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-07-06 20:53:11.184780 icdutil-0.2.0/LICENSE
--rw-r--r--   0        0        0     1178 2023-07-06 20:53:11.184780 icdutil-0.2.0/README.md
--rw-r--r--   0        0        0     1157 2023-07-06 20:53:11.184780 icdutil-0.2.0/icdutil/__init__.py
--rw-r--r--   0        0        0    18763 2023-07-06 20:53:11.184780 icdutil-0.2.0/icdutil/num.py
--rw-r--r--   0        0        0     8151 2023-07-06 20:53:11.184780 icdutil-0.2.0/icdutil/slices.py
--rw-r--r--   0        0        0     2176 2023-07-06 20:53:11.184780 icdutil-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 icdutil-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-27 13:39:32.958471 icdutil-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1178 2023-07-27 13:39:32.958471 icdutil-0.3.0/README.md
+-rw-r--r--   0        0        0     1177 2023-07-27 13:39:32.958471 icdutil-0.3.0/icdutil/__init__.py
+-rw-r--r--   0        0        0    30406 2023-07-27 13:39:32.958471 icdutil-0.3.0/icdutil/addrmap.py
+-rw-r--r--   0        0        0    15292 2023-07-27 13:39:32.958471 icdutil-0.3.0/icdutil/addrrange.py
+-rw-r--r--   0        0        0    20747 2023-07-27 13:39:32.958471 icdutil-0.3.0/icdutil/num.py
+-rw-r--r--   0        0        0     8151 2023-07-27 13:39:32.958471 icdutil-0.3.0/icdutil/slices.py
+-rw-r--r--   0        0        0     2242 2023-07-27 13:39:32.958471 icdutil-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 icdutil-0.3.0/PKG-INFO
```

### Comparing `icdutil-0.2.0/LICENSE` & `icdutil-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icdutil-0.2.0/README.md` & `icdutil-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `icdutil-0.2.0/icdutil/__init__.py` & `icdutil-0.3.0/icdutil/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 """
 IC Utilities.
 """
-from . import num, slices
+from . import addrmap, addrrange, num, slices
```

### Comparing `icdutil-0.2.0/icdutil/num.py` & `icdutil-0.3.0/icdutil/num.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 #
 
 """Hardware Related Numeric Calculations."""
 
 import math
 import typing
 
+from .addrrange import AddrRange
+
 
 class AlignError(RuntimeError):
     """Alignment Error."""
 
 
 def unsigned_to_hex(value: int, width: int, prefix: str = "") -> str:
     """
@@ -390,25 +392,26 @@
     AssertionError: Value must be positive. -5 is not.
     """
     assert value > 0, f"Value must be positive. {value!r} is not."
     exp = math.floor(math.log(value, base))
     return base**exp
 
 
+# pylint: disable=redefined-outer-name
 def align(
     value: int,
     offset: typing.Optional[int] = None,
-    nxtalign: typing.Optional[int] = None,
+    align: typing.Optional[int] = None,
     minalign: int = 1,
     rewind=False,
 ):
     """
-    Forward `value` to `offset` and `nxtalign` and `minalign`.
+    Forward `value` to `offset` and `align` and `minalign`.
 
-    Without `offset` and `nxtalign` nothing happens.
+    Without `offset` and `align` nothing happens.
 
     >>> align(5)
     5
     >>> align(7)
     7
 
     An `offset` forwards the count if necessary or raises an :any:`AlignError`.
@@ -416,47 +419,47 @@
     >>> align(5, offset=8)
     8
     >>> align(5, offset=3)
     Traceback (most recent call last):
         ...
     icdutil.num.AlignError: Cannot use offset 3 as we are already at 5
 
-    A `nxtalign` forwards the value to the next multiple of `nxtalign`.
+    A `align` forwards the value to the next multiple of `align`.
 
-    >>> align(5, nxtalign=4)
+    >>> align(5, align=4)
     8
-    >>> align(8, nxtalign=4)
+    >>> align(8, align=4)
     8
-    >>> align(9, nxtalign=4)
+    >>> align(9, align=4)
     12
 
-    A `minalign` without `nxtalign` forwards the value to the next multiple of `minalign`
+    A `minalign` without `align` forwards the value to the next multiple of `minalign`
     >>> align(5, minalign=4)
     8
     >>> align(8, minalign=4)
     8
     >>> align(9, minalign=4)
     12
 
-    If both `nxtalign` and `minalign` are given, then the value is moved to the next multiple
+    If both `align` and `minalign` are given, then the value is moved to the next multiple
     of whichever of the both align values is bigger
-    >>> align(8, nxtalign=5, minalign=4)
+    >>> align(8, align=5, minalign=4)
     10
-    >>> align(8, nxtalign=4, minalign=6)
+    >>> align(8, align=4, minalign=6)
     12
 
-    If `offset` is given it is dominant over both `nxtalign` and `minalign`
-    >>> align(8, offset=9, nxtalign=4, minalign=6)
+    If `offset` is given it is dominant over both `align` and `minalign`
+    >>> align(8, offset=9, align=4, minalign=6)
     9
     """
     if offset is not None:
         if not rewind and value > offset:
             raise AlignError(f"Cannot use offset {offset} as we are already at {value}")
         return offset
-    curalign = max(nxtalign, minalign) if nxtalign is not None else minalign
+    curalign = max(align, minalign) if align is not None else minalign
     misalign = value % curalign
     if misalign:
         value += curalign - misalign
     return value
 
 
 def bytes2words(bytes_: typing.Sequence[int], bytesperword=4) -> typing.Sequence[int]:
@@ -655,15 +658,15 @@
     0x26, 1
     """
     endaddr = baseaddr + size - 1
     # search largest chunk fitting aligned into window of size
     bits = 0
     for bits in reversed(range(size.bit_length())):
         csize = 1 << bits
-        cbase = align(baseaddr, nxtalign=csize)
+        cbase = align(baseaddr, align=csize)
         cend = cbase + csize - 1
         if bits and cend <= endaddr:
             break
     # before chunk
     if baseaddr < cbase:
         yield from _iter_powerof2_segs(baseaddr, (cbase - baseaddr))
     # chunk
@@ -694,7 +697,61 @@
     >>> calc_addrwinmasks(0xF000, 0x180, addrwidth=16, dontcare='x')
     ('11110000xxxxxxxx', '111100010xxxxxxx')
     >>> calc_addrwinmasks(0xEFF0, 0x100, addrwidth=16)
     ('111011111111????', '111100000???????', '1111000010??????', '11110000110?????', '111100001110????')
     """
     assert len(dontcare) == 1, f"dontcare '{dontcare}' shall have length of 1"
     return tuple(to_mask(addrwidth, base, exp, dontcare) for base, exp in _iter_powerof2_segs(baseaddr, size))
+
+
+def _iter_aligned_segs(baseaddr: int, size: int) -> typing.Generator[AddrRange, None, None]:
+    endaddr = baseaddr + size - 1
+    # search largest chunk fitting aligned into window of size
+    sizeup = calc_next_power_of2(size)
+    baseup = align(baseaddr, align=sizeup)
+    end = baseup + size - 1
+    while end > endaddr:
+        sizeup //= 2
+        size = sizeup
+        baseup = align(baseaddr, align=sizeup)
+        end = baseup + size - 1
+    assert baseaddr <= baseup
+    # before chunk
+    pre_size = baseup - baseaddr
+    if pre_size > 0:
+        yield from _iter_aligned_segs(baseaddr, pre_size)
+    # chunk
+    yield AddrRange(baseup, size)
+    # after chunk
+    post_size = endaddr - end
+    if post_size > 0:
+        yield from _iter_aligned_segs(end + 1, post_size)
+
+
+def split_aligned_segs(baseaddr: int, size: int) -> typing.Tuple[AddrRange, ...]:
+    """
+    Split address window starting at `baseaddr` with `size` into segments with aligned base addresses.
+
+    The base addresses of the segments are aligned to `calc_next_power_of2(size)`.
+
+    Returns tuple of :any:`AddrRange`. Segment starting at `baseaddr` with `size`.
+
+    Args:
+        baseaddr (int): Address window start addresss
+        size (int):     Address window size
+
+    Example:
+
+    >>> split_aligned_segs(0, 1)
+    (AddrRange(0x0, '1 byte'),)
+    >>> split_aligned_segs(1024, 16)
+    (AddrRange(0x400, '16 bytes'),)
+    >>> split_aligned_segs(1024, 1024)
+    (AddrRange(0x400, '1 KB'),)
+    >>> split_aligned_segs(1024, 1024+768)
+    (AddrRange(0x400, '1 KB'), AddrRange(0x800, '768 bytes'))
+    >>> split_aligned_segs(256, 1024+768)
+    (AddrRange(0x100, '256 bytes'), AddrRange(0x200, '512 bytes'), AddrRange(0x400, '1 KB'))
+    >>> split_aligned_segs(1000, 1024)  # doctest: +ELLIPSIS
+    (AddrRange(0x3E8, '8 bytes'), AddrRange(0x3F0, '16 bytes'), AddrRange(0x400, '512 bytes'), ...(0x600, '488 bytes'))
+    """
+    return tuple(_iter_aligned_segs(baseaddr, size))
```

### Comparing `icdutil-0.2.0/icdutil/slices.py` & `icdutil-0.3.0/icdutil/slices.py`

 * *Files identical despite different names*

### Comparing `icdutil-0.2.0/pyproject.toml` & `icdutil-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "icdutil"
-version = "0.2.0"
+version = "0.3.0"
 description = "IC Design Utilities"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -23,14 +23,17 @@
 #[tool.poetry.scripts]
 
 
 [tool.poetry.dependencies]
 python = '^3.7.2'
 attrs = "^23.1.0"
 mementos = "^1.3.1"
+humannum = "^1.0.0"
+tabulate = "^0.9.0"
+types-tabulate = "^0.9.0"
 
 [tool.poetry.group.test.dependencies]
 black = '^23.3.0'
 coverage = '^6.4.4'
 isort = '^5.9'
 mypy = "^1.3.0"
 nbcpychecker = '^1.0.0'
```

### Comparing `icdutil-0.2.0/PKG-INFO` & `icdutil-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: icdutil
-Version: 0.2.0
+Version: 0.3.0
 Summary: IC Design Utilities
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Requires-Dist: humannum (>=1.0.0,<2.0.0)
 Requires-Dist: mementos (>=1.3.1,<2.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: types-tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 [![PyPI Version](https://badge.fury.io/py/icdutil.svg)](https://badge.fury.io/py/icdutil)
 [![Python Build](https://github.com/nbiotcloud/icdutil/actions/workflows/main.yml/badge.svg)](https://github.com/nbiotcloud/icdutil/actions/workflows/main.yml)
 [![Documentation](https://readthedocs.org/projects/icdutil/badge/?version=latest)](https://icdutil.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/nbiotcloud/icdutil/badge.svg?branch=main)](https://coveralls.io/github/nbiotcloud/icdutil?branch=main)
 [![python-versions](https://img.shields.io/pypi/pyversions/icdutil.svg)](https://pypi.python.org/pypi/icdutil)
```

