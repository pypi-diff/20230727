# Comparing `tmp/baselibs-0.1.1.tar.gz` & `tmp/baselibs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\baselibs-0.1.1.tar", last modified: Thu Jun 29 03:51:44 2023, max compression
+gzip compressed data, was "dist\baselibs-0.1.2.tar", last modified: Thu Jul 27 01:29:27 2023, max compression
```

## Comparing `baselibs-0.1.1.tar` & `baselibs-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 03:51:44.000000 baselibs-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-29 03:51:44.000000 baselibs-0.1.1/baselibs.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-29 03:51:44.000000 baselibs-0.1.1/baselibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1317 2023-06-29 03:51:44.000000 baselibs-0.1.1/baselibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-06-29 03:51:44.000000 baselibs-0.1.1/baselibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 03:51:44.000000 baselibs-0.1.1/baselibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    30281 2023-06-29 03:45:22.000000 baselibs-0.1.1/baselibs.py
--rw-rw-rw-   0        0        0    35823 2020-04-20 05:16:32.000000 baselibs-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1317 2023-06-29 03:51:44.000000 baselibs-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      667 2023-06-14 01:22:02.000000 baselibs-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 03:51:44.000000 baselibs-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1518 2023-06-29 03:51:29.000000 baselibs-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:29:27.000000 baselibs-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-27 01:29:27.000000 baselibs-0.1.2/baselibs.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-27 01:29:27.000000 baselibs-0.1.2/baselibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1370 2023-07-27 01:29:27.000000 baselibs-0.1.2/baselibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-07-27 01:29:27.000000 baselibs-0.1.2/baselibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 01:29:27.000000 baselibs-0.1.2/baselibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    31512 2023-07-27 00:52:43.000000 baselibs-0.1.2/baselibs.py
+-rw-rw-rw-   0        0        0    35823 2020-04-20 05:16:32.000000 baselibs-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1370 2023-07-27 01:29:27.000000 baselibs-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      669 2023-06-29 03:58:20.000000 baselibs-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 01:29:27.000000 baselibs-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2023-07-27 01:12:06.000000 baselibs-0.1.2/setup.py
```

### Comparing `baselibs-0.1.1/baselibs.egg-info/PKG-INFO` & `baselibs-0.1.2/baselibs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: baselibs
-Version: 0.1.1
+Version: 0.1.2
 Summary: baselibs
 Home-page: https://github.com/xmxoxo/baselibs
 Author: He xi
 Author-email: xmhexi@qq.com
 License: UNKNOWN
 Project-URL: Blog, https://blog.csdn.net/xmxoxo
 Keywords: baselibs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 通用基础库 
 
-版本: v0.1
+版本: v0.1.1
 
 可对目录下的文件进行以下批量处理：
 
 * 清除空格 空行 按句子分行；
 * 删除空文件，找到后改名（改为"原文件名.del") 或者直接删除
 * 删除重复的文件:   根据文件的MD5判断文件是否相同，找到后改名（原文件.same)或者直接删除
 * 批量重命名:    可按序号进行重命名，默认从1开始，文件名会自动在前面补0，例如"0001.txt"
```

### Comparing `baselibs-0.1.1/baselibs.py` & `baselibs-0.1.2/baselibs.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import time
 import string
 import pandas as pd
 import numpy as np
 import traceback
 import logging
 
-#from CharsetFilter import *
+# from CharsetFilter import *
 
 pl = lambda x='', y='-': print(y*40) if x=='' else print(str(x)) if x[-3:]=='...' or y=='' else print(str(x).center(40, y))
 pr = lambda x: print('%s:%s' % (x, eval(x)))
 pt = lambda x, y=60: (print('\r%s'% (' '*y), end=''), print('\r%s'%x, end=''))
 
 
 def rand_filename(path='', pre='', ext=''):
@@ -315,14 +315,44 @@
                         yield file_path
                 if os.path.isdir(file_path):
                     yield from getAllFiles_Generator(file_path, fileExt)
     except Exception as e :
         print(e)
         pass
 
