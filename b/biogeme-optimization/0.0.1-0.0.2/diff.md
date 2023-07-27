# Comparing `tmp/biogeme_optimization-0.0.1.tar.gz` & `tmp/biogeme_optimization-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biogeme_optimization-0.0.1.tar", last modified: Fri Jul 14 11:49:03 2023, max compression
+gzip compressed data, was "biogeme_optimization-0.0.2.tar", last modified: Thu Jul 27 16:49:52 2023, max compression
```

## Comparing `biogeme_optimization-0.0.1.tar` & `biogeme_optimization-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-14 11:49:03.687442 biogeme_optimization-0.0.1/
--rw-r--r--   0 bierlair   (503) staff       (20)     3171 2023-07-14 11:49:03.687498 biogeme_optimization-0.0.1/PKG-INFO
--rw-r--r--   0 bierlair   (503) staff       (20)     2337 2023-07-03 14:06:53.000000 biogeme_optimization-0.0.1/README.md
--rw-r--r--   0 bierlair   (503) staff       (20)     1084 2023-07-14 11:49:03.687723 biogeme_optimization-0.0.1/setup.cfg
--rw-r--r--   0 bierlair   (503) staff       (20)       69 2023-06-21 07:47:31.000000 biogeme_optimization-0.0.1/setup.py
-drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-14 11:49:03.683269 biogeme_optimization-0.0.1/src/
-drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-14 11:49:03.685427 biogeme_optimization-0.0.1/src/biogeme_optimization/
--rw-r--r--   0 bierlair   (503) staff       (20)      105 2023-06-21 08:14:43.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/__init__.py
--rw-r--r--   0 bierlair   (503) staff       (20)     6589 2023-06-23 08:47:20.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/algebra.py
--rw-r--r--   0 bierlair   (503) staff       (20)     2790 2023-07-04 09:14:44.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/bfgs.py
--rw-r--r--   0 bierlair   (503) staff       (20)    32223 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/bounds.py
--rw-r--r--   0 bierlair   (503) staff       (20)      605 2023-07-03 14:01:16.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/diagnostics.py
--rw-r--r--   0 bierlair   (503) staff       (20)      203 2023-06-22 14:15:04.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/exceptions.py
--rw-r--r--   0 bierlair   (503) staff       (20)     2707 2023-07-04 14:20:02.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/format.py
--rw-r--r--   0 bierlair   (503) staff       (20)    12844 2023-07-08 15:15:57.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/function.py
--rw-r--r--   0 bierlair   (503) staff       (20)     6404 2023-07-08 15:16:05.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/hybrid_function.py
--rw-r--r--   0 bierlair   (503) staff       (20)    11130 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/linesearch.py
--rw-r--r--   0 bierlair   (503) staff       (20)     1851 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/logging.py
--rw-r--r--   0 bierlair   (503) staff       (20)     8473 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/neighborhood.py
--rw-r--r--   0 bierlair   (503) staff       (20)    14321 2023-07-10 06:02:44.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/pareto.py
--rw-r--r--   0 bierlair   (503) staff       (20)     9674 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/simple_bounds.py
--rw-r--r--   0 bierlair   (503) staff       (20)    20403 2023-07-08 15:17:14.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/trust_region.py
--rw-r--r--   0 bierlair   (503) staff       (20)     7961 2023-07-10 07:25:20.000000 biogeme_optimization-0.0.1/src/biogeme_optimization/vns.py
-drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-14 11:49:03.685973 biogeme_optimization-0.0.1/src/biogeme_optimization.egg-info/
--rw-r--r--   0 bierlair   (503) staff       (20)     3171 2023-07-14 11:49:03.000000 biogeme_optimization-0.0.1/src/biogeme_optimization.egg-info/PKG-INFO
--rw-r--r--   0 bierlair   (503) staff       (20)     1130 2023-07-14 11:49:03.000000 biogeme_optimization-0.0.1/src/biogeme_optimization.egg-info/SOURCES.txt
--rw-r--r--   0 bierlair   (503) staff       (20)        1 2023-07-14 11:49:03.000000 biogeme_optimization-0.0.1/src/biogeme_optimization.egg-info/dependency_links.txt
--rw-r--r--   0 bierlair   (503) staff       (20)       83 2023-07-14 11:49:03.000000 biogeme_optimization-0.0.1/src/biogeme_optimization.egg-info/requires.txt
--rw-r--r--   0 bierlair   (503) staff       (20)       21 2023-07-14 11:49:03.000000 biogeme_optimization-0.0.1/src/biogeme_optimization.egg-info/top_level.txt
-drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-14 11:49:03.687336 biogeme_optimization-0.0.1/tests/
--rw-r--r--   0 bierlair   (503) staff       (20)     6383 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.1/tests/test_algebra.py
--rw-r--r--   0 bierlair   (503) staff       (20)     3644 2023-06-24 16:11:17.000000 biogeme_optimization-0.0.1/tests/test_bfgs.py
--rw-r--r--   0 bierlair   (503) staff       (20)    28630 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.1/tests/test_bounds.py
--rw-r--r--   0 bierlair   (503) staff       (20)     2923 2023-07-03 12:35:53.000000 biogeme_optimization-0.0.1/tests/test_function.py
--rw-r--r--   0 bierlair   (503) staff       (20)     4592 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.1/tests/test_hybrid_function.py
--rw-r--r--   0 bierlair   (503) staff       (20)     9329 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.1/tests/test_linesearch.py
--rw-r--r--   0 bierlair   (503) staff       (20)     4928 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.1/tests/test_neighborhood.py
--rw-r--r--   0 bierlair   (503) staff       (20)     6436 2023-07-14 11:47:18.000000 biogeme_optimization-0.0.1/tests/test_pareto.py
--rw-r--r--   0 bierlair   (503) staff       (20)     9166 2023-07-03 13:09:42.000000 biogeme_optimization-0.0.1/tests/test_simple_bounds.py
--rw-r--r--   0 bierlair   (503) staff       (20)    21752 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.1/tests/test_trust_region.py
--rw-r--r--   0 bierlair   (503) staff       (20)     3674 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.1/tests/test_vns.py
+drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-27 16:49:52.644309 biogeme_optimization-0.0.2/
+-rw-r--r--   0 bierlair   (503) staff       (20)     3171 2023-07-27 16:49:52.644360 biogeme_optimization-0.0.2/PKG-INFO
+-rw-r--r--   0 bierlair   (503) staff       (20)     2337 2023-07-03 14:06:53.000000 biogeme_optimization-0.0.2/README.md
+-rw-r--r--   0 bierlair   (503) staff       (20)     1084 2023-07-27 16:49:52.644576 biogeme_optimization-0.0.2/setup.cfg
+-rw-r--r--   0 bierlair   (503) staff       (20)       69 2023-06-21 07:47:31.000000 biogeme_optimization-0.0.2/setup.py
+drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-27 16:49:52.639953 biogeme_optimization-0.0.2/src/
+drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-27 16:49:52.642122 biogeme_optimization-0.0.2/src/biogeme_optimization/
+-rw-r--r--   0 bierlair   (503) staff       (20)      105 2023-06-21 08:14:43.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/__init__.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     6589 2023-06-23 08:47:20.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/algebra.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     2790 2023-07-04 09:14:44.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/bfgs.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    32223 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/bounds.py
+-rw-r--r--   0 bierlair   (503) staff       (20)      605 2023-07-03 14:01:16.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/diagnostics.py
+-rw-r--r--   0 bierlair   (503) staff       (20)      203 2023-06-22 14:15:04.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/exceptions.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     2707 2023-07-04 14:20:02.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/format.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    12844 2023-07-08 15:15:57.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/function.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     6404 2023-07-08 15:16:05.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/hybrid_function.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    11130 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/linesearch.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     1851 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/logging.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     8540 2023-07-20 20:56:33.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/neighborhood.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    14134 2023-07-21 22:06:30.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/pareto.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     9681 2023-07-22 20:56:54.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/simple_bounds.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    20403 2023-07-08 15:17:14.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/trust_region.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     7986 2023-07-14 16:12:58.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/vns.py
+drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-27 16:49:52.642805 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/
+-rw-r--r--   0 bierlair   (503) staff       (20)     3171 2023-07-27 16:49:52.000000 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/PKG-INFO
+-rw-r--r--   0 bierlair   (503) staff       (20)     1130 2023-07-27 16:49:52.000000 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/SOURCES.txt
+-rw-r--r--   0 bierlair   (503) staff       (20)        1 2023-07-27 16:49:52.000000 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/dependency_links.txt
+-rw-r--r--   0 bierlair   (503) staff       (20)       83 2023-07-27 16:49:52.000000 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/requires.txt
+-rw-r--r--   0 bierlair   (503) staff       (20)       21 2023-07-27 16:49:52.000000 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/top_level.txt
+drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-27 16:49:52.644208 biogeme_optimization-0.0.2/tests/
+-rw-r--r--   0 bierlair   (503) staff       (20)     6383 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_algebra.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     3644 2023-06-24 16:11:17.000000 biogeme_optimization-0.0.2/tests/test_bfgs.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    28630 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_bounds.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     2923 2023-07-03 12:35:53.000000 biogeme_optimization-0.0.2/tests/test_function.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     4592 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_hybrid_function.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     9329 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_linesearch.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     4822 2023-07-27 16:37:09.000000 biogeme_optimization-0.0.2/tests/test_neighborhood.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     6436 2023-07-14 11:47:18.000000 biogeme_optimization-0.0.2/tests/test_pareto.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     9166 2023-07-03 13:09:42.000000 biogeme_optimization-0.0.2/tests/test_simple_bounds.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    21752 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_trust_region.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     3674 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_vns.py
```

### Comparing `biogeme_optimization-0.0.1/PKG-INFO` & `biogeme_optimization-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biogeme_optimization
-Version: 0.0.1
+Version: 0.0.2
 Summary: Various optimization algorithms for teaching and research
 Home-page: http://biogeme.epfl.ch
 Author: Michel Bierlaire
 Author-email: michel.bierlaire@epfl.ch
 Project-URL: Code, https://github.com/michelbierlaire/optimization
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `biogeme_optimization-0.0.1/README.md` & `biogeme_optimization-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/setup.cfg` & `biogeme_optimization-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = biogeme_optimization
-version = 0.0.1
+version = 0.0.2
 description = Various optimization algorithms for teaching and research
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Michel Bierlaire
 author_email = michel.bierlaire@epfl.ch
 url = http://biogeme.epfl.ch
 download_urls = https://pypi.org/project/bierlaire_optimization
```

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/algebra.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/algebra.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/bfgs.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/bfgs.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/bounds.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/diagnostics.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/diagnostics.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/format.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/format.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/function.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/function.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/hybrid_function.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/hybrid_function.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/linesearch.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/linesearch.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/logging.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/logging.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/neighborhood.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/neighborhood.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,25 @@
         """ Names of the operators """
 
         self.available = {k: True for k in operators}
         """ dict of availability of the operators """
 
         self.last_operator_name = None
 
