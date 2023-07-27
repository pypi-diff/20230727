# Comparing `tmp/magnetocaloric-1.1.9.tar.gz` & `tmp/magnetocaloric-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnetocaloric-1.1.9.tar", last modified: Thu Jun  2 12:02:04 2022, max compression
+gzip compressed data, was "magnetocaloric-1.2.0.tar", last modified: Thu Jul 27 08:36:41 2023, max compression
```

## Comparing `magnetocaloric-1.1.9.tar` & `magnetocaloric-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-06-02 12:02:04.678295 magnetocaloric-1.1.9/
--rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.1.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2022-04-10 10:58:56.000000 magnetocaloric-1.1.9/Licence.txt
--rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3777 2022-06-02 12:02:04.678295 magnetocaloric-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2668 2022-06-02 12:01:18.000000 magnetocaloric-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2022-06-02 12:02:04.647035 magnetocaloric-1.1.9/magnetocaloric/
--rw-rw-rw-   0        0        0    14691 2022-06-02 11:59:56.000000 magnetocaloric-1.1.9/magnetocaloric/__init__.py
--rw-rw-rw-   0        0        0    14691 2022-06-02 11:57:28.000000 magnetocaloric-1.1.9/magnetocaloric/mcepy.py
-drwxrwxrwx   0        0        0        0 2022-06-02 12:02:04.678295 magnetocaloric-1.1.9/magnetocaloric.egg-info/
--rw-rw-rw-   0        0        0     3777 2022-06-02 12:02:01.000000 magnetocaloric-1.1.9/magnetocaloric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2022-06-02 12:02:02.000000 magnetocaloric-1.1.9/magnetocaloric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-02 12:02:01.000000 magnetocaloric-1.1.9/magnetocaloric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2022-06-02 12:02:01.000000 magnetocaloric-1.1.9/magnetocaloric.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-06-02 12:02:01.000000 magnetocaloric-1.1.9/magnetocaloric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-02 12:02:04.678295 magnetocaloric-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1141 2022-06-02 12:01:15.000000 magnetocaloric-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:36:41.118427 magnetocaloric-1.2.0/
+-rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.2.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.2.0/Licence.txt
+-rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4467 2023-07-27 08:36:41.118427 magnetocaloric-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3720 2023-07-27 08:22:32.000000 magnetocaloric-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 08:36:41.102798 magnetocaloric-1.2.0/magnetocaloric/
+-rw-rw-rw-   0        0        0    15967 2023-07-27 07:04:32.000000 magnetocaloric-1.2.0/magnetocaloric/__init__.py
+-rw-rw-rw-   0        0        0    15967 2023-07-27 07:02:01.000000 magnetocaloric-1.2.0/magnetocaloric/mcepy.py
+drwxrwxrwx   0        0        0        0 2023-07-27 08:36:41.118427 magnetocaloric-1.2.0/magnetocaloric.egg-info/
+-rw-rw-rw-   0        0        0     4467 2023-07-27 08:36:40.000000 magnetocaloric-1.2.0/magnetocaloric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-27 08:36:40.000000 magnetocaloric-1.2.0/magnetocaloric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 08:36:40.000000 magnetocaloric-1.2.0/magnetocaloric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-27 08:36:40.000000 magnetocaloric-1.2.0/magnetocaloric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-27 08:36:40.000000 magnetocaloric-1.2.0/magnetocaloric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 08:36:41.118427 magnetocaloric-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2023-07-27 08:23:40.000000 magnetocaloric-1.2.0/setup.py
```

### Comparing `magnetocaloric-1.1.9/Licence.txt` & `magnetocaloric-1.2.0/Licence.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 Supratim Das
+Copyright 2023 Supratim Das
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `magnetocaloric-1.1.9/PKG-INFO` & `magnetocaloric-1.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,63 @@
-Metadata-Version: 2.1
-Name: magnetocaloric
-Version: 1.1.9
-Summary: Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python
-Home-page: https://github.com/supratimdasinfo/Magnetocaloric-Effect
-Author: Supratim Das
-Author-email: supratim0707@gmail.com
-License: MIT
-Description: # magnetocaloric 1.1.9
-        #### Developed by Supratim Das
-        ![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)
-        
-        Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
-        
-        ## What's New
-        - Relative cooling power (RCP) can be calculated.
-        - A method to visualize 'Full Width Of Half Maxima' has been employed.
-        - Another methods to illustrate Tricritical mean field model, 3D Heisenberg model and 3D Ising model have also been employed.
-        
-        
-        ## Examples of How To Use
-        
-        ### 1. Installation 
-        
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
-        
-        ```bash
-        
-         pip install magnetocaloric==1.1.9
-        
-        ```
-        ### 2. Manage Excel Spreadsheet
-        -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
-        
-        ![](https://github.com/supratimdasinfo/Magnetocaloric-Effect/blob/main/Screenshot%20(229).png?raw=True)
-        
-        -  And add one extra magnetic field (Hmax + del_H) with null magnetic moment values. This is nothing else than to bring magnetic moment values of the last row under calculation.
-        
-        ![](https://github.com/supratimdasinfo/Magnetocaloric-Effect/blob/main/Screenshot%20(232).png?raw=True)
-        
-        - Create two new files (file extension xlsx) to hold the results obtained after the calculation and definitely make them closed, other wise XlsxWriter will not get access.
-        
-        ###  3. Execution
-        Run the code at any python based environment ( IDLE, PyCharm, Spyder etc.). But I recommend you simply execute this code using command prompt or IDLE. 
-        
-        ```python
-        
-        import magnetocaloric.mcepy as mc
-        
-        print(mc.mce(a, b))
-        
-        ```
-        Here, 'a' is the total number of temperature and 'b' is the total number of applied magnetic field.
-        
-        ## Caution
-        
-        - Before adding the Hmax + del_H value into the M(H) spreadsheet, The maximum value of applied magnetic field (Hmax) must be the multiple of (10xdel_H). As an example, if del_H = 500 Oe / 0.05 T, Hmax must be like 5000 Oe/0.5 T, 10000 Oe / 1 T, 15000 Oe / 1.5 T,........ or any other multiple of (10x500 Oe) whether the value of the magnetic field is Tesla or Oersted. For another example, if del_H = 700 Oe / 0.07 T, Hmax must be like 7000 Oe/0.7 T, 14000 Oe / 1.4 T, 21000 Oe / 2.1 T,........ or any other multiple of (10x700 Oe). Otherwise Hmax for not being a proper numbered figure, an error may occur. This caution is also applicable to the previous versions of the package as well.
-Keywords: magnetocaloric,mcepy,magnetic,programming,code,python,supratim
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
+
+# magnetocaloric 1.2.0
+#### Developed by Supratim Das
+
+![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
+
+Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
+
+## What's New
+- Relative cooling power (RCP) can be calculated.
+- A method to visualize 'Full Width Of Half Maxima' has been employed.
+- Another methods to illustrate Tricritical mean field model, 3D Heisenberg model and 3D Ising model have also been employed.
+- Intuitive Graphical User Interface: Simplifying Program Interaction. Experience seamless interaction with our TKinter-powered UI. Standalone Python executable created using PyInstaller - no additional dependencies required. 
+
+![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/GUI.png?raw=True)
+
+For the Python programming approach, follow the steps in the README.
+
+
+## Examples of How To Use
+
+### 1. Installation 
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
+
+```bash
+
+ pip install magnetocaloric==1.2.0
+
+```
+### 2. Manage Excel Spreadsheet
+-  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
+
+![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
+
+-  And add one extra magnetic field (Hmax + del_H) with null magnetic moment values. This is nothing else than to bring magnetic moment values of the last row under calculation.
+
+![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(232).png?raw=True)
+
+- Create two new files (file extension xlsx) to hold the results obtained after the calculation and definitely make them closed, other wise XlsxWriter will not get access.
+
+###  3. Execution
+Run the code at any python based environment ( IDLE, PyCharm, Spyder etc.). But I recommend you simply execute this code using command prompt or IDLE. 
+
+```python
+
+import magnetocaloric.mcepy as mc
+mc.mce(a, b)
+
+```
+Here, 'a' is the total number of temperature and 'b' is the total number of applied magnetic field.
+
+## Contributing
+### We Welcome Your Contributions!
+
+If you're interested in contributing to the development of this project, your contributions are highly appreciated. Whether you find a bug, have an idea for a new feature, or want to improve the code, you can do so by raising an issue or pull request on our GitHub repository. Your input helps make this project better for everyone.
+
+Feel free to explore the code, try out the application, and share your thoughts with us. We value the contributions of our community members and look forward to collaborating with you. Let's make this project even more amazing together!
+
+
+## Caution
+
+- Before adding the Hmax + del_H value into the M(H) spreadsheet, The maximum value of applied magnetic field (Hmax) must be the multiple of (10xdel_H). As an example, if del_H = 500 Oe / 0.05 T, Hmax must be like 5000 Oe/0.5 T, 10000 Oe / 1 T, 15000 Oe / 1.5 T,........ or any other multiple of (10x500 Oe) whether the value of the magnetic field is Tesla or Oersted. For another example, if del_H = 700 Oe / 0.07 T, Hmax must be like 7000 Oe/0.7 T, 14000 Oe / 1.4 T, 21000 Oe / 2.1 T,........ or any other multiple of (10x700 Oe). Otherwise Hmax for not being a proper numbered figure, an error may occur. This caution is also applicable to the previous versions of the package as well.
```

