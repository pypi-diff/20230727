# Comparing `tmp/wxai-langchain-0.0.1.tar.gz` & `tmp/wxai-langchain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxai-langchain-0.0.1.tar", last modified: Thu Jul 27 10:30:19 2023, max compression
+gzip compressed data, was "wxai-langchain-0.0.2.tar", last modified: Thu Jul 27 10:46:50 2023, max compression
```

## Comparing `wxai-langchain-0.0.1.tar` & `wxai-langchain-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 10:30:19.550000 wxai-langchain-0.0.1/
--rw-rw-rw-   0        0        0     3237 2023-07-27 10:11:54.000000 wxai-langchain-0.0.1/.gitignore
--rw-rw-rw-   0        0        0    11525 2023-07-27 09:46:48.000000 wxai-langchain-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      781 2023-07-27 10:30:20.000000 wxai-langchain-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-07-27 10:24:30.000000 wxai-langchain-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 10:30:19.550000 wxai-langchain-0.0.1/examples/
--rw-rw-rw-   0        0        0    17252 2023-07-27 10:24:02.000000 wxai-langchain-0.0.1/examples/wxai_langchain_interface.ipynb
--rw-rw-rw-   0        0        0      798 2023-07-27 10:22:52.000000 wxai-langchain-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-27 10:30:20.000000 wxai-langchain-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-27 10:30:19.550000 wxai-langchain-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 10:30:19.550000 wxai-langchain-0.0.1/src/wxai_langchain/
--rw-rw-rw-   0        0        0      157 2023-07-27 10:02:04.000000 wxai-langchain-0.0.1/src/wxai_langchain/__init__.py
--rw-rw-rw-   0        0        0     1204 2023-07-27 09:34:42.000000 wxai-langchain-0.0.1/src/wxai_langchain/credentials.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:30:19.550000 wxai-langchain-0.0.1/src/wxai_langchain/extensions/
--rw-rw-rw-   0        0        0        0 2023-07-27 09:34:42.000000 wxai-langchain-0.0.1/src/wxai_langchain/extensions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:30:19.560000 wxai-langchain-0.0.1/src/wxai_langchain/extensions/langchain/
--rw-rw-rw-   0        0        0        0 2023-07-27 09:34:42.000000 wxai-langchain-0.0.1/src/wxai_langchain/extensions/langchain/__init__.py
--rw-rw-rw-   0        0        0     2822 2023-07-27 09:34:42.000000 wxai-langchain-0.0.1/src/wxai_langchain/extensions/langchain/llm.py
--rw-rw-rw-   0        0        0      875 2023-07-27 09:34:42.000000 wxai-langchain-0.0.1/src/wxai_langchain/extensions/langchain/prompt.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:30:19.550000 wxai-langchain-0.0.1/src/wxai_langchain.egg-info/
--rw-rw-rw-   0        0        0      781 2023-07-27 10:30:20.000000 wxai-langchain-0.0.1/src/wxai_langchain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-07-27 10:30:20.000000 wxai-langchain-0.0.1/src/wxai_langchain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 10:30:20.000000 wxai-langchain-0.0.1/src/wxai_langchain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-07-27 10:30:20.000000 wxai-langchain-0.0.1/src/wxai_langchain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 10:30:20.000000 wxai-langchain-0.0.1/src/wxai_langchain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 10:46:50.320000 wxai-langchain-0.0.2/
+-rw-rw-rw-   0        0        0     3237 2023-07-27 10:11:54.000000 wxai-langchain-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0    11525 2023-07-27 09:46:48.000000 wxai-langchain-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      781 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2023-07-27 10:24:30.000000 wxai-langchain-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 10:46:50.330000 wxai-langchain-0.0.2/examples/
+-rw-rw-rw-   0        0        0    17233 2023-07-27 10:45:34.000000 wxai-langchain-0.0.2/examples/wxai_langchain_interface.ipynb
+-rw-rw-rw-   0        0        0      798 2023-07-27 10:46:38.000000 wxai-langchain-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 10:46:50.330000 wxai-langchain-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 10:46:50.330000 wxai-langchain-0.0.2/src/wxai_langchain/
+-rw-rw-rw-   0        0        0      157 2023-07-27 10:02:04.000000 wxai-langchain-0.0.2/src/wxai_langchain/__init__.py
+-rw-rw-rw-   0        0        0     1204 2023-07-27 09:34:42.000000 wxai-langchain-0.0.2/src/wxai_langchain/credentials.py
+-rw-rw-rw-   0        0        0     2316 2023-07-27 10:45:16.000000 wxai-langchain-0.0.2/src/wxai_langchain/llm.py
+-rw-rw-rw-   0        0        0      875 2023-07-27 09:34:42.000000 wxai-langchain-0.0.2/src/wxai_langchain/prompt.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:46:50.330000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/
+-rw-rw-rw-   0        0        0      781 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-27 10:46:52.000000 wxai-langchain-0.0.2/src/wxai_langchain.egg-info/top_level.txt
```

### Comparing `wxai-langchain-0.0.1/.gitignore` & `wxai-langchain-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `wxai-langchain-0.0.1/LICENSE` & `wxai-langchain-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wxai-langchain-0.0.1/PKG-INFO` & `wxai-langchain-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxai-langchain
-Version: 0.0.1
+Version: 0.0.2
 Summary: wxai-langchain enables the use of IBM watsonx.ai in LangChain projects. This is not supported by IBM.
 Author-email: Cong Nguyen <cong.nguyen@au1.ibm.com>
 Keywords: watsonx.ai,wxai,langchain
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wxai-langchain-0.0.1/examples/wxai_langchain_interface.ipynb` & `wxai-langchain-0.0.2/examples/wxai_langchain_interface.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995138888888889%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'name': 'stdout'}}}, 3: {'outputs': {0: {'name': 'stdout'}}}, 5: "*

 * *            "{'source': {insert: [(0, 'from wxai_langchain.llm import LangChainInterface\\n')], "*

 * *            'delete: [0]}}}'}*

```diff
@@ -116,15 +116,15 @@
                     "end_time": "2023-07-27T10:03:56.804542800Z",
                     "start_time": "2023-07-27T10:03:53.083266Z"
                 },
                 "tags": []
             },
             "outputs": [
                 {
-                    "name": "stdin",
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " \u00b7\u00b7\u00b7\u00b7\u00b7\u00b7\u00b7\u00b7\n"
                     ]
                 }
             ],
             "source": [
@@ -140,15 +140,15 @@
                     "end_time": "2023-07-27T10:04:00.252474Z",
                     "start_time": "2023-07-27T10:03:56.777540800Z"
                 },
                 "tags": []
             },
             "outputs": [
                 {
-                    "name": "stdin",
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " \u00b7\u00b7\u00b7\u00b7\u00b7\u00b7\u00b7\u00b7\n"
                     ]
                 }
             ],
             "source": [
@@ -180,15 +180,15 @@
                     "end_time": "2023-07-27T10:05:36.911412Z",
                     "start_time": "2023-07-27T10:05:36.873412800Z"
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "from wxai_langchain.extensions.langchain.llm import LangChainInterface\n",
+                "from wxai_langchain.llm import LangChainInterface\n",
                 "from wxai_langchain.credentials import Credentials\n",
                 "\n",
                 "creds = Credentials(api_key=api_key, project_id=project_id, api_endpoint=api_endpoint)\n",
                 "\n",
                 "parameters = {\n",
                 "    \"decoding_method\": \"sample\",\n",
                 "    \"max_new_tokens\": 100,\n",
```

### Comparing `wxai-langchain-0.0.1/pyproject.toml` & `wxai-langchain-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0.0", "wheel>=0.40.0", "setuptools_scm[toml]>=7.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wxai-langchain"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   {name="Cong Nguyen", email="cong.nguyen@au1.ibm.com"}
 ]
 keywords = ["watsonx.ai", "wxai", "langchain"]
 description = "wxai-langchain enables the use of IBM watsonx.ai in LangChain projects. This is not supported by IBM."
 readme = "README.md"
 dependencies = [
```

### Comparing `wxai-langchain-0.0.1/src/wxai_langchain/credentials.py` & `wxai-langchain-0.0.2/src/wxai_langchain/credentials.py`

 * *Files identical despite different names*

### Comparing `wxai-langchain-0.0.1/src/wxai_langchain/extensions/langchain/llm.py` & `wxai-langchain-0.0.2/src/wxai_langchain/llm.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,36 +6,26 @@
 
 try:
     from langchain.llms.base import LLM
     from langchain.llms.utils import enforce_stop_tokens
 except ImportError:
     raise ImportError("Could not import langchain: Please install langchain.")
 
-try:
-    from genai.schemas import GenerateParams
-except ImportError:
-    raise ImportError("Could not import genai: Please install ibm-generative-ai")
-
 from wxai_langchain.credentials import Credentials
-from wxai_langchain.extensions.langchain.prompt import Prompt
+from wxai_langchain.prompt import Prompt
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["LangChainInterface"]
 
 
 class LangChainInterface(LLM, BaseModel):
     """
     Wrapper around IBM watsonx.ai models.
-    To use, you should have the ``genai`` python package installed
-    and initialize the credentials attribute of this class with
-    an instance of ``genai.Credentials``. Model specific parameters
-    can be passed through to the constructor using the ``params``
-    parameter, which is an instance of GenerateParams.
-    Example:
+
         .. code-block:: python
             llm = LangChainInterface(model="google/flan-ul2", credentials=creds)
     """
 
     credentials: Credentials = None
     model: Optional[str] = None
     params: Optional[dict] = None
```

### Comparing `wxai-langchain-0.0.1/src/wxai_langchain/extensions/langchain/prompt.py` & `wxai-langchain-0.0.2/src/wxai_langchain/prompt.py`

 * *Files identical despite different names*

### Comparing `wxai-langchain-0.0.1/src/wxai_langchain.egg-info/PKG-INFO` & `wxai-langchain-0.0.2/src/wxai_langchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxai-langchain
-Version: 0.0.1
+Version: 0.0.2
 Summary: wxai-langchain enables the use of IBM watsonx.ai in LangChain projects. This is not supported by IBM.
 Author-email: Cong Nguyen <cong.nguyen@au1.ibm.com>
 Keywords: watsonx.ai,wxai,langchain
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

