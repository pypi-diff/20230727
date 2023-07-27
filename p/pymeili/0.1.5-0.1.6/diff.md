# Comparing `tmp/pymeili-0.1.5.tar.gz` & `tmp/pymeili-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.1.5.tar", last modified: Wed Jul 26 16:18:48 2023, max compression
+gzip compressed data, was "pymeili-0.1.6.tar", last modified: Thu Jul 27 10:00:28 2023, max compression
```

## Comparing `pymeili-0.1.5.tar` & `pymeili-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:18:48.968382 pymeili-0.1.5/
--rw-rw-rw-   0        0        0      314 2023-07-26 16:17:52.000000 pymeili-0.1.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.5/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1480 2023-07-26 16:18:48.967385 pymeili-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-07-26 14:23:15.000000 pymeili-0.1.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 16:18:48.935049 pymeili-0.1.5/pymeili/
-drwxrwxrwx   0        0        0        0 2023-07-26 16:18:48.965390 pymeili-0.1.5/pymeili/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.5/pymeili/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.5/pymeili/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.5/pymeili/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0      785 2023-07-26 16:14:50.000000 pymeili-0.1.5/pymeili/__init__.py
--rw-rw-rw-   0        0        0    55863 2023-07-26 16:18:19.000000 pymeili-0.1.5/pymeili/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:18:48.949518 pymeili-0.1.5/pymeili.egg-info/
--rw-rw-rw-   0        0        0     1480 2023-07-26 16:18:48.000000 pymeili-0.1.5/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-26 16:18:48.000000 pymeili-0.1.5/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:18:48.000000 pymeili-0.1.5/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 16:18:48.000000 pymeili-0.1.5/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 16:18:48.968382 pymeili-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-07-26 14:22:16.000000 pymeili-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:00:28.242092 pymeili-0.1.6/
+-rw-rw-rw-   0        0        0      384 2023-07-27 09:58:37.000000 pymeili-0.1.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.6/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-07-27 10:00:28.242092 pymeili-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-07-26 14:23:15.000000 pymeili-0.1.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 10:00:28.211522 pymeili-0.1.6/pymeili/
+drwxrwxrwx   0        0        0        0 2023-07-27 10:00:28.240590 pymeili-0.1.6/pymeili/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.6/pymeili/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.6/pymeili/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.6/pymeili/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0      785 2023-07-27 09:58:43.000000 pymeili-0.1.6/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    57797 2023-07-27 09:57:48.000000 pymeili-0.1.6/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:00:28.225074 pymeili-0.1.6/pymeili.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-07-27 10:00:28.000000 pymeili-0.1.6/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-27 10:00:28.000000 pymeili-0.1.6/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 10:00:28.000000 pymeili-0.1.6/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 10:00:28.000000 pymeili-0.1.6/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 10:00:28.242092 pymeili-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-07-27 09:58:47.000000 pymeili-0.1.6/setup.py
```

### Comparing `pymeili-0.1.5/LISCENCE.txt` & `pymeili-0.1.6/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.5/PKG-INFO` & `pymeili-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.5
+Version: 0.1.6
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -44,7 +44,10 @@
 - Add Subplot Function
 
 0.1.3 (26/07/2023)
 - Fix Some Minor Problems
 
 0.1.5 (27/07/2023)
 - Add Basic Basemap Function, fix some problems
+
+0.1.6 (27/07/2023)
+- Fix Some Problems, add common raise function
```

### Comparing `pymeili-0.1.5/README.txt` & `pymeili-0.1.6/README.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.5/pymeili/FONT/Futura Extra Black font.ttf` & `pymeili-0.1.6/pymeili/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.5/pymeili/FONT/Futura Heavy font.ttf` & `pymeili-0.1.6/pymeili/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.5/pymeili/FONT/futura medium bt.ttf` & `pymeili-0.1.6/pymeili/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.5/pymeili/__init__.py` & `pymeili-0.1.6/pymeili/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     fill_between, fill_betweenx,
     pause, normalize, adjust, addaxes, slider, set_xydata,
     figsize, show, clf, close, figure, savefig,
     imread, imshow, imsave,
     
 )
 
-__version__: str = '0.1.5'
+__version__: str = '0.1.6'
```

### Comparing `pymeili-0.1.5/pymeili/beautifyplot.py` & `pymeili-0.1.6/pymeili/beautifyplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,33 +4,47 @@
 import matplotlib.font_manager as fm
 from matplotlib.colors import LinearSegmentedColormap
 from mpl_toolkits.basemap import Basemap as Bp
 
 global fontscale
 fontscale = 0.6
 