### Comparing `magnetocaloric-1.1.9/magnetocaloric/__init__.py` & `magnetocaloric-1.2.0/magnetocaloric/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     for b in range(0, (n)):
          Temperature_val = input("    enter the temperature value : ")
          T.append(Temperature_val)
     plot_legend = input("\n\n    do you want to plot the figures with legend (YES/NO)?  ")     
     book = xlrd.open_workbook(Path_one)
     sheet = book.sheet_by_name('Sheet1')
     data = [[sheet.cell_value(r, c) for c in range(n+1)] for r in range(sheet.nrows)]
-
     for a in range(1, one_n+1, 1):          
          H.append((data[a])[0])
          for b in range(0, n):
               T.append(T[b])               
          for b in range(1, n+1):
               M.append((data[a])[b])
 
@@ -300,24 +299,27 @@
     row = 0
     for col, data in enumerate(M_sqr_vs_H_by_M):
          worksheet.write_column(row, col, data)
     workbook.close()
 
     T_FWHM_con = []
     RCP_con = []
+    RCP_error = []
+    RCP_final = []
+    H_for_RCP = []
     for j in range(1, (len(Label_one) + 1), 1):
         del_S_peak = np.max(six_entropy_change_con[j])
         for k in range(0, n-1, 1):
             if (six_entropy_change_con[j][k] == del_S_peak):
                 kth_index = k
                 max_entropy_at_T = six_entropy_change_con[0][kth_index]
             
         half_max = float(del_S_peak/2)
         half_max_entropy_at_T_con = []
