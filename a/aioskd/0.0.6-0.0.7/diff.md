# Comparing `tmp/aioskd-0.0.6.tar.gz` & `tmp/aioskd-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioskd-0.0.6.tar", last modified: Wed Jul 26 18:45:55 2023, max compression
+gzip compressed data, was "aioskd-0.0.7.tar", last modified: Thu Jul 27 16:33:00 2023, max compression
```

## Comparing `aioskd-0.0.6.tar` & `aioskd-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-26 18:45:55.906696 aioskd-0.0.6/
--rw-r--r--   0 bigmag_    (502) staff       (20)     1062 2023-07-25 16:20:16.000000 aioskd-0.0.6/LICENSE
--rw-r--r--   0 bigmag_    (502) staff       (20)     5993 2023-07-26 18:45:55.906852 aioskd-0.0.6/PKG-INFO
--rw-r--r--   0 bigmag_    (502) staff       (20)     5303 2023-07-26 18:41:55.000000 aioskd-0.0.6/README.md
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-26 18:45:55.897926 aioskd-0.0.6/aioskd/
--rw-r--r--   0 bigmag_    (502) staff       (20)       48 2023-07-25 20:22:27.000000 aioskd-0.0.6/aioskd/__init__.py
--rwxr-xr-x   0 bigmag_    (502) staff       (20)     1550 2023-07-26 11:13:59.000000 aioskd-0.0.6/aioskd/cli.py
--rw-r--r--   0 bigmag_    (502) staff       (20)     5212 2023-07-26 13:32:17.000000 aioskd-0.0.6/aioskd/scheduler.py
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-26 18:45:55.902943 aioskd-0.0.6/aioskd.egg-info/
--rw-r--r--   0 bigmag_    (502) staff       (20)     5993 2023-07-26 18:45:55.000000 aioskd-0.0.6/aioskd.egg-info/PKG-INFO
--rw-r--r--   0 bigmag_    (502) staff       (20)      313 2023-07-26 18:45:55.000000 aioskd-0.0.6/aioskd.egg-info/SOURCES.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-26 18:45:55.000000 aioskd-0.0.6/aioskd.egg-info/dependency_links.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)       39 2023-07-26 18:45:55.000000 aioskd-0.0.6/aioskd.egg-info/entry_points.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)       13 2023-07-26 18:45:55.000000 aioskd-0.0.6/aioskd.egg-info/requires.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        7 2023-07-26 18:45:55.000000 aioskd-0.0.6/aioskd.egg-info/top_level.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)       38 2023-07-26 18:45:55.907628 aioskd-0.0.6/setup.cfg
--rw-r--r--   0 bigmag_    (502) staff       (20)     1044 2023-07-26 18:45:28.000000 aioskd-0.0.6/setup.py
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-26 18:45:55.904932 aioskd-0.0.6/tests/
--rw-r--r--   0 bigmag_    (502) staff       (20)     1866 2023-07-26 12:38:24.000000 aioskd-0.0.6/tests/test_cli.py
--rw-r--r--   0 bigmag_    (502) staff       (20)     3636 2023-07-26 17:48:28.000000 aioskd-0.0.6/tests/test_scheduler.py
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-27 16:33:00.259545 aioskd-0.0.7/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1062 2023-07-26 18:50:14.000000 aioskd-0.0.7/LICENSE
+-rw-r--r--   0 bigmag_    (502) staff       (20)     8915 2023-07-27 16:33:00.261148 aioskd-0.0.7/PKG-INFO
+-rw-r--r--   0 bigmag_    (502) staff       (20)     8225 2023-07-27 16:28:49.000000 aioskd-0.0.7/README.md
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-27 16:33:00.238778 aioskd-0.0.7/aioskd/
+-rw-r--r--   0 bigmag_    (502) staff       (20)       48 2023-07-27 14:04:36.000000 aioskd-0.0.7/aioskd/__init__.py
+-rwxr-xr-x   0 bigmag_    (502) staff       (20)     1550 2023-07-26 18:50:14.000000 aioskd-0.0.7/aioskd/cli.py
+-rw-r--r--   0 bigmag_    (502) staff       (20)     6835 2023-07-27 15:45:58.000000 aioskd-0.0.7/aioskd/scheduler.py
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-27 16:33:00.247271 aioskd-0.0.7/aioskd.egg-info/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     8915 2023-07-27 16:33:00.000000 aioskd-0.0.7/aioskd.egg-info/PKG-INFO
+-rw-r--r--   0 bigmag_    (502) staff       (20)      313 2023-07-27 16:33:00.000000 aioskd-0.0.7/aioskd.egg-info/SOURCES.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-27 16:33:00.000000 aioskd-0.0.7/aioskd.egg-info/dependency_links.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)       39 2023-07-27 16:33:00.000000 aioskd-0.0.7/aioskd.egg-info/entry_points.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)       13 2023-07-27 16:33:00.000000 aioskd-0.0.7/aioskd.egg-info/requires.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        7 2023-07-27 16:33:00.000000 aioskd-0.0.7/aioskd.egg-info/top_level.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)       38 2023-07-27 16:33:00.267625 aioskd-0.0.7/setup.cfg
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1044 2023-07-27 16:31:35.000000 aioskd-0.0.7/setup.py
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-27 16:33:00.254191 aioskd-0.0.7/tests/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1866 2023-07-26 18:50:14.000000 aioskd-0.0.7/tests/test_cli.py
+-rw-r--r--   0 bigmag_    (502) staff       (20)     5236 2023-07-27 15:45:41.000000 aioskd-0.0.7/tests/test_scheduler.py
```

### Comparing `aioskd-0.0.6/LICENSE` & `aioskd-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aioskd-0.0.6/PKG-INFO` & `aioskd-0.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 Metadata-Version: 2.1
 Name: aioskd
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tool for execute async background tasks
 Author: Artem Sydorenko
 Author-email: kradworkmail@gmail.com
 Keywords: async,scheduling,background-tasks,asynchronous-programming,scheduler-library,python,task-scheduler,background-processing,concurrency,asyncio,timed-tasks,library,python3,interval-tasks,task-scheduling,asynchronous-background-tasks,background-scheduler,background-jobs,background-execution,task-execution,scheduling-tasks,async-jobs,async-tasks,job-scheduler,task-runner,task-manager
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# aioskd - Asynchronous Background Task Scheduler
+<div align="center">
+	
+# aioskd 
+	
+Asynchronous Background Task Scheduler
+
 [![PyPI version](https://img.shields.io/pypi/v/aioskd.svg)](https://pypi.org/project/aioskd/)
 ![License](https://img.shields.io/github/license/kradt/aioskd)
 [![codecov](https://codecov.io/gh/kradt/aioskd/branch/main/graph/badge.svg?token=P0YWHFXKQP)](https://codecov.io/gh/kradt/aioskd)
 [![tests](https://github.com/kradt/aioskd/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/kradt/aioskd/actions/workflows/ci_tests.yml)
+</div>
 
+## Project Overview
+
+aioskd is a powerful Python library designed to handle the execution of background tasks asynchronously and at scheduled intervals. It provides an efficient and flexible scheduler, making it effortless to integrate asynchronous background processing into your Python projects.
+
+As applications grow more complex, certain tasks need to be executed in the background without affecting the responsiveness of the main application. AIOSKD is the perfect solution for such scenarios, as it allows you to offload these tasks to asynchronous workers, ensuring smooth execution and a better user experience.
 
-aioskd is a powerful tool for executing background tasks asynchronously at scheduled intervals. It features a flexible scheduler that can be easily adapted to suit the user's specific needs.
 
 ## Features
 
 - Asynchronous execution of background tasks
 - Customizable scheduling of tasks at specified intervals
 - Easy-to-use API for integrating with your Python projects
 - Lightweight and efficient
@@ -43,39 +53,54 @@
 ```python
 from aioskd import Scheduler
 
 
 skd = Scheduler()
 ```
 
-### Scheduling Tasks
+## Scheduling Tasks
 
-You can now schedule tasks using the `schedule` decorator. 
+### Scheduling Tasks with Decorators (Existing Method)
+You can schedule tasks using the schedule decorator as shown below:
 
 ```python
-import datetime
-import asyncio  
 
+import datetime
+import asyncio
 
 @skd.schedule(interval=datetime.timedelta(seconds=1))
 async def task_one():
     print("Task One - Hello world!")     
-    await asyncio.sleep(2)  
-    # Simulate some async work taking 2 seconds  
-	
+    await asyncio.sleep(2)  # Simulate some async work taking 2 seconds  
 
 @skd.schedule(interval=datetime.timedelta(seconds=5))
 async def task_two():
     print("Task Two - I'm running every 5 seconds!")
-    await asyncio.sleep(1) 
-    # Simulate some async work taking 1 second
+    await asyncio.sleep(1)  # Simulate some async work taking 1 second
 ```
 
+### Scheduling Tasks without Decorators (New Method)
+Alternatively, you can also register tasks without using decorators. Here's how you can do it:
+
+```python
+
+import datetime
+import asyncio
+from aioskd import Scheduler
+
+skd = Scheduler()
+
+async def test_task(name: str, age: int = 25):
+    print(f"Hello {name} with age {age}")
 
-In this example, `task_one` will be executed every 1 second, and `task_two` will be executed every 5 seconds.
+skd.register_task(test_task, "John", age=30).schedule(interval=datetime.timedelta(seconds=5))
+skd.register_task(test_task, "Alice", age=28).schedule(interval=datetime.timedelta(seconds=2))
+```
+In this example, the test_task function is registered with the scheduler using the register_task method. 
+You can pass the function along with its arguments to register_task, and then schedule it with the desired interval using the schedule method.
 
 ### Running the Scheduler
 
 To start the scheduler and run the scheduled tasks, you can use the `run()` method:
 
 ```python
 skd.run()
@@ -145,16 +170,66 @@
 	await server.starttls()
 	await server.login("your_email@example.com", "your_email_password")
 	await server.send_message(msg)
 
 if __name__ == "__main__":
     skd.run()
 ```
+This example schedules the send_reminder_email task to run once every 24 hours, sending a reminder email to a specified recipient about an upcoming appointment.
+
+### Example 3: Sending Weather Update Emails
 
-This example schedules the `send_reminder_email` task to run once every 24 hours, sending a reminder email to a specified recipient about an upcoming appointment.
+```python
+import datetime
+import asyncio
+import aiohttp
+import aiosmtplib
+from email.message import EmailMessage
+from aioskd import Scheduler
+
+
+skd = Scheduler()
+
+async def get_weather_data(city: str) -> dict:
+    url = f"https://api.openweathermap.org/data/2.5/weather?q={city}&appid=YOUR_OPENWEATHERMAP_API_KEY"
+    async with aiohttp.ClientSession() as session:
+        async with session.get(url) as response:
+            data = await response.json()
+            return data
+
+
+async def send_weather_email(city: str, recipient: str):
+    data = await get_weather_data(city)
+    temperature = data["main"]["temp"]
+    description = data["weather"][0]["description"]
+    email_content = f"Weather Update for {city}:\n\nTemperature: {temperature} °C\nDescription: {description}"
+    msg = EmailMessage()
+    msg.set_content(email_content)
+    msg["Subject"] = f"Weather Update for {city}"
+    msg["From"] = "your_email@example.com"
+    msg["To"] = recipient
+    async with aiosmtplib.SMTP("smtp.example.com", 587) as server:
+        await server.starttls()
+        await server.login("your_email@example.com", "your_email_password")
+        await server.send_message(msg)
+        print(f"Weather update email sent to {recipient}")  
+
+
+# Register tasks with different cities and recipients
+task1 = skd.register_task(send_weather_email, "London", recipient="recipient1@example.com")
+task1.schedule(interval=datetime.timedelta(hours=1))
+
+task2 = skd.register_task(send_weather_email, "New York", recipient="recipient2@example.com")
+task2.schedule(interval=datetime.timedelta(hours=2))
+
+if __name__ == "__main__":
+    skd.run()
+
+```
+This code demonstrates the use of AIOSKD to send weather updates via email.
 
 ### `schedule` Decorator
 
 - **interval**: `datetime.timedelta` 
 	- The interval between which the asynchronous function should be executed. 
 - **repeat**: `bool` 
 	- A flag that indicates whether the asynchronous function should be repeated or executed only once. - If set to `True`, the function will be scheduled to run repeatedly at the specified interval. - If set to `False`, the function will be executed only once.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aioskd-0.0.6/README.md` & `aioskd-0.0.7/aioskd.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,37 @@
-# aioskd - Asynchronous Background Task Scheduler
+Metadata-Version: 2.1
+Name: aioskd
+Version: 0.0.7
+Summary: Tool for execute async background tasks
+Author: Artem Sydorenko
+Author-email: kradworkmail@gmail.com
+Keywords: async,scheduling,background-tasks,asynchronous-programming,scheduler-library,python,task-scheduler,background-processing,concurrency,asyncio,timed-tasks,library,python3,interval-tasks,task-scheduling,asynchronous-background-tasks,background-scheduler,background-jobs,background-execution,task-execution,scheduling-tasks,async-jobs,async-tasks,job-scheduler,task-runner,task-manager
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+	
+# aioskd 
+	
+Asynchronous Background Task Scheduler
+
 [![PyPI version](https://img.shields.io/pypi/v/aioskd.svg)](https://pypi.org/project/aioskd/)
 ![License](https://img.shields.io/github/license/kradt/aioskd)
 [![codecov](https://codecov.io/gh/kradt/aioskd/branch/main/graph/badge.svg?token=P0YWHFXKQP)](https://codecov.io/gh/kradt/aioskd)
 [![tests](https://github.com/kradt/aioskd/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/kradt/aioskd/actions/workflows/ci_tests.yml)
+</div>
+
+## Project Overview
+
+aioskd is a powerful Python library designed to handle the execution of background tasks asynchronously and at scheduled intervals. It provides an efficient and flexible scheduler, making it effortless to integrate asynchronous background processing into your Python projects.
 
+As applications grow more complex, certain tasks need to be executed in the background without affecting the responsiveness of the main application. AIOSKD is the perfect solution for such scenarios, as it allows you to offload these tasks to asynchronous workers, ensuring smooth execution and a better user experience.
 
-aioskd is a powerful tool for executing background tasks asynchronously at scheduled intervals. It features a flexible scheduler that can be easily adapted to suit the user's specific needs.
 
 ## Features
 
 - Asynchronous execution of background tasks
 - Customizable scheduling of tasks at specified intervals
 - Easy-to-use API for integrating with your Python projects
 - Lightweight and efficient
@@ -31,39 +53,54 @@
 ```python
 from aioskd import Scheduler
 
 
 skd = Scheduler()
 ```
 
-### Scheduling Tasks
+## Scheduling Tasks
 
-You can now schedule tasks using the `schedule` decorator. 
+### Scheduling Tasks with Decorators (Existing Method)
+You can schedule tasks using the schedule decorator as shown below:
 
 ```python
-import datetime
-import asyncio  
 
+import datetime
+import asyncio
 
 @skd.schedule(interval=datetime.timedelta(seconds=1))
 async def task_one():
     print("Task One - Hello world!")     
-    await asyncio.sleep(2)  
-    # Simulate some async work taking 2 seconds  
-	
+    await asyncio.sleep(2)  # Simulate some async work taking 2 seconds  
 
 @skd.schedule(interval=datetime.timedelta(seconds=5))
 async def task_two():
     print("Task Two - I'm running every 5 seconds!")
-    await asyncio.sleep(1) 
-    # Simulate some async work taking 1 second
+    await asyncio.sleep(1)  # Simulate some async work taking 1 second
 ```
 
+### Scheduling Tasks without Decorators (New Method)
+Alternatively, you can also register tasks without using decorators. Here's how you can do it:
+
+```python
+
+import datetime
+import asyncio
+from aioskd import Scheduler
+
+skd = Scheduler()
+
+async def test_task(name: str, age: int = 25):
+    print(f"Hello {name} with age {age}")
 
-In this example, `task_one` will be executed every 1 second, and `task_two` will be executed every 5 seconds.
+skd.register_task(test_task, "John", age=30).schedule(interval=datetime.timedelta(seconds=5))
+skd.register_task(test_task, "Alice", age=28).schedule(interval=datetime.timedelta(seconds=2))
+```
+In this example, the test_task function is registered with the scheduler using the register_task method. 
+You can pass the function along with its arguments to register_task, and then schedule it with the desired interval using the schedule method.
 
 ### Running the Scheduler
 
 To start the scheduler and run the scheduled tasks, you can use the `run()` method:
 
 ```python
 skd.run()
@@ -133,16 +170,66 @@
 	await server.starttls()
 	await server.login("your_email@example.com", "your_email_password")
 	await server.send_message(msg)
 
 if __name__ == "__main__":
     skd.run()
 ```
+This example schedules the send_reminder_email task to run once every 24 hours, sending a reminder email to a specified recipient about an upcoming appointment.
+
+### Example 3: Sending Weather Update Emails
+
+```python
+import datetime
+import asyncio
+import aiohttp
+import aiosmtplib
+from email.message import EmailMessage
+from aioskd import Scheduler
+
+
+skd = Scheduler()
+
+async def get_weather_data(city: str) -> dict:
+    url = f"https://api.openweathermap.org/data/2.5/weather?q={city}&appid=YOUR_OPENWEATHERMAP_API_KEY"
+    async with aiohttp.ClientSession() as session:
+        async with session.get(url) as response:
+            data = await response.json()
+            return data
+
 
-This example schedules the `send_reminder_email` task to run once every 24 hours, sending a reminder email to a specified recipient about an upcoming appointment.
+async def send_weather_email(city: str, recipient: str):
+    data = await get_weather_data(city)
+    temperature = data["main"]["temp"]
+    description = data["weather"][0]["description"]
+    email_content = f"Weather Update for {city}:\n\nTemperature: {temperature} °C\nDescription: {description}"
+    msg = EmailMessage()
+    msg.set_content(email_content)
+    msg["Subject"] = f"Weather Update for {city}"
+    msg["From"] = "your_email@example.com"
+    msg["To"] = recipient
+    async with aiosmtplib.SMTP("smtp.example.com", 587) as server:
+        await server.starttls()
+        await server.login("your_email@example.com", "your_email_password")
+        await server.send_message(msg)
+        print(f"Weather update email sent to {recipient}")  
+
+
+# Register tasks with different cities and recipients
+task1 = skd.register_task(send_weather_email, "London", recipient="recipient1@example.com")
+task1.schedule(interval=datetime.timedelta(hours=1))
+
+task2 = skd.register_task(send_weather_email, "New York", recipient="recipient2@example.com")
+task2.schedule(interval=datetime.timedelta(hours=2))
+
+if __name__ == "__main__":
+    skd.run()
+
+```
+This code demonstrates the use of AIOSKD to send weather updates via email.
 
 ### `schedule` Decorator
 
 - **interval**: `datetime.timedelta` 
 	- The interval between which the asynchronous function should be executed. 
 - **repeat**: `bool` 
 	- A flag that indicates whether the asynchronous function should be repeated or executed only once. - If set to `True`, the function will be scheduled to run repeatedly at the specified interval. - If set to `False`, the function will be executed only once.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aioskd-0.0.6/aioskd/cli.py` & `aioskd-0.0.7/aioskd/cli.py`

 * *Files identical despite different names*

### Comparing `aioskd-0.0.6/aioskd.egg-info/PKG-INFO` & `aioskd-0.0.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 2.1
-Name: aioskd
-Version: 0.0.6
-Summary: Tool for execute async background tasks
-Author: Artem Sydorenko
-Author-email: kradworkmail@gmail.com
-Keywords: async,scheduling,background-tasks,asynchronous-programming,scheduler-library,python,task-scheduler,background-processing,concurrency,asyncio,timed-tasks,library,python3,interval-tasks,task-scheduling,asynchronous-background-tasks,background-scheduler,background-jobs,background-execution,task-execution,scheduling-tasks,async-jobs,async-tasks,job-scheduler,task-runner,task-manager
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<div align="center">
+	
+# aioskd 
+	
+Asynchronous Background Task Scheduler
 
-# aioskd - Asynchronous Background Task Scheduler
 [![PyPI version](https://img.shields.io/pypi/v/aioskd.svg)](https://pypi.org/project/aioskd/)
 ![License](https://img.shields.io/github/license/kradt/aioskd)
 [![codecov](https://codecov.io/gh/kradt/aioskd/branch/main/graph/badge.svg?token=P0YWHFXKQP)](https://codecov.io/gh/kradt/aioskd)
 [![tests](https://github.com/kradt/aioskd/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/kradt/aioskd/actions/workflows/ci_tests.yml)
+</div>
+
+## Project Overview
 
+aioskd is a powerful Python library designed to handle the execution of background tasks asynchronously and at scheduled intervals. It provides an efficient and flexible scheduler, making it effortless to integrate asynchronous background processing into your Python projects.
+
+As applications grow more complex, certain tasks need to be executed in the background without affecting the responsiveness of the main application. AIOSKD is the perfect solution for such scenarios, as it allows you to offload these tasks to asynchronous workers, ensuring smooth execution and a better user experience.
 
-aioskd is a powerful tool for executing background tasks asynchronously at scheduled intervals. It features a flexible scheduler that can be easily adapted to suit the user's specific needs.
 
 ## Features
 
 - Asynchronous execution of background tasks
 - Customizable scheduling of tasks at specified intervals
 - Easy-to-use API for integrating with your Python projects
 - Lightweight and efficient
@@ -43,39 +41,54 @@
 ```python
 from aioskd import Scheduler
 
 
 skd = Scheduler()
 ```
 
-### Scheduling Tasks
+## Scheduling Tasks
 
-You can now schedule tasks using the `schedule` decorator. 
+### Scheduling Tasks with Decorators (Existing Method)
+You can schedule tasks using the schedule decorator as shown below:
 
 ```python
-import datetime
-import asyncio  
 
+import datetime
+import asyncio
 
 @skd.schedule(interval=datetime.timedelta(seconds=1))
 async def task_one():
     print("Task One - Hello world!")     
-    await asyncio.sleep(2)  
-    # Simulate some async work taking 2 seconds  
-	
+    await asyncio.sleep(2)  # Simulate some async work taking 2 seconds  
 
 @skd.schedule(interval=datetime.timedelta(seconds=5))
 async def task_two():
     print("Task Two - I'm running every 5 seconds!")
-    await asyncio.sleep(1) 
-    # Simulate some async work taking 1 second
+    await asyncio.sleep(1)  # Simulate some async work taking 1 second
 ```
 
+### Scheduling Tasks without Decorators (New Method)
+Alternatively, you can also register tasks without using decorators. Here's how you can do it:
 
-In this example, `task_one` will be executed every 1 second, and `task_two` will be executed every 5 seconds.
+```python
+
+import datetime
+import asyncio
+from aioskd import Scheduler
+
+skd = Scheduler()
+
+async def test_task(name: str, age: int = 25):
+    print(f"Hello {name} with age {age}")
+
+skd.register_task(test_task, "John", age=30).schedule(interval=datetime.timedelta(seconds=5))
+skd.register_task(test_task, "Alice", age=28).schedule(interval=datetime.timedelta(seconds=2))
+```
+In this example, the test_task function is registered with the scheduler using the register_task method. 
+You can pass the function along with its arguments to register_task, and then schedule it with the desired interval using the schedule method.
 
 ### Running the Scheduler
 
 To start the scheduler and run the scheduled tasks, you can use the `run()` method:
 
 ```python
 skd.run()
@@ -145,16 +158,66 @@
 	await server.starttls()
 	await server.login("your_email@example.com", "your_email_password")
 	await server.send_message(msg)
 
 if __name__ == "__main__":
     skd.run()
 ```
+This example schedules the send_reminder_email task to run once every 24 hours, sending a reminder email to a specified recipient about an upcoming appointment.
+
+### Example 3: Sending Weather Update Emails
+
+```python
+import datetime
+import asyncio
+import aiohttp
+import aiosmtplib
+from email.message import EmailMessage
+from aioskd import Scheduler
+
+
+skd = Scheduler()
+
+async def get_weather_data(city: str) -> dict:
+    url = f"https://api.openweathermap.org/data/2.5/weather?q={city}&appid=YOUR_OPENWEATHERMAP_API_KEY"
+    async with aiohttp.ClientSession() as session:
+        async with session.get(url) as response:
+            data = await response.json()
+            return data
+
 
-This example schedules the `send_reminder_email` task to run once every 24 hours, sending a reminder email to a specified recipient about an upcoming appointment.
+async def send_weather_email(city: str, recipient: str):
+    data = await get_weather_data(city)
+    temperature = data["main"]["temp"]
+    description = data["weather"][0]["description"]
+    email_content = f"Weather Update for {city}:\n\nTemperature: {temperature} °C\nDescription: {description}"
+    msg = EmailMessage()
+    msg.set_content(email_content)
+    msg["Subject"] = f"Weather Update for {city}"
+    msg["From"] = "your_email@example.com"
+    msg["To"] = recipient
+    async with aiosmtplib.SMTP("smtp.example.com", 587) as server:
+        await server.starttls()
+        await server.login("your_email@example.com", "your_email_password")
+        await server.send_message(msg)
+        print(f"Weather update email sent to {recipient}")  
+
+
+# Register tasks with different cities and recipients
+task1 = skd.register_task(send_weather_email, "London", recipient="recipient1@example.com")
+task1.schedule(interval=datetime.timedelta(hours=1))
+
+task2 = skd.register_task(send_weather_email, "New York", recipient="recipient2@example.com")
+task2.schedule(interval=datetime.timedelta(hours=2))
+
+if __name__ == "__main__":
+    skd.run()
+
+```
+This code demonstrates the use of AIOSKD to send weather updates via email.
 
 ### `schedule` Decorator
 
 - **interval**: `datetime.timedelta` 
 	- The interval between which the asynchronous function should be executed. 
 - **repeat**: `bool` 
 	- A flag that indicates whether the asynchronous function should be repeated or executed only once. - If set to `True`, the function will be scheduled to run repeatedly at the specified interval. - If set to `False`, the function will be executed only once.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aioskd-0.0.6/setup.py` & `aioskd-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_readme():
     with open("README.md", "r") as file:
         return file.read()
 
 
 setup(
   name='aioskd',
-  version='0.0.6',
+  version='0.0.7',
   author='Artem Sydorenko',
   author_email='kradworkmail@gmail.com',
   description='Tool for execute async background tasks',
   long_description=get_readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['click==8.1.3'],
```

### Comparing `aioskd-0.0.6/tests/test_cli.py` & `aioskd-0.0.7/tests/test_cli.py`

 * *Files identical despite different names*

