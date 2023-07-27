# Comparing `tmp/modvis-0.0.6.tar.gz` & `tmp/modvis-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modvis-0.0.6.tar", last modified: Tue Jun 14 19:36:38 2022, max compression
+gzip compressed data, was "modvis-0.0.7.tar", last modified: Thu Jul 27 20:20:04 2023, max compression
```

## Comparing `modvis-0.0.6.tar` & `modvis-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 shua784  (1520788915) PNL\Domain Users (2016721313)        0 2022-06-14 19:36:38.664477 modvis-0.0.6/
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)     1068 2022-05-04 19:51:52.000000 modvis-0.0.6/LICENSE
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)      122 2022-05-04 19:51:52.000000 modvis-0.0.6/MANIFEST.in
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)     2201 2022-06-14 19:36:38.664694 modvis-0.0.6/PKG-INFO
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)     1474 2022-05-19 20:45:37.000000 modvis-0.0.6/README.md
-drwxr-xr-x   0 shua784  (1520788915) PNL\Domain Users (2016721313)        0 2022-06-14 19:36:38.638120 modvis-0.0.6/modvis/
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)    32192 2022-06-13 19:31:13.000000 modvis-0.0.6/modvis/ATSutils.py
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)      125 2022-05-04 19:51:52.000000 modvis-0.0.6/modvis/__init__.py
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)    22370 2022-05-18 20:40:19.000000 modvis-0.0.6/modvis/ats_xdmf.py
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)     1219 2022-05-04 19:51:52.000000 modvis-0.0.6/modvis/colors.py
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)    18314 2022-06-14 18:52:52.000000 modvis-0.0.6/modvis/general_plots.py
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)       19 2022-05-04 19:51:52.000000 modvis-0.0.6/modvis/modvis.py
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)    20014 2022-05-04 19:51:52.000000 modvis-0.0.6/modvis/objectivefunctions.py
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)    23201 2022-05-18 21:23:49.000000 modvis-0.0.6/modvis/plot_vis_file.py
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)     7897 2022-05-18 20:39:35.000000 modvis-0.0.6/modvis/transect_data.py
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)    18215 2022-06-14 17:50:45.000000 modvis-0.0.6/modvis/utils.py
-drwxr-xr-x   0 shua784  (1520788915) PNL\Domain Users (2016721313)        0 2022-06-14 19:36:38.663751 modvis-0.0.6/modvis.egg-info/
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)     2201 2022-06-14 19:36:37.000000 modvis-0.0.6/modvis.egg-info/PKG-INFO
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)      451 2022-06-14 19:36:38.000000 modvis-0.0.6/modvis.egg-info/SOURCES.txt
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)      144 2022-06-14 19:36:37.000000 modvis-0.0.6/modvis.egg-info/dependency_links.txt
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)        1 2022-05-03 05:31:31.000000 modvis-0.0.6/modvis.egg-info/not-zip-safe
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)       70 2022-06-14 19:36:38.000000 modvis-0.0.6/modvis.egg-info/requires.txt
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)        7 2022-06-14 19:36:38.000000 modvis-0.0.6/modvis.egg-info/top_level.txt
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)      143 2022-06-14 19:35:17.000000 modvis-0.0.6/requirements.txt
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)      389 2022-06-14 19:36:38.666079 modvis-0.0.6/setup.cfg
--rw-r--r--   0 shua784  (1520788915) PNL\Domain Users (2016721313)     1684 2022-06-14 19:36:22.000000 modvis-0.0.6/setup.py
+drwxr-xr-x   0 shuai      (501) staff       (20)        0 2023-07-27 20:20:04.329650 modvis-0.0.7/
+-rw-r--r--   0 shuai      (501) staff       (20)     1068 2022-07-29 18:50:06.000000 modvis-0.0.7/LICENSE
+-rw-r--r--   0 shuai      (501) staff       (20)      122 2022-07-29 18:50:06.000000 modvis-0.0.7/MANIFEST.in
+-rw-r--r--   0 shuai      (501) staff       (20)     2516 2023-07-27 20:20:04.329723 modvis-0.0.7/PKG-INFO
+-rw-r--r--   0 shuai      (501) staff       (20)     1814 2023-05-25 20:09:30.000000 modvis-0.0.7/README.md
+drwxr-xr-x   0 shuai      (501) staff       (20)        0 2023-07-27 20:20:04.328395 modvis-0.0.7/modvis/
+-rw-r--r--   0 shuai      (501) staff       (20)    41362 2023-06-02 16:56:27.000000 modvis-0.0.7/modvis/ATSutils.py
+-rw-r--r--   0 shuai      (501) staff       (20)      125 2022-07-29 18:50:06.000000 modvis-0.0.7/modvis/__init__.py
+-rw-r--r--   0 shuai      (501) staff       (20)    24626 2023-07-27 20:01:25.000000 modvis-0.0.7/modvis/ats_xdmf.py
+-rw-r--r--   0 shuai      (501) staff       (20)    17039 2023-07-21 17:21:10.000000 modvis-0.0.7/modvis/ats_xml.py
+-rw-r--r--   0 shuai      (501) staff       (20)     1219 2022-11-22 22:46:43.000000 modvis-0.0.7/modvis/colors.py
+-rw-r--r--   0 shuai      (501) staff       (20)    19003 2023-05-24 18:15:14.000000 modvis-0.0.7/modvis/general_plots.py
+-rw-r--r--   0 shuai      (501) staff       (20)       19 2022-07-29 18:50:06.000000 modvis-0.0.7/modvis/modvis.py
+-rw-r--r--   0 shuai      (501) staff       (20)    20014 2022-07-29 18:50:06.000000 modvis-0.0.7/modvis/objectivefunctions.py
+-rw-r--r--   0 shuai      (501) staff       (20)    23201 2022-07-29 18:50:06.000000 modvis-0.0.7/modvis/plot_vis_file.py
+-rw-r--r--   0 shuai      (501) staff       (20)     7897 2022-07-29 18:50:06.000000 modvis-0.0.7/modvis/transect_data.py
+-rw-r--r--   0 shuai      (501) staff       (20)    21687 2023-06-02 16:52:26.000000 modvis-0.0.7/modvis/utils.py
+drwxr-xr-x   0 shuai      (501) staff       (20)        0 2023-07-27 20:20:04.329423 modvis-0.0.7/modvis.egg-info/
+-rw-r--r--   0 shuai      (501) staff       (20)     2516 2023-07-27 20:20:04.000000 modvis-0.0.7/modvis.egg-info/PKG-INFO
+-rw-r--r--   0 shuai      (501) staff       (20)      490 2023-07-27 20:20:04.000000 modvis-0.0.7/modvis.egg-info/SOURCES.txt
+-rw-r--r--   0 shuai      (501) staff       (20)      144 2023-07-27 20:20:04.000000 modvis-0.0.7/modvis.egg-info/dependency_links.txt
+-rw-r--r--   0 shuai      (501) staff       (20)        1 2022-11-17 20:27:10.000000 modvis-0.0.7/modvis.egg-info/not-zip-safe
+-rw-r--r--   0 shuai      (501) staff       (20)       70 2023-07-27 20:20:04.000000 modvis-0.0.7/modvis.egg-info/requires.txt
+-rw-r--r--   0 shuai      (501) staff       (20)        7 2023-07-27 20:20:04.000000 modvis-0.0.7/modvis.egg-info/top_level.txt
+-rw-r--r--   0 shuai      (501) staff       (20)      143 2022-07-29 18:50:06.000000 modvis-0.0.7/requirements.txt
+-rw-r--r--   0 shuai      (501) staff       (20)      389 2023-07-27 20:20:04.329970 modvis-0.0.7/setup.cfg
+-rw-r--r--   0 shuai      (501) staff       (20)     1679 2023-07-27 20:04:13.000000 modvis-0.0.7/setup.py
+drwxr-xr-x   0 shuai      (501) staff       (20)        0 2023-07-27 20:20:04.329528 modvis-0.0.7/tests/
+-rw-r--r--   0 shuai      (501) staff       (20)      382 2022-07-29 18:50:06.000000 modvis-0.0.7/tests/test_modvis.py
```

### Comparing `modvis-0.0.6/LICENSE` & `modvis-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modvis-0.0.6/PKG-INFO` & `modvis-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: modvis
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python package for model visualization.
 Home-page: https://github.com/pinshuai/modvis
 Author: Pin Shuai
-Author-email: pinshuai.phd@gmail.com
+Author-email: pin.shuai@usu.edu
 License: MIT license
 Keywords: modvis
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -45,14 +44,28 @@
 
 `ModVis` is available on PyPI. To install, run the following command:
 
 ```
 pip install modvis
 ```
 
+If you want to run the latest version of the code, you can install from git:
+
+```
+pip install -U git+https://github.com/pinshuai/modvis.git
+```
+
+Alternatively, if you want to debug and test the code, you can clone the repository and install from source:
+
+```
+git clone https://github.com/pinshuai/modvis.git
+cd modvis
+pip install -e .
+```
+
 ## Quick start
 
 To plot variables on the surface mesh:
 
 ```python
 import modvis.ats_xdmf as xdmf
 import modvis.plot_vis_file as pv
@@ -71,9 +84,7 @@
 
 
 ## Credits
 
 This work is supported by LDRD funding from PNNL.
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
-
-
```

