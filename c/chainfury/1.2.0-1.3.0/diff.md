# Comparing `tmp/chainfury-1.2.0.tar.gz` & `tmp/chainfury-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainfury-1.2.0.tar", max compression
+gzip compressed data, was "chainfury-1.3.0.tar", max compression
```

## Comparing `chainfury-1.2.0.tar` & `chainfury-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0    11351 2023-06-12 10:47:25.719426 chainfury-1.2.0/LICENSE
--rw-r--r--   0        0        0     8030 2023-06-26 17:41:18.027685 chainfury-1.2.0/README.md
--rw-r--r--   0        0        0      297 2023-06-26 17:41:18.082832 chainfury-1.2.0/chainfury/__init__.py
--rw-r--r--   0        0        0    19865 2023-07-17 10:21:32.408643 chainfury-1.2.0/chainfury/agent.py
--rw-r--r--   0        0        0    46008 2023-07-16 11:49:08.560482 chainfury-1.2.0/chainfury/base.py
--rw-r--r--   0        0        0      766 2023-07-17 09:33:13.149326 chainfury-1.2.0/chainfury/cli.py
--rw-r--r--   0        0        0    13266 2023-07-04 11:02:16.679972 chainfury-1.2.0/chainfury/client.py
--rw-r--r--   0        0        0     1699 2023-06-26 07:50:14.048396 chainfury-1.2.0/chainfury/components/README.md
--rw-r--r--   0        0        0      864 2023-07-03 11:39:00.427129 chainfury-1.2.0/chainfury/components/__init__.py
--rw-r--r--   0        0        0     1146 2023-06-26 07:50:14.048972 chainfury-1.2.0/chainfury/components/ai_actions/__init__.py
--rw-r--r--   0        0        0      836 2023-07-04 04:54:19.835188 chainfury-1.2.0/chainfury/components/const.py
--rw-r--r--   0        0        0     6808 2023-07-16 11:53:54.430158 chainfury-1.2.0/chainfury/components/functional/__init__.py
--rw-r--r--   0        0        0     4603 2023-07-05 13:25:46.908873 chainfury-1.2.0/chainfury/components/nbx/__init__.py
--rw-r--r--   0        0        0    10036 2023-07-07 20:05:42.618404 chainfury-1.2.0/chainfury/components/openai/__init__.py
--rw-r--r--   0        0        0       78 2023-06-26 07:50:14.049729 chainfury-1.2.0/chainfury/components/redis/__init__.py
--rw-r--r--   0        0        0     8659 2023-07-16 12:39:23.305115 chainfury-1.2.0/chainfury/components/serper/__init__.py
--rw-r--r--   0        0        0     9904 2023-07-03 13:14:41.480424 chainfury-1.2.0/chainfury/components/stability/__init__.py
--rw-r--r--   0        0        0     1013 2023-07-04 09:56:27.058762 chainfury-1.2.0/chainfury/types.py
--rw-r--r--   0        0        0     2616 2023-07-03 15:18:38.323479 chainfury-1.2.0/chainfury/utils.py
--rw-r--r--   0        0        0      135 2023-07-17 10:29:18.555431 chainfury-1.2.0/chainfury/version.py
--rw-r--r--   0        0        0      698 2023-07-17 10:29:27.765087 chainfury-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     9495 1970-01-01 00:00:00.000000 chainfury-1.2.0/setup.py
--rw-r--r--   0        0        0     8962 1970-01-01 00:00:00.000000 chainfury-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-06-12 10:47:25.719426 chainfury-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4500 2023-07-26 10:48:59.407812 chainfury-1.3.0/README.md
+-rw-r--r--   0        0        0      361 2023-07-26 11:58:05.957831 chainfury-1.3.0/chainfury/__init__.py
+-rw-r--r--   0        0        0       39 2023-07-26 05:41:33.286898 chainfury-1.3.0/chainfury/__main__.py
+-rw-r--r--   0        0        0    27439 2023-07-27 04:10:46.158868 chainfury-1.3.0/chainfury/agent.py
+-rw-r--r--   0        0        0    47544 2023-07-27 04:28:09.607193 chainfury-1.3.0/chainfury/base.py
+-rw-r--r--   0        0        0     3570 2023-07-26 05:41:33.288177 chainfury-1.3.0/chainfury/cli.py
+-rw-r--r--   0        0        0    13266 2023-07-20 12:08:00.208542 chainfury-1.3.0/chainfury/client.py
+-rw-r--r--   0        0        0     1699 2023-07-20 12:08:00.208666 chainfury-1.3.0/chainfury/components/README.md
+-rw-r--r--   0        0        0      608 2023-07-26 05:41:33.288471 chainfury-1.3.0/chainfury/components/__init__.py
+-rw-r--r--   0        0        0     1146 2023-07-20 12:08:00.209196 chainfury-1.3.0/chainfury/components/ai_actions/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-26 10:43:07.571250 chainfury-1.3.0/chainfury/components/const.py
+-rw-r--r--   0        0        0     6836 2023-07-25 12:00:51.905993 chainfury-1.3.0/chainfury/components/functional/__init__.py
+-rw-r--r--   0        0        0      419 2023-07-21 11:05:44.530297 chainfury-1.3.0/chainfury/components/milvus/__init__.py
+-rw-r--r--   0        0        0     4603 2023-07-20 12:08:00.210177 chainfury-1.3.0/chainfury/components/nbx/__init__.py
+-rw-r--r--   0        0        0    12708 2023-07-26 05:41:33.289125 chainfury-1.3.0/chainfury/components/openai/__init__.py
+-rw-r--r--   0        0        0     2831 2023-07-24 11:27:34.882593 chainfury-1.3.0/chainfury/components/pinecone_db/__init__.py
+-rw-r--r--   0        0        0     9326 2023-07-27 04:41:40.506974 chainfury-1.3.0/chainfury/components/qdrant/__init__.py
+-rw-r--r--   0        0        0       78 2023-07-20 12:08:00.210514 chainfury-1.3.0/chainfury/components/redis/__init__.py
+-rw-r--r--   0        0        0     8659 2023-07-20 12:08:00.210779 chainfury-1.3.0/chainfury/components/serper/__init__.py
+-rw-r--r--   0        0        0     6637 2023-07-20 12:08:00.211018 chainfury-1.3.0/chainfury/components/stability/__init__.py
+-rw-r--r--   0        0        0     1013 2023-07-20 12:08:00.211166 chainfury-1.3.0/chainfury/types.py
+-rw-r--r--   0        0        0     3556 2023-07-26 05:41:33.289789 chainfury-1.3.0/chainfury/utils.py
+-rw-r--r--   0        0        0      135 2023-07-26 05:41:33.290061 chainfury-1.3.0/chainfury/version.py
+-rw-r--r--   0        0        0      935 2023-07-26 07:03:35.791974 chainfury-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 chainfury-1.3.0/setup.py
+-rw-r--r--   0        0        0     5655 1970-01-01 00:00:00.000000 chainfury-1.3.0/PKG-INFO
```

### Comparing `chainfury-1.2.0/LICENSE` & `chainfury-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainfury-1.2.0/chainfury/agent.py` & `chainfury-1.3.0/chainfury/agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -326,15 +326,15 @@
 
         # check for keys even before calling any API or something
         # we need to create a sub dict that only contains the fields that are needed by the preprocessor
         # function and pass the rest of the data to the model call
         _data = {}
         for f in self.fields:
             if f.required and f.name not in data:
