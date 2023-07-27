# Comparing `tmp/hust_login-1.0.2.tar.gz` & `tmp/hust_login-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hust_login-1.0.2.tar", last modified: Wed Jul 26 03:41:11 2023, max compression
+gzip compressed data, was "hust_login-1.0.3.tar", last modified: Thu Jul 27 06:15:14 2023, max compression
```

## Comparing `hust_login-1.0.2.tar` & `hust_login-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:41:11.271213 hust_login-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:41:11.263213 hust_login-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:41:11.267213 hust_login-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-26 03:40:56.000000 hust_login-1.0.2/.github/workflows/auto-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-26 03:40:56.000000 hust_login-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 03:40:56.000000 hust_login-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 03:40:56.000000 hust_login-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:40:56.000000 hust_login-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-26 03:41:11.271213 hust_login-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-26 03:40:56.000000 hust_login-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-26 03:40:56.000000 hust_login-1.0.2/README_ZH.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:41:11.267213 hust_login-1.0.2/hust_login/
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-26 03:40:56.000000 hust_login-1.0.2/hust_login/_HustPass.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-26 03:40:56.000000 hust_login-1.0.2/hust_login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-26 03:40:56.000000 hust_login-1.0.2/hust_login/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-26 03:40:56.000000 hust_login-1.0.2/hust_login/autotest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-26 03:40:56.000000 hust_login-1.0.2/hust_login/curriculum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-26 03:40:56.000000 hust_login-1.0.2/hust_login/decaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-26 03:40:56.000000 hust_login-1.0.2/hust_login/ecard_bills.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-26 03:40:56.000000 hust_login-1.0.2/hust_login/free_room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-26 03:40:56.000000 hust_login-1.0.2/hust_login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-26 03:40:56.000000 hust_login-1.0.2/hust_login/utility_bills.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:41:11.267213 hust_login-1.0.2/hust_login.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-26 03:41:11.000000 hust_login-1.0.2/hust_login.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-26 03:41:11.000000 hust_login-1.0.2/hust_login.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 03:41:11.000000 hust_login-1.0.2/hust_login.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-26 03:41:11.000000 hust_login-1.0.2/hust_login.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 03:41:11.000000 hust_login-1.0.2/hust_login.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:41:11.271213 hust_login-1.0.2/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-26 03:40:56.000000 hust_login-1.0.2/images/captcha_code.gif
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-26 03:40:56.000000 hust_login-1.0.2/images/captcha_code_processed.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-26 03:40:56.000000 hust_login-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 03:41:11.271213 hust_login-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-26 03:40:56.000000 hust_login-1.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-26 03:40:56.000000 hust_login-1.0.2/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:15:14.094454 hust_login-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:15:14.086454 hust_login-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:15:14.090454 hust_login-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-27 06:15:02.000000 hust_login-1.0.3/.github/workflows/auto-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-27 06:15:02.000000 hust_login-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 06:15:02.000000 hust_login-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 06:15:02.000000 hust_login-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 06:15:02.000000 hust_login-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-27 06:15:14.094454 hust_login-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-27 06:15:02.000000 hust_login-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-27 06:15:02.000000 hust_login-1.0.3/README_ZH.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:15:14.094454 hust_login-1.0.3/hust_login/
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-27 06:15:02.000000 hust_login-1.0.3/hust_login/_HustPass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-27 06:15:02.000000 hust_login-1.0.3/hust_login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-27 06:15:02.000000 hust_login-1.0.3/hust_login/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-27 06:15:02.000000 hust_login-1.0.3/hust_login/autotest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-27 06:15:02.000000 hust_login-1.0.3/hust_login/curriculum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-27 06:15:02.000000 hust_login-1.0.3/hust_login/decaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-07-27 06:15:02.000000 hust_login-1.0.3/hust_login/ecard_bills.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-27 06:15:02.000000 hust_login-1.0.3/hust_login/free_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-27 06:15:02.000000 hust_login-1.0.3/hust_login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-27 06:15:02.000000 hust_login-1.0.3/hust_login/utility_bills.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:15:14.094454 hust_login-1.0.3/hust_login.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-27 06:15:14.000000 hust_login-1.0.3/hust_login.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-27 06:15:14.000000 hust_login-1.0.3/hust_login.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 06:15:14.000000 hust_login-1.0.3/hust_login.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 06:15:14.000000 hust_login-1.0.3/hust_login.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 06:15:14.000000 hust_login-1.0.3/hust_login.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:15:14.094454 hust_login-1.0.3/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-27 06:15:02.000000 hust_login-1.0.3/images/captcha_code.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-27 06:15:02.000000 hust_login-1.0.3/images/captcha_code_processed.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 06:15:02.000000 hust_login-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 06:15:14.094454 hust_login-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-27 06:15:02.000000 hust_login-1.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-27 06:15:02.000000 hust_login-1.0.3/test_basic.py
```

### Comparing `hust_login-1.0.2/.github/workflows/auto-test.yml` & `hust_login-1.0.3/.github/workflows/auto-test.yml`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/.github/workflows/ci.yml` & `hust_login-1.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/LICENSE` & `hust_login-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/PKG-INFO` & `hust_login-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hust_login
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python-lib for authenticating HustPass@2023
 Home-page: https://github.com/MarvinTerry/HustLogin
 Author: MarvinTerry
 Author-email: marvinterry2004@gmail.com
 Maintainer: Jackhr
 Maintainer-email: jj2460596@gmail.com
 License: MIT
```

