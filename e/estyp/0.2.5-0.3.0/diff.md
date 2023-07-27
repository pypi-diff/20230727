# Comparing `tmp/estyp-0.2.5.tar.gz` & `tmp/estyp-0.3.0.tar.gz`

## Comparing `estyp-0.2.5.tar` & `estyp-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 estyp-0.2.5/estyp/linear_model/__init__.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 estyp-0.2.5/estyp/linear_model/stepwise.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 estyp-0.2.5/estyp/testing/__init__.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 estyp-0.2.5/estyp/testing/__base/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 estyp-0.2.5/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.2.5/LICENSE
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 estyp-0.2.5/README.md
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 estyp-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 estyp-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/__init__.py
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/linear_model/__init__.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/linear_model/stepwise/__init__.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/linear_model/stepwise/__base/__init__.py
+-rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/testing/__init__.py
+-rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 estyp-0.3.0/estyp/testing/__base/__init__.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 estyp-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 estyp-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 estyp-0.3.0/README.md
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 estyp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 estyp-0.3.0/PKG-INFO
```

### Comparing `estyp-0.2.5/estyp/linear_model/__init__.py` & `estyp-0.3.0/estyp/linear_model/__init__.py`

 * *Files identical despite different names*

### Comparing `estyp-0.2.5/estyp/linear_model/stepwise.py` & `estyp-0.3.0/estyp/linear_model/stepwise/__base/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,19 @@
-import statsmodels.api as sm
-import warnings
-from pandas import DataFrame
-warnings.filterwarnings("ignore")
+from scipy.stats import f as fisher
+from estyp.testing.__base import __nested_models_test
 
-def both_selection(formula: str, data: DataFrame, model: sm.GLM, max_iter = 10000) -> str:
-    """
-# Both Forward and Backward Variable Selection for GLM's
 
-This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC).
 
-## Parameters
 
-* `formula`: A string representing the initial model formula.
-* `data`: A Pandas DataFrame containing the data to be used for model fitting.
-* `model`: A statsmodels.GLM object that represents the type of model to be fit.
-* `max_iter`: The maximum number of iterations to perform.
-
-## Returns
-
-A string representing the final model formula.
-
-## Example
-
-```python
-import statsmodels.api as sm
-import pandas as pd
-
-data = pd.DataFrame({
-    "y": [1, 2, 3, 4, 5],
-    "x1": [1, 2, 3, 4, 5],
-    "x2": [6, 7, 8, 9, 10],
-})
-
-formula = "y ~ x1 + x2"
-
-model = sm.GLM
-
-final_formula = both_selection(formula=formula, data=data, model=model)
-
-print(final_formula)
-    """
+def __both_selection(formula, data, model, max_iter, **kwargs) -> str:
+    
     print("Este proceso tarda un buen tiempo ¡Paciencia! Momento de cuestionarte si eres feliz.")
     # Preparación
     fi = formula
-    e = model.from_formula(fi, data)
+    e = model.from_formula(fi, data, **kwargs)
     m = e.fit()
     preds = e.formula.split("+")
     vr = preds[0].split("~")[0].strip()
     preds[0] = preds[0].split("~")[1]
     preds = [x.strip() for x in preds]
     
     # Algoritmo
@@ -62,67 +28,103 @@
 
     for i in range(max_iter):
         if i == 0:
             aics = []
             for p in preds:
                 # Crear formula
                 p0 = d.drop(columns=[p, vr]).columns.tolist()
-                f0 = f"{vr} ~ {' + '.join(p0)}"
+                f0 = f"{vr} ~ {' + '.join(p0) if p0 else 1}"
                 # Ajustar modelo y extraer AIC
-                m0 = model.from_formula(f0, d).fit()
+                m0 = model.from_formula(f0, d, **kwargs).fit()
                 aics.append(m0.aic)
             aic0 = min(aics)
             id_min_aic = aics.index(min(aics))
             if aic0 < aicf:
                 var_min = preds[id_min_aic]
                 data0 = d.drop(columns=var_min)
                 preds0 = data0.drop(columns=vr).columns.tolist()
-                ff = f"{vr} ~ {' + '.join(preds0)}"
+                ff = f"{vr} ~ {' + '.join(preds0) if preds0 else 1}"
                 var_el.append(var_min)
             else:
                 print("No hay mejoras en el AIC, por lo que no se eliminarán variables.")
                 return fi
         else:
             aicf = aic0
             # Quitar variable
             aics_a = []
             for p in preds0:
                 p0 = data0.drop(columns=[p, vr]).columns.tolist()
-                f0 = f"{vr} ~ {' + '.join(p0)}"
-                m0 = model.from_formula(f0, d).fit()
+                f0 = f"{vr} ~ {' + '.join(p0) if p0 else 1}"
+                m0 = model.from_formula(f0, d, **kwargs).fit()
                 aics_a.append(m0.aic)
             # Añadir variable
             aics_b = []
             for p in preds:
