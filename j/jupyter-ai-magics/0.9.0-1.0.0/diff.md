# Comparing `tmp/jupyter_ai_magics-0.9.0.tar.gz` & `tmp/jupyter_ai_magics-1.0.0.tar.gz`

## Comparing `jupyter_ai_magics-0.9.0.tar` & `jupyter_ai_magics-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/setup.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/aliases.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/embedding_providers.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/exception.py
--rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/parsers.py
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/README.md
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/setup.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/aliases.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/embedding_providers.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/parsers.py
+-rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/README.md
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/PKG-INFO
```

### Comparing `jupyter_ai_magics-0.9.0/package.json` & `jupyter_ai_magics-1.0.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'1.0.0'"}*

```diff
@@ -16,9 +16,9 @@
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
         "dev-install": "pip install -e \".[dev,all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y"
     },
-    "version": "0.9.0"
+    "version": "1.0.0"
 }
```

### Comparing `jupyter_ai_magics-0.9.0/jupyter_ai_magics/__init__.py` & `jupyter_ai_magics-1.0.0/jupyter_ai_magics/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .magics import AiMagics
 
 # expose model providers on the package root
 from .providers import (
     AI21Provider,
     AnthropicProvider,
     BaseProvider,
+    BedrockProvider,
     ChatOpenAINewProvider,
     ChatOpenAIProvider,
     CohereProvider,
     HfHubProvider,
     OpenAIProvider,
     SmEndpointProvider,
 )
```

### Comparing `jupyter_ai_magics-0.9.0/jupyter_ai_magics/embedding_providers.py` & `jupyter_ai_magics-1.0.0/jupyter_ai_magics/embedding_providers.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,49 +34,57 @@
 
     auth_strategy: ClassVar[AuthStrategy] = None
     """Authentication/authorization strategy. Declares what credentials are
     required to use this model provider. Generally should not be `None`."""
 
     model_id: str
 
-    provider_klass: ClassVar[Type[Embeddings]]
-
     registry: ClassVar[bool] = False
     """Whether this provider is a registry provider."""
 
     fields: ClassVar[List[Field]] = []
     """Fields expected by this provider in its constructor. Each `Field` `f`
     should be passed as a keyword argument, keyed by `f.key`."""
 
+    def __init__(self, *args, **kwargs):
+        try:
+            assert kwargs["model_id"]
+        except:
+            raise AssertionError(
+                "model_id was not specified. Please specify it as a keyword argument."
+            )
+
+        model_kwargs = {}
+        model_kwargs[self.__class__.model_id_key] = kwargs["model_id"]
+
+        super().__init__(*args, **kwargs, **model_kwargs)
+
 
-class OpenAIEmbeddingsProvider(BaseEmbeddingsProvider):
+class OpenAIEmbeddingsProvider(BaseEmbeddingsProvider, OpenAIEmbeddings):
     id = "openai"
     name = "OpenAI"
     models = ["text-embedding-ada-002"]
     model_id_key = "model"
     pypi_package_deps = ["openai"]
     auth_strategy = EnvAuthStrategy(name="OPENAI_API_KEY")
-    provider_klass = OpenAIEmbeddings
 
 
-class CohereEmbeddingsProvider(BaseEmbeddingsProvider):
+class CohereEmbeddingsProvider(BaseEmbeddingsProvider, CohereEmbeddings):
     id = "cohere"
     name = "Cohere"
     models = ["large", "multilingual-22-12", "small"]
     model_id_key = "model"
     pypi_package_deps = ["cohere"]
     auth_strategy = EnvAuthStrategy(name="COHERE_API_KEY")
-    provider_klass = CohereEmbeddings
 
 
-class HfHubEmbeddingsProvider(BaseEmbeddingsProvider):
+class HfHubEmbeddingsProvider(BaseEmbeddingsProvider, HuggingFaceHubEmbeddings):
     id = "huggingface_hub"
-    name = "HuggingFace Hub"
+    name = "Hugging Face Hub"
     models = ["*"]
     model_id_key = "repo_id"
     # ipywidgets needed to suppress tqdm warning
     # https://stackoverflow.com/questions/67998191
     # tqdm is a dependency of huggingface_hub
     pypi_package_deps = ["huggingface_hub", "ipywidgets"]
     auth_strategy = EnvAuthStrategy(name="HUGGINGFACEHUB_API_TOKEN")