+def rel_file(workpath, fname, outpath, new_name='', remain_deep=1, abspath=0):
+    ''' 生成相对的文件路径并保持目录结构
+    将workpath下的fname文件，生成到outpath目录下,
+    文件改名为new_name；new_name为空则保留原文件名
+    保留最后remain_deep级目录及子目录结构，
+    abspath: 是否输出绝对路径
+    '''
+
+    spath, sname = os.path.split(fname)
+    # 计算相对路径：remain_deep=保留的目录结构深度
+    remain_path = '../' * remain_deep
+    tpath = os.path.join(workpath, remain_path)
+    rpath = os.path.relpath(spath, tpath)
+    # 计算新的目录
+    folder = os.path.join(outpath, rpath)
+    # print('rpath:', rpath)
+    # print('folder:', folder)
+    # 创建目录
+    if not os.path.exists(folder):
+        os.makedirs(folder, exist_ok=True)
+
+    # 计算新的文件路径
+    if new_name == '':
+        new_name = sname
+    fout = os.path.join(folder, new_name)
+    # 返回绝对路径
+    if abspath:
+        fout = os.path.abspath(fout)
+    return fout
+
 # -----------------------------------------
 class TimeCount():
     '''简单计时器 '''
 
     def __init__(self):
         self.clean()
 
@@ -364,14 +394,15 @@
     def stop(self):
         ''' 停止计时器
         '''
 
         self.clean()
 
 # -----------------------------------------
+
 def api_post_data (url, data, timeout=30, data_format='json'):
     ''' 向URL发送数据并返回json格式化结果
     '''
 
     import requests
     import json
     try:
@@ -387,16 +418,14 @@
         return None
 
 # -----------------------------------------
 
 def pre_format (path):
     '''对目录下的文件遍历，处理文本内容清洗（含HTML格式去除）
     '''
-
-
     intTotalLines = 0
     lstF = getFiles(path)
 
     for fname in lstF[1] :
         print('Processing file:%s' % (fname))
         txt = readtxtfile(fname)
         txt = fmtText(txt)
@@ -464,81 +493,80 @@
         os.rename(f, nfname)
 
         # 调试用
         if intBegin>10:
             pass
             #break
 
-
-# 判断是否为空文件 空文件是替换了空格，制表符
 def blankfile (fname):
+    ''' 判断是否为空文件； 空文件是指替换了空格，制表符后内容为空的文件
+    '''
     pass
     txt = readtxtfile(fname)
     txt = delspace(txt)
     txt = txt.replace('\n','')
     txt = txt.replace('\r','')
     if txt == "":
         return fname
     else:
         return ''
 
-# 删除目录下的空文件 
 def delblankfile (path, isDel = False):
+    '''  删除目录下的空文件 
+    '''
     lstF = getFiles(path)
     for f in lstF[1] :
         print('\rfile:%s' % f,end = '')
         #print('file:%s' % f)
         if blankfile(f):
             print('\rblank file: %s' % f)
             if isDel:
                 os.remove(f)
             else:
                 os.rename(f, f+'.del')
     print('\r'+' '*60)
 
 
-# 计算文本的MD5值
 def txtmd5 (txt):
+    ''' 计算文本的MD5值
+    '''
     strMD5 = hashlib.md5(txt.encode(encoding='UTF-8')).hexdigest()
     return strMD5
 
-
 def SameFile (dicHash, strFileName, strBody):
     '''
     判断内容相同的文件，使用MD5进行计算
     参数：
         dicHash        哈希表，用来存放文件名与哈希值对应关系；
         strFileName    文件名，用来标识文件，也可用完整路径；
         strBody        文件内容
     返回：
         None 则表示没有重复，并且会更新哈希表
         重复时返回重复的文件名  
     '''
     
     strMD5 = txtmd5(strBody)
     if strMD5 in dicHash.keys():
-        #冲突表示重复了
+        # 冲突表示重复，返回对应的值
         return dicHash[strMD5]
     else:
         dicHash[strMD5] = strFileName
         return None
 
