# Comparing `tmp/chariot-sdk-1.3.1.tar.gz` & `tmp/chariot-sdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chariot-sdk-1.3.1.tar", last modified: Mon Jun  5 05:44:44 2023, max compression
+gzip compressed data, was "chariot-sdk-1.3.2.tar", last modified: Thu Jul 27 03:37:59 2023, max compression
```

## Comparing `chariot-sdk-1.3.1.tar` & `chariot-sdk-1.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 05:44:44.262516 chariot-sdk-1.3.1/
--rw-rw-rw-   0        0        0      225 2023-04-06 02:58:21.000000 chariot-sdk-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6048 2023-06-05 05:44:44.261632 chariot-sdk-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5796 2023-06-05 03:58:05.000000 chariot-sdk-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 05:44:44.197076 chariot-sdk-1.3.1/chariotCore/
--rw-rw-rw-   0        0        0       20 2023-04-19 03:33:16.000000 chariot-sdk-1.3.1/chariotCore/__init__.py
--rw-rw-rw-   0        0        0     5390 2023-04-27 03:57:04.000000 chariot-sdk-1.3.1/chariotCore/main.py
-drwxrwxrwx   0        0        0        0 2023-06-05 05:44:44.205077 chariot-sdk-1.3.1/chariotCore/res/
--rw-rw-rw-   0        0        0      728 2023-04-19 03:33:43.000000 chariot-sdk-1.3.1/chariotCore/res/Dockerfile
-drwxrwxrwx   0        0        0        0 2023-06-05 05:44:44.222054 chariot-sdk-1.3.1/chariotCore/res/SDK/
--rw-rw-rw-   0        0        0       18 2023-04-14 04:07:29.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/__init__.py
--rw-rw-rw-   0        0        0    20196 2023-04-20 02:42:22.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/base.py
--rw-rw-rw-   0        0        0     4104 2023-04-20 03:52:25.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/chariot.py
--rw-rw-rw-   0        0        0     2382 2023-04-10 07:11:20.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/cli.py
--rw-rw-rw-   0        0        0     2641 2023-05-06 10:07:45.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/models.py
--rw-rw-rw-   0        0        0    12157 2023-04-10 07:11:24.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/subassembly.py
--rw-rw-rw-   0        0        0    18426 2023-05-12 02:19:25.000000 chariot-sdk-1.3.1/chariotCore/res/SDK/web.py
--rw-rw-rw-   0        0        0        1 2023-03-22 01:39:01.000000 chariot-sdk-1.3.1/chariotCore/res/__init__.py
--rw-rw-rw-   0        0        0      712 2023-04-27 08:19:16.000000 chariot-sdk-1.3.1/chariotCore/res/config.ini
--rw-rw-rw-   0        0        0    29297 2022-04-11 01:54:53.000000 chariot-sdk-1.3.1/chariotCore/res/icon.png
--rw-rw-rw-   0        0        0      161 2023-04-23 02:20:36.000000 chariot-sdk-1.3.1/chariotCore/res/plugin.spec.yaml
--rw-rw-rw-   0        0        0       73 2023-03-22 01:39:45.000000 chariot-sdk-1.3.1/chariotCore/res/requirements.txt
--rw-rw-rw-   0        0        0    12874 2023-04-27 08:17:13.000000 chariot-sdk-1.3.1/chariotCore/tasks.py
--rw-rw-rw-   0        0        0    29369 2023-05-19 02:36:28.000000 chariot-sdk-1.3.1/chariotCore/templates.py
--rw-rw-rw-   0        0        0    40487 2023-05-16 06:23:27.000000 chariot-sdk-1.3.1/chariotCore/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-05 05:44:44.260925 chariot-sdk-1.3.1/chariot_sdk.egg-info/
--rw-rw-rw-   0        0        0     6048 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      736 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-05 05:44:44.000000 chariot-sdk-1.3.1/chariot_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 05:44:44.262516 chariot-sdk-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1255 2023-04-06 02:58:22.000000 chariot-sdk-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:37:59.271569 chariot-sdk-1.3.2/
+-rw-rw-rw-   0        0        0      225 2023-04-06 02:58:21.000000 chariot-sdk-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6588 2023-07-27 03:37:59.270569 chariot-sdk-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6336 2023-07-27 03:26:26.000000 chariot-sdk-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 03:37:59.243570 chariot-sdk-1.3.2/chariotCore/
+-rw-rw-rw-   0        0        0       20 2023-07-13 01:33:58.000000 chariot-sdk-1.3.2/chariotCore/__init__.py
+-rw-rw-rw-   0        0        0     5390 2023-04-27 03:57:04.000000 chariot-sdk-1.3.2/chariotCore/main.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:37:59.250573 chariot-sdk-1.3.2/chariotCore/res/
+-rw-rw-rw-   0        0        0      848 2023-06-21 03:51:37.000000 chariot-sdk-1.3.2/chariotCore/res/Dockerfile
+drwxrwxrwx   0        0        0        0 2023-07-27 03:37:59.259569 chariot-sdk-1.3.2/chariotCore/res/SDK/
+-rw-rw-rw-   0        0        0       18 2023-06-15 02:44:21.000000 chariot-sdk-1.3.2/chariotCore/res/SDK/__init__.py
+-rw-rw-rw-   0        0        0    20118 2023-07-17 07:37:10.000000 chariot-sdk-1.3.2/chariotCore/res/SDK/base.py
+-rw-rw-rw-   0        0        0     5036 2023-07-19 05:48:10.000000 chariot-sdk-1.3.2/chariotCore/res/SDK/chariot.py
+-rw-rw-rw-   0        0        0     2526 2023-07-19 01:41:29.000000 chariot-sdk-1.3.2/chariotCore/res/SDK/cli.py
+-rw-rw-rw-   0        0        0     2677 2023-07-27 03:37:34.000000 chariot-sdk-1.3.2/chariotCore/res/SDK/models.py
+-rw-rw-rw-   0        0        0    14550 2023-07-13 03:44:18.000000 chariot-sdk-1.3.2/chariotCore/res/SDK/subassembly.py
+-rw-rw-rw-   0        0        0    23082 2023-07-27 02:38:02.000000 chariot-sdk-1.3.2/chariotCore/res/SDK/web.py
+-rw-rw-rw-   0        0        0        1 2023-03-22 01:39:01.000000 chariot-sdk-1.3.2/chariotCore/res/__init__.py
+-rw-rw-rw-   0        0        0      712 2023-04-27 08:19:16.000000 chariot-sdk-1.3.2/chariotCore/res/config.ini
+-rw-rw-rw-   0        0        0    29297 2022-04-11 01:54:53.000000 chariot-sdk-1.3.2/chariotCore/res/icon.png
+-rw-rw-rw-   0        0        0      161 2023-06-15 02:44:12.000000 chariot-sdk-1.3.2/chariotCore/res/plugin.spec.yaml
+-rw-rw-rw-   0        0        0       99 2023-07-27 01:45:59.000000 chariot-sdk-1.3.2/chariotCore/res/requirements.txt
+-rw-rw-rw-   0        0        0    12874 2023-04-27 08:17:13.000000 chariot-sdk-1.3.2/chariotCore/tasks.py
+-rw-rw-rw-   0        0        0    29401 2023-07-19 03:52:06.000000 chariot-sdk-1.3.2/chariotCore/templates.py
+-rw-rw-rw-   0        0        0    40914 2023-07-27 01:49:15.000000 chariot-sdk-1.3.2/chariotCore/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:37:59.269571 chariot-sdk-1.3.2/chariot_sdk.egg-info/
+-rw-rw-rw-   0        0        0     6588 2023-07-27 03:37:59.000000 chariot-sdk-1.3.2/chariot_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      736 2023-07-27 03:37:59.000000 chariot-sdk-1.3.2/chariot_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:37:59.000000 chariot-sdk-1.3.2/chariot_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-27 03:37:59.000000 chariot-sdk-1.3.2/chariot_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2023-07-27 03:37:59.000000 chariot-sdk-1.3.2/chariot_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-27 03:37:59.000000 chariot-sdk-1.3.2/chariot_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 03:37:59.271569 chariot-sdk-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1236 2023-07-25 09:54:31.000000 chariot-sdk-1.3.2/setup.py
```

### Comparing `chariot-sdk-1.3.1/PKG-INFO` & `chariot-sdk-1.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: chariot-sdk
-Version: 1.3.1
-Summary: Chariot plugin maker
-Home-page: https://pypi.org/
-Author: chariot
-Author-email: chariot@example.com
-License: MIT
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-
 ## chariot-sdk
 
 ---
 
 ### 简介
 千乘插件生成器
 
