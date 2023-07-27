# Comparing `tmp/lqg-0.2.0.tar.gz` & `tmp/lqg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqg-0.2.0.tar", max compression
+gzip compressed data, was "lqg-0.2.1.tar", max compression
```

## Comparing `lqg-0.2.0.tar` & `lqg-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34523 2023-04-27 11:26:54.134688 lqg-0.2.0/LICENSE
--rw-r--r--   0        0        0     2675 2023-07-26 10:09:43.575186 lqg-0.2.0/README.md
--rw-r--r--   0        0        0      127 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/belief/__init__.py
--rw-r--r--   0        0        0      426 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/belief/kf.py
--rw-r--r--   0        0        0     2028 2023-04-27 11:26:54.148021 lqg-0.2.0/lqg/ccg.py
--rw-r--r--   0        0        0        0 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/control/__init__.py
--rw-r--r--   0        0        0     1243 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/control/glqr.py
--rw-r--r--   0        0        0     1078 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/control/lqr.py
--rw-r--r--   0        0        0     7298 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/glqg.py
--rw-r--r--   0        0        0      121 2023-04-27 11:26:54.148021 lqg-0.2.0/lqg/infer/__init__.py
--rw-r--r--   0        0        0     1758 2023-04-27 11:26:54.148021 lqg-0.2.0/lqg/infer/map.py
--rw-r--r--   0        0        0     1732 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/infer/mle.py
--rw-r--r--   0        0        0     2051 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/infer/models.py
--rw-r--r--   0        0        0     1764 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/infer/prior.py
--rw-r--r--   0        0        0     1908 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/infer/utils.py
--rw-r--r--   0        0        0     3014 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/io.py
--rw-r--r--   0        0        0     7846 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/lqg.py
--rw-r--r--   0        0        0     7607 2023-04-27 11:26:54.148021 lqg-0.2.0/lqg/optim.py
--rw-r--r--   0        0        0     1904 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/spec.py
--rw-r--r--   0        0        0      178 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/tracking/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-25 14:39:35.748708 lqg-0.2.0/lqg/tracking/basic.py
--rw-r--r--   0        0        0     2094 2023-07-25 14:39:35.748708 lqg-0.2.0/lqg/tracking/delay.py
--rw-r--r--   0        0        0     2824 2023-07-25 14:39:35.748708 lqg-0.2.0/lqg/tracking/signal_dependent.py
--rw-r--r--   0        0        0     1068 2023-07-25 14:39:35.748708 lqg-0.2.0/lqg/tracking/subjective.py
--rw-r--r--   0        0        0     1724 2023-07-25 14:39:35.748708 lqg-0.2.0/lqg/utils.py
--rw-r--r--   0        0        0      554 2023-07-25 14:39:35.755375 lqg-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 lqg-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-27 11:26:54.134688 lqg-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2675 2023-07-26 10:09:43.575186 lqg-0.2.1/README.md
+-rw-r--r--   0        0        0      127 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/belief/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/belief/kf.py
+-rw-r--r--   0        0        0     2028 2023-04-27 11:26:54.148021 lqg-0.2.1/lqg/ccg.py
+-rw-r--r--   0        0        0        0 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/control/__init__.py
+-rw-r--r--   0        0        0     1243 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/control/glqr.py
+-rw-r--r--   0        0        0     1078 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/control/lqr.py
+-rw-r--r--   0        0        0     7298 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/glqg.py
+-rw-r--r--   0        0        0      121 2023-04-27 11:26:54.148021 lqg-0.2.1/lqg/infer/__init__.py
+-rw-r--r--   0        0        0     1758 2023-04-27 11:26:54.148021 lqg-0.2.1/lqg/infer/map.py
+-rw-r--r--   0        0        0     1732 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/infer/mle.py
+-rw-r--r--   0        0        0     2058 2023-07-27 12:53:29.114840 lqg-0.2.1/lqg/infer/models.py
+-rw-r--r--   0        0        0     1764 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/infer/prior.py
+-rw-r--r--   0        0        0     1908 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/infer/utils.py
+-rw-r--r--   0        0        0     3014 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/io.py
+-rw-r--r--   0        0        0     7846 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/lqg.py
+-rw-r--r--   0        0        0     7607 2023-04-27 11:26:54.148021 lqg-0.2.1/lqg/optim.py
+-rw-r--r--   0        0        0     1904 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/spec.py
+-rw-r--r--   0        0        0      178 2023-07-25 14:39:35.745375 lqg-0.2.1/lqg/tracking/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-25 14:39:35.748708 lqg-0.2.1/lqg/tracking/basic.py
+-rw-r--r--   0        0        0     2094 2023-07-25 14:39:35.748708 lqg-0.2.1/lqg/tracking/delay.py
+-rw-r--r--   0        0        0     2824 2023-07-25 14:39:35.748708 lqg-0.2.1/lqg/tracking/signal_dependent.py
+-rw-r--r--   0        0        0     1068 2023-07-25 14:39:35.748708 lqg-0.2.1/lqg/tracking/subjective.py
+-rw-r--r--   0        0        0     1724 2023-07-25 14:39:35.748708 lqg-0.2.1/lqg/utils.py
+-rw-r--r--   0        0        0      554 2023-07-27 12:56:25.271663 lqg-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 lqg-0.2.1/PKG-INFO
```

### Comparing `lqg-0.2.0/LICENSE` & `lqg-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/README.md` & `lqg-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/ccg.py` & `lqg-0.2.1/lqg/ccg.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/control/glqr.py` & `lqg-0.2.1/lqg/control/glqr.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/control/lqr.py` & `lqg-0.2.1/lqg/control/lqr.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/glqg.py` & `lqg-0.2.1/lqg/glqg.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/infer/map.py` & `lqg-0.2.1/lqg/infer/map.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/infer/mle.py` & `lqg-0.2.1/lqg/infer/mle.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/infer/models.py` & `lqg-0.2.1/lqg/infer/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 params[name] = numpyro.param(name, jnp.array(default), constraint=dist.constraints.positive)
 
     for n in range(Nc):
         xn = x[n]
         # observation noise
         sigma_n = numpyro.param(f"sigma_target_{n}", jnp.array(1.), constraint=dist.constraints.positive)
 
