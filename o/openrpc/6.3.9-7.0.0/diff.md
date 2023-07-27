# Comparing `tmp/openrpc-6.3.9.tar.gz` & `tmp/openrpc-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrpc-6.3.9.tar", max compression
+gzip compressed data, was "openrpc-7.0.0.tar", max compression
```

## Comparing `openrpc-6.3.9.tar` & `openrpc-7.0.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-03-10 02:23:48.038498 openrpc-6.3.9/LICENSE
--rw-r--r--   0        0        0     3193 2023-03-10 02:23:48.039498 openrpc-6.3.9/README.md
--rw-r--r--   0        0        0     1044 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/__init__.py
--rw-r--r--   0        0        0      183 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_depends.py
--rw-r--r--   0        0        0    11339 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_discover.py
--rw-r--r--   0        0        0     7232 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_method_processor.py
--rw-r--r--   0        0        0     5585 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_method_registrar.py
--rw-r--r--   0        0        0     9488 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_objects.py
--rw-r--r--   0        0        0     7045 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_request_processor.py
--rw-r--r--   0        0        0      280 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_router.py
--rw-r--r--   0        0        0     1168 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_rpcmethod.py
--rw-r--r--   0        0        0     8406 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/_server.py
--rw-r--r--   0        0        0        0 2023-03-10 02:23:48.039498 openrpc-6.3.9/openrpc/py.typed
--rw-r--r--   0        0        0     1102 2023-03-10 02:23:48.040499 openrpc-6.3.9/pyproject.toml
--rw-r--r--   0        0        0     4354 1970-01-01 00:00:00.000000 openrpc-6.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-27 18:06:21.345543 openrpc-7.0.0/LICENSE
+-rw-r--r--   0        0        0     3257 2023-07-27 18:06:21.345543 openrpc-7.0.0/README.md
+-rw-r--r--   0        0        0     1045 2023-07-27 18:06:21.345543 openrpc-7.0.0/openrpc/__init__.py
+-rw-r--r--   0        0        0      183 2023-07-27 18:06:21.345543 openrpc-7.0.0/openrpc/_depends.py
+-rw-r--r--   0        0        0        0 2023-07-27 18:06:21.371542 openrpc-7.0.0/openrpc/_discover/__init__.py
+-rw-r--r--   0        0        0     4266 2023-07-27 18:06:21.345543 openrpc-7.0.0/openrpc/_discover/_methods.py
+-rw-r--r--   0        0        0     6112 2023-07-27 18:06:21.345543 openrpc-7.0.0/openrpc/_discover/_schemas.py
+-rw-r--r--   0        0        0     1289 2023-07-27 18:06:21.345543 openrpc-7.0.0/openrpc/_discover/discover.py
+-rw-r--r--   0        0        0     7862 2023-07-27 18:06:21.345543 openrpc-7.0.0/openrpc/_method_processor.py
+-rw-r--r--   0        0        0     6128 2023-07-27 18:06:21.345543 openrpc-7.0.0/openrpc/_method_registrar.py
+-rw-r--r--   0        0        0     9417 2023-07-27 18:06:21.346543 openrpc-7.0.0/openrpc/_objects.py
+-rw-r--r--   0        0        0     7616 2023-07-27 18:06:21.346543 openrpc-7.0.0/openrpc/_request_processor.py
+-rw-r--r--   0        0        0      280 2023-07-27 18:06:21.346543 openrpc-7.0.0/openrpc/_router.py
+-rw-r--r--   0        0        0     1168 2023-07-27 18:06:21.346543 openrpc-7.0.0/openrpc/_rpcmethod.py
+-rw-r--r--   0        0        0     9267 2023-07-27 18:06:21.346543 openrpc-7.0.0/openrpc/_server.py
+-rw-r--r--   0        0        0        0 2023-07-27 18:06:21.371542 openrpc-7.0.0/openrpc/py.typed
+-rw-r--r--   0        0        0     1479 2023-07-27 18:06:21.346543 openrpc-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4218 1970-01-01 00:00:00.000000 openrpc-7.0.0/PKG-INFO
```

### Comparing `openrpc-6.3.9/LICENSE` & `openrpc-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openrpc-6.3.9/README.md` & `openrpc-7.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -42,18 +42,18 @@
 from openrpc import RPCServer
 
 rpc = RPCServer(title="Demo Server", version="1.0.0")
 ```
 
 ### Register a function as an RPC Method
 
-To register a method with the RPCServer add the `@rpc.method` decorator to a function.
+To register a method with the RPCServer add the `@rpc.method()` decorator to a function.
 
 ```python
-@rpc.method
+@rpc.method()
 def add(a: int, b: int) -> int:
     return a + b
 ```
 
 ### Process JSON RPC Request
 
 OpenRPC is transport agnostic. To use it, pass JSON RPC requests as strings or byte
@@ -93,37 +93,41 @@
 from openrpc import RPCServer
 from sanic import Request, Sanic, Websocket
 
 app = Sanic("DemoServer")
 rpc = RPCServer(title="DemoServer", version="1.0.0")
 
 
-@rpc.method
+@rpc.method()
 async def add(a: int, b: int) -> int:
     return a + b
 
 
 @app.websocket("/api/v1/")
 async def process_websocket(_request: Request, ws: Websocket) -> None:
     async for msg in ws:
         json_rpc_response = await rpc.process_request_async(msg)
-        await ws.send(json_rpc_response)
+        if json_rpc_response is not None:
+            await ws.send(json_rpc_response)
 
 
 if __name__ == "__main__":
     app.run()
 ```
 
 Example In
 
 ```json
 {
   "id": 1,
   "method": "add",
-  "params": {"a": 1, "b": 3},
+  "params": {
+    "a": 1,
+    "b": 3
+  },
   "jsonrpc": "2.0"
 }
 ```
 
 Example Result Out
 
 ```json
```

