# Comparing `tmp/quantfactortest-1.3.tar.gz` & `tmp/quantfactortest-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantfactortest-1.3.tar", last modified: Thu Jul 27 03:17:13 2023, max compression
+gzip compressed data, was "quantfactortest-1.4.tar", last modified: Thu Jul 27 03:24:50 2023, max compression
```

## Comparing `quantfactortest-1.3.tar` & `quantfactortest-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 03:17:13.281663 quantfactortest-1.3/
--rw-rw-rw-   0        0        0     7466 2023-07-27 03:17:13.280666 quantfactortest-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6874 2023-07-27 03:16:42.000000 quantfactortest-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 03:17:13.280666 quantfactortest-1.3/quantfactortest.egg-info/
--rw-rw-rw-   0        0        0     7466 2023-07-27 03:17:13.000000 quantfactortest-1.3/quantfactortest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-27 03:17:13.000000 quantfactortest-1.3/quantfactortest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 03:17:13.000000 quantfactortest-1.3/quantfactortest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-27 03:17:13.000000 quantfactortest-1.3/quantfactortest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-27 03:17:13.000000 quantfactortest-1.3/quantfactortest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    40097 2023-07-27 02:32:49.000000 quantfactortest-1.3/quantfactortest.py
--rw-rw-rw-   0        0        0       42 2023-07-27 03:17:13.281663 quantfactortest-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1371 2023-07-27 02:45:57.000000 quantfactortest-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:24:50.178553 quantfactortest-1.4/
+-rw-rw-rw-   0        0        0     6701 2023-07-27 03:24:50.178553 quantfactortest-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6109 2023-07-27 03:23:34.000000 quantfactortest-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 03:24:50.176728 quantfactortest-1.4/quantfactortest.egg-info/
+-rw-rw-rw-   0        0        0     6701 2023-07-27 03:24:50.000000 quantfactortest-1.4/quantfactortest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-27 03:24:50.000000 quantfactortest-1.4/quantfactortest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:24:50.000000 quantfactortest-1.4/quantfactortest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-27 03:24:50.000000 quantfactortest-1.4/quantfactortest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-27 03:24:50.000000 quantfactortest-1.4/quantfactortest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    40097 2023-07-27 02:32:49.000000 quantfactortest-1.4/quantfactortest.py
+-rw-rw-rw-   0        0        0       42 2023-07-27 03:24:50.178553 quantfactortest-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1371 2023-07-27 03:23:49.000000 quantfactortest-1.4/setup.py
```

### Comparing `quantfactortest-1.3/PKG-INFO` & `quantfactortest-1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfactortest
-Version: 1.3
+Version: 1.4
 Summary: 单因子的测试（日级别and分钟级别）,非交互式
 Home-page: https://github.com/Masteryeda
 Author: IDEA_Wenzhi
 Author-email: 1259429314@qq.com
 Maintainer: IDEA_Wenzhi
 Maintainer-email: 1259429314@qq.com
 License: MIT License
@@ -81,66 +81,44 @@
 
     默认值为False，就是是否减去每一日的所有股票的平均收益（不是根据市值加权平均）。  
 
     如在周一的三只股票的收益为1%，2%，3%，如果demeaned=True，那么最后的结果将会为-1%，0%，1%。  
 
 
 ## 接下来将会解释结果：  
-
     请使用far.get_all(percentiles=[0.2,0.4,0.6,0.8],buy=[5],sell=[1],gap=10)  
 
     这里有额外的四个参数，我们将会在涉及到它们的结果中具体阐述用法。  
 
 
-1. 首先会输出一个有关于因子描述的dataframe，它会包含每一个分位的因子的情况。percentiles的参数就是为了更具体地展示某一个位置因子的大小。下图为在pyder里面显示的情况，使用的是默认参数。
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904274435198.png)
-
+1. 首先会输出一个有关于因子描述的dataframe，它会包含每一个分位的因子的情况。percentiles的参数就是为了更具体地展示某一个位置因子的大小。
 
 2. 接下来会展示IC（以及RankIC）的值以及IC（以及RankIC）的变化折线图，gap就是在作图的时候画的时间滚动平均线的周期，默认为10（2周）。
     
-    这是结果的具体展示。 
-    
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904277899124.png)
-
 3. 分组回测的相关情况。
 
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904275126169.png)
-
     然后会展示复利收益率各分组的折线图、累加收益率各分组的折线图；
 