### Comparing `modvis-0.0.6/README.md` & `modvis-0.0.7/modvis.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: modvis
+Version: 0.0.7
+Summary: A python package for model visualization.
+Home-page: https://github.com/pinshuai/modvis
+Author: Pin Shuai
+Author-email: pin.shuai@usu.edu
+License: MIT license
+Keywords: modvis
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ModVis
 
 
 [![image](https://img.shields.io/pypi/v/modvis.svg)](https://pypi.python.org/pypi/modvis)
 
 [![image](https://img.shields.io/conda/vn/conda-forge/modvis.svg)](https://anaconda.org/conda-forge/modvis)
 
@@ -23,14 +44,28 @@
 
 `ModVis` is available on PyPI. To install, run the following command:
 
 ```
 pip install modvis
 ```
 
+If you want to run the latest version of the code, you can install from git:
+
+```
+pip install -U git+https://github.com/pinshuai/modvis.git
+```
+
+Alternatively, if you want to debug and test the code, you can clone the repository and install from source:
+
+```
+git clone https://github.com/pinshuai/modvis.git
+cd modvis
+pip install -e .
+```
+
 ## Quick start
 
 To plot variables on the surface mesh:
 
 ```python
 import modvis.ats_xdmf as xdmf
 import modvis.plot_vis_file as pv
```

### Comparing `modvis-0.0.6/modvis/ATSutils.py` & `modvis-0.0.7/modvis/ATSutils.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,14 +22,48 @@
 
 colors = fcolors.colors('matplotlib')
 rho_m = 55500 # moles/m^3, water molar density
 # rho_m = 55000 # moles/m^3, water molar density. Make sure this is consistent with what's in the xml file!!
 rho = 997
 g = 9.80665
 
+def get_8dayET(obs_et, simu_et, dates):
+    """convert daily ET to cumulative 8-day ET using MODIS data
+    Parameters:
+        obs_et, dataframe with single column
+        simu_et, dataframe with single column
+        
+    Returns:
+        df_8d_et, dataframe with two columns: simu ET and obs ET (both in mm/8d)
+    """
+    df_et = simu_et.loc[dates[0]:dates[1]].copy()
+
+    # time_ind = df_et.dropna().index
+    time_ind = obs_et.loc[dates[0]:dates[1], :].index
+
+    # df_8d_et = df_et.dropna().copy()
+    df_8d_et = df_et.reindex(time_ind).copy()
+    for i in np.arange(len(time_ind))[:]:
+        itime = time_ind[i]
+        if i == 0:
+            btime = df_et.index[0]
+        else:
+            btime = time_ind[i-1]
+
+        istart = list(df_et.index).index(btime)
+        iend = list(df_et.index).index(itime)    
+        # `loc` includes both ends, but `iloc` does not include end bound!
+        isum = df_et.iloc[istart:iend+1, :].sum(min_count = 1) # return NA is sum() contains NA
+        df_8d_et.loc[itime, :] = isum.values    
+        
+    df_8d_et['obs ET [mm/8d]'] = obs_et.loc[time_ind[0] : time_ind[-1], :].values
+    df_8d_et.rename(columns = {df_8d_et.columns[0]:'simu ET [mm/8d]'}, inplace=True)
+    
+    return df_8d_et
+
 def get_snow_cover(model_dir, **kwargs):
     """Calculate snow cover data from model output. Return a dataframe with snow cover percentage.
     Parameters: 
         model_dir, str
             path to model directory
 
     Returns:
@@ -290,31 +324,36 @@
             splitline = re.split("\s+|,", line) 
             walltime = float(splitline[4])/3600 #convert s to h
 
     dt = np.array([float(i) for i in dt])
     assert len(dt) > 0, "0 timestep found!"
     time_dt = np.array([float(i) for i in time_dt])
     nyear = np.ptp(time_dt)/365 # cnvt d to year
+    logging.info(f"Start day: {time_dt[0]}d; End day: {time_dt[-1]}d; Finished simulation time: {nyear*365}d")
     
     step_dt = [float(i) for i in step_dt] 
     df = pd.DataFrame(np.stack([step_dt, dt, time_dt]).T, columns = ['cycle', 'timestep [d]', 'times [d]'])
     ave_dt = np.array(dt).mean()*24 # convert from day to hour
-    
+    logging.info(f"Average timestep: {ave_dt} h")
+
     # plot
     fig,ax = plt.subplots(1,1, figsize=(8,6))
-
     ax.plot(step_dt, dt, 'k', lw = 0.5)
     ax.set_ylabel('Timestep (day)')
     ax.set_xlabel('Cycle')
     ax.set_yscale('log')
     
     try:
         walltime_per_year = walltime / nyear
-        ax.set_title(f"Cores: {ncores}; wallclock time [h]: {walltime:.2f}; ave ts [h]: {ave_dt:.2f}; ave walltime/yr [h]: {walltime_per_year:.2f}")
+        title=f"Cores: {ncores}; wallclock time [h]: {walltime:.2f}; ave ts [h]: {ave_dt:.2f}; ave walltime/yr [h]: {walltime_per_year:.2f}"
+        ax.set_title(title)
+        logging.info(title)
+        
     except:
+        logging.info("Could not find total wallclock time. Job may not finish.")
         pass
 
     ax1 = ax.twinx()
     ax1.plot(step_dt, time_dt, 'r', lw=0.5)
     ax1.set_ylabel('Cumulative time (day)', color = 'red')
     ax1.tick_params('y', colors='r')   
     
@@ -327,16 +366,20 @@
 def rmLeapDays(time_ats, origin_date = "1980-01-01", noleap = True, freq = "D"):
     """remove Dec31 from leap years so that each year = 365 d. This applies to ATS and PRMS
     Parameters:
         time_ats: list
             list of days or hours
         origin_date: datetime str in "%Y-%m-%d", default is 1980-1-1
             original datetime. In ATS, this depends on the starting date of Daymet. 
+        noleap: bool, default is True
+            if True, remove Dec31 from leap years
+        freq: str, default is "D"
+            frequency of time_ats. Either "D" or "H"
     Returns:
-        datetime array with leap days removed.
+        datetime array.
     """
     # round to the nearest int, this maybe necessary for
     # floating point erros
     time_ats = np.rint(time_ats)
 
     if type(origin_date) is str:
         origin_date = datetime.strptime(origin_date, "%Y-%m-%d")
@@ -471,25 +514,29 @@
 
 
 def surfaceArea(model_dir):
     """get surface area of ATS model"""
     h5_files = glob.glob(os.path.join(model_dir, "*surface_data.h5"))
     if len(h5_files) == 1:
         with h5py.File(h5_files[0]) as f:
-            a_key = list(f['surface-cell_volume.cell.0'].keys())[0] # pick any timestamp
-            surface_area = f['surface-cell_volume.cell.0'][a_key][:].sum() # m^2  
+            keys = list(f.keys())
+            # find group name starts with 'surface-cell_volume'
+            groupname = np.array(keys)[[key.startswith('surface-cell_volume') for key in keys]][0]
+            a_key = list(f[groupname].keys())[0] # pick any timestamp
+            surface_area = f[groupname][a_key][:].sum() # m^2  
     else:
-        raise KeyError("*surface_data.h5 could not be found!")
+        path = os.path.join(model_dir, "*surface_data.h5")
+        raise KeyError(f"*surface_data.h5 could not be found in {path}!")
     return surface_area
     
 def load_waterBalance(model_dir, WB_filename = "water_balance.dat", timestep =
                       'D', UTC_time = None, resample_freq = None, canopy =
                       True, origin_date = "1980-01-01", noleap = True, cumsum = True,
                       restart_dir = None, out_file = None, plot = False,
-                      subcatchment=False, catchment_area=None,
+                      catchment_area=None,
                       **kwargs):
     """read ATS output files, new dataframe format
     Parameters:
         model_dir: str
             ATS model directory
         WB_filename: str
             water balance filename
@@ -510,24 +557,25 @@
         restart_dir: list or None
             If list, merge with restarted model output
         out_file: str or None
             If string, save water balance in a csv file.
         plot: bool,
             If true, plot water balance plots
     Returns:
-        datetime, data, and dataframe(datetime, data)
+        dataframe of model variables and/or a resampled dataframe.
     
     """
-    if subcatchment:
+    # get surface area
+    if catchment_area is not None:
         surface_area = catchment_area
     else:
         surface_area = surfaceArea(model_dir)
     assert(surface_area is not None)
 
-    df = load_output(model_dir, WB_filename, timestep, origin_date, **kwargs)
+    df = load_output(model_dir, WB_filename, timestep, origin_date, noleap=noleap, **kwargs)
     
     if restart_dir is not None:
         assert(type(restart_dir) is list)
         for idir in restart_dir:
             df_rst = load_output(idir, WB_filename, timestep, origin_date,
                                  **kwargs)
             if df.shape[-1] != df_rst.shape[-1]:
@@ -572,82 +620,180 @@
     df['snow precipitation [mm d^-1]'] = df['snow precipitation [m d^-1]']*1000
     df['snowmelt [mm d^-1]'] = df['snowmelt [m d^-1]']*1000
     df['watershed boundary discharge [m^3/d]'] = df['watershed boundary discharge [mol d^-1]'] / rho_m
     df['watershed boundary discharge [m/d]'] = df['watershed boundary discharge [m^3/d]'] / surface_area
     df["total evapotranspiration [mm d^-1]"] = df["total evapotranspiration [m d^-1]"] *1000         
     df['snow water content [m]'] = df['snow water content [mol]'] / rho_m / surface_area
     df['surface water content [m]'] = df['surface water content [mol]'] / rho_m / surface_area
-    df['subsurface water content [m]'] = df['subsurface water content [mol]'] / rho_m / surface_area        
+    df['subsurface water content [m]'] = df['subsurface water content [mol]'] / rho_m / surface_area     
+    df['exfiltration [m d^-1]'] = df['exfiltration [mol d^-1]'] / rho_m / surface_area
     if not canopy:            
         df['total water content [m]'] = df['surface water content [m]'] + df['subsurface water content [m]'] + df['snow water content [m]']
     else:
         df["canopy water content [m]"] = df["canopy water content [mol]"]/ rho_m / surface_area
-        df['(Ps_thru-SM-Es) [m/d]'] = df['snow to surface [m SWE d^-1]'] - df['snowmelt [m d^-1]'] -df['snow evaporation [m d^-1]']
+        # df['canopy interception [m d^-1]'] = np.zeros(len(df)) #DUMMY
+        # df['(Ps_thru-SM-Es) [m/d]'] = df['snow to surface [m SWE d^-1]'] - df['snowmelt [m d^-1]'] -df['snow evaporation [m d^-1]']
+        # df['(CanI-D-Ec) [m/d]'] = df['canopy interception [m d^-1]'] - df['canopy drainage [m d^-1]'] - df['canopy evaporation [m d^-1]']
         df['total water content [m]'] = df['surface water content [m]'] + df['subsurface water content [m]'] + df['snow water content [m]'] + df["canopy water content [m]"]
       
-    if "net groundwater flux [mol d^-1]" in df.columns:
-        df['(Pr+SM-ET-Q-gw) [m/d]'] = df['rain precipitation [m d^-1]'] + df['snowmelt [m d^-1]'] -\
-                            df['total evapotranspiration [m d^-1]'] - df['watershed boundary discharge [m/d]'] -\
-                            df['net groundwater flux [m/d]']
-        df['(Pr+Ps-ET-Q-gw) [m/d]'] = df['rain precipitation [m d^-1]'] + df['snow precipitation [m d^-1]'] -\
-                            df['total evapotranspiration [m d^-1]'] - df['watershed boundary discharge [m/d]'] -\
-                            df['net groundwater flux [m/d]']
+    # if "net groundwater flux [mol d^-1]" in df.columns:
+    #     df['(Pr+SM-ET-Q-gw) [m/d]'] = df['rain precipitation [m d^-1]'] + df['snowmelt [m d^-1]'] -\
+    #                         df['total evapotranspiration [m d^-1]'] - df['watershed boundary discharge [m/d]'] -\
+    #                         df['net groundwater flux [m/d]']
+    #     df['(Pr+Ps-ET-Q-gw) [m/d]'] = df['rain precipitation [m d^-1]'] + df['snow precipitation [m d^-1]'] -\
+    #                         df['total evapotranspiration [m d^-1]'] - df['watershed boundary discharge [m/d]'] -\
+    #                         df['net groundwater flux [m/d]']
     # calculate water balance
-    df['(Pr+SM-ET-Q) [m/d]'] = df['rain precipitation [m d^-1]'] + df['snowmelt [m d^-1]'] -\
-                        df['total evapotranspiration [m d^-1]'] - df['watershed boundary discharge [m/d]']
-    df['(Pr+Ps-ET-Q) [m/d]'] = df['rain precipitation [m d^-1]'] + df['snow precipitation [m d^-1]'] -\
-                        df['total evapotranspiration [m d^-1]'] - df['watershed boundary discharge [m/d]']
-    df['(Ps-SM) [m/d]'] = df['snow precipitation [m d^-1]'] - df['snowmelt [m d^-1]']
+    # df['(Pr+SM-ET-Q) [m/d]'] = df['rain precipitation [m d^-1]'] + df['snowmelt [m d^-1]'] -\
+    #                     df['total evapotranspiration [m d^-1]'] - df['watershed boundary discharge [m/d]']
+    # df['(Pr+Ps-ET-Q) [m/d]'] = df['rain precipitation [m d^-1]'] + df['snow precipitation [m d^-1]'] -\
+    #                     df['total evapotranspiration [m d^-1]'] - df['watershed boundary discharge [m/d]']
+    # df['(Ps-SM) [m/d]'] = df['snow precipitation [m d^-1]'] - df['snowmelt [m d^-1]']
 
     if resample_freq is not None:
         variables = ['rain precipitation [m d^-1]','snow precipitation [m d^-1]','snowmelt [m d^-1]', 'watershed boundary discharge [m/d]', 'watershed boundary discharge [m^3/d]', 'total evapotranspiration [m d^-1]', 'max ponded depth [m]', 'SWE [m]']
         df_rs = df.loc[:, variables].copy()
         logging.info(f"Resample to {resample_freq} frequency")
         df_rs = df_rs.resample(resample_freq).mean()
         df_rs.dropna(inplace = True)
         
         if UTC_time is not None:
             df_rs.index = df_rs.index.shift(UTC_time, freq = 'H')     
     
-    if cumsum:
+    # if cumsum:
         
-        if "net groundwater flux [mol d^-1]" in df.columns:
-            df["cum_groundwater flux [m]"] = df['net groundwater flux [m/d]'].cumsum()
-            df['cum_(Pr+Ps-ET-Q-gw) [m]'] = df['(Pr+Ps-ET-Q-gw) [m/d]'].cumsum()
+        # if "net groundwater flux [mol d^-1]" in df.columns:
+        #     df["cum_groundwater flux [m]"] = df['net groundwater flux [m/d]'].cumsum()
+        #     df['cum_(Pr+Ps-ET-Q-gw) [m]'] = df['(Pr+Ps-ET-Q-gw) [m/d]'].cumsum()
+        # if canopy:
+        #     # df['cum canopy mass change [m]'] = df["canopy water content [m]"].cumsum()
+        #     df['cum_canopy evaporation [m]'] = df['canopy evaporation [m d^-1]'].cumsum()
+        #     df['cum_canopy drainage [m]'] = df['canopy drainage [m d^-1]'].cumsum()
+        #     df['cum_canopy interception [m]'] = df['canopy interception [m d^-1]'].cumsum()
+        #     df['cum_snow evaporation [m]'] = df['snow evaporation [m d^-1]'].cumsum()
+        #     df["cum_snow to surface [m]"] = df['snow to surface [m SWE d^-1]'].cumsum()
+        #     df['cum_(CanI-D-Ec) [m]'] = df['(CanI-D-Ec) [m/d]'].cumsum()
+        #     df['cum_(Ps_thru-SM-Es) [m]'] = df['(Ps_thru-SM-Es) [m/d]'].cumsum()
+        #     df['cum_(P-Pt+S-St-Ec-drainage) [m]'] = (df['rain precipitation [m d^-1]'] - df["water to surface [m d^-1]"] + df["snow precipitation [m d^-1]"] - df["snow to surface [m SWE d^-1]"] - df["canopy evaporation [m d^-1]"] - df["canopy drainage [m d^-1]"]).cumsum()
+        # df["cum_rain precipitation [m]"] = df['rain precipitation [m d^-1]'].cumsum()
+        # df["cum_snow precipitation [m]"] = df['snow precipitation [m d^-1]'].cumsum()
+        # df["cum_snowmelt [m]"] = df['snowmelt [m d^-1]'].cumsum()
+        # df["cum_ET [m]"] = df["total evapotranspiration [m d^-1]"].cumsum()
+        # df['cum_overland flux [m]'] = df['watershed boundary discharge [m/d]'].cumsum()
+        # df['cum_(Pr+SM-ET-Q) [m]'] = df['(Pr+SM-ET-Q) [m/d]'].cumsum()
+        # df['cum_(Pr+Ps-ET-Q) [m]'] = df['(Pr+Ps-ET-Q) [m/d]'].cumsum()
+        # df['cum_(Ps-SM) [m]'] = df["(Ps-SM) [m/d]"].cumsum()
+        # df['cum canopy mass change [m]'] = df['canopy water content [m]'] - df['canopy water content [m]'].values[0]
+        # df['cum snow mass change [m]'] = df['snow water content [m]'] - df['snow water content [m]'].values[0]
+        # df['cum water mass change [m]'] = df['total water content [m]'] - df['total water content [m]'].values[0]
+
+        # if "net groundwater flux [mol d^-1]" in df.columns:
+        #     df['water mass error [m]'] = df['cum_(Pr+Ps-ET-Q-gw) [m]'] - df['cum water mass change [m]']
+        # else:
+        #     df['water mass error [m]'] = df['cum_(Pr+Ps-ET-Q) [m]'] - df['cum water mass change [m]']
+
+        # if not canopy:
+        #     df['snow mass error [m]'] = df['cum_(Ps-SM) [m]'] - df['cum snow mass change [m]']
+        # else:
+        #     df['snow mass error [m]'] = df['cum_(Ps_thru-SM-Es) [m]'] - df['cum snow mass change [m]']
+            
+    if plot:
+        # plot water balance
         if canopy:
-            df['cum canopy mass change [m]'] = df["canopy water content [m]"].cumsum()
-            df['cum_snow evaporation [m]'] = df['snow evaporation [m d^-1]'].cumsum()
-            df["cum_snow to surface [m]"] = df['snow to surface [m SWE d^-1]'].cumsum()
-            df['cum_(Ps_thru-SM-Es) [m]'] = df['(Ps_thru-SM-Es) [m/d]'].cumsum()
-            df['cum_(P-Pt+S-St-Ec-drainage) [m]'] = (df['rain precipitation [m d^-1]'] - df["water to surface [m d^-1]"] + df["snow precipitation [m d^-1]"] - df["snow to surface [m SWE d^-1]"] - df["canopy evaporation [m d^-1]"] - df["canopy drainage [m d^-1]"]).cumsum()
-        df["cum_rain precipitation [m]"] = df['rain precipitation [m d^-1]'].cumsum()
-        df["cum_snow precipitation [m]"] = df['snow precipitation [m d^-1]'].cumsum()
-        df["cum_snowmelt [m]"] = df['snowmelt [m d^-1]'].cumsum()
-        df["cum_ET [m]"] = df["total evapotranspiration [m d^-1]"].cumsum()
-        df['cum_overland flux [m]'] = df['watershed boundary discharge [m/d]'].cumsum()
-        df['cum_(Pr+SM-ET-Q) [m]'] = df['(Pr+SM-ET-Q) [m/d]'].cumsum()
-        df['cum_(Pr+Ps-ET-Q) [m]'] = df['(Pr+Ps-ET-Q) [m/d]'].cumsum()
-        df['cum_(Ps-SM) [m]'] = df["(Ps-SM) [m/d]"].cumsum()
-        df['cum snow mass change [m]'] = df['snow water content [m]'] - df['snow water content [m]'].values[0]
-        df['cum water mass change [m]'] = df['total water content [m]'] - df['total water content [m]'].values[0]
-
-        if "net groundwater flux [mol d^-1]" in df.columns:
-            df['water mass error [m]'] = df['cum_(Pr+Ps-ET-Q-gw) [m]'] - df['cum water mass change [m]']
+            domain_names = ['global', 'canopy', 'snow', 'surface', 'subsurface']
         else:
-            df['water mass error [m]'] = df['cum_(Pr+Ps-ET-Q) [m]'] - df['cum water mass change [m]']
+            domain_names = ['global', 'snow', 'surface', 'subsurface']
 
-        if not canopy:
-            df['snow mass error [m]'] = df['cum_(Ps-SM) [m]'] - df['cum snow mass change [m]']
-        else:
-            df['snow mass error [m]'] = df['cum_(Ps_thru-SM-Es) [m]'] - df['cum snow mass change [m]']
+        def cumu_plot(domain, df, ax):
+            """Plot cumulative fluxes
+            Parameters:
+            -----------
+                domain: str
+                    'global' or 'canopy' or 'snow' or 'surface' or 'subsurface'
+                df: pd.DataFrame
+                    dataframe containing fluxes
+                ax: matplotlib.axes
+                    axes to plot on
+
+            Water balances:
+                global: dWC/dt = Pr + Ps - ET - Q or dWC/dt = Pr + Ps - ET - Q - Gw (Pr: rain precipitation, Ps: snow precipitation, ET: evapotranspiration, Q: overland flow, Gw: groundwater flux)
+                canopy: dWC/dt = I - D - Ec (I: canopy interception, D: drainage, Ec: canopy evaporation)
+                snow: dWC/dt = S_thru+D - SM - Es (S_thru: snow throughfall, D: drainage, SM: snowmelt, Es: sublimation or snow evaporation)
+                surface: dWC/dt = R_thru+D - SM - E - Q - Inf (R_thru: rain throughfall, D: drainage, SM: snowmelt, E: surface evaporation, Q: overland flow, Inf: infiltration)
+                subsurface: dWC/dt = Inf - T or I - T - Gw (Inf: infiltration, T: transpiration, Gw: groundwater flux))   
+            """
+            time = df.index
+            fluxes = {}
+            if domain == "global":
+                fluxes['Pr'] = df['rain precipitation [m d^-1]']
+                fluxes['Ps'] = df['snow precipitation [m d^-1]']
+                fluxes['ET'] = df['total evapotranspiration [m d^-1]']
+                fluxes['Q'] = df['watershed boundary discharge [m/d]']
+                if "net groundwater flux [mol d^-1]" in df.columns:
+                    fluxes['Gw'] = df['net groundwater flux [m/d]']
+                    net_fluxes = fluxes['Pr'] + fluxes['Ps'] - fluxes['ET'] - fluxes['Q'] - fluxes['Gw']
+                else:
+                    net_fluxes = fluxes['Pr'] + fluxes['Ps'] - fluxes['ET'] - fluxes['Q']
+                water_content_change = df['total water content [m]'] - df['total water content [m]'].values[0]
+
+            if domain == 'canopy':
+                fluxes['I'] = df['canopy interception [m d^-1]']
+                fluxes['D'] = df['canopy drainage [m d^-1]']
+                fluxes['Ec'] = df['canopy evaporation [m d^-1]']
+                net_fluxes = fluxes['I'] - fluxes['D'] - fluxes['Ec']
+                water_content_change = df['canopy water content [m]'] - df['canopy water content [m]'].values[0]
+
+            if domain == 'snow':
+                fluxes['S_thru+D'] = df['snow to surface [m SWE d^-1]']
+                fluxes['Es'] = df['snow evaporation [m d^-1]']
+                fluxes['SM'] = df['snowmelt [m d^-1]']
+                net_fluxes = fluxes['S_thru+D'] - fluxes['Es'] - fluxes['SM']
+                water_content_change = df['snow water content [m]'] - df['snow water content [m]'].values[0]
+
+            if domain == 'surface':
+                fluxes['R_thru+D'] = df['water to surface [m d^-1]']
+                fluxes['SM'] = df['snowmelt [m d^-1]']
+                fluxes['E'] = df['surface evaporation [m d^-1]']
+                fluxes['Q'] = df['watershed boundary discharge [m/d]']
+                fluxes['Inf'] = -df['exfiltration [m d^-1]']
+                net_fluxes = fluxes['R_thru+D'] + fluxes['SM'] - fluxes['E'] - fluxes['Q'] - fluxes['Inf']
+                water_content_change = df['surface water content [m]'] - df['surface water content [m]'].values[0]
+
+            if domain == 'subsurface':
+                fluxes['Inf'] = -df['exfiltration [m d^-1]']
+                fluxes['T'] = df['transpiration [m d^-1]']
+                if "net groundwater flux [mol d^-1]" in df.columns:
+                    fluxes['Gw'] = df['net groundwater flux [m/d]']
+                    net_fluxes = fluxes['Inf'] - fluxes['T'] - fluxes['Gw']
+                else:
+                    net_fluxes = fluxes['Inf'] - fluxes['T']
+                water_content_change = df['subsurface water content [m]'] - df['subsurface water content [m]'].values[0]
+
+            error = np.cumsum(net_fluxes) - water_content_change
+            max_error = max(abs(error.max()), abs(error.min()))
+
+            for k,v in fluxes.items():
+                ax.plot(time, np.cumsum(v), label=k)
+
+            ax.plot(time, water_content_change, 'crimson', label='dW/dt')
+            ax.plot(time, np.cumsum(net_fluxes), 'k--', label='net fluxes')
+            ax.plot(time, error, '-.', color='grey', label='error')
+            ax.set_ylabel('CumFlux [m]')
+            ax.set_title(f'{domain} water balance (max error = {max_error*1000:.2f} mm)')
             
-    if plot:
-        
-        fig, axes = plt.subplots(3, 1, figsize=(8,8))
+            ax.set_xlim(df.index[0], df.index[-1])
+            ax.set_xlabel('')
+            ax.legend(loc='upper left', fontsize = 10, bbox_to_anchor = (1.0,1.15), frameon = False)
+            if domain != "subsurface":
+                ax.xaxis.set_ticklabels([])
 
+
+        fig, axes = plt.subplots(len(domain_names) + 1, 1, figsize=(8, 2.5*len(domain_names)))
+ 
+        # plot incoming and outgoing fluxes
         ax = axes[0]
         df.plot(y=["rain precipitation [m d^-1]", "snowmelt [m d^-1]" ], color
                 = colors[:2],
         ax = ax)
         ax1 = ax.twinx()
         if "river discharge [mol d^-1]" in df.columns:
             df.plot(y=["total evapotranspiration [m d^-1]", 
@@ -663,82 +809,105 @@
         ax1.legend(loc='upper left', fontsize = 10, bbox_to_anchor = (0.5,1.3),
                   frameon = False)
         ax.xaxis.set_ticklabels([])
         ax.invert_yaxis()
         ax.set_xlim(df.index[0], df.index[-1])
         ax.set_xlabel('')
 
-        ax = axes[1]
-        if "net groundwater flux [mol d^-1]" in df.columns:
-            df.plot(y=["cum_rain precipitation [m]", "cum_snow precipitation [m]", "cum_ET [m]", 
-                   "cum_overland flux [m]", "cum_groundwater flux [m]", 'cum_(Pr+Ps-ET-Q-gw) [m]'], ax = ax)
-        else:
-            df.plot(y=["cum_rain precipitation [m]", "cum_snow precipitation [m]", "cum_ET [m]", 
-                   "cum_overland flux [m]", 'cum_(Pr+Ps-ET-Q) [m]'], ax = ax)
-        df.plot(y = ['cum water mass change [m]', 'water mass error [m]'], style = ['-.','-'], color = ['k', 'grey'], ax = ax)
-        ax.set_ylabel('CumFlux [m]')
-        ax.legend(loc='upper left', fontsize = 10, bbox_to_anchor = (1.0,1.15), frameon = False)
-        max_error = max(abs(df['water mass error [m]'].max()), abs(df['water mass error [m]'].min()))
-#         print(max_error)
-        ax.set_title(f'max error = {max_error*1000:.2f} mm')
-        ax.xaxis.set_ticklabels([])
-        ax.set_xlim(df.index[0], df.index[-1])
-        ax.set_xlabel('')
 
-        ax = axes[2]
-        if not canopy:
-            df.plot(y=["cum_snow precipitation [m]", "cum_snowmelt [m]", 'cum_(Ps-SM) [m]'], ax = ax)
-            df.plot(y=['cum snow mass change [m]', 'snow mass error [m]'], style = ['-.','-'], color = ['k', 'grey'], ax = ax)
-        else:
-            df.plot(y=[ "cum_snow to surface [m]", "cum_snowmelt [m]", 'cum_snow evaporation [m]', 'cum_(Ps_thru-SM-Es) [m]'], ax=ax)
-            df.plot(y=['cum snow mass change [m]', 'snow mass error [m]'], style = ['-.','-'], color = ['k', 'grey'], ax = ax)
-        ax.set_ylabel('CumFlux [m]')
-        ax.legend(loc='upper left', fontsize = 10, bbox_to_anchor = (1.0,1.1), frameon = False)
-        max_error = max(abs(df['snow mass error [m]'].max()), abs(df['snow mass error [m]'].min()))
-        ax.set_title(f'max error = {max_error*1000:.2f} mm')
-        ax.set_xlim(df.index[0], df.index[-1])  
-        ax.set_xlabel('')
+
+        for i, domain in enumerate(domain_names):
+            ax = axes[i + 1]
+            cumu_plot(domain, df, ax)
+
+#         if "net groundwater flux [mol d^-1]" in df.columns:
+#             df.plot(y=["cum_rain precipitation [m]", "cum_snow precipitation [m]", "cum_ET [m]", 
+#                    "cum_overland flux [m]", "cum_groundwater flux [m]", 'cum_(Pr+Ps-ET-Q-gw) [m]'], ax = ax)
+#         else:
+#             df.plot(y=["cum_rain precipitation [m]", "cum_snow precipitation [m]", "cum_ET [m]", 
+#                    "cum_overland flux [m]", 'cum_(Pr+Ps-ET-Q) [m]'], ax = ax)
+#         df.plot(y = ['cum water mass change [m]', 'water mass error [m]'], style = ['-.','-'], color = ['k', 'grey'], ax = ax)
+#         ax.set_ylabel('CumFlux [m]')
+#         ax.legend(loc='upper left', fontsize = 10, bbox_to_anchor = (1.0,1.15), frameon = False)
+#         max_error = max(abs(df['water mass error [m]'].max()), abs(df['water mass error [m]'].min()))
+# #         print(max_error)
+#         ax.set_title(f'Total water balance (max error = {max_error*1000:.2f} mm)')
+#         ax.xaxis.set_ticklabels([])
+#         ax.set_xlim(df.index[0], df.index[-1])
+#         ax.set_xlabel('')
+
+        # plot canopy water balance
+        # dWC_canopy/dt = canopy_interception + canopy_drainage - canopy_evaporation
+        # ax = axes[2]
+        # if not canopy:
+        #     df.plot()
+        # else:
+        #     df.plot(y=[ "cum_canopy interception [m]", "cum_canopy drainage [m]", 'cum_canopy evaporation [m]', 'cum_(CanI) [m]'], ax=ax)
+        #     df.plot(y=['cum snow mass change [m]', 'snow mass error [m]'], style = ['-.','-'], color = ['k', 'grey'], ax = ax)
+        # ax.set_ylabel('CumFlux [m]')
+        # ax.legend(loc='upper left', fontsize = 10, bbox_to_anchor = (1.0,1.1), frameon = False)
+        # max_error = max(abs(df['snow mass error [m]'].max()), abs(df['snow mass error [m]'].min()))
+        # ax.set_title(f'Snow water balance (max error = {max_error*1000:.2f} mm'))
+        # ax.set_xlim(df.index[0], df.index[-1])  
+        # ax.set_xlabel('')
+
+        # # plot snow water balance
+        # ax = axes[3]
+        # if not canopy:
+        #     df.plot(y=["cum_snow precipitation [m]", "cum_snowmelt [m]", 'cum_(Ps-SM) [m]'], ax = ax)
+        #     df.plot(y=['cum snow mass change [m]', 'snow mass error [m]'], style = ['-.','-'], color = ['k', 'grey'], ax = ax)
+        # else:
+        #     df.plot(y=[ "cum_snow to surface [m]", "cum_snowmelt [m]", 'cum_snow evaporation [m]', 'cum_(Ps_thru-SM-Es) [m]'], ax=ax)
+        #     df.plot(y=['cum snow mass change [m]', 'snow mass error [m]'], style = ['-.','-'], color = ['k', 'grey'], ax = ax)
+        # ax.set_ylabel('CumFlux [m]')
+        # ax.legend(loc='upper left', fontsize = 10, bbox_to_anchor = (1.0,1.1), frameon = False)
+        # max_error = max(abs(df['snow mass error [m]'].max()), abs(df['snow mass error [m]'].min()))
+        # ax.set_title(f'Snow water balance (max error = {max_error*1000:.2f} mm'))
+        # ax.set_xlim(df.index[0], df.index[-1])  
+        # ax.set_xlabel('')
     
     if UTC_time is not None:
         df.index = df.index.shift(UTC_time, freq = 'H')         
     
     if out_file is not None:
         df.to_csv(out_file)
     
     if resample_freq is not None:
         return df, df_rs
     else:
         return df
 
 def load_output(model_dir, WB_filename, timestep = 'D', origin_date =
-                '1980-01-01', **kwargs):
+                '1980-01-01', noleap=True, **kwargs):
     """read ATS output files
     Parameters:
         model_dir: str
             ATS model directory
         WB_filename: str
             Waterbalance output filename, e.g. "water_balance.dat"
         timestep: str
-            timestep string, 'D', 'H'
+            timestep string, 'D', 'H'. Default is 'D'
         origin_date: str,
             origin of model time
+        noleap: bool
+            remove leap days or not. Default is True.
     Returns:
         datetime, data, and dataframe(datetime, data)
     
     """
     df = pd.read_csv(os.path.join(model_dir, WB_filename), comment='#')
     if timestep == 'D':
         # get datetime, convert seconds to days
-        datetime_noLeap = rmLeapDays(df['time [d]'], freq='D', origin_date =
-                                     origin_date, **kwargs)
+        datetime_ats = rmLeapDays(df['time [d]'], freq='D', origin_date =
+                                     origin_date, noleap=noleap, **kwargs)
     elif timestep == 'H':
-        datetime_noLeap = rmLeapDays(df['time [h]'], freq='H', origin_date =
-                                     origin_date, **kwargs)
+        datetime_ats = rmLeapDays(df['time [h]'], freq='H', origin_date =
+                                     origin_date, noleap=noleap, **kwargs)
     else:
         raise ValueError(f"Freq: {timestep} is not supported!")
-    df['datetime'] = datetime_noLeap
+    df['datetime'] = datetime_ats
     df.set_index('datetime', inplace=True, drop=True)
     
     return df
```

### Comparing `modvis-0.0.6/modvis/ats_xdmf.py` & `modvis-0.0.7/modvis/ats_xdmf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Functions for parsing Amanzi/ATS XDMF visualization files.
 
 This file was modified from https://github.com/amanzi/ats/tree/master/tools/utils. For questions, please contact the following author.
 
-Author: Ethan Coon (ecoon@ornl.gov)
+Authors: Ethan Coon (ecoon@ornl.gov)
+         Pin Shuai (pin.shuai@usu.edu)
 """
 import sys,os
 import numpy as np
 import h5py
 import matplotlib.collections
 import logging
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(name)s - %(levelname)s: %(message)s')
@@ -27,15 +28,15 @@
     if format is None:
         format = 'ats_vis_{}_mesh.h5'
     return valid_data_filename(domain, format)
 
 
 class VisFile:
     """Class managing the reading of ATS visualization files."""
-    def __init__(self, directory='.', domain=None, prefix='ats_vis', model_time_unit='yr', return_time_unit='d', load_mesh=False, **kwargs):
+    def __init__(self, directory='.', domain=None, prefix='ats_vis', model_time_unit='yr', return_time_unit='d', load_mesh=False, ats_version='dev', **kwargs):
         """Create a VisFile object.
 
         Parameters
         ----------
         directory : str, optional
           Directory containing vis files.  Default is '.'
         domain : str, optional
@@ -49,17 +50,17 @@
           Filename for the h5 mesh file.  Default is 'ats_vis_DOMAIN_mesh.h5'.
         model_time_unit: str, default is 'yr' 
           Time unit used for the h5 vis file. Default is year.
         return_time_unit: str, default is 'd'
           Time unit used for returned object self.times. Default is 'd'
         load_mesh, bool
             load mesh files if true. Default to False.
-        columnar, bool
-            If true, reorder 3D meshes to a "structured in z" mesh. Return shape of (ntriangles-per-layer, nlayers, ndim).
-            See loadMesh() for more information.
+        ats_version, str or float, optional. Default is 'dev'
+            Version of ats used in the simulations. Options include 'dev', '1.4', '1.3', '1.2'. 
+            This is used to parse the variable names. E.g., 'cell_volume' ('dev' version) vs 'cell_volume.cell.0' (older versions)
 
         Returns
         -------
         self : VisFile object
         """
         self.directory = directory
         self.domain = domain
@@ -67,76 +68,63 @@
         if self.domain is None:
             self.filename = f'{prefix}_data.h5'
             self.mesh_filename = f'{prefix}_mesh.h5'
         else:
             self.filename =f'{prefix}_{self.domain}_data.h5'
             self.mesh_filename = f'{prefix}_{self.domain}_mesh.h5'
 
-        # self.filename = filename
-        # if self.filename is None:
-        #     if self.domain is None:
-        #         self.filename = 'ats_vis_data.h5'
-        #     else:
-        #         self.filename = 'ats_vis_{}_data.h5'.format(self.domain)
-
-        # self.mesh_filename = mesh_filename
-        # if self.mesh_filename is None:
-        #     if self.domain is None:
-        #         self.mesh_filename = 'ats_vis_mesh.h5'
-        #     else:
-        #         self.mesh_filename = 'ats_vis_{}_mesh.h5'.format(self.domain)
-
         if model_time_unit == 'yr':
             if return_time_unit == 'yr':
                 time_factor = 1.0
             elif return_time_unit == 'noleap':
                 time_factor = 365.25 / 365
             elif return_time_unit == 'd':
                 time_factor = 365.25
             elif return_time_unit == 'hr':
                 time_factor = 365.25 * 24
             elif return_time_unit == 's':
                 time_factor = 365.25 * 24 * 3600
             else:
-                raise ValueError("Invalid time unit '{}': must be one of 'yr', 'noleap', 'd', 'hr', or 's'".format(return_time_unit))
+                raise ValueError("Invalid return time unit '{}': must be one of 'yr', 'noleap', 'd', 'hr', or 's'".format(return_time_unit))
         elif model_time_unit == 'd':
             if return_time_unit == 'yr':
                 time_factor = 1.0 / 365.25
             elif return_time_unit == 'noleap':
                 time_factor = 1.0 / 365
             elif return_time_unit == 'd':
                 time_factor = 1.0
             elif return_time_unit == 'hr':
                 time_factor = 24
             elif return_time_unit == 's':
                 time_factor = 24 * 3600
             else:
-                raise ValueError("Invalid time unit '{}': must be one of 'yr', 'noleap', 'd', 'hr', or 's'".format(return_time_unit))
-
+                raise ValueError("Invalid return time unit '{}': must be one of 'yr', 'noleap', 'd', 'hr', or 's'".format(return_time_unit))
+        else:
+            raise ValueError("Invalid model time unit '{}': must be one of 'yr', 'd'".format(model_time_unit))
         self.time_factor = time_factor
         self.time_unit = return_time_unit
 
         self.fname = os.path.join(self.directory, self.filename)
         if not os.path.isfile(self.fname):
             raise RuntimeError("Cannot load ATS XDMF h5 file at: {}".format(self.fname))
         self.d = h5py.File(self.fname,'r')
         self.loadTimes()
         self.map = None
-
+        self.version = ats_version
         if load_mesh:
             self.loadMesh(**kwargs)
             etype, vertex_coords, conn = meshXYZ(self.directory, self.mesh_filename)
             self.etype = etype
             self.vertex_xyz = np.array(list(vertex_coords.values()))
-            self.conn = conn
+            self.conn = conn        
         
     def __enter__(self):
         return self
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(self):
         self.close()
 
     def close(self):
         self.d.close()
 
     def loadTimes(self):
         """(Re-)loads the list of cycles and times."""
@@ -235,24 +223,24 @@
         -------
         variable_name : str
           Variable name mangled like it is used in Amanzi/ATS.  Something like
           'DOMAIN-vname.cell.0'
         """
         if self.domain and '-' not in vname:
             vname = self.domain + '-' + vname
-        if '.' not in vname:
+        if self.version != 'dev' and self.version < 1.4 and '.' not in vname:
             vname = vname + '.cell.0'
         return vname
 
     def _get(self, vname, cycle):
         """Private get: assumes vname is fully resolved, and does not deal with maps."""
         try:
             return self.d[vname][cycle][:,0]
         except KeyError:
-            logging.warning(f"cycle {cycle} not found in HDF5 file! Return Nans.")
+            logging.warning(f"{vname}/{cycle} not found in {self.fname}! Return Nans. Double check your variable name and cycle number, and make sure they exist in the HDF5 file.")
             self.loadMesh()
             return self.centroids.shape[0]*[np.nan] 
     
     def get(self, vname, cycle):
         """Access a data member.
 
         Parameters
@@ -269,15 +257,14 @@
 
         """
         val = self._get(self.variable(vname), cycle)
         if self.map is None:
             return val
         else:
             return reorder(val, self.map)
-        return 
 
     def getArray(self, vname):
         """Access an array of all cycle values.
 
         Parameters
         ----------
         vname : str
@@ -288,15 +275,15 @@
         value : np.ndarray
           Array of values of shape (n_cycles, n_elems)
         """
         vname = self.variable(vname)
         logging.debug(f"get variable: {vname}")
         # if vname does not exist, raise an error!
         if vname not in list(self.d.keys()):
-            raise RuntimeError(f"Variable: {vname} is not found in vis file!")
+            raise RuntimeError(f"Variable: {vname} is not found in {self.fname}! Double check the spelling of the variable and make sure it exists!")
         val = np.array([self._get(vname, k) for k in self.cycles])
         if self.map is None:
             return val
         else:
             return reorder(val, self.map)
             
     
@@ -310,14 +297,25 @@
           the first cycle's value.
         order : list(str), optional
           See arguments to structuredOrdering().  If provided, this
           reorders the data, and all future get() and getArray() calls will
           return data in this order.
         round : int
           Decimal places to round centroids to.  Supports sorting.
+        shape : list(int), optional
+          See arguments to structuredOrdering().  If provided, this
+          reorders the data, and all future get() and getArray() calls will
+          return data in this order.
+        columnar : bool, optional
+          If True, this sets order = ['x', 'y', 'z'] and shape is guessed by
+          assuming (x,y) coordinates are constant in map-view and cells
+          are vertical columns, a typical mesh layout generated by Watershed-Workflow.
+        round : int, optional
+          Number of decimals to round to -- this avoids roundoff issues in sorting.
+
         """
         if cycle is None:
             cycle = self.cycles[0]
         
         centroids = meshElemCentroids(self.directory, self.mesh_filename, cycle, round)
         if order is None and shape is None and not columnar:
             self.map = None
@@ -337,18 +335,20 @@
         self.mesh_elem_info = mesh_elems
         self.polygon_coordinates = meshElemPolygons(*mesh_elems)
 
     def getMeshPolygons(self, edgecolor='k', cmap='jet', linewidth=1):
         polygons = matplotlib.collections.PolyCollection(self.polygon_coordinates, edgecolor=edgecolor, cmap=cmap, linewidths=linewidth)
         return polygons
     
-elem_type = {5:'QUAD',
+elem_type = {3:'POLYGON',
+             5:'QUAD',
              8:'PRISM',
              9:'HEX',
-             4:'TRIANGLE'
+             4:'TRIANGLE',
+             16:'POLYHEDRON'
              }
 
 def meshXYZ(directory=".", filename="ats_vis_mesh.h5", key=None):
     """Reads a mesh nodal coordinates and connectivity.
 
     Note this only currently works for fixed structure meshes, i.e. not
     arbitrary polyhedra.
@@ -388,26 +388,79 @@
             nnodes_per_elem = 6
         elif (etype == 'HEX'):
             nnodes_per_elem = 8
         elif (etype == 'QUAD'):
             nnodes_per_elem = 4
         elif (etype == 'TRIANGLE'):
             nnodes_per_elem = 3
+        elif (etype == 'POLYHEDRAL'):
+            return meshXYZPolyhedron(dat, key)
+        elif (etype == 'POLYGON'):
+            return meshXYZPolygon(dat, key)
 
         if len(elem_conn) % (nnodes_per_elem + 1) != 0:
             raise ValueError('This reader only processes single-element-type meshes.')
         n_elems = int(len(elem_conn) / (nnodes_per_elem+1))
         coords = dict(zip(mesh['NodeMap'][:,0], mesh['Nodes'][:]))
 
     conn = elem_conn.reshape((n_elems, nnodes_per_elem+1))
     if (np.any(conn[:,0] != elem_conn[0])):
         raise ValueError('This reader only processes single-element-type meshes.')
     return etype, coords, conn
 
 
+def meshXYZPolyhedron(dat, key):
+    """Reads polyhedral mesh and just returns coordinates and conn info.  Note
+    this is not enough to be useful for a real mesh but at least does something 
+    for polyhedral meshes."""
+    # read faces
+    mesh = dat[key]['Mesh']
+    elem_conn = mesh['MixedElements'][:,0]
+
+    coords = dict(zip(mesh['NodeMap'][:,0], mesh['Nodes'][:]))
+
+    conn = []
+    i = 0
+    while i < len(elem_conn):
+        nfaces = elem_conn[i]; i+=1
+        faces = []
+        for j in range(nfaces):
+            nnodes = elem_conn[i]; i+=1
+            fnodes = [elem_conn[k] for k in range(i, i+nnodes)]
+            i += nnodes
+            faces.append(fnodes)
+
+        conn.append(list(set(n for f in faces for n in f)))
+    return 'POLYHEDRAL', coords, conn
+
+
+def meshXYZPolygon(dat, key):
+    """Reads polygonal mesh and just returns coordinates and conn info."""
+    # read faces
+    mesh = dat[key]['Mesh']
+    elem_conn = mesh['MixedElements'][:,0]
+
+    coords = dict(zip(mesh['NodeMap'][:,0], mesh['Nodes'][:]))
+
+    conn = []
+    i = 0
+    while i < len(elem_conn):
+        etype = elem_type[elem_conn[i]]; i+=1
+        if (etype == 'QUAD'):
+            nnodes = 4
+        elif (etype == 'TRIANGLE'):
+            nnodes = 3
+        elif (etype == 'POLYGON'):
+            nnodes = elem_conn[i]; i+=1
+
+        fnodes = [elem_conn[k] for k in range(i, i+nnodes)]
+        i += nnodes
+        conn.append(fnodes)
+    return 'POLYGON', coords, conn
+
 def meshElemPolygons(etype, coords, conn):
     """Given mesh info that is a bunch of HEXes, make polygons for 2D plotting."""
     if etype != 'HEX':
         raise RuntimeError("Only works for Hexs")
 
     y_mean = np.array([c[1] for c in coords.values()]).mean()
```

### Comparing `modvis-0.0.6/modvis/colors.py` & `modvis-0.0.7/modvis/colors.py`

 * *Files identical despite different names*

### Comparing `modvis-0.0.6/modvis/general_plots.py` & `modvis-0.0.7/modvis/general_plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,17 @@
         rank_method, str
             Ranking method used by scipy.stats.rankdata. Options include: 'average', 'min','max',
             'dense','ordinal'
         var, str
             Column variable if provided
         ax, axis
             axis for plotting
+
+    Returns:
+        fig, ax if ax is None.
     """
     ndf = len(dfs)
 
     if linestyles is None:
         linestyles = ['-']*ndf
 
     if ax is None:
@@ -188,35 +191,51 @@
     # Draw the heatmap with the mask and correct aspect ratio
     sns.heatmap(corr, mask=mask, annot= True, 
                 square=True, linewidths=.5, 
                 cbar_kws={"shrink": 0.7}, **kwargs
                )    
     plt.title('Correlation Matrix', fontsize = 14)
 def varsComp_plot(dfs, variables, labels, colors, linestyles=None, axes=None, **kwargs):
-    """compare variables across different model runs"""
+    """compare variables across different model runs.
+    Parameters:
+    ---
+        dfs, list of dataframes
+        variables, list of variables
+        labels, list of labels for legend
+        colors, list of colors for line plot
+
+    Returns:
+    ---
+        None or (fig, axes)
+    
+    """
     nvar = len(variables)
     if axes is None:
         fig, axes = plt.subplots(nvar,1, figsize=(8,3*nvar), sharex = True)
         new_axes = True
     else:
         new_axes = False
     if linestyles is None:
         linestyles = ['-']*len(dfs)
 
     if nvar > 1:
         for ax, var in zip(axes, variables):
             for i in np.arange(len(dfs)):
+                idf = dfs[i][var]
+                assert idf.empty is False, f"{var} does not exist in {i+1}th df!"
                 ax.plot(var, linestyles[i], color = colors[i], data = dfs[i], label = labels[i], **kwargs)
                 ax.set_ylabel(var, fontsize = 12)
                 ax.set_xlabel('')
                 ax.legend(frameon = True, facecolor = 'w', edgecolor = 'w', framealpha = 0.7)
     else:
         ax = axes
         var = variables[0]
         for i in np.arange(len(dfs)):
+            idf = dfs[i][var]
+            assert idf.empty is False, f"{var} does not exist in {i+1}th df!"
             ax.plot(var, linestyles[i], color = colors[i], data = dfs[i], label = labels[i], **kwargs)
             ax.set_ylabel(var, fontsize = 12)
             ax.set_xlabel('')
             ax.legend(frameon = True, facecolor = 'w', edgecolor = 'w', framealpha = 0.7)
 
     if new_axes is True:
         return fig, axes
@@ -356,15 +375,15 @@
             color = line_color, **kwargs)
     ax.set_xlim([idx[0], idx[-1]])
     
     return ax, quantiles_df
 
 def one2one_plot(df_obs, df_simu, metrics=["R^2"], show_metrics=True,
                 ax=None, equal_aspect=True, show_density=False,
-                 decompose_KGE=False, start_date=None, end_date=None, **kwargs):
+                 decompose_KGE=False, start_date=None, end_date=None, dropzero=False, **kwargs):
     """One to One plot with a line.
     Parameters:
         df_obs, df_simu are Pandas series.
         metric, list or 'all'
             available metrics are: pearsonr, R2, RMSE, KGE,...
         show_metrics, bool
             Show metrics on the plot if True.
@@ -377,33 +396,35 @@
             data is overlapped.
         decompose_KGE, bool
             Decompose the KGE into three components (e.g., r, alpha and beta)
         start_date, str
             The start of the datetime index. e.g., "2016-10-01"
         end_date, str
             The end of the datetime index. e.g., "2020-10-01"
+        dropzero, bool
+            Drop zero values from the data before calculating metrics. This is useful when artifacts are present in the data.
     Returns:
         A one to one plot with metrics.
     """
     assert(isinstance(df_obs, pd.Series)) 
     assert(isinstance(df_simu, pd.Series)) 
     if not isinstance(df_obs.index, pd.DatetimeIndex) or not isinstance(df_simu.index, pd.DatetimeIndex):
         raise ValueError("Data Series must have datetime as index.")
     
     if start_date is not None or end_date is not None:
         df_obs = df_obs.loc[start_date:end_date]
         df_simu = df_simu.loc[start_date:end_date]
 
     metric_dict, df = utils.get_metrics(df_obs.index, df_obs.values, 
-                 df_simu.index, df_simu.values, metrics = metrics)
+                 df_simu.index, df_simu.values, metrics = metrics, dropzero=dropzero)
     if "mKGE" in metrics or 'KGE' in metrics: 
         if decompose_KGE is True:
             KGE_metric, _ = utils.get_metrics(df_obs.index, df_obs.values, 
-                 df_simu.index, df_simu.values, metrics = ['mKGE'], return_all
-                                         = True)
+                 df_simu.index, df_simu.values, metrics = ['mKGE'], 
+                 return_all= True, dropzero=dropzero)
             print(f"mKGE: {KGE_metric['mKGE'][0]}, cc:  {KGE_metric['mKGE'][1]}, alpha:  {KGE_metric['mKGE'][2]}, beta:  {KGE_metric['mKGE'][3]}")
     
     max_ = max(df['obs'].values.max(), df['simu'].values.max())
     min_ = min(df['obs'].values.min(), df['simu'].values.min())
 
     if ax is None:
         fig, ax = plt.subplots(1,1, figsize=(4,4))