-    provider_klass = HuggingFaceHubEmbeddings
     registry = True
```

### Comparing `jupyter_ai_magics-0.9.0/jupyter_ai_magics/exception.py` & `jupyter_ai_magics-1.0.0/jupyter_ai_magics/exception.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.9.0/jupyter_ai_magics/magics.py` & `jupyter_ai_magics-1.0.0/jupyter_ai_magics/magics.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import warnings
 from typing import Optional
 
 import click
 from IPython import get_ipython
 from IPython.core.magic import Magics, line_cell_magic, magics_class
 from IPython.display import HTML, JSON, Markdown, Math
-from jupyter_ai_magics.utils import decompose_model_id, load_providers
+from jupyter_ai_magics.utils import decompose_model_id, get_lm_providers
 from langchain.chains import LLMChain
 
 from .parsers import (
     CellArgs,
     DeleteArgs,
     ErrorArgs,
     HelpArgs,
@@ -134,35 +134,41 @@
         warnings.filterwarnings(
             "ignore",
             message="You are trying to use a chat model. This way of initializing it is "
             "no longer supported. Instead, please use: "
             "`from langchain.chat_models import ChatOpenAI`",
         )
 
-        self.providers = load_providers()
+        self.providers = get_lm_providers()
 
         # initialize a registry of custom model/chain names
         self.custom_model_registry = MODEL_ID_ALIASES
 
     def _ai_bulleted_list_models_for_provider(self, provider_id, Provider):
         output = ""
         if len(Provider.models) == 1 and Provider.models[0] == "*":
-            output += f"* {PROVIDER_NO_MODELS}\n"
+            if Provider.help is None:
+                output += f"* {PROVIDER_NO_MODELS}\n"
+            else:
+                output += f"* {Provider.help}\n"
         else:
             for model_id in Provider.models:
                 output += f"* {provider_id}:{model_id}\n"
         output += "\n"  # End of bulleted list
 
         return output
 
     def _ai_inline_list_models_for_provider(self, provider_id, Provider):
         output = ""
 
         if len(Provider.models) == 1 and Provider.models[0] == "*":
-            return PROVIDER_NO_MODELS
+            if Provider.help is None:
+                return PROVIDER_NO_MODELS
+            else:
+                return Provider.help
 
         for model_id in Provider.models:
             output += f", `{provider_id}:{model_id}`"
 
         # Remove initial comma
         return re.sub(r"^, ", "", output)
 
@@ -520,14 +526,23 @@
                     "When using the sagemaker-endpoint provider, you must specify all of "
                     + "the --region-name, --request-schema, and --response-path options."
                 )
             provider_params["region_name"] = args.region_name
             provider_params["request_schema"] = args.request_schema
             provider_params["response_path"] = args.response_path
 
+            # Validate that the request schema is well-formed JSON
+            try:
+                json.loads(args.request_schema)
+            except json.JSONDecodeError as e:
+                raise ValueError(
+                    "request-schema must be valid JSON. "
+                    f"Error at line {e.lineno}, column {e.colno}: {e.msg}"
+                ) from None
+
         provider = Provider(**provider_params)
 
         # generate output from model via provider
         result = provider.generate([prompt])
         output = result.generations[0][0].text
 
         # if openai-chat, append exchange to transcript
```

### Comparing `jupyter_ai_magics-0.9.0/jupyter_ai_magics/parsers.py` & `jupyter_ai_magics-1.0.0/jupyter_ai_magics/parsers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.9.0/jupyter_ai_magics/providers.py` & `jupyter_ai_magics-1.0.0/jupyter_ai_magics/providers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+import asyncio
 import base64
 import copy
+import functools
 import io
 import json
-from typing import Any, ClassVar, Dict, List, Literal, Optional, Union
+from concurrent.futures import ThreadPoolExecutor
+from typing import Any, ClassVar, Coroutine, Dict, List, Literal, Optional, Union
 