### Comparing `openrpc-6.3.9/openrpc/__init__.py` & `openrpc-7.0.0/openrpc/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,8 @@
 """Provides OpenRPC objects and the RPCServer class."""
-from openrpc._depends import Depends
-from openrpc._objects import (
-    ComponentsObject,
-    ContactObject,
-    ContentDescriptorObject,
-    ErrorObject,
-    ExampleObject,
-    ExamplePairingObject,
-    ExternalDocumentationObject,
-    InfoObject,
-    LicenseObject,
-    LinkObject,
-    MethodObject,
-    OpenRPCObject,
-    ParamStructure,
-    ReferenceObject,
-    SchemaObject,
-    ServerObject,
-    ServerVariableObject,
-    TagObject,
-)
-from openrpc._router import RPCRouter
-from openrpc._server import RPCServer
 
 __all__ = (
     "ComponentsObject",
     "ContactObject",
     "ContentDescriptorObject",
     "ErrorObject",
     "ExampleObject",
@@ -42,7 +19,31 @@
     "ReferenceObject",
     "SchemaObject",
     "ServerObject",
     "ServerVariableObject",
     "TagObject",
     "Depends",
 )
+
+from openrpc._depends import Depends
+from openrpc._objects import (
+    ComponentsObject,
+    ContactObject,
+    ContentDescriptorObject,
+    ErrorObject,
+    ExampleObject,
+    ExamplePairingObject,
+    ExternalDocumentationObject,
+    InfoObject,
+    LicenseObject,
+    LinkObject,
+    MethodObject,
+    OpenRPCObject,
+    ParamStructure,
+    ReferenceObject,
+    SchemaObject,
+    ServerObject,
+    ServerVariableObject,
+    TagObject,
+)
+from openrpc._router import RPCRouter
+from openrpc._server import RPCServer
```

### Comparing `openrpc-6.3.9/openrpc/_method_processor.py` & `openrpc-7.0.0/openrpc/_request_processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,112 @@
-"""Provide JSON-RPC2 server class."""
+"""Module responsible for parsing JSON RPC 2.0 requests."""
+
+__all__ = ("RequestProcessor",)
+
 import asyncio
 import json
 import logging
 from json import JSONDecodeError
 from typing import Any, Optional, Union
 
 from jsonrpcobjects.errors import INVALID_REQUEST, METHOD_NOT_FOUND, PARSE_ERROR
 from jsonrpcobjects.objects import (
-    ErrorObjectData,
-    ErrorResponseObject,
-    NotificationObject,
-    NotificationObjectParams,
+    DataError,
+    ErrorResponse,
+    Notification,
     NotificationType,
-    RequestObject,
-    RequestObjectParams,
+    ParamsNotification,
+    ParamsRequest,
+    Request,
     RequestType,
 )
 from pydantic import ValidationError
 
-from openrpc._request_processor import RequestProcessor
+from openrpc._method_processor import MethodProcessor
 from openrpc._rpcmethod import RPCMethod
 
-__all__ = ("MethodProcessor",)
-
-
 log = logging.getLogger("openrpc")
-NotificationTypes = (NotificationObject, NotificationObjectParams)
-RequestTypes = (RequestObject, RequestObjectParams)
+NotificationTypes = (Notification, ParamsNotification)
+RequestTypes = (Request, ParamsRequest)
 _DEFAULT_ERROR_CODE = -32000
 
 
-class MethodProcessor:
-    """Class to register and execute methods."""
+class RequestProcessor:
+    """Class to parse requests and pass results to MethodProcessor."""
+
+    def __init__(self, *, debug: bool) -> None:
+        """Init a RequestProcessor.
 
-    def __init__(self) -> None:
-        """Init a MethodProcessor."""
+        :param debug: Include internal error details in responses.
+        """
+        self.debug = debug
         self.methods: dict[str, RPCMethod] = {}
         self.uncaught_error_code = _DEFAULT_ERROR_CODE
 
-    def method(self, func: RPCMethod, method_name: str) -> None:
+    def method(self, function: RPCMethod, method_name: str) -> None:
         """Register a method with this server for later calls.
 
-        :param func: Function to call for this method.
+        :param function: Function to call for this method.
         :param method_name: Name of the RPC method.
         :return: None.
         """
-        self.methods[method_name] = func
+        self.methods[method_name] = function
 
     def process(
         self, data: Union[bytes, str], depends: Optional[dict[str, Any]]
     ) -> Optional[str]:
-        """Process a JSON-RPC2 request and get the response.
+        """Parse a JSON-RPC2 request and get the response.
 
         :param data: A JSON-RPC2 request.
         :param depends: Values passed to functions with dependencies.
         :return: A valid JSON-RPC2 response.
         """
         parsed_json = _get_parsed_json(data)
-        if isinstance(parsed_json, ErrorResponseObject):
-            return parsed_json.json()
+        if isinstance(parsed_json, ErrorResponse):
+            return parsed_json.model_dump_json()
 
         # Batch
         if isinstance(parsed_json, list):
             requests = [_get_request_object(it) for it in parsed_json]
             results: list[str] = []
             for req in requests:
-                if isinstance(req, ErrorResponseObject):
-                    results.append(req.json())
+                if isinstance(req, ErrorResponse):
+                    results.append(req.model_dump_json())
                     continue
                 if req.method not in self.methods:
-                    if isinstance(req, (RequestObject, RequestObjectParams)):
+                    if isinstance(req, (Request, ParamsRequest)):
                         results.append(_get_method_not_found_error(req))
                     continue
 
-                resp = RequestProcessor(
-                    self.methods[req.method], self.uncaught_error_code, req, depends
+                resp = MethodProcessor(
+                    self.methods[req.method],
+                    self.uncaught_error_code,
+                    req,
+                    depends,
+                    debug=self.debug,
                 ).execute()
                 # If resp is None, request is a notification.
                 if resp is not None:
                     results.append(resp)
             return f"[{','.join(results)}]"
 
         # Single Request
         request = _get_request_object(parsed_json)
-        if isinstance(request, ErrorResponseObject):
-            return request.json()
+        if isinstance(request, ErrorResponse):
+            return request.model_dump_json()
         if request.method not in self.methods:
-            if isinstance(request, (RequestObject, RequestObjectParams)):
+            if isinstance(request, (Request, ParamsRequest)):
                 return _get_method_not_found_error(request)
             return None
-        result = RequestProcessor(
-            self.methods[request.method], self.uncaught_error_code, request, depends
+        result = MethodProcessor(
+            self.methods[request.method],
+            self.uncaught_error_code,
+            request,
+            depends,
+            debug=self.debug,
         ).execute()
         return None if isinstance(request, NotificationTypes) else result
 
     async def process_async(
         self, data: Union[bytes, str], depends: Optional[dict[str, Any]]
     ) -> Optional[str]:
         """Process a JSON-RPC2 request and get the response.