-                f0 = f"{ff} + {p}"
-                m0 = model.from_formula(f0, d).fit()
-                aics_b.append(m0.aic)
+                f0 = f"{ff} {('+ ' + p) if p not in preds0 else ''}"
+                m0 = model.from_formula(f0, d, **kwargs).fit() if p not in preds0 else None
+                aics_b.append(m0.aic if p not in preds0 else aics_a[preds0.index(p)])
             min_a, min_b = min(aics_a), min(aics_b)
             aic0 = min_a if min_a < min_b else min_b
             if aic0 < aicf:
                 if min_a < min_b:
                     var_min = preds0[aics_a.index(min_a)]
                     data0.drop(columns=var_min, inplace=True)
                     preds0 = data0.drop(columns=vr).columns.tolist()
-                    ff = f"{vr} ~ {' + '.join(preds0)}"
+                    ff = f"{vr} ~ {' + '.join(preds0) if preds0 else 1}"
                     var_el.append(var_min)
                 else:
                     var_min = preds[aics_b.index(min_b)]
                     data0 = d[preds0 + [var_min, vr]]
                     preds0.append(var_min)
-                    ff = f"{vr} ~ {' + '.join(preds0)}"
+                    ff = f"{vr} ~ {' + '.join(preds0) if preds0 else 1}"
                     var_ag.append(var_min)
                 aicf = aic0
             else:
                 print("=========================")
                 print("|| Fin de la selección ||")
                 print("=========================")
                 print(f"AIC Obtenido: {aicf:0.2f}")
                 print("Variables eliminadas:", var_el if var_el else "Ninguna")
                 print("Variables agregadas:", var_ag if var_ag else "Ninguna")
-                print("Formula obtenida:", ff)
+                print("Fórmula obtenida:", ff)
                 return ff
         print(f"Iteración {i + 1} Finalizada | AIC Actual: {aic0:0.2f}")
         if not preds0:
             return f"{vr} + 1"
     print("Máximas iteraciones alcanzadas")
-    return ff
+    return ff
+
+
+def __forward_selection(y, data, model, alpha, **kwargs):
+    preds = data.columns.to_list()
+    preds.remove(y)
+
+    f_actual = f"{y} ~ 1"
+    m_actual = model.from_formula(f_actual, data, **kwargs).fit(disp=0)
+    termino = False
+    
+    while not termino:
+        valores_p = []
+        for p in preds:
+            f_prueba = f"{f_actual} + {p}"
+            m_prueba = model.from_formula(f_prueba, data, **kwargs).fit(disp=0)
+            pv = __nested_models_test(m_actual, m_prueba).p_value
+            valores_p.append(pv)
+        min_vp = min(valores_p)
+        if min_vp >= alpha:
+            termino = True
+            f_actual = f_actual.replace(" 1 +", "")
+            m_actual = model.from_formula(f_actual, data, **kwargs).fit(disp=0)
+        else:
+            var_min = preds[valores_p.index(min_vp)]
+            f_actual = f"{f_actual} + {var_min}"
+            m_actual = model.from_formula(f_actual, data, **kwargs).fit(disp=0)
+            preds.remove(var_min)
+            termino = False if preds else True
+            vp = f"{min_vp:0.4f}" if min_vp >= 0.0001 else "<0.0001"
+            print(f"Variable agregada: {var_min:30} | valor-p: {vp}")
+    print("=========================")
+    print("|| Fin de la selección ||")
+    print("=========================")
+    print("Fórmula obtenida:", f_actual)
+    return f_actual
+
```

### Comparing `estyp-0.2.5/.gitignore` & `estyp-0.3.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 
 # pdm
 #   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
 #pdm.lock
 #   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
 #   in version control.
 #   https://pdm.fming.dev/#use-with-ide