@@ -20,14 +9,26 @@
 - python 3.8+
 
 ### 安装
 > pip install chariot-sdk
 
 ### 更新日志
 
+> 1.3.1 -> 1.3.2
+
+- 提高热编辑功能在启动有错误的动作时的兼容性
+- 修复热更新接口的参数验证bug
+- 修复动作API接口在传入特定参数时会卡死的问题
+- 修复Dockerfile中由于python官方镜像更新出现的问题
+- 添加异步动作功能和接口
+- 添加获取进程运行状态的接口
+- 为创建触发器和接收器添加子进程PID输出
+- requirements.txt添加psutil、chariot-sdk==1.3.2，SDK会在生成插件时自动
+- 初始化插件接口添加插件数据返回
+
 > 1.3.0 -> 1.3.1
 
 - 修改资产接收器的输出结构，现在资产的key值将决定前端展示的文本
 - 去除yaml文件中的multi_workers、hot_update参数，新增sdk参数用于记录开发插件用的SDK版本，以后千乘将根据sdk参数（版本）来判断插件支持的功能
 - 添加-r命令下测试资产接收器的功能
 - api接口现在会限制测试时接收器的数量为1，在启动下一个接收器时，上一个接收器会被自动关闭（也可以手动关闭接收器）
 - 提高了SDK对插件出现错误时的兼容，从而更好地防范热改动功能引发的SDK崩溃
@@ -87,8 +88,8 @@
 > 1.2.6 -> 1.2.7
 
 - 全新的日志记录系统，所有开发和运行时的警告、错误以及值得注意的信息都将以不同的颜色进行高亮显示，并且日志记录方法调用更加方便
 - 重构了SDK大部分功能的实现，极大地提高了可维护性和扩展性，大量重复的功能已重构为使用统一的函数处理
 - 优化SDK运行逻辑，业务错误将不再影响SDK的运行，但是会触发SDK的错误信息收集机制
 - 优化生成插件文件时的逻辑，一些文件在重写生成插件时不再会被覆盖
 - 优化了SDK对yaml文件的读取，SDK会对一些必要的数据进行审查，以减少开发阶段出现的bug
-- 可以通过命令自动生成一个yaml模板文件
+- 可以通过命令自动生成一个yaml模板文件
```

### Comparing `chariot-sdk-1.3.1/README.md` & `chariot-sdk-1.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: chariot-sdk
+Version: 1.3.2
+Summary: Chariot plugin maker
+Home-page: https://pypi.org/
+Author: chariot
+Author-email: chariot@example.com
+License: MIT
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+
 ## chariot-sdk
 
 ---
 
 ### 简介
 千乘插件生成器
 
@@ -9,14 +20,26 @@
 - python 3.8+
 
 ### 安装
 > pip install chariot-sdk
 
 ### 更新日志
 