@@ -102,92 +114,98 @@
         If the method called by the request is async it will be awaited.
 
         :param data: A JSON-RPC2 request.
         :param depends: Values passed to functions with dependencies.
         :return: A valid JSON-RPC2 response.
         """
         parsed_json = _get_parsed_json(data)
-        if isinstance(parsed_json, ErrorResponseObject):
-            return parsed_json.json()
+        if isinstance(parsed_json, ErrorResponse):
+            return parsed_json.model_dump_json()
 
         # Batch
         if isinstance(parsed_json, list):
 
             async def _process_request(
-                request: Union[ErrorResponseObject, NotificationType, RequestType]
+                request: Union[ErrorResponse, NotificationType, RequestType]
             ) -> Any:
-                if isinstance(request, ErrorResponseObject):
-                    return request.json()
+                if isinstance(request, ErrorResponse):
+                    return request.model_dump_json()
                 if request.method not in self.methods:
-                    if isinstance(request, (RequestObject, RequestObjectParams)):
+                    if isinstance(request, (Request, ParamsRequest)):
                         return _get_method_not_found_error(request)
                     return None
 
                 method = self.methods[request.method]
                 if isinstance(request, RequestTypes):
-                    return await RequestProcessor(
-                        method, self.uncaught_error_code, request, depends
+                    return await MethodProcessor(
+                        method,
+                        self.uncaught_error_code,
+                        request,
+                        depends,
+                        debug=self.debug,
                     ).execute_async()
                 # To get here, request must be a notification.
-                await RequestProcessor(
-                    method, self.uncaught_error_code, request, depends
+                await MethodProcessor(
+                    method, self.uncaught_error_code, request, depends, debug=self.debug
                 ).execute_async()
+                return None
 
             results = await asyncio.gather(
                 *[_process_request(_get_request_object(it)) for it in parsed_json]
             )
             return f"[{','.join(str(r) for r in results if r is not None)}]"
 
         # Single Request
         req = _get_request_object(parsed_json)
-        if isinstance(req, ErrorResponseObject):
-            return req.json()
+        if isinstance(req, ErrorResponse):
+            return req.model_dump_json()
         if req.method not in self.methods:
-            if isinstance(req, (RequestObject, RequestObjectParams)):
+            if isinstance(req, (Request, ParamsRequest)):
                 return _get_method_not_found_error(req)
             return None
-        result = await RequestProcessor(
-            self.methods[req.method], self.uncaught_error_code, req, depends
+        result = await MethodProcessor(
+            self.methods[req.method],
+            self.uncaught_error_code,
+            req,
+            depends,
+            debug=self.debug,
         ).execute_async()
+
         return None if isinstance(req, NotificationTypes) else result
 
 
 def _get_method_not_found_error(req: Union[NotificationType, RequestType]) -> str:
-    return ErrorResponseObject(
+    return ErrorResponse(
         id=None if isinstance(req, NotificationTypes) else req.id,
-        error=ErrorObjectData(**{**METHOD_NOT_FOUND.dict(), **{"data": req.method}}),
-    ).json()
+        error=DataError(**{**METHOD_NOT_FOUND.model_dump(), **{"data": req.method}}),
+    ).model_dump_json()
 
 
-def _get_parsed_json(data: Union[bytes, str]) -> Union[ErrorResponseObject, dict, list]:
+def _get_parsed_json(data: Union[bytes, str]) -> Union[ErrorResponse, dict, list]:
     try:
         parsed_json = json.loads(data)
     except (TypeError, JSONDecodeError) as error:
         log.exception("%s:", type(error).__name__)
-        return ErrorResponseObject(id=None, error=PARSE_ERROR)
+        return ErrorResponse(id=None, error=PARSE_ERROR)
     return parsed_json
 
 
 def _get_request_object(
     data: Any,
-) -> Union[ErrorResponseObject, NotificationType, RequestType]:
+) -> Union[ErrorResponse, NotificationType, RequestType]:
     try:
         is_request = data.get("id") is not None
         has_params = data.get("params") is not None
         if is_request:
-            return RequestObjectParams(**data) if has_params else RequestObject(**data)
-        return (
-            NotificationObjectParams(**data)
-            if has_params
-            else NotificationObject(**data)
-        )
+            return ParamsRequest(**data) if has_params else Request(**data)
+        return ParamsNotification(**data) if has_params else Notification(**data)
     except (TypeError, ValidationError) as error:
         log.exception("%s:", type(error).__name__)
-        return ErrorResponseObject(
+        return ErrorResponse(
             id=data.get("id"),
-            error=ErrorObjectData(**{**INVALID_REQUEST.dict(), **{"data": data}}),
+            error=DataError(**{**INVALID_REQUEST.model_dump(), **{"data": data}}),
         )
     except AttributeError:
-        return ErrorResponseObject(
+        return ErrorResponse(
             id=None,
-            error=ErrorObjectData(**{**INVALID_REQUEST.dict(), **{"data": data}}),
+            error=DataError(**{**INVALID_REQUEST.model_dump(), **{"data": data}}),
         )
```

### Comparing `openrpc-6.3.9/openrpc/_method_registrar.py` & `openrpc-7.0.0/openrpc/_method_registrar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 """Module providing method registrar interface."""
+
+__all__ = ("MethodRegistrar", "CallableType")
+
 import inspect
 import logging
+import warnings
 from functools import partial
 from typing import Callable, Optional, TypeVar, Union
 
 from openrpc import Depends
-from openrpc._method_processor import MethodProcessor
 from openrpc._objects import (
     ContentDescriptorObject,
     ErrorObject,
     ExamplePairingObject,
     ExternalDocumentationObject,
     LinkObject,
     ParamStructure,
     ServerObject,
     TagObject,
 )
+from openrpc._request_processor import RequestProcessor
 from openrpc._rpcmethod import MethodMetaData, RPCMethod
 
-__all__ = ("MethodRegistrar", "CallableType")
-
-
 log = logging.getLogger("openrpc")
 
 CallableType = TypeVar("CallableType", bound=Callable)
 DecoratedCallableType = TypeVar("DecoratedCallableType", bound=Callable)
 
 
 class MethodRegistrar:
     """Interface for registering RPC methods."""
 
     def __init__(self) -> None:
         """Initialize a new instance of the MethodRegistrar class."""
         self._rpc_methods: dict[str, RPCMethod] = {}
-        self._method_processor = MethodProcessor()
+        self._request_processor = RequestProcessor(debug=False)
 
-    def method(
+    @property
+    def debug(self) -> bool:
+        """Debug logging status."""
+        return self._request_processor.debug
+
+    @debug.setter
+    def debug(self, debug: bool) -> None:
+        self._request_processor.debug = debug
+
+    def method(  # noqa: PLR0913
         self,
         *args: CallableType,
         name: Optional[str] = None,
         params: Optional[list[ContentDescriptorObject]] = None,
         result: Optional[ContentDescriptorObject] = None,
         tags: Optional[list[Union[TagObject, str]]] = None,
         summary: Optional[str] = None,
@@ -92,14 +102,20 @@
         """
         tag_objects = (
             [tag if isinstance(tag, TagObject) else TagObject(name=tag) for tag in tags]
             if tags is not None
             else None
         )
         if not args:
+            warnings.warn(
+                "RPCServer `method` decorator must be called in future releases, use"
+                "`method()` instead.",
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
             return partial(  # type: ignore
                 self.method,
                 name=name,
                 params=params,
                 result=result,
                 tags=tag_objects,
                 summary=summary,
@@ -136,24 +152,24 @@
     def remove(self, method: str) -> None:
         """Remove a method from this server by name.
 
         :param method: Name of the method to remove.
         :return: None.
         """
         self._rpc_methods.pop(method)
-        self._method_processor.methods.pop(method)
+        self._request_processor.methods.pop(method)
 
-    def _method(self, func: CallableType, metadata: MethodMetaData) -> CallableType:
+    def _method(self, function: CallableType, metadata: MethodMetaData) -> CallableType:
         dependencies = [
             k
-            for k, v in inspect.signature(func).parameters.items()
+            for k, v in inspect.signature(function).parameters.items()
             if v.default is Depends
         ]
         rpc_method = RPCMethod(
-            function=func, metadata=metadata, depends_params=dependencies
+            function=function, metadata=metadata, depends_params=dependencies
         )
         self._rpc_methods[metadata.name] = rpc_method
         log.debug(
-            "Registering function [%s] as method [%s]", func.__name__, metadata.name
+            "Registering function [%s] as method [%s]", function.__name__, metadata.name
         )
-        self._method_processor.method(rpc_method, metadata.name)
-        return func
+        self._request_processor.method(rpc_method, metadata.name)
+        return function
```

### Comparing `openrpc-6.3.9/openrpc/_objects.py` & `openrpc-7.0.0/openrpc/_objects.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 """Python class representations of OpenRPC and JSON Schema objects."""
 from __future__ import annotations
 
-from enum import Enum
-from typing import Any, Optional, Union
-
-from pydantic import BaseModel, Field
-
 __all__ = (
     "ComponentsObject",
     "ContactObject",
     "ContentDescriptorObject",
     "ErrorObject",
     "ExampleObject",
     "ExamplePairingObject",
@@ -24,14 +19,19 @@
     "SchemaObject",
     "SchemaType",
     "ServerObject",
     "ServerVariableObject",
     "TagObject",
 )
 
+from enum import Enum
+from typing import Any, Optional, Union
+
+from pydantic import BaseModel, Field
+
 SchemaType = Union["SchemaObject", bool]
 
 
 class ParamStructure(Enum):
     """OpenRPC method param structure options."""
 
     BY_NAME = "by-name"
@@ -141,15 +141,15 @@
     additional_properties: Optional[SchemaType] = Field(
         alias="additionalProperties", default=None
     )
     property_names: Optional[SchemaType] = Field(alias="propertyNames", default=None)
     min_properties: Optional[int] = Field(alias="minProperties", default=None)
     max_properties: Optional[int] = Field(alias="maxProperties", default=None)
     required: Optional[list[str]] = None
-    definitions: Optional[dict[str, SchemaType]] = None
+    defs: Optional[dict[str, SchemaType]] = Field(alias="$defs", default=None)
     items: Optional[Union[SchemaType, bool]] = None
     prefix_items: Optional[list[SchemaType]] = Field(alias="prefixItems", default=None)
     contains: Optional[SchemaType] = None
     min_contains: Optional[int] = Field(alias="minContains", default=None)
     max_contains: Optional[int] = Field(alias="maxContains", default=None)
     min_items: Optional[int] = Field(alias="minItems", default=None)
     max_items: Optional[int] = Field(alias="maxItems", default=None)
@@ -186,15 +186,15 @@
 
 class ExampleObject(BaseModel):
     """Example that is intended to match a given Content Descriptor Schema."""
 
     name: Optional[str] = None
     summary: Optional[str] = None
     description: Optional[str] = None
-    value: Any = None
+    value: Optional[Any] = None
     external_value: Optional[str] = Field(None, alias="externalValue")
 
 
 class LinkObject(BaseModel):
     """The Link object represents a possible design-time link for a result."""
 
     name: str
@@ -206,15 +206,15 @@
 
 
 class ErrorObject(BaseModel):
     """Defines an application level error."""
 
     code: int
     message: str
-    data: Any = None
+    data: Optional[Any] = None
 
 
 class ComponentsObject(BaseModel):
     """Holds a set of reusable objects for different aspects of the OpenRPC."""
 
     content_descriptors: Optional[dict[str, ContentDescriptorObject]] = Field(
         default=None, alias="contentDescriptors"
@@ -250,38 +250,38 @@
 class ReferenceObject(BaseModel):
     """A simple object to allow referencing other components in the specification."""
 
     ref: str = Field(alias="$ref")
 
 
 class OpenRPCObject(BaseModel):
-    """This is the root object of the OpenRPC document."""
+    """Root object of the OpenRPC document."""
 
     openrpc: str
     info: InfoObject
     methods: list[MethodObject]
     servers: Union[list[ServerObject], ServerObject] = ServerObject(
         name="default", url="localhost"
     )
     components: Optional[ComponentsObject] = None
     external_docs: Optional[ExternalDocumentationObject] = Field(
         default=None, alias="externalDocs"
     )
 
 
-InfoObject.update_forward_refs()
-ContactObject.update_forward_refs()
-LicenseObject.update_forward_refs()
-ServerObject.update_forward_refs()
-ServerVariableObject.update_forward_refs()
-MethodObject.update_forward_refs()
-ContentDescriptorObject.update_forward_refs()
-SchemaObject.update_forward_refs()
-ExamplePairingObject.update_forward_refs()
-ExampleObject.update_forward_refs()
-LinkObject.update_forward_refs()
-ErrorObject.update_forward_refs()
-ComponentsObject.update_forward_refs()
-TagObject.update_forward_refs()
-ExternalDocumentationObject.update_forward_refs()
-OpenRPCObject.update_forward_refs()
-ReferenceObject.update_forward_refs()
+InfoObject.model_rebuild()
+ContactObject.model_rebuild()
+LicenseObject.model_rebuild()
+ServerObject.model_rebuild()
+ServerVariableObject.model_rebuild()
+MethodObject.model_rebuild()
+ContentDescriptorObject.model_rebuild()
+SchemaObject.model_rebuild()
+ExamplePairingObject.model_rebuild()
+ExampleObject.model_rebuild()
+LinkObject.model_rebuild()
+ErrorObject.model_rebuild()
+ComponentsObject.model_rebuild()
+TagObject.model_rebuild()
+ExternalDocumentationObject.model_rebuild()
+OpenRPCObject.model_rebuild()
+ReferenceObject.model_rebuild()
```

### Comparing `openrpc-6.3.9/openrpc/_request_processor.py` & `openrpc-7.0.0/openrpc/_method_processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,159 +1,190 @@
-"""Provides RequestProcessor class for processing a single request."""
+"""Module responsible for processing a method call."""
+
+__all__ = ("MethodProcessor",)
+
 import inspect
 import logging
 from enum import Enum
 from typing import (
     Any,
     get_args,
     get_origin,
     get_type_hints,
     Optional,
     Type,
     Union,
 )
 
-from jsonrpcobjects.errors import INTERNAL_ERROR, InternalError, JSONRPCError
+from jsonrpcobjects.errors import (
+    INTERNAL_ERROR,
+    InternalError,
+    InvalidParams,
+    JSONRPCError,
+)
 from jsonrpcobjects.objects import (
-    ErrorObjectData,
-    ErrorResponseObject,
-    NotificationObject,
-    NotificationObjectParams,
+    DataError,
+    Error,
+    ErrorResponse,
+    ErrorType,
+    Notification,
     NotificationType,
-    RequestObject,
-    RequestObjectParams,
+    ParamsNotification,
+    ParamsRequest,
+    Request,
     RequestType,
-    ResultResponseObject,
+    ResultResponse,
 )
 
+from openrpc import ParamStructure
 from openrpc._rpcmethod import RPCMethod
 
-__all__ = ("RequestProcessor",)
 log = logging.getLogger("openrpc")
+by_position_error = DataError(
+    code=-32602, message="Invalid params", data="Params must be passed by position."
+)
+by_name_error = DataError(
+    code=-32602, message="Invalid params", data="Params must be passed by name."
+)
 
 
 class DeserializationError(InternalError):
     """Raised when a request param cannot be deserialized."""
 
     def __init__(self, param: Any, p_type: Any) -> None:
         msg = f"Failed to deserialize request param [{param}] to type [{p_type}]"
-        super().__init__(ErrorObjectData(**{**INTERNAL_ERROR.dict(), **{"data": msg}}))
+        super().__init__(DataError(**{**INTERNAL_ERROR.model_dump(), **{"data": msg}}))
 
 
 class NotDeserializedType:
     """Returned by deserialization method if deserialization fails.
 
     The deserialized value may very well be False or None, so a custom
     type needs to be made to represent a failure to deserialize.
     """
 
 
 NotDeserialized = NotDeserializedType()
 
 
-class RequestProcessor:
-    """Execute a JSON-RPC2 request and get the response."""
+class MethodProcessor:
+    """Execute a method passing it a parsed JSON RPC 2.0 request."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         method: RPCMethod,
         uncaught_error_code: int,
         request: Union[RequestType, NotificationType],
         depends_values: Optional[dict[str, Any]],
+        *,
+        debug: bool,
     ) -> None:
-        """Init a request processor.
+        """Init a MethodProcessor.
 
         :param method: The Python callable.
         :param uncaught_error_code: Code for errors raised by method.
         :param request: Request to execute.
         :param depends_values: Values passed to functions with dependencies.
+        :param debug: Include internal error details in responses.
         """
+        self.debug = debug
         self.method = method
         self.request = request
         self.uncaught_error_code = uncaught_error_code
         self.depends = depends_values or {}
 
     def execute(self) -> Optional[str]:
         """Execute the method and get the JSON-RPC2 response."""
         try:
             result = self._execute()
-            if isinstance(self.request, (NotificationObject, NotificationObjectParams)):
+            if isinstance(self.request, (Notification, ParamsNotification)):
                 # If request was notification, return nothing.
                 return None
-            return ResultResponseObject(id=self.request.id, result=result).json()
+            return ResultResponse(id=self.request.id, result=result).model_dump_json()
 
         except Exception as error:
             return self._get_error_response(error)
 
     async def execute_async(self) -> Any:
         """Execute the method and get the JSON-RPC2 response.
 
         If the method is an async method it will be awaited.
         """
         try:
             result = self._execute()
             if inspect.isawaitable(result):
                 result = await result
-            if isinstance(self.request, (NotificationObject, NotificationObjectParams)):
+            if isinstance(self.request, (Notification, ParamsNotification)):
                 # If request was notification, return nothing.
                 return None
-            return ResultResponseObject(id=self.request.id, result=result).json()
+            return ResultResponse(id=self.request.id, result=result).model_dump_json()
 
         except Exception as error:
             return self._get_error_response(error)
 
     def _execute(self) -> Any:
         annotations = get_type_hints(self.method.function)
         params: Optional[Union[dict, list]]
         params_msg = ""
         missing_dependencies = [
             k for k in self.method.depends_params if k not in self.depends
         ]
         if missing_dependencies:
             raise AttributeError(
-                f"Missing dependent values {missing_dependencies}"
-                f" for method [{self.method.metadata.name}]"
+                "Missing dependent values %s  for method [%s]"
+                % (missing_dependencies, self.method.metadata.name)
             )
         dependencies = {k: self.depends.get(k) for k in self.method.depends_params}
         # Call method.
-        if isinstance(self.request, (RequestObject, NotificationObject)):
+        if isinstance(self.request, (Request, Notification)):
             result = self.method.function(**dependencies)
         elif isinstance(self.request.params, list):
+            if self.method.metadata.param_structure == ParamStructure.BY_NAME:
+                raise InvalidParams(by_name_error)
             params = self._get_list_params(self.request.params, annotations)
             result = self.method.function(*params, **dependencies)
             params_msg = ", ".join(str(p) for p in params)
         else:
+            if self.method.metadata.param_structure == ParamStructure.BY_POSITION:
+                raise InvalidParams(by_position_error)
             params = self._get_dict_params(self.request.params, annotations)
             result = self.method.function(**params, **dependencies)
             params_msg = ", ".join(f"{k}={v}" for k, v in params.items())
 
         # Logging
         id_msg = "None"
-        if isinstance(self.request, (RequestObject, RequestObjectParams)):
+        if isinstance(self.request, (Request, ParamsRequest)):
             if isinstance(self.request.id, str):
                 id_msg = f'"{self.request.id}"'
             else:
                 id_msg = str(self.request.id)
         log.info("%s: %s(%s) -> %s", id_msg, self.request.method, params_msg, result)
         return result
 
     def _get_error_response(self, error: Exception) -> Optional[str]:
         log.exception("%s:", type(error).__name__)
-        if not isinstance(self.request, (RequestObjectParams, RequestObject)):
+
+        if not isinstance(self.request, (ParamsRequest, Request)):
             return None
+
         if isinstance(error, JSONRPCError):
-            return ErrorResponseObject(id=self.request.id, error=error.rpc_error).json()
-        return ErrorResponseObject(
-            id=self.request.id,
-            error=ErrorObjectData(
+            return ErrorResponse(
+                id=self.request.id, error=error.rpc_error
+            ).model_dump_json()
+
+        if self.debug:
+            error_object: ErrorType = DataError(
                 code=self.uncaught_error_code,
                 message="Server error",
                 data=f"{type(error).__name__}: {error}",
-            ),
-        ).json()
+            )
+        else:
+            error_object = Error(code=self.uncaught_error_code, message="Server error")
+
+        return ErrorResponse(id=self.request.id, error=error_object).model_dump_json()
 
     def _get_list_params(self, params: list, annotations: dict) -> list:
         try:
             return [
                 self._deserialize(p, list(annotations.values())[i])
                 for i, p in enumerate(params)
             ]
```

### Comparing `openrpc-6.3.9/openrpc/_rpcmethod.py` & `openrpc-7.0.0/openrpc/_rpcmethod.py`

 * *Files identical despite different names*

### Comparing `openrpc-6.3.9/openrpc/_server.py` & `openrpc-7.0.0/openrpc/_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 """Module providing RPCServer class."""
+
+__all__ = ("RPCServer",)
+
 import logging
 from typing import Any, Callable, Optional, Union
 
 from jsonrpcobjects.errors import INTERNAL_ERROR
-from jsonrpcobjects.objects import ErrorObjectData
+from jsonrpcobjects.objects import DataError, Error, ErrorResponse
 
 from openrpc import RPCRouter
-from openrpc._discover import DiscoverHandler
 from openrpc._method_registrar import CallableType, MethodRegistrar
 from openrpc._objects import (
     ContactObject,
     ContentDescriptorObject,
     InfoObject,
     LicenseObject,
     MethodObject,
     SchemaObject,
     TagObject,
 )
 from openrpc._rpcmethod import MethodMetaData
+from ._discover.discover import get_openrpc_doc
 
-__all__ = ("RPCServer",)
 log = logging.getLogger("openrpc")
 _META_REF = "https://raw.githubusercontent.com/open-rpc/meta-schema/master/schema.json"
 
 
 class RPCServer(MethodRegistrar):
     """OpenRPC server to register methods with."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         title: Optional[str] = None,
         version: Optional[str] = None,
         description: Optional[str] = None,
         terms_of_service: Optional[str] = None,
         contact: Optional[ContactObject] = None,
         license_: Optional[LicenseObject] = None,
+        debug: bool = False,  # noqa: FBT001,FBT002
     ) -> None:
-        """Init an OpenRPC server.
+        """Init an Open-RPC server.
 
-        :param title: OpenRPC title.
+        :param title: Open-RPC title.
         :param version: API version.
         :param description: Description of the app.
         :param terms_of_service: App terms of service.
         :param contact: Contact information.
         :param license_: App license.
+        :param debug: Include internal error details in responses.
         """
         super().__init__()
+        self._routers: list[MethodRegistrar] = []
+        self._request_processor.debug = debug
         # Set OpenRPC server info.
+        self._debug = debug
         self._info = InfoObject(
             title=title or "RPC Server",
             version=version or "0.1.0",
             description=description,
             termsOfService=terms_of_service,
             contact=contact,
             license=license_,
@@ -117,24 +124,36 @@
     @license_.setter
     def license_(self, license_: LicenseObject) -> None:
         self._info.license_ = license_
 
     @property
     def default_error_code(self) -> int:
         """JSON-RPC error code used when a method raises an error."""
-        return self._method_processor.uncaught_error_code
+        return self._request_processor.uncaught_error_code
 
     @default_error_code.setter
     def default_error_code(self, default_error_code: int) -> None:
-        self._method_processor.uncaught_error_code = default_error_code
+        self._request_processor.uncaught_error_code = default_error_code
 
     @property
     def methods(self) -> list[MethodObject]:
         """Get all methods of this server."""
-        return DiscoverHandler(self._info, self._rpc_methods.values()).execute().methods
+        return get_openrpc_doc(self._info, self._rpc_methods.values()).methods
+
+    @property
+    def debug(self) -> bool:
+        """Include internal error details in responses if True."""
+        return self._debug
+
+    @debug.setter
+    def debug(self, debug: bool) -> None:
+        self._request_processor.debug = debug
+        self._debug = debug
+        for router in self._routers:
+            router.debug = debug
 
     def include_router(
         self,
         router: RPCRouter,
         prefix: Optional[str] = None,
         tags: Optional[list[Union[TagObject, str]]] = None,
     ) -> None:
@@ -145,15 +164,15 @@
         :param tags: Tags to add to methods in this router.
         :return: None.
         """
 
         def _add_router_method(
             func: CallableType, metadata: MethodMetaData
         ) -> CallableType:
-            new_data = metadata.copy()
+            new_data = metadata.model_copy()
             if prefix:
                 new_data.name = f"{prefix}{metadata.name}"
             if tags:
                 tag_objects = [
                     t if isinstance(t, TagObject) else TagObject(name=t) for t in tags
                 ]
                 if new_data.tags:
@@ -170,43 +189,42 @@
                 return func(fun, metadata)
 
             return _wrapper
 
         def _router_remove_partial(method: str) -> None:
             self.remove(f"{prefix}{method}") if prefix else self.remove(method)
             router._rpc_methods.pop(method)
-            router._method_processor.methods.pop(method)
+            router._request_processor.methods.pop(method)
 
         for rpc_method in router._rpc_methods.values():
             _add_router_method(rpc_method.function, rpc_method.metadata)
         router._method = _router_method_decorator(router._method)  # type: ignore
         router.remove = _router_remove_partial  # type: ignore
+        router.debug = self.debug
+        self._routers.append(router)
 
     def process_request(
         self, data: Union[bytes, str], depends: Optional[dict[str, Any]] = None
     ) -> Optional[str]:
         """Process a JSON-RPC2 request and get the response.
 
         :param data: A JSON-RPC2 request.
         :param depends: Values passed to functions with dependencies.
             Values will be passed if the keyname matches the arg name
             that is a dependency.
         :return: A valid JSON-RPC2 response.
         """
         try:
             log.debug("Processing request: %s", data)
-            resp = self._method_processor.process(data, depends)
+            resp = self._request_processor.process(data, depends)
             if resp:
                 log.debug("Responding: %s", resp)
-            return resp
+            return resp  # noqa: TRY300
         except Exception as error:
-            log.exception("%s:", type(error).__name__)
-            error_object = ErrorObjectData(**INTERNAL_ERROR.dict())
-            error_object.data = f"{type(error).__name__}: {', '.join(error.args)}"
-            return error_object.json()
+            return self._get_error_response(error).model_dump_json()
 
     async def process_request_async(
         self, data: Union[bytes, str], depends: Optional[dict[str, Any]] = None
     ) -> Optional[str]:
         """Process a JSON-RPC2 request and get the response.
 
         If the method called by the request is async it will be awaited.
@@ -215,24 +233,32 @@
         :param depends: Values passed to functions with dependencies.
             Values will be passed if the keyname matches the arg name
             that is a dependency.
         :return: A valid JSON-RPC2 response.
         """
         try:
             log.debug("Processing request: %s", data)
-            resp = await self._method_processor.process_async(data, depends)
+            resp = await self._request_processor.process_async(data, depends)
             if resp:
                 log.debug("Responding: %s", resp)
-            return resp
+            return resp  # noqa: TRY300
         except Exception as error:
-            log.exception("%s:", type(error).__name__)
-            error_object = ErrorObjectData(**INTERNAL_ERROR.dict())
-            error_object.data = f"{type(error).__name__}: {', '.join(error.args)}"
-            return error_object.json()
+            return self._get_error_response(error).model_dump_json()
 
     def discover(self) -> dict[str, Any]:
         """Execute "rpc.discover" method defined in OpenRPC spec."""
-        return (
-            DiscoverHandler(self._info, self._rpc_methods.values())
-            .execute()
-            .dict(by_alias=True, exclude_unset=True, exclude_none=True)
+        return get_openrpc_doc(self._info, self._rpc_methods.values()).model_dump(
+            by_alias=True, exclude_unset=True, exclude_none=True
         )
+
+    def _get_error_response(self, error: Exception) -> ErrorResponse:
+        log.exception("%s:", type(error).__name__)
+        if self._debug:
+            error_object: Union[Error, DataError] = DataError(
+                **{
+                    **INTERNAL_ERROR.model_dump(),
+                    **{"data": f"{type(error).__name__}: {error}"},
+                }
+            )
+        else:
+            error_object = Error(**INTERNAL_ERROR.model_dump())
+        return ErrorResponse(id=None, error=error_object)
```

### Comparing `openrpc-6.3.9/pyproject.toml` & `openrpc-7.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openrpc"
-version = "6.3.9"
+version = "7.0.0"
 description = "OpenRPC provides classes to rapidly develop an OpenRPC server."
 readme = "README.md"
 repository = "https://gitlab.com/mburkard/openrpc"
 homepage = "https://gitlab.com/mburkard/openrpc"
 license = "MIT"
 authors = ["Matthew Burkard <matthewjburkard@gmail.com>"]
 classifiers = [
@@ -17,23 +17,58 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = "^1.10.6"
-jsonrpc2-objects = "^2.0.0"
-case-switcher = "^1.2.13"
+pydantic = "^2.0.3"
+jsonrpc2-objects = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 coverage = "^7.1.0"
-flake8 = "^6.0.0"
 mypy = "^1.0.0"
 black = "^23.1.0"
 pytest = "^7.2.1"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = "^0.21.0"
+ruff = "^0.0.280"
 
 [build-system]
 
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.mypy]
+disallow_untyped_defs = true
+ignore_missing_imports = true
+
+[tool.ruff]
+select = [
+    "ARG",
+    "ASYNC",
+    "B",
+    "C4",
+    "D",
+    "E",
+    "EM",
+    "ERA",
+    "F",
+    "FBT",
+    "FA",
+    "FLY",
+    "FIX",
+    "ICN",
+    "INT",
+    "ISC",
+    "N",
+    "PL",
+    "PTH",
+    "PYI",
+    "Q",
+    "RET",
+    "S",
+    "SIM",
+    "T10",
+    "TD",
+    "TRY",
+]
+ignore = ["D203", "D213"]
```

### Comparing `openrpc-6.3.9/PKG-INFO` & `openrpc-7.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 Metadata-Version: 2.1
 Name: openrpc
-Version: 6.3.9
+Version: 7.0.0
 Summary: OpenRPC provides classes to rapidly develop an OpenRPC server.
 Home-page: https://gitlab.com/mburkard/openrpc
 License: MIT
 Author: Matthew Burkard
 Author-email: matthewjburkard@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: case-switcher (>=1.2.13,<2.0.0)
-Requires-Dist: jsonrpc2-objects (>=2.0.0,<3.0.0)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0)
+Requires-Dist: jsonrpc2-objects (>=3.0.0,<4.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Project-URL: Repository, https://gitlab.com/mburkard/openrpc
 Description-Content-Type: text/markdown
 
 <div align=center>
   <h1>OpenRPC</h1>
   <h3>OpenRPC provides classes to rapidly develop an
   <a href="https://open-rpc.org">OpenRPC</a> server.</h3>
@@ -70,18 +66,18 @@
 from openrpc import RPCServer
 
 rpc = RPCServer(title="Demo Server", version="1.0.0")
 ```
 
 ### Register a function as an RPC Method
 
-To register a method with the RPCServer add the `@rpc.method` decorator to a function.
+To register a method with the RPCServer add the `@rpc.method()` decorator to a function.
 
 ```python
-@rpc.method
+@rpc.method()
 def add(a: int, b: int) -> int:
     return a + b
 ```
 
 ### Process JSON RPC Request
 
 OpenRPC is transport agnostic. To use it, pass JSON RPC requests as strings or byte
@@ -121,37 +117,41 @@
 from openrpc import RPCServer
 from sanic import Request, Sanic, Websocket
 
 app = Sanic("DemoServer")
 rpc = RPCServer(title="DemoServer", version="1.0.0")
 
 
-@rpc.method
+@rpc.method()
 async def add(a: int, b: int) -> int:
     return a + b
 
 
 @app.websocket("/api/v1/")
 async def process_websocket(_request: Request, ws: Websocket) -> None:
     async for msg in ws:
         json_rpc_response = await rpc.process_request_async(msg)
-        await ws.send(json_rpc_response)
+        if json_rpc_response is not None:
+            await ws.send(json_rpc_response)
 
 
 if __name__ == "__main__":
     app.run()
 ```
 
 Example In
 
 ```json
 {
   "id": 1,
   "method": "add",
-  "params": {"a": 1, "b": 3},
+  "params": {
+    "a": 1,
+    "b": 3
+  },
   "jsonrpc": "2.0"
 }
 ```
 
 Example Result Out
 
 ```json
```

