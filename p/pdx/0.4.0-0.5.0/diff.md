# Comparing `tmp/pdx-0.4.0.tar.gz` & `tmp/pdx-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdx-0.4.0.tar", max compression
+gzip compressed data, was "pdx-0.5.0.tar", max compression
```

## Comparing `pdx-0.4.0.tar` & `pdx-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,47 @@
--rw-r--r--   0        0        0    11346 2023-06-17 05:57:05.771799 pdx-0.4.0/LICENSE
--rw-r--r--   0        0        0     1676 2023-07-04 20:25:52.208721 pdx-0.4.0/README.md
--rw-r--r--   0        0        0      832 2023-07-07 16:24:08.269082 pdx-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-07-02 10:21:05.627006 pdx-0.4.0/src/pdx/__init__.py
--rw-r--r--   0        0        0     1655 2023-07-02 10:40:15.375462 pdx-0.4.0/src/pdx/agent/__init__.py
--rw-r--r--   0        0        0     2843 2023-07-02 10:40:49.397512 pdx-0.4.0/src/pdx/agent/completer.py
--rw-r--r--   0        0        0     4155 2023-06-17 06:01:30.639029 pdx-0.4.0/src/pdx/agent/config.py
--rw-r--r--   0        0        0     1971 2023-07-02 10:37:06.519366 pdx-0.4.0/src/pdx/agent/metadata.py
--rw-r--r--   0        0        0     5005 2023-06-17 06:01:28.170575 pdx-0.4.0/src/pdx/agent/prompt.py
--rw-r--r--   0        0        0     2036 2023-06-17 06:00:09.706566 pdx-0.4.0/src/pdx/agent/prompt_session.py
--rw-r--r--   0        0        0     1894 2023-06-17 06:01:26.871641 pdx-0.4.0/src/pdx/agent/templater.py
--rw-r--r--   0        0        0     1965 2023-07-02 13:36:16.141378 pdx-0.4.0/src/pdx/agent/tester.py
--rw-r--r--   0        0        0     1746 2023-07-02 10:42:19.914775 pdx-0.4.0/src/pdx/cli.py
--rw-r--r--   0        0        0        0 2023-06-28 14:39:53.768534 pdx-0.4.0/src/pdx/commands/__init__.py
--rw-r--r--   0        0        0     1317 2023-06-28 15:01:30.272225 pdx-0.4.0/src/pdx/commands/create.py
--rw-r--r--   0        0        0     1043 2023-06-17 06:02:47.694295 pdx-0.4.0/src/pdx/exceptions.py
--rw-r--r--   0        0        0     2162 2023-06-17 06:03:02.108872 pdx-0.4.0/src/pdx/logger.py
--rw-r--r--   0        0        0     1951 2023-06-17 06:01:22.481929 pdx-0.4.0/src/pdx/models/__init__.py
--rw-r--r--   0        0        0     2913 2023-07-02 10:45:38.216714 pdx-0.4.0/src/pdx/models/anthropic/__init__.py
--rw-r--r--   0        0        0     4202 2023-06-17 06:01:17.123209 pdx-0.4.0/src/pdx/models/anthropic/client.py
--rw-r--r--   0        0        0       57 2023-06-17 06:00:09.710685 pdx-0.4.0/src/pdx/models/anthropic/constants.py
--rw-r--r--   0        0        0     1698 2023-06-17 06:01:13.890539 pdx-0.4.0/src/pdx/models/anthropic/exceptions.py
--rw-r--r--   0        0        0     3543 2023-06-17 06:01:20.740652 pdx-0.4.0/src/pdx/models/api_client.py
--rw-r--r--   0        0        0      478 2023-06-17 06:00:09.711427 pdx-0.4.0/src/pdx/models/metadata.py
--rw-r--r--   0        0        0     4639 2023-07-02 10:45:47.318103 pdx-0.4.0/src/pdx/models/openai/__init__.py
--rw-r--r--   0        0        0     2892 2023-06-17 06:01:10.182094 pdx-0.4.0/src/pdx/models/openai/client.py
--rw-r--r--   0        0        0     1414 2023-06-17 06:01:07.686125 pdx-0.4.0/src/pdx/models/openai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713048 pdx-0.4.0/src/pdx/models/utils.py
--rw-r--r--   0        0        0      252 2023-06-17 06:00:09.713261 pdx-0.4.0/src/pdx/settings.py
--rw-r--r--   0        0        0       54 2023-06-28 14:16:27.138776 pdx-0.4.0/src/pdx/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 14:38:23.123005 pdx-0.4.0/src/pdx/templates/simple/Readme.md
--rw-r--r--   0        0        0      405 2023-06-28 14:33:23.114668 pdx-0.4.0/src/pdx/templates/simple/__init__.py
--rw-r--r--   0        0        0      192 2023-06-28 14:54:47.892150 pdx-0.4.0/src/pdx/templates/simple/templates/1_prompt.defaults.yaml
--rw-r--r--   0        0        0      159 2023-06-28 14:27:03.141095 pdx-0.4.0/src/pdx/templates/simple/templates/1_prompt.jinja
--rw-r--r--   0        0        0      191 2023-06-28 14:54:26.649501 pdx-0.4.0/src/pdx/templates/simple/tests/test_1.yaml
--rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713573 pdx-0.4.0/src/pdx/utils/__init__.py
--rw-r--r--   0        0        0      595 2023-06-17 06:00:09.714358 pdx-0.4.0/src/pdx/utils/rw.py
--rw-r--r--   0        0        0       22 2023-07-02 16:26:56.721767 pdx-0.4.0/src/pdx/version.py
--rw-r--r--   0        0        0     2748 1970-01-01 00:00:00.000000 pdx-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-17 05:57:05.771799 pdx-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1678 2023-07-27 11:10:49.055554 pdx-0.5.0/README.md
+-rw-r--r--   0        0        0      832 2023-07-27 11:10:49.056921 pdx-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-07-27 11:10:49.057117 pdx-0.5.0/src/pdx/__init__.py
+-rw-r--r--   0        0        0     2881 2023-07-27 11:10:49.057347 pdx-0.5.0/src/pdx/agent/__init__.py
+-rw-r--r--   0        0        0     1327 2023-07-27 11:10:49.057529 pdx-0.5.0/src/pdx/agent/config.py
+-rw-r--r--   0        0        0     1898 2023-07-27 11:10:49.057733 pdx-0.5.0/src/pdx/agent/metadata.py
+-rw-r--r--   0        0        0     1947 2023-07-27 11:10:49.057944 pdx-0.5.0/src/pdx/agent/tester.py
+-rw-r--r--   0        0        0     1677 2023-07-27 11:10:49.058158 pdx-0.5.0/src/pdx/cli.py
+-rw-r--r--   0        0        0        0 2023-06-28 14:39:53.768534 pdx-0.5.0/src/pdx/commands/__init__.py
+-rw-r--r--   0        0        0     1317 2023-06-28 15:01:30.272225 pdx-0.5.0/src/pdx/commands/create.py
+-rw-r--r--   0        0        0     1043 2023-06-17 06:02:47.694295 pdx-0.5.0/src/pdx/exceptions.py
+-rw-r--r--   0        0        0     2172 2023-07-27 11:10:49.058505 pdx-0.5.0/src/pdx/logger.py
+-rw-r--r--   0        0        0       93 2023-07-27 11:10:49.058639 pdx-0.5.0/src/pdx/metadata.py
+-rw-r--r--   0        0        0        0 2023-07-27 11:10:49.058730 pdx-0.5.0/src/pdx/models/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-27 11:10:49.058958 pdx-0.5.0/src/pdx/models/anthropic/__init__.py
+-rw-r--r--   0        0        0     3860 2023-07-27 11:10:49.059167 pdx-0.5.0/src/pdx/models/anthropic/client.py
+-rw-r--r--   0        0        0     4400 2023-07-27 11:10:49.059316 pdx-0.5.0/src/pdx/models/anthropic/completion.py
+-rw-r--r--   0        0        0       57 2023-06-17 06:00:09.710685 pdx-0.5.0/src/pdx/models/anthropic/constants.py
+-rw-r--r--   0        0        0     1698 2023-06-17 06:01:13.890539 pdx-0.5.0/src/pdx/models/anthropic/exceptions.py
+-rw-r--r--   0        0        0     3543 2023-06-17 06:01:20.740652 pdx-0.5.0/src/pdx/models/api_client.py
+-rw-r--r--   0        0        0     2171 2023-07-27 11:10:49.059612 pdx-0.5.0/src/pdx/models/config.py
+-rw-r--r--   0        0        0      462 2023-07-27 11:10:49.059806 pdx-0.5.0/src/pdx/models/metadata.py
+-rw-r--r--   0        0        0     3764 2023-07-27 11:10:49.059941 pdx-0.5.0/src/pdx/models/model.py
+-rw-r--r--   0        0        0       57 2023-07-27 11:10:49.060153 pdx-0.5.0/src/pdx/models/openai/__init__.py
+-rw-r--r--   0        0        0     2165 2023-07-27 11:10:49.060479 pdx-0.5.0/src/pdx/models/openai/client.py
+-rw-r--r--   0        0        0     5636 2023-07-27 11:10:49.060629 pdx-0.5.0/src/pdx/models/openai/completion.py
+-rw-r--r--   0        0        0     1414 2023-06-17 06:01:07.686125 pdx-0.5.0/src/pdx/models/openai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713048 pdx-0.5.0/src/pdx/models/utils.py
+-rw-r--r--   0        0        0     2413 2023-07-27 11:10:49.060795 pdx-0.5.0/src/pdx/prompt/__init__.py
+-rw-r--r--   0        0        0     3081 2023-07-27 11:10:49.060934 pdx-0.5.0/src/pdx/prompt/config.py
+-rw-r--r--   0        0        0     1244 2023-07-27 11:10:49.061217 pdx-0.5.0/src/pdx/prompt/prompt_chain.py
+-rw-r--r--   0        0        0     1779 2023-07-27 11:10:49.061341 pdx-0.5.0/src/pdx/prompt/prompt_session.py
+-rw-r--r--   0        0        0     2727 2023-07-27 11:10:49.061477 pdx-0.5.0/src/pdx/prompt/prompt_template.py
+-rw-r--r--   0        0        0     5210 2023-07-27 11:10:49.061629 pdx-0.5.0/src/pdx/prompt/prompt_tree.py
+-rw-r--r--   0        0        0      254 2023-07-27 11:10:49.061964 pdx-0.5.0/src/pdx/settings.py
+-rw-r--r--   0        0        0       54 2023-06-28 14:16:27.138776 pdx-0.5.0/src/pdx/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 14:38:23.123005 pdx-0.5.0/src/pdx/templates/simple/Readme.md
+-rw-r--r--   0        0        0      405 2023-06-28 14:33:23.114668 pdx-0.5.0/src/pdx/templates/simple/__init__.py
+-rw-r--r--   0        0        0      192 2023-06-28 14:54:47.892150 pdx-0.5.0/src/pdx/templates/simple/templates/1_prompt.defaults.yaml
+-rw-r--r--   0        0        0      159 2023-06-28 14:27:03.141095 pdx-0.5.0/src/pdx/templates/simple/templates/1_prompt.jinja
+-rw-r--r--   0        0        0      191 2023-06-28 14:54:26.649501 pdx-0.5.0/src/pdx/templates/simple/tests/test_1.yaml
+-rw-r--r--   0        0        0        0 2023-06-17 06:00:09.713573 pdx-0.5.0/src/pdx/utils/__init__.py
+-rw-r--r--   0        0        0      595 2023-06-17 06:00:09.714358 pdx-0.5.0/src/pdx/utils/rw.py
+-rw-r--r--   0        0        0     2051 2023-07-27 11:10:49.062145 pdx-0.5.0/src/pdx/worker/__init__.py
+-rw-r--r--   0        0        0     1905 2023-07-27 11:10:49.062500 pdx-0.5.0/src/pdx/worker/metadata.py
+-rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 pdx-0.5.0/PKG-INFO
```

### Comparing `pdx-0.4.0/LICENSE` & `pdx-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdx-0.4.0/README.md` & `pdx-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ```bash
 pdx create my_first_agent
 ```
 
 Run and test out the agent by running:
 
 ```bash
-pdx test my_first_agent --debug
+pdx test my_first_agent --verbose
 ```
 
 More information here: [PDX - Main Concepts](https://pdxlabs.io/docs/getting-started/main-concepts)
 
 ## Why use PDX?
 
 -   🗃️ Low dependency footprint -> ease of production deployment and maintainance.
```

### Comparing `pdx-0.4.0/pyproject.toml` & `pdx-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdx"
-version = "0.4.0"
+version = "0.5.0"
 description = "Prompt Engineering and Dev-Ops toolkits. A faster way to build and manage applications powered by Language Models."
 keywords = ["prompt", "LLM", "prompt engineering", "dev-ops", "observability", "apps"]
 authors = ["Adithya Krishnan <krishsandeep@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "pdx", from = "src"}]
```

### Comparing `pdx-0.4.0/src/pdx/agent/__init__.py` & `pdx-0.5.0/src/pdx/agent/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,70 @@
-from typing import List, Dict, Union
-from pdx.logger import logger
-from pdx.settings import Keys
-from pdx.agent.completer import CompletionAgent
-from pdx.agent.prompt import PromptTree, PromptSession
+from typing import Union
+from uuid import uuid4
 from pdx.agent.config import AgentConfig
-from pdx.agent.metadata import AgentID, AgentResponse
-from dataclasses import asdict
-
-Request = Union[str, int, float, Dict, List]
-
-
-class AgentBuilder:
-    def __init__(self, path: str, api_keys: Keys = None):
-        self._folder_path = path
-        if api_keys is None:
-            self._api_keys = Keys()
+from pdx.prompt import Prompt
+from pdx.models.model import Model
+from pdx.prompt.prompt_chain import PromptChain
+from pdx.prompt.prompt_tree import PromptTree
+from pdx.prompt.prompt_session import PromptSession
+from pdx.models.metadata import ModelResponse
+from pdx.agent.metadata import AgentID, RequestMetadata, AgentResponse, AgentResponseMetadata
+
+
+class Agent(object):
+    def __init__(self, path: str = None, prompt: Union[Prompt, PromptChain, PromptTree] = None, model: Model = None):
+        if path is not None:
+            self._type = 'config'
+            self._config: AgentConfig = AgentConfig(path)
+            self._agent_id = AgentID(agent_name=self._config.name)
+            if prompt is None:
+                self._prompt: PromptTree = PromptTree(
+                    self._config.prompt_config)
+            else:
+                self._prompt = prompt
+
+            if model is None:
+                self._model: Model = self._config.model_config.build_model()
+            else:
+                self._model = model
         else:
-            self._api_keys = api_keys
-        self._config: AgentConfig = AgentConfig(path)
-        self.prompt_tree: PromptTree = PromptTree(self._config.prompt_config)
-        self._completion_agent = CompletionAgent(
-            self._config.model_config, self._api_keys)
-
-        self._agent_id = AgentID(agent_name=self._config.name)
-
-    async def aexecute(self, request: dict, metadata: dict = None) -> AgentResponse:
-        _prompt = PromptSession(self._config.prompt_config.prompt_type)
-        self.prompt_tree.execute(request, _prompt)
-        _response = await self._completion_agent.aexecute(_prompt, request, self._agent_id)
-        _response.metadata.add_custom(metadata=metadata)
-        return _response
-
-    def execute(self, request: dict, metadata: dict = None) -> AgentResponse:
-        _prompt = PromptSession(self._config.prompt_config.prompt_type)
-        self.prompt_tree.execute(request, _prompt)
-        _response = self._completion_agent.execute(_prompt, request, self._agent_id)
-        _response.metadata.add_custom(metadata=metadata)
-        return _response
+            if prompt is None and model is None:
+                raise ValueError(
+                    'Provide `Prompt` and `Model` if not providing Agent config path.')
+            self._type = 'prompt-model'
+            self._prompt = prompt
+            self._model = model
+            self._agent_id = AgentID(agent_name='agent')
+
+    def _postprocess(self, response: ModelResponse, request: dict, prompt_session: PromptSession) -> AgentResponse:
+        request_metadata = RequestMetadata(
+            agent_id=self._agent_id,
+            request_id=uuid4(),
+            request_values=request,
+            request_params=response.request_params,
+            prompt=prompt_session.export()
+        )
+        metadata = AgentResponseMetadata(
+            request=request_metadata,
+            response=response.metadata
+        )
+        agent_response = AgentResponse(
+            data=response.data,
+            metadata=metadata
+        )
+        return agent_response
+
+    async def aexecute(self, request: dict = {}, metadata: dict = {}):
+        _prompt_session = self._prompt.execute(request)
+        _model_response = await self._model.aexecute(_prompt_session)
+        _agent_response = self._postprocess(
+            _model_response, request, _prompt_session)
+        _agent_response.metadata.add_custom(metadata=metadata)
+        return _agent_response
+
+    def execute(self, request: dict = {}, metadata: dict = {}):
+        _prompt_session = self._prompt.execute(request)
+        _model_response = self._model.execute(_prompt_session)
+        _agent_response = self._postprocess(
+            _model_response, request, _prompt_session)
+        _agent_response.metadata.add_custom(metadata=metadata)
+        return _agent_response
```

### Comparing `pdx-0.4.0/src/pdx/agent/metadata.py` & `pdx-0.5.0/src/pdx/worker/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import uuid
 import subprocess
 from dataclasses import dataclass, field
+from pdx.metadata import PDXMetadata
 from pdx.models.metadata import ResponseMetadata
 from pdx.logger import logger
-from pdx.version import __version__
 
 
 @dataclass
-class PDXMetadata:
-    version: str
-
-
-@dataclass
-class AgentID:
-    agent_name: str
+class WorkerID:
+    worker_name: str
     git_hash: str = None
     git_branch: str = None
 
     def __post_init__(self):
         if self.git_hash is None and self.git_branch is None:
             try:
                 subprocess.check_output(
@@ -33,37 +28,37 @@
                     'It is recommended to run `pdx` from a initialized git repository.', event='warning')
                 self.git_hash = 'not-git-repo'
                 self.git_branch = 'not-git-repo'
 
 
 @dataclass
 class RequestMetadata:
-    agent_id: AgentID
+    worker_id: WorkerID
     request_id: uuid.UUID = None
     request_values: dict = None
     request_params: dict = None
     prompt: list = None
 
     def __post_init__(self):
         if self.request_id is None:
             self.request_id = uuid.uuid4()
 
 
 @dataclass
-class AgentResponseMetadata:
+class WorkerResponseMetadata:
     request: RequestMetadata
     response: ResponseMetadata
     custom: dict = None
     pdx: PDXMetadata = None
 
     def __post_init__(self):
         if self.pdx is None:
-            self.pdx = PDXMetadata(version=__version__)
+            self.pdx = PDXMetadata()
 
     def add_custom(self, metadata: dict):
         self.custom = metadata
 
 
 @dataclass
-class AgentResponse:
-    completion: str
-    metadata: AgentResponseMetadata
+class WorkerResponse:
+    data: str
+    metadata: WorkerResponseMetadata
```

### Comparing `pdx-0.4.0/src/pdx/agent/prompt.py` & `pdx-0.5.0/src/pdx/prompt/prompt_tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,132 @@
 import os
 from collections import OrderedDict
-from pdx.agent.templater import TemplateAgent
-from pdx.agent.config import PromptConfig
-from pdx.agent.prompt_session import PromptSession
-
-
-class TemplateConfig:
-    def __init__(self, config: dict, tempaltes_path: str, role: str = None):
-        self.role = role
-        if role is None:
-            self.name: str = config['template']
-        else:
-            self.name: str = config[role]
-        self.pointer = config.get('pointer', self.name.split('.')[0])
-        self.template_path = os.path.join(tempaltes_path, self.name)
-        self.id = self.name.split('.')[0]
-
-        self._template_agent = TemplateAgent(self.template_path, self.name)
-        self.template_fields = self._template_agent._fields
-
-    def execute(self, fields: dict, prompt_session: PromptSession = None):
-        if fields is None:
-            fields = {}
-        prompt = self._template_agent.execute(fields)
-        prompt_session.add(prompt, self.role)
+from pdx.prompt import Prompt
+from pdx.prompt.config import PromptConfig
+from pdx.prompt.prompt_session import PromptSession
 
 
 class WhenOperationConfig:
     def __init__(self, config: dict, operation: str):
         self.operation = operation
         self.pointer = config.get('pointer', config[operation])
         self.prompt_config = config['prompt']
-        self.prompt_tree = None
+        self.prompt_tree: PromptTree = None
 
-    def execute(self, fields: dict, prompt_session: PromptSession = None):
-        if fields != {}:
-            self.prompt_tree.execute(fields, prompt_session)
+    def execute(self, values: dict, prompt_session: PromptSession = None):
+        if values != {}:
+            self.prompt_tree.execute(values, prompt_session)
 
 
 class LoopOperationConfig:
     def __init__(self, config: dict, operation: str):
         self.operation = operation
         self.pointer = config.get('pointer', config[operation])
         self.prompt_config = config['prompt']
-        self.prompt_tree = None
+        self.prompt_tree: PromptTree = None
 
-    def execute(self, fields: dict, prompt_session: PromptSession = None):
-        for field in fields:
+    def execute(self, values: dict, prompt_session: PromptSession = None):
+        for field in values:
             self.prompt_tree.execute(field, prompt_session)
 
 
 class SwitchOperationConfig:
     def __init__(self, config: dict, operation: str):
         self.operation = operation
         self.pointer = config.get('pointer', config[operation])
         self.cases_config = config['prompt']
-        self.prompt_tree = None
+        self.prompt_tree: PromptTree = None
 
-    def execute(self, fields: dict, prompt_session: PromptSession = None):
-        for case, field in fields.items():
+    def execute(self, values: dict, prompt_session: PromptSession = None):
+        for case, field in values.items():
             if case in self.prompt_tree:
                 self.prompt_tree[case].execute(field, prompt_session)
             elif 'default' in self.prompt_tree:
                 self.prompt_tree['default'].execute(
                     field, prompt_session)
 
 
 class PromptTree:
     def __init__(self, prompt_config: PromptConfig, strict=False):
         self._templates_path = prompt_config.templates_path
         self.prompt_config = prompt_config.config
+        # `strict`: If pointers are not present, do not execute them in the tree.
         self._strict = strict
-        # If pointers are not present, do not execute them in the tree.
         self.tree = self._build_tree()
 
+    def _build_prompt(self, _p: dict, role: str):
+        _prompt_role = role
+        _template_name: str = _p[_prompt_role]
+        _template_path: str = os.path.join(
+            self._templates_path, _template_name)
+        _prompt_pointer = _p.get(
+            'pointer', _template_name.split('.')[0])
+        _prompt = Prompt(
+            template_path=_template_path,
+            pointer=_prompt_pointer,
+            role=_prompt_role
+        )
+
+        return _prompt
+
     def _build_tree(self):
         _tree = OrderedDict()
         for _p in self.prompt_config:
             if 'template' in _p:
-                _config = TemplateConfig(_p, self._templates_path)
-                _tree[_config.pointer] = _config
+                _prompt = self._build_prompt(_p, 'template')
+                _tree[_prompt.pointer] = _prompt
             elif 'system' in _p:
-                _config = TemplateConfig(
-                    _p, self._templates_path, role='system')
-                _tree[_config.pointer] = _config
+                _prompt = self._build_prompt(_p, 'system')
+                _tree[_prompt.pointer] = _prompt
             elif 'user' in _p:
-                _config = TemplateConfig(_p, self._templates_path, role='user')
-                _tree[_config.pointer] = _config
+                _prompt = self._build_prompt(_p, 'user')
+                _tree[_prompt.pointer] = _prompt
             elif 'assistant' in _p:
-                _config = TemplateConfig(
-                    _p, self._templates_path, role='assistant')
-                _tree[_config.pointer] = _config
+                _prompt = self._build_prompt(_p, 'assistant')
+                _tree[_prompt.pointer] = _prompt
             elif 'when' in _p:
                 _config = WhenOperationConfig(_p, operation='when')
+                _prompt_config = PromptConfig(
+                    _config.prompt_config, self._templates_path)
                 _config.prompt_tree = PromptTree(
-                    _p['prompt'], self._templates_path, self._strict)
+                    _prompt_config, self._strict)
                 _tree[_config.pointer] = _config
             elif 'loop' in _p:
                 _config = LoopOperationConfig(_p, operation='loop')
+                _prompt_config = PromptConfig(
+                    _config.prompt_config, self._templates_path)
                 _config.prompt_tree = PromptTree(
-                    _p['prompt'], self._templates_path, self._strict)
+                    _prompt_config, self._strict)
                 _tree[_config.pointer] = _config
             elif 'switch' in _p:
                 _config = SwitchOperationConfig(_p, operation='switch')
                 _cases_tree = OrderedDict()
                 for case in _config.cases_config:
+                    _prompt_config = PromptConfig(
+                        _config.cases_config[case], self._templates_path)
                     _cases_tree[case] = PromptTree(
-                        _config.cases_config[case], self._templates_path, self._strict)
+                        _prompt_config, self._strict)
                 _config.prompt_tree = _cases_tree
                 _tree[_config.pointer] = _config
 
         return _tree
 
-    def execute(self, request, prompt_session: PromptSession):
-        for key, value in self.tree.items():
+    def execute(self, request: dict, prompt_session: PromptSession = None):
+        _output = False
+
+        if prompt_session is None:
+            prompt_session = PromptSession()
+            _output = True
+
+        for key, tree_object in self.tree.items():
             if self._strict:
                 if key in request:
                     field_values = request.get(key, {})
-                    value.execute(field_values, prompt_session)
+                    tree_object.execute(values=field_values,
+                                        prompt_session=prompt_session)
             else:
                 field_values = request.get(key, {})
-                value.execute(field_values, prompt_session)
+                tree_object.execute(values=field_values,
+                                    prompt_session=prompt_session)
+
+        if _output:
+            return prompt_session
```

### Comparing `pdx-0.4.0/src/pdx/agent/templater.py` & `pdx-0.5.0/src/pdx/prompt/prompt_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,71 @@
 import os
 import json
 from jinja2 import Environment, FileSystemLoader, Template, meta
 from pdx.utils.rw import read_yaml
 
 