-                raise Exception(f"Field {f.name} is required in {self.node_id} but not present")
+                raise Exception(f"Field '{f.name}' is required in {self.node_id} but not present")
             if f.name in data:
                 _data[f.name] = data.pop(f.name)
 
         if self.action_source == AIAction.FUNC:
             try:
                 fn_out = self.fn(**_data)  # type: ignore
                 if self.action_source == AIAction.FUNC and not type(fn_out) == dict:
@@ -547,19 +547,195 @@
 
 ai_actions_registry = AIActionsRegistry()
 """
 `ai_actions_registry` is a global instance of `AIActionsRegistry` class. This is used to register and unregister
 `AIAction` instances. This is used by the server to serve the registered actions.
 """
 
-# Eventually build memory registry like the actions registry
-#
-# class Memory:
-#     def __init__(self, memory_id):
-#         self.node = Node(id=f"cf-memory-{memory_id}", type=Node.types.MEMORY)
-#
-#     # user can subclass this and override the following functions
-#     def get(self, key: str):
-#         ...
-#
-#     def put(self, key: str, value: Any):
-#         ...
+DEFAULT_MEMORY_CONSTANTS = {
+    "openai-embedding": {
+        "embedding_model_key": "input_strings",
+        "embedding_model_params": {
+            "model": "text-embedding-ada-002",
+        },
+        "translation_layer": {
+            "embeddings": ["data", "*", "embedding"],
+        },
+    }
+}
+
+
+class Memory:
+    """Class to wrap the DB functions as a callable.
+
+    Args:
+        node_id (str): The id of the node
+        fn (object): The function that is used for this action
+        vector_key (str): The key for the vector in the DB
+        read_mode (bool, optional): If the function is a read function, if `False` then this is a write function.
+    """
+
+    fields_model = [
+        Var(name="items", type=[Var(type="string"), Var(type="array", items=[Var(type="string")])], required=True),
+        Var(name="embedding_model", type="string", required=True),
+        Var(name="embedding_model_params", type="object", additionalProperties=Var(type="string")),
+        Var(name="embedding_model_key", type="string"),
+        Var(name="translation_layer", type="object", additionalProperties=Var(type="string")),
+    ]
+    """These are the fields that are used to map the input items to the embedding model, do not use directly"""
+
+    def __init__(self, node_id: str, fn: object, vector_key: str, read_mode: bool = False):
+        self.node_id = node_id
+        self.fn = fn
+        self.vector_key = vector_key
+        self.read_mode = read_mode
+        self.fields_fn = func_to_vars(fn)
+        self.fields = self.fields_fn + self.fields_model
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Serialize the Memory object to a dict."""
+        return {
+            "node_id": self.node_id.split("-")[0],
+            "vector_key": self.vector_key,
+            "read_mode": self.read_mode,
+        }
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any]):
+        """Deserialize the Memory object from a dict."""
+        read_mode = data["read_mode"]
+        if read_mode:
+            fn = memory_registry.get_read(data["node_id"])
+        else:
+            fn = memory_registry.get_write(data["node_id"])
+        return fn.fn
+
+    def __call__(self, **data: Dict[str, Any]) -> Any:
+        # the first thing we have to do is get the data for the model. This is actually a very hard problem because this
+        # function needs to call some other arbitrary function where we know the inputs to this function "items" but we
+        # do not know which variable to pass this to in the undelying model's function. Thus we need to take in a huge
+        # amount of things as more inputs ("embedding_model_key", "embedding_model_params"). Then we don't even know
+        # what the inputs to the underlying DB functionbare going to be, in which case we also need to add things like
+        # the translation that needs to be done ("translation_layer"). This makes the number of inputs a lot but
+        # ultimately is required to do the job for robust-ness. Which is why we provide a default for openai-embedding
+        # model. For any other model user will need to pass all the information.
+        model_fields: Dict[str, Any] = {}
+        for f in self.fields_model:
+            if f.required and f.name not in data:
+                raise Exception(f"Field '{f.name}' is required in {self.node_id} but not present")
+            if f.name in data:
+                model_fields[f.name] = data.pop(f.name)
+
+        model_data = {**model_fields.get("embedding_model_params", {})}
+        model_id = model_fields.pop("embedding_model")
+        embedding_model_default_config = DEFAULT_MEMORY_CONSTANTS.get(model_id, {})
+        if embedding_model_default_config:
+            model_data = {**embedding_model_default_config.get("embedding_model_params", {}), **model_data}
+            model_key = embedding_model_default_config.get("embedding_model_key", "items") or model_data.get("embedding_model_key")
+            model_fields["translation_layer"] = model_fields.get("translation_layer") or embedding_model_default_config.get(
+                "translation_layer"
+            )
+        else:
+            req_keys = [x.name for x in self.fields_model[2:]]
+            if not all([x in model_fields for x in req_keys]):
+                raise Exception(f"Model {model_id} requires {req_keys} to be passed")
+            model_key = model_fields.get("embedding_model_key")
+            model_data = {**model_fields.get("embedding_model_params", {}), **model_data}
+        model_data[model_key] = model_fields.pop("items")  # type: ignore
+        model = model_registry.get(model_id)
+        embeddings, err = model(model_data=model_data)
+        if err:
+            logger.error(f"error: {err}")
+            logger.error(f"traceback: {embeddings}")
+            raise err
+
+        # now that we have all the embeddings ready we now need to translate it to be fed into the DB function
+        translated_data = {}
+        for k, v in model_fields.get("translation_layer", {}).items():
+            translated_data[k] = get_value_by_keys(embeddings, v)
+
+        # create the dictionary to call the underlying function
+        db_data = {}
+        for f in self.fields_fn:
+            if f.required and not (f.name in data or f.name in translated_data):
+                raise Exception(f"Field '{f.name}' is required in {self.node_id} but not present")
+            if f.name in data:
+                db_data[f.name] = data.pop(f.name)
+            if f.name in translated_data:
+                db_data[f.name] = translated_data.pop(f.name)
+        out, err = self.fn(**db_data)  # type: ignore
+        return out, err
+
+
+class MemoryRegistry:
+    def __init__(self) -> None:
+        self._memories = {}
+
+    def register_write(
+        self,
+        component_name: str,
+        fn: object,
+        outputs: Dict[str, Any],
+        vector_key: str,
+        description: str = "",
+        tags: List[str] = [],
+    ) -> Node:
+        node_id = f"{component_name}-write"
+        mem_fn = Memory(node_id=node_id, fn=fn, vector_key=vector_key, read_mode=False)
+        output_fields = func_to_return_vars(fn, returns=outputs)
+        node = Node(
+            id=node_id,
+            fn=mem_fn,
+            type=Node.types.MEMORY,
+            fields=mem_fn.fields,
+            outputs=output_fields,
+            description=description,
+            tags=tags,
+        )
+        self._memories[node_id] = node
+        return node
+
+    def register_read(
+        self,
+        component_name: str,
+        fn: object,
+        outputs: Dict[str, Any],
+        vector_key: str,
+        description: str = "",
+        tags: List[str] = [],
+    ) -> Node:
+        node_id = f"{component_name}-read"
+        mem_fn = Memory(node_id=node_id, fn=fn, vector_key=vector_key, read_mode=True)
+        output_fields = func_to_return_vars(fn, returns=outputs)
+        node = Node(
+            id=node_id,
+            fn=mem_fn,
+            type=Node.types.MEMORY,
+            fields=mem_fn.fields,
+            outputs=output_fields,
+            description=description,
+            tags=tags,
+        )
+        self._memories[node_id] = node
+        return node
+
+    def get_write(self, node_id: str) -> Optional[Node]:
+        out = self._memories.get(node_id + "-write", None)
+        if out is None:
+            raise ValueError(f"Memory '{node_id}' not found")
+        return out
+
+    def get_read(self, node_id: str) -> Optional[Node]:
+        out = self._memories.get(node_id + "-read", None)
+        if out is None:
+            raise ValueError(f"Memory '{node_id}' not found")
+        return out
+
+    def get_nodes(self):
+        return {k: v.to_dict() for k, v in self._memories.items()}
+
+
+memory_registry = MemoryRegistry()
+"""
+`memory_registry` is a global instance of MemoryRegistry class. This is used to register and unregister Memory instances.
+This is what the user should use when they want to use the memory elements in their chain.
+"""
```

### Comparing `chainfury-1.2.0/chainfury/base.py` & `chainfury-1.3.0/chainfury/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.show = show
         self.name = name
         #
         self.value = None
         self.loc = loc  # this is the location from which this value is extracted
 
     def __repr__(self) -> str:
-        return f"Var({'*' if self.required else ''}'{self.name}', type={self.type}, items={self.items}, additionalProperties={self.additionalProperties})"
+        return f"Var({'*' if self.required else ''}name='{self.name}', type='{self.type}', items={self.items}, additionalProperties={self.additionalProperties})"
 
     def to_dict(self) -> Dict[str, Any]:
         """Serialise this Var to a dictionary that can be JSON serialised and sent to the client.
 
         Returns:
             Dict[str, Any]: The serialised Var.
         """
@@ -172,15 +172,15 @@
     clients.
 
     Args:
         x (Any): The annotation to convert.
         allow_any (bool): Whether to allow the `Any` type.
         allow_exc (bool): Whether to allow the `Exception` type.
         allow_none (bool): Whether to allow the `None` type.
-        trace (bool, optional): Adds verbosity the schema generation. Defaults to False.
+        trace (bool, optional): Adds verbosity the schema generation also set FURY_LOG_LEVEL='debug'. Defaults to False.
 
     Returns:
         Var: The converted annotation.
     """
     if isinstance(x, type):
         if trace:
             logger.debug("t0")