-        half_max_entropy_at_T_con.append(float(0.0))
+        half_max_entropy_at_T_con.append(float(six_entropy_change_con[0][0]))
         for i in range(0, n-2, 1):
             i_th = six_entropy_change_con[j][i]
             i_th_plus_one = six_entropy_change_con[j][i+1]
             if ((i_th_plus_one >= half_max >= i_th) or (i_th_plus_one <= half_max <= i_th)):
                 T_i_th = six_entropy_change_con[0][i]
                 T_i_th_plus_one = six_entropy_change_con[0][i+1]
                 del_S_dif = abs(float(i_th_plus_one - i_th))
@@ -333,29 +335,52 @@
                 T_left = l_th
                 T_right = l_th_plus_one
             
         T_FWHM = T_right - T_left
         RCP = T_FWHM * del_S_peak
         T_FWHM_con.append(float(round(T_FWHM,4)))
         RCP_con.append(float(round(RCP,4)))
+        if ((T_left == float(six_entropy_change_con[0][0]) != 0.0) or (T_right == float(six_entropy_change_con[0][n-2]))):
+                                                
+            RCP_error.append(Label_one[j-1])
+        else:
+            RCP_final.append(float(round(RCP,4)))
+            H_for_RCP.append(Label_one[j-1])
+    lst_RCP_error = (len(RCP_error) - 1)
+
+    if (len(RCP_error) == 1):
+        print ("\n    insufficient data! error have been detected while calculating RCP at H : {} T".format(RCP_error[0]))
+    elif (len(RCP_error) >= 1):
+        print ("\n    insufficient data! error have been detected while calculating RCP from H : {} T to H : {} T".format(RCP_error[0], RCP_error[lst_RCP_error]))
+    else:
+        print ('\n    RCP have been successfully calculated')
 
     samp_name_plus_RCP = "RCP (" + samp_name + ") :: max val : " + str(np.max(RCP_con))
     samp_name_plus_T_FWHM = "T_FWHM (" + samp_name + ") :: max width : " + str(np.max(T_FWHM_con))
 
     fig,ax1 = plt.subplots()
     ax1.set_xlabel("Magnetic Field(H)", fontname = "Georgia")
     ax1.set_ylabel("RCP", fontname = "Georgia")
     ax1.plot(Label_one, RCP_con, linestyle='solid', marker = 'h', label = samp_name_plus_RCP, color = 'b', markersize =6, linewidth=2)
     ax1.legend(loc='upper left',frameon = False, ncol= 2)
     ax1.tick_params(axis='y')
 
     ax2 = ax1.twinx()
     ax2.set_ylabel("T_FWHM", fontname = "Georgia")
