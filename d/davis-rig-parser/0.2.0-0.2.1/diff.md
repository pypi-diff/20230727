# Comparing `tmp/davis_rig_parser-0.2.0.tar.gz` & `tmp/davis_rig_parser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davis_rig_parser-0.2.0.tar", last modified: Tue Jul 25 19:05:02 2023, max compression
+gzip compressed data, was "davis_rig_parser-0.2.1.tar", last modified: Thu Jul 27 16:18:01 2023, max compression
```

## Comparing `davis_rig_parser-0.2.0.tar` & `davis_rig_parser-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-25 19:05:02.578502 davis_rig_parser-0.2.0/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-25 19:05:02.578502 davis_rig_parser-0.2.0/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5477 2023-07-06 15:43:33.000000 davis_rig_parser-0.2.0/README.md
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-25 19:05:02.578502 davis_rig_parser-0.2.0/davis_rig_parser/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.2.0/davis_rig_parser/__init__.py
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    19782 2023-07-25 18:56:33.000000 davis_rig_parser-0.2.0/davis_rig_parser/davis_rig_parser.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-25 19:05:02.578502 davis_rig_parser-0.2.0/davis_rig_parser.egg-info/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-25 19:05:02.000000 davis_rig_parser-0.2.0/davis_rig_parser.egg-info/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-25 19:05:02.000000 davis_rig_parser-0.2.0/davis_rig_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-25 19:05:02.000000 davis_rig_parser-0.2.0/davis_rig_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-25 19:05:02.000000 davis_rig_parser-0.2.0/davis_rig_parser.egg-info/requires.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-25 19:05:02.000000 davis_rig_parser-0.2.0/davis_rig_parser.egg-info/top_level.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-25 19:05:02.578502 davis_rig_parser-0.2.0/setup.cfg
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-25 19:04:48.000000 davis_rig_parser-0.2.0/setup.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-25 19:05:02.578502 davis_rig_parser-0.2.0/tests/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.2.0/tests/test.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-27 16:18:01.218374 davis_rig_parser-0.2.1/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-27 16:18:01.218374 davis_rig_parser-0.2.1/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5477 2023-07-06 15:43:33.000000 davis_rig_parser-0.2.1/README.md
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-27 16:18:01.218374 davis_rig_parser-0.2.1/davis_rig_parser/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.2.1/davis_rig_parser/__init__.py
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    19819 2023-07-27 16:13:47.000000 davis_rig_parser-0.2.1/davis_rig_parser/davis_rig_parser.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-27 16:18:01.218374 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-27 16:18:01.000000 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-27 16:18:01.000000 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-27 16:18:01.000000 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-27 16:18:01.000000 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/requires.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-27 16:18:01.000000 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/top_level.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-27 16:18:01.222375 davis_rig_parser-0.2.1/setup.cfg
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-27 16:17:34.000000 davis_rig_parser-0.2.1/setup.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-27 16:18:01.218374 davis_rig_parser-0.2.1/tests/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.2.1/tests/test.py
```

### Comparing `davis_rig_parser-0.2.0/README.md` & `davis_rig_parser-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `davis_rig_parser-0.2.0/davis_rig_parser/davis_rig_parser.py` & `davis_rig_parser-0.2.1/davis_rig_parser/davis_rig_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,16 @@
                             cut_t = 0
                             while row[0] < min_latency:
                                 cut_t += row[1] #total time cut from the trial in ms
                                 row[0] = row[0] + row[1]
                                 row[1:-1] = row[2:]
                                 row[-1] = 0
                                 cuts +=1
-                                if cuts >5: #failsafe so the loop doesn't go infinite, arbitrarily set at 5
+                                if cuts > len(row): #failsafe so the loop doesn't go infinite
+                                    row[0] = np.nan
                                     break
                             #then, set all ILIs under min_ILI to 0 to be deleted later
                             for j in range(1, len(row)):
                                 if row[j] < min_ILI and row[j] != 0:
                                     row[j] = 0
                                     cuts+=1
                         cutslist.append(cuts)
@@ -430,14 +431,13 @@
     if save_df==True:
         df.to_pickle(dir_name+'/%s_grouped_dframe.df' %(date.today().strftime("%d_%m_%Y")))
 
     return df
 
 
 
-
 #Work in progress below ---- No documentation yet
 def assign_day(df):
     #uses a date column to assign a day column
     for name, group in df.groupby(['Animal']):
         mindate = min(df['Date'])
         group['Day'] = [(x).days + 1 for x in (group['Date'] - mindate)]
```