@@ -474,34 +474,54 @@
             else:
                 new_index = key
             extract_jinja_indices(data=value, current_index=new_index, indices=indices)
 
     return indices
 
 
-def get_value_by_keys(obj, keys) -> Any:
+def get_value_by_keys(obj, keys, *, _first_sentinal: bool = False) -> Any:
     """Takes in an arbitrary nested object and returns the value at the location specified by the keys.
 
     Args:
         obj (Union[List, Dict[str, Any]]): The nested object.
         keys (Union[str, List[str], Tuple[str, ...]]): The keys. See `extract_jinja_indices` for examples.
+        _first_sentinal (bool, optional): flag to tell if this is the first input or not, user should not use this. Defaults to False.
 
     Returns:
         Any: The value at the location specified by the keys.
     """
     if not keys:
         return obj
+
     keys = (keys,) if not isinstance(keys, (list, tuple)) else keys
     key = keys[0]
+
+    if key == "*":
+        if not _first_sentinal:
+            raise ValueError("gvk1: Cannot use wildcard '*' as first key")
+
+        # If the key is "*", apply the subsequent keys to all elements in the current list or dictionary.
+        if isinstance(obj, list):
+            return [get_value_by_keys(elem, keys[1:], _first_sentinal=True) for elem in obj]
+        elif isinstance(obj, dict):
+            return {k: get_value_by_keys(v, keys[1:], _first_sentinal=True) for k, v in obj.items()}
+
     if isinstance(obj, dict):
