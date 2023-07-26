# Comparing `tmp/q2report-0.1.32.tar.gz` & `tmp/q2report-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2report-0.1.32.tar", max compression
+gzip compressed data, was "q2report-0.1.33.tar", max compression
```

## Comparing `q2report-0.1.32.tar` & `q2report-0.1.33.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.32/LICENSE
--rw-r--r--   0        0        0      536 2023-07-24 20:54:04.029178 q2report-0.1.32/pyproject.toml
--rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.32/q2report/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.32/q2report/q2engine/__init__.py
--rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.32/q2report/q2engine/q2engine_core.py
--rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.32/q2report/q2engine/q2engine_pyqt.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.32/q2report/q2printer/__init__.py
--rw-r--r--   0        0        0     8733 2023-07-12 19:54:50.695656 q2report-0.1.32/q2report/q2printer/docx_parts.py
--rw-r--r--   0        0        0     8479 2023-06-25 22:47:50.666231 q2report-0.1.32/q2report/q2printer/q2printer.py
--rw-r--r--   0        0        0    18818 2023-07-12 19:54:34.087531 q2report-0.1.32/q2report/q2printer/q2printer_docx.py
--rw-r--r--   0        0        0     6126 2023-06-21 17:49:50.189551 q2report-0.1.32/q2report/q2printer/q2printer_html.py
--rw-r--r--   0        0        0    20677 2023-07-21 15:58:27.016880 q2report-0.1.32/q2report/q2printer/q2printer_xlsx.py
--rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.32/q2report/q2printer/xlsx_parts.py
--rw-r--r--   0        0        0    31040 2023-07-24 20:45:33.537327 q2report-0.1.32/q2report/q2report.py
--rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.32/q2report/q2utils.py
--rw-r--r--   0        0        0       22 2023-07-24 20:54:06.238873 q2report-0.1.32/q2report/version.py
--rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.32/README.md
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 q2report-0.1.32/PKG-INFO
+-rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2report-0.1.33/LICENSE
+-rw-r--r--   0        0        0      537 2023-07-26 23:24:03.605825 q2report-0.1.33/pyproject.toml
+-rw-r--r--   0        0        0       42 2022-12-11 17:39:38.103740 q2report-0.1.33/q2report/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.103740 q2report-0.1.33/q2report/q2engine/__init__.py
+-rw-r--r--   0        0        0      115 2022-12-11 17:39:38.103740 q2report-0.1.33/q2report/q2engine/q2engine_core.py
+-rw-r--r--   0        0        0       90 2022-12-11 17:39:38.107739 q2report-0.1.33/q2report/q2engine/q2engine_pyqt.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:38.107739 q2report-0.1.33/q2report/q2printer/__init__.py
+-rw-r--r--   0        0        0     8733 2023-07-12 19:54:50.695656 q2report-0.1.33/q2report/q2printer/docx_parts.py
+-rw-r--r--   0        0        0     8338 2023-07-26 08:18:01.892779 q2report-0.1.33/q2report/q2printer/q2printer.py
+-rw-r--r--   0        0        0    18675 2023-07-26 08:17:38.485026 q2report-0.1.33/q2report/q2printer/q2printer_docx.py
+-rw-r--r--   0        0        0     5983 2023-07-26 08:17:46.036036 q2report-0.1.33/q2report/q2printer/q2printer_html.py
+-rw-r--r--   0        0        0    20534 2023-07-26 08:17:54.125833 q2report-0.1.33/q2report/q2printer/q2printer_xlsx.py
+-rw-r--r--   0        0        0     8792 2023-06-21 10:36:28.504330 q2report-0.1.33/q2report/q2printer/xlsx_parts.py
+-rw-r--r--   0        0        0    30897 2023-07-26 08:17:30.792654 q2report-0.1.33/q2report/q2report.py
+-rw-r--r--   0        0        0     1708 2023-02-10 16:01:23.063515 q2report-0.1.33/q2report/q2utils.py
+-rw-r--r--   0        0        0       22 2023-07-26 23:24:05.374565 q2report-0.1.33/q2report/version.py
+-rw-r--r--   0        0        0     1486 2022-12-11 17:39:38.099742 q2report-0.1.33/README.md
+-rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 q2report-0.1.33/PKG-INFO
```

### Comparing `q2report-0.1.32/LICENSE` & `q2report-0.1.33/LICENSE`

 * *Files identical despite different names*

### Comparing `q2report-0.1.32/pyproject.toml` & `q2report-0.1.33/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "q2report"
-version = "0.1.32"
+version = "0.1.33"
 description = ""
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
-pillow = "^9.4.0"
+pillow = ">=9.4.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 pytest = "^7.0.0"
 black = {version = "^22.3.0", allow-prereleases = true}
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `q2report-0.1.32/q2report/q2printer/docx_parts.py` & `q2report-0.1.33/q2report/q2printer/docx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.32/q2report/q2printer/q2printer.py` & `q2report-0.1.33/q2report/q2printer/q2printer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,14 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-if __name__ == "__main__":  # pragma: no cover
-    import sys
-
-    sys.path.insert(0, ".")
-    from demo.demo import demo
-
-    demo()
 
 import os
 from q2report.q2utils import num
 import sys
 import subprocess
```

