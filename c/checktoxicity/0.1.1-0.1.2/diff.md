# Comparing `tmp/checktoxicity-0.1.1.tar.gz` & `tmp/checktoxicity-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checktoxicity-0.1.1.tar", last modified: Fri Jul 21 13:25:08 2023, max compression
+gzip compressed data, was "checktoxicity-0.1.2.tar", last modified: Thu Jul 27 08:54:38 2023, max compression
```

## Comparing `checktoxicity-0.1.1.tar` & `checktoxicity-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 13:25:08.577561 checktoxicity-0.1.1/
--rw-rw-rw-   0        0        0        0 2023-07-21 12:15:50.000000 checktoxicity-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      224 2023-07-21 13:25:08.576050 checktoxicity-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 13:25:08.566235 checktoxicity-0.1.1/checktoxicity.egg-info/
--rw-rw-rw-   0        0        0      224 2023-07-21 13:25:08.000000 checktoxicity-0.1.1/checktoxicity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-07-21 13:25:08.000000 checktoxicity-0.1.1/checktoxicity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 13:25:08.000000 checktoxicity-0.1.1/checktoxicity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 13:25:08.000000 checktoxicity-0.1.1/checktoxicity.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-21 13:25:08.000000 checktoxicity-0.1.1/checktoxicity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 13:25:08.578578 checktoxicity-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      354 2023-07-21 13:24:47.000000 checktoxicity-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:25:08.572060 checktoxicity-0.1.1/toxic/
--rw-rw-rw-   0        0        0        0 2023-07-21 10:38:11.000000 checktoxicity-0.1.1/toxic/__init__.py
--rw-rw-rw-   0        0        0     1301 2023-07-21 13:18:10.000000 checktoxicity-0.1.1/toxic/toxic.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:54:38.095395 checktoxicity-0.1.2/
+-rw-rw-rw-   0        0        0        0 2023-07-21 12:15:50.000000 checktoxicity-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      224 2023-07-27 08:54:38.093387 checktoxicity-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 08:54:38.086389 checktoxicity-0.1.2/checktoxicity.egg-info/
+-rw-rw-rw-   0        0        0      224 2023-07-27 08:54:37.000000 checktoxicity-0.1.2/checktoxicity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-07-27 08:54:37.000000 checktoxicity-0.1.2/checktoxicity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 08:54:37.000000 checktoxicity-0.1.2/checktoxicity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 08:54:37.000000 checktoxicity-0.1.2/checktoxicity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 08:54:37.000000 checktoxicity-0.1.2/checktoxicity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 08:54:38.095395 checktoxicity-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      354 2023-07-27 04:13:04.000000 checktoxicity-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:54:38.091386 checktoxicity-0.1.2/toxic/
+-rw-rw-rw-   0        0        0        0 2023-07-21 10:38:11.000000 checktoxicity-0.1.2/toxic/__init__.py
+-rw-rw-rw-   0        0        0     1325 2023-07-27 04:10:13.000000 checktoxicity-0.1.2/toxic/toxic.py
```

### Comparing `checktoxicity-0.1.1/toxic/toxic.py` & `checktoxicity-0.1.2/toxic/toxic.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
         try:
             self.response = self.getScoreFromAPI()
         except Exception:
             self.response = "error in moderation layer"
 
     def check_toxicity(self, response_data):
         for label_info in response_data[0]:
-            if label_info['score'] >= 0.8:
-                return True
+            if label_info['label'] == 'toxic':
+                return label_info['score'] >= 0.9
         return False
 
     def getScoreFromAPI(self):
         payload = {"inputs": self.query}
         response = requests.post(self.API_ENDPOINT, headers=self.HEADERS, json=payload)
         if response.status_code == 200:
             response_json = response.json()
             self.check_toxicity(response_json)
             if self.check_toxicity(response_json):
                 return "Sorry, we can't show this content as it is flagged as toxic."
             else:
                 return self.query
         else:
-            raise Exception("Hugging Face Space is down...")
+            raise Exception("Hugging Face Space is down...")
```