-        return get_value_by_keys(obj.get(key), keys[1:])
-    elif isinstance(obj, (list, tuple)):
+        return get_value_by_keys(obj.get(key), keys[1:], _first_sentinal=True)
+    elif isinstance(obj, (tuple, list)):
+        try:
+            key = int(key)
+        except ValueError:
+            raise ValueError(f"gvk2: Cannot use key '{key}' on a list")
+        if not type(key) == int:
+            raise ValueError(f"gvk3: Cannot use key '{key}' on a list")
         key = int(key)
         if isinstance(key, int) and 0 <= key < len(obj):
-            return get_value_by_keys(obj[key], keys[1:])
+            return get_value_by_keys(obj[key], keys[1:], _first_sentinal=True)
+
     return None
 
 
 def put_value_by_keys(obj, keys, value: Any):
     """Takes in an arbitrary nested object and sets the value at the location specified by the keys.
 
     Args:
@@ -612,14 +632,16 @@
 
 
 class NodeType:
     PROGRAMATIC = "programatic"
     """constant for the programatic node type"""
     AI = "ai-powered"
     """constant for the AI node type"""
+    MEMORY = "memory"
+    """constant for the memory node type"""
 
 
 class Node:
     types = NodeType()
 
     def __init__(
         self,
@@ -639,20 +661,17 @@
             fn (object): The function to call.
             fields (List[Var]): The fields of the node.
             outputs (List[Var]): The outputs of the node.
             description (str, optional): The description of the node. Defaults to "".
             tags (List[str], optional): The tags for the node. Defaults to [].
         """
         # some bacic checks
