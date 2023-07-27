# Comparing `tmp/entrain-0.0.1.tar.gz` & `tmp/entrain-0.0.2.tar.gz`

## Comparing `entrain-0.0.1.tar` & `entrain-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 entrain-0.0.1/.DS_Store
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 entrain-0.0.1/twine_pypi_publish.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 entrain-0.0.1/entrain/__init__.py
--rw-r--r--   0        0        0    27954 2020-02-02 00:00:00.000000 entrain-0.0.1/entrain/entrain_scvelo.py
--rw-r--r--   0        0        0    28119 2020-02-02 00:00:00.000000 entrain-0.0.1/entrain/entrain_spatial.py
--rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 entrain-0.0.1/entrain/entrain_spatial_plotting.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 entrain-0.0.1/pypath_log/pypath-f3et0.log
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 entrain-0.0.1/pypath_log/pypath-tinuo.log
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 entrain-0.0.1/pypath_log/pypath-wez26.log
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 entrain-0.0.1/.gitignore
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 entrain-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 entrain-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 entrain-0.0.2/.DS_Store
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 entrain-0.0.2/twine_pypi_publish.sh
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 entrain-0.0.2/entrain/__init__.py
+-rw-r--r--   0        0        0    27954 2020-02-02 00:00:00.000000 entrain-0.0.2/entrain/entrain_scvelo.py
+-rw-r--r--   0        0        0    28119 2020-02-02 00:00:00.000000 entrain-0.0.2/entrain/entrain_spatial.py
+-rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 entrain-0.0.2/entrain/entrain_spatial_plotting.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 entrain-0.0.2/pypath_log/pypath-f3et0.log
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 entrain-0.0.2/pypath_log/pypath-tinuo.log
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 entrain-0.0.2/pypath_log/pypath-wez26.log
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 entrain-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 entrain-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 entrain-0.0.2/PKG-INFO
```

### Comparing `entrain-0.0.1/.DS_Store` & `entrain-0.0.2/.DS_Store`

 * *Files 12% similar despite different names*

```diff
@@ -75,48 +75,48 @@
 000004a0: 0000 0004 0064 006f 0063 0073 6d6f 4444  .....d.o.c.smoDD
 000004b0: 626c 6f62 0000 0008 980f d644 3e06 c541  blob.......D>..A
 000004c0: 0000 0004 0064 006f 0063 0073 6d6f 6444  .....d.o.c.smodD
 000004d0: 626c 6f62 0000 0008 980f d644 3e06 c541  blob.......D>..A
 000004e0: 0000 0004 0064 006f 0063 0073 7068 3153  .....d.o.c.sph1S
 000004f0: 636f 6d70 0000 0000 0164 3000 0000 0007  comp.....d0.....
 00000500: 0065 006e 0074 0072 0061 0069 006e 6277  .e.n.t.r.a.i.nbw