-        lqg = model_type(process_noise=process_noise, dt=dt, T=T, sigma=sigma_n, **params)
+        lqg = model_type(process_noise=process_noise, dt=dt, T=T, sigma_target=sigma_n, **params)
 
         numpyro.sample(f"x_{n}",
                        lqg.conditional_distribution(xn).to_event(1),
                        obs=xn[:, 1:])
 
 default_prior = prior()
```

### Comparing `lqg-0.2.0/lqg/infer/prior.py` & `lqg-0.2.1/lqg/infer/prior.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/infer/utils.py` & `lqg-0.2.1/lqg/infer/utils.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/io.py` & `lqg-0.2.1/lqg/io.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/lqg.py` & `lqg-0.2.1/lqg/lqg.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/optim.py` & `lqg-0.2.1/lqg/optim.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/spec.py` & `lqg-0.2.1/lqg/spec.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/tracking/basic.py` & `lqg-0.2.1/lqg/tracking/basic.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/tracking/delay.py` & `lqg-0.2.1/lqg/tracking/delay.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/tracking/signal_dependent.py` & `lqg-0.2.1/lqg/tracking/signal_dependent.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/tracking/subjective.py` & `lqg-0.2.1/lqg/tracking/subjective.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/lqg/utils.py` & `lqg-0.2.1/lqg/utils.py`

 * *Files identical despite different names*

### Comparing `lqg-0.2.0/pyproject.toml` & `lqg-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lqg"
-version = "0.2.0"
+version = "0.2.1"
 description = "(Inverse) optimal control for linear-quadratic Gaussian systems"
 authors = ["Dominik Straub <dominikstrb@mailbox.org>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `lqg-0.2.0/PKG-INFO` & `lqg-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqg
-Version: 0.2.0
+Version: 0.2.1
 Summary: (Inverse) optimal control for linear-quadratic Gaussian systems
 License: AGPL-3.0-only
 Author: Dominik Straub
 Author-email: dominikstrb@mailbox.org
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