-class TemplateAgent:
-    def __init__(self, template_path: str, name: str):
-        self._templates_path = os.path.dirname(template_path)
-        self._template_name = name
-        self._template_id = name.split('.')[0]
-
-        self._environment = None
-        self._template = self.load_template()
-        self._fields = self.parse_fields()
-        self._field_values = {}
-
-        _defaults_path = os.path.join(
-            self._templates_path, f"{self._template_id}.defaults.yaml")
-        if os.path.exists(_defaults_path):
-            self.set_field_values(read_yaml(_defaults_path))
+class PromptTemplate:
+    def __init__(self, template_path: str = None, template_string: str = None, name: str = None):
+        if template_string != None:
+            self._template_type = 'string'
+            self._template_string = template_string
+            self._template_name = name
+            self._template_id = name
+            self._environment = None
+            self._template = self.load_native_template()
+            self._fields = {}
+            self._field_values = {}
+        elif template_path != None:
+            self._template_type = 'file'
+            self._templates_path = os.path.dirname(template_path)            
+            self._template_name = os.path.basename(template_path)
+            self._template_id = name.split('.')[0]
+
+            self._environment = None
+            self._template = self.load_template()
+            self._fields = self.parse_fields()
+            self._field_values = {}
+
+            _defaults_path = os.path.join(
+                self._templates_path, f"{self._template_id}.defaults.yaml")
+            if os.path.exists(_defaults_path):
+                self.set_field_values(read_yaml(_defaults_path))
 
     def load_template(self):
         self._environment = Environment(
             loader=FileSystemLoader(self._templates_path))
         template: Template = self._environment.get_template(
             self._template_name)
 
         return template
 
