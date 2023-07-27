# Comparing `tmp/dec_ansi_parser-0.1.0.tar.gz` & `tmp/dec_ansi_parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dec_ansi_parser-0.1.0.tar", max compression
+gzip compressed data, was "dec_ansi_parser-0.2.0.tar", max compression
```

## Comparing `dec_ansi_parser-0.1.0.tar` & `dec_ansi_parser-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rwxr-xr-x   0        0        0     1508 2022-06-30 19:16:39.732958 dec_ansi_parser-0.1.0/LICENSE
--rw-r--r--   0        0        0     1050 2022-09-15 23:19:57.840436 dec_ansi_parser-0.1.0/README.md
--rw-r--r--   0        0        0      414 2022-11-14 19:46:04.177420 dec_ansi_parser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      166 2022-09-15 23:41:19.985860 dec_ansi_parser-0.1.0/src/dec_ansi_parser/__init__.py
--rw-r--r--   0        0        0    23984 2022-11-11 00:36:37.791093 dec_ansi_parser-0.1.0/src/dec_ansi_parser/formatter.py
--rw-r--r--   0        0        0    13241 2022-11-10 03:50:38.065966 dec_ansi_parser-0.1.0/src/dec_ansi_parser/parser.py
--rw-r--r--   0        0        0     4792 2022-11-10 04:08:01.454142 dec_ansi_parser-0.1.0/src/dec_ansi_parser/script_reader.py
--rw-r--r--   0        0        0     1786 2022-11-14 19:48:32.865074 dec_ansi_parser-0.1.0/setup.py
--rw-r--r--   0        0        0     1505 2022-11-14 19:48:32.865597 dec_ansi_parser-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1508 2023-07-27 21:28:07.043143 dec_ansi_parser-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1050 2023-07-27 21:28:07.043143 dec_ansi_parser-0.2.0/README.md
+-rw-r--r--   0        0        0      414 2023-07-27 21:36:18.337182 dec_ansi_parser-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-07-27 21:28:07.044143 dec_ansi_parser-0.2.0/src/dec_ansi_parser/__init__.py
+-rw-r--r--   0        0        0    24331 2023-07-27 21:28:07.045143 dec_ansi_parser-0.2.0/src/dec_ansi_parser/formatter.py
+-rw-r--r--   0        0        0    14271 2023-07-27 21:28:07.045143 dec_ansi_parser-0.2.0/src/dec_ansi_parser/parser.py
+-rw-r--r--   0        0        0     4792 2023-07-27 21:28:07.045143 dec_ansi_parser-0.2.0/src/dec_ansi_parser/script_reader.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 dec_ansi_parser-0.2.0/PKG-INFO
```

### Comparing `dec_ansi_parser-0.1.0/LICENSE` & `dec_ansi_parser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dec_ansi_parser-0.1.0/README.md` & `dec_ansi_parser-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dec_ansi_parser-0.1.0/src/dec_ansi_parser/formatter.py` & `dec_ansi_parser-0.2.0/src/dec_ansi_parser/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=too-many-locals, too-many-return-statements, too-few-public-methods
 from __future__ import annotations
 
 import abc
 import argparse
 import sys
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import Any, Callable, Dict, List, Optional, Union, cast
 
 from .parser import Action, Parser
 from .script_reader import ScriptLog
 
 __all__ = ["BaseHandler", "DescriptiveHandler", "VTParseHandler"]
 
 _UNKNOWN_TAG = "[[[UNKNOWN]]]"
@@ -602,22 +602,32 @@
         if parser.parameters:
             print(f"{len(parser.parameters)} Parameters:")
             for p in parser.parameters:
                 print(f"\t{p}")
         print()
 
 
+def null_handler(parser: Parser, action: Optional[Action], char: int) -> None:
+    pass
+
+
 def main() -> None:
     ap = argparse.ArgumentParser()
     ap.add_argument("-v", "--vtparse", action="store_true", help="emulate vtparse_test")
     ap.add_argument(
+        "-n",
+        "--null",
+        action="store_true",
+        help="null handler that does nothing (for profiling)",
+    )
+    ap.add_argument(
         "-d",
         "--debug",
         action="store_true",
-        help="include extra debugging output (only works with --vtparse)",
+        help="include extra debugging output (only works properly with --vtparse)",
     )
     ap.add_argument(
         "-s",
         "--script",
         action="store_true",
         help="read input file as a script(1) timing log (not compatible with stdin)",
     )
@@ -625,16 +635,18 @@
         "file",
         nargs="?",
         default="-",
         type=argparse.FileType("rb"),
         help="the file to parse, or - for stdin (defaults to stdin)",
     )
     args = ap.parse_args()
-    handler: BaseHandler
-    if args.vtparse:
+    handler: Callable[[Parser, Optional[Action], int], None]
+    if args.null:
+        handler = null_handler
+    elif args.vtparse:
         handler = VTParseHandler()
     else:
         handler = DescriptiveHandler()
     parser_ = Parser(handler, debug=args.debug and args.vtparse)
     if args.script:
         infile = ScriptLog(Path(args.file.name))
     else:
```

### Comparing `dec_ansi_parser-0.1.0/src/dec_ansi_parser/parser.py` & `dec_ansi_parser-0.2.0/src/dec_ansi_parser/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Terminal control sequence parser, following https://www.vt100.net/emu/dec_ansi_parser"""
 
 from __future__ import annotations
 
 import codecs
+import errno
 import io
-from enum import Enum, auto
+from enum import Enum
 from typing import (
     IO,
     Any,
     Callable,
     Dict,
     Iterator,
     List,
@@ -21,29 +22,32 @@
 )
 
 __all__ = ["State", "Action", "Parameters", "Parser"]
 
 
 # anywhere is denoted by None in the table generation code
 class State(Enum):
-    ground = auto()
-    escape = auto()
-    escape_intermediate = auto()
-    csi_entry = auto()
-    csi_param = auto()
-    csi_intermediate = auto()
-    csi_ignore = auto()
-    dcs_entry = auto()
-    dcs_param = auto()
-    dcs_intermediate = auto()
-    dcs_passthrough = auto()
-    dcs_ignore = auto()
-    osc_string = auto()
+    ground = 0
+    escape = 1
+    escape_intermediate = 2
+    csi_entry = 3
+    csi_param = 4
+    csi_intermediate = 5
+    csi_ignore = 6
+    dcs_entry = 7
+    dcs_param = 8
+    dcs_intermediate = 9
+    dcs_passthrough = 10
+    dcs_ignore = 11
+    osc_string = 12
     # sos/pm/apc string
-    other_string = auto()
+    other_string = 13
+
+    def __str__(self) -> str:
+        return self.name.upper()
 
 
 ground = State.ground
 escape = State.escape
 escape_intermediate = State.escape_intermediate
 csi_entry = State.csi_entry
 csi_param = State.csi_param
@@ -56,28 +60,28 @@
 dcs_ignore = State.dcs_ignore
 osc_string = State.osc_string
 # sos/pm/apc string
 other_string = State.other_string
 
 
 class Action(Enum):
-    ignore = auto()
-    print = auto()
-    execute = auto()
-    clear = auto()
-    collect = auto()
-    param = auto()
-    esc_dispatch = auto()
-    csi_dispatch = auto()
-    hook = auto()
-    put = auto()
-    unhook = auto()
-    osc_start = auto()
-    osc_put = auto()
-    osc_end = auto()
+    ignore = 0
+    print = 1
+    execute = 2
+    clear = 3
+    collect = 4
+    param = 5
+    esc_dispatch = 6
+    csi_dispatch = 7
+    hook = 8
+    put = 9
+    unhook = 10
+    osc_start = 11
+    osc_put = 12
+    osc_end = 13
 
 
 class Transition(NamedTuple):
     # if None, will stay in current state
     target: Optional[State]
     action: Optional[Action]
 
@@ -299,127 +303,161 @@
             return default
         return val
 
     def __bool__(self) -> bool:
         return len(self) != 0 and self != [None]
 
 
-def try_unicode(stream: Union[IO[bytes], io.RawIOBase]) -> Iterator[Tuple[int, bool]]:
-    "Yield a character code and whether the character was encoded as UTF-8."
+def try_unicode(
+    stream: Union[IO[bytes], io.RawIOBase], raw_bytes: bytearray
+) -> Iterator[int]:
+    """Yield a stream of character codes, with the sign denoting whether they
+    were parsed as raw ASCII or a multibyte UTF-8 sequence (positive if ASCII,
+    negative if UTF-8).
+    All bytes read are appended to `raw_bytes`.
+    """
     Decoder = codecs.getincrementaldecoder("utf-8")
-    while c := stream.read(1):
+    while True:
+        try:
+            c = stream.read(1)
+        except OSError as e:
+            if e.errno != errno.EIO:
+                raise
+            break  # EIO means EOF on some systems
+        if not c:
+            break
+        raw_bytes.extend(c)
         if 0xC2 <= c[0] <= 0xF4:
             # valid UTF-8 start byte
             try:
                 decoder = Decoder()
                 output = decoder.decode(c)
                 while not output:
                     # read() only returns None if it's non-blocking, which shouldn't
                     # be the case here
-                    output = decoder.decode(cast(bytes, stream.read(1)))
-                yield ord(output), True
+                    chars = cast(bytes, stream.read(1))
+                    raw_bytes.extend(chars)
+                    output = decoder.decode(chars)
+                yield -ord(output)
             except UnicodeDecodeError as ex:
                 # print(traceback.format_exc())
                 for x in ex.object:
-                    yield x, False
+                    yield x
         else:
-            yield c[0], False
+            yield c[0]
 
 
 class Parser:
     def __init__(
         self,
         callback: Callable[[Parser, Optional[Action], int], None],
         debug: bool = False,
     ):