+> 1.3.1 -> 1.3.2
+
+- 提高热编辑功能在启动有错误的动作时的兼容性
+- 修复热更新接口的参数验证bug
+- 修复动作API接口在传入特定参数时会卡死的问题
+- 修复Dockerfile中由于python官方镜像更新出现的问题
+- 添加异步动作功能和接口
+- 添加获取进程运行状态的接口
+- 为创建触发器和接收器添加子进程PID输出
+- requirements.txt添加psutil、chariot-sdk==1.3.2，SDK会在生成插件时自动
+- 初始化插件接口添加插件数据返回
+
 > 1.3.0 -> 1.3.1
 
 - 修改资产接收器的输出结构，现在资产的key值将决定前端展示的文本
 - 去除yaml文件中的multi_workers、hot_update参数，新增sdk参数用于记录开发插件用的SDK版本，以后千乘将根据sdk参数（版本）来判断插件支持的功能
 - 添加-r命令下测试资产接收器的功能
 - api接口现在会限制测试时接收器的数量为1，在启动下一个接收器时，上一个接收器会被自动关闭（也可以手动关闭接收器）
 - 提高了SDK对插件出现错误时的兼容，从而更好地防范热改动功能引发的SDK崩溃
@@ -76,8 +99,8 @@
 > 1.2.6 -> 1.2.7
 
 - 全新的日志记录系统，所有开发和运行时的警告、错误以及值得注意的信息都将以不同的颜色进行高亮显示，并且日志记录方法调用更加方便
 - 重构了SDK大部分功能的实现，极大地提高了可维护性和扩展性，大量重复的功能已重构为使用统一的函数处理
 - 优化SDK运行逻辑，业务错误将不再影响SDK的运行，但是会触发SDK的错误信息收集机制
 - 优化生成插件文件时的逻辑，一些文件在重写生成插件时不再会被覆盖
 - 优化了SDK对yaml文件的读取，SDK会对一些必要的数据进行审查，以减少开发阶段出现的bug
-- 可以通过命令自动生成一个yaml模板文件
+- 可以通过命令自动生成一个yaml模板文件
```

### Comparing `chariot-sdk-1.3.1/chariotCore/main.py` & `chariot-sdk-1.3.2/chariotCore/main.py`

 * *Files identical despite different names*

### Comparing `chariot-sdk-1.3.1/chariotCore/res/Dockerfile` & `chariot-sdk-1.3.2/chariotCore/res/Dockerfile`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 FROM python:3.11-slim
 
 WORKDIR /python/src
 ADD . /python/src
 RUN chmod +x /python/src/main.py
 
 # replace apt source && config pip source
-RUN sed -i "s@http://deb.debian.org@http://mirrors.aliyun.com@g" /etc/apt/sources.list && \
-  sed -i "s@http://security.debian.org@http://mirrors.aliyun.com@g" /etc/apt/sources.list && \
+RUN echo "deb http://mirrors.aliyun.com/debian $(cat /etc/os-release | grep -Po "(?<=VERSION_CODENAME=)(.+)") main" > /etc/apt/sources.list && \
+  echo "deb http://mirrors.aliyun.com/debian-security $(cat /etc/os-release | grep -Po "(?<=VERSION_CODENAME=)(.+)")-security main" >> /etc/apt/sources.list && \
   apt-get update && apt-get install -y iputils-ping net-tools vim && apt-get clean && \
   pip config set global.index-url https://mirrors.aliyun.com/pypi/simple && \
   /bin/echo -e [easy_install]\\nindex-url=https://mirrors.aliyun.com/pypi/simple > ~/.pydistutils.cfg
 
 # Install pip dependencies
 RUN if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
```

### Comparing `chariot-sdk-1.3.1/chariotCore/res/SDK/base.py` & `chariot-sdk-1.3.2/chariotCore/res/SDK/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         response = requests.post(dispatcher_url, json=data, verify=False)
 
         log("info", f"发送完成，状态码：{response.status_code}\n  返回信息：{response.text}")
 
         return response
 
 
-def save_update_pack(update_pack: bytes):
+def saveUpdatePack(update_pack: bytes):
     """
     #   将上传的更新包保存到插件根目录的update文件夹下
     参数说明：
     update_pack:bytes,  #   更新包
     """
 
     work_path = os.getcwd()
@@ -401,16 +401,14 @@
                     shutil.copy2(resource, file_path)
 
             log("info", "更新完成！")
 
     except Exception as error:
         error_trace = traceback.format_exc()
         log("error", "热更新执行失败，失败原因：\n  {}\n  详细信息：\n{}".format(error, error_trace))
-        log("attention", "将在5秒后重启服务")
-        time.sleep(5)
         return False
 
     return True
 
 
 def findLatestUpdate(update_packs_dir: str, update_packs: list):
     """
```

### Comparing `chariot-sdk-1.3.1/chariotCore/res/SDK/chariot.py` & `chariot-sdk-1.3.2/chariotCore/res/SDK/chariot.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,14 +84,43 @@
         #   缓存服务URL
         cache_url = data.get("dispatcher").get("cache_url")
         func._run(input_data, connection_data, dispatcher_url, cache_url)
 
     log("info", f"{_modules_dict[module]}（{module}）运行结束")
 
 
+def delayed(data: dict, plugin_object):
+    """
+    #   运行异步动作的整个流程
+    参数说明：
+    data:dict,      #   运行功能时的必要的数据
+    plugin_object:PLUGIN,      #   插件集合对象（类位于生成的插件后的根目录下main.py文件内）
+
+    """
+    log("info", "尝试获取数据中的 body")
+
+    #   必要的参数位于data内的body下
+    data_body = data.get("body")
+    if not data_body:
+        log("error", "body 为空")
+        return
+
+    func = plugin_object.actions[data_body["action"]]
+
+    #   run输入参数
+    input_data = data_body.get("input")
+    #   连接器参数
+    connection_data = data_body.get("connection")
+    #   转发地址
+    dispatcher_url = data_body.get("dispatcher").get("url")
+
+    func._runDelayed(input_data, connection_data, dispatcher_url, data_body.get("config"))
+
+    log("info", f"异步动作（delayed action）运行结束")
+
 def test(data: dict, plugin_object):
     """
     #   只运行连接器部分
     参数说明：
     data:dict,      #   运行功能时的必要的json数据
     plugin_object:PLUGIN,      #   插件集合对象（类位于生成的插件后的根目录下main.py文件内）
     """
```

### Comparing `chariot-sdk-1.3.1/chariotCore/res/SDK/cli.py` & `chariot-sdk-1.3.2/chariotCore/res/SDK/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,19 @@
         http(workers)
 
     elif sys.argv.count("test"):
         data = getData()
         log("info", "执行 test 命令")
         test(data, plugin_object)
 
+    elif sys.argv.count("delayed"):
+        data = getData()
+        log("info", "执行 delayed 命令")
+        delayed(data, plugin_object)
+
     else:
         log("error", "未知的命令，输入-h以获取帮助")
         return
 
 
 def getData() -> dict:
     """