-    ax2.plot(Label_one, T_FWHM_con, linestyle='solid', marker = 'H', label = samp_name_plus_T_FWHM, color = 'r', markersize =6, linewidth=2)
+    ax2.plot(Label_one, T_FWHM_con, linestyle='none', marker = 'H', label = samp_name_plus_T_FWHM, color = 'c', markersize =2, linewidth=0.5)
     ax2.legend(loc='lower right',frameon = False, ncol= 2)
     ax2.tick_params(axis='y')
 
     plt.title("RCP/T_FWHM vs H", fontname = "Georgia") 
     
     plt.show()
+    if ((len(RCP_final))>= 2):
+                                        
+        plt.xlabel("Magnetic Field(H)", fontname = "Georgia")
+        plt.ylabel("RCP", fontname = "Georgia")
+        plt.title("Magnetic Field vs RCP", fontname = "Georgia")
+        plt.plot(H_for_RCP, RCP_final, linestyle='solid', color = 'b', marker = 'h', markersize =6, linewidth=2)
+        plt.show()
+
     return ("\n    check the excel spreadsheets, data has been successfully saved.")
 
+
```

### Comparing `magnetocaloric-1.1.9/magnetocaloric/mcepy.py` & `magnetocaloric-1.2.0/magnetocaloric/mcepy.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     for b in range(0, (n)):
          Temperature_val = input("    enter the temperature value : ")
          T.append(Temperature_val)
     plot_legend = input("\n\n    do you want to plot the figures with legend (YES/NO)?  ")     
     book = xlrd.open_workbook(Path_one)
     sheet = book.sheet_by_name('Sheet1')
     data = [[sheet.cell_value(r, c) for c in range(n+1)] for r in range(sheet.nrows)]
-
     for a in range(1, one_n+1, 1):          
          H.append((data[a])[0])
          for b in range(0, n):
               T.append(T[b])               
          for b in range(1, n+1):
               M.append((data[a])[b])
 
@@ -300,24 +299,27 @@
     row = 0
     for col, data in enumerate(M_sqr_vs_H_by_M):
          worksheet.write_column(row, col, data)
     workbook.close()
 
     T_FWHM_con = []
     RCP_con = []
+    RCP_error = []
+    RCP_final = []
+    H_for_RCP = []
     for j in range(1, (len(Label_one) + 1), 1):
         del_S_peak = np.max(six_entropy_change_con[j])
         for k in range(0, n-1, 1):
             if (six_entropy_change_con[j][k] == del_S_peak):
                 kth_index = k
                 max_entropy_at_T = six_entropy_change_con[0][kth_index]
             
         half_max = float(del_S_peak/2)
         half_max_entropy_at_T_con = []
-        half_max_entropy_at_T_con.append(float(0.0))
+        half_max_entropy_at_T_con.append(float(six_entropy_change_con[0][0]))
         for i in range(0, n-2, 1):
             i_th = six_entropy_change_con[j][i]
             i_th_plus_one = six_entropy_change_con[j][i+1]
             if ((i_th_plus_one >= half_max >= i_th) or (i_th_plus_one <= half_max <= i_th)):
                 T_i_th = six_entropy_change_con[0][i]
                 T_i_th_plus_one = six_entropy_change_con[0][i+1]
                 del_S_dif = abs(float(i_th_plus_one - i_th))