-        if type == NodeType.AI:
-            pass
-        elif type == NodeType.PROGRAMATIC:
-            pass
-        else:
-            raise ValueError(f"Invalid node type: {type}, see Node.types for valid types")
+        _valid_types = [getattr(NodeType, x) for x in dir(NodeType) if not x.startswith("__")]
+        if type not in _valid_types:
+            raise ValueError(f"Invalid node type: {type}, {_valid_types}")
 
         # set the values
         self.id = id
         self.type = type
         self.description = description
         self.fields = fields
         self.outputs = outputs
@@ -683,21 +702,23 @@
 
     def to_dict(self) -> Dict[str, Any]:
         """Converts the node to a dictionary.
 
         Returns:
             Dict[str, Any]: The dictionary representation of the node.
         """
-        from chainfury.agent import AIAction
+        from chainfury.agent import AIAction, Memory
 
         fn = {}
         name = self.id
         if isinstance(self.fn, AIAction):
             fn = self.fn.to_dict(no_vars=True)
             name = fn.pop("action_name")
+        elif isinstance(self.fn, Memory):
+            fn = self.fn.to_dict()
 
         return {
             "id": self.id,
             "type": self.type,
             "fn": fn,
             "name": name,
             "description": self.description,
@@ -707,34 +728,43 @@
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any], verbose: bool = False) -> "Node":
         """Creates a node from a dictionary.
 
         Args:
             data (Dict[str, Any]): The dictionary representation of the node.
+            verbose (bool, optional): Whether to print verbose logs. Defaults to False.
 
         Returns:
             Node: The node created from the dictionary.
         """
         if verbose:
             logger.info("Creating node from dict: %s", data)
         fields = [Var.from_dict(x) for x in data["fields"]]
         outputs = [Var.from_dict(x) for x in data["outputs"]]
         fn = data["fn"]
         if not fn:
             raise ValueError(f"Invalid fn: {fn}")
 