```

### Comparing `chariot-sdk-1.3.1/chariotCore/res/SDK/models.py` & `chariot-sdk-1.3.2/chariotCore/res/SDK/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,36 +81,38 @@
 
 #   插件定义文件结构，用于初始化插件
 class PLUGIN_DATA_MODEL(BaseModel):
     plugin_spec_version: str = "v3"
     name: str
     version: str
     title: dict
-    sdk: str = "1.3.1"
-    description: dict = None
+    sdk: str = "1.3.2"
+    description: dict = {}
     vendor: str = "chariot"
     tags: List[str] = []
-    types: dict = None
-    connection: dict = None
-    actions: dict = None
-    triggers: dict = None
-    alarm_receivers: dict = None
-    indicator_receivers: dict = None
-    asset_receivers: dict = None
+    types: dict = {}
+    connection: dict = {}
+    actions: dict = {}
+    triggers: dict = {}
+    alarm_receivers: dict = {}
+    indicator_receivers: dict = {}
+    asset_receivers: dict = {}
 
 
 class FUNC_SET_MODEL(BaseModel):
     func_id: str
     func_code: str
 
 
 class CODE_DICT_MODEL(BaseModel):
-    actions: List[FUNC_SET_MODEL] = []
-    triggers: List[FUNC_SET_MODEL] = []
-    alarm_receivers: List[FUNC_SET_MODEL] = []
-    indicator_receivers: List[FUNC_SET_MODEL] = []
-    asset_receivers: List[FUNC_SET_MODEL] = []
+    actions: Optional[List[FUNC_SET_MODEL]] = []
+    triggers: Optional[List[FUNC_SET_MODEL]] = []
+    alarm_receivers: Optional[List[FUNC_SET_MODEL]] = []
+    indicator_receivers: Optional[List[FUNC_SET_MODEL]] = []
+    asset_receivers: Optional[List[FUNC_SET_MODEL]] = []
 
 
 class PLUGIN_CONSTRUCTION_MODEL(BaseModel):
     plugin_data: PLUGIN_DATA_MODEL
     plugin_code: CODE_DICT_MODEL
+
+
```

### Comparing `chariot-sdk-1.3.1/chariotCore/res/SDK/subassembly.py` & `chariot-sdk-1.3.2/chariotCore/res/SDK/subassembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,14 +124,89 @@
 
             #   构建错误输出的output
             log("info", "构建错误返回信息")
             output = self._buildOutput({}, False, error_trace)
 
         return output
 
