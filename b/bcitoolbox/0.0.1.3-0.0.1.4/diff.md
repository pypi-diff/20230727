# Comparing `tmp/bcitoolbox-0.0.1.3.tar.gz` & `tmp/bcitoolbox-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcitoolbox-0.0.1.3.tar", last modified: Fri Jul 21 01:26:38 2023, max compression
+gzip compressed data, was "bcitoolbox-0.0.1.4.tar", last modified: Thu Jul 27 06:35:54 2023, max compression
```

## Comparing `bcitoolbox-0.0.1.3.tar` & `bcitoolbox-0.0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-21 01:26:38.773249 bcitoolbox-0.0.1.3/
--rw-r--r--   0 evans      (501) staff       (20)      534 2023-07-21 01:26:38.772792 bcitoolbox-0.0.1.3/PKG-INFO
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-21 01:26:38.766495 bcitoolbox-0.0.1.3/bcitoolbox/
--rw-r--r--   0 evans      (501) staff       (20)    13082 2023-07-20 05:31:26.000000 bcitoolbox-0.0.1.3/bcitoolbox/BCIbox.py
--rw-r--r--   0 evans      (501) staff       (20)      137 2023-07-20 05:29:09.000000 bcitoolbox-0.0.1.3/bcitoolbox/__init__.py
--rw-r--r--   0 evans      (501) staff       (20)    38267 2023-07-21 01:24:31.000000 bcitoolbox-0.0.1.3/bcitoolbox/guifunc.py
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-21 01:26:38.772244 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/
--rw-r--r--   0 evans      (501) staff       (20)      534 2023-07-21 01:26:38.000000 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/PKG-INFO
--rw-r--r--   0 evans      (501) staff       (20)      243 2023-07-21 01:26:38.000000 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-21 01:26:38.000000 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 evans      (501) staff       (20)       23 2023-07-21 01:26:38.000000 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/requires.txt
--rw-r--r--   0 evans      (501) staff       (20)       11 2023-07-21 01:26:38.000000 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/top_level.txt
--rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-21 01:26:38.773383 bcitoolbox-0.0.1.3/setup.cfg
--rw-r--r--   0 evans      (501) staff       (20)      880 2023-07-21 01:25:03.000000 bcitoolbox-0.0.1.3/setup.py
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-27 06:35:54.614327 bcitoolbox-0.0.1.4/
+-rw-r--r--   0 evans      (501) staff       (20)     1142 2023-07-27 06:35:54.614000 bcitoolbox-0.0.1.4/PKG-INFO
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-27 06:35:54.610432 bcitoolbox-0.0.1.4/bcitoolbox/
+-rw-r--r--   0 evans      (501) staff       (20)    14743 2023-07-27 06:29:09.000000 bcitoolbox-0.0.1.4/bcitoolbox/BCIbox.py
+-rw-r--r--   0 evans      (501) staff       (20)      161 2023-07-27 06:29:27.000000 bcitoolbox-0.0.1.4/bcitoolbox/__init__.py
+-rw-r--r--   0 evans      (501) staff       (20)    40805 2023-07-27 06:27:21.000000 bcitoolbox-0.0.1.4/bcitoolbox/guifunc.py
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-27 06:35:54.613584 bcitoolbox-0.0.1.4/bcitoolbox.egg-info/
+-rw-r--r--   0 evans      (501) staff       (20)     1142 2023-07-27 06:35:54.000000 bcitoolbox-0.0.1.4/bcitoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 evans      (501) staff       (20)      243 2023-07-27 06:35:54.000000 bcitoolbox-0.0.1.4/bcitoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-27 06:35:54.000000 bcitoolbox-0.0.1.4/bcitoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 evans      (501) staff       (20)       23 2023-07-27 06:35:54.000000 bcitoolbox-0.0.1.4/bcitoolbox.egg-info/requires.txt
+-rw-r--r--   0 evans      (501) staff       (20)       11 2023-07-27 06:35:54.000000 bcitoolbox-0.0.1.4/bcitoolbox.egg-info/top_level.txt
+-rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-27 06:35:54.614421 bcitoolbox-0.0.1.4/setup.cfg
+-rw-r--r--   0 evans      (501) staff       (20)     1358 2023-07-27 06:35:44.000000 bcitoolbox-0.0.1.4/setup.py
```

### Comparing `bcitoolbox-0.0.1.3/bcitoolbox/BCIbox.py` & `bcitoolbox-0.0.1.4/bcitoolbox/BCIbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 
 import numpy as np
 import matplotlib.pyplot as plt
 import csv
 import time
 import random