-
-def FindSameFile (path, isDel = False):
+def FindSameFile (path, isDel=False):
     '''
     检查目录下文件内容是否相同,使用MD5值来判断文件的相同。
     相同的文件可以直接删除或者改名为"原文件名.same",
     同时输出提示信息,例如：
         File [./dat/1.txt] =same=> [./dat/92.txt] 
     参数:
        path    要检查的目录；只检查该目录不包含子目录；
        isDel   是否要删除，默认为否。 为“是”时直接删除文件，为“否”时将文件改名
     返回：
        无
-
     '''
 
     dicHash = {}
     lstF = getFiles(path)
     for fname in lstF[1] :
         print('\rcheck file:%s' % fname,end = '')
         txt = readtxtfile(fname)
@@ -549,16 +577,17 @@
                 os.remove(fname)
             else:
                 os.rename(fname, fname + '.same')
             #break
     print('\r'+' '*60)
 
 
-# 根据系统返回换行符
 def sysCRLF ():
+    ''' 根据系统返回换行符
+    '''
     if os.name == 'nt':
         strCRLF = '\n'
     else:
         strCRLF = '\r\n'
     return strCRLF
 
 def get_randstr (strlen=10):
@@ -584,15 +613,15 @@
     '''
     
     s = list(range(48,58)) + list(range(65,91)) + list(range(97,123))
     tmp = ''.join(map(chr, random.sample(s, 5)))
     filename = '%s%s%s' % (pre, time.strftime('%Y%m%d%H%M%S',time.localtime()) + tmp, ext)
     return filename
 
-def pre_process (path,addFirstLine = 0):
+def pre_process (path, addFirstLine=0):
     '''
     文本预处理，删除文件中的空格，空行，并按句子分行，然后在每句前面加上标签0；
     '''
 
     i = 0 
     lstF = getFiles(path)
     for fname in lstF[1] :
@@ -621,37 +650,35 @@
         #if i>9:
         #    pass
             #break
     #print('\r'+' '*60)
     print('Total files: %d' % i)
 
 def pre_NER (txt):
+    ''' NER标注处理，一个字一行
     '''
-    NER标注处理，一个字一行
-    '''
-
     lstL = list(txt)
     strRet = sysCRLF().join(lstL)
     return strRet
 
-def pre_addcolumn (lsttxt,lineBegin = 1):
+def pre_addcolumn (lsttxt, lineBegin=1):
     '''
     每行加上空列，参数可指定空列在行首还是行尾,默认为行首
     参数： lsttxt 每行的list
+    lineBegin： 1表示空列加在前面；
     '''
     pass
     if lineBegin:
         lstLine = [ '0\t'+x for x in lsttxt ]
     else:
         lstLine = [ x+'\t0' for x in lsttxt ]
     return lstLine
 
-def pre_allzero (lsttxt,lineNo = 1):
-    '''
-    判断数据文件第N列是否全为0 ，默认N=1
+def pre_allzero (lsttxt,lineNo=1):
+    ''' 判断数据文件第N列是否全为0 ，默认N=1
     '''
     
     ret = True
     for line in lsttxt:
         lstW = line.split('\t')
         if lstW[lineNo-1] != 0:
             ret = False
@@ -713,45 +740,43 @@
         return 0
     except Exception as e :
         print("Error in pd_datSample:")
         print(e)
         return -1    
 
 def pre_labelcount (lsttxt, columnindex=0, labelvalue='0'):
-    '''
-    统计文本中某类标签情况
+    '''统计文本中某类标签情况
     '''
 
     intLabel = 0
     for line in lsttxt:
         lstW = line.split('\t')
         if lstW[columnindex] == str(labelvalue):
             intLabel += 1
     return intLabel
 
-def str2List (strText,sp = ',' ):
-    '''
-    # 字符串转化为整数型List,用于参数传递
+def str2List (strText, sp=','):
+    ''' 字符串转化为整数型List,用于参数传递
     # 默认拆分符号为英文逗号","
     '''
     try:
         ret = strText.split(sp)
         ret = [int(x) for x in ret]
         return ret
     except Exception as e :
         print("Error in str2List:")
         print(e)
         return None    
-def splitset(datfile, lstScale =[7,2,1]):
-    '''
-    将指定的数据文件（文本文件）按指定的比例拆分成三个数据集(train,dev,test)
+
+def splitset(datfile, lstScale=[7,2,1]):
+    '''将指定的数据文件（文本文件）按指定的比例拆分成三个数据集(train,dev,test)
     默认比例为 train:dev:test = 6:2:2 
     自动将文件保存到当前目录下；
-    参数：
-    返回：无
+    参数：datfile
+    返回：保存为 'train.tsv','dev.tsv','test.tsv'
     '''
     pass
     if len(lstScale)!=3:
         return -1
     txt = readtxtfile(datfile)
     lstLines = txt.splitlines()
     intLines = len(lstLines)-1