+        # This quantity has been calculated to that if one operator
+        # has a score of 10, another has a score of -10, and all the
+        # others have a score of 1, the operator with the highest
+        # score is associated with a probability of about 0.9,
+        # irrespectively of the number of operators
+        self.scale = (
+            0.123184457025228 * np.log(float(len(self.scores)))
+            + 0.163017205688887
+        )
+        self.min_probability = 0.1 / len(self.scores)
+
     def increase_score_last_operator(self):
         """Increase the score of the last operator.
 
         :raise OptimizationError: if the operator is not known.
         """
         if self.last_operator_name not in self.scores:
             raise OptimizationError(f'Unknown operator: {self.last_operator_name}')
@@ -61,59 +72,60 @@
         :raise OptimizationError: if the operator is not known.
         """
         if self.last_operator_name not in self.scores:
             raise OptimizationError(f'Unknown operator: {self.last_operator_name}')
 
         self.scores[self.last_operator_name] -= 1
 
-    def probability_from_scores(self, min_probability=0.01, scale=0.1):
+    def probability_from_scores(self):
         """Calculates the probability from the scores
 
-        :param min_probability: minimum probability to select any
-                               operator. This is meant to avoid
-                               degeneracy, that is to have operators
-                               that have no chance to be chosen
-
-        :type min_probability: float
-
-        :param scale: parameter for the choice probability
-        :type scale: float
-
         :return: list of probabilities
         :rtype: list(float)
 
         :raise OptimizationError: if the minimum probability is too large
             for the number of operators. It must be less or equal to 1 /
             N, where N is the number of operators.
 
 
         """
-        if min_probability > 1.0 / len(self.scores):
+        if self.min_probability > 1.0 / len(self.scores):
             raise OptimizationError(
                 f'Cannot impose min. probability '
-                f'{min_probability} '
+                f'{self.min_probability} '
                 f'with {len(self.scores)} operators. '
                 f'Maximum is {1.0 / len(self.scores):.3f}.'
             )
 
         maxscore = max(list(self.scores.values()))
         list_of_scores = np.array(
             [
-                np.exp(scale * (s - maxscore)) if self.available[k] else 0
+                np.exp(self.scale * (s - maxscore)) if self.available[k] else 0
                 for k, s in self.scores.items()
             ]
         )
         if len(list_of_scores) == 0:
             return None
         total_score = sum(list_of_scores)
         prob = np.array([float(s) / float(total_score) for s in list_of_scores])
-        return self.enforce_minimum_probability(prob, min_probability)
+        return self.enforce_minimum_probability(prob, self.min_probability)
 
     @staticmethod
     def enforce_minimum_probability(prob, min_probability):
+        """
+        :param prob: vector of probabilities
+        :type prob: numpy.array
+        
+        :param min_probability: minimum probability to select any
+                               operator. This is meant to avoid
+                               degeneracy, that is to have operators
+                               that have no chance to be chosen
+        :type min_probability: float
+
+        """
         # Enforce minimum probability
         if not np.isclose(np.sum(prob), 1.0):
             error_msg = (
                 f'This is not a valid probability distribution as it '
                 f'does not sum up to one but to {np.sum(prob)}: {prob}'
             )
             raise OptimizationError(error_msg)
@@ -144,32 +156,22 @@
             raise OptimizationError(error_msg)
 
         total_high_scores = prob[ok].sum()
         prob[ok] = (1.0 - reserved_total) * prob[ok] / total_high_scores
         prob[update] = min_probability
         return prob
 
-    def select_operator(self, min_probability=0.01, scale=0.1):
+    def select_operator(self):
         """Select an operator based on the scores
 