@@ -333,29 +335,52 @@
                 T_left = l_th
                 T_right = l_th_plus_one
             
         T_FWHM = T_right - T_left
         RCP = T_FWHM * del_S_peak
         T_FWHM_con.append(float(round(T_FWHM,4)))
         RCP_con.append(float(round(RCP,4)))
+        if ((T_left == float(six_entropy_change_con[0][0]) != 0.0) or (T_right == float(six_entropy_change_con[0][n-2]))):
+                                                
+            RCP_error.append(Label_one[j-1])
+        else:
+            RCP_final.append(float(round(RCP,4)))
+            H_for_RCP.append(Label_one[j-1])
+    lst_RCP_error = (len(RCP_error) - 1)
+
+    if (len(RCP_error) == 1):
+        print ("\n    insufficient data! error have been detected while calculating RCP at H : {} T".format(RCP_error[0]))
+    elif (len(RCP_error) >= 1):
+        print ("\n    insufficient data! error have been detected while calculating RCP from H : {} T to H : {} T".format(RCP_error[0], RCP_error[lst_RCP_error]))
+    else:
+        print ('\n    RCP have been successfully calculated')
 
     samp_name_plus_RCP = "RCP (" + samp_name + ") :: max val : " + str(np.max(RCP_con))
     samp_name_plus_T_FWHM = "T_FWHM (" + samp_name + ") :: max width : " + str(np.max(T_FWHM_con))
 
     fig,ax1 = plt.subplots()
     ax1.set_xlabel("Magnetic Field(H)", fontname = "Georgia")
     ax1.set_ylabel("RCP", fontname = "Georgia")
     ax1.plot(Label_one, RCP_con, linestyle='solid', marker = 'h', label = samp_name_plus_RCP, color = 'b', markersize =6, linewidth=2)
     ax1.legend(loc='upper left',frameon = False, ncol= 2)
     ax1.tick_params(axis='y')
 
     ax2 = ax1.twinx()
     ax2.set_ylabel("T_FWHM", fontname = "Georgia")
-    ax2.plot(Label_one, T_FWHM_con, linestyle='solid', marker = 'H', label = samp_name_plus_T_FWHM, color = 'r', markersize =6, linewidth=2)
+    ax2.plot(Label_one, T_FWHM_con, linestyle='none', marker = 'H', label = samp_name_plus_T_FWHM, color = 'c', markersize =2, linewidth=0.5)
     ax2.legend(loc='lower right',frameon = False, ncol= 2)
     ax2.tick_params(axis='y')
 
     plt.title("RCP/T_FWHM vs H", fontname = "Georgia") 
     
     plt.show()
+    if ((len(RCP_final))>= 2):
+                                        
+        plt.xlabel("Magnetic Field(H)", fontname = "Georgia")
+        plt.ylabel("RCP", fontname = "Georgia")
+        plt.title("Magnetic Field vs RCP", fontname = "Georgia")
+        plt.plot(H_for_RCP, RCP_final, linestyle='solid', color = 'b', marker = 'h', markersize =6, linewidth=2)
+        plt.show()
+
     return ("\n    check the excel spreadsheets, data has been successfully saved.")
 
+
```

### Comparing `magnetocaloric-1.1.9/setup.py` & `magnetocaloric-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,21 +10,21 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='magnetocaloric',
-  version='1.1.9',
+  version='1.2.0',
   description='Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/supratimdasinfo/Magnetocaloric-Effect',  
   author='Supratim Das',
   author_email='supratim0707@gmail.com',
   license='MIT', 
   classifiers=classifiers,
-  keywords=['magnetocaloric', 'mcepy', 'magnetic', 'programming', 'code', 'python','supratim'],
+  keywords=['magnetocaloric', 'mcepy', 'magnetic', 'programming', 'code', 'python','supratim', 'das', 'bhaskar', 'biswas', 'physics'],
   include_package_data=True, 
   packages=['magnetocaloric'],
   install_requires=['num2words', 'matplotlib','xlrd==1.2.0','openpyxl','tableprint','XlsxWriter','numpy'] 
 )
```