-00000510: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
-00000520: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
+00000510: 7370 626c 6f62 0000 00b7 6270 6c69 7374  spblob....bplist
+00000520: 3030 d601 0203 0405 0607 0808 080b 085d  00.............]
 00000530: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00000540: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
 00000550: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
 00000560: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
 00000570: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-00000580: 6465 6261 7208 0908 095f 1018 7b7b 3237  debar...._..{{27
-00000590: 362c 2032 3236 7d2c 207b 3932 302c 2034  6, 226}, {920, 4
-000005a0: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
-000005b0: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
-000005c0: 000d 0000 0000 0000 0000 0000 0000 0000  ................
-000005d0: 008b 0000 0007 0065 006e 0074 0072 0061  .......e.n.t.r.a
-000005e0: 0069 006e 6c67 3153 636f 6d70 0000 0000  .i.nlg1Scomp....
-000005f0: 0001 1c10 0000 0007 0065 006e 0074 0072  .........e.n.t.r
-00000600: 0061 0069 006e 6d6f 4444 626c 6f62 0000  .a.i.nmoDDblob..
-00000610: 0008 015d 41fd 1d18 c541 0000 0007 0065  ...]A....A.....e
-00000620: 006e 0074 0072 0061 0069 006e 6d6f 6444  .n.t.r.a.i.nmodD
-00000630: 626c 6f62 0000 0008 015d 41fd 1d18 c541  blob.....]A....A
-00000640: 0000 0007 0065 006e 0074 0072 0061 0069  .....e.n.t.r.a.i
-00000650: 006e 7068 3153 636f 6d70 0000 0000 0001  .nph1Scomp......
-00000660: 6000 0000 0007 0065 006e 0074 0072 0061  `......e.n.t.r.a
-00000670: 0069 006e 7653 726e 6c6f 6e67 0000 0001  .i.nvSrnlong....
-00000680: 0000 000a 0070 0079 0070 0061 0074 0068  .....p.y.p.a.t.h
-00000690: 005f 006c 006f 0067 6c67 3153 636f 6d70  ._.l.o.glg1Scomp
-000006a0: 0000 0000 0000 27b7 0000 000a 0070 0079  ......'......p.y
-000006b0: 0070 0061 0074 0068 005f 006c 006f 0067  .p.a.t.h._.l.o.g
-000006c0: 6d6f 4444 626c 6f62 0000 0008 8333 3aa6  moDDblob.....3:.
-000006d0: 01ea c441 0000 000a 0070 0079 0070 0061  ...A.....p.y.p.a
-000006e0: 0074 0068 005f 006c 006f 0067 6d6f 6444  .t.h._.l.o.gmodD
-000006f0: 626c 6f62 0000 0008 8333 3aa6 01ea c441  blob.....3:....A
-00000700: 0000 000a 0070 0079 0070 0061 0074 0068  .....p.y.p.a.t.h
-00000710: 005f 006c 006f 0067 7068 3153 636f 6d70  ._.l.o.gph1Scomp
-00000720: 0000 0000 0000 3000 0000 0000 0000 0000  ......0.........
+00000580: 6465 6261 7208 0909 095f 1017 7b7b 3532  debar...._..{{52
+00000590: 2c20 3736 7d2c 207b 3136 3433 2c20 3633  , 76}, {1643, 63
+000005a0: 337d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  3}}...#/;R_klmno
+000005b0: 8900 0000 0000 0001 0100 0000 0000 0000  ................
+000005c0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
+000005d0: 8a00 0000 0700 6500 6e00 7400 7200 6100  ......e.n.t.r.a.
+000005e0: 6900 6e6c 6731 5363 6f6d 7000 0000 0000  i.nlg1Scomp.....
+000005f0: 011c 1000 0000 0700 6500 6e00 7400 7200  ........e.n.t.r.
+00000600: 6100 6900 6e6d 6f44 4462 6c6f 6200 0000  a.i.nmoDDblob...
+00000610: 0801 5d41 fd1d 18c5 4100 0000 0700 6500  ..]A....A.....e.
+00000620: 6e00 7400 7200 6100 6900 6e6d 6f64 4462  n.t.r.a.i.nmodDb
+00000630: 6c6f 6200 0000 0801 5d41 fd1d 18c5 4100  lob.....]A....A.
+00000640: 0000 0700 6500 6e00 7400 7200 6100 6900  ....e.n.t.r.a.i.
+00000650: 6e70 6831 5363 6f6d 7000 0000 0000 0160  nph1Scomp......`
+00000660: 0000 0000 0700 6500 6e00 7400 7200 6100  ......e.n.t.r.a.
+00000670: 6900 6e76 5372 6e6c 6f6e 6700 0000 0100  i.nvSrnlong.....
+00000680: 0000 0a00 7000 7900 7000 6100 7400 6800  ....p.y.p.a.t.h.
+00000690: 5f00 6c00 6f00 676c 6731 5363 6f6d 7000  _.l.o.glg1Scomp.
+000006a0: 0000 0000 0027 b700 0000 0a00 7000 7900  .....'......p.y.
+000006b0: 7000 6100 7400 6800 5f00 6c00 6f00 676d  p.a.t.h._.l.o.gm
+000006c0: 6f44 4462 6c6f 6200 0000 0883 333a a601  oDDblob.....3:..
+000006d0: eac4 4100 0000 0a00 7000 7900 7000 6100  ..A.....p.y.p.a.
+000006e0: 7400 6800 5f00 6c00 6f00 676d 6f64 4462  t.h._.l.o.gmodDb
+000006f0: 6c6f 6200 0000 0883 333a a601 eac4 4100  lob.....3:....A.
+00000700: 0000 0a00 7000 7900 7000 6100 7400 6800  ....p.y.p.a.t.h.
+00000710: 5f00 6c00 6f00 6770 6831 5363 6f6d 7000  _.l.o.gph1Scomp.
+00000720: 0000 0000 0030 0000 0000 0000 0000 0000  .....0..........
 00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `entrain-0.0.1/entrain/entrain_scvelo.py` & `entrain-0.0.2/entrain/entrain_scvelo.py`

 * *Files identical despite different names*

