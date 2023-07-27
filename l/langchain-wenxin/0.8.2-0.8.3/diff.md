# Comparing `tmp/langchain_wenxin-0.8.2.tar.gz` & `tmp/langchain_wenxin-0.8.3.tar.gz`

## Comparing `langchain_wenxin-0.8.2.tar` & `langchain_wenxin-0.8.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/examples/Langchain_wenxin_retrieval_qa_compared.ipynb
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/src/langchain_wenxin/__about__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/src/langchain_wenxin/__init__.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/src/langchain_wenxin/chat_models.py
--rw-r--r--   0        0        0    11065 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/src/langchain_wenxin/client.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/src/langchain_wenxin/embeddings.py
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/src/langchain_wenxin/llms.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/src/langchain_wenxin/retrievers.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/tests/integration_tests/chat_models/__init__.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/tests/integration_tests/chat_models/test_wenxin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/tests/integration_tests/embeddings/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/tests/integration_tests/embeddings/test_wenxin.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/tests/integration_tests/llms/__init__.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/tests/integration_tests/llms/test_wenxin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/tests/tools/__init__.py
--rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/tests/tools/test_callbacks.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/LICENSE.txt
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/README.md
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/examples/Langchain_wenxin_retrieval_qa_compared.ipynb
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/__about__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/__init__.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/chat_models.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/client.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/embeddings.py
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/llms.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/src/langchain_wenxin/retrievers.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/chat_models/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/chat_models/test_wenxin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/embeddings/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/embeddings/test_wenxin.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/llms/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/integration_tests/llms/test_wenxin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/tools/__init__.py
+-rw-r--r--   0        0        0     7616 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/tests/tools/test_callbacks.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/LICENSE.txt
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/README.md
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 langchain_wenxin-0.8.3/PKG-INFO
```

### Comparing `langchain_wenxin-0.8.2/examples/Langchain_wenxin_retrieval_qa_compared.ipynb` & `langchain_wenxin-0.8.3/examples/Langchain_wenxin_retrieval_qa_compared.ipynb`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/src/langchain_wenxin/chat_models.py` & `langchain_wenxin-0.8.3/src/langchain_wenxin/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/src/langchain_wenxin/client.py` & `langchain_wenxin-0.8.3/src/langchain_wenxin/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,20 @@
         self.request_timeout = request_timeout
 
         self.access_token = ""
         self.access_token_expires = 0
 
     def completions_url(self, model: str) -> str:
         """Get the URL for the completions endpoint."""
-        endpoint = "completions"
         if model in ["eb-instant", "ernie-bot-turbo"]:
             endpoint = "eb-instant"
+        elif model in  ["wenxin", "ernie-bot"]:
+            endpoint = "completions"
+        else:
+            endpoint = model
         return self.WENXIN_CHAT_URL.format(endpoint=endpoint)
 
     def grant_token(self) -> str:
         """Grant access token from Baidu Cloud."""
         now_timestamp = int(time.time())
         if self.access_token and now_timestamp < self.access_token_expires:
             return self.access_token
```

### Comparing `langchain_wenxin-0.8.2/src/langchain_wenxin/embeddings.py` & `langchain_wenxin-0.8.3/src/langchain_wenxin/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/src/langchain_wenxin/llms.py` & `langchain_wenxin-0.8.3/src/langchain_wenxin/llms.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class BaiduCommon(BaseModel):
     client: Any = None  #: :meta private:
     model: str = "ernie-bot"
-    """Model name to use. supported models: ernie-bot(wenxin)/ernie-bot-turbo(eb-instant)"""
+    """Model name to use. supported models: ernie-bot(wenxin)/ernie-bot-turbo(eb-instant)/other endpoints"""
 
     temperature: Optional[float] = None
     """A non-negative float that tunes the degree of randomness in generation. Model default is 0.95.
     range: (0.0, 1.0]."""
 
     penalty_score: Optional[float] = None
     """Repeating punishment involves penalizing already generated tokens to reduce the occurrence of repetition.
```

### Comparing `langchain_wenxin-0.8.2/src/langchain_wenxin/retrievers.py` & `langchain_wenxin-0.8.3/src/langchain_wenxin/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/tests/integration_tests/chat_models/test_wenxin.py` & `langchain_wenxin-0.8.3/tests/integration_tests/chat_models/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/tests/integration_tests/embeddings/test_wenxin.py` & `langchain_wenxin-0.8.3/tests/integration_tests/embeddings/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/tests/integration_tests/llms/test_wenxin.py` & `langchain_wenxin-0.8.3/tests/integration_tests/llms/test_wenxin.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/tests/tools/test_callbacks.py` & `langchain_wenxin-0.8.3/tests/tools/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/.gitignore` & `langchain_wenxin-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/LICENSE.txt` & `langchain_wenxin-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/README.md` & `langchain_wenxin-0.8.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
 Support models:
 
 - ernie-bot: Standard model, <https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11>
     - Also named `wenxin` for compatibility.
 - ernie-bot-turbo: Fast model, <https://cloud.baidu.com/doc/WENXINWORKSHOP/s/4lilb2lpf>
     - Also named `eb-instant` for compatibility.
+- other endpoints: eg: bloomz_7b1 or other custom endpoint.
 
 ## Development
 
 ```bash
 # Create virtual environment
 hatch env create
 # Activate virtual environment
```

### Comparing `langchain_wenxin-0.8.2/pyproject.toml` & `langchain_wenxin-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_wenxin-0.8.2/PKG-INFO` & `langchain_wenxin-0.8.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-wenxin
-Version: 0.8.2
+Version: 0.8.3
 Project-URL: Documentation, https://github.com/ninehills/langchain-wenxin#readme
 Project-URL: Issues, https://github.com/ninehills/langchain-wenxin/issues
 Project-URL: Source, https://github.com/ninehills/langchain-wenxin
 Author-email: Tao Yang <swulling@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -82,14 +82,15 @@
 
 Support models:
 
 - ernie-bot: Standard model, <https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11>
     - Also named `wenxin` for compatibility.
 - ernie-bot-turbo: Fast model, <https://cloud.baidu.com/doc/WENXINWORKSHOP/s/4lilb2lpf>
     - Also named `eb-instant` for compatibility.
+- other endpoints: eg: bloomz_7b1 or other custom endpoint.
 
 ## Development
 
 ```bash
 # Create virtual environment
 hatch env create
 # Activate virtual environment
```

