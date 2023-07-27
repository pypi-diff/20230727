# Comparing `tmp/RTFDE-0.0.2.tar.gz` & `tmp/RTFDE-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTFDE-0.0.2.tar", last modified: Mon Dec 28 15:12:26 2020, max compression
+gzip compressed data, was "RTFDE-0.1.0.tar", last modified: Thu Jul 27 11:55:00 2023, max compression
```

## Comparing `RTFDE-0.0.2.tar` & `RTFDE-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 s2e       (1000) s2e       (1000)        0 2020-12-28 15:12:26.167973 RTFDE-0.0.2/
--rw-r--r--   0 s2e       (1000) s2e       (1000)     3401 2020-12-28 15:12:26.167973 RTFDE-0.0.2/PKG-INFO
--rw-r--r--   0 s2e       (1000) s2e       (1000)     2157 2020-12-19 17:48:12.000000 RTFDE-0.0.2/README.md
-drwxr-xr-x   0 s2e       (1000) s2e       (1000)        0 2020-12-28 15:12:26.167973 RTFDE-0.0.2/RTFDE/
--rw-r--r--   0 s2e       (1000) s2e       (1000)     1256 2020-12-19 17:48:12.000000 RTFDE-0.0.2/RTFDE/__init__.py
--rw-r--r--   0 s2e       (1000) s2e       (1000)    19216 2020-12-19 17:48:12.000000 RTFDE-0.0.2/RTFDE/deencapsulate.py
--rw-r--r--   0 s2e       (1000) s2e       (1000)     2168 2020-12-19 17:48:12.000000 RTFDE-0.0.2/RTFDE/exceptions.py
--rw-r--r--   0 s2e       (1000) s2e       (1000)    10387 2020-12-19 17:48:12.000000 RTFDE-0.0.2/RTFDE/transformers.py
-drwxr-xr-x   0 s2e       (1000) s2e       (1000)        0 2020-12-28 15:12:26.167973 RTFDE-0.0.2/RTFDE.egg-info/
--rw-r--r--   0 s2e       (1000) s2e       (1000)     3401 2020-12-28 15:12:26.000000 RTFDE-0.0.2/RTFDE.egg-info/PKG-INFO
--rw-r--r--   0 s2e       (1000) s2e       (1000)      493 2020-12-28 15:12:26.000000 RTFDE-0.0.2/RTFDE.egg-info/SOURCES.txt
--rw-r--r--   0 s2e       (1000) s2e       (1000)        1 2020-12-28 15:12:26.000000 RTFDE-0.0.2/RTFDE.egg-info/dependency_links.txt
--rw-r--r--   0 s2e       (1000) s2e       (1000)       81 2020-12-28 15:12:26.000000 RTFDE-0.0.2/RTFDE.egg-info/requires.txt
--rw-r--r--   0 s2e       (1000) s2e       (1000)       12 2020-12-28 15:12:26.000000 RTFDE-0.0.2/RTFDE.egg-info/top_level.txt
--rw-r--r--   0 s2e       (1000) s2e       (1000)       38 2020-12-28 15:12:26.167973 RTFDE-0.0.2/setup.cfg
--rw-r--r--   0 s2e       (1000) s2e       (1000)     1119 2020-12-23 22:17:20.000000 RTFDE-0.0.2/setup.py
-drwxr-xr-x   0 s2e       (1000) s2e       (1000)        0 2020-12-28 15:12:26.167973 RTFDE-0.0.2/tests/
--rw-r--r--   0 s2e       (1000) s2e       (1000)        0 2020-12-19 17:48:12.000000 RTFDE-0.0.2/tests/__init__.py
-drwxr-xr-x   0 s2e       (1000) s2e       (1000)        0 2020-12-28 15:12:26.167973 RTFDE-0.0.2/tests/deencapsulate/
--rw-r--r--   0 s2e       (1000) s2e       (1000)        0 2020-12-19 17:48:12.000000 RTFDE-0.0.2/tests/deencapsulate/__init__.py
--rw-r--r--   0 s2e       (1000) s2e       (1000)     6099 2020-12-19 17:48:12.000000 RTFDE-0.0.2/tests/deencapsulate/test_de_encapsulate.py
-drwxr-xr-x   0 s2e       (1000) s2e       (1000)        0 2020-12-28 15:12:26.167973 RTFDE-0.0.2/tests/parse_rtf/
--rw-r--r--   0 s2e       (1000) s2e       (1000)        0 2020-12-19 17:48:12.000000 RTFDE-0.0.2/tests/parse_rtf/__init__.py
--rw-r--r--   0 s2e       (1000) s2e       (1000)    18940 2020-12-19 17:48:12.000000 RTFDE-0.0.2/tests/parse_rtf/test_parse_rtf.py
--rw-r--r--   0 s2e       (1000) s2e       (1000)     4113 2020-12-19 17:48:12.000000 RTFDE-0.0.2/tests/parse_rtf/test_validate_file.py
-drwxr-xr-x   0 s2e       (1000) s2e       (1000)        0 2020-12-28 15:12:26.167973 RTFDE-0.0.2/tests/test_utils/
--rw-r--r--   0 s2e       (1000) s2e       (1000)       21 2020-12-19 17:48:12.000000 RTFDE-0.0.2/tests/test_utils/__init__.py
--rw-r--r--   0 s2e       (1000) s2e       (1000)      381 2020-12-19 17:48:12.000000 RTFDE-0.0.2/tests/test_utils/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-27 11:55:00.377066 RTFDE-0.1.0/
+-rw-r--r--   0 user      (1000) user      (1000)     7651 2023-07-05 22:47:24.000000 RTFDE-0.1.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)       16 2023-07-05 22:47:24.000000 RTFDE-0.1.0/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     3563 2023-07-27 11:55:00.377066 RTFDE-0.1.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2769 2023-07-27 11:48:27.000000 RTFDE-0.1.0/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-27 11:55:00.377066 RTFDE-0.1.0/RTFDE/
+-rw-r--r--   0 user      (1000) user      (1000)     1093 2023-07-27 11:48:27.000000 RTFDE-0.1.0/RTFDE/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    20167 2023-07-27 11:48:27.000000 RTFDE-0.1.0/RTFDE/deencapsulate.py
+-rw-r--r--   0 user      (1000) user      (1000)     2168 2023-07-05 22:47:24.000000 RTFDE-0.1.0/RTFDE/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)    12665 2023-07-27 11:48:27.000000 RTFDE-0.1.0/RTFDE/grammar.py
+-rw-r--r--   0 user      (1000) user      (1000)    34525 2023-07-27 11:48:27.000000 RTFDE-0.1.0/RTFDE/text_extraction.py
+-rw-r--r--   0 user      (1000) user      (1000)    16502 2023-07-27 11:48:27.000000 RTFDE-0.1.0/RTFDE/transformers.py
+-rw-r--r--   0 user      (1000) user      (1000)    10607 2023-07-27 11:48:27.000000 RTFDE-0.1.0/RTFDE/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-27 11:55:00.377066 RTFDE-0.1.0/RTFDE.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3563 2023-07-27 11:55:00.000000 RTFDE-0.1.0/RTFDE.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      606 2023-07-27 11:55:00.000000 RTFDE-0.1.0/RTFDE.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-07-27 11:55:00.000000 RTFDE-0.1.0/RTFDE.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      117 2023-07-27 11:55:00.000000 RTFDE-0.1.0/RTFDE.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       12 2023-07-27 11:55:00.000000 RTFDE-0.1.0/RTFDE.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-07-27 11:55:00.377066 RTFDE-0.1.0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1270 2023-07-27 11:48:27.000000 RTFDE-0.1.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-27 11:55:00.377066 RTFDE-0.1.0/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-05 22:47:24.000000 RTFDE-0.1.0/tests/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-27 11:55:00.377066 RTFDE-0.1.0/tests/deencapsulate/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-05 22:47:24.000000 RTFDE-0.1.0/tests/deencapsulate/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    20851 2023-07-27 11:48:27.000000 RTFDE-0.1.0/tests/deencapsulate/test_de_encapsulate.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-27 11:55:00.377066 RTFDE-0.1.0/tests/parse_rtf/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-07-05 22:47:24.000000 RTFDE-0.1.0/tests/parse_rtf/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    24273 2023-07-27 11:48:27.000000 RTFDE-0.1.0/tests/parse_rtf/test_parse_rtf.py
+-rw-r--r--   0 user      (1000) user      (1000)     4660 2023-07-27 11:48:27.000000 RTFDE-0.1.0/tests/parse_rtf/test_validate_file.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-07-27 11:55:00.377066 RTFDE-0.1.0/tests/test_utils/
+-rw-r--r--   0 user      (1000) user      (1000)       21 2023-07-05 22:47:24.000000 RTFDE-0.1.0/tests/test_utils/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     6097 2023-07-27 11:48:27.000000 RTFDE-0.1.0/tests/test_utils/test_main_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)      381 2023-07-05 22:47:24.000000 RTFDE-0.1.0/tests/test_utils/utils.py
```

### Comparing `RTFDE-0.0.2/PKG-INFO` & `RTFDE-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,100 @@
 Metadata-Version: 2.1
 Name: RTFDE
-Version: 0.0.2
+Version: 0.1.0
 Summary: A library for extracting HTML content from RTF encapsulated HTML as commonly found in the exchange MSG email format.
 Home-page: https://github.com/seamustuohy/RTFDE
 Author: seamus tuohy
 Author-email: code@seamustuohy.com
