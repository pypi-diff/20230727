# Comparing `tmp/quant-alchemy-0.1.3.tar.gz` & `tmp/quant-alchemy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant-alchemy-0.1.3.tar", last modified: Wed Jul 26 21:50:32 2023, max compression
+gzip compressed data, was "quant-alchemy-0.1.4.tar", last modified: Thu Jul 27 00:37:12 2023, max compression
```

## Comparing `quant-alchemy-0.1.3.tar` & `quant-alchemy-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 21:50:32.930703 quant-alchemy-0.1.3/
--rw-rw-rw-   0        0        0      400 2023-07-26 21:50:32.930703 quant-alchemy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 21:50:32.923478 quant-alchemy-0.1.3/quant_alchemy/
--rw-rw-rw-   0        0        0       94 2023-07-26 18:55:50.000000 quant-alchemy-0.1.3/quant_alchemy/__init__.py
--rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.3/quant_alchemy/portfolio.py
--rw-rw-rw-   0        0        0    14668 2023-07-26 21:49:51.000000 quant-alchemy-0.1.3/quant_alchemy/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-07-26 21:50:32.928704 quant-alchemy-0.1.3/quant_alchemy.egg-info/
--rw-rw-rw-   0        0        0      400 2023-07-26 21:50:32.000000 quant-alchemy-0.1.3/quant_alchemy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-07-26 21:50:32.000000 quant-alchemy-0.1.3/quant_alchemy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 21:50:32.000000 quant-alchemy-0.1.3/quant_alchemy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-26 21:50:32.000000 quant-alchemy-0.1.3/quant_alchemy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 21:50:32.000000 quant-alchemy-0.1.3/quant_alchemy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 21:50:32.931705 quant-alchemy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-07-26 21:49:59.000000 quant-alchemy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 00:37:12.899590 quant-alchemy-0.1.4/
+-rw-rw-rw-   0        0        0      400 2023-07-27 00:37:12.899590 quant-alchemy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 00:37:12.894587 quant-alchemy-0.1.4/quant_alchemy/
+-rw-rw-rw-   0        0        0       94 2023-07-26 18:55:50.000000 quant-alchemy-0.1.4/quant_alchemy/__init__.py
+-rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.4/quant_alchemy/portfolio.py
+-rw-rw-rw-   0        0        0    14755 2023-07-27 00:35:53.000000 quant-alchemy-0.1.4/quant_alchemy/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-07-27 00:37:12.898588 quant-alchemy-0.1.4/quant_alchemy.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-07-27 00:37:12.000000 quant-alchemy-0.1.4/quant_alchemy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-07-27 00:37:12.000000 quant-alchemy-0.1.4/quant_alchemy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 00:37:12.000000 quant-alchemy-0.1.4/quant_alchemy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-27 00:37:12.000000 quant-alchemy-0.1.4/quant_alchemy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-27 00:37:12.000000 quant-alchemy-0.1.4/quant_alchemy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 00:37:12.899590 quant-alchemy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-07-27 00:37:04.000000 quant-alchemy-0.1.4/setup.py
```

### Comparing `quant-alchemy-0.1.3/quant_alchemy/portfolio.py` & `quant-alchemy-0.1.4/quant_alchemy/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant-alchemy-0.1.3/quant_alchemy/timeseries.py` & `quant-alchemy-0.1.4/quant_alchemy/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,26 +23,29 @@
         Calculate the simple returns of the time series data.
 
         Returns
         -------
         pandas.Series or pandas.DataFrame
             The simple returns of the time series data.
         """
-        return self.prices.pct_change()
+        returns = self.prices.pct_change()
+        returns = returns.dropna()
+
+        return returns
 
     def log_returns(self):
         """
         Calculate the logarithmic returns of the time series data.
 
         Returns
         -------
         pandas.Series or pandas.DataFrame
             The logarithmic returns of the time series data.
         """
-        return np.log(self.prices/self.prices.shift(1))
+        return np.log(self.prices / self.prices.shift(1))
 
     def volatility(self):
         """
         Calculate the volatility (standard deviation) of the returns of the time series data.
 
         Returns
         -------
@@ -261,19 +264,19 @@
         Calculates semideviation of the returns that are less than the provided threshold.
 
         Parameters:
             threshold (float, optional): The reference value below which a return is considered as underperforming. 
             Defaults to 0.0, meaning any negative return is considered underperforming.
 
         Returns:
-        float: The semideviation of the returns. This is computed as the square root of the 
-                average of the squared deviations of the underperforming returns from their mean.
-                The method uses a degrees of freedom (ddof) value of 1, implying that the function
-                computes sample standard deviation which is an unbiased estimator of the population 
-                standard deviation.
+            float: The semideviation of the returns. This is computed as the square root of the 
+                    average of the squared deviations of the underperforming returns from their mean.
+                    The method uses a degrees of freedom (ddof) value of 1, implying that the function
+                    computes sample standard deviation which is an unbiased estimator of the population 
+                    standard deviation.
         """
         returns = self.returns()
         return returns[returns < threshold].std(ddof=1)
 
     def var_historic(self, level=5):
         """
         This method calculates and returns the historic Value at Risk (VaR) at a specified level.
```

### Comparing `quant-alchemy-0.1.3/setup.py` & `quant-alchemy-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="quant-alchemy",
-    version="0.1.3",
+    version="0.1.4",
     author="Eladio Rocha Vizcaino",
     author_email="eladio.rocha99@gmail.com",
     description="Package for quantitative finance.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/EladioRocha/quant-alchemy",
     project_urls={
```