+    def _runDelayed(self, input_data, connection_data, dispatcher_url, config_data: dict = None):
+        """
+        #   运行异步动作
+        参数说明：
+        input_data:dict,    #   入参数据
+        conection_data:dict,    #   连接数据
+        dispatcher_url:str,     #   数据转发URL
+        config_data:dict,   #   配置数据
+        """
+
+        log("info", "插件运行中")
+
+        self.dispatcher_url = dispatcher_url
+
+        if config_data:
+            log("info", "检查到有配置信息")
+            loadConfig(config_data)
+        else:
+            log("info", "未传入配置信息，使用默认配置")
+            loadConfig()
+
+            #   运行connection
+        output = self._test(connection_data)
+
+        #   连接器异常时直接返回错误输出
+        if output["body"]["status"] == "False":
+            return output
+
+        #   运行run
+        try:
+
+            log("debug", f"获取功能数据：\n  {input_data}")
+
+            #   校验入参数据
+            log("info", "校验入参数据")
+            input_data = checkModel(input_data, self.inputModel)
+
+            log("info", "执行功能中")
+
+            output_data = self.run(input_data)
+
+            log("info", "功能执行完成")
+
+            output_data = checkModel(output_data, self.outputModel)
+
+            #   构建output
+            log("info", "构建输出数据")
+            output = self._buildOutput(output_data, True)
+
+        except Exception as error:
+            #   收集错误信息
+            log("error", f"功能执行异常，错误原因：\n  {error}")
+
+            error_trace = traceback.format_exc()
+            log("error", f"详细错误信息：\n{error_trace}")
+
+            #   构建错误输出的output
+            log("info", "构建错误返回信息")
+            output = self._buildOutput({}, False, error_trace)
+
+        self.send(output, False)
+
+        return output
+
+    def send(self, data: dict = {}, needCheck: bool = True):
+        """
+        #   转发信息
+        参数说明：
+        data:dict,  #   需要转发的信息
+        needCheck:bool, #   是否需要对转发的信息进行出参验证
+        """
+        #   创建转发线程
+        thread1 = threading.Thread(target=transpondData, args=(data, needCheck, self.outputModel, self.dispatcher_url))
+        thread1.start()
+
     def _buildOutput(self, output_data: dict = {}, status: bool = True, error_trace: str = ""):
         """
         #   构建出参信息，包括日志信息
         参数说明：
         output_data:dict,   #   输出信息
         status:bool,    #   run执行状态，执行成功为True，不成功为False
         error_trace:str,  #   详细的错误信息，用于给开发人员看
```

### Comparing `chariot-sdk-1.3.1/chariotCore/res/SDK/web.py` & `chariot-sdk-1.3.2/chariotCore/res/SDK/web.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,32 +6,34 @@
 import typing
 import multiprocessing
 from . import VERSION
 from .models import *
 from .base import *
 from importlib import reload
 from signal import SIGINT
+import psutil
 
 ####
 #
 #   插件的API服务
 #   全局变量前面请加下划线，这些变量应该只被web.py内方法调用
 #   --预计在将来某一个版本中被另外一种方法替代-- (这行划去)
 #   计划总赶不上变化不是吗
 #
 ####
 
 _rest_server = FastAPI(title="千乘插件API接口", version=VERSION, description="")
 
 
 @_rest_server.post("/actions/{action_name}", tags=["动作"])
-async def actions(action_name, plugin_stdin: typing.Optional[ACTION_TEST_MODEL]):
+async def actions(action_name: str, plugin_stdin: typing.Optional[ACTION_TEST_MODEL]):
     """
     #   动作接口
     """
+
     clearLog(clear_size=1)
 
     action = loadModule(action_name, "actions")
 
     if not action:
         log("error", f"无法导入功能：{action_name}")
         content = {
@@ -54,14 +56,74 @@
 
     if output["body"]["status"] != "True":
         return JSONResponse(content=output, status_code=500)
     else:
         return output
 
 
+@_rest_server.post("/actions/{action_name}/delayed", tags=["动作"])
+async def actions_delayed(action_name: str, plugin_stdin: typing.Optional[ACTION_TEST_MODEL]):
+    """
+    #   异步动作接口
+    """
+    clearLog(clear_size=1)
+
+    data = plugin_stdin.dict()
+
+    try:
+
+        plugin_data = getPluginData()
+
+        if not plugin_data.get("actions", {}).get(action_name):
+            log("error", f"无法在动作下找到该功能：{action_name}")
+            content = {
+                "msg": f"无法在动作下找到该功能：{action_name}"
+            }
+            return JSONResponse(content=content, status_code=404)
+
+        process = multiprocessing.Process(target=actionProcess, args=(action_name, data))
+
+        process.start()
+
+    except Exception as error:
+
+        from .base import _log_data
+
+        log("error", f"{error}")
+
+        content = {
+            "version": "v1",
+            "type": data["type"],
+            "body": {
+                "status": "False",
+                "log": _log_data,
+                "error_trace": traceback.format_exc(),
+                "msg": f"异步动作创建失败"
+            }
+        }
+
+        return JSONResponse(content=content, status_code=500)
+
+    from .base import _log_data
+
+    content = {
+        "version": "v1",
+        "type": data["type"],
+        "body": {
+            "status": "True",
+            "log": _log_data,
+            "error_trace": "",
+            "msg": f"异步动作已创建完成",
+            "pid": str(process.pid)
+        }
+    }
+
+    return JSONResponse(content=content, status_code=201)
+
+
 @_rest_server.post("/actions/{action_name}/test", tags=["动作"])
 async def actions_test(action_name: str, plugin_stdin: typing.Optional[ACTION_TEST_MODEL]):
     """
     #   动作连接器测试接口
     """
     return rest_test("actions", action_name, plugin_stdin)
 
@@ -162,18 +224,18 @@
         }
         return JSONResponse(content=content, status_code=404)
 
 
 @_rest_server.post("/update_plugin", tags=["插件热更新"])
 async def update_plugin(update_pack: bytes = File()):
     """
-    #   上传更新包
+    #   上传插件在线包
     """
     try:
-        save_update_pack(update_pack)
+        saveUpdatePack(update_pack)
         update_result = hotUpdate("http")
         clearUpdateFile()
         if update_result:
             return {
                 "msg": "更新完成"
             }
         else:
@@ -246,17 +308,63 @@
         }
         return JSONResponse(content=content, status_code=400)
 
     try:
         for func_path, func_code in dir_and_code:
             with open(func_path, "w", encoding="utf-8") as file:
                 file.write(func_code)
+
+        #   返回生成完成的代码
+        modules_dir = ["actions", "triggers", "alarm_receivers", "indicator_receivers", "asset_receivers"]
+
+        modules_dict = {}
+
+        try:
+
+            for temp_module in modules_dir:
+
+                modules_dict[temp_module] = []
+
+                modules_dir_path = os.path.join(work_path, temp_module)
+
+                if not os.path.exists(modules_dir_path):
+                    continue
+
+                module_files = os.listdir(modules_dir_path)
+
+                ignore_files = ["models.py", "__init__.py", "__pycache__"]
+
+                for ignore_file in ignore_files:
+                    if ignore_file in module_files:
+                        module_files.pop(module_files.index(ignore_file))
+
+                for module_file in module_files:
+                    module_file_path = os.path.join(modules_dir_path, module_file)
+
+                    with open(module_file_path, "r", encoding="utf-8") as module_file_code:
+                        modules_dict[temp_module].append({
+                            "func_id": module_file.replace(".py", ""),
+                            "func_code": module_file_code.read()
+                        })
+        except Exception as error:
+            content = {
+                "msg": f"功能代码读取失败 - {error}"
+            }
+            return JSONResponse(content=content, status_code=500)
+
+        plugin_data = getPluginData()
+
         return {
-            "msg": "插件生成完成"
+            "msg": "插件生成完成",
+            "editor": {
+                "plugin_data": plugin_data,
+                "plugin_code": modules_dict
+            }
         }
+
     except Exception as error:
         content = {
             "msg": f"代码写入失败 - {error}"
         }
         return JSONResponse(content=content, status_code=500)
 
 
@@ -314,14 +422,33 @@
 
     return {
         "plugin_data": plugin_data,
         "plugin_code": modules_dict
     }
 
 
+@_rest_server.get("/pid", tags=["PID查询"])
+async def pid(pid: str):
+    """
+    #   获取PID状态
+    """
+
+    try:
+        return {
+            "pid": pid,
+            #   status: “running”, “paused”, “start_pending”, “pause_pending”, “continue_pending”, “stop_pending” or “stopped” "Not Found"
+            "status": psutil.Process(int(pid)).status()
+        }
+    except:
+        return {
+            "pid": pid,
+            "status": "Not Found"
+        }
+
+
 @_rest_server.get("/sdk_version", tags=["插件信息"])
 async def sdk_version():
     """
     #   获取SDK版本
     """
     return {
         "sdk_version": VERSION
@@ -378,15 +505,16 @@
     如果无法找到方法或组件则返回None
     """
 
     if module == "actions":
         #   在生成插件之后有actions就能成功import了
         try:
             import actions