### Comparing `q2report-0.1.32/q2report/q2printer/q2printer_docx.py` & `q2report-0.1.33/q2report/q2printer/q2printer_docx.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-if __name__ == "__main__":  # pragma: no cover
-    import sys
-
-    sys.path.insert(0, ".")
-    from demo.demo import demo
-
-    demo()
-
 
 from q2report.q2printer.q2printer import Q2Printer
 from q2report.q2printer.docx_parts import docx_parts
 from q2report.q2utils import num, int_, reMultiSpaceDelete
 import zipfile
 import base64
```

### Comparing `q2report-0.1.32/q2report/q2printer/q2printer_html.py` & `q2report-0.1.33/q2report/q2printer/q2printer_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-if __name__ == "__main__":  # pragma: no cover
-    import sys
-
-    sys.path.insert(0, ".")
-    from demo.demo import demo
-
-    demo()
-
 
 from q2report.q2printer.q2printer import Q2Printer
 from q2report.q2utils import int_
 import webbrowser
 import os
```

### Comparing `q2report-0.1.32/q2report/q2printer/q2printer_xlsx.py` & `q2report-0.1.33/q2report/q2printer/q2printer_xlsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-if __name__ == "__main__":  # pragma: no cover
-    import sys
-
-    sys.path.insert(0, ".")
-    from demo.demo import demo
-
-    demo()
-
 
 from q2report.q2printer.q2printer import Q2Printer
 from q2report.q2printer.xlsx_parts import xlsx_parts
 from q2report.q2utils import num, int_, reMultiSpaceDelete
 
 import zipfile
 import re
```

### Comparing `q2report-0.1.32/q2report/q2printer/xlsx_parts.py` & `q2report-0.1.33/q2report/q2printer/xlsx_parts.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.32/q2report/q2report.py` & `q2report-0.1.33/q2report/q2report.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-if __name__ == "__main__":  # pragma: no cover
-    import sys
-
-    sys.path.insert(0, ".")
-    from demo.demo import demo
-
-    demo()
-
 
 import json
 from copy import deepcopy
 import re
 import os
 import html
 from io import BytesIO
```

### Comparing `q2report-0.1.32/q2report/q2utils.py` & `q2report-0.1.33/q2report/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2report-0.1.32/README.md` & `q2report-0.1.33/README.md`

 * *Files identical despite different names*

### Comparing `q2report-0.1.32/PKG-INFO` & `q2report-0.1.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: q2report
-Version: 0.1.32
+Version: 0.1.33
 Summary: 
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pillow (>=9.4.0,<10.0.0)
+Requires-Dist: pillow (>=9.4.0)
 Description-Content-Type: text/markdown
 
 # The light Python report builder.
 Converts data into formatted text (**HTML**, **DOCX**, **XLSX**):
 ```python
 data = {'data_source1':[{'col1': 'value row1', ....}, ...],
         'data_source2':[{'col_1': 'valie_row1', ....}, ...],
```