@@ -764,17 +789,16 @@
     for i in range (len(lstFile)):
         lstDat = lstLines[lstPos[i]+1:lstPos[i+1]+1]
         if lstDat:
             fName = './%s.tsv' % lstFile[i]
             savetofile(strFirstLine + '\n' + '\n'.join(lstDat),fName)
             print('%d  Lines data save to: %s' % (len(lstDat), fName) )
 
-def LabelCount (path,renfile = 0):
-    '''
-    统计目录下所有文件的label分布情况
+def LabelCount (path, renfile=0):
+    ''' 统计目录下所有文件的label分布情况
     '''
 
     pass
     lstF = getFiles(path)
     intTotalLines = 0
     intLabelLines = 0
 
@@ -905,15 +929,16 @@
                     print('%s 已存在，跳过。' % txtfile )
 
     finally:
         wordapp.Quit()
 
 
 def getFieldFromJson (obj, columns, mainname='items', subname=''):
-    ''' 从json格式中读取字段'''
+    ''' 从json格式中读取字段
+    '''
 
     # total = obj['result']['total']
     
     result = []
     if mainname:
         lstobj = obj['result'][mainname]
         for x in lstobj:
```

### Comparing `baselibs-0.1.1/LICENSE.txt` & `baselibs-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baselibs-0.1.1/PKG-INFO` & `baselibs-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: baselibs
-Version: 0.1.1
+Version: 0.1.2
 Summary: baselibs
 Home-page: https://github.com/xmxoxo/baselibs
 Author: He xi
 Author-email: xmhexi@qq.com
 License: UNKNOWN
 Project-URL: Blog, https://blog.csdn.net/xmxoxo
 Keywords: baselibs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 通用基础库 
 
-版本: v0.1
+版本: v0.1.1
 
 可对目录下的文件进行以下批量处理：
 
 * 清除空格 空行 按句子分行；
 * 删除空文件，找到后改名（改为"原文件名.del") 或者直接删除
 * 删除重复的文件:   根据文件的MD5判断文件是否相同，找到后改名（原文件.same)或者直接删除
 * 批量重命名:    可按序号进行重命名，默认从1开始，文件名会自动在前面补0，例如"0001.txt"
```

### Comparing `baselibs-0.1.1/README.md` & `baselibs-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 通用基础库 
 
-版本: v0.1
+版本: v0.1.1
 
 可对目录下的文件进行以下批量处理：
 
 * 清除空格 空行 按句子分行；
 * 删除空文件，找到后改名（改为"原文件名.del") 或者直接删除
 * 删除重复的文件:   根据文件的MD5判断文件是否相同，找到后改名（原文件.same)或者直接删除
 * 批量重命名:    可按序号进行重命名，默认从1开始，文件名会自动在前面补0，例如"0001.txt"
```

### Comparing `baselibs-0.1.1/setup.py` & `baselibs-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 # 导入静态文件
 file_data = []
 
 setuptools.setup(
     name='baselibs',
-    version='0.1.1',
+    version='0.1.2',
     description='baselibs',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords='baselibs',
     py_modules=['baselibs'],
     install_requires=[],
     # packages=setuptools.find_packages(),
@@ -33,14 +33,15 @@
         # 'Development Status :: 5 - Production/Stable'
         'Development Status :: 4 - Beta',  # 当前开发进度等级（测试版，正式版等）
         'Intended Audience :: Developers',  # 模块适用人群
         'Topic :: Software Development :: Code Generators',  # 给模块加话题标签
         'License :: OSI Approved :: MIT License',  # 模块的license
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
     ],
     project_urls={  # 项目相关的额外链接
         'Blog': 'https://blog.csdn.net/xmxoxo',
     },
     entry_points={}
 )
```