-from jsonpath_ng import jsonpath, parse
+from jsonpath_ng import parse
 from langchain.chat_models import ChatOpenAI
 from langchain.llms import (
     AI21,
     Anthropic,
+    Bedrock,
     Cohere,
     HuggingFaceHub,
     OpenAI,
     OpenAIChat,
     SagemakerEndpoint,
 )
 from langchain.llms.sagemaker_endpoint import LLMContentHandler
 from langchain.llms.utils import enforce_stop_tokens
-from langchain.schema import BaseModel as BaseLangchainProvider
 from langchain.utils import get_from_dict_or_env
 from pydantic import BaseModel, Extra, root_validator
 
 
 class EnvAuthStrategy(BaseModel):
     """Require one auth token via an environment variable."""
 
@@ -47,30 +50,33 @@
         EnvAuthStrategy,
         MultiEnvAuthStrategy,
         AwsAuthStrategy,
     ]
 ]
 
 
-class TextField(BaseModel):
-    type: Literal["text"] = "text"
+class Field(BaseModel):
     key: str
     label: str
+    # "text" accepts any text
+    format: Literal["json", "jsonpath", "text"]
+
+
+class TextField(Field):
+    type: Literal["text"] = "text"
 
 
-class MultilineTextField(BaseModel):
+class MultilineTextField(Field):
     type: Literal["text-multiline"] = "text-multiline"
-    key: str
-    label: str
 
 
 Field = Union[TextField, MultilineTextField]
 
 
-class BaseProvider(BaseLangchainProvider):
+class BaseProvider(BaseModel):
     #
     # pydantic config
     #
     class Config:
         extra = Extra.allow
 
     #
@@ -82,14 +88,18 @@
     name: ClassVar[str] = ...
     """User-facing name of this provider."""
 
     models: ClassVar[List[str]] = ...
     """List of supported models by their IDs. For registry providers, this will
     be just ["*"]."""
 
+    help: ClassVar[str] = None
+    """Text to display in lieu of a model list for a registry provider that does
+    not provide a list of models."""
+
     model_id_key: ClassVar[str] = ...
     """Kwarg expected by the upstream LangChain provider."""
 
     pypi_package_deps: ClassVar[List[str]] = []
     """List of PyPi package dependencies."""
 
     auth_strategy: ClassVar[AuthStrategy] = None
@@ -113,18 +123,29 @@
             assert kwargs["model_id"]
         except:
             raise AssertionError(
                 "model_id was not specified. Please specify it as a keyword argument."
             )
 
         model_kwargs = {}
-        model_kwargs[self.__class__.model_id_key] = kwargs["model_id"]
+        if self.__class__.model_id_key != "model_id":
+            model_kwargs[self.__class__.model_id_key] = kwargs["model_id"]
 
         super().__init__(*args, **kwargs, **model_kwargs)
 
+    async def _call_in_executor(self, *args, **kwargs) -> Coroutine[Any, Any, str]:
+        """
+        Calls self._call() asynchronously in a separate thread for providers
+        without an async implementation. Requires the event loop to be running.
+        """
+        executor = ThreadPoolExecutor(max_workers=1)
+        loop = asyncio.get_running_loop()
+        _call_with_args = functools.partial(self._call, *args, **kwargs)
+        return await loop.run_in_executor(executor, _call_with_args)
+
 
 class AI21Provider(BaseProvider, AI21):
     id = "ai21"
     name = "AI21"
     models = [
         "j1-large",
         "j1-grande",
@@ -136,14 +157,17 @@
         "j2-grande-instruct",
         "j2-jumbo-instruct",
     ]
     model_id_key = "model"
     pypi_package_deps = ["ai21"]
     auth_strategy = EnvAuthStrategy(name="AI21_API_KEY")
 