-        """Callback may be called with None as the action when the parser is reset."""
+        """Callback will be called with None as the action when the parser is reset and at EOF."""
         self._trans = state_transitions
         self._cb = callback
         self._enable_debug = debug
 
         self.state = State.ground
         self.intermediate = ""
         # None is used for an unspecified parameter (vtparse assumes 0)
         self.parameters = Parameters([None])
         # used to suppress an esc_dispatch after a 2-byte string terminator
         self.esc_ended_string = False
+        # the raw bytes read since the last time callback was called, for reconstruction
+        self.curr_raw = bytearray()
 
     def reset(self) -> None:
         self.state = State.ground
         self.esc_ended_string = False
         self._cb(self, None, -1)
+        self.curr_raw.clear()
         self.clear()
 
     def clear(self) -> None:
         self.intermediate = ""
         self.parameters = Parameters([None])
 
-    def debug(self, *args: Any, **kwargs: Any) -> None:
+    def debug(self, msg: str, *args: Any, **kwargs: Any) -> None:
         if self._enable_debug:
-            print(*args, **kwargs)
+            print(msg.format(*args), **kwargs)
 
     def parse(self, data: Union[IO[bytes], io.RawIOBase]) -> None:
-        for char, was_utf8 in try_unicode(data):
-            # print(f"got: {char=}, {was_utf8=}")
+        for char in try_unicode(data, self.curr_raw):
             trans_table = self._trans[self.state]
-            if was_utf8:
+            if char < 0:
                 # unicode character
                 new_state, action = trans_table[0x7E]
+                char = -char
             else:
                 new_state, action = trans_table[
                     char & 0x7F if 0xA0 <= char <= 0xFF else char
                 ]
 
             if new_state is not None:
                 if self.state in on_exit:
-                    self.debug(f"processing on_exit from {self.state.name.upper()}")
+                    self.debug("processing on_exit from {}", self.state)
                     self.process(on_exit[self.state])
                     if self.state in (S.osc_string, S.dcs_passthrough) and char == 0x1B:
                         self.esc_ended_string = True
                 if action is not None:
                     self.debug("processing action with state change")
                     self.process(action, char)
                 if new_state in on_entry:
-                    self.debug(f"processing on_entry to {new_state.name.upper()}")
+                    self.debug("processing on_entry to {}", new_state)
                     self.process(on_entry[new_state])
                 self.state = new_state
             elif action is not None:
                 self.debug("processing action")
                 self.process(action, char)
+        self._cb(self, None, -1)
+        self.curr_raw.clear()
 
-    def process(self, action: Action, char: int = -1) -> None:
-        if action is A.ignore:
+    def process(
+        self,
+        action: Action,
+        char: int = -1,
+        # optimization: avoid several dict lookups in Action per call by storing
+        # these as local parameters when the function is defined
+        # Saves ~20% on a 1.3MB file with lots of truecolor escape sequences
+        ignore: Action = Action.ignore,
+        clear: Action = Action.clear,
+        collect: Action = Action.collect,
+        param: Action = Action.param,
+    ) -> None:
+        if action is ignore:
             pass
-        elif action is A.clear:
+        elif action is clear:
             self.clear()
-        elif action is A.collect:
+        elif action is collect:
             self.intermediate += chr(char)
-        elif action is A.param:
+        elif action is param:
             assert char >= 0
             if chr(char) == ";":
                 self.parameters.append(None)
             elif chr(char) == ":":
                 # handle subparameters, from section 5.4.2 of ECMA-48
                 if isinstance(self.parameters[-1], list):
                     self.parameters[-1].append(None)
                 else:
                     self.parameters[-1] = [
                         self.parameters[-1],
                         None,
                     ]
             else:
                 assert len(self.parameters) != 0, "parameters should not be empty"
-                lst: List[Union[Optional[int], List[Optional[int]]]]
+                lst: Union[Parameters, List[Optional[int]]]
                 if isinstance(self.parameters[-1], list):
-                    lst = self.parameters[-1]  # type: ignore
+                    lst = self.parameters[-1]
                 else:
                     lst = self.parameters
                 assert lst[-1] is None or isinstance(lst[-1], int)
                 digit = char - ord("0")
                 # use or here to handle None neatly
                 lst[-1] = (lst[-1] or 0) * 10 + digit
         else:
             if self.esc_ended_string:
                 self.esc_ended_string = False
                 if action is A.esc_dispatch and chr(char) == "\\":
                     return
             self._cb(self, action, char)
+            self.curr_raw.clear()
```

### Comparing `dec_ansi_parser-0.1.0/src/dec_ansi_parser/script_reader.py` & `dec_ansi_parser-0.2.0/src/dec_ansi_parser/script_reader.py`

 * *Files identical despite different names*

### Comparing `dec_ansi_parser-0.1.0/PKG-INFO` & `dec_ansi_parser-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: dec-ansi-parser
-Version: 0.1.0
+Version: 0.2.0
 Summary: Terminal control sequence parser
 License: BSD 3-Clause
 Author: yut23
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # dec_ansi_parser
 
 Pure-python terminal control sequence parser, based on [Paul Williams' DEC-compatible parser](https://www.vt100.net/emu/dec_ansi_parser).
 
 Changes from Williams' parser:
```