+import os 
+from scipy.optimize import minimize
 from scipy.fftpack import dct
 from matplotlib.colors import ListedColormap
 from matplotlib.colors import LinearSegmentedColormap
 
 
 def prod_gaus(mu1, mu2, sigma1, sigma2):
     mu1 = np.array(mu1)
@@ -393,8 +395,37 @@
             plt.plot(model[1, i, :], 'r-.')
             plt.axis([0, a[2]-1, 0, 1])
     
     if save_path is not None:
         plt.savefig(save_path, dpi=300, bbox_inches="tight")
     
     plt.show()
+
+def fit(n_parameters, n_Simulation, Behavior_Data, n_seeds = 1, bounds = [(0, 1),(0.1, 3),(0.1, 3),(0.1,3),(0, 3.5)], biOnly = 1, Strategies = ['ave'], FitType = 'mll'):
+    result_M = None
+    start_time = time.time()
+    [13, 1089, 681, 304, 118, 817, 82, 736, 295, 424, 247, 732, 243, 366, 483, 415, 747, 926, 335, 394, 653, 968, 746, 944, 197, 871, 694, 466, 958, 42, 276, 45, 419, 43, 985, 190, 405, 35, 388, 523, 796, 239, 124, 291, 924, 491, 417, 482, 57, 861, 405, 226, 292, 501, 904, 920, 199, 287, 433, 531, 797, 686, 459, 812, 152, 243, 330, 306, 583, 397, 660, 729, 480, 925, 437, 831, 452, 506, 388, 988, 160, 169, 854, 353, 93, 872, 195, 556, 266, 752, 104, 64, 902, 103, 185, 216, 527, 802, 221, 778]
+    data = Behavior_Data
+    best_error = float('inf')
+    best_result = None
+    best_strategy = None
+    
+    for strategy in Strategies:
+        for seed in range(n_seeds):
+            np.random.seed(random_seeds[seed])
+            x0 = np.random.rand(n_parameters)
+     
+            result = minimize(lambda paras: simulateVV(paras, n_Simulation, data, biOnly, strategy = strategy, fitType=FitType)[0], x0, method='Powell', bounds=bounds)
+            if result.success and result.fun < best_error:
+                best_error = result.fun
+                best_result = result
+                best_strategy = strategy
+        
+    estimated_parameters = best_result.x
+    error = best_error
+    strategy = best_strategy
+    end_time = time.time()     
+    execution_time = end_time - start_time  
+    print("Running time:", execution_time, "s")
+
+    return estimated_parameters, error, strategy
```

### Comparing `bcitoolbox-0.0.1.3/bcitoolbox/guifunc.py` & `bcitoolbox-0.0.1.4/bcitoolbox/guifunc.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,49 @@
             data_matrices.append(df)
     
 def open_document():
     file_path = filedialog.askopenfilename()
     if file_path:  
         print(file_path)
 
