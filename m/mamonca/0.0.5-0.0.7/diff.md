# Comparing `tmp/mamonca-0.0.5.tar.gz` & `tmp/mamonca-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamonca-0.0.5.tar", last modified: Thu Feb  9 16:46:36 2023, max compression
+gzip compressed data, was "mamonca-0.0.7.tar", last modified: Thu Jul 27 16:02:25 2023, max compression
```

## Comparing `mamonca-0.0.5.tar` & `mamonca-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-02-09 16:46:36.301615 mamonca-0.0.5/
--rw-r--r--   0 jovyan    (1000) users      (100)     1455 2023-02-08 14:55:46.000000 mamonca-0.0.5/LICENSE.md
--rw-r--r--   0 jovyan    (1000) users      (100)       92 2023-02-09 16:27:35.000000 mamonca-0.0.5/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)      242 2023-02-09 16:46:36.301615 mamonca-0.0.5/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     1269 2023-02-09 09:01:50.000000 mamonca-0.0.5/README.md
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-02-09 16:46:36.265613 mamonca-0.0.5/mamonca/
--rw-r--r--   0 jovyan    (1000) users      (100)    24922 2023-02-09 07:49:52.000000 mamonca-0.0.5/mamonca/cMC.cpp
--rw-r--r--   0 jovyan    (1000) users      (100)     6983 2023-02-08 22:51:22.000000 mamonca-0.0.5/mamonca/cMC.h
--rw-r--r--   0 jovyan    (1000) users      (100)     1454 2023-02-08 12:07:46.000000 mamonca-0.0.5/mamonca/cMC.pxd
--rw-r--r--   0 jovyan    (1000) users      (100)   421081 2023-02-09 16:28:14.000000 mamonca-0.0.5/mamonca/mc.cpp
--rw-r--r--   0 jovyan    (1000) users      (100)    14479 2023-02-09 07:49:52.000000 mamonca-0.0.5/mamonca/mc.pyx
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-02-09 16:46:36.293614 mamonca-0.0.5/mamonca.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)      242 2023-02-09 16:46:34.000000 mamonca-0.0.5/mamonca.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      251 2023-02-09 16:46:34.000000 mamonca-0.0.5/mamonca.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-02-09 16:46:34.000000 mamonca-0.0.5/mamonca.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        3 2023-02-09 16:46:34.000000 mamonca-0.0.5/mamonca.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) users      (100)      106 2023-02-09 16:46:36.309615 mamonca-0.0.5/setup.cfg
--rw-r--r--   0 jovyan    (1000) users      (100)      968 2023-02-09 16:46:02.000000 mamonca-0.0.5/setup.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-07-27 16:02:25.168359 mamonca-0.0.7/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1455 2023-07-27 16:02:05.000000 mamonca-0.0.7/LICENSE.md
+-rw-r--r--   0 jovyan    (1000) users      (100)       92 2023-07-27 16:02:05.000000 mamonca-0.0.7/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     1521 2023-07-27 16:02:25.168359 mamonca-0.0.7/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     1238 2023-07-27 16:02:05.000000 mamonca-0.0.7/README.md
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-07-27 16:02:25.064358 mamonca-0.0.7/mamonca/
+-rw-r--r--   0 jovyan    (1000) users      (100)    24838 2023-07-27 16:02:05.000000 mamonca-0.0.7/mamonca/cMC.cpp
+-rw-r--r--   0 jovyan    (1000) users      (100)     6935 2023-07-27 16:02:05.000000 mamonca-0.0.7/mamonca/cMC.h
+-rw-r--r--   0 jovyan    (1000) users      (100)     1454 2023-07-27 16:02:05.000000 mamonca-0.0.7/mamonca/cMC.pxd
+-rw-r--r--   0 jovyan    (1000) users      (100)   424520 2023-07-27 16:02:24.000000 mamonca-0.0.7/mamonca/mc.cpp
+-rw-r--r--   0 jovyan    (1000) users      (100)    14487 2023-07-27 16:02:05.000000 mamonca-0.0.7/mamonca/mc.pyx
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-07-27 16:02:25.100359 mamonca-0.0.7/mamonca.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1521 2023-07-27 16:02:24.000000 mamonca-0.0.7/mamonca.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      327 2023-07-27 16:02:24.000000 mamonca-0.0.7/mamonca.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-07-27 16:02:24.000000 mamonca-0.0.7/mamonca.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        6 2023-07-27 16:02:24.000000 mamonca-0.0.7/mamonca.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        8 2023-07-27 16:02:24.000000 mamonca-0.0.7/mamonca.egg-info/top_level.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)      106 2023-07-27 16:02:25.172359 mamonca-0.0.7/setup.cfg
+-rw-r--r--   0 jovyan    (1000) users      (100)      824 2023-07-27 16:02:05.000000 mamonca-0.0.7/setup.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-07-27 16:02:25.112359 mamonca-0.0.7/tests/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1451 2023-07-27 16:02:05.000000 mamonca-0.0.7/tests/test_heisenberg.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1358 2023-07-27 16:02:05.000000 mamonca-0.0.7/tests/test_landau.py
```

### Comparing `mamonca-0.0.5/LICENSE.md` & `mamonca-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mamonca-0.0.5/README.md` & `mamonca-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Magnetic Metropolis Monte Carlo following classical Boltzmann statistics
+# mamonca - interactive Magnetic Monte Carlo
 
 This code allows you to launch Metropolis Monte Carlo simulations via Heisenberg Landau models (with various polynomial degrees) from a jupyter notebook.
 
 ## How to compile
 
 Download all files and run `python setup.py build_ext --inplace`.
 
@@ -29,8 +29,7 @@
 
 mc.run(temperature=300, number_of_iterations=1000)
 ```
 
 ## How to set inputs and get outputs
 
 As a rule of thumb, you can set all input parameters via functions starting with `set_`. Similarly, output values can be obtained via functions whose names start with `get_`. Take a look at the list of auto-complete and see their docstrings
-
```

