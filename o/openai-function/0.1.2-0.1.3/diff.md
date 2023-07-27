# Comparing `tmp/openai_function-0.1.2.tar.gz` & `tmp/openai_function-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function-0.1.2.tar", max compression
+gzip compressed data, was "openai_function-0.1.3.tar", max compression
```

## Comparing `openai_function-0.1.2.tar` & `openai_function-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-07-26 11:34:37.860827 openai_function-0.1.2/README.md
--rw-r--r--   0        0        0     3517 2023-07-26 17:12:21.525691 openai_function-0.1.2/openai_function/__init__.py
--rw-r--r--   0        0        0     2626 2023-07-26 15:12:49.735133 openai_function-0.1.2/openai_function/chat_completion.py
--rw-r--r--   0        0        0    12597 2023-07-26 17:06:59.504095 openai_function-0.1.2/openai_function/client.py
--rw-r--r--   0        0        0      463 2023-07-26 16:38:20.109822 openai_function-0.1.2/openai_function/embeddings.py
--rw-r--r--   0        0        0        0 2023-07-26 17:12:06.025143 openai_function-0.1.2/openai_function/faunadb/__init__.py
--rwxr-xr-x   0        0        0     7771 2023-07-26 16:40:14.681565 openai_function-0.1.2/openai_function/faunadb/errors.py
--rwxr-xr-x   0        0        0     5659 2023-07-26 16:40:14.681565 openai_function-0.1.2/openai_function/faunadb/objects.py
--rwxr-xr-x   0        0        0     1637 2023-07-26 16:40:14.681565 openai_function-0.1.2/openai_function/faunadb/page.py
--rwxr-xr-x   0        0        0    17374 2023-07-26 16:40:14.681565 openai_function-0.1.2/openai_function/faunadb/query.py
--rwxr-xr-x   0        0        0     6628 2023-07-26 16:41:01.737479 openai_function-0.1.2/openai_function/json.py
--rw-r--r--   0        0        0     2863 2023-07-26 14:58:26.964143 openai_function-0.1.2/openai_function/logging.py
--rwxr-xr-x   0        0        0    11253 2023-07-26 17:12:04.473088 openai_function-0.1.2/openai_function/odm.py
--rw-r--r--   0        0        0     3868 2023-07-26 17:06:58.160026 openai_function-0.1.2/openai_function/openai_functions.py
--rw-r--r--   0        0        0     1052 2023-07-26 17:06:56.179925 openai_function-0.1.2/openai_function/typedefs.py
--rw-r--r--   0        0        0     2450 2023-07-26 17:12:57.330924 openai_function-0.1.2/openai_function/vectorstore.py
--rw-r--r--   0        0        0      445 2023-07-26 17:52:39.293498 openai_function-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 openai_function-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 11:34:37.860827 openai_function-0.1.3/README.md
+-rw-r--r--   0        0        0      464 2023-07-27 02:43:17.922311 openai_function-0.1.3/openai_function/__init__.py
+-rw-r--r--   0        0        0     2715 2023-07-27 01:54:52.192346 openai_function-0.1.3/openai_function/chat_completion.py
+-rw-r--r--   0        0        0    12278 2023-07-27 02:35:12.968719 openai_function-0.1.3/openai_function/client.py
+-rw-r--r--   0        0        0        0 2023-07-26 17:12:06.025143 openai_function-0.1.3/openai_function/faunadb/__init__.py
+-rwxr-xr-x   0        0        0     7771 2023-07-26 16:40:14.681565 openai_function-0.1.3/openai_function/faunadb/errors.py
+-rwxr-xr-x   0        0        0     5659 2023-07-26 16:40:14.681565 openai_function-0.1.3/openai_function/faunadb/objects.py
+-rwxr-xr-x   0        0        0     1637 2023-07-26 16:40:14.681565 openai_function-0.1.3/openai_function/faunadb/page.py
+-rwxr-xr-x   0        0        0    17374 2023-07-26 16:40:14.681565 openai_function-0.1.3/openai_function/faunadb/query.py
+-rw-r--r--   0        0        0      230 2023-07-27 02:40:20.845792 openai_function-0.1.3/openai_function/fields.py
+-rwxr-xr-x   0        0        0     6628 2023-07-26 16:41:01.737479 openai_function-0.1.3/openai_function/json.py
+-rw-r--r--   0        0        0     2863 2023-07-26 14:58:26.964143 openai_function-0.1.3/openai_function/logging.py
+-rwxr-xr-x   0        0        0    11253 2023-07-27 02:35:12.984719 openai_function-0.1.3/openai_function/odm.py
+-rw-r--r--   0        0        0     3868 2023-07-26 17:06:58.160026 openai_function-0.1.3/openai_function/openai_functions.py
+-rw-r--r--   0        0        0     8670 2023-07-27 02:59:40.216643 openai_function-0.1.3/openai_function/store.py
+-rw-r--r--   0        0        0     1053 2023-07-27 02:35:12.648718 openai_function-0.1.3/openai_function/typedefs.py
+-rw-r--r--   0        0        0      464 2023-07-27 02:58:49.164533 openai_function-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 openai_function-0.1.3/PKG-INFO
```

### Comparing `openai_function-0.1.2/openai_function/chat_completion.py` & `openai_function-0.1.3/openai_function/chat_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     )
     max_tokens: int = Field(
         default=1024,
         ge=128,
         le=2048,
         description="The maximum number of tokens in the output.",
     )