+    async def _acall(self, *args, **kwargs) -> Coroutine[Any, Any, str]:
+        return await self._call_in_executor(*args, **kwargs)
+
 
 class AnthropicProvider(BaseProvider, Anthropic):
     id = "anthropic"
     name = "Anthropic"
     models = [
         "claude-v1",
         "claude-v1.0",
@@ -160,27 +184,34 @@
     id = "cohere"
     name = "Cohere"
     models = ["medium", "xlarge"]
     model_id_key = "model"
     pypi_package_deps = ["cohere"]
     auth_strategy = EnvAuthStrategy(name="COHERE_API_KEY")
 
+    async def _acall(self, *args, **kwargs) -> Coroutine[Any, Any, str]:
+        return await self._call_in_executor(*args, **kwargs)
+
 
 HUGGINGFACE_HUB_VALID_TASKS = (
     "text2text-generation",
     "text-generation",
     "text-to-image",
 )
 
 
 class HfHubProvider(BaseProvider, HuggingFaceHub):
     id = "huggingface_hub"
-    name = "HuggingFace Hub"
+    name = "Hugging Face Hub"
     models = ["*"]
     model_id_key = "repo_id"
+    help = (
+        "See https://huggingface.co/models for a list of models. "
+        "Pass a model's repository ID as the model ID; for example, `huggingface_hub:ExampleOwner/example-model`."
+    )
     # ipywidgets needed to suppress tqdm warning
     # https://stackoverflow.com/questions/67998191
     # tqdm is a dependency of huggingface_hub
     pypi_package_deps = ["huggingface_hub", "ipywidgets"]
     auth_strategy = EnvAuthStrategy(name="HUGGINGFACEHUB_API_TOKEN")
     registry = True
 
@@ -211,15 +242,15 @@
                 "Could not import huggingface_hub python package. "
                 "Please install it with `pip install huggingface_hub`."
             )
         return values
 
     # Handle image outputs
     def _call(self, prompt: str, stop: Optional[List[str]] = None) -> str:
-        """Call out to HuggingFace Hub's inference endpoint.
+        """Call out to Hugging Face Hub's inference endpoint.
 
         Args:
             prompt: The prompt to pass into the model.
             stop: Optional list of stop words to use when generating.
 
         Returns:
             The string or image generated by the model.
@@ -265,14 +296,17 @@
             )
         if stop is not None:
             # This is a bit hacky, but I can't figure out a better way to enforce
             # stop tokens when making calls to huggingface_hub.
             text = enforce_stop_tokens(text, stop)
         return text
 