+def about_bci():
+
+    about_window = tk.Toplevel(welcome_frame)
+    about_window.title("About BCI Toolbox")
+    
+    g_font = ("Georgia", 18, "bold")
+    title_font = ("Georgia", 17, "bold")
+    name_font = ("Georgia", 15, "bold")
+    info_font = ("Script MT Bold", 13)
+
+    title_label = tk.Label(about_window, text="About BCI Toolbox", font=g_font)
+    title_label.pack(pady=10)
+    names_text = tk.Text(about_window, wrap=tk.WORD, font=name_font, padx=10, pady=10)
+    names_text.pack()
+    names_info_c = [
+        ("Dr. Ladan Shams", "University of California, Los Angeles", "ladan@psych.ucla.edu"),
+        ("Dr. Ulrik R. Beierholm", "Durham University", "beierh@gmail.com")   
+    ]
+    names_info_i = [
+        ("Haocheng (Evans) Zhu", "Soochow University", "evanszhu2001@gmail.com"),   
+    ]
+    names_text.insert(tk.END, "Conceptualization\n\n", "title")
+    for name, univ, emailA in names_info_c:
+        names_text.insert(tk.END, f"{name}\n", "name")
+        names_text.insert(tk.END, f"{univ}\n{emailA}\n\n", "info")
+
+    names_text.insert(tk.END, "\nImplementation\n\n", "title")
+    for name, univ, emailA in names_info_i:
+        names_text.insert(tk.END, f"{name}\n", "name")
+        names_text.insert(tk.END, f"{univ}\n{emailA}\n\n", "info") 
+
+    names_text.tag_configure("title", font=title_font, justify=tk.CENTER)
+    names_text.tag_configure("name", font=name_font, justify=tk.CENTER)
+    names_text.tag_configure("info", font=info_font, justify=tk.CENTER)
+
 def done_setting():
     global count
     global bounds
     checkbox_vars = [var1, var2, var3, var4, var5, var6, var7]
     count = sum(var.get() for var in checkbox_vars)
     print("Number of free parameters:", count)
     bounds = [
@@ -339,19 +374,16 @@
                 file_name = os.path.splitext(file_name)[0]
                 figure_name = file_name + f"_{strategy_list[ndata]}"+ ".png"
                 figure_path = os.path.join(target_folder, figure_name)
                 plt.savefig(figure_path)
 
                 
 
-            
-
-
     
-def plot_Simu():
+def plot_Simu(ifdata):
     plt.clf()
     # Default Parameters
     sti1 = variable_sti1.get()
     sti2 = variable_sti2.get()
     pcommon = variable_pcommon.get()
     sigmaU = variable_sigmaU.get()
     sigmaD = variable_sigmaD.get()
@@ -441,14 +473,23 @@
     
     else:
         # Matching
         p_cutoff = np.random.rand(Sc.shape[0])
         responsesSim[:, 0] = np.where(PCDU > p_cutoff, Sc, Snc1)
         responsesSim[:, 1] = np.where(PCDU > p_cutoff, Sc, Snc2)
 
+    if ifdata == 2:
+        file_path_simudata = filedialog.asksaveasfilename(defaultextension=".csv", filetypes=[("CSV Files", "*.csv")])
+        if file_path_simudata:
+            with open(file_path_simudata, 'w') as file:
+                for row in responsesSim:
+                    line = ','.join(str(item) for item in row) + '\n'
+                    file.write(line)
+        return file_path_simudata
+        
     if var_respD.get():  
         D1 = responsesSim[:, 0]
         D2 = responsesSim[:, 1]
         # kernel density estimation
         kde1 = gaussian_kde(D1)
         kde2 = gaussian_kde(D2)
 
@@ -531,28 +572,29 @@
 def generate_combinations(n):
     combinations = [[i, j] for i in range(n) for j in range(n)]
     combinations = np.array(combinations[1:], dtype=float)
     return combinations
 
 def save_p():
     file_list = []
+    header_list = ['pcommon', 'sigmaU', 'sigmaD', 'sigmap', 'mup', 'sU', 'sD']
     for file_path in file_paths:
         file_name = os.path.basename(file_path)
         file_name = os.path.splitext(file_name)[0]
         file_list.append(file_name)
 
     result_list = list(zip(file_list, parameters_list, error_list, strategy_list))
     file_path = filedialog.asksaveasfilename(defaultextension=".txt",
                                              filetypes=[("Text Files", "*.txt"), ("All Files", "*.*")])
     if file_path:
-        header = "File Name\tParameters\tError\tStrategy\n" 
+        header = "File Name\t" + "\t".join(header_list[:count]) + "\tError\tStrategy\n"
         with open(file_path, "w") as txtfile:
             txtfile.write(header)
             for rdata in result_list:
-                arr_str = np.array2string(rdata[1], separator=',', precision=6, suppress_small=True)
+                arr_str = '\t'.join(f"{element:.6f}" for element in rdata[1])
                 txtfile.write(f"{rdata[0]}\t{arr_str}\t{rdata[2]}\t{rdata[3]}\n")
 
 def plot_Simuall():
     Nums = variable_Num.get()
     pcommon = variable_pcommon.get()
     sigmaU = variable_sigmaU.get()
     sigmaD = variable_sigmaD.get()
@@ -697,16 +739,25 @@
         progressbar.pack_forget()
         parameters_list.append(best_result.x)
         error_list.append(result_fun)
         strategy_list.append(plot_strategy)
 
     result_window = tk.Tk()
     result_window.title('Estimated Parameters')
-    result_label2 = tk.Label(result_window, text=finalR)
-    result_label2.pack()
+
+    def on_scroll(*args):
+        text_box.yview(*args)
+
+    scrollbar = tk.Scrollbar(result_window)
+    scrollbar.pack(side=tk.RIGHT, fill=tk.Y)
+    text_box = tk.Text(result_window, wrap=tk.WORD, yscrollcommand=scrollbar.set)
+    text_box.pack(expand=True, fill=tk.BOTH)
+    scrollbar.config(command=text_box.yview)
+    text_box.insert(tk.END, finalR)
+
     result_label.config(text= 'Finished' , fg="black")
     save_paras = tk.Button(result_window, text="Save", command=save_p)
     save_paras.pack()
 
 
     
     
@@ -790,16 +841,16 @@
 
     # Save
     save_fit = tk.Button(fit_frame, text="Save", command=lambda: plot_func(2))
     save_fit.pack()
 
     
     # Back
-    plot_Simu_but = tk.Button(fit_frame, text="Main Page", fg="green", command=back_main1)
-    plot_Simu_but.pack()
+    Back_but = tk.Button(fit_frame, text="Main Page", fg="green", command=back_main1)
+    Back_but.pack()
 
     
     
 def back_main():
     simu_frame.pack_forget()
     open_welcome()
     
@@ -922,104 +973,107 @@
     
         entry_sti2 = tk.Entry(simu_frame, textvariable=variable_sti2, width=5)
         entry_sti2.pack()
         entry_sti2.bind('<Return>', entry_changed)
     
         
         pcommon_label = tk.Label(simu_frame, text="Pcommon", fg="black")
-        pcommon_label.place(relx=0.3, rely=0.09, anchor="w")
+        pcommon_label.place(relx=0.3, rely=0.08, anchor="w")
     
         sigmaU_label = tk.Label(simu_frame, text="sigmaU", fg="blue")
-        sigmaU_label.place(relx=0.3, rely=0.2, anchor="w")
+        sigmaU_label.place(relx=0.3, rely=0.19, anchor="w")
     
         sigmaD_label = tk.Label(simu_frame, text="sigmaD", fg="red")
-        sigmaD_label.place(relx=0.3, rely=0.3, anchor="w")
+        sigmaD_label.place(relx=0.3, rely=0.29, anchor="w")
     
         sigmaZ_label = tk.Label(simu_frame, text="sigmaZ", fg="black")
-        sigmaZ_label.place(relx=0.3, rely=0.41, anchor="w")
+        sigmaZ_label.place(relx=0.3, rely=0.395, anchor="w")
     
         mup_label = tk.Label(simu_frame, text="Z_center", fg="black")
-        mup_label.place(relx=0.3, rely=0.52, anchor="w")
+        mup_label.place(relx=0.3, rely=0.5, anchor="w")
     
     
         sti1_label = tk.Label(simu_frame, text="stimulusU", fg="blue")
-        sti1_label.place(relx=0.3, rely=0.63, anchor="w")
+        sti1_label.place(relx=0.3, rely=0.6, anchor="w")
     
         sti2_label = tk.Label(simu_frame, text="stimulusD", fg="red")
-        sti2_label.place(relx=0.3, rely=0.74, anchor="w")
+        sti2_label.place(relx=0.3, rely=0.7, anchor="w")
         
         placeholder = tk.Frame(simu_frame, height=90)
         placeholder.pack()
         # Plot
-        plot_Simu_but = tk.Button(simu_frame, text="Simulate", command=plot_Simu)
+        plot_Simu_but = tk.Button(simu_frame, text="Simulate", command= lambda: plot_Simu(1))
         plot_Simu_but.pack()
 
+        save_Simu_but = tk.Button(simu_frame, text="Save Simulated Data", command= lambda: plot_Simu(2))
+        save_Simu_but.pack()
+
         var_respD = tk.BooleanVar(value=True)
         var_stiE = tk.BooleanVar()
         var_priorD = tk.BooleanVar()
 
         button_respD = tk.Checkbutton(simu_frame, text="Response Distribution", variable=var_respD)
         button_stiE= tk.Checkbutton(simu_frame, text="Stimulus Encoding", variable=var_stiE)
         button_prior = tk.Checkbutton(simu_frame, text="Prior Distribution", variable=var_priorD)
     
-        button_respD.place(relx=0.35, rely=0.8, anchor="e")
-        button_stiE.place(relx=0.65, rely=0.8, anchor="e")
-        button_prior.place(relx=0.95, rely=0.8, anchor="e")  
+        button_respD.place(relx=0.35, rely=0.75, anchor="e")
+        button_stiE.place(relx=0.65, rely=0.75, anchor="e")
+        button_prior.place(relx=0.95, rely=0.75, anchor="e")  
 
         var_peak = tk.BooleanVar(value=True)
         var_mean = tk.BooleanVar()
         var_disp = tk.BooleanVar()
 
         button_peak = tk.Checkbutton(simu_frame, text="Peak", variable=var_peak)
         button_mean = tk.Checkbutton(simu_frame, text="Mean", variable=var_mean)
         button_disp = tk.Checkbutton(simu_frame, text="Display Value", variable=var_disp)
     
-        button_peak.place(relx=0.15, rely=0.9, anchor="e")
-        button_mean.place(relx=0.5, rely=0.9, anchor="e")
-        button_disp.place(relx=0.91, rely=0.9, anchor="e")  
+        button_peak.place(relx=0.15, rely=0.85, anchor="e")
+        button_mean.place(relx=0.5, rely=0.85, anchor="e")
+        button_disp.place(relx=0.91, rely=0.85, anchor="e")  
         
         
     else:
         
         entry_N = tk.Entry(simu_frame, textvariable=variable_Num, width=3)
         entry_N.pack()
     
         # Plot
-        placeholder = tk.Frame(simu_frame, height=30)
+        placeholder = tk.Frame(simu_frame, height=50)
         placeholder.pack()
         plot_Simuall_but = tk.Button(simu_frame, text="Simulate", command=plot_Simuall)
         plot_Simuall_but.pack()
         pcommon_label = tk.Label(simu_frame, text="Pcommon", fg="black")
-        pcommon_label.place(relx=0.3, rely=0.12, anchor="w")
+        pcommon_label.place(relx=0.3, rely=0.11, anchor="w")
     
         sigmaU_label = tk.Label(simu_frame, text="sigmaU", fg="blue")
-        sigmaU_label.place(relx=0.3, rely=0.27, anchor="w")
+        sigmaU_label.place(relx=0.3, rely=0.26, anchor="w")
     
         sigmaD_label = tk.Label(simu_frame, text="sigmaD", fg="red")
-        sigmaD_label.place(relx=0.3, rely=0.43, anchor="w")
+        sigmaD_label.place(relx=0.3, rely=0.4, anchor="w")
     
         sigmaZ_label = tk.Label(simu_frame, text="sigmaZ", fg="black")
-        sigmaZ_label.place(relx=0.3, rely=0.57, anchor="w")
+        sigmaZ_label.place(relx=0.3, rely=0.54, anchor="w")
     
         mup_label = tk.Label(simu_frame, text="Z_center", fg="black")
-        mup_label.place(relx=0.3, rely=0.72, anchor="w")
+        mup_label.place(relx=0.3, rely=0.68, anchor="w")
         Num_label = tk.Label(simu_frame, text="Number of stimuli", fg="black")
-        Num_label.place(relx=0.3, rely=0.78, anchor="center")
+        Num_label.place(relx=0.3, rely=0.75, anchor="center")
                 
     var_a_simu = tk.BooleanVar(value=True)
     var_b_simu = tk.BooleanVar()
     var_c_simu = tk.BooleanVar()
 
     check_button_a_simu = tk.Checkbutton(simu_frame, text="Averaging", variable=var_a_simu, command=function_a_simu)
     check_button_b_simu = tk.Checkbutton(simu_frame, text="Selecting", variable=var_b_simu, command=function_b_simu)
     check_button_c_simu = tk.Checkbutton(simu_frame, text="Matching", variable=var_c_simu, command=function_c_simu)
     
-    check_button_a_simu.place(relx=0.2, rely=0.85, anchor="e")
-    check_button_b_simu.place(relx=0.53, rely=0.85, anchor="e")
-    check_button_c_simu.place(relx=0.86, rely=0.85, anchor="e")       
+    check_button_a_simu.place(relx=0.2, rely=0.8, anchor="e")
+    check_button_b_simu.place(relx=0.53, rely=0.8, anchor="e")
+    check_button_c_simu.place(relx=0.86, rely=0.8, anchor="e")       
     # Back
     plot_Simu_but = tk.Button(simu_frame, text="Main Page", fg="green", command=back_main)
     plot_Simu_but.pack()
 def open_welcome():
     global welcome_frame
     # Create Welcome page
     welcome_frame = tk.Frame(window)
@@ -1041,9 +1095,13 @@
 
     startSim_button = tk.Button(welcome_frame, text="Simulate for Continuous Condition", command=lambda: simu_page(1))
     startSim_button.place(relx=0.5, rely=0.45, anchor="center")
 
     startSimall_button = tk.Button(welcome_frame, text="Simulate for Numerosity Task", command=lambda: simu_page(2))
     startSimall_button.place(relx=0.5, rely=0.5, anchor="center")
 
+    about_button = tk.Button(welcome_frame, text="About BCI Toolbox", command=about_bci)
+    about_button.place(relx=0.5, rely=0.6, anchor="center")
+
     # 
     tk.Label(welcome_frame).pack()
+
```