+    stream: bool = Field(default=False, description="Whether the response is a stream.")
 
 
 class ChatCompletionUssage(BaseModel):
     """Defines the usage of the tokens for a chat completion."""
 
     prompt_tokens: int = Field(
         ..., description="The number of tokens used in the prompt."
```

### Comparing `openai_function-0.1.2/openai_function/client.py` & `openai_function-0.1.3/openai_function/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,34 @@
 import logging
 import os
 import typing
 from dataclasses import dataclass, field
 from functools import wraps
 from re import T
 from threading import Lock
-from typing import (Any, AsyncGenerator, Dict, List, Literal, NamedTuple,
-                    Optional, Type, Union)
-
-from aiohttp import (ClientConnectionError, ClientConnectorSSLError,
-                     ClientResponse, ClientSession, ClientTimeout,
-                     TCPConnector)
+from typing import (
+    Any,
+    AsyncGenerator,
+    Dict,
+    List,
+    Literal,
+    NamedTuple,
+    Optional,
+    Type,
+    Union,
+)
+
+from aiohttp import (
+    ClientConnectionError,
+    ClientConnectorSSLError,
+    ClientResponse,
+    ClientSession,
+    ClientTimeout,
+    TCPConnector,
+)
 from aiohttp.web_exceptions import HTTPException
 from dotenv import load_dotenv
 from multidict import CIMultiDict
 from pydantic import BaseModel
 
 from .faunadb.errors import FaunaException
 from .faunadb.objects import Expr
@@ -30,108 +44,121 @@
 
 Method = Literal["GET", "POST", "PUT", "PATCH", "DELETE"]
 Json = Union[Dict[str, Any], List[Dict[str, Any]]]
 MaybeJson = Optional[Json]
 Headers = Dict[str, str]
 MaybeHeaders = Optional[Headers]
 
+
 class MissingEnvironmentVariable(Exception):
     """Exception for missing environment variable."""
+
     ...
 
+
 if "FAUNA_SECRET" not in os.environ:
-    raise MissingEnvironmentVariable("The FAUNA_SECRET environment variable is not set.")
+    raise MissingEnvironmentVariable(
+        "The FAUNA_SECRET environment variable is not set."
+    )
 
 
 FAUNA_SECRET = os.environ["FAUNA_SECRET"]
 HEADERS = {
     "Authorization": f"Bearer {FAUNA_SECRET}",
     "Content-type": "application/json",
-    "Accept": "application/json"
+    "Accept": "application/json",
 }
 
 T = typing.TypeVar("T")
 
-def singleton(cls: typing.Type[T]) -> typing.Callable[..., T]: # type: ignore
+
+def singleton(cls: typing.Type[T]) -> typing.Callable[..., T]:  # type: ignore
     instance = None
     lock = Lock()
+
     @wraps(cls)
     def wrapper(*args, **kwargs):
         nonlocal instance
         if instance is None:
             with lock:
                 if instance is None:
                     instance = cls(*args, **kwargs)
         return instance
+
     return wrapper
 
+
 class APIException(HTTPException):
     """Base class for all exceptions raised by an API client."""
+
     def __init__(self, message: str, status_code: int = 500) -> None:
         self.message = message
         self.status_code = status_code
-        super().__init__(text=json.dumps({"message": message, "status": status_code}),content_type="application/json")
+        super().__init__(
+            text=json.dumps({"message": message, "status": status_code}),
+            content_type="application/json",
+        )
+
 
 @dataclass(frozen=True)
 class ConnectorConfig:
     ssl: bool = field(default=False)
     limit: int = field(default=1000)
     keepalive_timeout: int = field(default=10)
 
 
 @dataclass(init=True, repr=True, unsafe_hash=False, frozen=False)
 class APIConfig:
     base_url: str
     headers: Headers
-    logger: logging.Logger = field(default=setup_logging(__name__))  
+    logger: logging.Logger = field(default=setup_logging(__name__))
     exception_class: Type[HTTPException] = field(default=APIException)
     session: Optional[ClientSession] = field(default=None)
     connector_config: ConnectorConfig = field(default_factory=ConnectorConfig)
     read_bufsize: int = field(default=2**16)
     connector_owner: bool = field(default=True)
     trust_env: bool = field(default=True)
 
+
 @singleton
 @dataclass(init=True, repr=True, unsafe_hash=False, frozen=False)
 class FaunaClient(LazyProxy[ClientSession]):
     """
     FaunaDB Client
-    
+
     Args:
         config (APIConfig): APIConfig object
     """
-    
+
     config: APIConfig = APIConfig(
         base_url="https://db.fauna.com",
         headers=HEADERS,
         logger=setup_logging(__name__),
         exception_class=APIException,
         session=None,
-        connector_config=ConnectorConfig()
+        connector_config=ConnectorConfig(),
     )
     session_creation_lock = asyncio.Lock()
-    
-    
-        
+
     def __load__(self) -> ClientSession:
         if self.config.session is None:
             return ClientSession(
                 "https://db.fauna.com",
-                headers=CIMultiDict(self.config.headers), # type: ignore
+                headers=CIMultiDict(self.config.headers),  # type: ignore
                 connector=TCPConnector(
-                keepalive_timeout=self.config.connector_config.keepalive_timeout,           
-                ssl=self.config.connector_config.ssl,
-                limit=self.config.connector_config.limit,
+                    keepalive_timeout=self.config.connector_config.keepalive_timeout,
+                    ssl=self.config.connector_config.ssl,
+                    limit=self.config.connector_config.limit,
                 ),
                 connector_owner=self.config.connector_owner,
                 trust_env=self.config.trust_env,
                 read_bufsize=self.config.read_bufsize,
             )
         return self.config.session
-    
+
     async def query(self, expr: Expr) -> Any:
         async with self.session_creation_lock:
             if self.config.session is None:
                 self.config.session = self.__load__()
         session = self.config.session
         async with session.post(
             "/",
@@ -143,28 +170,28 @@
                 if data.get("resource") is not None:
                     return data["resource"]
                 if data.get("error") is not None:
                     return data["error"]
                 return data
 
             except (
-                    FaunaException,
-                    ValueError,
-                    KeyError,
-                    TypeError,
-                    Exception,
-                    UnicodeError,
-                    json.JSONDecodeError,
-                    RuntimeError,
-                    ClientConnectionError,
-                    ClientConnectorSSLError
+                FaunaException,
+                ValueError,
+                KeyError,
+                TypeError,
+                Exception,
+                UnicodeError,
+                json.JSONDecodeError,
+                RuntimeError,
+                ClientConnectionError,
+                ClientConnectorSSLError,
             ) as exc:  # pylint:disable=all
                 self.config.logger.error(exc)
                 raise self.config.exception_class from exc
-    
+
     async def stream(self, expr: Expr) -> AsyncGenerator[str, None]:
         session = self.__load__()
         async with session.post(
             "",
             data=to_json(expr),
             headers={
                 "Authorization": f"Bearer {self.secret}",
@@ -188,80 +215,81 @@
                     KeyError,
                     TypeError,
                     Exception,
                     UnicodeError,
                     json.JSONDecodeError,
                     RuntimeError,
                     ClientConnectionError,
-                    ClientConnectorSSLError
+                    ClientConnectorSSLError,
                 ) as exc:
                     self.config.logger.error(exc)
                     yield str(exc)
-       
+
     async def cleanup(self):
         if self.config.session is not None:
             await self.config.session.close()
-            
+
     def __del__(self):
         asyncio.run(self.cleanup())
-            
-            
+
+
 @dataclass(init=True, repr=True, unsafe_hash=False, frozen=False)
 class APIClient(LazyProxy[ClientSession]):
     """
     Generic HTTP Client
     """
+
     config: APIConfig
     subclasses: Optional[List[Type[APIClient]]] = field(default=None)
     session_creation_lock = asyncio.Lock()
-    
-    @classmethod    
+
+    @classmethod
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         if cls.subclasses is None:
             cls.subclasses = []
         cls.subclasses.append(cls)
-        
+
     @classmethod
     async def cleanup(cls):
         if hasattr(cls, "subclasses") and cls.subclasses is not None:
             tasks = []
             for subclass in cls.subclasses:
                 if subclass.config.session is not None:
                     tasks.append(subclass.config.session.close())
             await asyncio.gather(*tasks)
-    
+
     async def __load__(self) -> ClientSession:
         self.config.logger.info("Loading session for %s", self.config.base_url)
         async with self.session_creation_lock:
             if self.config.session is None:
                 self.config.session = ClientSession(
-                self.config.base_url,
-                headers=CIMultiDict(self.config.headers), 
-                response_class=ClientResponse,
-                connector=TCPConnector(
-                    keepalive_timeout=self.config.connector_config.keepalive_timeout,           
-                    ssl=self.config.connector_config.ssl,
-                    limit=self.config.connector_config.limit,
-                ),  
-                connector_owner=self.config.connector_owner,
-                trust_env=self.config.trust_env,
-                read_bufsize=self.config.read_bufsize,
-            )
+                    self.config.base_url,
+                    headers=CIMultiDict(self.config.headers),
+                    response_class=ClientResponse,
+                    connector=TCPConnector(
+                        keepalive_timeout=self.config.connector_config.keepalive_timeout,
+                        ssl=self.config.connector_config.ssl,
+                        limit=self.config.connector_config.limit,
+                    ),
+                    connector_owner=self.config.connector_owner,
+                    trust_env=self.config.trust_env,
+                    read_bufsize=self.config.read_bufsize,
+                )
         return self.config.session
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} {self.config.base_url}>"
-            
+
     async def fetch(
         self,
         url: str,
         method: Method = "GET",
         json: MaybeJson = None,
-         ):
+    ):
         session = await self.__load__()
         async with session.request(
             method, url, headers=self.config.headers, json=json
         ) as response:
             self.config.logger.info("Fetching JSON from %s with method %s", url, method)
             try:
                 return await response.json()