+    def load_native_template(self):
+        self._environment = Environment()
+        template: Template = self._environment.from_string(
+            self._template_string)
+
+        return template
+
     def parse_fields(self):
         template_source = self._environment.loader.get_source(
             self._environment, self._template_name)
         parsed_content = self._environment.parse(template_source)
         return meta.find_undeclared_variables(parsed_content)
 
     def set_field_values(self, field_values: dict):
         for key, value in field_values.items():
             if isinstance(value, dict):
                 self._field_values[key] = json.dumps(value)
             else:
                 self._field_values[key] = str(value)
 
     def execute(self, field_values: dict = {}):
+        if field_values is None:
+            field_values = {}
         _current_field_values = self._field_values
         for key, value in field_values.items():
             if isinstance(value, dict):
                 _current_field_values[key] = json.dumps(value)
             else:
                 _current_field_values[key] = str(value)
```

### Comparing `pdx-0.4.0/src/pdx/agent/tester.py` & `pdx-0.5.0/src/pdx/agent/tester.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os
 import asyncio
-from pdx.agent import AgentBuilder
+from pdx.agent import Agent
 from pdx.utils.rw import read_yaml
 from pdx.logger import logger
 import click
 from pdx.settings import process
 
 
-def prompt_echo_console(prompt_session: list):
-    for _p in prompt_session:
+def prompt_echo_console(prompt_chain: list):
+    for _p in prompt_chain:
         _role: str = _p['role']
         if _role != None:
             click.echo(
                 f'{click.style(f"{_role.upper()} PROMPT", fg="yellow")}')
         click.echo(f"{_p['content']}\n")
 
 
 class AgentTestBuilder:
-    def __init__(self, folder_path: str, agent: AgentBuilder):
+    def __init__(self, folder_path: str, agent: Agent):
         self._folder_path = folder_path
         self._agent = agent
         self._test_cases = self.build_tests()
 
     def build_tests(self):
         test_folder_files = os.listdir(
             os.path.join(self._folder_path, "tests"))
@@ -38,18 +38,18 @@
             test_cases[_test_name] = _test_input
 
         return test_cases
 
     async def run_test(self, _test_name, _test_input):
         logger.echo(f"Running: {_test_name}", event="test")
         _r = await self._agent.aexecute(_test_input)
-        logger.debug(f"Test {_test_name}: prompt\n")
-        if process.debug:
+        logger.verbose(f"Test {_test_name}: prompt\n")
+        if process.verbose:
             prompt_echo_console(_r.metadata.request.prompt)
-        logger.debug(f"Test {_test_name}: completion\n{_r.completion}")
+        logger.verbose(f"Test {_test_name}: completion\n{_r.data}")
 
     async def run_tests(self):
         _test_run_list = []
         for _test_name, _test_input in self._test_cases.items():
             _test_run_list.append(self.run_test(_test_name, _test_input))
         _run_output_list = await asyncio.gather(*_test_run_list)
         return _run_output_list
