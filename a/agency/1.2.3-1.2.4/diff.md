# Comparing `tmp/agency-1.2.3.tar.gz` & `tmp/agency-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-1.2.3.tar", max compression
+gzip compressed data, was "agency-1.2.4.tar", max compression
```

## Comparing `agency-1.2.3.tar` & `agency-1.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35148 2023-07-21 03:42:25.783268 agency-1.2.3/LICENSE
--rw-r--r--   0        0        0    10342 2023-07-21 03:42:25.783268 agency-1.2.3/README.md
--rw-r--r--   0        0        0        0 2023-07-21 03:42:25.783268 agency-1.2.3/agency/__init__.py
--rw-r--r--   0        0        0     9541 2023-07-21 03:42:25.783268 agency-1.2.3/agency/agent.py
--rw-r--r--   0        0        0     7953 2023-07-21 03:42:25.783268 agency-1.2.3/agency/amqp_space.py
--rw-r--r--   0        0        0     2770 2023-07-21 03:42:25.783268 agency-1.2.3/agency/native_space.py
--rw-r--r--   0        0        0      802 2023-07-21 03:42:25.783268 agency-1.2.3/agency/schema.py
--rwxr-xr-x   0        0        0      754 2023-07-21 03:42:25.783268 agency-1.2.3/agency/space.py
--rw-r--r--   0        0        0     3824 2023-07-21 03:42:25.787268 agency-1.2.3/agency/util.py
--rw-r--r--   0        0        0      556 2023-07-21 03:42:27.663282 agency-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    11005 1970-01-01 00:00:00.000000 agency-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-27 02:25:10.950351 agency-1.2.4/LICENSE
+-rw-r--r--   0        0        0     8857 2023-07-27 02:25:10.950351 agency-1.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 02:25:10.950351 agency-1.2.4/agency/__init__.py
+-rw-r--r--   0        0        0     9541 2023-07-27 02:25:10.950351 agency-1.2.4/agency/agent.py
+-rw-r--r--   0        0        0     7951 2023-07-27 02:25:10.950351 agency-1.2.4/agency/amqp_space.py
+-rw-r--r--   0        0        0     2745 2023-07-27 02:25:10.950351 agency-1.2.4/agency/native_space.py
+-rw-r--r--   0        0        0      802 2023-07-27 02:25:10.950351 agency-1.2.4/agency/schema.py
+-rwxr-xr-x   0        0        0      754 2023-07-27 02:25:10.950351 agency-1.2.4/agency/space.py
+-rw-r--r--   0        0        0     5595 2023-07-27 02:25:10.950351 agency-1.2.4/agency/util.py
+-rw-r--r--   0        0        0      512 2023-07-27 02:25:12.242344 agency-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     9484 1970-01-01 00:00:00.000000 agency-1.2.4/PKG-INFO
```

### Comparing `agency-1.2.3/LICENSE` & `agency-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-1.2.3/README.md` & `agency-1.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,79 @@
+Metadata-Version: 2.1
+Name: agency
+Version: 1.2.4
+Summary: A fast and minimal framework for building agent-integrated systems
+License: GPL-3.0
+Author: Daniel Rodriguez
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: colorama (>=0.4,<0.5)
+Requires-Dist: kombu (>=5.3.1,<6.0.0)
+Requires-Dist: pydantic (>=1.8,<2.0)
+Description-Content-Type: text/markdown
+
 # Summary
 
-`agency` is a python library that provides a minimal framework for creating
+Agency is a python library that provides a minimal framework for creating
 agent-integrated systems.
 
-The library provides a simple foundation for connecting agents, software systems,
-and human users by defining actions, callbacks, and access policies that you can
-use to connect, monitor, and interact with your agents.
+The library enables you to connect agents with software systems and human users
+by allowing you to define actions, callbacks, and access policies making it easy
+to connect, monitor, and interact with your agents.
 