-    ![Alt text](image.png)
-
     某一组的复利（以及累加）月度收益图，其目的是为了判断时间轮动（季节轮动）等。
 
-    ![Alt text](image-1.png)
-
     然后就和buy以及sell有关，buy=[5]和sell=[1]意味着我们做多第五分位和做空第一分位，资金的分配都是平均的。默认值是做多最大分位和做空最小分位。
 
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904275888881.png)
-
     然后是该策略的复利收益率的折线图
 
-    ![Alt text](image-2.png)
-
-
 4. 各分位以及各个周期的换手率，帮助我们判断策略的实现难度以及各种手续费。
     
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_1690427761896.png)
-
 5. 因子的自相关性系数，辅助判断第四条。
 
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_1690427663344.png)
-
-
 ## 以上就是日级别的回测，分钟级别的回测仅有稍微的变动，我将只阐述不一样的变化。
 far=analyze_minute_factor(factor,price,minute,quantiles=5,periods=[240],demeaned=False,trade_day=[],       trade_time=[])
 
 1. minute，请输入您的时间间隔。假如是5分钟，那么请输入5。
 
 2. periods，默认值为240。假设您的时间间隔为5，那么建议不要将交易周期低于240/5=48，因为240分钟=4小时是A股日内的交易时间，A股日内不允许买卖，所以请将periods设置的间隔大于240/minute 
 
 3. 因为baostock没有分钟级别的指数数据，所以我在此删掉了neutralize。
 
-4. trade_day和trade_time是用来计算收益率的。我要详细地表明它和periods的区别。如果我的minute是5，periods为48，那么我在周一的9:35的股票将会在周二的9:35再次交易，周一的9：40的股票将会在周二的9：40再次交易......
-如果trade_day为[1],trade_time为['15:00']，这意味着我统一在次日的15：00进行交易。也就是不管我是在周一的9:35买的还是10：00买的，我都会统一在周二的15：00进行交易来计算收益率。
+4. trade_day和trade_time是用来计算收益率的。我要详细地表明它和periods的区别。如果我的minute是5，periods为48，那么我在周一的9:35的股票将会在周二的9:35再次交易，周一的9：40的股票将会在周二的9：40再次交易......  
+
+    如果trade_day为[1],trade_time为['15:00']，这意味着我统一在次日的15：00进行交易。也就是不管我是在周一的9:35买的还是10：00买的，我都会统一在周二的15：00进行交易来计算收益率。
 
 5. 在最终的结果中，将不会再产生月度收益率图标。
```

### Comparing `quantfactortest-1.3/README.md` & `quantfactortest-1.4/quantfactortest.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: quantfactortest
+Version: 1.4
+Summary: 单因子的测试（日级别and分钟级别）,非交互式
+Home-page: https://github.com/Masteryeda
+Author: IDEA_Wenzhi
+Author-email: 1259429314@qq.com
+Maintainer: IDEA_Wenzhi
+Maintainer-email: 1259429314@qq.com
+License: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+
 # 请直接使用pip install quantfactortest安装。
 
 安装的时候有一个额外的包叫做baostock，它是用来获取指数收益率的（只有日频才有），其目的是用来计算超额收益率（在后面会有详细的说明）。  
 
 本单因子测试分为分钟级别（可以是1分钟、5分钟、10分钟不等）以及日级别（每天）。
 首先对日级别的做出参数上的解释。  
 
@@ -64,66 +81,44 @@
 
     默认值为False，就是是否减去每一日的所有股票的平均收益（不是根据市值加权平均）。  
 
     如在周一的三只股票的收益为1%，2%，3%，如果demeaned=True，那么最后的结果将会为-1%，0%，1%。  
 
 
 ## 接下来将会解释结果：  
-
     请使用far.get_all(percentiles=[0.2,0.4,0.6,0.8],buy=[5],sell=[1],gap=10)  
 
     这里有额外的四个参数，我们将会在涉及到它们的结果中具体阐述用法。  
 
 
-1. 首先会输出一个有关于因子描述的dataframe，它会包含每一个分位的因子的情况。percentiles的参数就是为了更具体地展示某一个位置因子的大小。下图为在pyder里面显示的情况，使用的是默认参数。
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904274435198.png)
-
+1. 首先会输出一个有关于因子描述的dataframe，它会包含每一个分位的因子的情况。percentiles的参数就是为了更具体地展示某一个位置因子的大小。
 
 2. 接下来会展示IC（以及RankIC）的值以及IC（以及RankIC）的变化折线图，gap就是在作图的时候画的时间滚动平均线的周期，默认为10（2周）。
     