-        :param min_probability: minimum probability to select any
-                               operator. This is meant to avoid
-                               degeneracy, that is to have operators
-                               that have no chance to be chosen
-
-        :type min_probability: float
-
-        :param scale: parameter for the choice probability
-        :type scale: float
-
         :return: name of the selected operator
         :rtype: str
 
         """
-        prob = self.probability_from_scores(min_probability, scale)
+        prob = self.probability_from_scores()
         self.last_operator_name = np.random.choice(self.names, 1, p=prob)[0]
         return self.operators[self.last_operator_name]
 
 
 class Neighborhood(metaclass=abc.ABCMeta):
     """
     Abstract class defining a problem
```

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/pareto.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/pareto.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,18 +332,15 @@
 
         :return: tuple of messages, possibly empty.
         :rtype: tuple(str)
         """
         if self.pareto is None:
             return tuple()
         msg = (
-            f'Initial Pareto: {self.size_init_pareto} ',
-            f'Initial considered: {self.size_init_considered} ',
-            f'Initial invalid: {self.size_init_invalid} ',
-            f'Final Pareto: {len(self.pareto)} ',
+            f'Pareto: {len(self.pareto)} ',
             f'Condidered: {len(self.considered)} ',
             f'Removed: {len(self.removed)}',
         )
         return msg
 
     def plot(
         self,
```

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/simple_bounds.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/simple_bounds.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         def logmessage():
             values_to_report = [k]
             if variable_names is not None:
                 values_to_report += list(iterate)
             values_to_report += [
                 current_function.function,
                 the_function.relgrad,
-                radius,
+                float(radius),
                 rho,
                 status,
             ]
             logger.info(the_formatter.formatted_row(values_to_report))
 
         # Solve the quadratic problem in the subspace defined by the GCP
         candidate, _ = bounds.truncated_conjugate_gradient_subspace(
```

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/trust_region.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/trust_region.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization/vns.py` & `biogeme_optimization-0.0.2/src/biogeme_optimization/vns.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
              pareto set and then removed, and the set of all models
              considered by the algorithm.
     :rtype: class :class:`biogeme.vns.ParetoClass`
 
     :raise OptimizationError: if the first Pareto set is empty.
 
     """
+    print('*** VNS ***')
     if first_solutions is not None:
         for solution in first_solutions:
             valid, why = problem.is_valid(solution)
             if valid:
                 pareto.add(solution)
                 logger.info(solution)
             else:
```

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization.egg-info/PKG-INFO` & `biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biogeme-optimization
-Version: 0.0.1
+Version: 0.0.2
 Summary: Various optimization algorithms for teaching and research
 Home-page: http://biogeme.epfl.ch
 Author: Michel Bierlaire
 Author-email: michel.bierlaire@epfl.ch
 Project-URL: Code, https://github.com/michelbierlaire/optimization
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `biogeme_optimization-0.0.1/src/biogeme_optimization.egg-info/SOURCES.txt` & `biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/tests/test_algebra.py` & `biogeme_optimization-0.0.2/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/tests/test_bfgs.py` & `biogeme_optimization-0.0.2/tests/test_bfgs.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/tests/test_bounds.py` & `biogeme_optimization-0.0.2/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/tests/test_function.py` & `biogeme_optimization-0.0.2/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/tests/test_hybrid_function.py` & `biogeme_optimization-0.0.2/tests/test_hybrid_function.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/tests/test_linesearch.py` & `biogeme_optimization-0.0.2/tests/test_linesearch.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/tests/test_neighborhood.py` & `biogeme_optimization-0.0.2/tests/test_neighborhood.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,41 +53,37 @@
         with self.assertRaises(OptimizationError):
             self.op_management.decrease_score_last_operator()
 
     def test_select_operator(self):
         # Mocking np.random.choice to always return 'operator1'
         chosen = ('operator1',)
         with patch('numpy.random.choice', return_value=chosen):
-            operator = self.op_management.select_operator(
-                min_probability=0.01, scale=0.1
-            )
+            operator = self.op_management.select_operator()
             self.assertEqual(operator, self.operators['operator1'])
 
     def test_select_operator_with_unavailable_operators(self):
         self.op_management.available['operator2'] = False
         # Mocking np.random.choice to always return 'operator1'
         chosen = ('operator1',)
         with patch('numpy.random.choice', return_value=chosen):
-            operator = self.op_management.select_operator(
-                min_probability=0.01, scale=0.1
-            )
+            operator = self.op_management.select_operator()
             self.assertEqual(operator, self.operators['operator1'])
 
     def test_select_operator_with_min_probability(self):
         # Mocking np.random.choice to always return 'operator1'
         chosen = ('operator1',)
         with patch('numpy.random.choice', return_value=chosen):
-            operator = self.op_management.select_operator(
-                min_probability=0.5, scale=0.1
-            )
+            self.op_management.min_probability = 0.5
+            operator = self.op_management.select_operator()
             self.assertEqual(operator, self.operators['operator1'])
 
     def test_select_operator_with_large_min_probability(self):
         with self.assertRaises(OptimizationError):
-            self.op_management.select_operator(min_probability=0.7, scale=0.1)
+            self.op_management.min_probability = 0.7
+            self.op_management.select_operator()
 
     def test_probability(self):
         self.op_management.available = [True, True, True]
         prob = np.array([0.0, 0.1, 0.45, 0.45])
         processed_prob = OperatorsManagement.enforce_minimum_probability(
             prob=prob, min_probability=0.2
         )
```

### Comparing `biogeme_optimization-0.0.1/tests/test_pareto.py` & `biogeme_optimization-0.0.2/tests/test_pareto.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/tests/test_simple_bounds.py` & `biogeme_optimization-0.0.2/tests/test_simple_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/tests/test_trust_region.py` & `biogeme_optimization-0.0.2/tests/test_trust_region.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.1/tests/test_vns.py` & `biogeme_optimization-0.0.2/tests/test_vns.py`

 * *Files identical despite different names*