### Comparing `entrain-0.0.1/entrain/entrain_spatial.py` & `entrain-0.0.2/entrain/entrain_spatial.py`

 * *Files identical despite different names*

### Comparing `entrain-0.0.1/entrain/entrain_spatial_plotting.py` & `entrain-0.0.2/entrain/entrain_spatial_plotting.py`

 * *Files identical despite different names*

### Comparing `entrain-0.0.1/pypath_log/pypath-f3et0.log` & `entrain-0.0.2/pypath_log/pypath-f3et0.log`

 * *Files identical despite different names*

### Comparing `entrain-0.0.1/pypath_log/pypath-tinuo.log` & `entrain-0.0.2/pypath_log/pypath-tinuo.log`

 * *Files identical despite different names*

### Comparing `entrain-0.0.1/pypath_log/pypath-wez26.log` & `entrain-0.0.2/pypath_log/pypath-wez26.log`

 * *Files identical despite different names*

### Comparing `entrain-0.0.1/pyproject.toml` & `entrain-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "entrain"
-version = "0.0.1"
+version = "0.0.2"
 description = "A single-cell analysis package to elucidate environmental factors controlling cell differentiation in RNA velocity and spatial datasets."
 license = {text = "MIT License"}
 requires-python = ">=3.10"
 authors = [
   {name = "Wunna Kyaw", email = "wunna.a.kyaw@gmail.com"}
 ]
 maintainers = [
@@ -26,18 +26,15 @@
 keywords = ["RNA", "single cell", "differentiation", "bioinformatics", "ligand", "receptor", "velocity"]
 
 dependencies = [
     "anndata>=0.7.5",
     "scanpy>=1.5",
     "rpy2",
     "scvelo",
-    "squidpy",
-"scikit-learn",
-"matplotlib",
-"seaborn"
+    "squidpy"
 ]
 
 [project.optional-dependencies]
 labeltransfer = [
     "tangram-sc"
 ]
 ligandreceptor = [
```

### Comparing `entrain-0.0.1/PKG-INFO` & `entrain-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: entrain
-Version: 0.0.1
+Version: 0.0.2
 Summary: A single-cell analysis package to elucidate environmental factors controlling cell differentiation in RNA velocity and spatial datasets.
 Author-email: Wunna Kyaw <wunna.a.kyaw@gmail.com>
 Maintainer-email: Wunna Kyaw <wunna.a.kyaw@gmail.com>
 License: MIT License
 Keywords: RNA,bioinformatics,differentiation,ligand,receptor,single cell,velocity
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Requires-Dist: anndata>=0.7.5
-Requires-Dist: matplotlib
 Requires-Dist: rpy2
 Requires-Dist: scanpy>=1.5
-Requires-Dist: scikit-learn
 Requires-Dist: scvelo
-Requires-Dist: seaborn
 Requires-Dist: squidpy
 Provides-Extra: labeltransfer
 Requires-Dist: tangram-sc; extra == 'labeltransfer'
 Provides-Extra: ligandreceptor
 Requires-Dist: omnipath-pypath; extra == 'ligandreceptor'
```