```

### Comparing `modvis-0.0.6/modvis/objectivefunctions.py` & `modvis-0.0.7/modvis/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `modvis-0.0.6/modvis/plot_vis_file.py` & `modvis-0.0.7/modvis/plot_vis_file.py`

 * *Files identical despite different names*

### Comparing `modvis-0.0.6/modvis/transect_data.py` & `modvis-0.0.7/modvis/transect_data.py`

 * *Files identical despite different names*

### Comparing `modvis-0.0.6/modvis/utils.py` & `modvis-0.0.7/modvis/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 '''
 import os, re, scipy
 import numpy as np
 import pandas as pd
 import h5py
 from math import cos, sin, asin, sqrt, radians
 from sklearn.metrics import mean_squared_error
-from scipy.stats.stats import pearsonr
+from scipy.stats import pearsonr, mannwhitneyu
 import matplotlib.pyplot as plt
 from datetime import datetime, timedelta
 import time
 import matplotlib.lines as mlines
 import matplotlib.patches as mpatches
 # from calendar import isleap
 import logging
@@ -19,14 +19,78 @@
 import dataretrieval.nwis as nwis
 import sys
 # sys.path.append("..")
 
 # import objectivefunctions as ofs
 import modvis.objectivefunctions as ofs
 
+def insertNA(df, dt_col, freq=None):
+    '''
+    Automatically insert NAs for missing data.
+    Arguments:
+      - df. A dataframe contains the missing data.
+      - dt_col. Column name in the df which contains time series.
+    '''
+    df[dt_col] = pd.to_datetime(df[dt_col])
+    ## remove duplicates in the datetime index
+#     df = df[~df[dt_col].duplicated()]
+    df.drop_duplicates(subset=dt_col, inplace=True)
+    df.sort_values(by = dt_col, inplace = True)
+    # drop na
+    # df = df.loc[df.index.notnull()]
+    df.dropna(subset=[dt_col], inplace=True)
+    ## create a new index
+    start_time = df[dt_col].iloc[0]
+    end_time = df[dt_col].iloc[-1]
+    # ic(start_time)
+    # ic(end_time)
+    
+    # find frequency
+    if freq is None:
+        ## get the highest frequency in sec
+        freq_list = df[dt_col].diff().dt.seconds.value_counts()
+
+        # the first freq with the most samples on the list may not be the highest freq
+        if freq_list.index[0] == freq_list.index.min():
+            freq = freq_list.index[0]
+        else:
+            freq = freq_list.index.min()
+    logging.info(f'Found the highest frequency: {freq} sec')
+    new_index = pd.date_range(start_time, end_time, freq=pd.DateOffset(seconds = freq),
+                              name = dt_col)
+    ## reindex and reset index
+    df = df.set_index(dt_col).reindex(new_index).reset_index()
+
+    return df
+
+def days_between(d0,d1, noLeap=False):
+    """calculates days between two dates
+        Parameters:
+            d0, datetime.date()
+                starting date
+            d1, datetime.date() object
+                ending date
+            noLeap, bool
+                whether to consider leap years. 
+                If True, only 365 days are considered each year.
+                
+        Returns:
+            days in between dates.
+    """
+    delta = d1-d0
+    if noLeap:
+        # remove one day from leap year 
+        start_year = d0.year
+        end_year = d1.year
+        leap_years = list(range(start_year + (4 - start_year % 4), end_year + 1, 4))
+        
+        return delta.days - len(leap_years)
+    else:
+        return delta.days
+
 def load_nwis(service='dv', parameterCd='00060', SI_unit=True, insert_NA=True, rm_tz=True, **kwargs):
     """Load USGS streaflow from NWIS.
         Parameters:
             service, str
                 NWIS service including dv, iv...
             parameterCd, str
                 NWIS  parameter code including 00060, 00065, 00010 ...
@@ -65,35 +129,44 @@
         date_ind = pd.date_range(start = df.index[0], end = df.index[-1])
         new_df = pd.DataFrame(index = date_ind)
         df = df.join(new_df, how = 'outer')   
         
     return df
 
 
-def mark_start_end(df, label = None):
-    """Mark the start and end of the dateframe time series."""
-    ranges = []
-    # Start of good data block defined by a number preceeded by a NaN
-    start_mark = (df.notnull() & df.shift().isnull())
-    start = df[start_mark].index
-
-    # End of good data block defined by a number followed by a Nan
-    end_mark = (df.notnull() & df.shift(-1).isnull())
-    end = df[end_mark].index  
-    
-    for s, e in zip(start, end):
-        if label is None:
-            ranges.append((s, e))
-            # ranges = pd.DataFrame(ranges, columns=['start', 'end']) 
-        else:
-            ranges.append((label, s, e))
-            # ranges = pd.DataFrame(ranges, columns=['id', 'start', 'end']) 
-            # ranges.set_index('id', inplace = True)
-    
-    return ranges
+def mark_start_end(df, freq='1D'):
+    """Mark the start and end of the dateframe time series. This can be used in combination with
+    utils.gantt_plot().
+
+    Parameters:
+        df: pandas.DataFrame
+            dataframe with datetime index and at least one column of data
+        freq: str
+            frequency of the data. Defaults to '1D' (daily).
+
+    Returns:
+        start_dates: list of datetime
+        end_dates: list of datetime
+    """
+
+    # drop NaN data first
+    df.dropna(inplace=True)
+    # create a mask for missing data (assumes data is spaced evenly)
+    mask = df.index.to_series().diff() > pd.Timedelta(freq)    
+
+    # find the date before the mask (i.e. new starting date), will get new ending date
+    end_idx = list(np.where(mask.values)[0] - 1)
+
+    # find the start and end dates for each available time period
+    start_dates = [df.index[0]] + df.index[mask].to_list()
+    end_dates = df.index[end_idx].to_list() + [df.index[-1]]
+
+    assert len(start_dates) == len(end_dates)
+
+    return start_dates, end_dates
 
 def K_perm_conversion(K=None, k=None):
     """convert between hydraulic conductivity (K) and permeability (k)
     
     Parameters:
         K: float
             hydraulic conductivity in m/d