-License: UNKNOWN
-Description: # RTFDE: RTF De-Encapsulator
-        
-        A python3 library for extracting encapsulated `HTML` & `plain text` content from the `RTF` bodies of .msg files.
-        
-        De-encapsulation enables previously encapsulated HTML and plain text content to be extracted and rendered as HTML and plain text instead of the encapsulating RTF content. After de-encapsulation, the HTML and plain text should differ only minimally from the original HTML or plain text content.
-        
-        # Features
-        
-        - De-encapsulate HTML from RTF encapsulated HTML.
-        - De-encapsulate plain text from RTF encapsulated text.
-        
-        # Known Issues
-        
-        - This library *fully* unquotes text it de-encapsulates because it does not know which text was quoted in the RTF conversion process and which text was quoted in the original html/text. So, for instance escaped [Quoted-Printable](https://en.wikipedia.org/wiki/Quoted-printable) text will be returned un-escaped.
-        - This library currently can't [combine attachments](https://docs.microsoft.com/en-us/openspecs/exchange_server_protocols/ms-oxrtfex/b518f0bc-468c-4218-87a7-8f8859bf5773) from a .MSG Message object with the de-encapsulated HTML. This is mostly because I could not get a good set of examples of encapsulated HTML which had attachment objects that needed to be integrated back into the body of the HTML.
-        
-        # Anti-Features (I don't intend to have this library do this.)
-        
-        - Extract plain text from RTF encapsulated HTML. If you want this, then you will have to parse the HTML using another library.
-        
-        # Installation
-        
-        **To install from the pip package.**
-        
-        ```
-        pip3 install RTFDE
-        
-        ```
-        
-        # Usage
-        
-        ## De-encapsulating HTML or TEXT
-        
-        ```python
-        from RTFDE.deencapsulate import DeEncapsulator
-        
-        with open('rtf_file', 'r') as fp:
-            raw_rtf  = fp.read()
-            rtf_obj = DeEncapsulator(raw_rtf)
-            rtf_obj.deencapsulate()
-            if rtf_obj.content_type == 'html':
-                print(rtf_obj.html)
-            else:
-                print(rtf_obj.text)
-        ```
-        
-        # Contribute
-        
-        Please check the [contributing guidelines](./CONTRIBUTING.md)
-        
-        # License
-        
-        Please see the [license file](./LICENSE) for license information on RTFDE. If you have further questions related to licensing PLEASE create an issue about it on github.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Communications :: Email :: Filters
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: msg_parse
+Provides-Extra: dev
+License-File: LICENSE
+
+# RTFDE: RTF De-Encapsulator
+
+A python3 library for extracting encapsulated `HTML` & `plain text` content from the `RTF` bodies of .msg files.
+
+De-encapsulation enables previously encapsulated HTML and plain text content to be extracted and rendered as HTML and plain text instead of the encapsulating RTF content. After de-encapsulation, the HTML and plain text should differ only minimally from the original HTML or plain text content.
+
+# Features
+
+- De-encapsulate HTML from RTF encapsulated HTML.
+- De-encapsulate plain text from RTF encapsulated text.
+
+# Known Issues
+
+- This library *fully* unquotes text it de-encapsulates because it does not know which text was quoted in the RTF conversion process and which text was quoted in the original html/text. So, for instance escaped [Quoted-Printable](https://en.wikipedia.org/wiki/Quoted-printable) text will be returned un-escaped.
+- This library currently can't [combine attachments](https://docs.microsoft.com/en-us/openspecs/exchange_server_protocols/ms-oxrtfex/b518f0bc-468c-4218-87a7-8f8859bf5773) from a .MSG Message object with the de-encapsulated HTML. This is mostly because I could not get a good set of examples of encapsulated HTML which had attachment objects that needed to be integrated back into the body of the HTML.
+
+# Anti-Features (I don't intend to have this library do this.)
+
+- Extract plain text from RTF encapsulated HTML. If you want this, then you will have to parse the HTML using another library.
+
+# Installation
+
+**To install from the pip package.**
+
+```
+pip3 install RTFDE
+
+```
+
+# Usage
+
+## De-encapsulating HTML or TEXT
+
+```python
+from RTFDE.deencapsulate import DeEncapsulator
+
+with open('rtf_file', 'rb') as fp:
+    raw_rtf  = fp.read()
+    rtf_obj = DeEncapsulator(raw_rtf)
+    rtf_obj.deencapsulate()
+    if rtf_obj.content_type == 'html':
+        print(rtf_obj.html)
+    else:
+        print(rtf_obj.text)
+```
+
+
+
+# Enabling Logging
+
+Any logging (including how verbose the logging is) can be handled by configuring logging. You can enable RTFDE's logging at the highest level by getting and setting the "RTFDE" logger.
+
+```
+log = logging.getLogger("RTFDE")
+log.setLevel(logging.INFO)
+```
+
+
+
+
+
+
+To see how to enable more in-depth logging for debugging check out the CONTRIBUTING.md file.
+
+```
+# Now, get the log that you want
+# The main logger is simply called RTFDE. That will get you all the *normal* logs.
+requests_log = logging.getLogger("RTFDE")
+requests_log.setLevel(logging.DEBUG)
+requests_log.propagate = True
+```
+
+
+# Contribute
+
+Please check the [contributing guidelines](./CONTRIBUTING.md)
+
+# License
+
+Please see the [license file](./LICENSE) for license information on RTFDE. If you have further questions related to licensing PLEASE create an issue about it on github.
```

### Comparing `RTFDE-0.0.2/README.md` & `RTFDE-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -30,24 +30,51 @@
 # Usage
 
 ## De-encapsulating HTML or TEXT
 
 ```python
 from RTFDE.deencapsulate import DeEncapsulator
 
-with open('rtf_file', 'r') as fp:
+with open('rtf_file', 'rb') as fp:
     raw_rtf  = fp.read()
     rtf_obj = DeEncapsulator(raw_rtf)
     rtf_obj.deencapsulate()
     if rtf_obj.content_type == 'html':
         print(rtf_obj.html)
     else:
         print(rtf_obj.text)
 ```
 
+
+
+# Enabling Logging
+
+Any logging (including how verbose the logging is) can be handled by configuring logging. You can enable RTFDE's logging at the highest level by getting and setting the "RTFDE" logger.
+
+```
+log = logging.getLogger("RTFDE")
+log.setLevel(logging.INFO)
+```
+
+
+
+
+
+
+To see how to enable more in-depth logging for debugging check out the CONTRIBUTING.md file.
+
+```
+# Now, get the log that you want
+# The main logger is simply called RTFDE. That will get you all the *normal* logs.
+requests_log = logging.getLogger("RTFDE")
+requests_log.setLevel(logging.DEBUG)
+requests_log.propagate = True
+```
+
+
 # Contribute
 
 Please check the [contributing guidelines](./CONTRIBUTING.md)
 
 # License
 
 Please see the [license file](./LICENSE) for license information on RTFDE. If you have further questions related to licensing PLEASE create an issue about it on github.
```

### Comparing `RTFDE-0.0.2/RTFDE/__init__.py` & `RTFDE-0.1.0/RTFDE/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,26 +13,23 @@
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
 # FITNESS FOR A PARTICULAR PURPOSE. See the included LICENSE file for details.
 
 """
 RTFDE: A python3 library for extracting HTML content from RTF encapsulated HTML.
 
-https://github.com/seamustuohy/RTF_De-Encapsulator
+https://github.com/seamustuohy/RTFDE
 """
 
 __author__ = 'seamus tuohy'
-__date__ = '2020-12-05'
-__version__ = '0.00.1'
+__date__ = '2023-06-18'
+__version__ = '0.1.0'
 
 import logging
+from logging import NullHandler
+
+logging.getLogger(__name__).addHandler(NullHandler())
+logging.getLogger(__name__ + ".tree_logger").addHandler(NullHandler())
+
 
-FORMAT = "%(levelname)s [%(filename)s:%(lineno)s - %(funcName)s() ] %(message)s"
-formatter = logging.Formatter(FORMAT)
-default_handler = logging.StreamHandler()
-default_handler.setFormatter(formatter)
-
-logger = logging.getLogger(__name__)
-logger.addHandler(default_handler)
-logger.setLevel(logging.WARNING)
 
 from RTFDE.deencapsulate import DeEncapsulator
```

### Comparing `RTFDE-0.0.2/RTFDE/deencapsulate.py` & `RTFDE-0.1.0/RTFDE/deencapsulate.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,333 +9,382 @@
 # Software Foundation, either version 3 of the License, or (at your option)
 # any later version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
 # FITNESS FOR A PARTICULAR PURPOSE. See the included LICENSE file for details.
 
-import re
+from typing import Union, AnyStr, Tuple, Dict, Any
+from io import BufferedReader
+
 from lark import Lark
 from lark.tree import Tree
 from lark.lexer import Token
-from oletools.common import codepages
+from lark.exceptions import UnexpectedInput
 
-from RTFDE.transformers import RTFUnicodeDecoder, StripNonVisibleRTFGroups, RTFCleaner
+from RTFDE.transformers import RTFCleaner, StripControlWords
+from RTFDE.transformers import StripNonVisibleRTFGroups
+from RTFDE.transformers import StripUnusedSpecialCharacters
+from RTFDE.utils import encode_escaped_control_chars
+from RTFDE.utils import log_validators, log_transformations, is_logger_on
+from RTFDE.transformers import get_stripped_HTMLRTF_values, DeleteTokensFromTree, strip_binary_objects
+from RTFDE.grammar import make_concise_grammar
+from RTFDE.text_extraction import TextDecoder
+from RTFDE.text_extraction import validate_ansi_cpg
 
 # For catching exceptions
 from RTFDE.exceptions import NotEncapsulatedRtf, MalformedEncapsulatedRtf, MalformedRtf
-from io import BufferedReader
-
 
 import logging
-log = logging.getLogger('RTFDE')
+log = logging.getLogger("RTFDE")
 
 class DeEncapsulator():
     """De-Encapsulating RTF converter of HTML/TEXT found in .msg files.
 
-    De-encapsulation enables previously encapsulated HTML and plain text content to be extracted and rendered as HTML and plain text instead of the encapsulating RTF content. After de-encapsulation, the HTML and plain text should differ only minimally from the original HTML or plain text content.
-
+De-encapsulation enables previously encapsulated HTML and plain text content to be extracted and rendered as HTML and plain text instead of the encapsulating RTF content. After de-encapsulation, the HTML and plain text should differ only minimally from the original HTML or plain text content.
 
-        Parameters:
-            raw_rtf: (str): It's the raw RTF string.
 
-            grammar: (raw str): OPTIONAL - Lark (https://github.com/lark-parser/lark) parsing grammar which defines the RTF language. If you think my grammar is shoddy this is your chance to test out a better one and make a pull request. :D
+Parameters:
+    raw_rtf: (bytes): It's the raw RTF file as bytes.
+    grammar: (str): OPTIONAL - Lark parsing grammar which defines the RTF language. https://github.com/lark-parser/lark If you think my grammar is shoddy this is your chance to test out a better one and make a pull request.
+
+Attributes:
+    content: (bytes) The deencapsulated content no matter what format it is in. Populated by the `deencapsulate` function.
+    html: (bytes) The deencapsulated content IF it is HTML content. Populated by the `set_content` function.
+    text: (bytes) The deencapsulated content IF it is plain text content. Populated by the `set_content` function.
+    found_binary: List of dictionaries containing binary data extracted from the rtf file.
+    content_type: The type of content encapsulated in .rtf data (html or text). Populated by the `get_content_type` function.
+    full_tree: The full .rtf object parsed into an object Tree using the grammar. Populated by the `parse_rtf` function.
+    doc_tree: The `document` portion of the .rtf full_tree object.
+    raw_rtf: The raw encapsulated .rtf data in byte format.
+    grammar: The Lark parsing grammer used to parse the .rtf data.
+    content_type_token: The .rtf header token identifying the content type. (\\fromhtml1 OR \\fromtext)
+    parser: The lark parser. Should not need to be manipulated directly. But, useful for debugging and saving the parsed object.
     """
 
-    def __init__(self, raw_rtf:str, grammar:str = None):
+    def __init__(self, raw_rtf:bytes, grammar: Union[str,None] = None):
         """Load in the Encapsulated test and setup the grammar used to parse the encapsulated RTF.
 
-        NOTE: This does not do the parsing in the init so that you can initiate the object and do the parsing step by step.
-
+NOTE: This does not do the parsing in the init so that you can initiate the object and do the parsing step by step.
 
-        Parameters:
-            raw_rtf: (str): It's the raw RTF string.
+Parameters:
+        raw_rtf: (bytes): It's the raw RTF string.
+        grammar: (str): OPTIONAL - Lark parsing grammar which defines the RTF language. https://github.com/lark-parser/lark If you think my grammar is shoddy this is your chance to test out a better one and make a pull request.
 
-            grammar: (raw str): OPTIONAL - Lark (https://github.com/lark-parser/lark) parsing grammar which defines the RTF language. If you think my grammar is shoddy this is your chance to test out a better one and make a pull request. :D
-
-        """
-        self.content = None
-        self.content_type = None
-        self._content_type_token = None
-        self.html = None
-        self.plain_text = None
-        self.stripped_rtf = None
-        self.simplified_rtf = None
-        self.full_tree = None
-        self.doc_tree = None
-        self.charset = None
-        self.text_codec = None
-        self._catch_common_validation_issues(raw_rtf)
+Raises:
+        TypeError: The raw_rtf data passed is not the correct type of data (string/byte string).
+"""
+        self.content: str
+        self.content_type: str
+        self.content_type_token: str
+        self.parser: Any
+
+        self.html: str
+        self.text: str
+        self.found_binary: list
+        self.full_tree: Tree
+        self.doc_tree: Tree
+        self.catch_common_validation_issues(raw_rtf)
         if isinstance(raw_rtf, bytes):
-            self.raw_rtf = raw_rtf.decode()
-        elif isinstance(raw_rtf, str):
-            self.raw_rtf = raw_rtf
+            raw_rtf_bytes = raw_rtf
         else:
             raise TypeError("DeEncapssulator only accepts RTF files in string or byte-string formats")
+        raw_rtf_bytes = raw_rtf_bytes.rstrip(b'\x00')
+        raw_rtf_bytes = raw_rtf_bytes.replace(b'\r\n',b'\n')
+        raw_rtf_bytes = raw_rtf_bytes.replace(b'\r',b'\n')
+        self.raw_rtf: bytes = raw_rtf_bytes
         if grammar is not None:
-            self._grammar = grammar
+            self.grammar: str = grammar
         else:
-            self._grammar = r"""
-start : OPENPAREN document CLOSEPAREN
+            self.grammar = make_concise_grammar()
 
-document: (CONTROLWORD | CONTROLSYMBOL | TEXT | group | " " | RTFESCAPE)+
-group: OPENPAREN (CONTROLWORD | CONTROLSYMBOL | TEXT | group | RTFESCAPE)* CLOSEPAREN
+    def deencapsulate(self):
+        """De-encapsulate the RTF content loaded into the De-Encapsulator.
 
-// Text is given priority over control terms with TERM.PRIORITY = 2
-// This is used to ensure that escaped \ AND { AND } are not matched in others
-TEXT.2: /\\\\/ | /\\[{}]/+ | /[^\\{}]/+
-CONTROLWORD: /(?<!\\)\\/ /[a-zA-Z]/+ /[0-9\-]/*
-CONTROLSYMBOL: /(?<!\\)\\/ "|" | "~" | "-" | "_" | ":" | "\*" | "\\{" | "\\}"
-
-// Increased priority of escape chars to make unescaping easier
-// Multiple char acceptance is important here because if you just catch one escape at a time you mess up multi-byte values.
-RTFESCAPE.3: ("\\'" /[0-9A-Fa-f]/~2)+ | ("\\u" /[-]*[0-9]+\s?\??/)+
+Once you have loaded in the raw rtf this function will set the properties containing the encapsulated content. The `content` property will store the content no matter what format it is in. The `html` and `text` properties will be populated based on the type of content that is extracted. (self.html will be populated if it is html and self.text if it is plain text.)
+        """
+        stripped_data = strip_binary_objects(self.raw_rtf)
+        non_binary_rtf = stripped_data[0]
+        found_binary = stripped_data[1]
+        if len(found_binary) > 0:
+            self.found_binary = found_binary
+            log.info("Binary data found and extracted from rtf file.")
+        escaped_rtf = encode_escaped_control_chars(non_binary_rtf)
+        if is_logger_on("RTFDE.transform_logger") is True:
+            log_transformations(escaped_rtf)
+        try:
+            self.parse_rtf(escaped_rtf)
+        except UnexpectedInput as _e:
+            raise MalformedEncapsulatedRtf(f"Malformed encapsulated RTF discovered:") from _e
+        Decoder = TextDecoder()
+        Decoder.update_children(self.full_tree)
+        self.get_doc_tree()
+        self.validate_encapsulation()
+
+        # remove htmlrtf escaped values
+        htmlrtf_stripped = self.strip_htmlrtf_tokens()
+        # Strips whitespace from control words
+        control_stripped = StripControlWords().transform(htmlrtf_stripped)
+        # Strip unused control chars
+        special_stripper = StripUnusedSpecialCharacters()
+        non_special_tree = special_stripper.transform(control_stripped)
+        # Strip out non-visible RTF groups
+        stripper = StripNonVisibleRTFGroups()
+        stripped_tree = stripper.transform(non_special_tree)
+        # Converts any remaining tokens
+        cleaner = RTFCleaner(visit_tokens=True)
+        cleaned_text = cleaner.transform(stripped_tree)
 
-OPENPAREN:  "{"
-CLOSEPAREN: "}"
+        self.content = cleaned_text
+        self.set_content() # Populates self.html || self.text
 
-%import common.ESCAPED_STRING
-%import common.SIGNED_NUMBER
+    def validate_charset(self, fallback_to_default:bool =False) -> bytes:
+        """Validate and return the RTF charset keyword from the RTF streams header.
 
-%import common.WS
-%ignore WS
-"""
-    @staticmethod
-    def _catch_common_validation_issues(raw_rtf):
-        """Checks for likely common valid input mistakes that may occur when folks try to use this library and raises exceptions to try and help identify them."""
-        if isinstance(raw_rtf, BufferedReader):
-            raise TypeError("Data passed as file pointer. DeEncapsulator only accepts strings and byte-strings.")
-        if raw_rtf == None:
-            raise TypeError("Data passed as raw RTF file is a null object `None` keyword.")
-        if raw_rtf[:8] == b"\xd0\xcf\x11\xe0\xa1\xb1\x1a\xe1":
-            raise TypeError("Data passed is a full MSG object. You must extract the encapsulated RTF body first.")
-        if (raw_rtf == b"") or (raw_rtf == ""):
-            raise MalformedRtf("Data passed as raw RTF file is an empty string.")
+Args:
+        fallback_to_default (bool): Allows you to force the use of the default charset "\\ansi" if one is not found.
 
-    def _simplify_text_for_parsing(self):
-        """Replaces control chars within the text with their RTF encoded versions \\'HH.
-        """
-        cleaned = self.stripped_rtf.replace('\\\\', "\\'5c")
-        cleaned = cleaned.replace('\\{', "\\'7b")
-        cleaned = cleaned.replace('\\}', "\\'7d")
-        return cleaned
+Raises:
+        MalformedRtf: RTF stream does not include charset control word.
 
+Returns:
+        The RTF charset keyword from the RTF streams header.
+"""
+        main_headers = self.get_header_control_words_before_first_group()
 
-    def deencapsulate(self):
-        """De-encapsulate the RTF content loaded into the De-Encapsulator.
+        for token in main_headers:
+            if token.value in [b'\\ansi', b'\\mac', b'\\pc', b'\\pca']:
+                return token
 
-        Once you have loaded in the raw rtf this function will set the properties containing the encapsulated content. The `content` property will store the content no matter what format it is in. The `html` and `text` properties will be populated based on the type of content that is extracted. (self.html will be populated if it is html and self.text if it is plain text.)
-        """
-        self.stripped_rtf = self._strip_htmlrtf_sections()
-        self.simplified_rtf = self._simplify_text_for_parsing()
-        self.doc_tree = self._parse_rtf()
-        self._validate_encapsulation()
-        self.charset = self._get_charset()
-        self.text_codec = self._get_python_codec()
-        self.content = self._deencapsulate_from_tree()
+        log.debug("Acceptable charset not found as the second token in the RTF stream. The control word for the character set must precede any plain text or any table control words. So, if this stream doesn't have one it is malformed or corrupted.")
+        if fallback_to_default is False:
+            raise MalformedRtf("RTF stream does not include charset control word.")
+
+        log.warning("The fallback_to_default option on _get_charset is considered DANGEROUS if used on possibly malicious samples. Make sure you know what you are doing before using it.")
+        log.info("Attempting to decode RTF using the default charset ansi. This is not recommended and could have unforeseen consequences for the resulting file and your systems security.")
+        log.debug("You have a malformed RTF stream. Are you sure you really want to be parsing it? It might not just be corrupted. It could be maliciously constructed.")
+        return b"\\ansi"
+
+    def set_content(self):
+        """Populate the html or text content based on the content type. Populates self.html and/or self.text variables."""
         self.content_type = self.get_content_type()
         if self.content_type == 'html':
             self.html = self.content
         else:
             self.text = self.content
 
+    def get_doc_tree(self):
+        """Extract the document portion of the .rtf full_tree object. Populates the classes doc_tree attribute.
+
+Raises:
+        ValueError: The .rtf document object is missing or mis-located in the .rtf's full_tree object.
+"""
+        if self.full_tree.children[1].data == "document":
+            self.doc_tree = self.full_tree.children[1]
+        else:
+            raise ValueError("Document object in the wrong place after parsing.")
+
     def get_content_type(self):
         """Provide the type of content encapsulated in RTF.
 
-        NOTE: This function will only work after the header validation has completed. Header validation also extracts the content type of the encapsulated data.
-        """
-        if self._content_type_token is None:
-            self._validate_FROM_in_doc_header()
-        elif self._content_type_token == '\\fromhtml1':
+NOTE: This function will only work after the header validation has completed. Header validation also extracts the content type of the encapsulated data.
+
+Raises:
+        NotEncapsulatedRtf: The .rtf object is missing an encapsulated content type header. Which means that it is likely just a regular .rtf file.
+"""
+        if self.content_type_token is None:
+            self.validate_FROM_in_doc_header()
+        elif self.content_type_token == b'\\fromhtml1':
             return 'html'
-        elif self._content_type_token == '\\fromtext':
+        elif self.content_type_token == b'\\fromtext':
             return "text"
-        else:
-            raise NotEncapsulatedRtf("Data is missing encapsulated content type header (the FROM header).")
 
-    def _validate_encapsulation(self):
-        """Runs simple tests to validate that the file in question is an rtf document which contains encapsulation.
-        """
-        self._validate_rtf_doc_header()
-        self._validate_FROM_in_doc_header()
+        raise NotEncapsulatedRtf("Data is missing encapsulated content type header (the FROM header).")
 
-    def _parse_rtf(self) -> Tree:
-        """Parse RTF file's header and document and extract the objects within the RTF into a Tree."""
-        parser = Lark(self._grammar, parser='lalr')
-        self.full_tree = parser.parse(self.simplified_rtf)
-        # An RTF file has the following syntax: '{' <header & document>'}'
-        # We only need the header and document so we only extract the 1st obj.
-        return self.full_tree.children[1]
+    def validate_encapsulation(self):
+        """Runs simple tests to validate that the file in question is an rtf document which contains encapsulation."""
+        self.validate_rtf_doc_header(self.doc_tree)
+        self.validate_charset()
+        self.validate_FROM_in_doc_header()
+        ansicpg = self.get_ansicpg_header()
+        if ansicpg is not None: # ansicpg is not manditory
+            validate_ansi_cpg(ansicpg.value)
 
-    def _strip_htmlrtf_sections(self) -> Tree:
-        """Strip out \\htmlrtf tagged sections which need to be ignored in the de-encapsulation and are difficult to extract after it has been converted into a tree.
+    def get_ansicpg_header(self) -> Union[Token,None]:
+        """Extract the ansicpg control word from the .rtf header.
 
-        The \\htmlrtf keyword toggles pieces of RTF to be ignored during reverse RTF->HTML conversion. Lack of a parameter turns it on, parameter 0 turns it off. But, these are not always included in a consistent way. They can appear withing and across groups in the stream. So, they need to be extracted before the stream is tokenized and placed into a tree.
-        """
-        htmlrtf = re.compile(r'[\s]*\\htmlrtf[^0].*?\\htmlrtf0[\n]*', flags=re.MULTILINE|re.DOTALL)
-        return  htmlrtf.sub("", self.raw_rtf)
+Returns:
+        A lark CONTROLWORD Token with the `\\ansicpg` value. Returns None if the `\\ansicpg` control word is not included as this is only required if there is Unicode which needs to be converted to ANSI within a .rtf file.
+"""
+        headers = self.get_header_control_words_before_first_group()
+        for item in headers:
+            if item.value.startswith(b'\\ansicpg'):
+                return item
+        return None
 
-    def _deencapsulate_from_tree(self) -> str:
-        """De-encapsulates HTML from document tree into final content.
-        """
-        decoded_tree = RTFUnicodeDecoder().visit_topdown(self.doc_tree)
+    def parse_rtf(self, rtf: str):
+        """Parse RTF file's header and document and extract the objects within the RTF into a Tree. Populates the self.full_tree attribute.
 
-        stripper = StripNonVisibleRTFGroups()
-        stripped_tree = stripper.transform(decoded_tree)
+Args:
+        rtf: The .rtf string to parse with the projects lark grammar.
+"""
+        # Uncomment Lark debug argument if you want to enable logging.
+        # Note, this not enable ALL lark debug logging.
+        # To do that we would not be able to use the Lark convinence class which we are using here.
+        self.parser = Lark(self.grammar,
+                           parser='lalr',
+                           keep_all_tokens=True,
+                           use_bytes=True,
+                           # debug=True,
+                           propagate_positions=True)
+        self.full_tree = self.parser.parse(rtf)
+        if is_logger_on("RTFDE.transform_logger") is True:
+            log_transformations(self.full_tree)
 
-        cleaner = RTFCleaner(rtf_codec=self.text_codec)
-        cleaned_text = cleaner.transform(stripped_tree)
-        # The conversion process inserts spaces on newlines where there were none
-        cleaned_text = re.sub(r'[\r\n][\s\r\n]{2,}', '\n', cleaned_text)
-        return cleaned_text
+
+    def strip_htmlrtf_tokens(self) -> Tree:
+        """Strip tokens from with htmlrtf regions of the doc_tree as they were not part of the original HTML content.
+
+Returns:
+        .rtf doc_tree stripped of all non-original tokens.
+"""
+        # remove htmlrtf escaped values
+        delete_generator = get_stripped_HTMLRTF_values(self.doc_tree)
+        tokens_to_delete = list(delete_generator)
+        deleter = DeleteTokensFromTree(tokens_to_delete)
+        htmlrtf_cleaned_tree = deleter.transform(self.doc_tree)
+        return htmlrtf_cleaned_tree
 
 
-    def _get_header_control_words_before_first_group(self) -> list:
+    def get_header_control_words_before_first_group(self) -> list:
         """Extracts all the control words in the first 20 tokens of the document or all the tokens which occur before the first group (whichever comes first.)
 
-        This is used to extract initial header values for validation functions.
+This is used to extract initial header values for validation functions.
+
+Returns:
+        A list containing the header tokens in the .rtf data.
         """
         initial_control_words = []
         for token in self.doc_tree.children[:20]:
             if isinstance(token, Token):
                 initial_control_words.append(token)
             else:
                 return initial_control_words
         return initial_control_words
 
 
-    def _get_charset(self, fallback_to_default:bool =False) -> str:
-        """Extracts the RTF charset keyword from the RTF streams header.
-
-        Parameters:
-            fallback_to_default (bool): Allows you to force the use of the default charset "\ansi" if one is not found.
-        """
-        main_headers = self._get_header_control_words_before_first_group()
-        charset = None
-        for token in main_headers:
-            if token in ["\\ansi", "\\mac", "\\pc", "\\pac"]:
-                return token
-
-        if charset is None:
-            log.debug("Acceptable charset not found as the second token in the RTF stream. The control word for the character set must precede any plain text or any table control words. So, if this stream doesn't have one it is malformed or corrupted.")
-            if fallback_to_default is False:
-                raise MalformedRtf("RTF stream does not include charset control word.")
-            else:
-                log.warning("The fallback_to_default option on _get_charset is considered DANGEROUS if used on possibly malicious samples. Make sure you know what you are doing before using it.")
-                log.info("Attempting to decode RTF using the defulat charset ansi. This is not recommended and could have unforeseen consequences for the resulting file and your systems security.")
-                log.debug("You have a malformed RTF stream. Are you sure you really want to be parsing it? It might not just be corrupted. It could be maliciously constructed.")
-                return "\\ansi"
-
-    def _get_codepage_num(self) -> int:
-        """Extracts the unicode codepage number from the RTF streams header.
-        """
-        # This keyword should be emitted in the RTF header section right after the \ansi, \mac, \pc or \pca keyword. But, various document tags like \fbids often are thrown all over the header so we have to check the first group of headers for it.
-        # Code page names from https://docs.microsoft.com/en-gb/windows/desktop/Intl/code-page-identifiers
-        # Retrieved on 2020-12-18
-        allowed_codepage_nums = set([37, 437, 500, 708, 709, 710, 720, 737, 775, 850, 852, 855, 857, 858, 860, 861, 862, 863, 864, 865, 866, 869, 870, 874, 875, 932, 936, 949, 950, 1026, 1047, 1140, 1141, 1142, 1143, 1144, 1145, 1146, 1147, 1148, 1149, 1200, 1201, 1250, 1251, 1252, 1253, 1254, 1255, 1256, 1257, 1258, 1361, 10000, 10001, 10002, 10003, 10004, 10005, 10006, 10007, 10008, 10010, 10017, 10021, 10029, 10079, 10081, 10082, 12000, 12001, 20000, 20001, 20002, 20003, 20004, 20005, 20105, 20106, 20107, 20108, 20127, 20261, 20269, 20273, 20277, 20278, 20280, 20284, 20285, 20290, 20297, 20420, 20423, 20424, 20833, 20838, 20866, 20871, 20880, 20905, 20924, 20932, 20936, 20949, 21025, 21027, 21866, 28591, 28592, 28593, 28594, 28595, 28596, 28597, 28598, 28599, 28603, 28605, 29001, 38598, 50220, 50221, 50222, 50225, 50227, 50229, 50930, 50931, 50933, 50935, 50936, 50937, 50939, 51932, 51936, 51949, 51950, 52936, 54936, 57002, 57003, 57004, 57005, 57006, 57007, 57008, 57009, 57010, 57011, 65000, 65001])
-        charset_check = re.compile(r'\\ansicpg([0-9]+)')
-        main_headers = self._get_header_control_words_before_first_group()
-        for unicode_charset in main_headers:
-            cmatch = charset_check.match(unicode_charset.strip())
-            if cmatch is not None:
-                codepage_num = int(cmatch.groups()[0])
-                if codepage_num in allowed_codepage_nums:
-                    return codepage_num
-                else:
-                    raise MalformedRtf("Unsupported unicode codepage number `{}` found in the header".format(codepage_num))
-
-        log.debug("No unicode codepage number found in the header. The following headers were checked: {0}".format(main_headers))
-        raise MalformedRtf("No unicode codepage number found in the header")
-
-    def _get_python_codec(self) -> str:
-        """Returns the python codec needed to decode bytes to unicode.
-        """
-        _codepage_num = self._get_codepage_num()
-        text_codec = codepages.codepage2codec(_codepage_num)
-        log.debug('Found python codec corresponding to code page {0}: {1}'.format(_codepage_num, text_codec))
-        return text_codec
-
-    def _validate_FROM_in_doc_header(self):
+    def validate_FROM_in_doc_header(self):
         """Inspect the header to identify what type of content (html/plain text) is encapsulated within the document.
 
-        NOTE: The de-encapsulating RTF reader inspects no more than the first 10 RTF tokens (that is, begin group marks and control words) in the input RTF document, in sequence, starting from the beginning of the RTF document. If one of the control words is the FROMHTML control word, the de-encapsulating RTF reader will conclude that the RTF document contains an encapsulated HTML document and stop further inspection. If one of the control words is the FROMTEXT control word, the de-encapsulating RTF reader concludes that the RTF document was produced from a plain text document and stops further inspection. - MS-OXRTFEX
+NOTE: The de-encapsulating RTF reader inspects no more than the first 10 RTF tokens (that is, begin group marks and control words) in the input RTF document, in sequence, starting from the beginning of the RTF document. If one of the control words is the FROMHTML control word, the de-encapsulating RTF reader will conclude that the RTF document contains an encapsulated HTML document and stop further inspection. If one of the control words is the FROMTEXT control word, the de-encapsulating RTF reader concludes that the RTF document was produced from a plain text document and stops further inspection. - MS-OXRTFEX
+
+Raises:
+        MalformedEncapsulatedRtf: The .rtf headers are malformed.
+        NotEncapsulatedRtf: The .rtf object is missing an encapsulated content type header. Which means that it is likely just a regular .rtf file.
         """
         cw_found = {"rtf1":False,
                     "from":False,
                     "fonttbl":False,
                     "malformed":False}
         # The de-encapsulating RTF reader SHOULD inspect no more than the first 10 RTF tokens (that is, begin group marks and control words) in the input RTF document, in sequence, starting from the beginning of the RTF document. This means more than just control words.
-        first_ten_tokens = self.doc_tree.children[:10]
+        decoded_tree = StripControlWords().transform(self.doc_tree)
+        first_ten_tokens = decoded_tree.children[:10]
         operating_tokens = []
         found_token = None
         for token in first_ten_tokens:
             if isinstance(token, Token):
                 operating_tokens.append(token)
             else:
-                operating_tokens += [i for i in token.scan_values(lambda t: t.type in ('CONTROLWORD'))]
-        log.debug("Header tokens being evaluated: {0}".format(operating_tokens))
+                operating_tokens += list(token.scan_values(lambda t: t.type == 'CONTROLWORD'))
+        if is_logger_on("RTFDE.validation_logger") is True:
+            log_validators(f"Header tokens being evaluated: {operating_tokens}")
 
         for token in operating_tokens:
-            cw_found,found_token = self._check_from_token(token=token, cw_found=cw_found)
+            cw_found,found_token = self.check_from_token(token=token, cw_found=cw_found)
             if cw_found['from'] is True and cw_found["malformed"] is True:
                 raise MalformedEncapsulatedRtf("RTF file looks like is was supposed to be encapsulated HTML/TEXT but the headers are malformed. Turn on debugging to see specific information")
             # Save content type token available for id-ing type of content later
             if found_token is not None:
-                self._content_type_token = found_token
+                self.content_type_token = found_token
 
         if cw_found['from'] is False:
             log.debug("FROMHTML/TEXT control word not found in first 10 RTF tokens. This is not an HTML/TEXT encapsulated RTF document.")
             raise NotEncapsulatedRtf("FROMHTML/TEXT control word not found.")
 
-    def _get_font_table(self) -> Tree:
-        """Extract the font table group from the document"""
-        for token in self.doc_tree.children[:20]:
-            if isinstance(token, Tree):
-                table_type = token.children[1].value
-                if table_type == "\\fonttbl":
-                    return token
-
     @staticmethod
-    def _check_from_token(token, cw_found:dict) -> dict:
-        """Checks if fromhtml1 or fromtext tokens are in the proper place in the header based on the state passed to it by the _validate_FROM_in_doc_header function.
+    def check_from_token(token:Token, cw_found:dict) -> Tuple[Dict,Union[None,str]] :
+        """Checks if fromhtml1 or fromtext tokens are in the proper place in the header based on the state passed to it by the validate_FROM_in_doc_header function.
+
+Args:
+        token: The token to check for in the cw_found state dictionary.
+        cw_found: The state dictionary which is used to track the position of the from token within the header.
+
+        `cw_found = {"rtf1":<BOOL>, "from":<BOOL>, "fonttbl":<BOOL>, "malformed":<BOOL>}`
+
+
+Returns:
+        cw_found: Updated state dictionary
+        found_token: The content_type_token found in the header.
 
-        Parameters:
-            cw_found: (dict): The state dictionary which is used to track the position of the from token within the header
-                `cw_found = {"rtf1":<BOOL>, "from":<BOOL>, "fonttbl":<BOOL>, "malformed":<BOOL>}`
         """
-        from_cws = ['\\fromhtml1', '\\fromtext']
+        from_cws = [b'\\fromhtml1', b'\\fromtext']
         # This control word MUST appear before the \fonttbl control word and after the \rtf1 control word, as specified in [MSFT-RTF].
-        rtf1_cw = "\\rtf1"
+        rtf1_cw = b"\\rtf1"
         found_token = None
-        fonttbl_cw = "\\fonttbl"
-        maltype = []
+        fonttbl_cw = b"\\fonttbl"
         if token.type == "CONTROLWORD":
-            if token.value in from_cws:
+            if token.value.strip() in from_cws:
                 if cw_found['from'] is True:
                     cw_found["malformed"] = True
                     log.debug("Multiple FROM HTML/TXT tokens found in the header. This encapsulated RTF is malformed.")
                 if cw_found['rtf1'] is True:
                     cw_found['from'] = True
                     found_token = token.value
                 else:
                     log.debug("FROMHTML/TEXT control word found before rtf1 control word. That's not allowed in the RTF spec.")
                     cw_found['from'] = True
                     cw_found["malformed"] = True
-            elif token.value == rtf1_cw:
+            elif token.value.strip() == rtf1_cw:
                 cw_found['rtf1'] = True
-            elif token.value == fonttbl_cw:
+            elif token.value.strip() == fonttbl_cw:
                 cw_found['fonttbl'] = True
-                if cw_found['from'] != True:
+                if cw_found['from'] is not True:
                     log.debug("\\fonttbl code word found before FROMTML/TEXT was defined. This is not allowed for encapsulated HTML/TEXT. So... this is not encapsulated HTML/TEXT or it was badly encapsulated.")
                     cw_found["malformed"] = True
         return cw_found, found_token
 
 
-    def _validate_rtf_doc_header(self):
+    @staticmethod
+    def validate_rtf_doc_header(doc_tree: Tree):
         """Check if doc starts with a valid RTF header `\\rtf1`.
 
-        "Before the de-encapsulating RTF reader tries to recognize the encapsulation, the reader SHOULD ensure that the document has a valid RTF document heading according to [MSFT-RTF] (that is, it starts with the character sequence "{\rtf1")." - MS-OXRTFEX
-        """
-        first_token = self.doc_tree.children[0].value
-        if first_token != "\\rtf1":
+        "Before the de-encapsulating RTF reader tries to recognize the encapsulation, the reader SHOULD ensure that the document has a valid RTF document heading according to [MSFT-RTF] (that is, it starts with the character sequence "{\\rtf1")." - MS-OXRTFEX
+
+Raises:
+        MalformedRtf: The .rtf headers do not include \\rtf1.
+"""
+        first_token = doc_tree.children[0].value
+        if first_token != b"\\rtf1":
             log.debug("RTF stream does not contain valid valid RTF document heading. The file must start with \"{\\rtf1\"")
-            raise MalformedRtf("RTF stream does not start with {rtf1")
+            if is_logger_on("RTFDE.validation_logger") is True:
+                log_validators(f"First child object in document tree is: {first_token!r}")
+            raise MalformedRtf("RTF stream does not start with {\\rtf1")
+
+    @staticmethod
+    def catch_common_validation_issues(raw_rtf: AnyStr):
+        """Checks for likely common valid input mistakes that may occur when folks try to use this library and raises exceptions to try and help identify them.
+
+Args:
+        raw_rtf: A raw .rtf string or byte-string.
+
+Raises:
+        TypeError: The data passed is the wrong type of data.
+        MalformedRtf: The data passed is not a correctly formatted .rtf string.
+"""
+        if isinstance(raw_rtf, BufferedReader):
+            raise TypeError("Data passed as file pointer. DeEncapsulator only accepts byte objects.")
+        if raw_rtf is None:
+            raise TypeError("Data passed as raw RTF file is a null object `None` keyword.")
+        if raw_rtf[:8] == b"\xd0\xcf\x11\xe0\xa1\xb1\x1a\xe1":
+            raise TypeError("Data passed is a full MSG object. You must extract the encapsulated RTF body first.")
+        if raw_rtf in (b'', ''):
+            raise MalformedRtf("Data passed as raw RTF file is an empty string.")
```

### Comparing `RTFDE-0.0.2/RTFDE/exceptions.py` & `RTFDE-0.1.0/RTFDE/exceptions.py`

 * *Files identical despite different names*

### Comparing `RTFDE-0.0.2/RTFDE.egg-info/PKG-INFO` & `RTFDE-0.1.0/RTFDE.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,100 @@
 Metadata-Version: 2.1
 Name: RTFDE
-Version: 0.0.2
+Version: 0.1.0
 Summary: A library for extracting HTML content from RTF encapsulated HTML as commonly found in the exchange MSG email format.
 Home-page: https://github.com/seamustuohy/RTFDE
 Author: seamus tuohy
 Author-email: code@seamustuohy.com
-License: UNKNOWN
-Description: # RTFDE: RTF De-Encapsulator
-        
-        A python3 library for extracting encapsulated `HTML` & `plain text` content from the `RTF` bodies of .msg files.
-        
-        De-encapsulation enables previously encapsulated HTML and plain text content to be extracted and rendered as HTML and plain text instead of the encapsulating RTF content. After de-encapsulation, the HTML and plain text should differ only minimally from the original HTML or plain text content.
-        
-        # Features
-        
-        - De-encapsulate HTML from RTF encapsulated HTML.
-        - De-encapsulate plain text from RTF encapsulated text.
-        
-        # Known Issues
-        
-        - This library *fully* unquotes text it de-encapsulates because it does not know which text was quoted in the RTF conversion process and which text was quoted in the original html/text. So, for instance escaped [Quoted-Printable](https://en.wikipedia.org/wiki/Quoted-printable) text will be returned un-escaped.
-        - This library currently can't [combine attachments](https://docs.microsoft.com/en-us/openspecs/exchange_server_protocols/ms-oxrtfex/b518f0bc-468c-4218-87a7-8f8859bf5773) from a .MSG Message object with the de-encapsulated HTML. This is mostly because I could not get a good set of examples of encapsulated HTML which had attachment objects that needed to be integrated back into the body of the HTML.
-        
-        # Anti-Features (I don't intend to have this library do this.)
-        
-        - Extract plain text from RTF encapsulated HTML. If you want this, then you will have to parse the HTML using another library.
-        
-        # Installation
-        
-        **To install from the pip package.**
-        
-        ```
-        pip3 install RTFDE
-        
-        ```
-        
-        # Usage
-        
-        ## De-encapsulating HTML or TEXT
-        
-        ```python
-        from RTFDE.deencapsulate import DeEncapsulator
-        
-        with open('rtf_file', 'r') as fp:
-            raw_rtf  = fp.read()
-            rtf_obj = DeEncapsulator(raw_rtf)
-            rtf_obj.deencapsulate()
-            if rtf_obj.content_type == 'html':
-                print(rtf_obj.html)
-            else:
-                print(rtf_obj.text)
-        ```
-        
-        # Contribute
-        
-        Please check the [contributing guidelines](./CONTRIBUTING.md)
-        
-        # License
-        
-        Please see the [license file](./LICENSE) for license information on RTFDE. If you have further questions related to licensing PLEASE create an issue about it on github.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Communications :: Email :: Filters
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: msg_parse
+Provides-Extra: dev
+License-File: LICENSE
+
+# RTFDE: RTF De-Encapsulator
+
+A python3 library for extracting encapsulated `HTML` & `plain text` content from the `RTF` bodies of .msg files.
+
+De-encapsulation enables previously encapsulated HTML and plain text content to be extracted and rendered as HTML and plain text instead of the encapsulating RTF content. After de-encapsulation, the HTML and plain text should differ only minimally from the original HTML or plain text content.
+
+# Features
+
+- De-encapsulate HTML from RTF encapsulated HTML.
+- De-encapsulate plain text from RTF encapsulated text.
+
+# Known Issues
+
+- This library *fully* unquotes text it de-encapsulates because it does not know which text was quoted in the RTF conversion process and which text was quoted in the original html/text. So, for instance escaped [Quoted-Printable](https://en.wikipedia.org/wiki/Quoted-printable) text will be returned un-escaped.
+- This library currently can't [combine attachments](https://docs.microsoft.com/en-us/openspecs/exchange_server_protocols/ms-oxrtfex/b518f0bc-468c-4218-87a7-8f8859bf5773) from a .MSG Message object with the de-encapsulated HTML. This is mostly because I could not get a good set of examples of encapsulated HTML which had attachment objects that needed to be integrated back into the body of the HTML.
+
+# Anti-Features (I don't intend to have this library do this.)
+
+- Extract plain text from RTF encapsulated HTML. If you want this, then you will have to parse the HTML using another library.
+
+# Installation
+
+**To install from the pip package.**
+
+```
+pip3 install RTFDE
+
+```
+
+# Usage
+
+## De-encapsulating HTML or TEXT
+
+```python
+from RTFDE.deencapsulate import DeEncapsulator
+
+with open('rtf_file', 'rb') as fp:
+    raw_rtf  = fp.read()
+    rtf_obj = DeEncapsulator(raw_rtf)
+    rtf_obj.deencapsulate()
+    if rtf_obj.content_type == 'html':
+        print(rtf_obj.html)
+    else:
+        print(rtf_obj.text)
+```
+
+
+
+# Enabling Logging
+
+Any logging (including how verbose the logging is) can be handled by configuring logging. You can enable RTFDE's logging at the highest level by getting and setting the "RTFDE" logger.
+
+```
+log = logging.getLogger("RTFDE")
+log.setLevel(logging.INFO)
+```
+
+
+
+
+
+
+To see how to enable more in-depth logging for debugging check out the CONTRIBUTING.md file.
+
+```
+# Now, get the log that you want
+# The main logger is simply called RTFDE. That will get you all the *normal* logs.
+requests_log = logging.getLogger("RTFDE")
+requests_log.setLevel(logging.DEBUG)
+requests_log.propagate = True
+```
+
+
+# Contribute
+
+Please check the [contributing guidelines](./CONTRIBUTING.md)
+
+# License
+
+Please see the [license file](./LICENSE) for license information on RTFDE. If you have further questions related to licensing PLEASE create an issue about it on github.
```

### Comparing `RTFDE-0.0.2/setup.py` & `RTFDE-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="RTFDE",
-    version="0.0.2",
+    version="0.1.0",
     author="seamus tuohy",
     author_email="code@seamustuohy.com",
     description="A library for extracting HTML content from RTF encapsulated HTML as commonly found in the exchange MSG email format.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/seamustuohy/RTFDE",
     packages=setuptools.find_packages(),
@@ -19,11 +19,15 @@
         "Operating System :: OS Independent",
         "Topic :: Text Processing :: Markup :: HTML",
         "Intended Audience :: Developers",
         "Topic :: Text Processing :: Filters",
         "Topic :: Communications :: Email :: Filters"
     ],
     python_requires='>=3.6',
-    install_requires=['lark-parser>=0.11', 'oletools>=0.56'],
+    install_requires=['lark==1.1.5',
+                      'oletools>=0.56'],
     extras_require={'msg_parse': ['extract_msg>=0.27'],
-                    'dev': ['lxml>=4.6']}
+                    'dev': ['lxml>=4.6',
+                            'mypy>=1.1.1',
+                            'pdoc3>=0.10.0',
+                            'coverage>=7.2.2']}
 )
```

### Comparing `RTFDE-0.0.2/tests/parse_rtf/test_parse_rtf.py` & `RTFDE-0.1.0/tests/parse_rtf/test_parse_rtf.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,18 +4,24 @@
 - Correct RTF data doesn't raise any errors.
 - Malformed RTF data fails to parse and is described helpfully
 - Malformed encapsulated RTF data fails to parse and is described helpfully
 - RTF parsing captures the correct data
 """
 
 import unittest
+import logging
 from os.path import join
 from RTFDE.exceptions import MalformedRtf, MalformedEncapsulatedRtf, NotEncapsulatedRtf
 from RTFDE.deencapsulate import DeEncapsulator
+from RTFDE.utils import encode_escaped_control_chars
+from RTFDE.text_extraction import get_python_codec
+from RTFDE.text_extraction import TextDecoder
+
 from tests.test_utils import DATA_BASE_DIR
+from lark import logger as lark_logger
 
 class TestParseRtf(unittest.TestCase):
     """Test proper parsing of RTF files
 
 Ensure that:
     - Correct RTF data doesn't raise any errors.
     - Malformed RTF data fails to parse and is described helpfully
@@ -26,260 +32,275 @@
 
     def test_get_first_20_header_control_words(self):
         """ Check that _get_header_control_words__before_first_group gets the first 20 control words of the RTF data or all the tokens which occur before the first group (whichever comes first.)"""
         template_path =  join(DATA_BASE_DIR,
                                           "rtf_parsing",
                                           "from_header_template.rtf")
         # Has 20 control words
-        ctrl_words = ("\\deff0"*16) + "\\fromhtml1"
-        rtf = self.replace_from_header(template_path, ctrl_words)
+        ctrl_words = (b"\\deff0"*16) + b"\\fromhtml1"
+        rtf = self.replace_text_in_template(template_path, ctrl_words)
         output = self.run_parsing(rtf)
-        ctrl_wds = output._get_header_control_words_before_first_group()
-        ctrl_wds =[i.value for i in ctrl_wds]
-        correct_ctrl = ['\\rtf1', '\\ansi', '\\ansicpg1252', '\\deff0', '\\deff0', '\\deff0',
-                        '\\deff0', '\\deff0', '\\deff0', '\\deff0', '\\deff0', '\\deff0',
-                        '\\deff0', '\\deff0', '\\deff0', '\\deff0', '\\deff0', '\\deff0',
-                        '\\deff0', '\\fromhtml1']
+        ctrl_wds = output.get_header_control_words_before_first_group()
+        ctrl_wds =[i.value.strip() for i in ctrl_wds]
+        correct_ctrl = [b'\\rtf1',
+                        b'\\ansi',
+                        b'\\ansicpg1252',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\deff0',
+                        b'\\fromhtml1']
         self.assertEqual(ctrl_wds, correct_ctrl)
 
         # group comes before 20 control words
-        ctrl_words = ("\\deff0"*5) + "\\fromhtml1 \\deff0" + '{\colortbl\red0\green0\blue0;\red5\green99\blue193;}'
-        rtf = self.replace_from_header(template_path, ctrl_words)
+        ctrl_words = (b"\\deff0"*5) + b"\\fromhtml1 \\deff0" + b'{\colortbl\red0\green0\blue0;\red5\green99\blue193;}'
+        rtf = self.replace_text_in_template(template_path, ctrl_words)
         output = self.run_parsing(rtf)
-        ctrl_wds = output._get_header_control_words_before_first_group()
-        ctrl_wds = [i.value for i in ctrl_wds]
-        correct_ctrl = ['\\rtf1', '\\ansi', '\\ansicpg1252', '\\deff0', '\\deff0', '\\deff0', '\\deff0', '\\deff0', '\\fromhtml1', '\\deff0']
+        ctrl_wds = output.get_header_control_words_before_first_group()
+        ctrl_wds = [i.value.strip() for i in ctrl_wds]
+        correct_ctrl = [b'\\rtf1', b'\\ansi', b'\\ansicpg1252', b'\\deff0', b'\\deff0', b'\\deff0', b'\\deff0', b'\\deff0', b'\\fromhtml1', b'\\deff0']
         self.assertEqual(ctrl_wds, correct_ctrl)
 
         # fromhtml header parsing not affected by this function
-        ctrl_words = '{\\colortbl\\red0\\green0\\blue0;\\red5\\green99\\blue193;}' + "\\fromhtml1 \\deff0"
-        rtf = self.replace_from_header(template_path, ctrl_words)
+        ctrl_words = b'{\\colortbl\\red0\\green0\\blue0;\\red5\\green99\\blue193;}' + b"\\fromhtml1 \\deff0"
+        rtf = self.replace_text_in_template(template_path, ctrl_words)
         # The fromhtml header needs to be in the first 10 tokens. Tokens includes groups in this case. So this should succeed.
         self.check_deencapsulate_validity(rtf,
                                           expect_error=None,
                                           name="group before fromhtml in header")
 
     def test_codepage_num(self):
         template_path =  join(DATA_BASE_DIR,
                               "rtf_parsing",
                               "from_header_template.rtf")
 
         # bad
-        bad_charsets = ["\\ansicpg1234", "\\pccpg1252", "\\ansicpg"]
+        bad_charsets = [b"\\ansicpg1234", b"\\ansicpg"]
         for badchar in bad_charsets:
-            rtf = self.replace_from_header(template_path, "\\fromhtml1")
-            rtf = self.replace_from_header(None, badchar, rep_str="\\ansicpg1252", string=rtf)
+            rtf = self.replace_text_in_template(template_path, b"\\fromhtml1")
+            rtf = self.replace_text_in_template(None, badchar, rep_str=b"\\ansicpg1252", string=rtf)
             self.check_deencapsulate_validity(rtf,
                                               expect_error=MalformedRtf,
                                               name="bad codepage keyword: {0}".format(badchar))
 
         # good
         # Supported code pages from https://github.com/decalage2/oletools/blob/master/oletools/common/codepages.py
         # Retrieved on 2020-12-18
         # Doesn't include when it attempts to pull the cpNNN codepage from python
         # utf8 (65001) codepage removed so we can check against fallback to utf8
         # NOTE: oletools supports some codepages which MS doesn't include so those are not included here: (32768, 32769)
         supported_codepage_nums = [37, 708, 709, 710, 870, 1047, 1141, 1201, 10000, 10001, 10002, 10003, 10004, 10005, 10006, 10007, 10008, 10021, 10029, 10079, 10081, 12000, 12001, 20127, 28591, 28592, 28593, 28594, 28595, 28596, 28597, 28598, 28599, 28603, 28605, 38598, 65000]
         for goodpg in supported_codepage_nums:
-            rtf = self.replace_from_header(template_path, "\\fromhtml1")
-            good_codepage = "\\ansicpg{0}".format(goodpg)
-            rtf = self.replace_from_header(None, good_codepage, rep_str="\\ansicpg1252", string=rtf)
-            output = self.run_parsing(rtf)
-            output._validate_encapsulation()
-            codec = output._get_python_codec()
+            codec = get_python_codec(goodpg)
             self.assertIsInstance(codec, str)
             self.assertNotEqual(codec, 'utf8')
 
-        # missing
-        rtf = self.replace_from_header(template_path, "\\fromhtml1")
-        rtf = self.replace_from_header(None, "", rep_str="\\ansicpg1252", string=rtf)
+        # Codepage is optional. Therefore a missing codepage number is fine.
+        rtf = self.replace_text_in_template(template_path, b"\\fromhtml1")
+        rtf = self.replace_text_in_template(None, b"", rep_str=b"\\ansicpg1252", string=rtf)
         self.check_deencapsulate_validity(rtf,
-                                          expect_error=MalformedRtf,
-                                          name="Missing codepage num")
+                                          expect_error=None,
+                                          name="Ansi codepage num is optional")
 
     def test_charset_header(self):
         template_path =  join(DATA_BASE_DIR,
                               "rtf_parsing",
                               "from_header_template.rtf")
 
         # Bad charset
-        bad_charsets = ["\\ANSI", "ansi", "\\PC", "\\osx"]
+        bad_charsets = [b"\\ANSI", b"ansi", b"\\PC", b"\\osx"]
         for badchar in bad_charsets:
-            rtf = self.replace_from_header(template_path, "\\fromhtml1")
-            rtf = self.replace_from_header(None, badchar, rep_str="\\ansi", string=rtf)
+            rtf = self.replace_text_in_template(template_path, b"\\fromhtml1")
+            rtf = self.replace_text_in_template(None, badchar, rep_str=b"\\ansi", string=rtf)
             self.check_deencapsulate_validity(rtf,
                                               expect_error=MalformedRtf,
                                               name="bad charset keyword: {0}".format(badchar))
 
         # Good charset
         # included \\ after the charset keyword to ensure we don't capture the \\ansicpg
-        good_charsets = ["\\ansi\\", "\\mac\\", "\\pc\\", "\\pac\\"]
+        good_charsets = [b"\\ansi\\", b"\\mac\\", b"\\pc\\", b"\\pca\\"]
         for goodchar in good_charsets:
-            rtf = self.replace_from_header(template_path, "\\fromhtml1")
-            rtf = self.replace_from_header(None, goodchar, rep_str="\\ansi\\", string=rtf)
+            rtf = self.replace_text_in_template(template_path, b"\\fromhtml1")
+            rtf = self.replace_text_in_template(None, goodchar, rep_str=b"\\ansi\\", string=rtf)
             self.check_deencapsulate_validity(rtf,
                                               expect_error=None,
                                               name="Good charset keyword: {0}".format(goodchar))
 
         # group before charset
-        new_front = '{\\rtf1{\\colortbl\\red0\\green0\\blue0;\\red5\\green99\\blue193;}'
-        rtf = self.replace_from_header(template_path, "\\fromhtml1")
+        new_front = b'{\\rtf1{\\colortbl\\red0\\green0\\blue0;\\red5\\green99\\blue193;}'
+        rtf = self.replace_text_in_template(template_path, b"\\fromhtml1")
         rtf = new_front + rtf[6:] # Replaces `{\\rtf1`
         self.check_deencapsulate_validity(rtf,
                                           expect_error=MalformedRtf,
                                           name="no groups before charset")
 
         # Missing
-        rtf = self.replace_from_header(template_path, "\\fromhtml1")
-        rtf = self.replace_from_header(None, "\\", rep_str="\\ansi\\", string=rtf)
+        rtf = self.replace_text_in_template(template_path, b"\\fromhtml1")
+        rtf = self.replace_text_in_template(None, b"\\", rep_str=b"\\ansi\\", string=rtf)
         self.check_deencapsulate_validity(rtf,
                                           expect_error=MalformedRtf,
                                           name="missing charset")
         # Test missing using default fallback to ansi
         output = self.run_parsing(rtf)
-        output._validate_encapsulation()
-        charset = output._get_charset(fallback_to_default=True)
-        self.assertEqual("\\ansi", charset)
+        charset = output.validate_charset(fallback_to_default=True)
+        self.assertEqual(b"\\ansi", charset)
 
     def test_get_python_codec(self):
         """Test getting correct python codec."""
         template_path =  join(DATA_BASE_DIR,
                               "rtf_parsing",
                               "from_header_template.rtf")
-        base = self.replace_from_header(template_path, "\\fromhtml1")
+        base = self.replace_text_in_template(template_path, b"\\fromhtml1")
         # Big-5
         big5string = b'\xb3o\xacO\xa4@\xad\xd3\xa4\xe5\xa5\xbb\xa6r\xb2\xc5\xa6\xea\xa1C'
-        rtf = self.replace_from_header(None,
-                                       replacement="\\ansicpg10002",
-                                       rep_str="\\ansicpg1252",
+        rtf = self.replace_text_in_template(None,
+                                       replacement=b"\\ansicpg10002",
+                                       rep_str=b"\\ansicpg1252",
                                        string=base)
 
         output = self.run_parsing(rtf)
-        output._validate_encapsulation()
-        output.charset = output._get_charset()
-        output.text_codec = output._get_python_codec()
-        big5string.decode(output.text_codec)
-        self.assertEqual(output.text_codec, "big5")
-        self.assertEqual(big5string.decode(output.text_codec),
+        # output.validate_encapsulation()
+        # charset = output._validate_charset()
+        ansicpg_header = output.get_ansicpg_header()
+        possible_cpg_num = int(ansicpg_header.value.strip()[8:])
+        text_codec = get_python_codec(possible_cpg_num)
+        big5string.decode(text_codec)
+        self.assertEqual(text_codec, "big5")
+        self.assertEqual(big5string.decode(text_codec),
                          '這是一個文本字符串。')
         # Hebrew
         hebrew = b'\xe6\xe4\xe5 \xee\xe7\xf8\xe5\xe6\xfa \xe8\xf7\xf1\xe8.'
-        rtf = self.replace_from_header(None,
-                                       replacement="\\ansicpg10005",
-                                       rep_str="\\ansicpg1252",
+        rtf = self.replace_text_in_template(None,
+                                       replacement=b"\\ansicpg10005",
+                                       rep_str=b"\\ansicpg1252",
                                        string=base)
         output = self.run_parsing(rtf)
-        output._validate_encapsulation()
-        output.charset = output._get_charset()
-        output.text_codec = output._get_python_codec()
-        self.assertEqual(output.text_codec, "hebrew")
-        self.assertEqual(hebrew.decode(output.text_codec), "זהו מחרוזת טקסט.")
+        ansicpg_header = output.get_ansicpg_header()
+        possible_cpg_num = int(ansicpg_header.value.strip()[8:])
+        text_codec = get_python_codec(possible_cpg_num)
+        self.assertEqual(text_codec, "hebrew")
+        self.assertEqual(hebrew.decode(text_codec), "זהו מחרוזת טקסט.")
 
 
     def test_from_header_html(self):
         """ check that a basic fromhtml header works."""
         from_html =  join(DATA_BASE_DIR,
                           "rtf_parsing",
                           "from_header_template.rtf")
-        rtf = self.replace_from_header(from_html, "\\fromhtml1")
+        rtf = self.replace_text_in_template(from_html, b"\\fromhtml1")
         self.check_deencapsulate_validity(rtf,
                                           expect_error=None,
                                           name="working fromheaderhtml")
 
-
     def test_from_header_text(self):
         """Check that a basic fromtext header works."""
         from_text =  join(DATA_BASE_DIR,
                           "rtf_parsing",
                           "from_header_template.rtf")
-        rtf = self.replace_from_header(from_text, "\\fromtext")
+        rtf = self.replace_text_in_template(from_text, b"\\fromtext")
         self.check_deencapsulate_validity(rtf,
                                           expect_error=None,
                                           name="working fromheader text")
 
     def test_missing_from_header(self):
         """Ensure that if a from header isn't present we don't parse the file."""
         missing_from =  join(DATA_BASE_DIR,
                              "rtf_parsing",
                              "from_header_template.rtf")
-        rtf = self.replace_from_header(missing_from, "")
+        rtf = self.replace_text_in_template(missing_from, b"")
         self.check_deencapsulate_validity(rtf,
                                           expect_error=NotEncapsulatedRtf,
                                           name="missing fromheader text")
 
         missing_but_one_in_body =  join(DATA_BASE_DIR,
                                      "rtf_parsing",
                                      "from_header_template.rtf")
-        rtf = self.replace_from_header(missing_but_one_in_body, "")
-        rtf = self.replace_from_header(None, "\\fromtext",
-                                       rep_str="INSERT_BODY_TEXT_HERE",
+        rtf = self.replace_text_in_template(missing_but_one_in_body, b"")
+        rtf = self.replace_text_in_template(None, b"\\fromtext",
+                                       rep_str=b"INSERT_BODY_TEXT_HERE",
                                        string=rtf)
         self.check_deencapsulate_validity(rtf,
                                           expect_error=NotEncapsulatedRtf,
                                           name="Missing from header, but one far later.")
 
     def test_multiple_from_headers(self):
         """Test what happens when you have multiple FROM (fromhtml1 or fromtext) headers."""
         multiple_from_html =  join(DATA_BASE_DIR,
                                    "rtf_parsing",
                                    "from_header_template.rtf")
-        rtf = self.replace_from_header(multiple_from_html, "\\fromhtml1\\fromhtml1")
+        rtf = self.replace_text_in_template(multiple_from_html, b"\\fromhtml1\\fromhtml1")
         self.check_deencapsulate_validity(rtf,
                                           expect_error=MalformedEncapsulatedRtf,
                                           name="multiple FROM headers means malformed")
 
         multiple_from_html_first =  join(DATA_BASE_DIR,
                                          "rtf_parsing",
                                          "from_header_template.rtf")
-        rtf = self.replace_from_header(multiple_from_html_first, "\\fromhtml1\\fromtext")
+        rtf = self.replace_text_in_template(multiple_from_html_first, b"\\fromhtml1\\fromtext")
         self.check_deencapsulate_validity(rtf,
                                           expect_error=MalformedEncapsulatedRtf,
                                           name="multiple FROM headers means malformed")
 
         multiple_from_txt_first =  join(DATA_BASE_DIR,
                                         "rtf_parsing",
                                         "from_header_template.rtf")
-        rtf = self.replace_from_header(multiple_from_txt_first, "\\fromtext\\fromhtml1")
+        rtf = self.replace_text_in_template(multiple_from_txt_first, b"\\fromtext\\fromhtml1")
         self.check_deencapsulate_validity(rtf,
                                           expect_error=MalformedEncapsulatedRtf,
                                           name="multiple FROM headers means malformed")
 
     def test_from_header_before_rtf(self):
         """Check that this fails. """
         missing_from =  join(DATA_BASE_DIR,
                              "rtf_parsing",
                              "from_header_template.rtf")
-        rtf = self.replace_from_header(missing_from, "")
+        rtf = self.replace_text_in_template(missing_from, b"")
         # Append a new curly and the control word to the start of the rtf file
-        rtf = "{\\fromhtml1" + rtf[1:]
+        # TODO: Fix this array use on a bytes object
+        rtf = b"{\\fromhtml1" + rtf[1:]
         self.check_deencapsulate_validity(rtf,
                                           expect_error=MalformedRtf,
                                           name="from header before magic")
 
     def test_broken_magic(self):
         """Ensure that if a from header is before rtf1 that we fail."""
         missing_from =  join(DATA_BASE_DIR,
                              "rtf_parsing",
                              "from_header_template.rtf")
-        rtf = self.replace_from_header(missing_from, "\\fromhtml1")
+        rtf = self.replace_text_in_template(missing_from, b"\\fromhtml1")
         # Append a new curly and broken rtf to the start of the rtf file
-        rtf_no_one = "{\\rtf" + rtf[6:] # Removes `{\\rtf1`
+        # TODO: Fix this array use on a bytes object
+        rtf_no_one = b"{\\rtf" + rtf[6:] # Removes `{\\rtf1`
         self.check_deencapsulate_validity(rtf_no_one,
                                           expect_error=MalformedRtf,
                                           name="malformed file magic")
-
-        rtf_two = "{\\rtf2" + rtf[6:]
+        # TODO: Fix this array use on a bytes object
+        rtf_two = b"{\\rtf2" + rtf[6:]
         self.check_deencapsulate_validity(rtf_two,
                                           expect_error=MalformedRtf,
                                           name="malformed file magic")
-        RTF = "{\\RTF1" + rtf[6:]
+        # TODO: Fix this array use on a bytes object
+        RTF = b"{\\RTF1" + rtf[6:]
         self.check_deencapsulate_validity(RTF,
                                           expect_error=MalformedRtf,
                                           name="malformed file magic")
-        PiRTF = "{\\ARRRRRR-TEEE-FFF" + rtf[6:] # Because Pirates
+        # TODO: Fix this array use on a bytes object
+        PiRTF = b"{\\ARRRRRR-TEEE-FFF" + rtf[6:] # Because Pirates
         self.check_deencapsulate_validity(PiRTF,
                                           expect_error=MalformedRtf,
                                           name="Ahoy, matey! this here file magic be broken")
 
 
     def test_fonttble_too_early(self):
         """fail when fonttable is before the fromhtml keyword
@@ -287,77 +308,191 @@
         - correctly extract the header type
         - with multiple header vals (one in header and one string later on)
         """
         template_path =  join(DATA_BASE_DIR,
                               "rtf_parsing",
                               "from_header_template.rtf")
 
-        early_font_table = '{\\fonttbl\n{\\f0\\fswiss Arial;}\n{\\f1\\fmodern Courier New;}\n{\\f2\\fnil\\fcharset2 Symbol;}\n{\\f3\\fmodern\\fcharset0 Courier New;}}' + "\\fromhtml1 \\deff0"
-        rtf = self.replace_from_header(template_path, early_font_table)
+        early_font_table = b'{\\fonttbl\n{\\f0\\fswiss Arial;}\n{\\f1\\fmodern Courier New;}\n{\\f2\\fnil\\fcharset2 Symbol;}\n{\\f3\\fmodern\\fcharset0 Courier New;}}' + b"\\fromhtml1 \\deff0"
+        rtf = self.replace_text_in_template(template_path, early_font_table)
         self.check_deencapsulate_validity(rtf,
                                           expect_error=MalformedEncapsulatedRtf,
                                           name="fonttable before fromhtml in header")
 
+    def test_missing_fonttable(self):
+        """fail when fonttable is missing"""
+        template_path =  join(DATA_BASE_DIR,
+                              "rtf_parsing",
+                              "font_table_template.rtf")
+
+        no_font_table = b""
+        rtf = self.replace_text_in_template(template_path,
+                                            no_font_table,
+                                            rep_str=b"REPLACE_FONT_TABLE_HERE")
+        NA = b"REPLACE_FONT_TABLE_HERE"
+        default = b"""{\\fonttbl
+{\\f0\\fswiss Arial;}
+{\\f1\\fmodern Courier New;}
+{\\f2\\fnil\\fcharset2 Symbol;}
+{\\f3\\fmodern\\fcharset0 Courier New;}}"""
+        self.check_deencapsulate_validity(rtf,
+                                          expect_error=ValueError,
+                                          name="fonttable Missing")
+                                          # print_error=True)
+
     def test_extracted_correct_from_header(self):
         """
         - correctly extract the header type
         - with multiple header vals (one in header and one string in body of)
         """
         template_data =  join(DATA_BASE_DIR,
                           "rtf_parsing",
                           "from_header_template.rtf")
-        rtf = self.replace_from_header(template_data, "\\fromhtml1")
+        rtf = self.replace_text_in_template(template_data, b"\\fromhtml1")
         output = DeEncapsulator(rtf)
         output.deencapsulate()
         self.assertEqual('html', output.get_content_type())
 
-        rtf = self.replace_from_header(template_data, "\\fromtext")
+        rtf = self.replace_text_in_template(template_data, b"\\fromtext")
         output = DeEncapsulator(rtf)
         output.deencapsulate()
         self.assertEqual('text', output.get_content_type())
 
          # Try with them back to back. First should win.
-        rtf = self.replace_from_header(template_data, "\\fromtext\\fromhtml1")
+        rtf = self.replace_text_in_template(template_data, b"\\fromtext\\fromhtml1")
         self.check_deencapsulate_validity(rtf,
                                           expect_error=MalformedEncapsulatedRtf,
                                           name="multiple FROM headers means malformed")
 
-        rtf = self.replace_from_header(template_data, "\\fromhtml1\\fromtext")
+        rtf = self.replace_text_in_template(template_data, b"\\fromhtml1\\fromtext")
         self.check_deencapsulate_validity(rtf,
                                           expect_error=MalformedEncapsulatedRtf,
                                           name="multiple FROM headers means malformed")
 
+    def test_parse_tilde_control_chars(self):
+        """Correctly parse control chars
+        """
+        path =  join(DATA_BASE_DIR,
+                     "rtf_parsing",
+                     "control_chars.rtf")
+        if path is not None:
+            with open(path, 'rb') as fp:
+                rtf = fp.read()
+        self.check_deencapsulate_validity(rtf,
+                                          expect_error=None,
+                                          name="Parse the tilde the \~ command char.")
 
-    def replace_from_header(self, path, replacement,
-                            rep_str="REPLACE_FROM_HEADER_HERE",
+    def test_parse_spaces_in_own_groups(self):
+        """Correctly parse spaces when in their own groups
+        """
+        path =  join(DATA_BASE_DIR,
+                     "rtf_parsing",
+                     "five_spaces.rtf")
+        if path is not None:
+            with open(path, 'rb') as fp:
+                rtf = fp.read()
+        self.check_deencapsulate_validity(rtf,
+                                          expect_error=None,
+                                          name="Parse spaces in their own groups.")
+        output = DeEncapsulator(rtf)
+        output.deencapsulate()
+        # self.maxDiff = None
+        self.assertEqual(b'INSERT_BODY_TEXT_HERE     ', output.text)
+
+    def test_parse_multiple_features(self):
+        """Correctly parse spaces when in their own groups
+        """
+        path =  join(DATA_BASE_DIR,
+                     "rtf_parsing",
+                     "encapsulated_example.rtf")
+        htmlpath =  join(DATA_BASE_DIR,
+                        "rtf_parsing",
+                        "encapsulated_example.html")
+
+        if path is not None:
+            with open(path, 'rb') as fp:
+                rtf = fp.read()
+        if htmlpath is not None:
+            with open(htmlpath, 'rb') as fp:
+                html = fp.read()
+
+        self.check_deencapsulate_validity(rtf,
+                                          expect_error=None,
+                                          print_error=True,
+                                          name="Test parse multiple features.")
+        self.maxDiff = None
+        output = DeEncapsulator(rtf)
+        output.deencapsulate()
+        # print("RUNNING DIFF")
+        # print(repr(html))
+        # The CR+LF newlines should not match.
+        self.assertNotEqual(html, output.html)
+        # The LF newlines should be replaced.
+        html = html.replace(b'\r\n', b'\n')
+        self.assertEqual(html, output.html)
+
+
+    def debug_error(self, err):
+        print("FOUND ERROR")
+        # print(dir(err))
+        # print(err)
+        # print(err.start)
+        # print(err.considered_rules)
+        # print(err.state)
+        # print(dir(err.state))
+        print("Current stack of tokens")
+        # print(err.state.state_stack)
+        # print(err.state.value_stack)
+        for i in err.state.value_stack:
+            print(i)
+            # print(dir(i))
+            # print(len(i))
+            # print(type(i))
+        # 'lexer', 'parse_conf', 'position', 'state_stack', 'value_stack'
+        print(err.token_history)
+        # print(err.interactive_parser.lexer_thread )
+
+        print("FOUND ERROR DONE")
+        return True
+
+    def replace_text_in_template(self, path, replacement,
+                            rep_str=b"REPLACE_FROM_HEADER_HERE",
                             string=None):
         if path is not None:
-            with open(path, 'r') as fp:
+            with open(path, 'rb') as fp:
                 raw_rtf = fp.read()
         else:
             raw_rtf = string
         rep_rtf = raw_rtf.replace(rep_str, replacement)
         return rep_rtf
 
     def run_parsing(self, rtf):
         output = DeEncapsulator(rtf)
-        output.stripped_rtf = output._strip_htmlrtf_sections()
-        output.simplified_rtf = output._simplify_text_for_parsing()
-        output.doc_tree = output._parse_rtf()
+        escaped_rtf = encode_escaped_control_chars(output.raw_rtf)
+        output.parse_rtf(escaped_rtf)
+        output.get_doc_tree()
         return output
 
-    def check_deencapsulate_validity(self, data, expect_error=None, name="test"):
+    def check_deencapsulate_validity(self, data,
+                                     expect_error=None,
+                                     name="test",
+                                     print_error=False):
         """Helper to check if a test input raises or doesn't raise an error."""
         found_error = None
         try:
             output = DeEncapsulator(data)
             output.deencapsulate()
         except Exception as _e:
             found_error = _e
-
+            if print_error is True:
+                import traceback
+                traceback.print_exception(type(found_error),
+                                          found_error,
+                                          found_error.__traceback__)
+        # output.deencapsulate()
         if expect_error is not None:
             if found_error is None:
                 self.fail("Expected {} but DeEncapsulator finished without error on {}.".format(expect_error, name))
             if not isinstance(found_error, expect_error):
                 self.fail('Unexpected error {} from DeEncapsulator for {}.'.format(found_error, name))
         else:
             if found_error is not None:
```

### Comparing `RTFDE-0.0.2/tests/parse_rtf/test_validate_file.py` & `RTFDE-0.1.0/tests/parse_rtf/test_validate_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,42 +4,43 @@
 - Correct RTF data doesn't raise any errors.
 - Garbage data fails verbosely.
 - Likely common misuse of the library fails verbosely.
 """
 
 import unittest
 from os.path import join
-from RTFDE.exceptions import MalformedRtf
+from RTFDE.exceptions import MalformedRtf, MalformedEncapsulatedRtf
 from RTFDE.deencapsulate import DeEncapsulator
 from tests.test_utils import DATA_BASE_DIR
 
+
 class TestInputValidity(unittest.TestCase):
     """ Tests basic valid and invalid inputs."""
 
     def test_valid_rtf_string(self):
-        """ Check that a valid encapsulated rtf string returns 0 exit status."""
+        """ Check that opening an rtf file as a string returns a TypeError."""
         quote_printable_rtf_path = join(DATA_BASE_DIR, "plain_text", "quoted_printable_01.rtf")
         with open(quote_printable_rtf_path, 'r') as fp:
             raw_rtf = fp.read()
             self.check_deencapsulate_validity(raw_rtf,
-                                              expect_error=None,
+                                              expect_error=TypeError,
                                               name="quoted_printable_01.rtf")
 
     def test_valid_rtf_bytes(self):
         """ Check that a valid encapsulated rtf byte string returns 0 exit status."""
         quote_printable_rtf_path = join(DATA_BASE_DIR, "plain_text", "quoted_printable_01.rtf")
         with open(quote_printable_rtf_path, 'rb') as fp:
             raw_rtf = fp.read()
             self.check_deencapsulate_validity(raw_rtf,
                                               expect_error=None,
                                               name="quoted_printable_01.rtf")
 
     def test_invalid_none(self):
         """ Check that passing nothing returns a non-zero exit status."""
-        self.check_deencapsulate_validity("",
+        self.check_deencapsulate_validity(b"",
                                           expect_error=MalformedRtf,
                                           name="empty string")
         self.check_deencapsulate_validity(b"",
                                           expect_error=MalformedRtf,
                                           name="empty byte string")
         self.check_deencapsulate_validity(None,
                                           expect_error=TypeError,
@@ -58,14 +59,24 @@
         """ Check that passing a file pointer to a valid rtf file returns a non-zero exit status."""
         quote_printable_rtf_path = join(DATA_BASE_DIR, "plain_text", "quoted_printable_01.rtf")
         with open(quote_printable_rtf_path, 'rb') as fp:
             self.check_deencapsulate_validity(fp,
                                               expect_error=TypeError,
                                               name="rtf file pointer")
 
+    def test_far_too_minimal_rtf_file(self):
+        raw_rtf = b"{\\rtf1}}"
+        self.check_deencapsulate_validity(raw_rtf,
+                                          expect_error=MalformedEncapsulatedRtf,
+                                          name="rtf with an extra brace")
+        raw_rtf = b"{\\rtf1}1"
+        self.check_deencapsulate_validity(raw_rtf,
+                                          expect_error=MalformedEncapsulatedRtf,
+                                          name="rtf with an extra 1")
+
     def check_deencapsulate_validity(self, data, expect_error=None, name="test"):
         """Helper to check if a test input raises or doesn't raise an error."""
         found_error = None
         try:
             output = DeEncapsulator(data)
             output.deencapsulate()
         except Exception as _e:
```