+    async def _acall(self, *args, **kwargs) -> Coroutine[Any, Any, str]:
+        return await self._call_in_executor(*args, **kwargs)
+
 
 class OpenAIProvider(BaseProvider, OpenAI):
     id = "openai"
     name = "OpenAI"
     models = [
         "text-davinci-003",
         "text-davinci-002",
@@ -358,35 +392,55 @@
         response_json = json.loads(output.read().decode("utf-8"))
         matches = self.response_parser.find(response_json)
         return matches[0].value
 
 
 class SmEndpointProvider(BaseProvider, SagemakerEndpoint):
     id = "sagemaker-endpoint"
-    name = "Sagemaker Endpoint"
+    name = "SageMaker endpoint"
     models = ["*"]
     model_id_key = "endpoint_name"
+    # This all needs to be on one line of markdown, for use in a table
+    help = (
+        "Specify an endpoint name as the model ID. "
+        "In addition, you must include the `--region_name`, `--request_schema`, and the `--response_path` arguments. "
+        "For more information, see the documentation about [SageMaker endpoints deployment](https://docs.aws.amazon.com/sagemaker/latest/dg/realtime-endpoints-deployment.html) "
+        "and about [using magic commands with SageMaker endpoints](https://jupyter-ai.readthedocs.io/en/latest/users/index.html#using-magic-commands-with-sagemaker-endpoints)."
+    )
+
     pypi_package_deps = ["boto3"]
     auth_strategy = AwsAuthStrategy()
     registry = True
     fields = [
-        TextField(
-            key="region_name",
-            label="Region name",
-        ),
-        MultilineTextField(
-            key="request_schema",
-            label="Request schema",
-        ),
-        TextField(
-            key="response_path",
-            label="Response path",
-        ),
+        TextField(key="region_name", label="Region name", format="text"),
+        MultilineTextField(key="request_schema", label="Request schema", format="json"),
+        TextField(key="response_path", label="Response path", format="jsonpath"),
     ]
 
     def __init__(self, *args, **kwargs):
         request_schema = kwargs.pop("request_schema")
         response_path = kwargs.pop("response_path")
         content_handler = JsonContentHandler(
             request_schema=request_schema, response_path=response_path
         )
         super().__init__(*args, **kwargs, content_handler=content_handler)
+
+    async def _acall(self, *args, **kwargs) -> Coroutine[Any, Any, str]:
+        return await self._call_in_executor(*args, **kwargs)
+
+
+class BedrockProvider(BaseProvider, Bedrock):
+    id = "bedrock"
+    name = "Amazon Bedrock"
+    models = [
+        "amazon.titan-tg1-large",
+        "anthropic.claude-v1",
+        "anthropic.claude-instant-v1",
+        "ai21.j2-jumbo-instruct",
+        "ai21.j2-grande-instruct",
+    ]
+    model_id_key = "model_id"
+    pypi_package_deps = ["boto3"]
+    auth_strategy = AwsAuthStrategy()
+
+    async def _acall(self, *args, **kwargs) -> Coroutine[Any, Any, str]:
+        return await self._call_in_executor(*args, **kwargs)
```

### Comparing `jupyter_ai_magics-0.9.0/.gitignore` & `jupyter_ai_magics-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.9.0/LICENSE` & `jupyter_ai_magics-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.9.0/pyproject.toml` & `jupyter_ai_magics-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 dependencies = [
     "ipython",
     "pydantic",
     "importlib_metadata~=5.2.0",
-    "langchain==0.0.159",
+    "langchain==0.0.220",
     "typing_extensions==4.5.0",
     "click~=8.0",
     "jsonpath-ng~=1.5.3",
 ]
 
 [project.optional-dependencies]
 dev = [
@@ -40,15 +40,15 @@
     "pytest",
     "pytest-asyncio",
     "pytest-cov"
 ]
 
 all = [
     "ai21",
-    "anthropic",
+    "anthropic~=0.2.10",
     "cohere",
     "huggingface_hub",
     "ipywidgets",
     "pillow",
     "openai",
     "boto3"
 ]
@@ -58,14 +58,15 @@
 anthropic = "jupyter_ai_magics:AnthropicProvider"
 cohere = "jupyter_ai_magics:CohereProvider"
 huggingface_hub = "jupyter_ai_magics:HfHubProvider"
 openai = "jupyter_ai_magics:OpenAIProvider"
 openai-chat = "jupyter_ai_magics:ChatOpenAIProvider"
 openai-chat-new = "jupyter_ai_magics:ChatOpenAINewProvider"
 sagemaker-endpoint = "jupyter_ai_magics:SmEndpointProvider"
+amazon-bedrock = "jupyter_ai_magics:BedrockProvider"
 
 [project.entry-points."jupyter_ai.embeddings_model_providers"]
 cohere = "jupyter_ai_magics:CohereEmbeddingsProvider"
 huggingface_hub = "jupyter_ai_magics:HfHubEmbeddingsProvider"
 openai = "jupyter_ai_magics:OpenAIEmbeddingsProvider"
 
 [tool.hatch.version]
```

### Comparing `jupyter_ai_magics-0.9.0/PKG-INFO` & `jupyter_ai_magics-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 0.9.0
+Version: 1.0.0
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -45,20 +45,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: click~=8.0
 Requires-Dist: importlib-metadata~=5.2.0
 Requires-Dist: ipython
 Requires-Dist: jsonpath-ng~=1.5.3
-Requires-Dist: langchain==0.0.159
+Requires-Dist: langchain==0.0.220
 Requires-Dist: pydantic
 Requires-Dist: typing-extensions==4.5.0
 Provides-Extra: all
 Requires-Dist: ai21; extra == 'all'
-Requires-Dist: anthropic; extra == 'all'
+Requires-Dist: anthropic~=0.2.10; extra == 'all'
 Requires-Dist: boto3; extra == 'all'
 Requires-Dist: cohere; extra == 'all'
 Requires-Dist: huggingface-hub; extra == 'all'
 Requires-Dist: ipywidgets; extra == 'all'
 Requires-Dist: openai; extra == 'all'
 Requires-Dist: pillow; extra == 'all'
 Provides-Extra: dev
```