+.vscode/*
 .pdm.toml
 
 # PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
 __pypackages__/
 
 # Celery stuff
 celerybeat-schedule
```

### Comparing `estyp-0.2.5/LICENSE` & `estyp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `estyp-0.2.5/README.md` & `estyp-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
 ## Description
 
-This library is a collection of statistical functions for Python. It includes a function for performing stepwise with AIC criterion and a function for the F-ratio test.
+This library is a collection of statistical functions for Python.
 
 Actually, the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
 
 ## Changelog 
 
-### V0.2.5
+### V0.3.0
 
-* Added `scipy>=1.11.1` as a depedency of the library.
-* New modularization of the functions in the `testing` module.
-* R like documentation in the `testing.var_test()` function.
-* Added `testing.t_test()` function to perform t-test like in software R.
+* Changed `scipy>=1.11.1` to `scipy>=1.10.1` as a depedency of the library.
+* New modularization of the functions in the `linear_model` module.
+* Added `linear_model.stepwise.forward_selection()` function to perform forward variable selection based in p-values.
+* Added `testing.nested_models_test()` function to perform nested models testing.
+* Added option to specity aditional parameters of the model like `kwargs` in `linear_model.stepwise.forward_selection()` and `linear_model.stepwise.both_selection()` functions.  
+* Minor changes in the README.
 
 ## Functions
 
-* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression()` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
+* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `LogisticRegression()` class from `scikit-learn`, but adds additional methods for calculating confidence intervals, p-values, and model summaries like `Logit` class in `statsmodels`.
 * `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
-* `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
+* `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
 * `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the software R.
+* `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
+* `testing.nested_models_test()`: Performs a nested models test to compare two nested models using deviance criterion.
 
 # Installation
 
 To install this library, you can use pip:
 
 ```bash
 pip install estyp
```

### Comparing `estyp-0.2.5/pyproject.toml` & `estyp-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "estyp"
-version = "0.2.5"
+version = "0.3.0"
 authors = [
     { name="estebanrucan", email="errucan@gmail.com" },
 ]
 description = "Extended Statistical Toolkit Yet Practical"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9.12"
@@ -19,13 +19,13 @@
     "Development Status :: 1 - Planning"
 ]
 dependencies = [
     "numpy >= 1.22.3",
     "scikit-learn >= 1.2.1",
     "patsy >= 0.5.3",
     "statsmodels >= 0.13.5",
-    "scipy >= 1.11.1"
+    "scipy >= 1.10.1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/estebanrucan/estyp"
 "Bug Tracker" = "https://github.com/estebanrucan/estyp/issues"
```

### Comparing `estyp-0.2.5/PKG-INFO` & `estyp-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estyp
-Version: 0.2.5
+Version: 0.3.0
 Summary: Extended Statistical Toolkit Yet Practical
 Project-URL: Homepage, https://github.com/estebanrucan/estyp
 Project-URL: Bug Tracker, https://github.com/estebanrucan/estyp/issues
 Author-email: estebanrucan <errucan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Esteban Rucán Carrasco
@@ -31,41 +31,45 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9.12
 Requires-Dist: numpy>=1.22.3
 Requires-Dist: patsy>=0.5.3
 Requires-Dist: scikit-learn>=1.2.1
-Requires-Dist: scipy>=1.11.1
+Requires-Dist: scipy>=1.10.1
 Requires-Dist: statsmodels>=0.13.5
 Description-Content-Type: text/markdown
 
 # ESTYP: Extended Statistical Toolkit Yet Practical
 
 ## Description
 
-This library is a collection of statistical functions for Python. It includes a function for performing stepwise with AIC criterion and a function for the F-ratio test.
+This library is a collection of statistical functions for Python.
 
 Actually, the name comes from the way my friends call me (esty), plus the "p" which is the initial of `python`.
 
 ## Changelog 
 
-### V0.2.5
+### V0.3.0
 
-* Added `scipy>=1.11.1` as a depedency of the library.
-* New modularization of the functions in the `testing` module.
-* R like documentation in the `testing.var_test()` function.
-* Added `testing.t_test()` function to perform t-test like in software R.
+* Changed `scipy>=1.11.1` to `scipy>=1.10.1` as a depedency of the library.
+* New modularization of the functions in the `linear_model` module.
+* Added `linear_model.stepwise.forward_selection()` function to perform forward variable selection based in p-values.
+* Added `testing.nested_models_test()` function to perform nested models testing.
+* Added option to specity aditional parameters of the model like `kwargs` in `linear_model.stepwise.forward_selection()` and `linear_model.stepwise.both_selection()` functions.  
+* Minor changes in the README.
 
 ## Functions
 
-* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `sklearn.linear_model.LogisticRegression()` class, but adds additional methods for calculating confidence intervals, p-values, and model summaries.
+* `linear_model.LogisticRegression()`: This class implements a logistic regression model. It inherits from the `LogisticRegression()` class from `scikit-learn`, but adds additional methods for calculating confidence intervals, p-values, and model summaries like `Logit` class in `statsmodels`.
 * `linear_model.stepwise.both_selection()`: This function performs both forward and backward variable selection using the Akaike Information Criterion (AIC). 
-* `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
+* `linear_model.stepwise.forward_selection()`: This function performs forward variable selection based on p-values.
 * `testing.t_test()`: Performs one and two sample t-tests on groups of data. This function is inspired by the `t.test()` function of the software R.
+* `testing.var_test()`: Performs an F test to compare the variances of two samples from normal populations. This function is inspired by the `var.test()` function of the software R.
+* `testing.nested_models_test()`: Performs a nested models test to compare two nested models using deviance criterion.
 
 # Installation
 
 To install this library, you can use pip:
 
 ```bash
 pip install estyp
```