+class bcolors:
+    HEADER = '\033[95m'
+    OKBLUE = '\033[94m'
+    OKCYAN = '\033[96m'
+    OKGREEN = '\033[92m'
+    WARNING = '\033[93m'
+    FAIL = '\033[91m'
+    ENDC = '\033[0m'
+    BOLD = '\033[1m'
+    UNDERLINE = '\033[4m'
+
+
+# METHOD I
 # 獲取當前檔案位址
 currentfilepath = __file__
 
 # 刪去__file__中最後面自"\"開始的字串(刪除檔名)
 motherpath = currentfilepath[:-len(currentfilepath.split('\\')[-1])]
-
 try:
     fontpath = Path(mpl.get_data_path(), motherpath+"\\futura medium bt.ttf")
     fontpath_bold = Path(mpl.get_data_path(), motherpath+"\Futura Heavy font.ttf")
     fontpath_black = Path(mpl.get_data_path(), motherpath+"\Futura Extra Black font.ttf")
 except: # 未安裝字體
-    raise Exception('Please install Futura fonts in the same directory as this file.\ninstall font-packages: https://dwl.freefontsfamily.com/download/futura/;\n Moving the font file to installed module folder(e.g."C:>Users>Username>AppData>Local>Programs>Python>Python311>Lib>site-packages>pymeili").')
-
+    raise Exception(bcolors.WARNING+'Please install Futura fonts in the same directory as this file.\ninstall font-packages: https://dwl.freefontsfamily.com/download/futura/;\n Moving the font file to installed module folder(e.g."C:>Users>Username>AppData>Local>Programs>Python>Python311>Lib>site-packages>pymeili").'+bcolors.ENDC)
 '''
-motherpath = 'C:/Windows/Fonts'
-
-fontpath = Path(mpl.get_data_path(), "C:\Windows\Fonts\Futura Md BT\\futura medium bt.ttf")
-fontpath_bold = Path(mpl.get_data_path(), "\FONT\Futura Heavy font.ttf")
-fontpath_black = Path(mpl.get_data_path(),"\FONT\Futura Extra Black font.ttf")
+# METHOD II
+url_medium = r'https://github.com/VVVICTORZHOU/resources/blob/main/futura%20medium%20bt.ttf'
+url_Heavy = r'https://github.com/VVVICTORZHOU/resources/blob/main/Futura%20Heavy%20font.ttf'
+url_Black = r'https://github.com/VVVICTORZHOU/resources/blob/main/Futura%20Extra%20Black%20font.ttf'
+
+fontpath = Path(mpl.get_data_path(), urllib3.PoolManager().request('GET', url_medium).data)
+fontpath_bold = Path(mpl.get_data_path(), urllib3.PoolManager().request('GET', url_Heavy).data)
+fontpath_black = Path(mpl.get_data_path(), urllib3.PoolManager().request('GET', url_Black).data)
 '''
 
 # 初始化
 def initplot(style='default',figsize=(10,8),background=True):
     global theme
     if style == 'default'or style == 'light_background' or style == 'light' or style == 'l':
         theme = 'default'
@@ -57,137 +71,148 @@
         if all(i in ['bg', 'bg1', 'bg2', 'fg', '1', '2', '3', '4', 'rfg'] for i in index):
             return [colorseries[i] for i in index]
         else:
             return index
     else:
         str(index)
         if index in ['bg', 'bg1', 'bg2', 'fg', '1', '2', '3', '4', 'rfg']:
-            if theme == 'default':
-                colorseries = {'bg': '#D9EEFD',
-                            'bg1': '#D9EEFD',
-                            'bg2': '#F7DCD1',
-                            'rfg': '#F5F5F5',
-                            'fg': '#111111',
-                            '1': '#0A9CCF',
-                            '2': '#AC005A',
-                            '3': '#A19253',
-                            '4': '#A43713'}
-                return colorseries[index]
-                            
-            elif theme == 'dark_background':
-                colorseries = {'bg': '#122D64',
-                            'bg1': '#122D64',
-                            'bg2': '#122D64',
-                            'rfg': '#080808',
-                            'fg': '#EEEEEE',
-                            '1': '#0A9CCF',
-                            '2': '#AC005A',
-                            '3': '#A19253',
-                            '4': '#A43713'}
-                return colorseries[index]
+            try:    
+                if theme == 'default':
+                    colorseries = {'bg': '#D9EEFD',
+                                'bg1': '#D9EEFD',
+                                'bg2': '#F7DCD1',
+                                'rfg': '#F5F5F5',
+                                'fg': '#111111',
+                                '1': '#0A9CCF',
+                                '2': '#AC005A',
+                                '3': '#A19253',
+                                '4': '#A43713'}
+                    return colorseries[index]
+                                
+                elif theme == 'dark_background':
+                    colorseries = {'bg': '#122D64',
+                                'bg1': '#122D64',
+                                'bg2': '#122D64',
+                                'rfg': '#080808',
+                                'fg': '#EEEEEE',
+                                '1': '#0A9CCF',
+                                '2': '#AC005A',
+                                '3': '#A19253',
+                                '4': '#A43713'}
+                    return colorseries[index]
+            except: # NameError: name 'theme' is not defined
+                raise Exception(bcolors.WARNING+'Please run initplot() first.'+bcolors.ENDC)
+                
         else:
             return index
     
 def cmaplist(index):
     str(index)
     if index in ['-28','28','-27','-26','-25','-24','-23','-22','22','23','24','25','26','27','12','13','14','15','-12','-13','-14','-15']:
-        if theme == 'default':
-            if index == '15':
-                return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#D5EDD5','#E08A16','#AB503B'])
-            if index == '14':
-                return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#E08A16','#AB503B'])
-            if index == '13':
-                return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#D5EDD5','#AB503B'])
-            if index == '12':
-                return LinearSegmentedColormap.from_list('mycmap', ['#47A7DE','#E08A16'])
-
-            if index == '-15': # reversed 1
-                return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#D5EDD5','#47A7DE','#454FB4'])
-            if index == '-14': # reversed 1 but 4 colors
-                return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#47A7DE','#454FB4'])
-            if index == '-13': # reversed 1 but 3 colors
-                return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#D5EDD5','#454FB4'])
-            if index == '-12': # reversed 1 but 2 colors
-                return LinearSegmentedColormap.from_list('mycmap', ['#E08A16','#47A7DE'])
-
-            if index == '28':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E','#BB8263'])        
-            if index == '27':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E','#BB8263'])
-            if index == '26':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E'])
-            if index == '25':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F'])
-            if index == '24':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A'])
-            if index == '23':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4'])
-            if index == '22':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF'])
-
-            if index == '-28': # reversed 2
-                return LinearSegmentedColormap.from_list('mycmap', ['#BB8263','#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE','#EEEEEE']) 
-            if index == '-27': # reversed 2
-                return LinearSegmentedColormap.from_list('mycmap', ['#BB8263','#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
-            if index == '-26': # reversed 2 but 6 colors
-                return LinearSegmentedColormap.from_list('mycmap', ['#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
-            if index == '-25':
-                return LinearSegmentedColormap.from_list('mycmap', ['#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
-            if index == '-24':
-                return LinearSegmentedColormap.from_list('mycmap', ['#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
-            if index == '-23':
-                return LinearSegmentedColormap.from_list('mycmap', ['#F1C9B4','#F2CABF','#EEEEEE'])
-            if index == '-22':
-                return LinearSegmentedColormap.from_list('mycmap', ['#F2CABF','#EEEEEE'])
-        
-        
-        elif theme == 'dark_background':
-            if index == '15':
-                return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#D5EDD5','#E08A16','#AB503B'])
-            if index == '14':
-                return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#E08A16','#AB503B'])
-            if index == '13':
-                return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#D5EDD5','#AB503B'])
-            if index == '12':
-                return LinearSegmentedColormap.from_list('mycmap', ['#47A7DE','#E08A16'])
-
-            if index == '-15': # reversed 1
-                return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#D5EDD5','#47A7DE','#454FB4'])
-            if index == '-14': # reversed 1 but 4 colors
-                return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#47A7DE','#454FB4'])
-            if index == '-13': # reversed 1 but 3 colors
-                return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#D5EDD5','#454FB4'])
-            if index == '-12': # reversed 1 but 2 colors
-                return LinearSegmentedColormap.from_list('mycmap', ['#E08A16','#47A7DE'])
-                    
-            if index == '27':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E','#BB8263'])
-            if index == '26':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E'])
-            if index == '25':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F'])
-            if index == '24':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A'])
-            if index == '23':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4'])
-            if index == '22':
-                return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF'])
-              
-            if index == '-27': # reversed 2
-                return LinearSegmentedColormap.from_list('mycmap', ['#BB8263','#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
-            if index == '-26': # reversed 2 but 6 colors
-                return LinearSegmentedColormap.from_list('mycmap', ['#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
-            if index == '-25':
-                return LinearSegmentedColormap.from_list('mycmap', ['#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
-            if index == '-24':
-                return LinearSegmentedColormap.from_list('mycmap', ['#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
-            if index == '-23':
-                return LinearSegmentedColormap.from_list('mycmap', ['#F1C9B4','#F2CABF','#EEEEEE'])
-            if index == '-22':
-                return LinearSegmentedColormap.from_list('mycmap', ['#F2CABF','#EEEEEE'])
+        try:
+            if theme == 'default':
+                if index == '15':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#D5EDD5','#E08A16','#AB503B'])
+                if index == '14':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#E08A16','#AB503B'])
+                if index == '13':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#D5EDD5','#AB503B'])
+                if index == '12':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#47A7DE','#E08A16'])
+
+                if index == '-15': # reversed 1
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#D5EDD5','#47A7DE','#454FB4'])
+                if index == '-14': # reversed 1 but 4 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#47A7DE','#454FB4'])
+                if index == '-13': # reversed 1 but 3 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#D5EDD5','#454FB4'])
+                if index == '-12': # reversed 1 but 2 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#E08A16','#47A7DE'])
+
+                if index == '28':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#D9EEFD','#FFFFFF','#FFFFFF','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E','#BB8263'])        
+                if index == '27':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E','#BB8263'])
+                if index == '26':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E'])
+                if index == '25':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F'])
+                if index == '24':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A'])
+                if index == '23':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4'])
+                if index == '22':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF'])
+
+                if index == '-28': # reversed 2
+                    return LinearSegmentedColormap.from_list('mycmap', ['#BB8263','#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#FFFFFF','#FFFFFF','#D9EEFD']) 
+                if index == '-27': # reversed 2
+                    return LinearSegmentedColormap.from_list('mycmap', ['#BB8263','#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE','#EEEEEE'])
+                if index == '-26': # reversed 2 but 6 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
+                if index == '-25':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
+                if index == '-24':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
+                if index == '-23':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#F1C9B4','#F2CABF','#EEEEEE'])
+                if index == '-22':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#F2CABF','#EEEEEE'])
+            
+            
+            elif theme == 'dark_background':
+                if index == '15':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#D5EDD5','#E08A16','#AB503B'])
+                if index == '14':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#47A7DE','#E08A16','#AB503B'])
+                if index == '13':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#454FB4','#D5EDD5','#AB503B'])
+                if index == '12':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#47A7DE','#E08A16'])
+
+                if index == '-15': # reversed 1
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#D5EDD5','#47A7DE','#454FB4'])
+                if index == '-14': # reversed 1 but 4 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#E08A16','#47A7DE','#454FB4'])
+                if index == '-13': # reversed 1 but 3 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#AB503B','#D5EDD5','#454FB4'])
+                if index == '-12': # reversed 1 but 2 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#E08A16','#47A7DE'])
+                        
+                if index == '28':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#D9EEFD','#FFFFFF','#FFFFFF','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E','#BB8263'])        
+                if index == '27':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E','#BB8263'])
+                if index == '26':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F','#CF725E'])
+                if index == '25':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A','#DB997F'])
+                if index == '24':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4','#DCB29A'])
+                if index == '23':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF','#F1C9B4'])
+                if index == '22':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#EEEEEE','#F2CABF'])
+                
+                if index == '-28': # reversed 2
+                    return LinearSegmentedColormap.from_list('mycmap', ['#BB8263','#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#FFFFFF','#FFFFFF','#D9EEFD']) 
+                if index == '-27': # reversed 2
+                    return LinearSegmentedColormap.from_list('mycmap', ['#BB8263','#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
+                if index == '-26': # reversed 2 but 6 colors
+                    return LinearSegmentedColormap.from_list('mycmap', ['#CF725E','#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
+                if index == '-25':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#DB997F','#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
+                if index == '-24':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#DCB29A','#F1C9B4','#F2CABF','#EEEEEE'])
+                if index == '-23':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#F1C9B4','#F2CABF','#EEEEEE'])
+                if index == '-22':
+                    return LinearSegmentedColormap.from_list('mycmap', ['#F2CABF','#EEEEEE'])
+        except: # NameError: name 'theme' is not defined
+            raise Exception(bcolors.WARNING+'Please run initplot() first.'+bcolors.ENDC)
     else: 
         return index
 
 # LABEL設定
 '''
 默認下系統會在使用者繪製不同種類的圖形添加LABEL計數，依種類分開計數，無法在圖例中顯示出來的LABEL不用計數；使用者依然可以手動為LABEL賦值進行覆蓋
 '''
@@ -266,28 +291,28 @@
 # contour繪圖
 def contour(x, y, z, colors='fg', levels=10, linewidths=2, clabel=True, fontsize=12, color='fg', **kwargs):
     CS = plt.contour(x, y, z, colors=colorlist(colors), levels=levels, linewidths=linewidths, **kwargs)
     if clabel == True:
         CL = CS.clabel(fontsize=fontsize, colors=colorlist(color), inline=True)
 
 # contourf繪圖
-def contourf(x, y, z, levels=10, cmap='2', contour=True, clabel=True,linewidths=1.5, color='fg', **kwargs):
+def contourf(x, y, z, levels=10, cmap='28', contour=True, clabel=True,linewidths=1.5, color='fg', **kwargs):
     if contour == True:
         CS = plt.contour(x, y, z, colors=colorlist(color), levels=levels, linewidths=linewidths)
     if clabel == True:
         CL = CS.clabel(fontsize=8, colors=colorlist(color), inline=True)
     plt.contourf(x, y, z, cmap=cmaplist(cmap), **kwargs)
 
 # colorbar顯示
-def colorbar(ticks,label=' ', orientation='vertical',shrink=0.95, aspect=20, labelfontsize=16, font=fontpath, color='fg',**kwargs):
+def colorbar(ticks,label=' ', orientation='vertical',shrink=0.95, aspect=20, fraction=0.046, pad=0.04, labelfontsize=16, font=fontpath, color='fg',**kwargs):
     if orientation == 'v' or 'V':
         orientation = 'vertical'
     elif orientation == 'h' or 'H':
         orientation = 'horizontal'
-    CB = plt.colorbar(orientation=orientation, shrink=shrink, aspect=aspect, label=label, **kwargs)
+    CB = plt.colorbar(orientation=orientation, shrink=shrink, aspect=aspect, label=label, fraction=fraction, pad=pad, **kwargs)
     CB.ax.tick_params(labelsize=labelfontsize, labelcolor=colorlist(color), color=colorlist(color))
     CB.ax.set_ylabel(label, fontproperties=fm.FontProperties(fname=font, size=labelfontsize), color=colorlist(color))
     CB.ax.set_yticks(ticks,ticks, fontproperties=fm.FontProperties(fname=font, size=labelfontsize))
     CB.ax.yaxis.set_tick_params(color=colorlist(color), labelcolor=colorlist(color))
     CB.outline.set_color(colorlist(color))
     CB.outline.set_linewidth(2)
 
@@ -485,15 +510,15 @@
 def figure():
     plt.figure()
 
 # 圖像處理
 def imread(filename, format=None):
     return plt.imread(filename, format=format)
 
-def imshow(X, cmap='2', vmin=None, vmax=None, interpolation='nearest', alpha=None, aspect=None, **kwargs):
+def imshow(X, cmap='28', vmin=None, vmax=None, interpolation='nearest', alpha=None, aspect=None, **kwargs):
     plt.imshow(X, cmap=cmaplist(cmap), vmin=vmin, vmax=vmax, interpolation=interpolation, alpha=alpha, aspect=aspect, **kwargs)
 
 def imsave(filename, arr, vmin=None, vmax=None, cmap='2', format=None, origin=None, dpi=300, **kwargs):
     plt.imsave(filename, arr, vmin=vmin, vmax=vmax, cmap=cmaplist(cmap), format=format, origin=origin, dpi=dpi, **kwargs)
 
 # 重設值
 def set_xydata(x=None, y=None):
@@ -1019,13 +1044,20 @@
 def normalize(data, vmin=None, vmax=None):
     plt.Normalize(data, vmin=vmin, vmax=vmax)
 
 def slider(ax, label, valmin, valmax, valinit=0, valfmt='%1.2f', valstep=None, orientation='horizontal', **kwargs):
     return Slider(ax, label, valmin, valmax, valinit=valinit, valfmt=valfmt, valstep=valstep, orientation=orientation, **kwargs)
 
 
+
+
+
+    
+
+
+
 # https://matplotlib.org/stable/gallery/widgets/slider_demo.html
```

### Comparing `pymeili-0.1.5/pymeili.egg-info/PKG-INFO` & `pymeili-0.1.6/pymeili.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.5
+Version: 0.1.6
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -44,7 +44,10 @@
 - Add Subplot Function
 
 0.1.3 (26/07/2023)
 - Fix Some Minor Problems
 
 0.1.5 (27/07/2023)
 - Add Basic Basemap Function, fix some problems
+
+0.1.6 (27/07/2023)
+- Fix Some Problems, add common raise function
```

### Comparing `pymeili-0.1.5/setup.py` & `pymeili-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.1.5',
+    version='0.1.6',
     description='a module to beautify your python plot.',
     long_description=open('README.txt',encoding="utf-8").read() + '\n\n' + open('CHANGELOG.txt',encoding="utf-8").read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