@@ -271,21 +299,16 @@
                 ValueError,
                 KeyError,
                 TypeError,
                 Exception,
             ) as exc:  # pylint:disable=broad-exception-caught, unused-variable
                 self.config.logger.error(exc)
                 raise self.config.exception_class from exc
-                
-    async def text(
-        self,
-        url: str,
-        method: Method = "GET",
-        json: MaybeJson = None
-    ):
+
+    async def text(self, url: str, method: Method = "GET", json: MaybeJson = None):
         session = await self.__load__()
         async with session.request(
             method, url, headers=self.config.headers, json=json
         ) as response:
             self.config.logger.info("Fetching Text from %s with method %s", url, method)
             try:
                 return await response.text()
@@ -301,15 +324,14 @@
                 raise self.config.exception_class from exc
 
     async def stream(
         self,
         url: str,
         method: Method = "GET",
         json: MaybeJson = None,
-       
     ):
         session = await self.__load__()
         async with session.request(
             method, url, headers=self.config.headers, json=json
         ) as response:
             self.config.logger.info("Streaming from %s with method %s", url, method)
             async for chunk in response.content.iter_any():
@@ -322,59 +344,37 @@
                     KeyError,
                     TypeError,
                     Exception,
                 ) as exc:
                     self.config.logger.error(exc)
                     yield str(exc)
                     raise self.config.exception_class from exc