```

### Comparing `pdx-0.4.0/src/pdx/cli.py` & `pdx-0.5.0/src/pdx/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import os
 import click
-from pdx.version import __version__
+from pdx import pdx_metadata
 from pdx.logger import logger
-from pdx.agent import AgentBuilder
+from pdx.agent import Agent
 from pdx.agent.tester import AgentTestBuilder
 from pdx.settings import Keys, process
 from pdx.commands.create import create_agent
 
 
 @click.group()
-@click.option('--version', is_flag=True, show_default=True, default=False, help='Version of the installed `pdx` package.')
+@click.version_option(pdx_metadata.version, message=f'\n{click.style("PDX", fg="magenta")} installed version: {click.style("%(version)s", fg="magenta")}\n')
 @click.pass_context
-def main(ctx, version: bool):
+def main(ctx):
     ctx.ensure_object(dict)
 
-    if version:
-        click.echo(__version__)
-
 
 @main.command("create")
 @click.argument("agent_name", required=True, type=str)
 @click.option('--template', default='simple', show_default=True, help='Creates an agent with a template. Options: `simple`, `chat`, `tree`.')
 @click.pass_context
 def test(ctx, agent_name: str, template: str):
 
@@ -30,20 +27,19 @@
         _dest = create_agent(agent_name, template)
         logger.echo(f"Agent `{agent_name}` created.")
         logger.echo(f"Agent path: {_dest}")
 
 
 @main.command("test")
 @click.argument("path", required=True, type=str)
-@click.option('--debug', is_flag=True, show_default=True, default=False, help='Enables the logging of all requests and responses to the console.')
+@click.option('-v', '--verbose', is_flag=True, show_default=True, default=False, help='Enables the logging of all requests and responses to the console.')
 @click.option('--report', is_flag=True, show_default=True, default=False, help='Enables the generation of reports of the tests.')
 @click.pass_context
-def test(ctx, path: str, debug: bool, report: bool):
+def test(ctx, path: str, verbose: bool, report: bool):
 
-    if debug:
-        process.debug = True
+    if verbose:
+        process.verbose = True
 
-    api_keys = Keys()
     agent_path = os.path.join(os.getcwd(), path)
-    _agent = AgentBuilder(agent_path, api_keys)
+    _agent = Agent(agent_path)
     _tester = AgentTestBuilder(agent_path, _agent)
     _tester.execute()
