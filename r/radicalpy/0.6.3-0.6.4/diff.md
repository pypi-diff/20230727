# Comparing `tmp/radicalpy-0.6.3.tar.gz` & `tmp/radicalpy-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radicalpy-0.6.3.tar", last modified: Thu Jul 20 10:25:27 2023, max compression
+gzip compressed data, was "radicalpy-0.6.4.tar", last modified: Thu Jul 27 08:40:56 2023, max compression
```

## Comparing `radicalpy-0.6.3.tar` & `radicalpy-0.6.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.553914 radicalpy-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-20 10:25:08.000000 radicalpy-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-20 10:25:27.553914 radicalpy-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-20 10:25:08.000000 radicalpy-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-20 10:25:08.000000 radicalpy-0.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.549914 radicalpy-0.6.3/radicalpy/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4965 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/classical.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.553914 radicalpy-0.6.3/radicalpy/data/
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/constants.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.553914 radicalpy-0.6.3/radicalpy/data/molecules/
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/2_6_aqds.json
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/adenine_cation.json
--rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/flavin_anion.json
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/flavin_neutral.json
--rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/tryptophan_cation.json
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/molecules/tyrosine_neutral.json
--rw-r--r--   0 runner    (1001) docker     (122)    27847 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data/spin_data.json
--rw-r--r--   0 runner    (1001) docker     (122)    16112 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    20209 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/estimations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6365 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     9706 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/shared.py
--rw-r--r--   0 runner    (1001) docker     (122)    31601 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    11420 2023-07-20 10:25:08.000000 radicalpy-0.6.3/radicalpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.549914 radicalpy-0.6.3/radicalpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-20 10:25:27.000000 radicalpy-0.6.3/radicalpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-20 10:25:27.000000 radicalpy-0.6.3/radicalpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 10:25:27.000000 radicalpy-0.6.3/radicalpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-20 10:25:27.000000 radicalpy-0.6.3/radicalpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-20 10:25:27.000000 radicalpy-0.6.3/radicalpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-20 10:25:08.000000 radicalpy-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 10:25:27.553914 radicalpy-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 10:25:27.553914 radicalpy-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-07-20 10:25:08.000000 radicalpy-0.6.3/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-07-20 10:25:08.000000 radicalpy-0.6.3/tests/test_estimations.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-20 10:25:08.000000 radicalpy-0.6.3/tests/test_relaxations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-20 10:25:08.000000 radicalpy-0.6.3/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-20 10:25:08.000000 radicalpy-0.6.3/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.683224 radicalpy-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-27 08:40:45.000000 radicalpy-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-27 08:40:56.683224 radicalpy-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-27 08:40:45.000000 radicalpy-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-27 08:40:45.000000 radicalpy-0.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.679224 radicalpy-0.6.4/radicalpy/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7250 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/classical.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.683224 radicalpy-0.6.4/radicalpy/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/constants.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.683224 radicalpy-0.6.4/radicalpy/data/molecules/
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/2_6_aqds.json
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/adenine_cation.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/flavin_anion.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/flavin_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/tryptophan_cation.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/molecules/tyrosine_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (122)    27847 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data/spin_data.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16112 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20209 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/estimations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6365 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9706 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34500 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11420 2023-07-27 08:40:45.000000 radicalpy-0.6.4/radicalpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.683224 radicalpy-0.6.4/radicalpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-27 08:40:56.000000 radicalpy-0.6.4/radicalpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-27 08:40:56.000000 radicalpy-0.6.4/radicalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 08:40:56.000000 radicalpy-0.6.4/radicalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-27 08:40:56.000000 radicalpy-0.6.4/radicalpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-27 08:40:56.000000 radicalpy-0.6.4/radicalpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-27 08:40:45.000000 radicalpy-0.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 08:40:56.683224 radicalpy-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 08:40:56.683224 radicalpy-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-07-27 08:40:45.000000 radicalpy-0.6.4/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-07-27 08:40:45.000000 radicalpy-0.6.4/tests/test_estimations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-27 08:40:45.000000 radicalpy-0.6.4/tests/test_relaxations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-27 08:40:45.000000 radicalpy-0.6.4/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-27 08:40:45.000000 radicalpy-0.6.4/tests/test_simulation.py
```

### Comparing `radicalpy-0.6.3/LICENSE` & `radicalpy-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/PKG-INFO` & `radicalpy-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicalpy
-Version: 0.6.3
+Version: 0.6.4
 Summary: RadicalPy: a toolbox for radical pair spin dynamics
 Author-email: "Lewis M. Antill" <lewismantill@gmail.com>, Emil Vatai <emil.vatai@gmail.com>
 Maintainer-email: Emil Vatai <emil.vatai@gmail.com>, "Lewis M. Antill" <lewismantill@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Spin-Chemistry-Labs/radicalpy
 Project-URL: Documentation, https://radicalpy.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spin-Chemistry-Labs/radicalpy