-        from chainfury.agent import AIAction
+        from chainfury.agent import AIAction, Memory
+
+        node_type = data["type"]
+        print("----->>>>>", node_type)
+        print("#######", fn)
+        if node_type == NodeType.AI:
+            fn = AIAction.from_dict(fn)
+        elif node_type == NodeType.MEMORY:
+            fn = Memory.from_dict(fn)
 
-        ai_action = AIAction.from_dict(fn)
+            print("ASDFASDFADSFADSFASFD", fn)
 
         return cls(
             id=data["id"],
-            type=data["type"],
-            fn=ai_action,
+            type=node_type,
+            fn=fn,
             description=data["description"],
             fields=fields,
             outputs=outputs,
         )
 
     def to_json(self, indent=None) -> str:
         """Converts the node to a json string.
@@ -775,21 +805,22 @@
             if not data_keys.issubset(template_keys):
                 raise ValueError(f"Invalid keys passed to node '{self.id}': {data_keys - template_keys}")
             if print_thoughts:
                 print(terminal_top_with_text(f"Node: {self.id}"))
                 print("Inputs:\n------")
                 print(pformat(data))
 
+            print("ASSSSSSSSSSS:", self.fn)
             out, err = self.fn(**data)  # type: ignore
             if err:
                 raise err
 
             # this is where we have to polish this outgoing result into the structure as configured in self.outputs
-            # logger.debug("> fnout: ", out)
-            # logger.debug("OUTPUTS:", self.outputs)
+            logger.debug(f"> fn_out: {out}")
+            logger.debug(f"> OUTPUTS: {self.outputs}")
             for o in self.outputs:
                 # logger.debug("  OP:", o.name, o._loc)
                 o.set_value(get_value_by_keys(out, o.loc))
 
             fout = {o.name: o.value for o in self.outputs}
             if print_thoughts:
                 print("Outputs:\n-------")
```

### Comparing `chainfury-1.2.0/chainfury/client.py` & `chainfury-1.3.0/chainfury/client.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.2.0/chainfury/components/README.md` & `chainfury-1.3.0/chainfury/components/README.md`

 * *Files identical despite different names*

### Comparing `chainfury-1.2.0/chainfury/components/ai_actions/__init__.py` & `chainfury-1.3.0/chainfury/components/ai_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.2.0/chainfury/components/functional/__init__.py` & `chainfury-1.3.0/chainfury/components/functional/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         timeout (float, optional): The timeout in seconds. Defaults to 0.
         max_retries (int, optional): The number of times to retry the request. Defaults to 3.
         retry_delay (int, optional): The number of seconds to wait between retries. Defaults to 1.
 
     Returns:
         Tuple[Tuple[str, int], Optional[Exception]]: The response text and status code, and the exception if there was one.
     """
+    method = method.upper()
     if method not in _VALID_HTTP_METHODS:
         raise ValueError(f"method must be one of {_VALID_HTTP_METHODS}")
 
     def _fn():
         with requests.Session() as sess:
             out = sess.request(
                 method,
```

### Comparing `chainfury-1.2.0/chainfury/components/nbx/__init__.py` & `chainfury-1.3.0/chainfury/components/nbx/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.2.0/chainfury/components/openai/__init__.py` & `chainfury-1.3.0/chainfury/components/openai/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     logit_bias: dict = {},
     user: str = "",
     *,
     retry_count: int = 3,
     retry_delay: int = 1,
 ) -> Dict[str, Any]:
     """
-    Generate text completion using OpenAI's GPT-3 API.
+    Generate text completion using OpenAI's GPT API.
 
     Args:
         model (str): ID of the model to use.
         prompt (Union[str, List[Union[str, List[str]]]]): The prompt(s) to generate completions for.
             Encoded as a string, array of strings, array of tokens, or array of token arrays.
         openai_api_key (Secret): The OpenAI API key. Defaults to "" or the OPENAI_TOKEN environment variable.
         max_tokens (Optional[int]): The maximum number of tokens to generate in the completion. Defaults to 16.
@@ -51,14 +51,16 @@
         best_of (Optional[int]): Generates best_of completions server-side and returns the "best".
             Results cannot be streamed. Defaults to 1.
         logit_bias (Optional[dict]): Modify the likelihood of specified tokens appearing in the completion.
             Accepts a json object that maps tokens (specified by their token ID in the GPT tokenizer) to an associated
             bias value from -100 to 100. Defaults to None.
         user (Optional[str]): A unique identifier representing your end-user, which can help OpenAI to monitor and detect
             abuse. Defaults to None.
+        retry_count: Optional. Number of times to retry the API call. Defaults to 3.
+        retry_delay: Optional. Number of seconds to wait before retrying the API call. Defaults to 1.
 
     Returns:
         Any: The completion(s) generated by the API.
 
     """
     if not openai_api_key:
         openai_api_key = Secret(Env.OPENAI_TOKEN("")).value