```

### Comparing `pdx-0.4.0/src/pdx/commands/create.py` & `pdx-0.5.0/src/pdx/commands/create.py`

 * *Files identical despite different names*

### Comparing `pdx-0.4.0/src/pdx/exceptions.py` & `pdx-0.5.0/src/pdx/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.4.0/src/pdx/logger.py` & `pdx-0.5.0/src/pdx/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 
         if self.options['console_log']:
             if self.options['use_click']:
                 self._click_echo(msg=msg, event=event)
             else:
                 print(msg)
 
-    def debug(self, msg: Union[str, dict], event: str = 'debug'):
+    def verbose(self, msg: Union[str, dict], event: str = 'verbose'):
         '''
         Example usage:            
-            logger.debug(msg="A debug message.")
+            logger.verbose(msg="A verbose message.")
         '''
-        if process.debug:
+        if process.verbose:
             if self.options['console_log']:
                 if self.options['use_click']:
                     self._click_echo(msg=msg, event=event)
                 else:
                     print(msg)
```

### Comparing `pdx-0.4.0/src/pdx/models/anthropic/client.py` & `pdx-0.5.0/src/pdx/models/anthropic/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,30 +83,16 @@
             method,
             abs_url,
             final_headers,
             data,
             stream,
             request_timeout or self.request_timeout,
         )
-    
+
     def _response_middleware(self, response: Union[requests.Response, aiohttp.ClientResponse], content: str) -> dict:
         if isinstance(response, requests.Response):
             if response.status_code != 200:
                 handle_anthropic_request_error(response.status_code, content)
-        
+
         if isinstance(response, aiohttp.ClientResponse):
             if response.status != 200:
                 handle_anthropic_request_error(response.status, content)
-
-    def completion(self, **kwargs) -> dict:
-        return self.request(
-            "post",
-            "v1/complete",
-            params=kwargs,
-        )
-
-    async def acompletion(self, **kwargs) -> dict:
-        return await self.arequest(
-            "post",
-            "v1/complete",
-            params=kwargs,
-        )
```

### Comparing `pdx-0.4.0/src/pdx/models/anthropic/exceptions.py` & `pdx-0.5.0/src/pdx/models/anthropic/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.4.0/src/pdx/models/api_client.py` & `pdx-0.5.0/src/pdx/models/api_client.py`

 * *Files identical despite different names*

### Comparing `pdx-0.4.0/src/pdx/models/openai/__init__.py` & `pdx-0.5.0/src/pdx/models/openai/completion.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from time import time
 from pdx.logger import logger
-from pdx.agent.prompt_session import PromptSession
+from pdx.models.model import Model
+from pdx.prompt.prompt_session import PromptSession
 from pdx.models.openai.client import OpenAIClient
 from pdx.models.metadata import ModelResponse, ResponseMetadata, ModelTokenUsage
-from time import time
 
 
-class OpenAI(object):
+class CompletionModel(Model):
     def __init__(self,
                  api_key: str,
                  model: str,
                  max_tokens: int = 1200,
                  stop: list = ["#", "---"],
                  temperature: float = 0,
                  **kwargs,
@@ -17,95 +18,126 @@
         if model in ["gpt-3.5-turbo", "gpt-4"]:
             self._client_type = "chat"
         elif model in ["text-davinci-003", "text-davinci-002", "davinci", "curie", "babbage", "ada"]:
             self._client_type = "text"
         else:
             raise Exception("Model not supported")
 
+        if self._client_type == "chat":
+            self._api_url = "v1/chat/completions"
+        else:  # self._client_type == "text"
+            self._api_url = "v1/completions"
+
         self._provider = "openai"
         self._client = OpenAIClient(api_key)
         self._model = model
         self._max_tokens = max_tokens
         self._stop = stop
         self._temperature = temperature
         self._top_p = kwargs.get('top_p', 1)
         self._best_of = kwargs.get('best_of', 1)
         self._frequency_penalty = kwargs.get('frequency_penalty', 0)
         self._presence_penalty = kwargs.get('presence_penalty', 0)
+        self._retries = kwargs.get('retries', 2)
 
-    def _preprocess(self, prompt: PromptSession):
+    def _preprocess(self, prompt: PromptSession) -> dict:
         request_params = {
             "model": self._model,
             "max_tokens": self._max_tokens,
             "temperature": self._temperature,
             "top_p": self._top_p,
             "frequency_penalty": self._frequency_penalty,
             "presence_penalty": self._presence_penalty,
             "stop": self._stop
         }
         if self._client_type == "chat":
-            if prompt.type == "text":
-                _prompt_session = prompt.text_to_chat_prompt_openai()
+            if prompt.session_type == "text":
+                _content = prompt.text_prompt({})
+                _chat_prompt = [{"role": "user", "content": _content}]
             else:
-                _prompt_session = prompt.session
-            request_params['messages'] = _prompt_session
+                _chat_prompt = prompt.chat_prompt()
+            request_params['messages'] = _chat_prompt
 
         if self._client_type == "text":
-            if prompt.type == "chat":
-                _prompt_session = prompt.chat_to_text_prompt_openai()
+            if prompt.session_type == "chat":
+                _text_prompt = prompt.text_prompt()
             else:
-                _prompt_session = prompt.stitch_for_text_completion()
-            request_params['prompt'] = _prompt_session
+                _text_prompt = prompt.text_prompt({})
+            request_params['prompt'] = _text_prompt
             request_params['best_of'] = self._best_of
 
         return request_params
 
-    def _postprocess(self, response: dict, request_params: dict, completion_time: float) -> ModelResponse:
+    def _postprocess(self, response: dict, request_params: dict, request_time: float) -> ModelResponse:
         token_usage = ModelTokenUsage(
-            completion=response['usage']['completion_tokens'],
+            response=response['usage']['completion_tokens'],
             prompt=response['usage']['prompt_tokens'],
             total=response['usage']['total_tokens'])
         response_metadata = ResponseMetadata(
             model=response['model'],
             api_log_id=response['id'],
             stop=response['choices'][0]['finish_reason'],
             stop_reason=response['choices'][0]['finish_reason'],
             token_usage=token_usage,
-            completion_time=completion_time)
+            latency=request_time)
 
         if self._client_type == "chat":
             params = {key: value for key,
                       value in request_params.items() if key != 'messages'}
             model_response = ModelResponse(
                 metadata=response_metadata,
                 request_params=params,
-                completion=response['choices'][0]['message']['content'])
+                data=response['choices'][0]['message']['content'])
             return model_response
 
         if self._client_type == "text":
             params = {key: value for key,
                       value in request_params.items() if key != 'prompt'}
             model_response = ModelResponse(
                 metadata=response_metadata,
                 request_params=params,
-                completion=response['choices'][0]['text'])
+                data=response['choices'][0]['text'])
             return model_response
 
