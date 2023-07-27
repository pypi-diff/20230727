# Comparing `tmp/TensorFlow1-2.2.1.tar.gz` & `tmp/TensorFlow1-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TensorFlow1-2.2.1.tar", last modified: Thu Jul 27 18:56:19 2023, max compression
+gzip compressed data, was "TensorFlow1-2.2.4.tar", last modified: Thu Jul 27 19:07:38 2023, max compression
```

## Comparing `TensorFlow1-2.2.1.tar` & `TensorFlow1-2.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 18:56:19.536582 TensorFlow1-2.2.1/
--rw-rw-rw-   0        0        0      193 2023-07-27 18:56:19.536582 TensorFlow1-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-25 12:12:58.000000 TensorFlow1-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 18:56:19.520265 TensorFlow1-2.2.1/TensorFlow1/
--rw-rw-rw-   0        0        0    19024 2023-07-27 18:48:05.000000 TensorFlow1-2.2.1/TensorFlow1/TensorFlow.py
--rw-rw-rw-   0        0        0       40 2023-07-25 14:53:10.000000 TensorFlow1-2.2.1/TensorFlow1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 18:56:19.534187 TensorFlow1-2.2.1/TensorFlow1.egg-info/
--rw-rw-rw-   0        0        0      193 2023-07-27 18:56:19.000000 TensorFlow1-2.2.1/TensorFlow1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-07-27 18:56:19.000000 TensorFlow1-2.2.1/TensorFlow1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 18:56:19.000000 TensorFlow1-2.2.1/TensorFlow1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-27 18:56:19.000000 TensorFlow1-2.2.1/TensorFlow1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-07-25 12:13:11.000000 TensorFlow1-2.2.1/license.txt
--rw-rw-rw-   0        0        0      158 2023-07-27 18:56:19.541341 TensorFlow1-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0      304 2023-07-27 18:52:50.000000 TensorFlow1-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:07:38.353910 TensorFlow1-2.2.4/
+-rw-rw-rw-   0        0        0      193 2023-07-27 19:07:38.353910 TensorFlow1-2.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-25 12:12:58.000000 TensorFlow1-2.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 19:07:38.335433 TensorFlow1-2.2.4/TensorFlow1/
+-rw-rw-rw-   0        0        0    18353 2023-07-27 19:07:03.000000 TensorFlow1-2.2.4/TensorFlow1/TensorFlow.py
+-rw-rw-rw-   0        0        0       40 2023-07-25 14:53:10.000000 TensorFlow1-2.2.4/TensorFlow1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:07:38.351916 TensorFlow1-2.2.4/TensorFlow1.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-07-27 19:07:38.000000 TensorFlow1-2.2.4/TensorFlow1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-07-27 19:07:38.000000 TensorFlow1-2.2.4/TensorFlow1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 19:07:38.000000 TensorFlow1-2.2.4/TensorFlow1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-27 19:07:38.000000 TensorFlow1-2.2.4/TensorFlow1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-07-25 12:13:11.000000 TensorFlow1-2.2.4/license.txt
+-rw-rw-rw-   0        0        0      158 2023-07-27 19:07:38.355908 TensorFlow1-2.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      304 2023-07-27 19:07:13.000000 TensorFlow1-2.2.4/setup.py
```

### Comparing `TensorFlow1-2.2.1/TensorFlow1/TensorFlow.py` & `TensorFlow1-2.2.4/TensorFlow1/TensorFlow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,62 @@
 class mllab:
     def m1(self):
-        print('''   import pandas as pd
-                    import numpy as np
-                    import matplotlib.pyplot as plt
-                    import seaborn as sns
-                    #Reading the dataset
-                    dataset = pd.read_csv("tv.csv")
-                    #Setting the value for X and Y
-                    x = dataset[['TV']]
-                    y = dataset['Sales']
-                    #Splitting the dataset
-                    from sklearn.model_selection import train_test_split
-                    x_train, x_test, y_train, y_test = train_test_split(x, y, test_size =
-                    #Fitting the Linear Regression model
-                    from sklearn.linear_model import LinearRegression
-                    slr = LinearRegression()
-                    slr.fit(x_train, y_train)
-                    #Intercept and Coefficient
-                    print("Intercept: ", slr.intercept_)
-                    print("Coefficient: ", slr.coef_)
-                    ## Regression Equation: Sales = 6.948 + 0.054 * TV
-                    #Prediction of test set
-                    y_pred_slr= slr.predict(x_test)
-                    #Predicted values
-                    print("Prediction for test set: {}".format(y_pred_slr))
-                    #Actual value and the predicted value
-                    slr_diff = pd.DataFrame({'Actual value': y_test, 'Predicted value': y_pred_slr_diff.head()
-                    #Line of best fit
-                    plt.scatter(x_test,y_test)
-                    plt.plot(x_test, y_pred_slr, 'Red')
-                    plt.show()
-                    #Model Evaluation
-                    from sklearn import metrics
-                    meanAbErr = metrics.mean_absolute_error(y_test, y_pred_slr)
-                    meanSqErr = metrics.mean_squared_error(y_test, y_pred_slr)
-                    rootMeanSqErr = np.sqrt(metrics.mean_squared_error(y_test, y_pred_slr
-                    print('R squared: {:.2f}'.format(slr.score(x,y)*100))
-                    print('Mean Absolute Error:', meanAbErr)
-                    print('Mean Square Error:', meanSqErr)
-                    print('Root Mean Square Error:', rootMeanSqErr)''')
+        print('''   
+#Importing the libraries
+import pandas as pd
+import numpy as np
+import matplotlib.pyplot as plt
+import seaborn as sns
+
+#Reading the dataset
+dataset = pd.read_csv("Book1.csv")
+
+#Setting the value for X and Y
+x = dataset[['TV']]
+y = dataset['Sales']
+
+#Splitting the dataset
+from sklearn.model_selection import train_test_split
+x_train, x_test, y_train, y_test = train_test_split(x, y, test_size = 0.3, random_state = 100)
+
+#Fitting the Linear Regression model
+from sklearn.linear_model import LinearRegression
+slr = LinearRegression()  
+slr.fit(x_train, y_train)
+
+#Intercept and Coefficient
+print("Intercept: ", slr.intercept_)
+print("Coefficient: ", slr.coef_)
+
+
+## Regression Equation: Sales = 6.948 + 0.054 * TV
+
+#Prediction of test set
+y_pred_slr= slr.predict(x_test)
+#Predicted values
+print("Prediction for test set: {}".format(y_pred_slr))
+
+#Actual value and the predicted value
+slr_diff = pd.DataFrame({'Actual value': y_test, 'Predicted value': y_pred_slr})
+slr_diff.head()
+
+#Line of best fit
+plt.scatter(x_test,y_test)
+plt.plot(x_test, y_pred_slr, 'Red')
+plt.show()
+
+#Model Evaluation
+from sklearn import metrics
+meanAbErr = metrics.mean_absolute_error(y_test, y_pred_slr)
+meanSqErr = metrics.mean_squared_error(y_test, y_pred_slr)
+rootMeanSqErr = np.sqrt(metrics.mean_squared_error(y_test, y_pred_slr))
+print('R squared: {:.2f}'.format(slr.score(x,y)*100))
+print('Mean Absolute Error:', meanAbErr)
+print('Mean Square Error:', meanSqErr)
+print('Root Mean Square Error:', rootMeanSqErr)''')
     def m2(self):
         print('''
         import pandas as pd
         import numpy as np
         import matplotlib.pyplot as plt
         a=pd.read_csv('seattle-weather.csv')
         a
```