### Comparing `mamonca-0.0.5/mamonca/cMC.cpp` & `mamonca-0.0.7/mamonca/cMC.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -61,35 +61,35 @@
 }
 
 valarray<double> Square::gradient(valarray<double> &m){
     return 2.*m;
 }
 
 valarray<double> Quartic::gradient(valarray<double> &m){
-    return 4*m.apply([](double x){return x*x;}).sum()*m;
+    return 4.*m.apply([](double x){return x*x;}).sum()*m;
 }
 
 valarray<double> Sextic::gradient(valarray<double> &m){
-    return 6*m.apply([](double x){return x*x*x*x;}).sum()*m;
+    return 6.*m.apply([](double x){return x*x*x*x;}).sum()*m;
 }
 
 valarray<double> Octic::gradient(valarray<double> &m){
-    return 8*m.apply([](double x){return x*x*x*x*x*x;}).sum()*m;
+    return 8.*m.apply([](double x){return x*x*x*x*x*x;}).sum()*m;
 }
 
 valarray<double> Decic::gradient(valarray<double> &m){
-    return 10*m.apply([](double x){return x*x*x*x*x*x*x*x;}).sum()*m;
+    return 10.*m.apply([](double x){return x*x*x*x*x*x*x*x;}).sum()*m;
 }
 
 double Product::value(Atom &neigh, Atom &me){
-    return 0;
+    return 0.;
 }
 
 double Product::diff(Atom &neigh, Atom &me){
-    return 0;
+    return 0.;
 }
 
 valarray<double> Product::gradient(Atom &neigh, Atom &me){
     return 0.*neigh.m;
 }
 
 double J_lin_lin::value(Atom &neigh, Atom &me){
@@ -151,15 +151,15 @@
 void Atom::activate_debug(){
     debug = true;
 }
 
 double Atom::get_acceptance_ratio(){
     if(count!=0)
         return acc/(double) count;
-    return 0;
+    return 0.;
 }
 
 double Atom::get_magnitude(int exponent, bool old)
 {
     if(old)
         return power(mabs_tmp, exponent);
     else
@@ -284,28 +284,28 @@
     landau_coeff[index].clear();
     landau_func[index].clear();
 }
 
 void Atom::propose_new_state(){
     set_m(rand_generator.on_sphere(3), true);
     if(flip && rand()%2==1)
-        m *= -1;
+        m *= -1.;
 }
 
 valarray<double> Atom::delta_m(){
     return m-m_tmp;
 }
 
 void Atom::rescale_magnitude(double rescale_m, double rescale_phi){
     if (rescale_m==1 && dm>0)
-        dm = 1;
+        dm = 1.;
     else
         dm *= rescale_m;
     if (rescale_phi==1 && dphi>0)
-        dphi = 1;
+        dphi = 1.;
     else
         dphi *= rescale_phi;
 }
 
 void Atom::set_magnitude(double ddm, double ddphi, bool flip_in)
 {
     if(ddm<0 || ddphi<0)
@@ -498,21 +498,18 @@
     if(lambda>=0)
         return true;
     return false;
 }
 
 void cMC::run_spin_dynamics(double kBT, int threads){
     double mu_s = sqrt(2*constants.damping_parameter*constants.hbar*kBT/constants.delta_t);
-    #pragma omp parallel num_threads(threads)
     {
-        #pragma omp for
         for (int i=0; i<n_tot; i++)
             atom[i].calc_spin_dynamics(
                 constants.damping_parameter, constants.delta_t, mu_s, lambda);
-        #pragma omp for
         for (int i=0; i<n_tot; i++)
             atom[i].update_spin_dynamics();
     }
     E_tot.add(get_energy(0), true);
     if(thermodynamic_integration())
         E_tot.add(get_energy(1), true);
     reset_magnetization();
```

### Comparing `mamonca-0.0.5/mamonca/cMC.h` & `mamonca-0.0.7/mamonca/cMC.h`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 #include <cstdlib>
 #include <ctime>
 #include <valarray>
 #include <chrono>
 #include <numeric>
 #include <random>
-#include <omp.h>
 #include <string>
 
 using namespace std;
 
 double power(double, int);
 double m_norm(valarray<double>);
 valarray<double> m_cross(valarray<double>&, valarray<double>);
@@ -50,15 +49,15 @@
         vector<Product*> heisen_func[2];
         vector<Atom*> neigh[2];
         int acc, count;
         // This does not work when neighbors change their m
         struct UpToDate{
             vector<bool> E, dE;
         } up_to_date;
-        bool E_uptodate[2], dE_uptodate[2], debug, flip;
+        bool debug, flip;
         void update_flag(bool ff=false);
         friend Product;
     public:
         void calc_spin_dynamics(double, double, double, double); // gamma, delta_t, mu_s, lambda
         void update_spin_dynamics();
         valarray<double> m, m_tmp;
         valarray<double> get_gradient(double); // lambda
```

### Comparing `mamonca-0.0.5/mamonca/cMC.pxd` & `mamonca-0.0.7/mamonca/cMC.pxd`

 * *Files identical despite different names*

### Comparing `mamonca-0.0.5/mamonca/mc.cpp` & `mamonca-0.0.7/mamonca/mc.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "depends": [],
+        "depends": [
+            "mamonca/cMC.cpp",
+            "mamonca/cMC.h"
+        ],
         "extra_compile_args": [
-            "-fopenmp"
+            "-std=c++11"
         ],
-        "extra_link_args": [
-            "-lgomp"
+        "include_dirs": [
+            "./mamonca"
         ],
         "language": "c++",
-        "name": "mc",
+        "name": "mamonca",
         "sources": [
             "mamonca/mc.pyx"
         ]
     },
-    "module_name": "mc"
+    "module_name": "mamonca"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -219,15 +222,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -258,15 +261,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -768,16 +771,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__mc
-#define __PYX_HAVE_API__mc
+#define __PYX_HAVE__mamonca
+#define __PYX_HAVE_API__mamonca
 /* Early includes */
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
 #include "cMC.cpp"
@@ -992,24 +995,24 @@
 
 static const char *__pyx_f[] = {
   "mamonca/mc.pyx",
   "stringsource",
 };
 
 /*--- Type declarations ---*/
-struct __pyx_obj_2mc_MC;
+struct __pyx_obj_7mamonca_MC;
 
-/* "mc.pyx":7
+/* "mamonca/mc.pyx":7
  * import numpy as np
  * 
  * cdef class MC:             # <<<<<<<<<<<<<<
  *     """
  * 
  */
-struct __pyx_obj_2mc_MC {
+struct __pyx_obj_7mamonca_MC {
   PyObject_HEAD
   cMC c_mc;
 };
 
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
@@ -1450,26 +1453,26 @@
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
 /* Module declarations from 'libcpp.vector' */
 
-/* Module declarations from 'cMC' */
+/* Module declarations from 'mamonca.cMC' */
 
-/* Module declarations from 'mc' */
-static PyTypeObject *__pyx_ptype_2mc_MC = 0;
+/* Module declarations from 'mamonca' */
+static PyTypeObject *__pyx_ptype_7mamonca_MC = 0;
 static std::vector<double>  __pyx_convert_vector_from_py_double(PyObject *); /*proto*/
 static std::vector<int>  __pyx_convert_vector_from_py_int(PyObject *); /*proto*/
 static PyObject *__pyx_convert_vector_to_py_double(const std::vector<double>  &); /*proto*/
-#define __Pyx_MODULE_NAME "mc"
-extern int __pyx_module_is_main_mc;
-int __pyx_module_is_main_mc = 0;
+#define __Pyx_MODULE_NAME "mamonca"
+extern int __pyx_module_is_main_mamonca;
+int __pyx_module_is_main_mamonca = 0;
 
-/* Implementation of 'mc' */
+/* Implementation of 'mamonca' */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_range;
 static const char __pyx_k_C[] = "C";
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_j[] = "j";
 static const char __pyx_k_MC[] = "MC";
@@ -1627,43 +1630,43 @@
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_threads;
 static PyObject *__pyx_n_s_tile;
 static PyObject *__pyx_n_s_tolist;
 static PyObject *__pyx_n_s_turn_on;
 static PyObject *__pyx_n_s_use_derivative;
 static PyObject *__pyx_n_s_where;
-static int __pyx_pf_2mc_2MC___cinit__(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_number_of_atoms); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_2set_landau_coeff(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_coeff, PyObject *__pyx_v_deg, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_4set_heisenberg_coeff(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_coeff, PyObject *__pyx_v_i, PyObject *__pyx_v_j, PyObject *__pyx_v_deg, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_6clear_heisenberg_coeff(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_8clear_landau_coeff(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_10clear_all_coeff(struct __pyx_obj_2mc_MC *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_12get_magnetic_gradients(struct __pyx_obj_2mc_MC *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_14get_magnetic_moments(struct __pyx_obj_2mc_MC *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_16set_magnetic_moments(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_magmoms); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_18get_magnetization(struct __pyx_obj_2mc_MC *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_20get_output(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_22run(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_temperature, PyObject *__pyx_v_number_of_iterations, PyObject *__pyx_v_reset, PyObject *__pyx_v_threads); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_24get_acceptance_ratio(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_individual); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_26get_energy(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_28get_mean_energy(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_30get_energy_variance(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_32revoke_qmc(struct __pyx_obj_2mc_MC *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_34set_lambda(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_36select_id(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_indices); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_38get_steps_per_second(struct __pyx_obj_2mc_MC *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_40set_magnitude(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_dm, PyObject *__pyx_v_dphi, PyObject *__pyx_v_flip); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_42run_gradient_descent(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_max_iter, PyObject *__pyx_v_step_size, PyObject *__pyx_v_decrement, PyObject *__pyx_v_diff); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_44set_metadynamics(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_max_range, PyObject *__pyx_v_energy_increment, PyObject *__pyx_v_length_scale, PyObject *__pyx_v_bins, PyObject *__pyx_v_cutoff, PyObject *__pyx_v_use_derivative); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_46get_metadynamics_free_energy(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_derivative); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_48switch_spin_dynamics(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_turn_on, PyObject *__pyx_v_damping_parameter, PyObject *__pyx_v_delta_t, PyObject *__pyx_v_rescale_mag); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_50activate_debug(struct __pyx_obj_2mc_MC *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_52__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2mc_MC *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_2mc_2MC_54__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2mc_MC *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_2mc_MC(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static int __pyx_pf_7mamonca_2MC___cinit__(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_number_of_atoms); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_2set_landau_coeff(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_coeff, PyObject *__pyx_v_deg, PyObject *__pyx_v_index); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_4set_heisenberg_coeff(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_coeff, PyObject *__pyx_v_i, PyObject *__pyx_v_j, PyObject *__pyx_v_deg, PyObject *__pyx_v_index); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_6clear_heisenberg_coeff(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_8clear_landau_coeff(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_10clear_all_coeff(struct __pyx_obj_7mamonca_MC *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_12get_magnetic_gradients(struct __pyx_obj_7mamonca_MC *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_14get_magnetic_moments(struct __pyx_obj_7mamonca_MC *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_16set_magnetic_moments(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_magmoms); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_18get_magnetization(struct __pyx_obj_7mamonca_MC *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_20get_output(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_22run(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_temperature, PyObject *__pyx_v_number_of_iterations, PyObject *__pyx_v_reset, PyObject *__pyx_v_threads); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_24get_acceptance_ratio(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_individual); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_26get_energy(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_28get_mean_energy(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_30get_energy_variance(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_32revoke_qmc(struct __pyx_obj_7mamonca_MC *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_34set_lambda(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_val); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_36select_id(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_indices); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_38get_steps_per_second(struct __pyx_obj_7mamonca_MC *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_40set_magnitude(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_dm, PyObject *__pyx_v_dphi, PyObject *__pyx_v_flip); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_42run_gradient_descent(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_max_iter, PyObject *__pyx_v_step_size, PyObject *__pyx_v_decrement, PyObject *__pyx_v_diff); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_44set_metadynamics(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_max_range, PyObject *__pyx_v_energy_increment, PyObject *__pyx_v_length_scale, PyObject *__pyx_v_bins, PyObject *__pyx_v_cutoff, PyObject *__pyx_v_use_derivative); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_46get_metadynamics_free_energy(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_derivative); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_48switch_spin_dynamics(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_turn_on, PyObject *__pyx_v_damping_parameter, PyObject *__pyx_v_delta_t, PyObject *__pyx_v_rescale_mag); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_50activate_debug(struct __pyx_obj_7mamonca_MC *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_52__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7mamonca_MC *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7mamonca_2MC_54__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7mamonca_MC *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_tp_new_7mamonca_MC(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_float_0_1;
 static PyObject *__pyx_float_1eneg_3;
 static PyObject *__pyx_float_0_001;
 static PyObject *__pyx_float_1_0eneg_3;
 static PyObject *__pyx_float_1_0eneg_8;
 static PyObject *__pyx_float_8_0eneg_3;
 static PyObject *__pyx_int_0;
@@ -1681,25 +1684,25 @@
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
 /* Late includes */
 
-/* "mc.pyx":44
+/* "mamonca/mc.pyx":44
  *     cdef MCcpp c_mc
  * 
  *     def __cinit__(self, number_of_atoms):             # <<<<<<<<<<<<<<
  *         """
  *         args:
  */
 
 /* Python wrapper */
-static int __pyx_pw_2mc_2MC_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_2mc_2MC_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_7mamonca_2MC_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_7mamonca_2MC_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_number_of_atoms = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
@@ -1731,80 +1734,80 @@
     }
     __pyx_v_number_of_atoms = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 44, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC___cinit__(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_number_of_atoms);
+  __pyx_r = __pyx_pf_7mamonca_2MC___cinit__(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_number_of_atoms);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_2mc_2MC___cinit__(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_number_of_atoms) {
+static int __pyx_pf_7mamonca_2MC___cinit__(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_number_of_atoms) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "mc.pyx":49
+  /* "mamonca/mc.pyx":49
  *             number_of_atoms (int): number of atoms
  *         """
  *         self.c_mc.create_atoms(number_of_atoms)             # <<<<<<<<<<<<<<
  * 
  *     def set_landau_coeff(self, coeff, deg, index=0):
  */
   __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_number_of_atoms); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L1_error)
   try {
     __pyx_v_self->c_mc.create_atoms(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 49, __pyx_L1_error)
   }
 
-  /* "mc.pyx":44
+  /* "mamonca/mc.pyx":44
  *     cdef MCcpp c_mc
  * 
  *     def __cinit__(self, number_of_atoms):             # <<<<<<<<<<<<<<
  *         """
  *         args:
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("mc.MC.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":51
+/* "mamonca/mc.pyx":51
  *         self.c_mc.create_atoms(number_of_atoms)
  * 
  *     def set_landau_coeff(self, coeff, deg, index=0):             # <<<<<<<<<<<<<<
  *         """
  *         Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_3set_landau_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_2set_landau_coeff[] = "\n        Args:\n            coeff (float/list/ndarray): Coefficient to the Landau term. If a single number is\n                given, the same parameter is applied to all the atoms.\n            deg (int): Polynomial degree (usually an even number)\n            index (int): Potential index for thermodynamic integration (0 or 1; choose 0 if\n                not thermodynamic integration)\n\n        Comment:\n            Landau term is given by: sum_i coeff_i*m_i^deg\n        ";
-static PyObject *__pyx_pw_2mc_2MC_3set_landau_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_3set_landau_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_2set_landau_coeff[] = "\n        Args:\n            coeff (float/list/ndarray): Coefficient to the Landau term. If a single number is\n                given, the same parameter is applied to all the atoms.\n            deg (int): Polynomial degree (usually an even number)\n            index (int): Potential index for thermodynamic integration (0 or 1; choose 0 if\n                not thermodynamic integration)\n\n        Comment:\n            Landau term is given by: sum_i coeff_i*m_i^deg\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_3set_landau_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_coeff = 0;
   PyObject *__pyx_v_deg = 0;
   PyObject *__pyx_v_index = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -1862,26 +1865,26 @@
     __pyx_v_deg = values[1];
     __pyx_v_index = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("set_landau_coeff", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 51, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.set_landau_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.set_landau_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_2set_landau_coeff(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_coeff, __pyx_v_deg, __pyx_v_index);
+  __pyx_r = __pyx_pf_7mamonca_2MC_2set_landau_coeff(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_coeff, __pyx_v_deg, __pyx_v_index);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_2set_landau_coeff(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_coeff, PyObject *__pyx_v_deg, PyObject *__pyx_v_index) {
+static PyObject *__pyx_pf_7mamonca_2MC_2set_landau_coeff(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_coeff, PyObject *__pyx_v_deg, PyObject *__pyx_v_index) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -1892,15 +1895,15 @@
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_landau_coeff", 0);
   __Pyx_INCREF(__pyx_v_coeff);
 
-  /* "mc.pyx":63
+  /* "mamonca/mc.pyx":63
  *             Landau term is given by: sum_i coeff_i*m_i^deg
  *         """
  *         coeff = np.array([coeff]).flatten()             # <<<<<<<<<<<<<<
  *         if len(coeff)==1:
  *             coeff = np.tile(coeff, self.c_mc.get_number_of_atoms())
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
@@ -1946,26 +1949,26 @@
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF_SET(__pyx_v_coeff, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "mc.pyx":64
+  /* "mamonca/mc.pyx":64
  *         """
  *         coeff = np.array([coeff]).flatten()
  *         if len(coeff)==1:             # <<<<<<<<<<<<<<
  *             coeff = np.tile(coeff, self.c_mc.get_number_of_atoms())
  *         if len(coeff)!=self.c_mc.get_number_of_atoms():
  */
   __pyx_t_6 = PyObject_Length(__pyx_v_coeff); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 64, __pyx_L1_error)
   __pyx_t_7 = ((__pyx_t_6 == 1) != 0);
   if (__pyx_t_7) {
 
-    /* "mc.pyx":65
+    /* "mamonca/mc.pyx":65
  *         coeff = np.array([coeff]).flatten()
  *         if len(coeff)==1:
  *             coeff = np.tile(coeff, self.c_mc.get_number_of_atoms())             # <<<<<<<<<<<<<<
  *         if len(coeff)!=self.c_mc.get_number_of_atoms():
  *             raise ValueError('coeff has to be a single number or a list of length'
  */
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 65, __pyx_L1_error)
@@ -2021,57 +2024,57 @@
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_coeff, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "mc.pyx":64
+    /* "mamonca/mc.pyx":64
  *         """
  *         coeff = np.array([coeff]).flatten()
  *         if len(coeff)==1:             # <<<<<<<<<<<<<<
  *             coeff = np.tile(coeff, self.c_mc.get_number_of_atoms())
  *         if len(coeff)!=self.c_mc.get_number_of_atoms():
  */
   }
 
-  /* "mc.pyx":66
+  /* "mamonca/mc.pyx":66
  *         if len(coeff)==1:
  *             coeff = np.tile(coeff, self.c_mc.get_number_of_atoms())
  *         if len(coeff)!=self.c_mc.get_number_of_atoms():             # <<<<<<<<<<<<<<
  *             raise ValueError('coeff has to be a single number or a list of length'
  *                              'corresponding to the number of atoms in the box')
  */
   __pyx_t_6 = PyObject_Length(__pyx_v_coeff); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 66, __pyx_L1_error)
   __pyx_t_7 = ((__pyx_t_6 != __pyx_v_self->c_mc.get_number_of_atoms()) != 0);
   if (unlikely(__pyx_t_7)) {
 
-    /* "mc.pyx":67
+    /* "mamonca/mc.pyx":67
  *             coeff = np.tile(coeff, self.c_mc.get_number_of_atoms())
  *         if len(coeff)!=self.c_mc.get_number_of_atoms():
  *             raise ValueError('coeff has to be a single number or a list of length'             # <<<<<<<<<<<<<<
  *                              'corresponding to the number of atoms in the box')
  *         self.c_mc.set_landau_coeff(coeff, deg, index)
  */
     __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(0, 67, __pyx_L1_error)
 
-    /* "mc.pyx":66
+    /* "mamonca/mc.pyx":66
  *         if len(coeff)==1:
  *             coeff = np.tile(coeff, self.c_mc.get_number_of_atoms())
  *         if len(coeff)!=self.c_mc.get_number_of_atoms():             # <<<<<<<<<<<<<<
  *             raise ValueError('coeff has to be a single number or a list of length'
  *                              'corresponding to the number of atoms in the box')
  */
   }
 
-  /* "mc.pyx":69
+  /* "mamonca/mc.pyx":69
  *             raise ValueError('coeff has to be a single number or a list of length'
  *                              'corresponding to the number of atoms in the box')
  *         self.c_mc.set_landau_coeff(coeff, deg, index)             # <<<<<<<<<<<<<<
  * 
  *     def set_heisenberg_coeff(self, coeff, i=None, j=None, deg=1, index=0):
  */
   __pyx_t_9 = __pyx_convert_vector_from_py_double(__pyx_v_coeff); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 69, __pyx_L1_error)
@@ -2080,15 +2083,15 @@
   try {
     __pyx_v_self->c_mc.set_landau_coeff(__pyx_t_9, __pyx_t_8, __pyx_t_10);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 69, __pyx_L1_error)
   }
 
-  /* "mc.pyx":51
+  /* "mamonca/mc.pyx":51
  *         self.c_mc.create_atoms(number_of_atoms)
  * 
  *     def set_landau_coeff(self, coeff, deg, index=0):             # <<<<<<<<<<<<<<
  *         """
  *         Args:
  */
 
@@ -2097,35 +2100,35 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("mc.MC.set_landau_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.set_landau_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_coeff);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":71
+/* "mamonca/mc.pyx":71
  *         self.c_mc.set_landau_coeff(coeff, deg, index)
  * 
  *     def set_heisenberg_coeff(self, coeff, i=None, j=None, deg=1, index=0):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_5set_heisenberg_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_4set_heisenberg_coeff[] = "\n            Args:\n                coeff (float/list/ndarray): Heisenberg coefficient. If a single number is given,\n                    the same parameter is applied to all the pairs defined in me and neigh.\n                    Instead of giving me and neigh, you can also give a n_atom x n_atom tensor.\n                i (list/ndarray): list of indices i (s. definition in the comment)\n                j (list/ndarray): list of indices j (s. definition in the comment)\n                deg (int): polynomial degree\n                index (int): potential index for thermodynamic integration (0 or 1; choose 0 if\n                    not thermodynamic integration)\n            Comment:\n                Heisenberg term is given by: -sum_ij coeff_ij*(m_i*m_j)^deg. Beware of the\n                negative sign.\n        ";
-static PyObject *__pyx_pw_2mc_2MC_5set_heisenberg_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_5set_heisenberg_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_4set_heisenberg_coeff[] = "\n            Args:\n                coeff (float/list/ndarray): Heisenberg coefficient. If a single number is given,\n                    the same parameter is applied to all the pairs defined in me and neigh.\n                    Instead of giving me and neigh, you can also give a n_atom x n_atom tensor.\n                i (list/ndarray): list of indices i (s. definition in the comment)\n                j (list/ndarray): list of indices j (s. definition in the comment)\n                deg (int): polynomial degree\n                index (int): potential index for thermodynamic integration (0 or 1; choose 0 if\n                    not thermodynamic integration)\n            Comment:\n                Heisenberg term is given by: -sum_ij coeff_ij*(m_i*m_j)^deg. Beware of the\n                negative sign.\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_5set_heisenberg_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_coeff = 0;
   PyObject *__pyx_v_i = 0;
   PyObject *__pyx_v_j = 0;
   PyObject *__pyx_v_deg = 0;
   PyObject *__pyx_v_index = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -2211,26 +2214,26 @@
     __pyx_v_deg = values[3];
     __pyx_v_index = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("set_heisenberg_coeff", 0, 1, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 71, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.set_heisenberg_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.set_heisenberg_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_4set_heisenberg_coeff(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_coeff, __pyx_v_i, __pyx_v_j, __pyx_v_deg, __pyx_v_index);
+  __pyx_r = __pyx_pf_7mamonca_2MC_4set_heisenberg_coeff(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_coeff, __pyx_v_i, __pyx_v_j, __pyx_v_deg, __pyx_v_index);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_4set_heisenberg_coeff(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_coeff, PyObject *__pyx_v_i, PyObject *__pyx_v_j, PyObject *__pyx_v_deg, PyObject *__pyx_v_index) {
+static PyObject *__pyx_pf_7mamonca_2MC_4set_heisenberg_coeff(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_coeff, PyObject *__pyx_v_i, PyObject *__pyx_v_j, PyObject *__pyx_v_deg, PyObject *__pyx_v_index) {
   int __pyx_v_n;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
@@ -2250,15 +2253,15 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_heisenberg_coeff", 0);
   __Pyx_INCREF(__pyx_v_coeff);
   __Pyx_INCREF(__pyx_v_i);
   __Pyx_INCREF(__pyx_v_j);
 
-  /* "mc.pyx":86
+  /* "mamonca/mc.pyx":86
  *                 negative sign.
  *         """
  *         if i is None and j is None:             # <<<<<<<<<<<<<<
  *             n = self.c_mc.get_number_of_atoms()
  *             if np.array(coeff).shape!=(n, n):
  */
   __pyx_t_2 = (__pyx_v_i == Py_None);
@@ -2270,24 +2273,24 @@
   }
   __pyx_t_3 = (__pyx_v_j == Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "mc.pyx":87
+    /* "mamonca/mc.pyx":87
  *         """
  *         if i is None and j is None:
  *             n = self.c_mc.get_number_of_atoms()             # <<<<<<<<<<<<<<
  *             if np.array(coeff).shape!=(n, n):
  *                 raise ValueError(
  */
     __pyx_v_n = __pyx_v_self->c_mc.get_number_of_atoms();
 
-    /* "mc.pyx":88
+    /* "mamonca/mc.pyx":88
  *         if i is None and j is None:
  *             n = self.c_mc.get_number_of_atoms()
  *             if np.array(coeff).shape!=(n, n):             # <<<<<<<<<<<<<<
  *                 raise ValueError(
  *                     'If i and j are not specified, coeff has to be a 2d tensor with the length '
  */
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
@@ -2328,37 +2331,37 @@
     __pyx_t_5 = PyObject_RichCompare(__pyx_t_6, __pyx_t_7, Py_NE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(__pyx_t_1)) {
 
-      /* "mc.pyx":89
+      /* "mamonca/mc.pyx":89
  *             n = self.c_mc.get_number_of_atoms()
  *             if np.array(coeff).shape!=(n, n):
  *                 raise ValueError(             # <<<<<<<<<<<<<<
  *                     'If i and j are not specified, coeff has to be a 2d tensor with the length '
  *                     + 'equal to the number of atoms in each direction.'
  */
       __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(0, 89, __pyx_L1_error)
 
-      /* "mc.pyx":88
+      /* "mamonca/mc.pyx":88
  *         if i is None and j is None:
  *             n = self.c_mc.get_number_of_atoms()
  *             if np.array(coeff).shape!=(n, n):             # <<<<<<<<<<<<<<
  *                 raise ValueError(
  *                     'If i and j are not specified, coeff has to be a 2d tensor with the length '
  */
     }
 
-    /* "mc.pyx":93
+    /* "mamonca/mc.pyx":93
  *                     + 'equal to the number of atoms in each direction.'
  *                 )
  *             i,j = np.where(coeff!=0)             # <<<<<<<<<<<<<<
  *             coeff = coeff[coeff!=0]
  *         coeff = np.array([coeff]).flatten()
  */
     __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 93, __pyx_L1_error)
@@ -2431,39 +2434,39 @@
       __pyx_L8_unpacking_done:;
     }
     __Pyx_DECREF_SET(__pyx_v_i, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_DECREF_SET(__pyx_v_j, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "mc.pyx":94
+    /* "mamonca/mc.pyx":94
  *                 )
  *             i,j = np.where(coeff!=0)
  *             coeff = coeff[coeff!=0]             # <<<<<<<<<<<<<<
  *         coeff = np.array([coeff]).flatten()
  *         i = np.array(i).flatten()
  */
     __pyx_t_5 = __Pyx_PyInt_NeObjC(__pyx_v_coeff, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_coeff, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_coeff, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "mc.pyx":86
+    /* "mamonca/mc.pyx":86
  *                 negative sign.
  *         """
  *         if i is None and j is None:             # <<<<<<<<<<<<<<
  *             n = self.c_mc.get_number_of_atoms()
  *             if np.array(coeff).shape!=(n, n):
  */
   }
 
-  /* "mc.pyx":95
+  /* "mamonca/mc.pyx":95
  *             i,j = np.where(coeff!=0)
  *             coeff = coeff[coeff!=0]
  *         coeff = np.array([coeff]).flatten()             # <<<<<<<<<<<<<<
  *         i = np.array(i).flatten()
  *         j = np.array(j).flatten()
  */
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 95, __pyx_L1_error)
@@ -2509,15 +2512,15 @@
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF_SET(__pyx_v_coeff, __pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "mc.pyx":96
+  /* "mamonca/mc.pyx":96
  *             coeff = coeff[coeff!=0]
  *         coeff = np.array([coeff]).flatten()
  *         i = np.array(i).flatten()             # <<<<<<<<<<<<<<
  *         j = np.array(j).flatten()
  *         if len(coeff)==1:
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
@@ -2557,15 +2560,15 @@
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF_SET(__pyx_v_i, __pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "mc.pyx":97
+  /* "mamonca/mc.pyx":97
  *         coeff = np.array([coeff]).flatten()
  *         i = np.array(i).flatten()
  *         j = np.array(j).flatten()             # <<<<<<<<<<<<<<
  *         if len(coeff)==1:
  *             coeff = np.tile(coeff, len(i))
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
@@ -2605,26 +2608,26 @@
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF_SET(__pyx_v_j, __pyx_t_7);
   __pyx_t_7 = 0;
 
-  /* "mc.pyx":98
+  /* "mamonca/mc.pyx":98
  *         i = np.array(i).flatten()
  *         j = np.array(j).flatten()
  *         if len(coeff)==1:             # <<<<<<<<<<<<<<
  *             coeff = np.tile(coeff, len(i))
  *         if len(coeff)!=len(i) or len(i)!=len(j):
  */
   __pyx_t_10 = PyObject_Length(__pyx_v_coeff); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 98, __pyx_L1_error)
   __pyx_t_1 = ((__pyx_t_10 == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "mc.pyx":99
+    /* "mamonca/mc.pyx":99
  *         j = np.array(j).flatten()
  *         if len(coeff)==1:
  *             coeff = np.tile(coeff, len(i))             # <<<<<<<<<<<<<<
  *         if len(coeff)!=len(i) or len(i)!=len(j):
  *             raise ValueError('Length of vectors not the same')
  */
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
@@ -2681,24 +2684,24 @@
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF_SET(__pyx_v_coeff, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "mc.pyx":98
+    /* "mamonca/mc.pyx":98
  *         i = np.array(i).flatten()
  *         j = np.array(j).flatten()
  *         if len(coeff)==1:             # <<<<<<<<<<<<<<
  *             coeff = np.tile(coeff, len(i))
  *         if len(coeff)!=len(i) or len(i)!=len(j):
  */
   }
 
-  /* "mc.pyx":100
+  /* "mamonca/mc.pyx":100
  *         if len(coeff)==1:
  *             coeff = np.tile(coeff, len(i))
  *         if len(coeff)!=len(i) or len(i)!=len(j):             # <<<<<<<<<<<<<<
  *             raise ValueError('Length of vectors not the same')
  *         self.c_mc.set_heisenberg_coeff(coeff, i, j, deg, index)
  */
   __pyx_t_10 = PyObject_Length(__pyx_v_coeff); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 100, __pyx_L1_error)
@@ -2712,37 +2715,37 @@
   __pyx_t_12 = PyObject_Length(__pyx_v_i); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 100, __pyx_L1_error)
   __pyx_t_10 = PyObject_Length(__pyx_v_j); if (unlikely(__pyx_t_10 == ((Py_ssize_t)-1))) __PYX_ERR(0, 100, __pyx_L1_error)
   __pyx_t_2 = ((__pyx_t_12 != __pyx_t_10) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L11_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "mc.pyx":101
+    /* "mamonca/mc.pyx":101
  *             coeff = np.tile(coeff, len(i))
  *         if len(coeff)!=len(i) or len(i)!=len(j):
  *             raise ValueError('Length of vectors not the same')             # <<<<<<<<<<<<<<
  *         self.c_mc.set_heisenberg_coeff(coeff, i, j, deg, index)
  * 
  */
     __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_Raise(__pyx_t_7, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __PYX_ERR(0, 101, __pyx_L1_error)
 
-    /* "mc.pyx":100
+    /* "mamonca/mc.pyx":100
  *         if len(coeff)==1:
  *             coeff = np.tile(coeff, len(i))
  *         if len(coeff)!=len(i) or len(i)!=len(j):             # <<<<<<<<<<<<<<
  *             raise ValueError('Length of vectors not the same')
  *         self.c_mc.set_heisenberg_coeff(coeff, i, j, deg, index)
  */
   }
 
-  /* "mc.pyx":102
+  /* "mamonca/mc.pyx":102
  *         if len(coeff)!=len(i) or len(i)!=len(j):
  *             raise ValueError('Length of vectors not the same')
  *         self.c_mc.set_heisenberg_coeff(coeff, i, j, deg, index)             # <<<<<<<<<<<<<<
  * 
  *     def clear_heisenberg_coeff(self, index=0):
  */
   __pyx_t_13 = __pyx_convert_vector_from_py_double(__pyx_v_coeff); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 102, __pyx_L1_error)
@@ -2753,15 +2756,15 @@
   try {
     __pyx_v_self->c_mc.set_heisenberg_coeff(__pyx_t_13, __pyx_t_14, __pyx_t_15, __pyx_t_11, __pyx_t_16);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 102, __pyx_L1_error)
   }
 
-  /* "mc.pyx":71
+  /* "mamonca/mc.pyx":71
  *         self.c_mc.set_landau_coeff(coeff, deg, index)
  * 
  *     def set_heisenberg_coeff(self, coeff, i=None, j=None, deg=1, index=0):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
@@ -2770,37 +2773,37 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("mc.MC.set_heisenberg_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.set_heisenberg_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_coeff);
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XDECREF(__pyx_v_j);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":104
+/* "mamonca/mc.pyx":104
  *         self.c_mc.set_heisenberg_coeff(coeff, i, j, deg, index)
  * 
  *     def clear_heisenberg_coeff(self, index=0):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_7clear_heisenberg_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_6clear_heisenberg_coeff[] = "\n            Args:\n                index (int): potential index for thermodynamic integration (0 or 1; choose 0 if\n                             not thermodynamic integration)\n\n            This function erases all the Heisenberg coefficients defined before.\n        ";
-static PyObject *__pyx_pw_2mc_2MC_7clear_heisenberg_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_7clear_heisenberg_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_6clear_heisenberg_coeff[] = "\n            Args:\n                index (int): potential index for thermodynamic integration (0 or 1; choose 0 if\n                             not thermodynamic integration)\n\n            This function erases all the Heisenberg coefficients defined before.\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_7clear_heisenberg_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_index = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("clear_heisenberg_coeff (wrapper)", 0);
@@ -2838,81 +2841,81 @@
     }
     __pyx_v_index = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("clear_heisenberg_coeff", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 104, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.clear_heisenberg_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.clear_heisenberg_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_6clear_heisenberg_coeff(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_index);
+  __pyx_r = __pyx_pf_7mamonca_2MC_6clear_heisenberg_coeff(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_index);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_6clear_heisenberg_coeff(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index) {
+static PyObject *__pyx_pf_7mamonca_2MC_6clear_heisenberg_coeff(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear_heisenberg_coeff", 0);
 
-  /* "mc.pyx":112
+  /* "mamonca/mc.pyx":112
  *             This function erases all the Heisenberg coefficients defined before.
  *         """
  *         self.c_mc.clear_heisenberg_coeff(index)             # <<<<<<<<<<<<<<
  * 
  *     def clear_landau_coeff(self, index=0):
  */
   __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 112, __pyx_L1_error)
   try {
     __pyx_v_self->c_mc.clear_heisenberg_coeff(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 112, __pyx_L1_error)
   }
 
-  /* "mc.pyx":104
+  /* "mamonca/mc.pyx":104
  *         self.c_mc.set_heisenberg_coeff(coeff, i, j, deg, index)
  * 
  *     def clear_heisenberg_coeff(self, index=0):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("mc.MC.clear_heisenberg_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.clear_heisenberg_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":114
+/* "mamonca/mc.pyx":114
  *         self.c_mc.clear_heisenberg_coeff(index)
  * 
  *     def clear_landau_coeff(self, index=0):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_9clear_landau_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_8clear_landau_coeff[] = "\n            Args:\n                index (int): potential index for thermodynamic integration (0 or 1; choose 0 if\n                             not thermodynamic integration)\n\n            This function erases all the Landau coefficients defined before.\n        ";
-static PyObject *__pyx_pw_2mc_2MC_9clear_landau_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_9clear_landau_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_8clear_landau_coeff[] = "\n            Args:\n                index (int): potential index for thermodynamic integration (0 or 1; choose 0 if\n                             not thermodynamic integration)\n\n            This function erases all the Landau coefficients defined before.\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_9clear_landau_coeff(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_index = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("clear_landau_coeff (wrapper)", 0);
@@ -2950,103 +2953,103 @@
     }
     __pyx_v_index = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("clear_landau_coeff", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 114, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.clear_landau_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.clear_landau_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_8clear_landau_coeff(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_index);
+  __pyx_r = __pyx_pf_7mamonca_2MC_8clear_landau_coeff(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_index);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_8clear_landau_coeff(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index) {
+static PyObject *__pyx_pf_7mamonca_2MC_8clear_landau_coeff(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear_landau_coeff", 0);
 
-  /* "mc.pyx":122
+  /* "mamonca/mc.pyx":122
  *             This function erases all the Landau coefficients defined before.
  *         """
  *         self.c_mc.clear_landau_coeff(index)             # <<<<<<<<<<<<<<
  * 
  *     def clear_all_coeff(self):
  */
   __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 122, __pyx_L1_error)
   try {
     __pyx_v_self->c_mc.clear_landau_coeff(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 122, __pyx_L1_error)
   }
 
-  /* "mc.pyx":114
+  /* "mamonca/mc.pyx":114
  *         self.c_mc.clear_heisenberg_coeff(index)
  * 
  *     def clear_landau_coeff(self, index=0):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("mc.MC.clear_landau_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.clear_landau_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":124
+/* "mamonca/mc.pyx":124
  *         self.c_mc.clear_landau_coeff(index)
  * 
  *     def clear_all_coeff(self):             # <<<<<<<<<<<<<<
  *         """
  *             This function erases all the coefficients defined before.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_11clear_all_coeff(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_2mc_2MC_10clear_all_coeff[] = "\n            This function erases all the coefficients defined before.\n        ";
-static PyObject *__pyx_pw_2mc_2MC_11clear_all_coeff(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7mamonca_2MC_11clear_all_coeff(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7mamonca_2MC_10clear_all_coeff[] = "\n            This function erases all the coefficients defined before.\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_11clear_all_coeff(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("clear_all_coeff (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_10clear_all_coeff(((struct __pyx_obj_2mc_MC *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7mamonca_2MC_10clear_all_coeff(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_10clear_all_coeff(struct __pyx_obj_2mc_MC *__pyx_v_self) {
+static PyObject *__pyx_pf_7mamonca_2MC_10clear_all_coeff(struct __pyx_obj_7mamonca_MC *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear_all_coeff", 0);
 
-  /* "mc.pyx":128
+  /* "mamonca/mc.pyx":128
  *             This function erases all the coefficients defined before.
  *         """
  *         self.clear_heisenberg_coeff()             # <<<<<<<<<<<<<<
  *         self.clear_heisenberg_coeff(1)
  *         self.clear_landau_coeff()
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear_heisenberg_coeff); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
@@ -3064,15 +3067,15 @@
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mc.pyx":129
+  /* "mamonca/mc.pyx":129
  *         """
  *         self.clear_heisenberg_coeff()
  *         self.clear_heisenberg_coeff(1)             # <<<<<<<<<<<<<<
  *         self.clear_landau_coeff()
  *         self.clear_landau_coeff(1)
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear_heisenberg_coeff); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
@@ -3090,15 +3093,15 @@
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_int_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_int_1);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mc.pyx":130
+  /* "mamonca/mc.pyx":130
  *         self.clear_heisenberg_coeff()
  *         self.clear_heisenberg_coeff(1)
  *         self.clear_landau_coeff()             # <<<<<<<<<<<<<<
  *         self.clear_landau_coeff(1)
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear_landau_coeff); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
@@ -3116,15 +3119,15 @@
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mc.pyx":131
+  /* "mamonca/mc.pyx":131
  *         self.clear_heisenberg_coeff(1)
  *         self.clear_landau_coeff()
  *         self.clear_landau_coeff(1)             # <<<<<<<<<<<<<<
  * 
  *     def get_magnetic_gradients(self):
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_clear_landau_coeff); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
@@ -3142,82 +3145,82 @@
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_int_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_int_1);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mc.pyx":124
+  /* "mamonca/mc.pyx":124
  *         self.c_mc.clear_landau_coeff(index)
  * 
  *     def clear_all_coeff(self):             # <<<<<<<<<<<<<<
  *         """
  *             This function erases all the coefficients defined before.
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("mc.MC.clear_all_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.clear_all_coeff", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":133
+/* "mamonca/mc.pyx":133
  *         self.clear_landau_coeff(1)
  * 
  *     def get_magnetic_gradients(self):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_13get_magnetic_gradients(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_2mc_2MC_12get_magnetic_gradients[] = "\n            Returns:\n                nx3 array of magnetic gradients\n        ";
-static PyObject *__pyx_pw_2mc_2MC_13get_magnetic_gradients(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7mamonca_2MC_13get_magnetic_gradients(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7mamonca_2MC_12get_magnetic_gradients[] = "\n            Returns:\n                nx3 array of magnetic gradients\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_13get_magnetic_gradients(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_magnetic_gradients (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_12get_magnetic_gradients(((struct __pyx_obj_2mc_MC *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7mamonca_2MC_12get_magnetic_gradients(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_12get_magnetic_gradients(struct __pyx_obj_2mc_MC *__pyx_v_self) {
+static PyObject *__pyx_pf_7mamonca_2MC_12get_magnetic_gradients(struct __pyx_obj_7mamonca_MC *__pyx_v_self) {
   std::vector<double>  __pyx_v_m;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_magnetic_gradients", 0);
 
-  /* "mc.pyx":138
+  /* "mamonca/mc.pyx":138
  *                 nx3 array of magnetic gradients
  *         """
  *         m = self.c_mc.get_magnetic_gradients()             # <<<<<<<<<<<<<<
  *         return np.array(m).reshape(-1, 3)
  * 
  */
   __pyx_v_m = __pyx_v_self->c_mc.get_magnetic_gradients();
 
-  /* "mc.pyx":139
+  /* "mamonca/mc.pyx":139
  *         """
  *         m = self.c_mc.get_magnetic_gradients()
  *         return np.array(m).reshape(-1, 3)             # <<<<<<<<<<<<<<
  * 
  *     def get_magnetic_moments(self):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3250,81 +3253,81 @@
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":133
+  /* "mamonca/mc.pyx":133
  *         self.clear_landau_coeff(1)
  * 
  *     def get_magnetic_gradients(self):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("mc.MC.get_magnetic_gradients", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_magnetic_gradients", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":141
+/* "mamonca/mc.pyx":141
  *         return np.array(m).reshape(-1, 3)
  * 
  *     def get_magnetic_moments(self):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_15get_magnetic_moments(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_2mc_2MC_14get_magnetic_moments[] = "\n            Returns:\n                nx3 array of magnetic moments\n        ";
-static PyObject *__pyx_pw_2mc_2MC_15get_magnetic_moments(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7mamonca_2MC_15get_magnetic_moments(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7mamonca_2MC_14get_magnetic_moments[] = "\n            Returns:\n                nx3 array of magnetic moments\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_15get_magnetic_moments(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_magnetic_moments (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_14get_magnetic_moments(((struct __pyx_obj_2mc_MC *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7mamonca_2MC_14get_magnetic_moments(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_14get_magnetic_moments(struct __pyx_obj_2mc_MC *__pyx_v_self) {
+static PyObject *__pyx_pf_7mamonca_2MC_14get_magnetic_moments(struct __pyx_obj_7mamonca_MC *__pyx_v_self) {
   std::vector<double>  __pyx_v_m;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_magnetic_moments", 0);
 
-  /* "mc.pyx":146
+  /* "mamonca/mc.pyx":146
  *                 nx3 array of magnetic moments
  *         """
  *         m = self.c_mc.get_magnetic_moments()             # <<<<<<<<<<<<<<
  *         return np.array(m).reshape(-1, 3)
  * 
  */
   __pyx_v_m = __pyx_v_self->c_mc.get_magnetic_moments();
 
-  /* "mc.pyx":147
+  /* "mamonca/mc.pyx":147
  *         """
  *         m = self.c_mc.get_magnetic_moments()
  *         return np.array(m).reshape(-1, 3)             # <<<<<<<<<<<<<<
  * 
  *     def set_magnetic_moments(self, magmoms):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3357,72 +3360,72 @@
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":141
+  /* "mamonca/mc.pyx":141
  *         return np.array(m).reshape(-1, 3)
  * 
  *     def get_magnetic_moments(self):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("mc.MC.get_magnetic_moments", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_magnetic_moments", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":149
+/* "mamonca/mc.pyx":149
  *         return np.array(m).reshape(-1, 3)
  * 
  *     def set_magnetic_moments(self, magmoms):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_17set_magnetic_moments(PyObject *__pyx_v_self, PyObject *__pyx_v_magmoms); /*proto*/
-static char __pyx_doc_2mc_2MC_16set_magnetic_moments[] = "\n            Args:\n                magmoms (ndarray/list): nx3 magnetic moments to set\n        ";
-static PyObject *__pyx_pw_2mc_2MC_17set_magnetic_moments(PyObject *__pyx_v_self, PyObject *__pyx_v_magmoms) {
+static PyObject *__pyx_pw_7mamonca_2MC_17set_magnetic_moments(PyObject *__pyx_v_self, PyObject *__pyx_v_magmoms); /*proto*/
+static char __pyx_doc_7mamonca_2MC_16set_magnetic_moments[] = "\n            Args:\n                magmoms (ndarray/list): nx3 magnetic moments to set\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_17set_magnetic_moments(PyObject *__pyx_v_self, PyObject *__pyx_v_magmoms) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_magnetic_moments (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_16set_magnetic_moments(((struct __pyx_obj_2mc_MC *)__pyx_v_self), ((PyObject *)__pyx_v_magmoms));
+  __pyx_r = __pyx_pf_7mamonca_2MC_16set_magnetic_moments(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), ((PyObject *)__pyx_v_magmoms));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_16set_magnetic_moments(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_magmoms) {
+static PyObject *__pyx_pf_7mamonca_2MC_16set_magnetic_moments(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_magmoms) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   std::vector<double>  __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_magnetic_moments", 0);
 
-  /* "mc.pyx":154
+  /* "mamonca/mc.pyx":154
  *                 magmoms (ndarray/list): nx3 magnetic moments to set
  *         """
  *         self.c_mc.set_magnetic_moments(np.array(magmoms).flatten())             # <<<<<<<<<<<<<<
  * 
  *     def get_magnetization(self):
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
@@ -3468,15 +3471,15 @@
   try {
     __pyx_v_self->c_mc.set_magnetic_moments(__pyx_t_5);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 154, __pyx_L1_error)
   }
 
-  /* "mc.pyx":149
+  /* "mamonca/mc.pyx":149
  *         return np.array(m).reshape(-1, 3)
  * 
  *     def set_magnetic_moments(self, magmoms):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
@@ -3484,58 +3487,58 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("mc.MC.set_magnetic_moments", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.set_magnetic_moments", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":156
+/* "mamonca/mc.pyx":156
  *         self.c_mc.set_magnetic_moments(np.array(magmoms).flatten())
  * 
  *     def get_magnetization(self):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_19get_magnetization(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_2mc_2MC_18get_magnetization[] = "\n            Returns:\n                average magnetization value or vector\n        ";
-static PyObject *__pyx_pw_2mc_2MC_19get_magnetization(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7mamonca_2MC_19get_magnetization(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7mamonca_2MC_18get_magnetization[] = "\n            Returns:\n                average magnetization value or vector\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_19get_magnetization(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_magnetization (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_18get_magnetization(((struct __pyx_obj_2mc_MC *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7mamonca_2MC_18get_magnetization(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_18get_magnetization(struct __pyx_obj_2mc_MC *__pyx_v_self) {
+static PyObject *__pyx_pf_7mamonca_2MC_18get_magnetization(struct __pyx_obj_7mamonca_MC *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   std::vector<double>  __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_magnetization", 0);
 
-  /* "mc.pyx":161
+  /* "mamonca/mc.pyx":161
  *                 average magnetization value or vector
  *         """
  *         return np.array(self.c_mc.get_magnetization())             # <<<<<<<<<<<<<<
  * 
  *     def get_output(self, index=0):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3568,48 +3571,48 @@
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":156
+  /* "mamonca/mc.pyx":156
  *         self.c_mc.set_magnetic_moments(np.array(magmoms).flatten())
  * 
  *     def get_magnetization(self):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("mc.MC.get_magnetization", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_magnetization", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":163
+/* "mamonca/mc.pyx":163
  *         return np.array(self.c_mc.get_magnetization())
  * 
  *     def get_output(self, index=0):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_21get_output(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_20get_output[] = "\n            Args:\n                index (int): Potential index (only for thermodynamic integration)\n\n            Returns:\n                dict of output values\n        ";
-static PyObject *__pyx_pw_2mc_2MC_21get_output(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_21get_output(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_20get_output[] = "\n            Args:\n                index (int): Potential index (only for thermodynamic integration)\n\n            Returns:\n                dict of output values\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_21get_output(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_index = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_output (wrapper)", 0);
@@ -3647,40 +3650,40 @@
     }
     __pyx_v_index = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("get_output", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 163, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.get_output", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_output", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_20get_output(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_index);
+  __pyx_r = __pyx_pf_7mamonca_2MC_20get_output(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_index);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_20get_output(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index) {
+static PyObject *__pyx_pf_7mamonca_2MC_20get_output(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_output", 0);
 
-  /* "mc.pyx":171
+  /* "mamonca/mc.pyx":171
  *                 dict of output values
  *         """
  *         return {'energy': self.get_energy(index=index),             # <<<<<<<<<<<<<<
  *                 'mean_energy': self.get_mean_energy(index=index),
  *                 'magnetization': np.mean(self.get_magnetization()),
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3694,15 +3697,15 @@
   __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_energy, __pyx_t_4) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "mc.pyx":172
+  /* "mamonca/mc.pyx":172
  *         """
  *         return {'energy': self.get_energy(index=index),
  *                 'mean_energy': self.get_mean_energy(index=index),             # <<<<<<<<<<<<<<
  *                 'magnetization': np.mean(self.get_magnetization()),
  *                 'energy_variance': self.get_energy_variance(index=index),
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_mean_energy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 172, __pyx_L1_error)
@@ -3713,15 +3716,15 @@
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_mean_energy, __pyx_t_2) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "mc.pyx":173
+  /* "mamonca/mc.pyx":173
  *         return {'energy': self.get_energy(index=index),
  *                 'mean_energy': self.get_mean_energy(index=index),
  *                 'magnetization': np.mean(self.get_magnetization()),             # <<<<<<<<<<<<<<
  *                 'energy_variance': self.get_energy_variance(index=index),
  *                 'acceptance_ratio': self.get_acceptance_ratio(),
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
@@ -3761,15 +3764,15 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_magnetization, __pyx_t_2) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "mc.pyx":174
+  /* "mamonca/mc.pyx":174
  *                 'mean_energy': self.get_mean_energy(index=index),
  *                 'magnetization': np.mean(self.get_magnetization()),
  *                 'energy_variance': self.get_energy_variance(index=index),             # <<<<<<<<<<<<<<
  *                 'acceptance_ratio': self.get_acceptance_ratio(),
  *                 'steps_per_second': self.get_steps_per_second()}
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_energy_variance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
@@ -3780,15 +3783,15 @@
   __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_energy_variance, __pyx_t_3) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "mc.pyx":175
+  /* "mamonca/mc.pyx":175
  *                 'magnetization': np.mean(self.get_magnetization()),
  *                 'energy_variance': self.get_energy_variance(index=index),
  *                 'acceptance_ratio': self.get_acceptance_ratio(),             # <<<<<<<<<<<<<<
  *                 'steps_per_second': self.get_steps_per_second()}
  * 
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_acceptance_ratio); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 175, __pyx_L1_error)
@@ -3807,15 +3810,15 @@
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_acceptance_ratio, __pyx_t_3) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "mc.pyx":176
+  /* "mamonca/mc.pyx":176
  *                 'energy_variance': self.get_energy_variance(index=index),
  *                 'acceptance_ratio': self.get_acceptance_ratio(),
  *                 'steps_per_second': self.get_steps_per_second()}             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_steps_per_second); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 176, __pyx_L1_error)
@@ -3837,15 +3840,15 @@
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_steps_per_second, __pyx_t_3) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":163
+  /* "mamonca/mc.pyx":163
  *         return np.array(self.c_mc.get_magnetization())
  * 
  *     def get_output(self, index=0):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
@@ -3853,34 +3856,34 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("mc.MC.get_output", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_output", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":179
+/* "mamonca/mc.pyx":179
  * 
  * 
  *     def run(self, temperature, number_of_iterations=1, reset=True, threads=1):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_23run(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_22run[] = "\n            Args:\n                temperature (float): Temperature in K\n                number_of_iterations (int): Number of MC steps (internally multiplied\n                                            by the number of atoms)\n                reset (bool): Resets statistics (s. get_mean_energy() etc.)\n        ";
-static PyObject *__pyx_pw_2mc_2MC_23run(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_23run(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_22run[] = "\n            Args:\n                temperature (float): Temperature in K\n                number_of_iterations (int): Number of MC steps (internally multiplied\n                                            by the number of atoms)\n                reset (bool): Resets statistics (s. get_mean_energy() etc.)\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_23run(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_temperature = 0;
   PyObject *__pyx_v_number_of_iterations = 0;
   PyObject *__pyx_v_reset = 0;
   PyObject *__pyx_v_threads = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -3953,66 +3956,66 @@
     __pyx_v_reset = values[2];
     __pyx_v_threads = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("run", 0, 1, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 179, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_22run(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_temperature, __pyx_v_number_of_iterations, __pyx_v_reset, __pyx_v_threads);
+  __pyx_r = __pyx_pf_7mamonca_2MC_22run(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_temperature, __pyx_v_number_of_iterations, __pyx_v_reset, __pyx_v_threads);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_22run(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_temperature, PyObject *__pyx_v_number_of_iterations, PyObject *__pyx_v_reset, PyObject *__pyx_v_threads) {
+static PyObject *__pyx_pf_7mamonca_2MC_22run(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_temperature, PyObject *__pyx_v_number_of_iterations, PyObject *__pyx_v_reset, PyObject *__pyx_v_threads) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   double __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("run", 0);
 
-  /* "mc.pyx":187
+  /* "mamonca/mc.pyx":187
  *                 reset (bool): Resets statistics (s. get_mean_energy() etc.)
  *         """
  *         if reset:             # <<<<<<<<<<<<<<
  *             self.c_mc.reset()
  *         self.c_mc.run(temperature, number_of_iterations, threads)
  */
   __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_reset); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mc.pyx":188
+    /* "mamonca/mc.pyx":188
  *         """
  *         if reset:
  *             self.c_mc.reset()             # <<<<<<<<<<<<<<
  *         self.c_mc.run(temperature, number_of_iterations, threads)
  * 
  */
     __pyx_v_self->c_mc.reset();
 
-    /* "mc.pyx":187
+    /* "mamonca/mc.pyx":187
  *                 reset (bool): Resets statistics (s. get_mean_energy() etc.)
  *         """
  *         if reset:             # <<<<<<<<<<<<<<
  *             self.c_mc.reset()
  *         self.c_mc.run(temperature, number_of_iterations, threads)
  */
   }
 
-  /* "mc.pyx":189
+  /* "mamonca/mc.pyx":189
  *         if reset:
  *             self.c_mc.reset()
  *         self.c_mc.run(temperature, number_of_iterations, threads)             # <<<<<<<<<<<<<<
  * 
  *     def get_acceptance_ratio(self, individual=False):
  */
   __pyx_t_2 = __pyx_PyFloat_AsDouble(__pyx_v_temperature); if (unlikely((__pyx_t_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L1_error)
@@ -4021,46 +4024,46 @@
   try {
     __pyx_v_self->c_mc.run(__pyx_t_2, __pyx_t_3, __pyx_t_4);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 189, __pyx_L1_error)
   }
 
-  /* "mc.pyx":179
+  /* "mamonca/mc.pyx":179
  * 
  * 
  *     def run(self, temperature, number_of_iterations=1, reset=True, threads=1):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("mc.MC.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.run", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":191
+/* "mamonca/mc.pyx":191
  *         self.c_mc.run(temperature, number_of_iterations, threads)
  * 
  *     def get_acceptance_ratio(self, individual=False):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_25get_acceptance_ratio(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_24get_acceptance_ratio[] = "\n            Args:\n                individual (bool): If true, an array containing each acceptance ratio is returned\n            Returns:\n                Acceptance ratio since the last reset (s. reset())\n        ";
-static PyObject *__pyx_pw_2mc_2MC_25get_acceptance_ratio(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_25get_acceptance_ratio(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_24get_acceptance_ratio[] = "\n            Args:\n                individual (bool): If true, an array containing each acceptance ratio is returned\n            Returns:\n                Acceptance ratio since the last reset (s. reset())\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_25get_acceptance_ratio(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_individual = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_acceptance_ratio (wrapper)", 0);
@@ -4098,49 +4101,49 @@
     }
     __pyx_v_individual = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("get_acceptance_ratio", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 191, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.get_acceptance_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_acceptance_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_24get_acceptance_ratio(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_individual);
+  __pyx_r = __pyx_pf_7mamonca_2MC_24get_acceptance_ratio(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_individual);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_24get_acceptance_ratio(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_individual) {
+static PyObject *__pyx_pf_7mamonca_2MC_24get_acceptance_ratio(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_individual) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_acceptance_ratio", 0);
 
-  /* "mc.pyx":198
+  /* "mamonca/mc.pyx":198
  *                 Acceptance ratio since the last reset (s. reset())
  *         """
  *         if individual:             # <<<<<<<<<<<<<<
  *             return np.array(self.c_mc.get_acceptance_ratios())
  *         return self.c_mc.get_acceptance_ratio()
  */
   __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_individual); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mc.pyx":199
+    /* "mamonca/mc.pyx":199
  *         """
  *         if individual:
  *             return np.array(self.c_mc.get_acceptance_ratios())             # <<<<<<<<<<<<<<
  *         return self.c_mc.get_acceptance_ratio()
  * 
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4167,71 +4170,71 @@
     if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "mc.pyx":198
+    /* "mamonca/mc.pyx":198
  *                 Acceptance ratio since the last reset (s. reset())
  *         """
  *         if individual:             # <<<<<<<<<<<<<<
  *             return np.array(self.c_mc.get_acceptance_ratios())
  *         return self.c_mc.get_acceptance_ratio()
  */
   }
 
-  /* "mc.pyx":200
+  /* "mamonca/mc.pyx":200
  *         if individual:
  *             return np.array(self.c_mc.get_acceptance_ratios())
  *         return self.c_mc.get_acceptance_ratio()             # <<<<<<<<<<<<<<
  * 
  *     def get_energy(self, index=0, per_atom=False):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = PyFloat_FromDouble(__pyx_v_self->c_mc.get_acceptance_ratio()); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":191
+  /* "mamonca/mc.pyx":191
  *         self.c_mc.run(temperature, number_of_iterations, threads)
  * 
  *     def get_acceptance_ratio(self, individual=False):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("mc.MC.get_acceptance_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_acceptance_ratio", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":202
+/* "mamonca/mc.pyx":202
  *         return self.c_mc.get_acceptance_ratio()
  * 
  *     def get_energy(self, index=0, per_atom=False):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_27get_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_26get_energy[] = "\n            Returns:\n                Energy value of current snapshot in eV\n        ";
-static PyObject *__pyx_pw_2mc_2MC_27get_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_27get_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_26get_energy[] = "\n            Returns:\n                Energy value of current snapshot in eV\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_27get_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_index = 0;
   PyObject *__pyx_v_per_atom = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4282,48 +4285,48 @@
     __pyx_v_index = values[0];
     __pyx_v_per_atom = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("get_energy", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 202, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.get_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_26get_energy(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_index, __pyx_v_per_atom);
+  __pyx_r = __pyx_pf_7mamonca_2MC_26get_energy(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_index, __pyx_v_per_atom);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_26get_energy(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom) {
+static PyObject *__pyx_pf_7mamonca_2MC_26get_energy(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   double __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_energy", 0);
 
-  /* "mc.pyx":207
+  /* "mamonca/mc.pyx":207
  *                 Energy value of current snapshot in eV
  *         """
  *         if per_atom:             # <<<<<<<<<<<<<<
  *             return self.c_mc.get_energy(index)/self.c_mc.get_number_of_atoms()
  *         return self.c_mc.get_energy(index)
  */
   __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_per_atom); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 207, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mc.pyx":208
+    /* "mamonca/mc.pyx":208
  *         """
  *         if per_atom:
  *             return self.c_mc.get_energy(index)/self.c_mc.get_number_of_atoms()             # <<<<<<<<<<<<<<
  *         return self.c_mc.get_energy(index)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4336,69 +4339,69 @@
     }
     __pyx_t_4 = PyFloat_FromDouble((__pyx_t_3 / ((double)__pyx_t_2))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "mc.pyx":207
+    /* "mamonca/mc.pyx":207
  *                 Energy value of current snapshot in eV
  *         """
  *         if per_atom:             # <<<<<<<<<<<<<<
  *             return self.c_mc.get_energy(index)/self.c_mc.get_number_of_atoms()
  *         return self.c_mc.get_energy(index)
  */
   }
 
-  /* "mc.pyx":209
+  /* "mamonca/mc.pyx":209
  *         if per_atom:
  *             return self.c_mc.get_energy(index)/self.c_mc.get_number_of_atoms()
  *         return self.c_mc.get_energy(index)             # <<<<<<<<<<<<<<
  * 
  *     def get_mean_energy(self, index=0, per_atom=False):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 209, __pyx_L1_error)
   __pyx_t_4 = PyFloat_FromDouble(__pyx_v_self->c_mc.get_energy(__pyx_t_2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":202
+  /* "mamonca/mc.pyx":202
  *         return self.c_mc.get_acceptance_ratio()
  * 
  *     def get_energy(self, index=0, per_atom=False):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("mc.MC.get_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":211
+/* "mamonca/mc.pyx":211
  *         return self.c_mc.get_energy(index)
  * 
  *     def get_mean_energy(self, index=0, per_atom=False):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_29get_mean_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_28get_mean_energy[] = "\n            Returns:\n                Mean energy value since the last reset (s. reset())\n        ";
-static PyObject *__pyx_pw_2mc_2MC_29get_mean_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_29get_mean_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_28get_mean_energy[] = "\n            Returns:\n                Mean energy value since the last reset (s. reset())\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_29get_mean_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_index = 0;
   PyObject *__pyx_v_per_atom = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4449,48 +4452,48 @@
     __pyx_v_index = values[0];
     __pyx_v_per_atom = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("get_mean_energy", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 211, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.get_mean_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_mean_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_28get_mean_energy(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_index, __pyx_v_per_atom);
+  __pyx_r = __pyx_pf_7mamonca_2MC_28get_mean_energy(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_index, __pyx_v_per_atom);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_28get_mean_energy(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom) {
+static PyObject *__pyx_pf_7mamonca_2MC_28get_mean_energy(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   double __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_mean_energy", 0);
 
-  /* "mc.pyx":216
+  /* "mamonca/mc.pyx":216
  *                 Mean energy value since the last reset (s. reset())
  *         """
  *         if per_atom:             # <<<<<<<<<<<<<<
  *             return self.c_mc.get_mean_energy(index)/self.c_mc.get_number_of_atoms()
  *         return self.c_mc.get_mean_energy(index)
  */
   __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_per_atom); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 216, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mc.pyx":217
+    /* "mamonca/mc.pyx":217
  *         """
  *         if per_atom:
  *             return self.c_mc.get_mean_energy(index)/self.c_mc.get_number_of_atoms()             # <<<<<<<<<<<<<<
  *         return self.c_mc.get_mean_energy(index)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4503,69 +4506,69 @@
     }
     __pyx_t_4 = PyFloat_FromDouble((__pyx_t_3 / ((double)__pyx_t_2))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 217, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "mc.pyx":216
+    /* "mamonca/mc.pyx":216
  *                 Mean energy value since the last reset (s. reset())
  *         """
  *         if per_atom:             # <<<<<<<<<<<<<<
  *             return self.c_mc.get_mean_energy(index)/self.c_mc.get_number_of_atoms()
  *         return self.c_mc.get_mean_energy(index)
  */
   }
 
-  /* "mc.pyx":218
+  /* "mamonca/mc.pyx":218
  *         if per_atom:
  *             return self.c_mc.get_mean_energy(index)/self.c_mc.get_number_of_atoms()
  *         return self.c_mc.get_mean_energy(index)             # <<<<<<<<<<<<<<
  * 
  *     def get_energy_variance(self, index=0, per_atom=False):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 218, __pyx_L1_error)
   __pyx_t_4 = PyFloat_FromDouble(__pyx_v_self->c_mc.get_mean_energy(__pyx_t_2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":211
+  /* "mamonca/mc.pyx":211
  *         return self.c_mc.get_energy(index)
  * 
  *     def get_mean_energy(self, index=0, per_atom=False):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("mc.MC.get_mean_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_mean_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":220
+/* "mamonca/mc.pyx":220
  *         return self.c_mc.get_mean_energy(index)
  * 
  *     def get_energy_variance(self, index=0, per_atom=False):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_31get_energy_variance(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_30get_energy_variance[] = "\n            Returns:\n                Energy variance since the last reset (s. reset())\n        ";
-static PyObject *__pyx_pw_2mc_2MC_31get_energy_variance(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_31get_energy_variance(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_30get_energy_variance[] = "\n            Returns:\n                Energy variance since the last reset (s. reset())\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_31get_energy_variance(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_index = 0;
   PyObject *__pyx_v_per_atom = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4616,48 +4619,48 @@
     __pyx_v_index = values[0];
     __pyx_v_per_atom = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("get_energy_variance", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 220, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.get_energy_variance", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_energy_variance", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_30get_energy_variance(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_index, __pyx_v_per_atom);
+  __pyx_r = __pyx_pf_7mamonca_2MC_30get_energy_variance(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_index, __pyx_v_per_atom);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_30get_energy_variance(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom) {
+static PyObject *__pyx_pf_7mamonca_2MC_30get_energy_variance(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_per_atom) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   double __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_energy_variance", 0);
 
-  /* "mc.pyx":225
+  /* "mamonca/mc.pyx":225
  *                 Energy variance since the last reset (s. reset())
  *         """
  *         if per_atom:             # <<<<<<<<<<<<<<
  *             return self.c_mc.get_energy_variance(index)/self.c_mc.get_number_of_atoms()
  *         return self.c_mc.get_energy_variance(index)
  */
   __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_per_atom); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 225, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "mc.pyx":226
+    /* "mamonca/mc.pyx":226
  *         """
  *         if per_atom:
  *             return self.c_mc.get_energy_variance(index)/self.c_mc.get_number_of_atoms()             # <<<<<<<<<<<<<<
  *         return self.c_mc.get_energy_variance(index)
  * 
  */
     __Pyx_XDECREF(__pyx_r);
@@ -4670,90 +4673,90 @@
     }
     __pyx_t_4 = PyFloat_FromDouble((__pyx_t_3 / ((double)__pyx_t_2))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "mc.pyx":225
+    /* "mamonca/mc.pyx":225
  *                 Energy variance since the last reset (s. reset())
  *         """
  *         if per_atom:             # <<<<<<<<<<<<<<
  *             return self.c_mc.get_energy_variance(index)/self.c_mc.get_number_of_atoms()
  *         return self.c_mc.get_energy_variance(index)
  */
   }
 
-  /* "mc.pyx":227
+  /* "mamonca/mc.pyx":227
  *         if per_atom:
  *             return self.c_mc.get_energy_variance(index)/self.c_mc.get_number_of_atoms()
  *         return self.c_mc.get_energy_variance(index)             # <<<<<<<<<<<<<<
  * 
  *     def revoke_qmc(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 227, __pyx_L1_error)
   __pyx_t_4 = PyFloat_FromDouble(__pyx_v_self->c_mc.get_energy_variance(__pyx_t_2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":220
+  /* "mamonca/mc.pyx":220
  *         return self.c_mc.get_mean_energy(index)
  * 
  *     def get_energy_variance(self, index=0, per_atom=False):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("mc.MC.get_energy_variance", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_energy_variance", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":229
+/* "mamonca/mc.pyx":229
  *         return self.c_mc.get_energy_variance(index)
  * 
  *     def revoke_qmc(self):             # <<<<<<<<<<<<<<
  *         self.set_eta(1)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_33revoke_qmc(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_2mc_2MC_33revoke_qmc(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7mamonca_2MC_33revoke_qmc(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_7mamonca_2MC_33revoke_qmc(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("revoke_qmc (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_32revoke_qmc(((struct __pyx_obj_2mc_MC *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7mamonca_2MC_32revoke_qmc(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_32revoke_qmc(struct __pyx_obj_2mc_MC *__pyx_v_self) {
+static PyObject *__pyx_pf_7mamonca_2MC_32revoke_qmc(struct __pyx_obj_7mamonca_MC *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("revoke_qmc", 0);
 
-  /* "mc.pyx":230
+  /* "mamonca/mc.pyx":230
  * 
  *     def revoke_qmc(self):
  *         self.set_eta(1)             # <<<<<<<<<<<<<<
  * 
  *     def set_lambda(self, val):
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_eta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 230, __pyx_L1_error)
@@ -4771,72 +4774,72 @@
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_int_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_int_1);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mc.pyx":229
+  /* "mamonca/mc.pyx":229
  *         return self.c_mc.get_energy_variance(index)
  * 
  *     def revoke_qmc(self):             # <<<<<<<<<<<<<<
  *         self.set_eta(1)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("mc.MC.revoke_qmc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.revoke_qmc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":232
+/* "mamonca/mc.pyx":232
  *         self.set_eta(1)
  * 
  *     def set_lambda(self, val):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_35set_lambda(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
-static char __pyx_doc_2mc_2MC_34set_lambda[] = "\n            Args:\n                val (float): Lambda value for thermodynamic integration\n        ";
-static PyObject *__pyx_pw_2mc_2MC_35set_lambda(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
+static PyObject *__pyx_pw_7mamonca_2MC_35set_lambda(PyObject *__pyx_v_self, PyObject *__pyx_v_val); /*proto*/
+static char __pyx_doc_7mamonca_2MC_34set_lambda[] = "\n            Args:\n                val (float): Lambda value for thermodynamic integration\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_35set_lambda(PyObject *__pyx_v_self, PyObject *__pyx_v_val) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_lambda (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_34set_lambda(((struct __pyx_obj_2mc_MC *)__pyx_v_self), ((PyObject *)__pyx_v_val));
+  __pyx_r = __pyx_pf_7mamonca_2MC_34set_lambda(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), ((PyObject *)__pyx_v_val));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_34set_lambda(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_val) {
+static PyObject *__pyx_pf_7mamonca_2MC_34set_lambda(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_val) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_lambda", 0);
 
-  /* "mc.pyx":237
+  /* "mamonca/mc.pyx":237
  *                 val (float): Lambda value for thermodynamic integration
  *         """
  *         if val<0 or val>1:             # <<<<<<<<<<<<<<
  *             raise ValueError("Lambda value has to be between 0 and 1")
  *         self.c_mc.set_lambda(val)
  */
   __pyx_t_2 = PyObject_RichCompare(__pyx_v_val, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
@@ -4850,108 +4853,108 @@
   __pyx_t_2 = PyObject_RichCompare(__pyx_v_val, __pyx_int_1, Py_GT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
   __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 237, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "mc.pyx":238
+    /* "mamonca/mc.pyx":238
  *         """
  *         if val<0 or val>1:
  *             raise ValueError("Lambda value has to be between 0 and 1")             # <<<<<<<<<<<<<<
  *         self.c_mc.set_lambda(val)
  * 
  */
     __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 238, __pyx_L1_error)
 
-    /* "mc.pyx":237
+    /* "mamonca/mc.pyx":237
  *                 val (float): Lambda value for thermodynamic integration
  *         """
  *         if val<0 or val>1:             # <<<<<<<<<<<<<<
  *             raise ValueError("Lambda value has to be between 0 and 1")
  *         self.c_mc.set_lambda(val)
  */
   }
 
-  /* "mc.pyx":239
+  /* "mamonca/mc.pyx":239
  *         if val<0 or val>1:
  *             raise ValueError("Lambda value has to be between 0 and 1")
  *         self.c_mc.set_lambda(val)             # <<<<<<<<<<<<<<
  * 
  *     def select_id(self, indices):
  */
   __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_val); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 239, __pyx_L1_error)
   try {
     __pyx_v_self->c_mc.set_lambda(__pyx_t_4);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 239, __pyx_L1_error)
   }
 
-  /* "mc.pyx":232
+  /* "mamonca/mc.pyx":232
  *         self.set_eta(1)
  * 
  *     def set_lambda(self, val):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("mc.MC.set_lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.set_lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":241
+/* "mamonca/mc.pyx":241
  *         self.c_mc.set_lambda(val)
  * 
  *     def select_id(self, indices):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_37select_id(PyObject *__pyx_v_self, PyObject *__pyx_v_indices); /*proto*/
-static char __pyx_doc_2mc_2MC_36select_id[] = "\n            Args:\n                indices (list): list of id's that can be chosen\n        ";
-static PyObject *__pyx_pw_2mc_2MC_37select_id(PyObject *__pyx_v_self, PyObject *__pyx_v_indices) {
+static PyObject *__pyx_pw_7mamonca_2MC_37select_id(PyObject *__pyx_v_self, PyObject *__pyx_v_indices); /*proto*/
+static char __pyx_doc_7mamonca_2MC_36select_id[] = "\n            Args:\n                indices (list): list of id's that can be chosen\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_37select_id(PyObject *__pyx_v_self, PyObject *__pyx_v_indices) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("select_id (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_36select_id(((struct __pyx_obj_2mc_MC *)__pyx_v_self), ((PyObject *)__pyx_v_indices));
+  __pyx_r = __pyx_pf_7mamonca_2MC_36select_id(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), ((PyObject *)__pyx_v_indices));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_36select_id(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_indices) {
+static PyObject *__pyx_pf_7mamonca_2MC_36select_id(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_indices) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   std::vector<int>  __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("select_id", 0);
 
-  /* "mc.pyx":246
+  /* "mamonca/mc.pyx":246
  *                 indices (list): list of id's that can be chosen
  *         """
  *         self.c_mc.select_id(np.array(indices).tolist())             # <<<<<<<<<<<<<<
  * 
  *     def get_steps_per_second(self):
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
@@ -4997,15 +5000,15 @@
   try {
     __pyx_v_self->c_mc.select_id(__pyx_t_5);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 246, __pyx_L1_error)
   }
 
-  /* "mc.pyx":241
+  /* "mamonca/mc.pyx":241
  *         self.c_mc.set_lambda(val)
  * 
  *     def select_id(self, indices):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
@@ -5013,58 +5016,58 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("mc.MC.select_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.select_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":248
+/* "mamonca/mc.pyx":248
  *         self.c_mc.select_id(np.array(indices).tolist())
  * 
  *     def get_steps_per_second(self):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_39get_steps_per_second(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_2mc_2MC_38get_steps_per_second[] = "\n            Returns:\n                Number of MC steps performed per second\n        ";
-static PyObject *__pyx_pw_2mc_2MC_39get_steps_per_second(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7mamonca_2MC_39get_steps_per_second(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7mamonca_2MC_38get_steps_per_second[] = "\n            Returns:\n                Number of MC steps performed per second\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_39get_steps_per_second(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_steps_per_second (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_38get_steps_per_second(((struct __pyx_obj_2mc_MC *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7mamonca_2MC_38get_steps_per_second(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_38get_steps_per_second(struct __pyx_obj_2mc_MC *__pyx_v_self) {
+static PyObject *__pyx_pf_7mamonca_2MC_38get_steps_per_second(struct __pyx_obj_7mamonca_MC *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_steps_per_second", 0);
 
-  /* "mc.pyx":253
+  /* "mamonca/mc.pyx":253
  *                 Number of MC steps performed per second
  *         """
  *         return np.rint(self.c_mc.get_steps_per_second()).astype(int)             # <<<<<<<<<<<<<<
  * 
  *     def set_magnitude(self, dm, dphi, flip=1):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -5109,49 +5112,49 @@
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":248
+  /* "mamonca/mc.pyx":248
  *         self.c_mc.select_id(np.array(indices).tolist())
  * 
  *     def get_steps_per_second(self):             # <<<<<<<<<<<<<<
  *         """
  *             Returns:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("mc.MC.get_steps_per_second", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_steps_per_second", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":255
+/* "mamonca/mc.pyx":255
  *         return np.rint(self.c_mc.get_steps_per_second()).astype(int)
  * 
  *     def set_magnitude(self, dm, dphi, flip=1):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_41set_magnitude(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_40set_magnitude[] = "\n            Args:\n                dm (float/list/ndarray): Magnitude variation strength. If a single value is set,\n                    the same value is used for all the atoms (applies to dphi and dtheta)\n                dphi (float/list/ndarray): Phi variation strength\n                dtheta (float/list/ndarray): Theta variation strength\n\n            Comment:\n                MC algorithm proposes a new magnetic moment by\n\n                m_new = abs(m_old+dm*random_number)\n                phi_new = phi_old+dphi*2*PI*random_number;\n\n                where random_number is a random number between -1 and 1.\n        ";
-static PyObject *__pyx_pw_2mc_2MC_41set_magnitude(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_41set_magnitude(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_40set_magnitude[] = "\n            Args:\n                dm (float/list/ndarray): Magnitude variation strength. If a single value is set,\n                    the same value is used for all the atoms (applies to dphi and dtheta)\n                dphi (float/list/ndarray): Phi variation strength\n                dtheta (float/list/ndarray): Theta variation strength\n\n            Comment:\n                MC algorithm proposes a new magnetic moment by\n\n                m_new = abs(m_old+dm*random_number)\n                phi_new = phi_old+dphi*2*PI*random_number;\n\n                where random_number is a random number between -1 and 1.\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_41set_magnitude(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_dm = 0;
   PyObject *__pyx_v_dphi = 0;
   PyObject *__pyx_v_flip = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -5209,26 +5212,26 @@
     __pyx_v_dphi = values[1];
     __pyx_v_flip = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("set_magnitude", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 255, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.set_magnitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.set_magnitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_40set_magnitude(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_dm, __pyx_v_dphi, __pyx_v_flip);
+  __pyx_r = __pyx_pf_7mamonca_2MC_40set_magnitude(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_dm, __pyx_v_dphi, __pyx_v_flip);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_40set_magnitude(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_dm, PyObject *__pyx_v_dphi, PyObject *__pyx_v_flip) {
+static PyObject *__pyx_pf_7mamonca_2MC_40set_magnitude(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_dm, PyObject *__pyx_v_dphi, PyObject *__pyx_v_flip) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -5242,15 +5245,15 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_magnitude", 0);
   __Pyx_INCREF(__pyx_v_dm);
   __Pyx_INCREF(__pyx_v_dphi);
   __Pyx_INCREF(__pyx_v_flip);
 
-  /* "mc.pyx":271
+  /* "mamonca/mc.pyx":271
  *                 where random_number is a random number between -1 and 1.
  *         """
  *         dm = np.array([dm]).flatten()             # <<<<<<<<<<<<<<
  *         dphi = np.array([dphi]).flatten()
  *         flip = np.array([flip]).flatten()
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
@@ -5296,15 +5299,15 @@
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF_SET(__pyx_v_dm, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "mc.pyx":272
+  /* "mamonca/mc.pyx":272
  *         """
  *         dm = np.array([dm]).flatten()
  *         dphi = np.array([dphi]).flatten()             # <<<<<<<<<<<<<<
  *         flip = np.array([flip]).flatten()
  *         if len(dm)==1:
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 272, __pyx_L1_error)
@@ -5350,15 +5353,15 @@
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_dphi, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "mc.pyx":273
+  /* "mamonca/mc.pyx":273
  *         dm = np.array([dm]).flatten()
  *         dphi = np.array([dphi]).flatten()
  *         flip = np.array([flip]).flatten()             # <<<<<<<<<<<<<<
  *         if len(dm)==1:
  *             dm = np.array(self.c_mc.get_number_of_atoms()*dm.tolist())
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 273, __pyx_L1_error)
@@ -5404,26 +5407,26 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF_SET(__pyx_v_flip, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "mc.pyx":274
+  /* "mamonca/mc.pyx":274
  *         dphi = np.array([dphi]).flatten()
  *         flip = np.array([flip]).flatten()
  *         if len(dm)==1:             # <<<<<<<<<<<<<<
  *             dm = np.array(self.c_mc.get_number_of_atoms()*dm.tolist())
  *         if len(dphi)==1:
  */
   __pyx_t_6 = PyObject_Length(__pyx_v_dm); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 274, __pyx_L1_error)
   __pyx_t_7 = ((__pyx_t_6 == 1) != 0);
   if (__pyx_t_7) {
 
-    /* "mc.pyx":275
+    /* "mamonca/mc.pyx":275
  *         flip = np.array([flip]).flatten()
  *         if len(dm)==1:
  *             dm = np.array(self.c_mc.get_number_of_atoms()*dm.tolist())             # <<<<<<<<<<<<<<
  *         if len(dphi)==1:
  *             dphi = np.array(self.c_mc.get_number_of_atoms()*dphi.tolist())
  */
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L1_error)
@@ -5469,35 +5472,35 @@
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_dm, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "mc.pyx":274
+    /* "mamonca/mc.pyx":274
  *         dphi = np.array([dphi]).flatten()
  *         flip = np.array([flip]).flatten()
  *         if len(dm)==1:             # <<<<<<<<<<<<<<
  *             dm = np.array(self.c_mc.get_number_of_atoms()*dm.tolist())
  *         if len(dphi)==1:
  */
   }
 
-  /* "mc.pyx":276
+  /* "mamonca/mc.pyx":276
  *         if len(dm)==1:
  *             dm = np.array(self.c_mc.get_number_of_atoms()*dm.tolist())
  *         if len(dphi)==1:             # <<<<<<<<<<<<<<
  *             dphi = np.array(self.c_mc.get_number_of_atoms()*dphi.tolist())
  *         if len(flip)==1:
  */
   __pyx_t_6 = PyObject_Length(__pyx_v_dphi); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 276, __pyx_L1_error)
   __pyx_t_7 = ((__pyx_t_6 == 1) != 0);
   if (__pyx_t_7) {
 
-    /* "mc.pyx":277
+    /* "mamonca/mc.pyx":277
  *             dm = np.array(self.c_mc.get_number_of_atoms()*dm.tolist())
  *         if len(dphi)==1:
  *             dphi = np.array(self.c_mc.get_number_of_atoms()*dphi.tolist())             # <<<<<<<<<<<<<<
  *         if len(flip)==1:
  *             flip = np.array(self.c_mc.get_number_of_atoms()*flip.tolist())
  */
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
@@ -5543,35 +5546,35 @@
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_dphi, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "mc.pyx":276
+    /* "mamonca/mc.pyx":276
  *         if len(dm)==1:
  *             dm = np.array(self.c_mc.get_number_of_atoms()*dm.tolist())
  *         if len(dphi)==1:             # <<<<<<<<<<<<<<
  *             dphi = np.array(self.c_mc.get_number_of_atoms()*dphi.tolist())
  *         if len(flip)==1:
  */
   }
 
-  /* "mc.pyx":278
+  /* "mamonca/mc.pyx":278
  *         if len(dphi)==1:
  *             dphi = np.array(self.c_mc.get_number_of_atoms()*dphi.tolist())
  *         if len(flip)==1:             # <<<<<<<<<<<<<<
  *             flip = np.array(self.c_mc.get_number_of_atoms()*flip.tolist())
  *         self.c_mc.set_magnitude(dm, dphi, flip)
  */
   __pyx_t_6 = PyObject_Length(__pyx_v_flip); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 278, __pyx_L1_error)
   __pyx_t_7 = ((__pyx_t_6 == 1) != 0);
   if (__pyx_t_7) {
 
-    /* "mc.pyx":279
+    /* "mamonca/mc.pyx":279
  *             dphi = np.array(self.c_mc.get_number_of_atoms()*dphi.tolist())
  *         if len(flip)==1:
  *             flip = np.array(self.c_mc.get_number_of_atoms()*flip.tolist())             # <<<<<<<<<<<<<<
  *         self.c_mc.set_magnitude(dm, dphi, flip)
  * 
  */
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 279, __pyx_L1_error)
@@ -5617,24 +5620,24 @@
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_flip, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "mc.pyx":278
+    /* "mamonca/mc.pyx":278
  *         if len(dphi)==1:
  *             dphi = np.array(self.c_mc.get_number_of_atoms()*dphi.tolist())
  *         if len(flip)==1:             # <<<<<<<<<<<<<<
  *             flip = np.array(self.c_mc.get_number_of_atoms()*flip.tolist())
  *         self.c_mc.set_magnitude(dm, dphi, flip)
  */
   }
 
-  /* "mc.pyx":280
+  /* "mamonca/mc.pyx":280
  *         if len(flip)==1:
  *             flip = np.array(self.c_mc.get_number_of_atoms()*flip.tolist())
  *         self.c_mc.set_magnitude(dm, dphi, flip)             # <<<<<<<<<<<<<<
  * 
  *     def run_gradient_descent(self, max_iter=None, step_size=1, decrement=0.001, diff=1.0e-8):
  */
   __pyx_t_9 = __pyx_convert_vector_from_py_double(__pyx_v_dm); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 280, __pyx_L1_error)
@@ -5643,15 +5646,15 @@
   try {
     __pyx_v_self->c_mc.set_magnitude(__pyx_t_9, __pyx_t_10, __pyx_t_11);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 280, __pyx_L1_error)
   }
 
-  /* "mc.pyx":255
+  /* "mamonca/mc.pyx":255
  *         return np.rint(self.c_mc.get_steps_per_second()).astype(int)
  * 
  *     def set_magnitude(self, dm, dphi, flip=1):             # <<<<<<<<<<<<<<
  *         """
  *             Args:
  */
 
@@ -5661,37 +5664,37 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("mc.MC.set_magnitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.set_magnitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_dm);
   __Pyx_XDECREF(__pyx_v_dphi);
   __Pyx_XDECREF(__pyx_v_flip);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":282
+/* "mamonca/mc.pyx":282
  *         self.c_mc.set_magnitude(dm, dphi, flip)
  * 
  *     def run_gradient_descent(self, max_iter=None, step_size=1, decrement=0.001, diff=1.0e-8):             # <<<<<<<<<<<<<<
  *         """
  *             args:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_43run_gradient_descent(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_42run_gradient_descent[] = "\n            args:\n                max_iter (int): number of steps to perform\n                step_size (float): step size\n                decrement (float): decrement value\n        ";
-static PyObject *__pyx_pw_2mc_2MC_43run_gradient_descent(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_43run_gradient_descent(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_42run_gradient_descent[] = "\n            args:\n                max_iter (int): number of steps to perform\n                step_size (float): step size\n                decrement (float): decrement value\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_43run_gradient_descent(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_max_iter = 0;
   PyObject *__pyx_v_step_size = 0;
   PyObject *__pyx_v_decrement = 0;
   PyObject *__pyx_v_diff = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -5768,26 +5771,26 @@
     __pyx_v_decrement = values[2];
     __pyx_v_diff = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("run_gradient_descent", 0, 0, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 282, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.run_gradient_descent", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.run_gradient_descent", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_42run_gradient_descent(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_max_iter, __pyx_v_step_size, __pyx_v_decrement, __pyx_v_diff);
+  __pyx_r = __pyx_pf_7mamonca_2MC_42run_gradient_descent(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_max_iter, __pyx_v_step_size, __pyx_v_decrement, __pyx_v_diff);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_42run_gradient_descent(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_max_iter, PyObject *__pyx_v_step_size, PyObject *__pyx_v_decrement, PyObject *__pyx_v_diff) {
+static PyObject *__pyx_pf_7mamonca_2MC_42run_gradient_descent(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_max_iter, PyObject *__pyx_v_step_size, PyObject *__pyx_v_decrement, PyObject *__pyx_v_diff) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   double __pyx_t_5;
@@ -5796,47 +5799,47 @@
   double __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("run_gradient_descent", 0);
   __Pyx_INCREF(__pyx_v_max_iter);
 
-  /* "mc.pyx":289
+  /* "mamonca/mc.pyx":289
  *                 decrement (float): decrement value
  *         """
  *         if max_iter is None:             # <<<<<<<<<<<<<<
  *             max_iter = self.c_mc.get_number_of_atoms()**2;
  *         return self.c_mc.run_gradient_descent(max_iter, step_size, decrement, diff)
  */
   __pyx_t_1 = (__pyx_v_max_iter == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "mc.pyx":290
+    /* "mamonca/mc.pyx":290
  *         """
  *         if max_iter is None:
  *             max_iter = self.c_mc.get_number_of_atoms()**2;             # <<<<<<<<<<<<<<
  *         return self.c_mc.run_gradient_descent(max_iter, step_size, decrement, diff)
  * 
  */
     __pyx_t_3 = __Pyx_PyInt_From_long(__Pyx_pow_long(((long)__pyx_v_self->c_mc.get_number_of_atoms()), 2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF_SET(__pyx_v_max_iter, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "mc.pyx":289
+    /* "mamonca/mc.pyx":289
  *                 decrement (float): decrement value
  *         """
  *         if max_iter is None:             # <<<<<<<<<<<<<<
  *             max_iter = self.c_mc.get_number_of_atoms()**2;
  *         return self.c_mc.run_gradient_descent(max_iter, step_size, decrement, diff)
  */
   }
 
-  /* "mc.pyx":291
+  /* "mamonca/mc.pyx":291
  *         if max_iter is None:
  *             max_iter = self.c_mc.get_number_of_atoms()**2;
  *         return self.c_mc.run_gradient_descent(max_iter, step_size, decrement, diff)             # <<<<<<<<<<<<<<
  * 
  *     def set_metadynamics(
  */
   __Pyx_XDECREF(__pyx_r);
@@ -5852,46 +5855,46 @@
   }
   __pyx_t_3 = PyFloat_FromDouble(__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":282
+  /* "mamonca/mc.pyx":282
  *         self.c_mc.set_magnitude(dm, dphi, flip)
  * 
  *     def run_gradient_descent(self, max_iter=None, step_size=1, decrement=0.001, diff=1.0e-8):             # <<<<<<<<<<<<<<
  *         """
  *             args:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("mc.MC.run_gradient_descent", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.run_gradient_descent", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_max_iter);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":293
+/* "mamonca/mc.pyx":293
  *         return self.c_mc.run_gradient_descent(max_iter, step_size, decrement, diff)
  * 
  *     def set_metadynamics(             # <<<<<<<<<<<<<<
  *         self,
  *         max_range=4,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_45set_metadynamics(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_44set_metadynamics[] = "\n        Set metadynamics calculation. Currently only the average magnetization can be chosen as\n        the collective variable.\n\n        Args:\n            max_range (float): Maximum magnetization value (larger: less accurate; smaller:\n                potentially misses free energy minimum)\n            energy_increment (float): Energy increment (or prefactor) for the Gaussian histogram\n                (larger: less accurate; smaller: slower convergence)\n            length_scale (float): Magnetization length scale (or Gaussian smearing) (larger:\n                potentially smears out free energy minimum; smaller: MC could become unstable)\n            bins (int): Number of bins for histogram (larger: slower; smaller: less accurate)\n            cutoff (float): Cutoff value (in length_scale unit) above which the Gaussian smearing\n                is considered to be 0\n            use_derivative (bool): Use derivative information of metadynamics. This should be set\n                to True if the number of atoms is sufficiently high (>1000) and the MC step\n                magnitude is not too large (around 0.1). In other words, except for code testing,\n                it is unlikely that this should be set to False. If set to False, make sure that\n                the number of bins is large enough for the Metadynamics to make sense (it has to\n                be at least 10 x max_range x n_atoms / displacement_magnitude).\n        ";
-static PyObject *__pyx_pw_2mc_2MC_45set_metadynamics(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_45set_metadynamics(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_44set_metadynamics[] = "\n        Set metadynamics calculation. Currently only the average magnetization can be chosen as\n        the collective variable.\n\n        Args:\n            max_range (float): Maximum magnetization value (larger: less accurate; smaller:\n                potentially misses free energy minimum)\n            energy_increment (float): Energy increment (or prefactor) for the Gaussian histogram\n                (larger: less accurate; smaller: slower convergence)\n            length_scale (float): Magnetization length scale (or Gaussian smearing) (larger:\n                potentially smears out free energy minimum; smaller: MC could become unstable)\n            bins (int): Number of bins for histogram (larger: slower; smaller: less accurate)\n            cutoff (float): Cutoff value (in length_scale unit) above which the Gaussian smearing\n                is considered to be 0\n            use_derivative (bool): Use derivative information of metadynamics. This should be set\n                to True if the number of atoms is sufficiently high (>1000) and the MC step\n                magnitude is not too large (around 0.1). In other words, except for code testing,\n                it is unlikely that this should be set to False. If set to False, make sure that\n                the number of bins is large enough for the Metadynamics to make sense (it has to\n                be at least 10 x max_range x n_atoms / displacement_magnitude).\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_45set_metadynamics(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_max_range = 0;
   PyObject *__pyx_v_energy_increment = 0;
   PyObject *__pyx_v_length_scale = 0;
   PyObject *__pyx_v_bins = 0;
   PyObject *__pyx_v_cutoff = 0;
   PyObject *__pyx_v_use_derivative = 0;
   int __pyx_lineno = 0;
@@ -5905,15 +5908,15 @@
     PyObject* values[6] = {0,0,0,0,0,0};
     values[0] = ((PyObject *)__pyx_int_4);
     values[1] = ((PyObject *)__pyx_float_1eneg_3);
     values[2] = ((PyObject *)__pyx_float_0_1);
     values[3] = ((PyObject *)__pyx_int_100);
     values[4] = ((PyObject *)__pyx_int_5);
 
-    /* "mc.pyx":300
+    /* "mamonca/mc.pyx":300
  *         bins=100,
  *         cutoff=5,
  *         use_derivative=True,             # <<<<<<<<<<<<<<
  *     ):
  *         """
  */
     values[5] = ((PyObject *)Py_True);
@@ -6002,34 +6005,34 @@
     __pyx_v_cutoff = values[4];
     __pyx_v_use_derivative = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("set_metadynamics", 0, 0, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 293, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.set_metadynamics", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.set_metadynamics", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_44set_metadynamics(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_max_range, __pyx_v_energy_increment, __pyx_v_length_scale, __pyx_v_bins, __pyx_v_cutoff, __pyx_v_use_derivative);
+  __pyx_r = __pyx_pf_7mamonca_2MC_44set_metadynamics(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_max_range, __pyx_v_energy_increment, __pyx_v_length_scale, __pyx_v_bins, __pyx_v_cutoff, __pyx_v_use_derivative);
 
-  /* "mc.pyx":293
+  /* "mamonca/mc.pyx":293
  *         return self.c_mc.run_gradient_descent(max_iter, step_size, decrement, diff)
  * 
  *     def set_metadynamics(             # <<<<<<<<<<<<<<
  *         self,
  *         max_range=4,
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_44set_metadynamics(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_max_range, PyObject *__pyx_v_energy_increment, PyObject *__pyx_v_length_scale, PyObject *__pyx_v_bins, PyObject *__pyx_v_cutoff, PyObject *__pyx_v_use_derivative) {
+static PyObject *__pyx_pf_7mamonca_2MC_44set_metadynamics(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_max_range, PyObject *__pyx_v_energy_increment, PyObject *__pyx_v_length_scale, PyObject *__pyx_v_bins, PyObject *__pyx_v_cutoff, PyObject *__pyx_v_use_derivative) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   double __pyx_t_4;
   double __pyx_t_5;
@@ -6038,52 +6041,52 @@
   double __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_metadynamics", 0);
 
-  /* "mc.pyx":323
+  /* "mamonca/mc.pyx":323
  *                 be at least 10 x max_range x n_atoms / displacement_magnitude).
  *         """
  *         if bins < max_range/length_scale:             # <<<<<<<<<<<<<<
  *             raise ValueError('Number of bins too small for this length_scale and max_range')
  *         self.c_mc.set_metadynamics(
  */
   __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_v_max_range, __pyx_v_length_scale); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyObject_RichCompare(__pyx_v_bins, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "mc.pyx":324
+    /* "mamonca/mc.pyx":324
  *         """
  *         if bins < max_range/length_scale:
  *             raise ValueError('Number of bins too small for this length_scale and max_range')             # <<<<<<<<<<<<<<
  *         self.c_mc.set_metadynamics(
  *             max_range, energy_increment, length_scale, bins, cutoff, use_derivative*1
  */
     __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 324, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 324, __pyx_L1_error)
 
-    /* "mc.pyx":323
+    /* "mamonca/mc.pyx":323
  *                 be at least 10 x max_range x n_atoms / displacement_magnitude).
  *         """
  *         if bins < max_range/length_scale:             # <<<<<<<<<<<<<<
  *             raise ValueError('Number of bins too small for this length_scale and max_range')
  *         self.c_mc.set_metadynamics(
  */
   }
 
-  /* "mc.pyx":326
+  /* "mamonca/mc.pyx":326
  *             raise ValueError('Number of bins too small for this length_scale and max_range')
  *         self.c_mc.set_metadynamics(
  *             max_range, energy_increment, length_scale, bins, cutoff, use_derivative*1             # <<<<<<<<<<<<<<
  *         )
  * 
  */
   __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_max_range); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
@@ -6092,62 +6095,62 @@
   __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_bins); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
   __pyx_t_8 = __pyx_PyFloat_AsDouble(__pyx_v_cutoff); if (unlikely((__pyx_t_8 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
   __pyx_t_2 = PyNumber_Multiply(__pyx_v_use_derivative, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "mc.pyx":325
+  /* "mamonca/mc.pyx":325
  *         if bins < max_range/length_scale:
  *             raise ValueError('Number of bins too small for this length_scale and max_range')
  *         self.c_mc.set_metadynamics(             # <<<<<<<<<<<<<<
  *             max_range, energy_increment, length_scale, bins, cutoff, use_derivative*1
  *         )
  */
   try {
     __pyx_v_self->c_mc.set_metadynamics(__pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9);
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 325, __pyx_L1_error)
   }
 
-  /* "mc.pyx":293
+  /* "mamonca/mc.pyx":293
  *         return self.c_mc.run_gradient_descent(max_iter, step_size, decrement, diff)
  * 
  *     def set_metadynamics(             # <<<<<<<<<<<<<<
  *         self,
  *         max_range=4,
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("mc.MC.set_metadynamics", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.set_metadynamics", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":329
+/* "mamonca/mc.pyx":329
  *         )
  * 
  *     def get_metadynamics_free_energy(self, derivative=False):             # <<<<<<<<<<<<<<
  *         """
  *         Get free energy of the metadynamics simulation
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_47get_metadynamics_free_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_46get_metadynamics_free_energy[] = "\n        Get free energy of the metadynamics simulation\n\n        Args:\n            derivative (bool): Whether to return the derivative values (only available if\n                derivative is used for metadynamics).\n\n        Returns:\n            (dict) Containing ndarray of 'magnetization' and 'free_energy'\n        ";
-static PyObject *__pyx_pw_2mc_2MC_47get_metadynamics_free_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_47get_metadynamics_free_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_46get_metadynamics_free_energy[] = "\n        Get free energy of the metadynamics simulation\n\n        Args:\n            derivative (bool): Whether to return the derivative values (only available if\n                derivative is used for metadynamics).\n\n        Returns:\n            (dict) Containing ndarray of 'magnetization' and 'free_energy'\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_47get_metadynamics_free_energy(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_derivative = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_metadynamics_free_energy (wrapper)", 0);
@@ -6185,41 +6188,41 @@
     }
     __pyx_v_derivative = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("get_metadynamics_free_energy", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 329, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.get_metadynamics_free_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_metadynamics_free_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_46get_metadynamics_free_energy(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_derivative);
+  __pyx_r = __pyx_pf_7mamonca_2MC_46get_metadynamics_free_energy(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_derivative);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_46get_metadynamics_free_energy(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_derivative) {
+static PyObject *__pyx_pf_7mamonca_2MC_46get_metadynamics_free_energy(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_derivative) {
   PyObject *__pyx_v_data = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   std::vector<double>  __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_metadynamics_free_energy", 0);
 
-  /* "mc.pyx":340
+  /* "mamonca/mc.pyx":340
  *             (dict) Containing ndarray of 'magnetization' and 'free_energy'
  *         """
  *         data = np.array(self.c_mc.get_histogram(derivative*1)).reshape(2, -1, order='C')             # <<<<<<<<<<<<<<
  *         return {'magnetization': data[0], 'free_energy': -data[1]}
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
@@ -6264,15 +6267,15 @@
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__7, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "mc.pyx":341
+  /* "mamonca/mc.pyx":341
  *         """
  *         data = np.array(self.c_mc.get_histogram(derivative*1)).reshape(2, -1, order='C')
  *         return {'magnetization': data[0], 'free_energy': -data[1]}             # <<<<<<<<<<<<<<
  * 
  *     def switch_spin_dynamics(
  */
   __Pyx_XDECREF(__pyx_r);
@@ -6289,64 +6292,64 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_free_energy, __pyx_t_3) < 0) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "mc.pyx":329
+  /* "mamonca/mc.pyx":329
  *         )
  * 
  *     def get_metadynamics_free_energy(self, derivative=False):             # <<<<<<<<<<<<<<
  *         """
  *         Get free energy of the metadynamics simulation
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("mc.MC.get_metadynamics_free_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.get_metadynamics_free_energy", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":343
+/* "mamonca/mc.pyx":343
  *         return {'magnetization': data[0], 'free_energy': -data[1]}
  * 
  *     def switch_spin_dynamics(             # <<<<<<<<<<<<<<
  *         self, turn_on=True, damping_parameter=8.0e-3, delta_t=1.0e-3, rescale_mag=True
  *     ):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_49switch_spin_dynamics(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2mc_2MC_48switch_spin_dynamics[] = "\n        Turn on (or off) spin dynamics calculation\n\n        Args:\n            turn_on (bool): Turn on or off (turning it off means mc)\n            damping_parameter (float): damping parameter (default: 8.0e-3)\n            delta_t (float): time discretization in fs (default: 1.0e-3)\n            rescaler_mag (bool): Whether or not rescale the displacement magnitude. Not setting\n                it to True when spin dynamics on might rescale the time scale. This argument is\n                probably going to be removed in the near future.\n\n        The equations are based on this paper:\n        Ma, Pui-Wai, and S. L. Dudarev.\n        \"Longitudinal magnetic fluctuations in Langevin spin dynamics.\"\n        Physical Review B 86.5 (2012): 054416.\n        https://journals.aps.org/prb/pdf/10.1103/PhysRevB.86.054416\n        ";
-static PyObject *__pyx_pw_2mc_2MC_49switch_spin_dynamics(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7mamonca_2MC_49switch_spin_dynamics(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7mamonca_2MC_48switch_spin_dynamics[] = "\n        Turn on (or off) spin dynamics calculation\n\n        Args:\n            turn_on (bool): Turn on or off (turning it off means mc)\n            damping_parameter (float): damping parameter (default: 8.0e-3)\n            delta_t (float): time discretization in fs (default: 1.0e-3)\n            rescaler_mag (bool): Whether or not rescale the displacement magnitude. Not setting\n                it to True when spin dynamics on might rescale the time scale. This argument is\n                probably going to be removed in the near future.\n\n        The equations are based on this paper:\n        Ma, Pui-Wai, and S. L. Dudarev.\n        \"Longitudinal magnetic fluctuations in Langevin spin dynamics.\"\n        Physical Review B 86.5 (2012): 054416.\n        https://journals.aps.org/prb/pdf/10.1103/PhysRevB.86.054416\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_49switch_spin_dynamics(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_turn_on = 0;
   PyObject *__pyx_v_damping_parameter = 0;
   PyObject *__pyx_v_delta_t = 0;
   PyObject *__pyx_v_rescale_mag = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("switch_spin_dynamics (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_turn_on,&__pyx_n_s_damping_parameter,&__pyx_n_s_delta_t,&__pyx_n_s_rescale_mag,0};
     PyObject* values[4] = {0,0,0,0};
 
-    /* "mc.pyx":344
+    /* "mamonca/mc.pyx":344
  * 
  *     def switch_spin_dynamics(
  *         self, turn_on=True, damping_parameter=8.0e-3, delta_t=1.0e-3, rescale_mag=True             # <<<<<<<<<<<<<<
  *     ):
  *         """
  */
     values[0] = ((PyObject *)Py_True);
@@ -6416,46 +6419,46 @@
     __pyx_v_delta_t = values[2];
     __pyx_v_rescale_mag = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("switch_spin_dynamics", 0, 0, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 343, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("mc.MC.switch_spin_dynamics", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.switch_spin_dynamics", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2mc_2MC_48switch_spin_dynamics(((struct __pyx_obj_2mc_MC *)__pyx_v_self), __pyx_v_turn_on, __pyx_v_damping_parameter, __pyx_v_delta_t, __pyx_v_rescale_mag);
+  __pyx_r = __pyx_pf_7mamonca_2MC_48switch_spin_dynamics(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), __pyx_v_turn_on, __pyx_v_damping_parameter, __pyx_v_delta_t, __pyx_v_rescale_mag);
 
-  /* "mc.pyx":343
+  /* "mamonca/mc.pyx":343
  *         return {'magnetization': data[0], 'free_energy': -data[1]}
  * 
  *     def switch_spin_dynamics(             # <<<<<<<<<<<<<<
  *         self, turn_on=True, damping_parameter=8.0e-3, delta_t=1.0e-3, rescale_mag=True
  *     ):
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_48switch_spin_dynamics(struct __pyx_obj_2mc_MC *__pyx_v_self, PyObject *__pyx_v_turn_on, PyObject *__pyx_v_damping_parameter, PyObject *__pyx_v_delta_t, PyObject *__pyx_v_rescale_mag) {
+static PyObject *__pyx_pf_7mamonca_2MC_48switch_spin_dynamics(struct __pyx_obj_7mamonca_MC *__pyx_v_self, PyObject *__pyx_v_turn_on, PyObject *__pyx_v_damping_parameter, PyObject *__pyx_v_delta_t, PyObject *__pyx_v_rescale_mag) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   double __pyx_t_2;
   double __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("switch_spin_dynamics", 0);
 
-  /* "mc.pyx":363
+  /* "mamonca/mc.pyx":363
  *         https://journals.aps.org/prb/pdf/10.1103/PhysRevB.86.054416
  *         """
  *         self.c_mc.switch_spin_dynamics(1*turn_on, damping_parameter, delta_t, rescale_mag*1)             # <<<<<<<<<<<<<<
  * 
  *     def activate_debug(self):
  */
   __pyx_t_1 = PyNumber_Multiply(__pyx_int_1, __pyx_v_turn_on); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
@@ -6469,72 +6472,72 @@
   } catch(...) {
     __Pyx_CppExn2PyErr();
     __PYX_ERR(0, 363, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "mc.pyx":343
+  /* "mamonca/mc.pyx":343
  *         return {'magnetization': data[0], 'free_energy': -data[1]}
  * 
  *     def switch_spin_dynamics(             # <<<<<<<<<<<<<<
  *         self, turn_on=True, damping_parameter=8.0e-3, delta_t=1.0e-3, rescale_mag=True
  *     ):
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("mc.MC.switch_spin_dynamics", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.switch_spin_dynamics", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "mc.pyx":365
+/* "mamonca/mc.pyx":365
  *         self.c_mc.switch_spin_dynamics(1*turn_on, damping_parameter, delta_t, rescale_mag*1)
  * 
  *     def activate_debug(self):             # <<<<<<<<<<<<<<
  *         """
  *             Activate debug mode (not so helpful though...)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_51activate_debug(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_2mc_2MC_50activate_debug[] = "\n            Activate debug mode (not so helpful though...)\n        ";
-static PyObject *__pyx_pw_2mc_2MC_51activate_debug(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7mamonca_2MC_51activate_debug(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7mamonca_2MC_50activate_debug[] = "\n            Activate debug mode (not so helpful though...)\n        ";
+static PyObject *__pyx_pw_7mamonca_2MC_51activate_debug(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("activate_debug (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_50activate_debug(((struct __pyx_obj_2mc_MC *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7mamonca_2MC_50activate_debug(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_50activate_debug(struct __pyx_obj_2mc_MC *__pyx_v_self) {
+static PyObject *__pyx_pf_7mamonca_2MC_50activate_debug(struct __pyx_obj_7mamonca_MC *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("activate_debug", 0);
 
-  /* "mc.pyx":369
+  /* "mamonca/mc.pyx":369
  *             Activate debug mode (not so helpful though...)
  *         """
  *         self.c_mc.activate_debug()             # <<<<<<<<<<<<<<
  * 
  */
   __pyx_v_self->c_mc.activate_debug();
 
-  /* "mc.pyx":365
+  /* "mamonca/mc.pyx":365
  *         self.c_mc.switch_spin_dynamics(1*turn_on, damping_parameter, delta_t, rescale_mag*1)
  * 
  *     def activate_debug(self):             # <<<<<<<<<<<<<<
  *         """
  *             Activate debug mode (not so helpful though...)
  */
 
@@ -6548,27 +6551,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_53__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_2mc_2MC_53__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7mamonca_2MC_53__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_7mamonca_2MC_53__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_52__reduce_cython__(((struct __pyx_obj_2mc_MC *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7mamonca_2MC_52__reduce_cython__(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_52__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2mc_MC *__pyx_v_self) {
+static PyObject *__pyx_pf_7mamonca_2MC_52__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7mamonca_MC *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -6590,42 +6593,42 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("mc.MC.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_2mc_2MC_55__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_2mc_2MC_55__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7mamonca_2MC_55__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_7mamonca_2MC_55__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_2mc_2MC_54__setstate_cython__(((struct __pyx_obj_2mc_MC *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_7mamonca_2MC_54__setstate_cython__(((struct __pyx_obj_7mamonca_MC *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2mc_2MC_54__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2mc_MC *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7mamonca_2MC_54__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7mamonca_MC *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -6647,15 +6650,15 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("mc.MC.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("mamonca.MC.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "vector.from_py":45
@@ -6955,80 +6958,80 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_tp_new_2mc_MC(PyTypeObject *t, PyObject *a, PyObject *k) {
-  struct __pyx_obj_2mc_MC *p;
+static PyObject *__pyx_tp_new_7mamonca_MC(PyTypeObject *t, PyObject *a, PyObject *k) {
+  struct __pyx_obj_7mamonca_MC *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_2mc_MC *)o);
+  p = ((struct __pyx_obj_7mamonca_MC *)o);
   new((void*)&(p->c_mc)) cMC();
-  if (unlikely(__pyx_pw_2mc_2MC_1__cinit__(o, a, k) < 0)) goto bad;
+  if (unlikely(__pyx_pw_7mamonca_2MC_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_2mc_MC(PyObject *o) {
-  struct __pyx_obj_2mc_MC *p = (struct __pyx_obj_2mc_MC *)o;
+static void __pyx_tp_dealloc_7mamonca_MC(PyObject *o) {
+  struct __pyx_obj_7mamonca_MC *p = (struct __pyx_obj_7mamonca_MC *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->c_mc);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static PyMethodDef __pyx_methods_2mc_MC[] = {
-  {"set_landau_coeff", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_3set_landau_coeff, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_2set_landau_coeff},
-  {"set_heisenberg_coeff", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_5set_heisenberg_coeff, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_4set_heisenberg_coeff},
-  {"clear_heisenberg_coeff", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_7clear_heisenberg_coeff, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_6clear_heisenberg_coeff},
-  {"clear_landau_coeff", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_9clear_landau_coeff, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_8clear_landau_coeff},
-  {"clear_all_coeff", (PyCFunction)__pyx_pw_2mc_2MC_11clear_all_coeff, METH_NOARGS, __pyx_doc_2mc_2MC_10clear_all_coeff},
-  {"get_magnetic_gradients", (PyCFunction)__pyx_pw_2mc_2MC_13get_magnetic_gradients, METH_NOARGS, __pyx_doc_2mc_2MC_12get_magnetic_gradients},
-  {"get_magnetic_moments", (PyCFunction)__pyx_pw_2mc_2MC_15get_magnetic_moments, METH_NOARGS, __pyx_doc_2mc_2MC_14get_magnetic_moments},
-  {"set_magnetic_moments", (PyCFunction)__pyx_pw_2mc_2MC_17set_magnetic_moments, METH_O, __pyx_doc_2mc_2MC_16set_magnetic_moments},
-  {"get_magnetization", (PyCFunction)__pyx_pw_2mc_2MC_19get_magnetization, METH_NOARGS, __pyx_doc_2mc_2MC_18get_magnetization},
-  {"get_output", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_21get_output, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_20get_output},
-  {"run", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_23run, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_22run},
-  {"get_acceptance_ratio", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_25get_acceptance_ratio, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_24get_acceptance_ratio},
-  {"get_energy", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_27get_energy, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_26get_energy},
-  {"get_mean_energy", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_29get_mean_energy, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_28get_mean_energy},
-  {"get_energy_variance", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_31get_energy_variance, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_30get_energy_variance},
-  {"revoke_qmc", (PyCFunction)__pyx_pw_2mc_2MC_33revoke_qmc, METH_NOARGS, 0},
-  {"set_lambda", (PyCFunction)__pyx_pw_2mc_2MC_35set_lambda, METH_O, __pyx_doc_2mc_2MC_34set_lambda},
-  {"select_id", (PyCFunction)__pyx_pw_2mc_2MC_37select_id, METH_O, __pyx_doc_2mc_2MC_36select_id},
-  {"get_steps_per_second", (PyCFunction)__pyx_pw_2mc_2MC_39get_steps_per_second, METH_NOARGS, __pyx_doc_2mc_2MC_38get_steps_per_second},
-  {"set_magnitude", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_41set_magnitude, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_40set_magnitude},
-  {"run_gradient_descent", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_43run_gradient_descent, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_42run_gradient_descent},
-  {"set_metadynamics", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_45set_metadynamics, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_44set_metadynamics},
-  {"get_metadynamics_free_energy", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_47get_metadynamics_free_energy, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_46get_metadynamics_free_energy},
-  {"switch_spin_dynamics", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2mc_2MC_49switch_spin_dynamics, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2mc_2MC_48switch_spin_dynamics},
-  {"activate_debug", (PyCFunction)__pyx_pw_2mc_2MC_51activate_debug, METH_NOARGS, __pyx_doc_2mc_2MC_50activate_debug},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_2mc_2MC_53__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_2mc_2MC_55__setstate_cython__, METH_O, 0},
+static PyMethodDef __pyx_methods_7mamonca_MC[] = {
+  {"set_landau_coeff", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_3set_landau_coeff, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_2set_landau_coeff},
+  {"set_heisenberg_coeff", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_5set_heisenberg_coeff, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_4set_heisenberg_coeff},
+  {"clear_heisenberg_coeff", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_7clear_heisenberg_coeff, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_6clear_heisenberg_coeff},
+  {"clear_landau_coeff", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_9clear_landau_coeff, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_8clear_landau_coeff},
+  {"clear_all_coeff", (PyCFunction)__pyx_pw_7mamonca_2MC_11clear_all_coeff, METH_NOARGS, __pyx_doc_7mamonca_2MC_10clear_all_coeff},
+  {"get_magnetic_gradients", (PyCFunction)__pyx_pw_7mamonca_2MC_13get_magnetic_gradients, METH_NOARGS, __pyx_doc_7mamonca_2MC_12get_magnetic_gradients},
+  {"get_magnetic_moments", (PyCFunction)__pyx_pw_7mamonca_2MC_15get_magnetic_moments, METH_NOARGS, __pyx_doc_7mamonca_2MC_14get_magnetic_moments},
+  {"set_magnetic_moments", (PyCFunction)__pyx_pw_7mamonca_2MC_17set_magnetic_moments, METH_O, __pyx_doc_7mamonca_2MC_16set_magnetic_moments},
+  {"get_magnetization", (PyCFunction)__pyx_pw_7mamonca_2MC_19get_magnetization, METH_NOARGS, __pyx_doc_7mamonca_2MC_18get_magnetization},
+  {"get_output", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_21get_output, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_20get_output},
+  {"run", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_23run, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_22run},
+  {"get_acceptance_ratio", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_25get_acceptance_ratio, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_24get_acceptance_ratio},
+  {"get_energy", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_27get_energy, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_26get_energy},
+  {"get_mean_energy", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_29get_mean_energy, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_28get_mean_energy},
+  {"get_energy_variance", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_31get_energy_variance, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_30get_energy_variance},
+  {"revoke_qmc", (PyCFunction)__pyx_pw_7mamonca_2MC_33revoke_qmc, METH_NOARGS, 0},
+  {"set_lambda", (PyCFunction)__pyx_pw_7mamonca_2MC_35set_lambda, METH_O, __pyx_doc_7mamonca_2MC_34set_lambda},
+  {"select_id", (PyCFunction)__pyx_pw_7mamonca_2MC_37select_id, METH_O, __pyx_doc_7mamonca_2MC_36select_id},
+  {"get_steps_per_second", (PyCFunction)__pyx_pw_7mamonca_2MC_39get_steps_per_second, METH_NOARGS, __pyx_doc_7mamonca_2MC_38get_steps_per_second},
+  {"set_magnitude", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_41set_magnitude, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_40set_magnitude},
+  {"run_gradient_descent", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_43run_gradient_descent, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_42run_gradient_descent},
+  {"set_metadynamics", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_45set_metadynamics, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_44set_metadynamics},
+  {"get_metadynamics_free_energy", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_47get_metadynamics_free_energy, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_46get_metadynamics_free_energy},
+  {"switch_spin_dynamics", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7mamonca_2MC_49switch_spin_dynamics, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7mamonca_2MC_48switch_spin_dynamics},
+  {"activate_debug", (PyCFunction)__pyx_pw_7mamonca_2MC_51activate_debug, METH_NOARGS, __pyx_doc_7mamonca_2MC_50activate_debug},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_7mamonca_2MC_53__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_7mamonca_2MC_55__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_2mc_MC = {
+static PyTypeObject __pyx_type_7mamonca_MC = {
   PyVarObject_HEAD_INIT(0, 0)
-  "mc.MC", /*tp_name*/
-  sizeof(struct __pyx_obj_2mc_MC), /*tp_basicsize*/
+  "mamonca.MC", /*tp_name*/
+  sizeof(struct __pyx_obj_7mamonca_MC), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_2mc_MC, /*tp_dealloc*/
+  __pyx_tp_dealloc_7mamonca_MC, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -7053,25 +7056,25 @@
   "\n\n    Magnetic Metropolis Monte Carlo module. It does not have to work with pyiron, but for\n    convenience it is strongly recommended to do so. Here's a short example:\n\n    >>> from pyiron import Project\n    >>> from mc import MC\n    >>> \n    >>> structure = Project('.').create.structure.bulk(\n    >>>     name='Fe',\n    >>>     cubic=True\n    >>> )\n    >>> \n    >>> structure.set_repeat(10)\n    >>> J = 0.1 # eV\n    >>> neighbors = structure.get_neighbors()\n    >>> first_shell_tensor = neighbors.get_shell_matrix()[0]\n    >>> \n    >>> mc = MC(len(structure))\n    >>> mc.set_heisenberg_coeff(J*first_shell_tensor.toarray())\n    >>> \n    >>> mc.run(temperature=300, number_of_iterations=1000)\n\n    The results can be analysed by attributes like `get_mean_energy()` or\n    `get_magnetic_moments()`.\n\n    The Hamiltonian H is given in the form:\n\n    H = -0.5*sum_ij J_ij*(m_i*m_j)^deg + sum_i A_i*m_i^deg\n\n    The first coefficients (J_ij) can be inserted with set_heisenberg_coeff and the\n    magnitude dependent terms (A_i) can be set via set_landau_coeff. Beware of the signs for\n    the Heisenberg coefficients.\n    ", /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_2mc_MC, /*tp_methods*/
+  __pyx_methods_7mamonca_MC, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_2mc_MC, /*tp_new*/
+  __pyx_tp_new_7mamonca_MC, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -7094,25 +7097,25 @@
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_mc(PyObject* module); /*proto*/
+static int __pyx_pymod_exec_mamonca(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_mc},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_mamonca},
   {0, NULL}
 };
 #endif
 
 static struct PyModuleDef __pyx_moduledef = {
     PyModuleDef_HEAD_INIT,
-    "mc",
+    "mamonca",
     0, /* m_doc */
   #if CYTHON_PEP489_MULTI_PHASE_INIT
     0, /* m_size */
   #else
     -1, /* m_size */
   #endif
     __pyx_methods /* m_methods */,
@@ -7229,81 +7232,81 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "mc.pyx":67
+  /* "mamonca/mc.pyx":67
  *             coeff = np.tile(coeff, self.c_mc.get_number_of_atoms())
  *         if len(coeff)!=self.c_mc.get_number_of_atoms():
  *             raise ValueError('coeff has to be a single number or a list of length'             # <<<<<<<<<<<<<<
  *                              'corresponding to the number of atoms in the box')
  *         self.c_mc.set_landau_coeff(coeff, deg, index)
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_coeff_has_to_be_a_single_number); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "mc.pyx":89
+  /* "mamonca/mc.pyx":89
  *             n = self.c_mc.get_number_of_atoms()
  *             if np.array(coeff).shape!=(n, n):
  *                 raise ValueError(             # <<<<<<<<<<<<<<
  *                     'If i and j are not specified, coeff has to be a 2d tensor with the length '
  *                     + 'equal to the number of atoms in each direction.'
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_If_i_and_j_are_not_specified_coe); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "mc.pyx":101
+  /* "mamonca/mc.pyx":101
  *             coeff = np.tile(coeff, len(i))
  *         if len(coeff)!=len(i) or len(i)!=len(j):
  *             raise ValueError('Length of vectors not the same')             # <<<<<<<<<<<<<<
  *         self.c_mc.set_heisenberg_coeff(coeff, i, j, deg, index)
  * 
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_Length_of_vectors_not_the_same); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "mc.pyx":139
+  /* "mamonca/mc.pyx":139
  *         """
  *         m = self.c_mc.get_magnetic_gradients()
  *         return np.array(m).reshape(-1, 3)             # <<<<<<<<<<<<<<
  * 
  *     def get_magnetic_moments(self):
  */
   __pyx_tuple__4 = PyTuple_Pack(2, __pyx_int_neg_1, __pyx_int_3); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "mc.pyx":238
+  /* "mamonca/mc.pyx":238
  *         """
  *         if val<0 or val>1:
  *             raise ValueError("Lambda value has to be between 0 and 1")             # <<<<<<<<<<<<<<
  *         self.c_mc.set_lambda(val)
  * 
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_Lambda_value_has_to_be_between_0); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "mc.pyx":324
+  /* "mamonca/mc.pyx":324
  *         """
  *         if bins < max_range/length_scale:
  *             raise ValueError('Number of bins too small for this length_scale and max_range')             # <<<<<<<<<<<<<<
  *         self.c_mc.set_metadynamics(
  *             max_range, energy_increment, length_scale, bins, cutoff, use_derivative*1
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_Number_of_bins_too_small_for_thi); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "mc.pyx":340
+  /* "mamonca/mc.pyx":340
  *             (dict) Containing ndarray of 'magnetization' and 'free_energy'
  *         """
  *         data = np.array(self.c_mc.get_histogram(derivative*1)).reshape(2, -1, order='C')             # <<<<<<<<<<<<<<
  *         return {'magnetization': data[0], 'free_energy': -data[1]}
  * 
  */
   __pyx_tuple__7 = PyTuple_Pack(2, __pyx_int_2, __pyx_int_neg_1); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 340, __pyx_L1_error)
@@ -7391,24 +7394,24 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_2mc_MC) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7mamonca_MC) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_2mc_MC.tp_print = 0;
+  __pyx_type_7mamonca_MC.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2mc_MC.tp_dictoffset && __pyx_type_2mc_MC.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_2mc_MC.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7mamonca_MC.tp_dictoffset && __pyx_type_7mamonca_MC.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_7mamonca_MC.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MC, (PyObject *)&__pyx_type_2mc_MC) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2mc_MC) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  __pyx_ptype_2mc_MC = &__pyx_type_2mc_MC;
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MC, (PyObject *)&__pyx_type_7mamonca_MC) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7mamonca_MC) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_ptype_7mamonca_MC = &__pyx_type_7mamonca_MC;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -7451,19 +7454,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initmc(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initmc(void)
+__Pyx_PyMODINIT_FUNC initmamonca(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC initmamonca(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_mc(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_mc(void)
+__Pyx_PyMODINIT_FUNC PyInit_mamonca(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit_mamonca(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -7522,42 +7525,42 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_mc(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_mamonca(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'mc' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module 'mamonca' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_mc(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_mamonca(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -7586,15 +7589,15 @@
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("mc", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("mamonca", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
@@ -7604,22 +7607,22 @@
   Py_INCREF(__pyx_cython_runtime);
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_mc) {
+  if (__pyx_module_is_main_mamonca) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "mc")) {
-      if (unlikely(PyDict_SetItemString(modules, "mc", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "mamonca")) {
+      if (unlikely(PyDict_SetItemString(modules, "mamonca", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -7632,30 +7635,30 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "mc.pyx":5
- * from cMC cimport cMC as MCcpp
+  /* "mamonca/mc.pyx":5
+ * from mamonca.cMC cimport cMC as MCcpp
  * from libcpp.vector cimport vector
  * import numpy as np             # <<<<<<<<<<<<<<
  * 
  * cdef class MC:
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "mc.pyx":1
+  /* "mamonca/mc.pyx":1
  * # distutils: language = c++             # <<<<<<<<<<<<<<
  * 
- * from cMC cimport cMC as MCcpp
+ * from mamonca.cMC cimport cMC as MCcpp
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "vector.to_py":60
@@ -7669,19 +7672,19 @@
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init mc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init mamonca", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init mc");
+    PyErr_SetString(PyExc_ImportError, "init mamonca");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -8369,28 +8372,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
```

### Comparing `mamonca-0.0.5/mamonca/mc.pyx` & `mamonca-0.0.7/mamonca/mc.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # distutils: language = c++
 
-from cMC cimport cMC as MCcpp
+from mamonca.cMC cimport cMC as MCcpp
 from libcpp.vector cimport vector
 import numpy as np
 
 cdef class MC:
     """
 
     Magnetic Metropolis Monte Carlo module. It does not have to work with pyiron, but for
```