-`agency` handles the communication details and allows discovering and invoking
+Agency handles the communication details and allows discovering and invoking
 actions across parties, automatically handling things such as reporting
 exceptions, enforcing access restrictions, and more.
 
 
 ## Features
 
 ### Low-Level API Flexibility
 * Straightforward class/method based agent and action definition
 * Supports defining single process applications or networked agent systems
-using AMQP
 
 ### Observability and Control
 * Before/after action and lifecycle callbacks for observability or other needs
 * Access policies and permission callbacks for access control
 
 ### Performance and Scalability
 * Multithreaded (though python's GIL is a bottleneck for single process apps)
 * AMQP support for multiprocess and networked systems (avoids GIL)
 * [_Python multiprocess support is planned for better scalability on
   single-host systems_](https://github.com/operand/agency/issues/33)
 * [_Decentralized networking support planned_](https://github.com/operand/agency/issues/83)
 
 ### Multimodal support
-* [_In development_](https://github.com/operand/agency/issues/26), though a
-timeline of features is not yet determined.
+* [_In development_](https://github.com/operand/agency/issues/26)
 
-### Full demo available at [`examples/demo`](./examples/demo/)
-* Two OpenAI agent examples
-* HuggingFace transformers agent example
-* Simple Flask/React web interface included
-* Operating system access for agents
+### Demo application available at [`examples/demo`](./examples/demo/)
+* Includes Gradio UI (Flask/React UI also available)
+* Multiple agent examples for experimentation
+  * Two OpenAI agent examples
+  * HuggingFace transformers agent example
+  * Operating system access
 * Docker configuration for reference and development
 
-(_Please note that [a Gradio UI is being developed](https://github.com/operand/agency/issues/82) to replace the Flask/React app above_)
 
 # API Overview
 
-`agency` is an implementation of the [Actor
+Agency is an implementation of the [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) for building AI agent
 integrated systems.
 
-In `agency`, all entities are represented as instances of the `Agent` class.
-This includes all humans, software, and AI-driven agents that may communicate as
+In Agency, all entities are represented as instances of the `Agent` class. This
+includes all human users, software, and AI-driven agents that may communicate as
 part of your application.
 
 All agents may expose "actions" that other agents can discover and invoke at run
-time. An example of a simple agent implemention could be:
+time. An example of a simple agent could be:
 
 ```python
 class CalculatorAgent(Agent):
   def _action__add(a, b):
     return a + b
 ```
 
@@ -112,108 +127,104 @@
 with others until it is added to a common `Space`.
 
 There are two included `Space` implementations to choose from:
 * `NativeSpace` - which connects agents within the same python process
 * `AMQPSpace` - which connects agents across processes and systems using an AMQP
   server like RabbitMQ.
 
-Here is an example of creating a `NativeSpace` and adding two agents to it.
+Finally, here is an example of creating a `NativeSpace` and adding two agents to it.
 
 ```python
 space = NativeSpace()
 space.add(CalculatorAgent("CalcAgent"))
 space.add(AIAgent("AIAgent"))
 # The agents above can now communicate
 ```
 
-These are just some of the main `agency` features. For more detailed information
+These are just some of the main features. For more detailed information
 please see [the docs directory](./docs/).
 
 
 # Install
 
 ```sh
 pip install agency
 ```
 or
 ```sh
 poetry add agency
 ```
 
 
-# Running the Demo Application
-_(Note: [a Gradio app is being developed](https://github.com/operand/agency/issues/82) to replace the following UI soon.)_
+# The Demo Application
 
 To run the demo, please follow the directions at
-[examples/demo](./examples/demo/). After a short boot time you can visit the
-web app at `http://localhost:8080` and you should see a simple chat interface.
-
-The following is a screenshot of the web UI that demonstrates multiple demo
-agents interacting and following orders.
+[examples/demo](./examples/demo/).
 
-The screenshot also demonstrates the results of rejecting an action and
-directing an agent to use a different approach in real time. After I explained
-my rejection of the `read_file` action (which happened behind the scenes on the
-terminal), `"FunctionAI"` appropriately used the `shell_command` action with `wc
--l Dockerfile`.
+The following is a screenshot of the Gradio UI that demonstrates the example
+`OpenAIFunctionAgent` following orders and interacting with the `Host`.
 
 <p align="center">
-  <img src="https://i.ibb.co/nbvLJvg/Screenshot-2023-06-14-at-3-59-01-AM.png"
-       alt="Screenshot-2023-06-14-at-3-59-01-AM" border="0" width=500>
+  <img src="https://i.ibb.co/h29m5S4/Screenshot-2023-07-26-at-4-53-05-PM.png"
+      alt="Screenshot-2023-07-26-at-4-53-05-PM" border="0">
 </p>
 
+The screenshot above also demonstrates rejecting an action and directing an
+agent to use a different approach in real time. After I explained my rejection
+of the `read_file` action (which happened behind the scenes on the terminal),
+`"FunctionAI"` appropriately used the `shell_command` action with `head -n 2
+Dockerfile`.
+
 
 # FAQ
 
-## How does `agency` compare to other agent libraries?
+## How does Agency compare to other agent libraries?
 
 Though you could entirely create a simple agent using only the primitives in
-`agency` (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
-intended to be an agent toolset like other libraries. For example, you won't
-find much support for building prompts or working with vector databases, etc.
-Implementation of agent behavior is left up to you.
-
-`agency` is concerned with providing a minimal communication and control
-foundation on which to define and integrate agent systems in a performant
-and flexible way, allowing developers to create custom agent solutions as
-they see fit.
+Agency (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
+intended to be an all-inclusive toolset like other libraries. For example, it
+does not include support for constructing prompts or working with vector
+databases, etc. Implementation of agent behavior is left up to you.
+
+The goal of Agency is to enable developers to experiment and create their own
+agent solutions by providing a minimal set of functionality. So if you're
+looking for a flexible yet minimal foundation for building your own agent
+system, Agency might be for you.
 
-So if you're looking for a library with just enough structure to build from
-but not so much that it gets in your way, then `agency` might be for you.
 
 ## What are some known limitations or issues?
 
-* `agency` is still in early development. Like many projects in the AI agent
+* Agency is still in early development. Like many projects in the AI agent
   space it is somewhat experimental at this time, with the goal of finding and
   providing a minimal yet useful foundation for building agent systems.
 
   Expect changes to the API over time as features are added or changed. The
-  library follows semver versioning starting at 1.x.x. Minor version updates
-  may contain breaking API changes. Patch versions should not.
+  library follows semver versioning starting at 1.x.x. Patch version updates may
+  contain breaking API changes. Minor versions should not.
 
 * This library makes use of threads for each individual agent. Multithreading
   is limited by [python's
   GIL](https://wiki.python.org/moin/GlobalInterpreterLock), meaning that if you
   run a local model or other heavy computation in the same process as other
   agents, they may have to wait for their "turn". Note that I/O does not block,
   so networked backends or services will execute in parallel.
 
   For blocking processes, it's recommended to use the `AMQPSpace` class and run
-  heavy computations in isolation to avoid blocking other agents. [Multiprocessing
-  support](https://github.com/operand/agency/issues/33) is also planned as
-  another option for avoiding the GIL.
+  heavy computations in isolation to avoid blocking other agents.
+  [Multiprocessing support](https://github.com/operand/agency/issues/33) is also
+  planned as another option for avoiding the GIL.
 
 * This API does not assume or enforce predefined roles like "user", "system",
   "assistant", etc. This is an intentional decision and is not likely to change.
 
-  `agency` is intended to allow potentially large numbers of agents, systems,
-  and people to come together. A small predefined set of roles gets in the way
-  of representing many things generally. This is a core design feature of
-  `agency`: that all entities are represented similarly and may be interacted
-  with through common means.
+  Agency is intended to allow potentially large numbers of agents, systems, and
+  people to come together. A small predefined set of roles gets in the way of
+  representing many things generally. This is a core design feature of Agency:
+  that all entities are represented similarly and may be interacted with through
+  common means.
 
   The lack of roles may require extra work when integrating with role based
   APIs. See the implementation of
   [`OpenAIFunctionAgent`](./examples/demo/agents/openai_function_agent.py) for
   an example.
 
 * There is currently not much by way of storage support. That is mostly left up
@@ -223,74 +234,43 @@
   for storage APIs will likely be considered in the future.
   
 
 # Contributing
 
 Please do!
 
-
 ## Development Installation
 
 ```bash
 git clone git@github.com:operand/agency.git
 cd agency
 poetry install
 ```
 
-
 ## Developing with the Demo Application
 
 See [the demo directory](./examples/demo/) for instructions on how to run the
 demo.
 
 The demo application is written to showcase both native and AMQP spaces and
 several agent examples. It can also be used for experimentation and development.
 
 The application is configured to read the agency library source when running,
 allowing changes to be tested manually.
 
-
 ## Test Suite
 
 Ensure you have Docker installed. A small RabbitMQ container will be
 automatically created.
 
 You can run the test suite with:
 
 ```bash
 poetry run pytest
 ```
 
-
-# Roadmap
-
-- **Multimodal Support**:
-Multimedia transfer for use with multimodal models or other multimedia services.
-
-- **Multiprocess Support**:
-An additional `Space` type utilizing python multiprocessing, as another
-parallelism option for single-host systems.
-
-- **Storage Support**
-Durable session support will be included. Other forms of storage will be
-considered though it's not clear yet what that may look like.
-
-- **Gradio Application**
-The current demo application uses a proof-of-concept quality Flask/React
-web app. A Gradio application will be developed to replace the Flask app
-and serve as a reference example that can be extended or modified.
-
-- **Decentralized Networking**
-An additional `Space` type using decentralized protocols, enabling the
-highest levels of scalability and opening the door for peer-to-peer
-agent networks.
-
-- **More Examples**:
-More examples of integrations with popular AI libraries and services will be
-added.
-
-
 ## Planned Work
 
 [Please see the issues page.](https://github.com/operand/agency/issues)
 
 If you have any suggestions or otherwise, feel free to add an issue!
+
```

### Comparing `agency-1.2.3/agency/agent.py` & `agency-1.2.4/agency/agent.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.3/agency/amqp_space.py` & `agency-1.2.4/agency/amqp_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             # point to point
             routing_key = message['to']
         else:
             # broadcast
             routing_key = self.BROADCAST_KEY
 
         sender._message_log.append(message)
-        if routing_key == self.BROADCAST_KEY or self.__check_queue_exists(routing_key):
+        if routing_key == self.BROADCAST_KEY or self._check_queue_exists(routing_key):
             self.__publish(routing_key, message)
         else:
             if routing_key == sender.id():
                 # if the routing key equals the sender id, we have a problem.
                 # the sender's own queue doesn't exist so we can't route an
                 # error back. raise an exception to prevent an infinite loop.
                 raise Exception("Cannot route error. Missing sender queue.")
@@ -197,15 +197,15 @@
             with connection.Producer(serializer="json") as producer:
                 producer.publish(
                     json.dumps(message),
                     exchange=self.__topic_exchange,
                     routing_key=routing_key,
                 )
 
-    def __check_queue_exists(self, queue_name):
+    def _check_queue_exists(self, queue_name):
         with Connection(**self.__kombu_connection_options) as connection:
             try:
                 with connection.channel() as channel:
                     channel.queue_declare(
                         queue=queue_name,
                         passive=True,
                     )
```

### Comparing `agency-1.2.3/agency/native_space.py` & `agency-1.2.4/agency/native_space.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import queue
 import threading
 import time
 from typing import List
-
-from agency import util
 from agency.agent import Agent
 from agency.schema import MessageSchema
 from agency.space import Space
 
 
 class NativeSpace(Space):
     """
```

### Comparing `agency-1.2.3/agency/schema.py` & `agency-1.2.4/agency/schema.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.3/agency/space.py` & `agency-1.2.4/agency/space.py`

 * *Files identical despite different names*

### Comparing `agency-1.2.3/pyproject.toml` & `agency-1.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [tool.poetry]
 name = "agency"
-version = "1.2.3"
+version = "1.2.4"
 description = "A fast and minimal framework for building agent-integrated systems"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 include = ["agency/**/*"]
 exclude = ["*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-asyncio = "^3.4"
 colorama = "^0.4"
 pydantic = "^1.8"
 kombu = "^5.3.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
-pytest-asyncio = "^0.21.0"
 pytest-randomly = "^3.13.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `agency-1.2.3/PKG-INFO` & `agency-1.2.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,62 @@
-Metadata-Version: 2.1
-Name: agency
-Version: 1.2.3
-Summary: A fast and minimal framework for building agent-integrated systems
-License: GPL-3.0
-Author: Daniel Rodriguez
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asyncio (>=3.4,<4.0)
-Requires-Dist: colorama (>=0.4,<0.5)
-Requires-Dist: kombu (>=5.3.1,<6.0.0)
-Requires-Dist: pydantic (>=1.8,<2.0)
-Description-Content-Type: text/markdown
-
 # Summary
 
-`agency` is a python library that provides a minimal framework for creating
+Agency is a python library that provides a minimal framework for creating
 agent-integrated systems.
 
-The library provides a simple foundation for connecting agents, software systems,
-and human users by defining actions, callbacks, and access policies that you can
-use to connect, monitor, and interact with your agents.
+The library enables you to connect agents with software systems and human users
+by allowing you to define actions, callbacks, and access policies making it easy
+to connect, monitor, and interact with your agents.
 
-`agency` handles the communication details and allows discovering and invoking
+Agency handles the communication details and allows discovering and invoking
 actions across parties, automatically handling things such as reporting
 exceptions, enforcing access restrictions, and more.
 
 
 ## Features
 
 ### Low-Level API Flexibility
 * Straightforward class/method based agent and action definition
 * Supports defining single process applications or networked agent systems
-using AMQP
 
 ### Observability and Control
 * Before/after action and lifecycle callbacks for observability or other needs
 * Access policies and permission callbacks for access control
 
 ### Performance and Scalability
 * Multithreaded (though python's GIL is a bottleneck for single process apps)
 * AMQP support for multiprocess and networked systems (avoids GIL)
 * [_Python multiprocess support is planned for better scalability on
   single-host systems_](https://github.com/operand/agency/issues/33)
 * [_Decentralized networking support planned_](https://github.com/operand/agency/issues/83)
 
 ### Multimodal support
-* [_In development_](https://github.com/operand/agency/issues/26), though a
-timeline of features is not yet determined.
+* [_In development_](https://github.com/operand/agency/issues/26)
 
-### Full demo available at [`examples/demo`](./examples/demo/)
-* Two OpenAI agent examples
-* HuggingFace transformers agent example
-* Simple Flask/React web interface included
-* Operating system access for agents
+### Demo application available at [`examples/demo`](./examples/demo/)
+* Includes Gradio UI (Flask/React UI also available)
+* Multiple agent examples for experimentation
+  * Two OpenAI agent examples
+  * HuggingFace transformers agent example
+  * Operating system access
 * Docker configuration for reference and development
 
-(_Please note that [a Gradio UI is being developed](https://github.com/operand/agency/issues/82) to replace the Flask/React app above_)
 
 # API Overview
 
-`agency` is an implementation of the [Actor
+Agency is an implementation of the [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) for building AI agent
 integrated systems.
 
-In `agency`, all entities are represented as instances of the `Agent` class.
-This includes all humans, software, and AI-driven agents that may communicate as
+In Agency, all entities are represented as instances of the `Agent` class. This
+includes all human users, software, and AI-driven agents that may communicate as
 part of your application.
 
 All agents may expose "actions" that other agents can discover and invoke at run
-time. An example of a simple agent implemention could be:
+time. An example of a simple agent could be:
 
 ```python
 class CalculatorAgent(Agent):
   def _action__add(a, b):
     return a + b
 ```
 
@@ -130,108 +110,104 @@
 with others until it is added to a common `Space`.
 
 There are two included `Space` implementations to choose from:
 * `NativeSpace` - which connects agents within the same python process
 * `AMQPSpace` - which connects agents across processes and systems using an AMQP
   server like RabbitMQ.
 
-Here is an example of creating a `NativeSpace` and adding two agents to it.
+Finally, here is an example of creating a `NativeSpace` and adding two agents to it.
 
 ```python
 space = NativeSpace()
 space.add(CalculatorAgent("CalcAgent"))
 space.add(AIAgent("AIAgent"))
 # The agents above can now communicate
 ```
 
-These are just some of the main `agency` features. For more detailed information
+These are just some of the main features. For more detailed information
 please see [the docs directory](./docs/).
 
 
 # Install
 
 ```sh
 pip install agency
 ```
 or
 ```sh
 poetry add agency
 ```
 
 
-# Running the Demo Application
-_(Note: [a Gradio app is being developed](https://github.com/operand/agency/issues/82) to replace the following UI soon.)_
+# The Demo Application
 
 To run the demo, please follow the directions at
-[examples/demo](./examples/demo/). After a short boot time you can visit the
-web app at `http://localhost:8080` and you should see a simple chat interface.
-
-The following is a screenshot of the web UI that demonstrates multiple demo
-agents interacting and following orders.
+[examples/demo](./examples/demo/).
 
-The screenshot also demonstrates the results of rejecting an action and
-directing an agent to use a different approach in real time. After I explained
-my rejection of the `read_file` action (which happened behind the scenes on the
-terminal), `"FunctionAI"` appropriately used the `shell_command` action with `wc
--l Dockerfile`.
+The following is a screenshot of the Gradio UI that demonstrates the example
+`OpenAIFunctionAgent` following orders and interacting with the `Host`.
 
 <p align="center">
-  <img src="https://i.ibb.co/nbvLJvg/Screenshot-2023-06-14-at-3-59-01-AM.png"
-       alt="Screenshot-2023-06-14-at-3-59-01-AM" border="0" width=500>
+  <img src="https://i.ibb.co/h29m5S4/Screenshot-2023-07-26-at-4-53-05-PM.png"
+      alt="Screenshot-2023-07-26-at-4-53-05-PM" border="0">
 </p>
 
+The screenshot above also demonstrates rejecting an action and directing an
+agent to use a different approach in real time. After I explained my rejection
+of the `read_file` action (which happened behind the scenes on the terminal),
+`"FunctionAI"` appropriately used the `shell_command` action with `head -n 2
+Dockerfile`.
+
 
 # FAQ
 
-## How does `agency` compare to other agent libraries?
+## How does Agency compare to other agent libraries?
 
 Though you could entirely create a simple agent using only the primitives in
-`agency` (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
-intended to be an agent toolset like other libraries. For example, you won't
-find much support for building prompts or working with vector databases, etc.
-Implementation of agent behavior is left up to you.
-
-`agency` is concerned with providing a minimal communication and control
-foundation on which to define and integrate agent systems in a performant
-and flexible way, allowing developers to create custom agent solutions as
-they see fit.
+Agency (see [`examples/demo/agents/`](./examples/demo/agents/)), it is not
+intended to be an all-inclusive toolset like other libraries. For example, it
+does not include support for constructing prompts or working with vector
+databases, etc. Implementation of agent behavior is left up to you.
+
+The goal of Agency is to enable developers to experiment and create their own
+agent solutions by providing a minimal set of functionality. So if you're
+looking for a flexible yet minimal foundation for building your own agent
+system, Agency might be for you.
 
-So if you're looking for a library with just enough structure to build from
-but not so much that it gets in your way, then `agency` might be for you.
 
 ## What are some known limitations or issues?
 
-* `agency` is still in early development. Like many projects in the AI agent
+* Agency is still in early development. Like many projects in the AI agent
   space it is somewhat experimental at this time, with the goal of finding and
   providing a minimal yet useful foundation for building agent systems.
 
   Expect changes to the API over time as features are added or changed. The
-  library follows semver versioning starting at 1.x.x. Minor version updates
-  may contain breaking API changes. Patch versions should not.
+  library follows semver versioning starting at 1.x.x. Patch version updates may
+  contain breaking API changes. Minor versions should not.
 
 * This library makes use of threads for each individual agent. Multithreading
   is limited by [python's
   GIL](https://wiki.python.org/moin/GlobalInterpreterLock), meaning that if you
   run a local model or other heavy computation in the same process as other
   agents, they may have to wait for their "turn". Note that I/O does not block,
   so networked backends or services will execute in parallel.
 
   For blocking processes, it's recommended to use the `AMQPSpace` class and run
-  heavy computations in isolation to avoid blocking other agents. [Multiprocessing
-  support](https://github.com/operand/agency/issues/33) is also planned as
-  another option for avoiding the GIL.
+  heavy computations in isolation to avoid blocking other agents.
+  [Multiprocessing support](https://github.com/operand/agency/issues/33) is also
+  planned as another option for avoiding the GIL.
 
 * This API does not assume or enforce predefined roles like "user", "system",
   "assistant", etc. This is an intentional decision and is not likely to change.
 
-  `agency` is intended to allow potentially large numbers of agents, systems,
-  and people to come together. A small predefined set of roles gets in the way
-  of representing many things generally. This is a core design feature of
-  `agency`: that all entities are represented similarly and may be interacted
-  with through common means.
+  Agency is intended to allow potentially large numbers of agents, systems, and
+  people to come together. A small predefined set of roles gets in the way of
+  representing many things generally. This is a core design feature of Agency:
+  that all entities are represented similarly and may be interacted with through
+  common means.
 
   The lack of roles may require extra work when integrating with role based
   APIs. See the implementation of
   [`OpenAIFunctionAgent`](./examples/demo/agents/openai_function_agent.py) for
   an example.
 
 * There is currently not much by way of storage support. That is mostly left up
@@ -241,75 +217,42 @@
   for storage APIs will likely be considered in the future.
   
 
 # Contributing
 
 Please do!
 
-
 ## Development Installation
 
 ```bash
 git clone git@github.com:operand/agency.git
 cd agency
 poetry install
 ```
 
-
 ## Developing with the Demo Application
 
 See [the demo directory](./examples/demo/) for instructions on how to run the
 demo.
 
 The demo application is written to showcase both native and AMQP spaces and
 several agent examples. It can also be used for experimentation and development.
 
 The application is configured to read the agency library source when running,
 allowing changes to be tested manually.
 
-
 ## Test Suite
 
 Ensure you have Docker installed. A small RabbitMQ container will be
 automatically created.
 
 You can run the test suite with:
 
 ```bash
 poetry run pytest
 ```
 
-
-# Roadmap
-
-- **Multimodal Support**:
-Multimedia transfer for use with multimodal models or other multimedia services.
-
-- **Multiprocess Support**:
-An additional `Space` type utilizing python multiprocessing, as another
-parallelism option for single-host systems.
-
-- **Storage Support**
-Durable session support will be included. Other forms of storage will be
-considered though it's not clear yet what that may look like.
-
-- **Gradio Application**
-The current demo application uses a proof-of-concept quality Flask/React
-web app. A Gradio application will be developed to replace the Flask app
-and serve as a reference example that can be extended or modified.
-
-- **Decentralized Networking**
-An additional `Space` type using decentralized protocols, enabling the
-highest levels of scalability and opening the door for peer-to-peer
-agent networks.
-
-- **More Examples**:
-More examples of integrations with popular AI libraries and services will be
-added.
-
-
 ## Planned Work
 
 [Please see the issues page.](https://github.com/operand/agency/issues)
 
 If you have any suggestions or otherwise, feel free to add an issue!
-
```