-    这是结果的具体展示。 
-    
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904277899124.png)
-
 3. 分组回测的相关情况。
 
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904275126169.png)
-
     然后会展示复利收益率各分组的折线图、累加收益率各分组的折线图；
 
-    ![Alt text](image.png)
-
     某一组的复利（以及累加）月度收益图，其目的是为了判断时间轮动（季节轮动）等。
 
-    ![Alt text](image-1.png)
-
     然后就和buy以及sell有关，buy=[5]和sell=[1]意味着我们做多第五分位和做空第一分位，资金的分配都是平均的。默认值是做多最大分位和做空最小分位。
 
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904275888881.png)
-
     然后是该策略的复利收益率的折线图
 
-    ![Alt text](image-2.png)
-
-
 4. 各分位以及各个周期的换手率，帮助我们判断策略的实现难度以及各种手续费。
     
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_1690427761896.png)
-
 5. 因子的自相关性系数，辅助判断第四条。
 
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_1690427663344.png)
-
-
 ## 以上就是日级别的回测，分钟级别的回测仅有稍微的变动，我将只阐述不一样的变化。
 far=analyze_minute_factor(factor,price,minute,quantiles=5,periods=[240],demeaned=False,trade_day=[],       trade_time=[])
 
 1. minute，请输入您的时间间隔。假如是5分钟，那么请输入5。
 
 2. periods，默认值为240。假设您的时间间隔为5，那么建议不要将交易周期低于240/5=48，因为240分钟=4小时是A股日内的交易时间，A股日内不允许买卖，所以请将periods设置的间隔大于240/minute 
 
 3. 因为baostock没有分钟级别的指数数据，所以我在此删掉了neutralize。
 
-4. trade_day和trade_time是用来计算收益率的。我要详细地表明它和periods的区别。如果我的minute是5，periods为48，那么我在周一的9:35的股票将会在周二的9:35再次交易，周一的9：40的股票将会在周二的9：40再次交易......
-如果trade_day为[1],trade_time为['15:00']，这意味着我统一在次日的15：00进行交易。也就是不管我是在周一的9:35买的还是10：00买的，我都会统一在周二的15：00进行交易来计算收益率。
+4. trade_day和trade_time是用来计算收益率的。我要详细地表明它和periods的区别。如果我的minute是5，periods为48，那么我在周一的9:35的股票将会在周二的9:35再次交易，周一的9：40的股票将会在周二的9：40再次交易......  
+
+    如果trade_day为[1],trade_time为['15:00']，这意味着我统一在次日的15：00进行交易。也就是不管我是在周一的9:35买的还是10：00买的，我都会统一在周二的15：00进行交易来计算收益率。
 
-5. 在最终的结果中，将不会再产生月度收益率图标。
+5. 在最终的结果中，将不会再产生月度收益率图标。
```

### Comparing `quantfactortest-1.3/quantfactortest.egg-info/PKG-INFO` & `quantfactortest-1.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: quantfactortest
-Version: 1.3
-Summary: 单因子的测试（日级别and分钟级别）,非交互式
-Home-page: https://github.com/Masteryeda
-Author: IDEA_Wenzhi
-Author-email: 1259429314@qq.com
-Maintainer: IDEA_Wenzhi
-Maintainer-email: 1259429314@qq.com
-License: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-
 # 请直接使用pip install quantfactortest安装。
 
 安装的时候有一个额外的包叫做baostock，它是用来获取指数收益率的（只有日频才有），其目的是用来计算超额收益率（在后面会有详细的说明）。  
 
 本单因子测试分为分钟级别（可以是1分钟、5分钟、10分钟不等）以及日级别（每天）。
 首先对日级别的做出参数上的解释。  
 
@@ -81,66 +64,44 @@
 
     默认值为False，就是是否减去每一日的所有股票的平均收益（不是根据市值加权平均）。  
 
     如在周一的三只股票的收益为1%，2%，3%，如果demeaned=True，那么最后的结果将会为-1%，0%，1%。  
 
 
 ## 接下来将会解释结果：  
-
     请使用far.get_all(percentiles=[0.2,0.4,0.6,0.8],buy=[5],sell=[1],gap=10)  
 
     这里有额外的四个参数，我们将会在涉及到它们的结果中具体阐述用法。  
 
 