-       
-    async def get(
-        self,
-        url: str
-    ):
 
+    async def get(self, url: str):
         return await self.fetch(url=url, method="GET")
-    
-    async def post(
-        self,
-        url: str,
-        json: MaybeJson = None
-    ):
+
+    async def post(self, url: str, json: MaybeJson = None):
         return await self.fetch(url=url, method="POST", json=json)
-        
-    async def put(
-        self,
-        url: str,
-        json: MaybeJson = None
-    ):
+
+    async def put(self, url: str, json: MaybeJson = None):
         return await self.fetch(url=url, method="PUT", json=json)
-    
-    async def patch(
-        self,
-        url: str,
-        json: MaybeJson = None
-    ):
+
+    async def patch(self, url: str, json: MaybeJson = None):
         return await self.fetch(url=url, method="PATCH", json=json)
-    
-    async def delete(
-        self,
-        url: str,
-        json: MaybeJson = None
-    ):
-        
-        return await self.fetch(url=url, method="DELETE", json=json)             
-    
-        
-    def update_headers(self, headers: Dict[str,str]):
+
+    async def delete(self, url: str, json: MaybeJson = None):
+        return await self.fetch(url=url, method="DELETE", json=json)
+
+    def update_headers(self, headers: Dict[str, str]):
         """
         Update the headers used by this API client.
 
         Returns:
             self: Allows method chaining.
         """
         self.config.headers = headers
         self.config.logger.info("Updated headers to %s", headers)
         return self
