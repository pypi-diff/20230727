# Comparing `tmp/quantfactortest-1.2.tar.gz` & `tmp/quantfactortest-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantfactortest-1.2.tar", last modified: Wed Jul 26 02:52:43 2023, max compression
+gzip compressed data, was "quantfactortest-1.3.tar", last modified: Thu Jul 27 03:17:13 2023, max compression
```

## Comparing `quantfactortest-1.2.tar` & `quantfactortest-1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 02:52:43.929515 quantfactortest-1.2/
--rw-rw-rw-   0        0        0      597 2023-07-26 02:52:43.928518 quantfactortest-1.2/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-07-19 02:18:20.000000 quantfactortest-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 02:52:43.928518 quantfactortest-1.2/quantfactortest.egg-info/
--rw-rw-rw-   0        0        0      597 2023-07-26 02:52:43.000000 quantfactortest-1.2/quantfactortest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-26 02:52:43.000000 quantfactortest-1.2/quantfactortest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 02:52:43.000000 quantfactortest-1.2/quantfactortest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-26 02:52:43.000000 quantfactortest-1.2/quantfactortest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-26 02:52:43.000000 quantfactortest-1.2/quantfactortest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    39995 2023-07-26 01:52:13.000000 quantfactortest-1.2/quantfactortest.py
--rw-rw-rw-   0        0        0       42 2023-07-26 02:52:43.929515 quantfactortest-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1353 2023-07-26 02:52:30.000000 quantfactortest-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:17:13.281663 quantfactortest-1.3/
+-rw-rw-rw-   0        0        0     7466 2023-07-27 03:17:13.280666 quantfactortest-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6874 2023-07-27 03:16:42.000000 quantfactortest-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 03:17:13.280666 quantfactortest-1.3/quantfactortest.egg-info/
+-rw-rw-rw-   0        0        0     7466 2023-07-27 03:17:13.000000 quantfactortest-1.3/quantfactortest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-27 03:17:13.000000 quantfactortest-1.3/quantfactortest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:17:13.000000 quantfactortest-1.3/quantfactortest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-27 03:17:13.000000 quantfactortest-1.3/quantfactortest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-27 03:17:13.000000 quantfactortest-1.3/quantfactortest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    40097 2023-07-27 02:32:49.000000 quantfactortest-1.3/quantfactortest.py
+-rw-rw-rw-   0        0        0       42 2023-07-27 03:17:13.281663 quantfactortest-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1371 2023-07-27 02:45:57.000000 quantfactortest-1.3/setup.py
```

### Comparing `quantfactortest-1.2/quantfactortest.py` & `quantfactortest-1.3/quantfactortest.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,14 +306,16 @@
                 df[str(i+1)+'分位'][7]=victory_rate
             print()
             print(df.T)
             self.group_picture(time_gap,factor)
             self.buy_and_sell(total_list,buy,sell,time_gap,factor)
     
     def IC_value(self,gap=10):
+        sns.set(palette="muted", color_codes=True)
+        sns.set(font='SimHei', font_scale=0.8)
         names=[]
         for i in self.periods:
             names.append('period_'+str(i))
 
         day_IC=pd.DataFrame(index=names)
         IC_mean=[]
         IC_std=[]
@@ -467,15 +469,15 @@
         self.exchange_rate()
         self.self_corr()
 
         
 
 
 class analyze_minute_factor:
-    def __init__(self,factor,price,minute,quantiles=5,periods=[1],demeaned=False,trade_day=[],trade_time=[]):
+    def __init__(self,factor,price,minute,quantiles=5,periods=[240],demeaned=False,trade_day=[],trade_time=[]):
         factor.replace(np.inf,np.nan,inplace=True)
         factor.index=pd.to_datetime(factor.index)
         price.index=pd.to_datetime(price.index)
         self.factor=factor
         self.price=price
         self.quantiles=quantiles
         self.periods=periods
```

### Comparing `quantfactortest-1.2/setup.py` & `quantfactortest-1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
  
 setup(
     name='quantfactortest',#包名
-    version='1.2',#版本
+    version='1.3',#版本
     description="单因子的测试（日级别and分钟级别）,非交互式",#包简介
-    long_description=open('README.md').read(),#读取文件中介绍包的详细内容
+    long_description=open('README.md', encoding='utf-8').read(),#读取文件中介绍包的详细内容
     include_package_data=True,#是否允许上传资源文件
     author='IDEA_Wenzhi',#作者
     author_email='1259429314@qq.com',#作者邮件
     maintainer='IDEA_Wenzhi',#维护者
     maintainer_email='1259429314@qq.com',#维护者邮件
     license='MIT License',#协议
     url='https://github.com/Masteryeda',#github或者自己的网站地址
```