@@ -141,14 +143,16 @@
         n: Optional. How many chat completion choices to generate for each input message. Defaults to 1.
         stop: Optional. Up to 4 sequences where the API will stop generating further tokens.
         max_tokens: Optional. The maximum number of tokens to generate in the chat completion. The total length of input tokens and generated tokens is limited by the model's context length. Defaults to infinity.
         presence_penalty: Optional. Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the text so far, increasing the model's likelihood to talk about new topics. See more information about frequency and presence penalties. Defaults to 0.
         frequency_penalty: Optional. Number between -2.0 and 2.0. Positive values penalize new tokens based on their existing frequency in the text so far, decreasing the model's likelihood to repeat the same line verbatim. See more information about frequency and presence penalties. Defaults to 0.
         logit_bias: Optional. Modify the likelihood of specified tokens appearing in the completion. Accepts a json object that maps tokens (specified by their token ID in the tokenizer) to an associated bias value from -100 to 100. Mathematically, the bias is added to the logits generated by the model prior to sampling. The exact effect will vary per model, but values between -1 and 1 should decrease or increase likelihood of selection; values like -100 or 100 should result in a ban or exclusive selection of the relevant
         user: Optional. A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. Defaults to None.
+        retry_count: Optional. Number of times to retry the API call. Defaults to 3.
+        retry_delay: Optional. Number of seconds to wait before retrying the API call. Defaults to 1.
 
     Returns:
         Any: The completion(s) generated by the API.
     """
     if not openai_api_key:
         openai_api_key = Secret(Env.OPENAI_TOKEN("")).value
     if not openai_api_key:
@@ -189,7 +193,69 @@
         collection_name="openai",
         id="openai-chat",
         fn=openai_chat,
         description="Given a list of messages describing a conversation, the model will return a response.",
         usage=["usage", "total_tokens"],
     )
 )
+
+
+def openai_embedding(
+    model: str,
+    input_strings: Union[str, List[str]],
+    openai_api_key: Secret = Secret(""),
+    user: str = "",
+    *,
+    retry_count: int = 3,
+    retry_delay: int = 1,
+) -> Any:
+    """
+    Returns a JSON object containing the OpenAI's embeddings API response
+
+    Args:
+        model: ID of the model to use. See the model endpoint compatibility table for details on which models work with the Embeddings API.
+        input_strings: A list of strings to embed, encoded as a string, array of strings, array of tokens, or array of token arrays.
+        openai_api_key (Secret): The OpenAI API key. Defaults to "" or the OPENAI_TOKEN environment variable.
+        user: Optional. A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. Defaults to None.
+        retry_count: Optional. Number of times to retry the API call. Defaults to 3.
+        retry_delay: Optional. Number of seconds to wait before retrying the API call. Defaults to 1.
+
+    Returns:
+        Any: The completion(s) generated by the API.
+    """
+
+    if not openai_api_key:
+        openai_api_key = Secret(Env.OPENAI_TOKEN("")).value
+    if not openai_api_key:
+        raise Exception("OpenAI API key not found. Please set OPENAI_TOKEN environment variable or pass through function")
+
+    def _fn():
+        r = requests.post(
+            "https://api.openai.com/v1/embeddings",
+            headers={
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {openai_api_key}",
+            },
+            json={
+                "model": model,
+                "input": input_strings,
+                "user": user,
+            },
+        )
+        if r.status_code == 401:
+            raise UnAuthException(r.text)
+        if r.status_code != 200:
+            raise Exception(f"OpenAI API returned status code {r.status_code}: {r.text}")
+        return r.json()
+
+    return exponential_backoff(_fn, max_retries=retry_count, retry_delay=retry_delay)
+
+
+model_registry.register(
+    model=Model(
+        collection_name="openai",
+        id="openai-embedding",
+        fn=openai_embedding,
+        description="Given a list of messages create embeddings for each message.",
+        usage=["usage", "total_tokens"],
+    )
+)
```

### Comparing `chainfury-1.2.0/chainfury/components/serper/__init__.py` & `chainfury-1.3.0/chainfury/components/serper/__init__.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.2.0/chainfury/types.py` & `chainfury-1.3.0/chainfury/types.py`

 * *Files identical despite different names*

### Comparing `chainfury-1.2.0/chainfury/utils.py` & `chainfury-1.3.0/chainfury/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,36 @@
 import os
 import time
 import logging
 from typing import Any, Dict
 
 
+class CFEnv:
+    """
+    Single namespace for all environment variables.
+
+    * CF_FOLDER: database connection string
+    """
+
+    CF_FOLDER = lambda: os.path.expanduser(os.getenv("CF_FOLDER", "~/cf"))
+    CF_BLOB_STORAGE = lambda: os.path.join(CFEnv.CF_FOLDER(), "blob")
+
+
+os.makedirs(CFEnv.CF_FOLDER(), exist_ok=True)
+os.makedirs(CFEnv.CF_BLOB_STORAGE(), exist_ok=True)
+
+
+def store_blob(key: str, value: bytes) -> str:
+    """A function that stores the information in a file."""
+    fp = os.path.join(CFEnv.CF_BLOB_STORAGE(), key)
+    with open(fp, "wb") as f:
+        f.write(value)
+    return fp
+
+
 def terminal_top_with_text(msg: str = "") -> str:
     """Prints full wodth text message on the terminal
 
     Args:
         msg (str, optional): The message to print. Defaults to "".
 
     Returns:
@@ -43,14 +66,18 @@
 """
 
 
 class UnAuthException(Exception):
     """Raised when the API returns a 401"""
 
 
+class DoNotRetryException(Exception):
+    """Raised when code tells not to retry"""
+
+
 def exponential_backoff(foo, *args, max_retries=2, retry_delay=1, **kwargs) -> Dict[str, Any]:
     """Exponential backoff function
 
     Args:
         foo (function): The function to call
         max_retries (int, optional): maximum number of retries. Defaults to 2.
         retry_delay (int, optional): Initial delay in seconds. Defaults to 1.
@@ -63,20 +90,31 @@
         Dict[str, Any]: The completion(s) generated by the API.
     """
 
     for attempt in range(max_retries):
         try:
             out = foo(*args, **kwargs)  # Call the function that may crash
             return out  # If successful, break out of the loop and return
+        except DoNotRetryException as e:
+            raise e
         except UnAuthException as e:
-            logger.error(f"Unauth Error: {e}")
             raise e
         except Exception as e:
             logger.warning(f"Function crashed: {e}")
             if attempt == max_retries - 1:
                 logger.error("Max retries reached. Exiting...")
                 raise e
             else:
                 delay = retry_delay * (2**attempt)  # Calculate the backoff delay
                 logger.info(f"Retrying in {delay} seconds...")
                 time.sleep(delay)  # Wait for the calculated delay
     raise Exception("This should never happen")
+
+
+def folder(x: str) -> str:
+    """get the folder of this file path"""
+    return os.path.split(os.path.abspath(x))[0]
+
+
+def joinp(x: str, *args) -> str:
+    """convienience function for os.path.join"""
+    return os.path.join(x, *args)
```

### Comparing `chainfury-1.2.0/pyproject.toml` & `chainfury-1.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 [tool.poetry]
 name = "chainfury"
-version = "1.2.0"
+version = "1.3.0"
 description = "ChainFury is a powerful tool that simplifies the creation and management of chains of prompts, making it easier to build complex chat applications using LLMs."
 authors = ["NimbleBox Engineering <engineering@nimblebox.ai>"]
-license = "Apache V2.0"
+license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/ChainFury"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "0.5.0"
 Jinja2 = "3.1.2"
 jinja2schema = "0.1.4"
 pydantic = "^1.10.7"
 requests = "^2.28.2"
+stability-sdk = { version = "0.8.3", optional = true }
+qdrant-client = { version = "1.3.1", optional = true }
+
+[tool.poetry.extras]
+all = [
+  "stability-sdk",
+  "qdrant-client",
+]
+
+stability = ["stability-sdk"]
+qdrant = ["qdrant-client"]
 
 [tool.poetry.scripts]
 chainfury = "chainfury.cli:main"
 cf = "chainfury.cli:main"
 
 [build-system]
 requires = ["poetry-core"]
```