-            #   先初始化并释放一次功能类，以清空缓存
+            #   先初始化并释放一次功能类，以清空缓存（甚至是错误的缓存）
+            actions.modules_dict()
             actions.modules_dict()[func_id]()
             #   清空完再reload
             reload(actions)
             return actions.modules_dict()[func_id]()
         except:
             log("error", traceback.format_exc())
 
@@ -422,30 +550,30 @@
     return None
 
 
 def rest_test(module, func_id, plugin_stdin):
     """
     #   通用的连接器测试方法
     参数说明：
-    module:str,         #   组件，module = action,trigger,alarm_receiver,indicator_receiver,asset_receiver
+    module:str,         #   组件，module = actions,triggers,alarm_receivers,indicator_receivers,asset_receivers
     func_id:str,  #   方法id
     plugin_stdin:str,   #   接口传入数据
 
     因为测试连接器流程一样
     所有使用一个通用方法进行维护
     """
 
     clearLog(clear_size=1)
 
     func = loadModule(func_id, module)
 
     if not func:
         log("error", f"无法导入功能：{func_id}")
         content = {
-            "msg": "无法导入功能：{func_id}"
+            "msg": f"无法导入功能：{func_id}"
         }
         return JSONResponse(content=content, status_code=400)
 
     #   取出body
     data = plugin_stdin.dict()
     data_body = data.get("body")
 
@@ -466,15 +594,15 @@
         return output
 
 
 def createReceivers(module, receiver_name, plugin_stdin):
     """
     #   通用接收器方法
     参数说明：
-    module:str,         #   组件，module = trigger,alarm_receiver,indicator_receiver,asset_receiver
+    module:str,         #   组件，module = triggers,alarm_receivers,indicator_receivers,asset_receivers
     receiver_name:str,  #   接收器名称
     plugin_stdin:str,   #   接口传入数据
 
     因为触发器、告警接收器、情报接收器、资产接收器代码重复率极高（或者可以说一模一样的），
     因此使用一个通用方法进行维护
     """
 