-    
+
 
 def make_client(base_url: str, headers: Dict[str, str]):
-    return APIClient(APIConfig(base_url=base_url, headers=headers))
+    return APIClient(APIConfig(base_url=base_url, headers=headers))
```

### Comparing `openai_function-0.1.2/openai_function/faunadb/errors.py` & `openai_function-0.1.3/openai_function/faunadb/errors.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.2/openai_function/faunadb/objects.py` & `openai_function-0.1.3/openai_function/faunadb/objects.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.2/openai_function/faunadb/page.py` & `openai_function-0.1.3/openai_function/faunadb/page.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.2/openai_function/faunadb/query.py` & `openai_function-0.1.3/openai_function/faunadb/query.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.2/openai_function/json.py` & `openai_function-0.1.3/openai_function/json.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.2/openai_function/logging.py` & `openai_function-0.1.3/openai_function/logging.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.2/openai_function/odm.py` & `openai_function-0.1.3/openai_function/odm.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from .logging import setup_logging
 
 load_dotenv()
 
 T = TypeVar("T", bound="FaunaModel")
 
 
-
 class FaunaModelMetaclass(ModelMetaclass):
     def __new__(cls, name, bases, attrs):
         new_cls = super().__new__(cls, name, bases, attrs)
         cls.Metadata.__subclasses__.append(new_cls)
         return new_cls
 
     class Metadata:
@@ -343,8 +342,8 @@
         if isinstance(self.ref, str) and len(self.ref) == 18:
             return await self.update(self.ref, kwargs=self.dict())
 
         return await self.create()
 
     @classmethod
     async def cleanup(cls):
-        await cls.client().cleanup()
+        await cls.client().cleanup()
```

### Comparing `openai_function-0.1.2/openai_function/openai_functions.py` & `openai_function-0.1.3/openai_function/openai_functions.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.2/openai_function/typedefs.py` & `openai_function-0.1.3/openai_function/typedefs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Dict, Generic, Iterable, List, TypeVar, Union, cast
 
 Vector = List[float]
 MetaData = Dict[str, str]
 
 T = TypeVar("T")
 
+
 class LazyProxy(Generic[T], ABC):
     def __init__(self) -> None:
         self.__proxied: Union[T, None] = None
 
     def __getattr__(self, attr: str) -> object:
         return getattr(self.__get_proxied__(), attr)
```