@@ -296,32 +369,38 @@
 #     h5_file.close()
 
 def print_xml(file):
     """Print xml file in a clean way."""
     print(''.join(file))
 
 def get_metrics(obs_t, obs, simu_t, simu, metrics = 'all', start_date = None,
-                end_date = None, epsilon=0, **kwargs):
-    """compute R2 and RMSE between simulated and observed
+                end_date = None, epsilon=0, dropzero=False, **kwargs):
+    """
+    Calculate metrics between simulated and observed data.
     Parameters:
         obs_t: list or array
             observed datetime series
         obs: list or array
             observed numeric series
         simu_t: list or array
             simulated datetime series
         simu: list or array
             simulated numeric sereis
         start_date: datetime object
-            starting date for RMSE and R^2 calculation
+            starting date for metric calculation
         end_date: datetime object
-            ending date for RMSE and R^2 calculation
+            ending date for metric calculation
         epsilon: float
-            small number added to the data to avoid zero issue when using log transformation (e.g., logNSE). Recommended value is 1/100 of the mean observed flow (see Santos et al., 2018 HESS for discussion).
-
+            small number added to the data to avoid zero issue when using log transformation (e.g., logNSE). 
+            Recommended value is 1/100 of the mean observed flow (see Santos et al., 2018 HESS for discussion).
+        dropzero: bool
+            if True, drop zero values in observed data. This is useful for dataframe with artifacts of zero values 
+            (e.g., when using the restarted output from ATS).
+        **kwargs: keyword arguments
+            keyword arguments {return_all = True} for KGE components calculation
     Returns:
         dict of metrics and dataframe used.
     
     """
     VALID_METRICS = ['pearsonr', 'R^2', 'RMSE', 'rRMSE', 'NSE', 'logNSE',
                      'bias', 'pbias', 'KGE','npKGE', 'mKGE']
     
@@ -334,14 +413,18 @@
     df2 = pd.DataFrame((np.array(simu_t), simu))
     #, columns=['datetime', 'q_obs']
     df2 = df2.T
     df2.columns = ['datetime', 'simu']
     df2.dropna(inplace = True)
     
     df = df1.merge(df2, how='inner', on = 'datetime')
+
+    if dropzero:
+        # drop rows with any zero values
+        df = df[(df != 0).all(1)]
     
     if start_date != None or end_date != None:
         df = df[df.datetime < end_date].copy()
         df = df[df.datetime > start_date]
         
     assert(df.shape[0] > 2)
 
@@ -360,14 +443,15 @@
         elif i == 'RMSE':
             val = sqrt(mean_squared_error(df['obs'].values, df['simu'].values))
         elif i == 'rRMSE':
             val = ofs.rrmse(df['obs'].values, df['simu'].values)
         elif i == 'NSE':
             val = ofs.nashsutcliffe(df['obs'].values, df['simu'].values)
         elif i == 'logNSE':
+            # default epsilon is 1/100 of the mean observed flow
             if epsilon == 0:
                 epsilon = df['obs'].mean() / 100
             val = ofs.lognashsutcliffe(df['obs'].values, df['simu'].values, epsilon=epsilon)
         elif i == 'bias':
             val = ofs.bias(df['obs'].values, df['simu'].values)
         elif i == 'pbias':
             val = ofs.pbias(df['obs'].values, df['simu'].values)
@@ -497,7 +581,27 @@
         TheFile.write("\n")#write new line
 
     TheFile.close()
     
     print('Exported ASCII file is in {}'.format(file_asc))
     
     return None
+
+def mann_whitney_test(data1, data2, alpha=0.05):
+    """
+    perform a Mann-Whitney test, and return statistics and p-value
+    Parameters:
+        x: data1, dataframe timeseries
+        y: data2, dataframe timeseries
+        alpha: significance factor, default 0.05
+    Returns:
+        stat, p
+    """
+    stat, p = mannwhitneyu(data1, data2)
+    print('Statistics=%.3f, p=%.3f' % (stat, p))
+    if p > alpha:
+        print('Same distributions (fail to reject H0)')
+    else:
+        print('Different distributions (reject H0)')
+    return stat, p
+        
+    return stat, p
```

### Comparing `modvis-0.0.6/setup.py` & `modvis-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
 
 setup(
     author="Pin Shuai",
-    author_email='pinshuai.phd@gmail.com',
+    author_email='pin.shuai@usu.edu',
     python_requires='>=3.7',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
@@ -48,10 +48,10 @@
     keywords='modvis',
     name='modvis',
     packages=find_packages(include=['modvis', 'modvis.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/pinshuai/modvis',
-    version='0.0.6',
+    version='0.0.7',
     zip_safe=False,
 )
```