@@ -541,28 +669,29 @@
     content = {
         "version": "v1",
         "type": data["type"],
         "body": {
             "status": "True",
             "log": _log_data,
             "error_trace": "",
-            "msg": f"{module_dict[module]}已创建完成"
+            "msg": f"{module_dict[module]}已创建完成",
+            "pid": str(process.pid)
         }
     }
 
     return JSONResponse(content=content, status_code=201)
 
 
 def receiverProcess(module, receiver_name, data):
     """
     #   此方法用于创建各类接收器进程
     参数说明：
-    module:str,         #   组件，module = trigger,alarm_receiver,indicator_receiver,asset_receiver
+    module:str,         #   组件，module = triggers,alarm_receivers,indicator_receivers,asset_receivers
     receiver_name:str,  #   接收器名称
-    data:dict,  #   接收的数据
+    data:dict,  #   运行数据
     """
 
     receiver = loadModule(receiver_name, module)
     if not receiver:
         log("error", f"无法导入功能：{receiver_name}")
         content = {
             "msg": f"无法导入功能：{receiver_name}"
@@ -579,14 +708,42 @@
     dispatcher_url = data_body.get("dispatcher").get("url")
     #   缓存地址
     cache_url = data_body.get("dispatcher").get("cache_url")
 
     receiver._run(input_data, connection_data, dispatcher_url, cache_url, data_body.get("config"))
 
 
+def actionProcess(action_name, data):
+    """
+    #   此方法用于创建异步动作进程
+    参数说明：
+    action_name:str,  #   动作名称
+    data:dict,  #   运行数据
+    """
+    action = loadModule(action_name, "actions")
+
+    if not action:
+        log("error", f"无法导入功能：{action_name}")
+        content = {
+            "msg": f"无法导入功能：{action_name}"
+        }
+        return JSONResponse(content=content, status_code=400)
+
+    #   data中的body部分
+    data_body = data.get("body")
+    #   run输入参数
+    input_data = data_body.get("input")
+    #   连接器参数
+    connection_data = data_body.get("connection")
+    #   转发地址
+    dispatcher_url = data_body.get("dispatcher").get("url")
+
+    action._runDelayed(input_data, connection_data, dispatcher_url, data_body.get("config"))
+
+
 def runserver(workers):
     """
     #   启动api服务
     参数说明：
     workers:int,    #   工作进程数量
     """
     log("attention", "在浏览器内输入 http://127.0.0.1:10001/docs 以进行接口测试")
```

### Comparing `chariot-sdk-1.3.1/chariotCore/res/config.ini` & `chariot-sdk-1.3.2/chariotCore/res/config.ini`

 * *Files identical despite different names*

### Comparing `chariot-sdk-1.3.1/chariotCore/res/icon.png` & `chariot-sdk-1.3.2/chariotCore/res/icon.png`

 * *Files identical despite different names*

### Comparing `chariot-sdk-1.3.1/chariotCore/tasks.py` & `chariot-sdk-1.3.2/chariotCore/tasks.py`

 * *Files identical despite different names*

### Comparing `chariot-sdk-1.3.1/chariotCore/templates.py` & `chariot-sdk-1.3.2/chariotCore/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,20 +608,22 @@
 reload(models)
 
 {% for name, className in init_list %}
 try:
     from .{{ name }} import {{ className }}
 except:
     log("error",traceback.format_exc())
+    {{ className }} = None
 {% endfor %}
 
 def modules_dict():
 
     reload(sys.modules[__name__])
-    {% for name, className in init_list %}reload({{ name }})
+    {% for name, className in init_list %}
+    reload({{ name }})
     {% endfor %}
     return {
         {% for name, className in init_list %}"{{ name }}": {{ className }},
         {% endfor %}
     }
 """
```

### Comparing `chariot-sdk-1.3.1/chariotCore/tools.py` & `chariot-sdk-1.3.2/chariotCore/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 ####
 #
 #   此文件用于存放task.py中所使用的各种方法
 #
 ####
 
 #   需要添加新的预设类型时，请修改typesDict
-types_dict = {
+_types_dict = {
     "string": "str",
     "bytes": "str",
     "boolean": "bool",
     "float": "float",
     "date": "str",
     "object": "dict",
     "password": "str",
     "integer": "int",
+    #   file的类型是一个包含filename和content的字典，filename为文件名称，content则为文件数据的base64格式
     "file": "dict",
-    #   file的类型是一个包含filename和content的字典
     "any": "Any"
 }
 
-module_dict = {
+_module_dict = {
     "actions": "动作",
     "triggers": "触发器",
     "indicator_receivers": "情报接收器",
     "alarm_receivers": "告警接收器",
     "asset_receivers": "资产接收器"
 }
 
@@ -332,15 +332,15 @@
     types_model:str,    #   自定义类型校验数据
     connection_model:str,   #   连接器校验数据
     connection_keys:list of str,    #   连接器参数列表
     """
     module_data = data.get(module)
 
     if not module_data:
-        log("attention", f"未检测到{module_dict[module]}，跳过{module_dict[module]}的生成")
+        log("attention", f"未检测到{_module_dict[module]}，跳过{_module_dict[module]}的生成")
         return []
 
     #   生成校验数据和校验文件
     generateModel(module, module_data, types_model, connection_model)
 
     modules_list = generateModuleFile(os.getcwd(), module, module_data, connection_keys)
 
@@ -379,15 +379,15 @@
     参数说明：
     module:str,     #   组件，module = actions, triggers, indicator_receivers, alarm_receivers, asset_receivers
     module_data:dict,    #   插件定义文件中组件的参数
 
     返回需要在models.py文件中写入的动作的入参和出参校验数据
     """
 
-    log("info", f"生成 {module_dict[module]}（{module}）校验数据中")
+    log("info", f"生成 {_module_dict[module]}（{module}）校验数据中")
 
     model = ""
 
     for module_key, key_params in module_data.items():
         log("info", f"生成 {module_key} 校验数据中")
 
         #   获取输入与输出载荷
@@ -423,15 +423,15 @@
             "asset_receivers": asset_receivers_model_template
         }
 
         model += renderStrTemplate(output_data, model_template_dict.get(module, model_template))
 
         log("info", f"{module_key} 校验数据生成完成")
 
-    log("info", f"{module_dict[module]}（{module}）校验数据生成完成")
+    log("info", f"{_module_dict[module]}（{module}）校验数据生成完成")
 
     return model
 
 
 def generateModelFile(work_path: str, model_module: str, model_data: str):
     """
     #   根据目录及校验数据生成校验文件models.py
@@ -478,15 +478,15 @@
 
     #   用于记录要在初始化文件（__init__.py）中写入的功能导入（import）
     init_list = []
 
     #   组件文件夹路径
     module_path = os.path.join(work_path, module)
 
-    log("info", f"生成 {module_dict[module]}（{module}）所有功能中")
+    log("info", f"生成 {_module_dict[module]}（{module}）所有功能中")
 
     #   遍历组件内每一个功能和功能的参数
     for func_id, params in module_data.items():
         try:
 
             log("info", rf"生成 {module}\{func_id}.py 文件中")
 
@@ -511,15 +511,15 @@
 
         #   生成测试用的json文件
         generateTestFile(func_data, module_test_template_dict[module])
 
     #   生成插件功能初始化文件
     generateInitFile(module, module_path, init_list)
 
-    log("info", f"{module_dict[module]}（{module}）所有功能生成完成")
+    log("info", f"{_module_dict[module]}（{module}）所有功能生成完成")
 
     #   功能类名称列表 func_class_name_list，用于生成入口文件 main.py
     func_class_name_list = [func[1] for func in init_list]
 
     return func_class_name_list
 
 
@@ -723,26 +723,32 @@
                                 log("attention", "兼容性更新完成")
 
                             #   1.2.8对清除空参数的方法进行了重写，并且更改为全局可用
 
                             if data.find("self._popEmpty") != -1:
                                 data = data.replace("self._popEmpty", "popEmpty")
 
-                        with open(file_path, "w", encoding="utf-8") as f:
+                        with open(file_path, "w", encoding="utf-8", newline="\n") as f:
                             f.write(data)
             else:
                 pass
 
         requirements_path = os.path.join(work_path, "requirements.txt")
         if os.path.exists(requirements_path):
             with open(requirements_path, "r", encoding="utf-8") as f:
                 data = f.read()
             if data.find("python-multipart") == -1:
                 with open(requirements_path, "a", encoding="utf-8") as f:
                     f.write("\npython-multipart\n")
+            if data.find("chariot-sdk") == -1:
+                with open(requirements_path, "a", encoding="utf-8") as f:
+                    f.write("\nchariot-sdk==1.3.2\n")
+            if data.find("psutil") == -1:
+                with open(requirements_path, "a", encoding="utf-8") as f:
+                    f.write("\npsutil\n")
 
         config_path = os.path.join(work_path, "config.ini")
         if os.path.exists(config_path):
             with open(config_path, "r", encoding="utf-8") as f:
                 data = f.read()
             if "[ignore]" not in data:
                 data += "\n[ignore]\n#   打包时忽略的根目录下的文件\n#   以逗号分隔多个文件（文件夹）\nignore = env,venv,tests,.git,.vs,.gitignore,.idea,__sdkcache__,__pycache__,temp_image.tar.gz,temp_plugin.tar.gz"
@@ -920,18 +926,18 @@
     value_enum,     #   构成参数的枚举集合
 
     #   检验不通过时抛出异常
     """
     if not value_type and not value_enum:
         raise Exception(f"类型与枚举集合都为空\n类型（type）与枚举集合（enum）请至少填写一项")
 
-    if value_type and not types_dict.get(value_type):
-        if value_type.startswith("[]") and not types_dict.get(value_type[2:]):
+    if value_type and not _types_dict.get(value_type):
+        if value_type.startswith("[]") and not _types_dict.get(value_type[2:]):
             log("attention", f"未知类型的列表组合：{value_type}，如果是自定义类型请忽略此信息")
-        elif not value_type.startswith("[]") and not types_dict.get(value_type[2:]):
+        elif not value_type.startswith("[]") and not _types_dict.get(value_type[2:]):
             log("attention", f"未知的类型：{value_type}，如果是自定义类型请忽略此信息")
 
     if value_enum and not isinstance(value_enum, list):
         raise Exception("枚举集合（enum）填写不符合规范")
 
     if value_default and value_enum and value_default not in value_enum:
         raise Exception(f"默认值 {value_default}\n无法在枚举的集合中找到")
@@ -959,27 +965,27 @@
     """
     #   存在枚举集合时
     if value_enum:
         argType = f"Literal{value_enum}"
 
     #   非枚举集合时，尝试从typeDict中获取预设类
     else:
-        argType = types_dict.get(value_type)
+        argType = _types_dict.get(value_type)
 
     #   无法直接获取到预设类
     if not argType:
 
         #   是否为列表
         if value_type.startswith("[]"):
 
             #   查看是否为预设类的列表形式
             #   Optional，意为此参数可以为None或已经声明的类型
-            if types_dict.get(value_type[2:]):
+            if _types_dict.get(value_type[2:]):
                 #   预设类的列表形式将直接取预设类型的 列表 形式
-                argType = f"Optional[List[{types_dict.get(value_type[2:])}]]"
+                argType = f"Optional[List[{_types_dict.get(value_type[2:])}]]"
             else:
                 #   非预设类的列表形式将取自定义类型的全大写的 列表 形式
                 argType = f"Optional[List[{value_type[2:].upper()}]]"
 
         else:
             #   非预设类直接采用自定义类型的全大写形式
             argType = value_type.upper()
@@ -1055,15 +1061,14 @@
 
     #   builds文件夹用于放置构建好的包
     builds_dir_path = os.path.join(work_path, "builds")
 
     if not os.path.exists(builds_dir_path) or not os.path.isdir(builds_dir_path):
         os.mkdir(builds_dir_path)
 
-
     #   在线包文件名
     #   当传入在线包名称时，一般是要创建临时在线包
     if pack_name:
         tar_name = pack_name
     #   当打包在线包时，需要创建临时插件结构文件
     else:
         tar_name = f"{vendor}-{name}-{version}.tar.gz"
@@ -1176,12 +1181,12 @@
                 module_files.pop(module_files.index(ignore_file))
 
         for module_file in module_files:
             module_file_path = os.path.join(modules_dir_path, module_file)
 
             with open(module_file_path, "r", encoding="utf-8") as module_file_code:
                 modules_dict[temp_module].append({
-                    "func_name": module_file.replace(".py", ""),
+                    "func_id": module_file.replace(".py", ""),
                     "func_code": module_file_code.read()
                 })
 
     return modules_dict
```

### Comparing `chariot-sdk-1.3.1/chariot_sdk.egg-info/PKG-INFO` & `chariot-sdk-1.3.2/chariot_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chariot-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: Chariot plugin maker
 Home-page: https://pypi.org/
 Author: chariot
 Author-email: chariot@example.com
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -20,14 +20,26 @@
 - python 3.8+
 
 ### 安装
 > pip install chariot-sdk
 
 ### 更新日志
 
+> 1.3.1 -> 1.3.2
+
+- 提高热编辑功能在启动有错误的动作时的兼容性
+- 修复热更新接口的参数验证bug
+- 修复动作API接口在传入特定参数时会卡死的问题
+- 修复Dockerfile中由于python官方镜像更新出现的问题
+- 添加异步动作功能和接口
+- 添加获取进程运行状态的接口
+- 为创建触发器和接收器添加子进程PID输出
+- requirements.txt添加psutil、chariot-sdk==1.3.2，SDK会在生成插件时自动
+- 初始化插件接口添加插件数据返回
+
 > 1.3.0 -> 1.3.1
 
 - 修改资产接收器的输出结构，现在资产的key值将决定前端展示的文本
 - 去除yaml文件中的multi_workers、hot_update参数，新增sdk参数用于记录开发插件用的SDK版本，以后千乘将根据sdk参数（版本）来判断插件支持的功能
 - 添加-r命令下测试资产接收器的功能
 - api接口现在会限制测试时接收器的数量为1，在启动下一个接收器时，上一个接收器会被自动关闭（也可以手动关闭接收器）
 - 提高了SDK对插件出现错误时的兼容，从而更好地防范热改动功能引发的SDK崩溃
```

### Comparing `chariot-sdk-1.3.1/chariot_sdk.egg-info/SOURCES.txt` & `chariot-sdk-1.3.2/chariot_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

