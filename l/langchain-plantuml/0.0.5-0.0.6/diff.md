# Comparing `tmp/langchain_plantuml-0.0.5.tar.gz` & `tmp/langchain_plantuml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_plantuml-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "langchain_plantuml-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `langchain_plantuml-0.0.5.tar` & `langchain_plantuml-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11356 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/LICENSE
--rw-r--r--   0        0        0     3006 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/README.md
--rw-r--r--   0        0        0      573 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/__init__.py
--rw-r--r--   0        0        0      573 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/__init__.py
--rw-r--r--   0        0        0     9487 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py
--rw-r--r--   0        0        0    13343 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py
--rw-r--r--   0        0        0      573 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/core/__init__.py
--rw-r--r--   0        0        0     2819 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/core/plantuml_callback_handler.py
--rw-r--r--   0        0        0     1255 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/langchain_plantuml/diagram.py
--rw-r--r--   0        0        0     1749 2023-07-24 08:48:46.560902 langchain_plantuml-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 langchain_plantuml-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-27 03:01:44.585948 langchain_plantuml-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3176 2023-07-27 03:01:44.585948 langchain_plantuml-0.0.6/README.md
+-rw-r--r--   0        0        0      573 2023-07-27 03:01:44.585948 langchain_plantuml-0.0.6/langchain_plantuml/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-27 03:01:44.585948 langchain_plantuml-0.0.6/langchain_plantuml/core/__init__.py
+-rw-r--r--   0        0        0     3400 2023-07-27 03:01:44.585948 langchain_plantuml-0.0.6/langchain_plantuml/core/plantuml_callback_handler.py
+-rw-r--r--   0        0        0     1391 2023-07-27 03:01:44.585948 langchain_plantuml-0.0.6/langchain_plantuml/diagram.py
+-rw-r--r--   0        0        0      573 2023-07-27 03:01:44.585948 langchain_plantuml-0.0.6/langchain_plantuml/plantuml/__init__.py
+-rw-r--r--   0        0        0     9562 2023-07-27 03:01:44.585948 langchain_plantuml-0.0.6/langchain_plantuml/plantuml/plantuml_activity_diagram_beta_callback_handler.py
+-rw-r--r--   0        0        0    13418 2023-07-27 03:01:44.585948 langchain_plantuml-0.0.6/langchain_plantuml/plantuml/plantuml_sequence_diagram_callback_handler.py
+-rw-r--r--   0        0        0     1749 2023-07-27 03:01:44.585948 langchain_plantuml-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4288 1970-01-01 00:00:00.000000 langchain_plantuml-0.0.6/PKG-INFO
```

### Comparing `langchain_plantuml-0.0.5/LICENSE` & `langchain_plantuml-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.5/README.md` & `langchain_plantuml-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPi version](https://img.shields.io/pypi/v/langchain-plantuml.svg)](https://pypi.org/project/langchain-plantuml/)
 [![lint](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml)
 [![Build status](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/release.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![](https://img.shields.io/pypi/dm/langchain-plantuml)](https://pypi.org/project/langchain-plantuml/)
 
-Subscribe to events using a callback and store them in PlantUML format **Activity Diagram** and **Sequence Diagram**. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
+Subscribe to events using a callback and store them in PlantUML format to easily visualize LangChain workflow in Activity Diagram and Sequence Diagram. 
+You can easily subscribe to events and keep them in a form that is easy to visualize and analyze using PlantUML.
 
 Activity Diagram 
 
 ![](screenshot/activity-diagram.png)
 
 Sequence Diagram
 
@@ -36,28 +37,28 @@
 
 Running the minimal activity diagram example.
 
 ```python
 from langchain import OpenAI, LLMChain, PromptTemplate
 from langchain.memory import ConversationBufferMemory
 
-from langchain_plantuml import diagram
+from langchain_plantuml import plantuml
 
 template = """You are a chatbot having a conversation with a human.
 
 {chat_history}
 Human: {human_input}
 Chatbot:"""
 
 prompt = PromptTemplate(
     input_variables=["chat_history", "human_input"], template=template
 )
 memory = ConversationBufferMemory(memory_key="chat_history")
 
-callback_handler = diagram.activity_diagram_callback()
+callback_handler = plantuml.activity_diagram_callback()
 
 llm_chain = LLMChain(
     llm=OpenAI(),
     prompt=prompt,
     verbose=True,
     memory=memory,
     callbacks=[callback_handler]
@@ -75,20 +76,26 @@
 
 Sequence Diagram
 
 ```python
 callback_handler = diagram.sequence_diagram_callback()
 ```
 
-Support Custom Note Max Length(default 1000)
+Custom note max Length(default 1000)
 
 ```python
 callback_handler = diagram.activity_diagram_callback(note_max_length=2000)
 ```
 
+Custom note wrap width(default 500)
+
+```python
+callback_handler = diagram.activity_diagram_callback(note_wrap_width=500)
+```
+
 ## Exporting PlantUML to PNG
 
 You can download [plantuml.1.2023.10.jar](https://github.com/plantuml/plantuml/releases/download/v1.2023.10/plantuml-1.2023.10.jar)
 
 ```shell
 java -DPLANTUML_LIMIT_SIZE=81920 -jar plantuml-1.2023.10.jar example-activity.puml
 ```
```

### Comparing `langchain_plantuml-0.0.5/langchain_plantuml/__init__.py` & `langchain_plantuml-0.0.6/langchain_plantuml/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/__init__.py` & `langchain_plantuml-0.0.6/langchain_plantuml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py` & `langchain_plantuml-0.0.6/langchain_plantuml/plantuml/plantuml_activity_diagram_beta_callback_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,23 @@
     _runs_metrics: dict = {}
 
     def __init__(
         self,
         color: Optional[str] = None,
         skin_param: List[str] = DEFAULT_SKIN_PARAM,
         note_max_length: int = 1000,
+        note_wrap_width: int = 500,
     ) -> None:
-        super().__init__()
+        super().__init__(
+            note_max_length=note_max_length, note_wrap_width=note_wrap_width
+        )
         for param in skin_param:
             self.uml_content.append(param)
         self.uml_content.append("start")
         self.color = color
-        self.note_max_length = note_max_length
 
     def on_llm_start(
         self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
     ) -> None:
         run_metric = self._get_run_object(serialized=serialized, **kwargs)
         activity_name = self._wrapper_activity_name(
             self.on_llm_start.__name__,
```

### Comparing `langchain_plantuml-0.0.5/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py` & `langchain_plantuml-0.0.6/langchain_plantuml/plantuml/plantuml_sequence_diagram_callback_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,23 +34,25 @@
     _runs_metrics: dict = {}
 
     def __init__(
         self,
         color: Optional[str] = None,
         skin_param: List[str] = DEFAULT_SKIN_PARAM,
         note_max_length: int = 1000,
+        note_wrap_width: int = 500,
     ) -> None:
-        super().__init__()
+        super().__init__(
+            note_max_length=note_max_length, note_wrap_width=note_wrap_width
+        )
         for param in skin_param:
             self.uml_content.append(param)
         self.uml_content.append(UML_PARTICIPANTS_FLAG)
         self.participants = {}
         self.participant_name_indexes = []
         self.color = color
-        self.note_max_length = note_max_length
 
     def on_llm_start(
         self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
     ) -> None:
         run_metric = self._get_run_object(serialized=serialized, **kwargs)
         activity_name = self._wrapper_sequence_name(
             self.on_llm_start.__name__,
```

### Comparing `langchain_plantuml-0.0.5/langchain_plantuml/core/__init__.py` & `langchain_plantuml-0.0.6/langchain_plantuml/plantuml/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.5/langchain_plantuml/core/plantuml_callback_handler.py` & `langchain_plantuml-0.0.6/langchain_plantuml/core/plantuml_callback_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,33 +17,36 @@
 
 from langchain.callbacks.base import BaseCallbackHandler
 
 
 class BasePlantUMLCallbackHandler(BaseCallbackHandler, ABC):
     crlf: str = "⏎"
     note_max_length: int = 1000
+    note_wrap_width: int = 500
     emojis = {
         "on_llm_start": "<:1f916:>",
         "on_llm_end": "<:1f916:>",
         "on_chain_start": "<:1f3af:>",
         "on_chain_end": "<:1f3af:>",
         "on_tool_start": "<:1f528:>",
         "on_tool_end": "<:1f528:>",
         "on_text": "<:1f4c6:>",
     }
 
-    def __init__(self):
+    def __init__(self, note_max_length: int = 1000, note_wrap_width: int = 500):
+        self.note_wrap_width = note_wrap_width
+        self.note_max_length = note_max_length
         self.step = 0
         self.total_tokens = 0
         self.prompt_tokens = 0
         self.completion_tokens = 0
         self.uml_content = []
         self.uml_content.append("@startuml")
         self.uml_content.append("skinparam dpi 300")
-        self.uml_content.append("skinparam wrapWidth 500")
+        self.uml_content.append(f"skinparam wrapWidth {self.note_wrap_width}")
         self.uml_content.append("skinparam shadowing false")
         self.uml_content.append("skinparam noteFontName Arial")
         self.uml_content.append("skinparam noteFontSize 10")
         self.uml_content.append("skinparam noteBackgroundColor #ECECEC")
         self.uml_content.append("skinparam noteBorderColor #C0C0C0")
         self.uml_content.append("skinparam noteFontColor #333333")
         self.uml_content.append("skinparam noteBorderThickness 0")
@@ -66,9 +69,23 @@
         for line in lines:
             self.uml_content.append(line)
 
     def _wrapper_note(self, note: str) -> List[str]:
         new_note = note.strip()
         if len(new_note) > self.note_max_length:
             new_note = f"{new_note[:self.note_max_length]} ... (Omit {len(new_note) - self.note_max_length} words)"
-        new_lines = [f"{line}{self.crlf}" for line in new_note.split("\n")]
-        return new_lines
+
+        new_notes = [f"{line}{self.crlf}" for line in new_note.split("\n")]
+
+        wrap_notes = [
+            word
+            for phrase in new_notes
+            for word in (
+                [
+                    phrase[i : i + self.note_wrap_width]
+                    for i in range(0, len(phrase), self.note_wrap_width)
+                ]
+                if len(phrase) > self.note_wrap_width
+                else [phrase]
+            )
+        ]
+        return wrap_notes
```

### Comparing `langchain_plantuml-0.0.5/langchain_plantuml/diagram.py` & `langchain_plantuml-0.0.6/langchain_plantuml/diagram.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,19 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from langchain.callbacks.base import BaseCallbackHandler
 
-from langchain_plantuml.activity_diagram_beta.plantuml_activity_diagram_beta_callback_handler import \
+from langchain_plantuml.plantuml.plantuml_activity_diagram_beta_callback_handler import \
     PlantUMLActivityDiagramCallbackHandler
-from langchain_plantuml.activity_diagram_beta.plantuml_sequence_diagram_callback_handler import \
+from langchain_plantuml.plantuml.plantuml_sequence_diagram_callback_handler import \
     PlantUMLSequenceDiagramCallbackHandler
 
 
-def activity_diagram_callback(note_max_length: int = 1000) -> BaseCallbackHandler:
-    return PlantUMLActivityDiagramCallbackHandler(note_max_length=note_max_length)
+def activity_diagram_callback(
+    note_max_length: int = 1000, note_wrap_width: int = 500
+) -> BaseCallbackHandler:
+    return PlantUMLActivityDiagramCallbackHandler(
+        note_max_length=note_max_length, note_wrap_width=note_wrap_width
+    )
 
 
-def sequence_diagram_callback(note_max_length: int = 1000) -> BaseCallbackHandler:
-    return PlantUMLSequenceDiagramCallbackHandler(note_max_length=note_max_length)
+def sequence_diagram_callback(
+    note_max_length: int = 1000, note_wrap_width: int = 500
+) -> BaseCallbackHandler:
+    return PlantUMLSequenceDiagramCallbackHandler(
+        note_max_length=note_max_length, note_wrap_width=note_wrap_width
+    )
```

### Comparing `langchain_plantuml-0.0.5/pyproject.toml` & `langchain_plantuml-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [build-system]
 requires = ["flit_core==3.9.0"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "langchain-plantuml"
-version = "0.0.5"
+version = "0.0.6"
 description = "Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze."
 authors = [{ name = "Lei Zhang", email = "zhanglei@apache.org" }]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "langchain>=0.0.228"
```

### Comparing `langchain_plantuml-0.0.5/PKG-INFO` & `langchain_plantuml-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-plantuml
-Version: 0.0.5
+Version: 0.0.6
 Summary: Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
 Author-email: Lei Zhang <zhanglei@apache.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: langchain>=0.0.228
 Requires-Dist: flake8==5.0.4 ; extra == "lint"
 Requires-Dist: pyproject-flake8==5.0.4 ; extra == "lint"
@@ -27,15 +27,16 @@
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPi version](https://img.shields.io/pypi/v/langchain-plantuml.svg)](https://pypi.org/project/langchain-plantuml/)
 [![lint](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/lint.yml)
 [![Build status](https://github.com/coolbeevip/langchain_plantuml/actions/workflows/release.yml/badge.svg)](https://github.com/coolbeevip/langchain_plantuml/actions)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![](https://img.shields.io/pypi/dm/langchain-plantuml)](https://pypi.org/project/langchain-plantuml/)
 
-Subscribe to events using a callback and store them in PlantUML format **Activity Diagram** and **Sequence Diagram**. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
+Subscribe to events using a callback and store them in PlantUML format to easily visualize LangChain workflow in Activity Diagram and Sequence Diagram. 
+You can easily subscribe to events and keep them in a form that is easy to visualize and analyze using PlantUML.
 
 Activity Diagram 
 
 ![](screenshot/activity-diagram.png)
 
 Sequence Diagram
 
@@ -60,28 +61,28 @@
 
 Running the minimal activity diagram example.
 
 ```python
 from langchain import OpenAI, LLMChain, PromptTemplate
 from langchain.memory import ConversationBufferMemory
 
-from langchain_plantuml import diagram
+from langchain_plantuml import plantuml
 
 template = """You are a chatbot having a conversation with a human.
 
 {chat_history}
 Human: {human_input}
 Chatbot:"""
 
 prompt = PromptTemplate(
     input_variables=["chat_history", "human_input"], template=template
 )
 memory = ConversationBufferMemory(memory_key="chat_history")
 
-callback_handler = diagram.activity_diagram_callback()
+callback_handler = plantuml.activity_diagram_callback()
 
 llm_chain = LLMChain(
     llm=OpenAI(),
     prompt=prompt,
     verbose=True,
     memory=memory,
     callbacks=[callback_handler]
@@ -99,20 +100,26 @@
 
 Sequence Diagram
 
 ```python
 callback_handler = diagram.sequence_diagram_callback()
 ```
 
-Support Custom Note Max Length(default 1000)
+Custom note max Length(default 1000)
 
 ```python
 callback_handler = diagram.activity_diagram_callback(note_max_length=2000)
 ```
 
+Custom note wrap width(default 500)
+
+```python
+callback_handler = diagram.activity_diagram_callback(note_wrap_width=500)
+```
+
 ## Exporting PlantUML to PNG
 
 You can download [plantuml.1.2023.10.jar](https://github.com/plantuml/plantuml/releases/download/v1.2023.10/plantuml-1.2023.10.jar)
 
 ```shell
 java -DPLANTUML_LIMIT_SIZE=81920 -jar plantuml-1.2023.10.jar example-activity.puml
 ```
```