### Comparing `hust_login-1.0.2/README.md` & `hust_login-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/README_ZH.md` & `hust_login-1.0.3/README_ZH.md`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/hust_login/_HustPass.py` & `hust_login-1.0.3/hust_login/_HustPass.py`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/hust_login/__main__.py` & `hust_login-1.0.3/hust_login/__main__.py`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/hust_login/autotest.py` & `hust_login-1.0.3/hust_login/autotest.py`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/hust_login/curriculum.py` & `hust_login-1.0.3/hust_login/curriculum.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,20 @@
     week = weeks_from(start_date_semester, date_query)
     return _GetOneDay(session, date_query, week)
     
 def _GetOneDay(session:requests.Session, date_query:str, week:int) -> tuple[list[dict], dict]:
     resp_api = session.get('http://hub.m.hust.edu.cn/kcb/todate/JsonCourse.action?sj={}&zc={}'.format(date_query, week))
     content=json.loads(resp_api.text)
     class_list = []
-    ret = {'Date':date_query} 
+    ret = {'date':date_query} 
     for item in content:
         if item['kc'][0]['JSMC']=='—':
             continue
-        class_list.append({'No':item['jcx'],'ClassName':item['kc'][0]['KCMC'],'TeacherName':item['kc'][0]['XM'],'Place':item['kc'][0]['JSMC']})
-    ret['Curriculum'] = class_list
+        class_list.append({'No':item['jcx'],'course':item['kc'][0]['KCMC'],'teacher':item['kc'][0]['XM'],'place':item['kc'][0]['JSMC']})
+    ret['curriculum'] = class_list
     return ret
 
 def GetCurriculum(session:requests.Session, _date_query:str|list[str]|int|tuple[str,str]) -> list:
     '''
     PARAMETERS:\n
     session -- should be already logged in\n
     date    -- str  : the day you want, in form of YYYY-MM-DD\n
```

### Comparing `hust_login-1.0.2/hust_login/decaptcha.py` & `hust_login-1.0.3/hust_login/decaptcha.py`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/hust_login/ecard_bills.py` & `hust_login-1.0.3/hust_login/ecard_bills.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,20 +79,25 @@
         url = '{}?account={}&curpage={}&dateStatus={}&typeStatus=1'.format(url_base,account,current_page,_QueryMonth)    
         resp = session.get(url).text
         # print(resp.strip().strip('callJson(').strip(')'))
         raw = json.loads(resp.strip().strip('callJson(').strip(')'))
         next_page_obt = str(raw['nextpage'])
         entrys = raw['total']
         ret.extend(entrys)
-    selected_col = ['mercname','sign_tranamt','cardbal','occtime']
-    ret = [{column:entry[column] for column in selected_col} for entry in ret]
+    selected_col = {
+        'name'    :'mercname',
+        'money' :'sign_tranamt',
+        'balance' :'cardbal',
+        'time'    :'occtime'
+    }
+    ret = [{column_new:entry[column_old] for column_new,column_old in selected_col.items()} for entry in ret]
     for entry in ret:
-        for col in ['sign_tranamt','cardbal']:
+        for col in ['money','balance']:
             entry[col] = float(entry[col])/100
-        entry['occtime'] = raw_to_iso_format(entry['occtime'])
+        entry['time'] = raw_to_iso_format(entry['time'])
     return ret
 
 def GetEcardBills(session:requests.Session, _QueryDate:str|list[str]|tuple[str,str]) -> dict:
     '''
     PARAMETERS:\n
     session     -- should be already logged in\n
     Uid         -- str  : your student uid\n