```

### Comparing `radicalpy-0.6.3/README.md` & `radicalpy-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/pyproject.toml` & `radicalpy-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/data/constants.json` & `radicalpy-0.6.4/radicalpy/data/constants.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/data/molecules/flavin_anion.json` & `radicalpy-0.6.4/radicalpy/data/molecules/flavin_anion.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/data/molecules/flavin_neutral.json` & `radicalpy-0.6.4/radicalpy/data/molecules/flavin_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/data/molecules/tryptophan_cation.json` & `radicalpy-0.6.4/radicalpy/data/molecules/tryptophan_cation.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/data/molecules/tyrosine_neutral.json` & `radicalpy-0.6.4/radicalpy/data/molecules/tyrosine_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/data/spin_data.json` & `radicalpy-0.6.4/radicalpy/data/spin_data.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/data.py` & `radicalpy-0.6.4/radicalpy/data.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/estimations.py` & `radicalpy-0.6.4/radicalpy/estimations.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/kinetics.py` & `radicalpy-0.6.4/radicalpy/kinetics.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/plot.py` & `radicalpy-0.6.4/radicalpy/plot.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/relaxation.py` & `radicalpy-0.6.4/radicalpy/relaxation.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/shared.py` & `radicalpy-0.6.4/radicalpy/shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy/simulation.py` & `radicalpy-0.6.4/radicalpy/simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -616,27 +616,51 @@
         return self.convert(H)
 
     def time_evolution(
         self, init_state: State, time: np.ndarray, H: np.ndarray
     ) -> np.ndarray:
         """Evolve the system through time.
 
+        See also:
+
+        - `HilbertSimulation.unitary_propagator`
+        - `HilbertSimulation.propagate`
+        - `LiouvilleSimulation.unitary_propagator`
+        - `LiouvilleSimulation.propagate`
+
         Args:
-            init_state (State): blah blah
 
-            time (np.ndarray): blah blah
+            init_state (State): Initial `State` of the density matrix
+                (see `projection_operator`).
 
-            H (np.ndarray): blah blah
+            time (np.ndarray): An sequence of (uniform) time points,
+                usually created using `np.arange` or `np.linspace`.
+
+            H (np.ndarray): Hamiltonian operator.
 
         Returns:
             np.ndarray:
 
-                TODO
+                Return a sequence of density matrices evolved through
+                `time`, starting from a given initial `state` using
+                the Hamiltonian `H`.
+
+        Examples:
+
+            >>> molecules = [Molecule.fromdb("flavin_anion", ["N5"]),
+            ...              Molecule("Z")]
+            >>> sim = HilbertSimulation(molecules)
+            >>> H = sim.total_hamiltonian(B0=0, J=0, D=0)
+            >>> time = np.arange(0, 2e-6, 5e-9)
+            >>> time.shape
+            (400,)
+            >>> rhos = sim.time_evolution(State.SINGLET, time, H)
+            >>> rhos.shape
+            (400, 12, 12)
 
-        .. todo:: Write proper docs.
         """
         dt = time[1] - time[0]
         propagator = self.unitary_propagator(H, dt)
 
         rho0 = self.initial_density_matrix(init_state, H)
         rhos = np.zeros([len(time), *rho0.shape], dtype=complex)
         rhos[0] = rho0
@@ -856,27 +880,36 @@
             rho0 = Pi / np.trace(Pi)
         return rho0
 
     @staticmethod
     def unitary_propagator(H: np.ndarray, dt: float) -> np.ndarray:
         """Create unitary propagator (Hilbert space).
 
-        Create unitary propagator matrices for time evolution of the
-        spin Hamiltonian density matrix in Hilbert space.
+        Create unitary propagator matrices **U** and **U*** for time
+        evolution of the density matrix in Hilbert space (for the spin
+        Hamiltonian `H`).
+
+        .. math::
+            \mathbf{U}   =& \exp( -i \hat{H} t ) \\\\
+            \mathbf{U}^* =& \exp( +i \hat{H} t )
 
-        Arguments:
+        See also: `propagate` and `time_evolution`.
+
+        Args:
 
             H (np.ndarray): Spin Hamiltonian in Hilbert space.
 
             dt (float): Time evolution timestep.
 
         Returns:
             np.ndarray:
 
-                Two matrices (a tensor) in either Hilbert.
+                Two matrices (as tensor) in Hilbert space which are
+                used by the `propagate` method to perform a single
+                step in the `time_evolution` method.
 
         Examples:
 
             >>> molecules = [Molecule.fromdb("flavin_anion", ["N5"]),
             ...              Molecule("Z")]
             >>> sim = HilbertSimulation(molecules)
             >>> H = sim.total_hamiltonian(B0=0, J=0, D=0)
@@ -886,14 +919,38 @@
 
         """
         Up = sp.sparse.linalg.expm(1j * H * dt)
         Um = sp.sparse.linalg.expm(-1j * H * dt)
         return Up, Um
 
     def propagate(self, propagator: np.ndarray, rho: np.ndarray) -> np.ndarray:
+        """Propagate the density matrix (Hilbert space).
+
+        Propagates the density matrix using the propagator obtained
+        using the `unitary_propagator` method.
+
+        .. math::
+            \\rho (t) = \\mathbf{U} \\rho_0 \\mathbf{U}^*
+
+        See also: `unitary_propagator` and `time_evolution`.
+
+        Args:
+
+            propagator (np.ndarray): Unitary operator obtained via the
+                `unitary_propagator` method.
+
+            rho (np.ndarray): (Initial) density matrix.
+
+        Returns:
+            np.ndarray:
+
+                The new density matrix after the unitary operator was
+                applied to it.
+
+        """
         Up, Um = propagator
         return Um @ rho @ Up
 
     def observable_projection_operator(self, state: State) -> np.ndarray:
         return self.projection_operator(state)
 
 
@@ -940,38 +997,74 @@
             rho0 = np.reshape(rho0, (len(H) ** 2, 1))
         else:
             rho0 = Pi / np.vdot(Pi, Pi)
         return rho0
 
     @staticmethod
     def unitary_propagator(H, dt):
-        """Create unitary propagator.
+        """Create unitary propagator (Liouville space).
 
-        Create unitary propagator matrices for time evolution of the
-        spin Hamiltonian density matrix in Liouville space.
+        Create unitary propagator matrix **U** for the time evolution
+        of the density matrix in Liouville space (for the spin
+        Hamiltonian `H`).
+
+        .. math::
+            \mathbf{U} = \exp( \hat{\hat{L}} t )
+
+        See also: `propagate` and `time_evolution`.
+
+        Args:
+
+            H (np.ndarray): Spin Hamiltonian in Liouville space.
+
+            dt (float): Time evolution timestep.
+
+        Returns:
+            np.ndarray:
+
+                The matrix in Liouville space which is used by the
+                `propagate` method to perform a single step in the
+                `time_evolution` method.
 
         Examples:
 
             >>> molecules = [Molecule.fromdb("flavin_anion", ["N5"]),
             ...              Molecule("Z")]
             >>> sim = LiouvilleSimulation(molecules)
             >>> H = sim.total_hamiltonian(B0=0, J=0, D=0)
             >>> sim.unitary_propagator(H, 3e-9).shape
             (144, 144)
 
-        Arguments:
-            H (np.ndarray):
-
-                Spin Hamiltonian in Hilbert or Liouville space dt
-                (float): Time evolution timestep.  space (str): Select
-                the spin space.
-
         """
         return sp.sparse.linalg.expm(H * dt)
 
     def propagate(self, propagator: np.ndarray, rho: np.ndarray) -> np.ndarray:
+        """Propagate the density matrix (Liouville space).
+
+        Propagates the density matrix using the propagator obtained
+        using the `unitary_propagator` method.
+
+        .. math::
+            \\rho (t) = \\mathbf{U} \\rho_0
+
+        See also: `unitary_propagator` and `time_evolution`.
+
+        Args:
+
+            propagator (np.ndarray): Unitary operator obtained via the
+                `unitary_propagator` method.
+
+            rho (np.ndarray): (Initial) density matrix.
+
+        Returns:
+            np.ndarray:
+
+                The new density matrix after the unitary operator was
+                applied to it.
+
+        """
         return propagator @ rho
 
 
 class LiouvilleIncoherentProcessBase(HilbertIncoherentProcessBase):
     def adjust_hamiltonian(self, H: np.ndarray):
         H -= self.subH
```

### Comparing `radicalpy-0.6.3/radicalpy/utils.py` & `radicalpy-0.6.4/radicalpy/utils.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/radicalpy.egg-info/PKG-INFO` & `radicalpy-0.6.4/radicalpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicalpy
-Version: 0.6.3
+Version: 0.6.4
 Summary: RadicalPy: a toolbox for radical pair spin dynamics
 Author-email: "Lewis M. Antill" <lewismantill@gmail.com>, Emil Vatai <emil.vatai@gmail.com>
 Maintainer-email: Emil Vatai <emil.vatai@gmail.com>, "Lewis M. Antill" <lewismantill@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Spin-Chemistry-Labs/radicalpy
 Project-URL: Documentation, https://radicalpy.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spin-Chemistry-Labs/radicalpy
```

### Comparing `radicalpy-0.6.3/radicalpy.egg-info/SOURCES.txt` & `radicalpy-0.6.4/radicalpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/tests/test_data.py` & `radicalpy-0.6.4/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/tests/test_estimations.py` & `radicalpy-0.6.4/tests/test_estimations.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/tests/test_shared.py` & `radicalpy-0.6.4/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.3/tests/test_simulation.py` & `radicalpy-0.6.4/tests/test_simulation.py`

 * *Files identical despite different names*