-    def run(self, prompt: PromptSession) -> ModelResponse:
+    def execute(self, prompt: PromptSession) -> ModelResponse:
         start_time = time()
         request_params = self._preprocess(prompt)
-        if self._client_type == "chat":
-            _r = self._client.completion_chat(**request_params)
-        if self._client_type == "text":
-            _r = self._client.completion(**request_params)
-        completion_time = time() - start_time
-        return self._postprocess(_r, request_params, completion_time)
 
-    async def arun(self, prompt: PromptSession) -> ModelResponse:
+        _try_count = 0
+        while (_try_count <= self._retries):
+            try:
+                _r = self._client.request(
+                    "post",
+                    self._api_url,
+                    params=request_params,
+                )
+                request_time = time() - start_time
+                return self._postprocess(_r, request_params, request_time)
+            except Exception as e:
+                logger.verbose(
+                    f"{self._provider} {self._model} model failed to run.\nReason: {e}")
+                _try_count += 1
+
+        raise ValueError(
+            f"{self._provider} {self._model} model failed to run successfully.")
+
+    async def aexecute(self, prompt: PromptSession) -> ModelResponse:
         start_time = time()
         request_params = self._preprocess(prompt)
-        if self._client_type == "chat":
-            _r = await self._client.acompletion_chat(**request_params)
-        if self._client_type == "text":
-            _r = await self._client.acompletion(**request_params)
-        completion_time = time() - start_time
-        return self._postprocess(_r, request_params, completion_time)
+
+        _try_count = 0
+        while (_try_count <= self._retries):
+            try:
+                _r = await self._client.arequest(
+                    "post",
+                    self._api_url,
+                    params=request_params,
+                )
+                request_time = time() - start_time
+                return self._postprocess(_r, request_params, request_time)
+            except Exception as e:
+                logger.verbose(
+                    f"{self._provider} {self._model} model failed to run.\nReason: {e}")
+                _try_count += 1
+
+        raise ValueError(
+            f"{self._provider} {self._model} model failed to run successfully.")
```

### Comparing `pdx-0.4.0/src/pdx/models/openai/client.py` & `pdx-0.5.0/src/pdx/models/openai/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
         data = None
         if params:
             if method in {"post"}:
                 data = json.dumps(params).encode()
             else:
                 raise ValueError(f"Unrecognized method: {method}")
-            
-        # If we're requesting a stream from the server, let's tell requests to expect the same
+
+        # TODO: Add support for stream, tell requests if to expect a stream
         stream = params.get("stream", None)
         return APIRequest(
             method,
             abs_url,
             final_headers,
             data,
             stream,
@@ -59,35 +59,7 @@
         if isinstance(response, requests.Response):
             if response.status_code != 200:
                 handle_openai_request_error(response.status_code, content)
 
         if isinstance(response, aiohttp.ClientResponse):
             if response.status != 200:
                 handle_openai_request_error(response.status, content)
-
-    def completion(self, **kwargs) -> dict:
-        return self.request(
-            "post",
-            "v1/completions",
-            params=kwargs,
-        )
-
-    async def acompletion(self, **kwargs) -> dict:
-        return await self.arequest(
-            "post",
-            "v1/completions",
-            params=kwargs,
-        )
-    
-    def completion_chat(self, **kwargs) -> dict:
-        return self.request(
-            "post",
-            "v1/chat/completions",
-            params=kwargs,
-        )
-
-    async def acompletion_chat(self, **kwargs) -> dict:
-        return await self.arequest(
-            "post",
-            "v1/chat/completions",
-            params=kwargs,
-        )
```

### Comparing `pdx-0.4.0/src/pdx/models/openai/exceptions.py` & `pdx-0.5.0/src/pdx/models/openai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdx-0.4.0/src/pdx/utils/rw.py` & `pdx-0.5.0/src/pdx/utils/rw.py`

 * *Files identical despite different names*

### Comparing `pdx-0.4.0/PKG-INFO` & `pdx-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdx
-Version: 0.4.0
+Version: 0.5.0
 Summary: Prompt Engineering and Dev-Ops toolkits. A faster way to build and manage applications powered by Language Models.
 License: Apache-2.0
 Keywords: prompt,LLM,prompt engineering,dev-ops,observability,apps
 Author: Adithya Krishnan
 Author-email: krishsandeep@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
@@ -51,15 +51,15 @@
 ```bash
 pdx create my_first_agent
 ```
 
 Run and test out the agent by running:
 
 ```bash
-pdx test my_first_agent --debug
+pdx test my_first_agent --verbose
 ```
 
 More information here: [PDX - Main Concepts](https://pdxlabs.io/docs/getting-started/main-concepts)
 
 ## Why use PDX?
 
 -   🗃️ Low dependency footprint -> ease of production deployment and maintainance.
```