```

### Comparing `hust_login-1.0.2/hust_login/free_room.py` & `hust_login-1.0.3/hust_login/free_room.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,18 +31,18 @@
     }
     
     # 必要的跳转步骤
     session.get('http://mhub.hust.edu.cn/cas/login?redirectUrl=/kxjsController/selectFreeRoom')
 
     raw_data = []
     # 建立数据结构(AI写的，蛮炫酷)
-    ret = {'Date':date_query,'Buildings':{buiding_name: [{'No': str(i), 'Roomlist': []} for i in range(1,13)] for buiding_name,buiding_id in buildings.items()}}
+    ret = {'date':date_query,'buildings':{buiding_name: [{'No': str(i), 'roomlist': []} for i in range(1,13)] for buiding_name,buiding_id in buildings.items()}}
 
     for buiding_name,buiding_id in buildings.items():
         # 爬取每个教学楼数据
         resp = session.get('http://mhub.hust.edu.cn/kxjsController/selectFreeRoom?sj={}&jxlbh={}'.format(date_query,buiding_id))
         raw_data.extend(json.loads(resp.text)['dataList'])
     
     for item in raw_data:
-        ret['Buildings'][item['JXLMC']][item['JC']-1]['Roomlist'].append(item['JSMC'].strip('教室'))
+        ret['buildings'][item['JXLMC']][item['JC']-1]['roomlist'].append(item['JSMC'].strip('教室'))
 
     return ret
```

### Comparing `hust_login-1.0.2/hust_login/login.py` & `hust_login-1.0.3/hust_login/login.py`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/hust_login/utility_bills.py` & `hust_login-1.0.3/hust_login/utility_bills.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,23 +83,23 @@
     ret = []
     if isinstance(Query_list, list):
         for item in Query_list:
             ret.append(_GetOneDay(session, MeterID, item, item)[0])
     elif isinstance(Query_list, tuple):
         ret = _GetOneDay(session, MeterID, Query_list[0], Query_list[1])
 
-    return {'RoomName':ret_Name, 'RemainPower':ret_remainPower, 'DayCosts':ret}
+    return {'room':ret_Name, 'remain_power':ret_remainPower, 'daily_cost':ret}
 
 def _GetOneDay(session:requests.Session, MeterID:str, S_Date:str, E_Date:str) -> list[dict]:
     payload3 = session.get(
         'http://sdhq.hust.edu.cn/icbs/PurchaseWebService.asmx/getMeterDayValue?AmMeter_ID={}&startDate={}&endDate={}'.format(MeterID, S_Date, E_Date)).text
     if re.search('<msg>成功</msg>', payload3) is None:
         raise
     ret_daycost = []
     for _item in re.finditer('<DayValueInfo>(.*?)</DayValueInfo>', payload3, re.S): # 解决匹配错误 *?表示最小匹配(non-greedy quantifier)
         item = _item.group(1)
         elc_cost = re.search('<dayValue>(.*)</dayValue>', item).group(1)
         cost_unit = re.search('<dw>(.*)</dw>', item).group(1)
         money = re.search('<dayUseMeony>(.*)</dayUseMeony>',item).group(1)
         date = re.search('<curDayTime>(.*)</curDayTime>', item).group(1)
-        ret_daycost.append({'date':date,'daycost':elc_cost+cost_unit,'money':money}) # 调换日期、电费顺序，更加合理
+        ret_daycost.append({'date':date,'cost':elc_cost+cost_unit,'money':money}) # 调换日期、电费顺序，更加合理
     return ret_daycost
```

### Comparing `hust_login-1.0.2/hust_login.egg-info/PKG-INFO` & `hust_login-1.0.3/hust_login.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hust-login
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python-lib for authenticating HustPass@2023
 Home-page: https://github.com/MarvinTerry/HustLogin
 Author: MarvinTerry
 Author-email: marvinterry2004@gmail.com
 Maintainer: Jackhr
 Maintainer-email: jj2460596@gmail.com
 License: MIT
```

### Comparing `hust_login-1.0.2/hust_login.egg-info/SOURCES.txt` & `hust_login-1.0.3/hust_login.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/images/captcha_code.gif` & `hust_login-1.0.3/images/captcha_code.gif`

 * *Files identical despite different names*

### Comparing `hust_login-1.0.2/setup.py` & `hust_login-1.0.3/setup.py`

 * *Files identical despite different names*