-1. 首先会输出一个有关于因子描述的dataframe，它会包含每一个分位的因子的情况。percentiles的参数就是为了更具体地展示某一个位置因子的大小。下图为在pyder里面显示的情况，使用的是默认参数。
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904274435198.png)
-
+1. 首先会输出一个有关于因子描述的dataframe，它会包含每一个分位的因子的情况。percentiles的参数就是为了更具体地展示某一个位置因子的大小。
 
 2. 接下来会展示IC（以及RankIC）的值以及IC（以及RankIC）的变化折线图，gap就是在作图的时候画的时间滚动平均线的周期，默认为10（2周）。
     
-    这是结果的具体展示。 
-    
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904277899124.png)
-
 3. 分组回测的相关情况。
 
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904275126169.png)
-
     然后会展示复利收益率各分组的折线图、累加收益率各分组的折线图；
 
-    ![Alt text](image.png)
-
     某一组的复利（以及累加）月度收益图，其目的是为了判断时间轮动（季节轮动）等。
 
-    ![Alt text](image-1.png)
-
     然后就和buy以及sell有关，buy=[5]和sell=[1]意味着我们做多第五分位和做空第一分位，资金的分配都是平均的。默认值是做多最大分位和做空最小分位。
 
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_16904275888881.png)
-
     然后是该策略的复利收益率的折线图
 
-    ![Alt text](image-2.png)
-
-
 4. 各分位以及各个周期的换手率，帮助我们判断策略的实现难度以及各种手续费。
     
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_1690427761896.png)
-
 5. 因子的自相关性系数，辅助判断第四条。
 
-    ![Alt text](%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_1690427663344.png)
-
-
 ## 以上就是日级别的回测，分钟级别的回测仅有稍微的变动，我将只阐述不一样的变化。
 far=analyze_minute_factor(factor,price,minute,quantiles=5,periods=[240],demeaned=False,trade_day=[],       trade_time=[])
 
 1. minute，请输入您的时间间隔。假如是5分钟，那么请输入5。
 
 2. periods，默认值为240。假设您的时间间隔为5，那么建议不要将交易周期低于240/5=48，因为240分钟=4小时是A股日内的交易时间，A股日内不允许买卖，所以请将periods设置的间隔大于240/minute 
 
 3. 因为baostock没有分钟级别的指数数据，所以我在此删掉了neutralize。
 
-4. trade_day和trade_time是用来计算收益率的。我要详细地表明它和periods的区别。如果我的minute是5，periods为48，那么我在周一的9:35的股票将会在周二的9:35再次交易，周一的9：40的股票将会在周二的9：40再次交易......
-如果trade_day为[1],trade_time为['15:00']，这意味着我统一在次日的15：00进行交易。也就是不管我是在周一的9:35买的还是10：00买的，我都会统一在周二的15：00进行交易来计算收益率。
+4. trade_day和trade_time是用来计算收益率的。我要详细地表明它和periods的区别。如果我的minute是5，periods为48，那么我在周一的9:35的股票将会在周二的9:35再次交易，周一的9：40的股票将会在周二的9：40再次交易......  
+
+    如果trade_day为[1],trade_time为['15:00']，这意味着我统一在次日的15：00进行交易。也就是不管我是在周一的9:35买的还是10：00买的，我都会统一在周二的15：00进行交易来计算收益率。
 
-5. 在最终的结果中，将不会再产生月度收益率图标。
+5. 在最终的结果中，将不会再产生月度收益率图标。
```

### Comparing `quantfactortest-1.3/quantfactortest.py` & `quantfactortest-1.4/quantfactortest.py`

 * *Files identical despite different names*

### Comparing `quantfactortest-1.3/setup.py` & `quantfactortest-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
  
 setup(
     name='quantfactortest',#包名
-    version='1.3',#版本
+    version='1.4',#版本
     description="单因子的测试（日级别and分钟级别）,非交互式",#包简介
     long_description=open('README.md', encoding='utf-8').read(),#读取文件中介绍包的详细内容
     include_package_data=True,#是否允许上传资源文件
     author='IDEA_Wenzhi',#作者
     author_email='1259429314@qq.com',#作者邮件
     maintainer='IDEA_Wenzhi',#维护者
     maintainer_email='1259429314@qq.com',#维护者邮件
```

