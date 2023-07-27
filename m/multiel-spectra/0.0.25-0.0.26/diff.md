# Comparing `tmp/multiel_spectra-0.0.25.tar.gz` & `tmp/multiel_spectra-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiel_spectra-0.0.25.tar", last modified: Wed Jun 21 16:49:01 2023, max compression
+gzip compressed data, was "multiel_spectra-0.0.26.tar", last modified: Thu Jul 27 10:49:44 2023, max compression
```

## Comparing `multiel_spectra-0.0.25.tar` & `multiel_spectra-0.0.26.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 16:49:01.364710 multiel_spectra-0.0.25/
--rw-rw-rw-   0        0        0      352 2023-06-13 15:09:48.000000 multiel_spectra-0.0.25/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-06-21 16:49:01.282136 multiel_spectra-0.0.25/.github/
-drwxrwxrwx   0        0        0        0 2023-06-21 16:49:01.371248 multiel_spectra-0.0.25/.github/workflows/
--rw-rw-rw-   0        0        0      667 2023-06-13 15:56:38.000000 multiel_spectra-0.0.25/.github/workflows/release.yml
--rw-rw-rw-   0        0        0      613 2023-06-13 15:09:48.000000 multiel_spectra-0.0.25/.github/workflows/test.yml
--rw-rw-rw-   0        0        0     2173 2023-06-13 15:09:48.000000 multiel_spectra-0.0.25/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-21 16:49:01.376246 multiel_spectra-0.0.25/.vscode/
--rw-rw-rw-   0        0        0      187 2023-06-13 15:09:48.000000 multiel_spectra-0.0.25/.vscode/settings.json
--rw-rw-rw-   0        0        0     1100 2023-06-13 15:09:48.000000 multiel_spectra-0.0.25/LICENSE
--rw-rw-rw-   0        0        0      175 2023-06-19 12:44:52.000000 multiel_spectra-0.0.25/MANIFEST.in
--rw-rw-rw-   0        0        0     8263 2023-06-21 16:49:01.505987 multiel_spectra-0.0.25/PKG-INFO
--rw-rw-rw-   0        0        0     7031 2023-06-20 13:25:46.000000 multiel_spectra-0.0.25/README.md
--rw-rw-rw-   0        0        0      101 2023-06-13 15:09:48.000000 multiel_spectra-0.0.25/pyproject.toml
--rw-rw-rw-   0        0        0      126 2023-06-21 16:49:01.512553 multiel_spectra-0.0.25/setup.cfg
--rw-rw-rw-   0        0        0     2632 2023-06-19 16:14:52.000000 multiel_spectra-0.0.25/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:49:01.282136 multiel_spectra-0.0.25/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 16:49:01.396873 multiel_spectra-0.0.25/src/multiel_spectra/
--rw-rw-rw-   0        0        0       58 2023-06-20 13:25:56.000000 multiel_spectra-0.0.25/src/multiel_spectra/__init__.py
--rw-rw-rw-   0        0        0      311 2023-06-14 14:06:06.000000 multiel_spectra-0.0.25/src/multiel_spectra/install_skbeam.py
--rw-rw-rw-   0        0        0      231 2023-06-13 15:27:34.000000 multiel_spectra-0.0.25/src/multiel_spectra/install_spekpy.py
--rw-rw-rw-   0        0        0    63836 2023-06-19 16:55:34.000000 multiel_spectra-0.0.25/src/multiel_spectra/multiel_spectra.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:49:01.484440 multiel_spectra-0.0.25/src/multiel_spectra.egg-info/
--rw-rw-rw-   0        0        0     8263 2023-06-21 16:48:59.000000 multiel_spectra-0.0.25/src/multiel_spectra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-06-21 16:49:00.000000 multiel_spectra-0.0.25/src/multiel_spectra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       58 2023-06-21 16:48:59.000000 multiel_spectra-0.0.25/src/multiel_spectra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-06-21 16:48:59.000000 multiel_spectra-0.0.25/src/multiel_spectra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-21 16:48:59.000000 multiel_spectra-0.0.25/src/multiel_spectra.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 16:49:01.496921 multiel_spectra-0.0.25/tests/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:09:48.000000 multiel_spectra-0.0.25/tests/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-06-19 13:58:38.000000 multiel_spectra-0.0.25/tests/test_module1.py
--rw-rw-rw-   0        0        0      295 2023-06-13 15:09:48.000000 multiel_spectra-0.0.25/tox.ini
--rw-rw-rw-   0        0        0       33 2023-06-13 15:09:48.000000 multiel_spectra-0.0.25/vscode.env
+drwxrwxrwx   0        0        0        0 2023-07-27 10:49:43.982496 multiel_spectra-0.0.26/
+-rw-rw-rw-   0        0        0      352 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-07-27 10:49:43.921180 multiel_spectra-0.0.26/.github/
+drwxrwxrwx   0        0        0        0 2023-07-27 10:49:43.989853 multiel_spectra-0.0.26/.github/workflows/
+-rw-rw-rw-   0        0        0      667 2023-06-13 15:56:38.000000 multiel_spectra-0.0.26/.github/workflows/release.yml
+-rw-rw-rw-   0        0        0      613 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0     2173 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-27 10:49:43.993917 multiel_spectra-0.0.26/.vscode/
+-rw-rw-rw-   0        0        0      187 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1100 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/LICENSE
+-rw-rw-rw-   0        0        0      175 2023-06-19 12:44:52.000000 multiel_spectra-0.0.26/MANIFEST.in
+-rw-rw-rw-   0        0        0     8263 2023-07-27 10:49:44.042986 multiel_spectra-0.0.26/PKG-INFO
+-rw-rw-rw-   0        0        0     7031 2023-06-20 13:25:46.000000 multiel_spectra-0.0.26/README.md
+-rw-rw-rw-   0        0        0      101 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/pyproject.toml
+-rw-rw-rw-   0        0        0      126 2023-07-27 10:49:44.051008 multiel_spectra-0.0.26/setup.cfg
+-rw-rw-rw-   0        0        0     2632 2023-06-19 16:14:52.000000 multiel_spectra-0.0.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:49:43.928383 multiel_spectra-0.0.26/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 10:49:44.010402 multiel_spectra-0.0.26/src/multiel_spectra/
+-rw-rw-rw-   0        0        0       58 2023-07-27 10:49:36.000000 multiel_spectra-0.0.26/src/multiel_spectra/__init__.py
+-rw-rw-rw-   0        0        0      311 2023-06-14 14:06:06.000000 multiel_spectra-0.0.26/src/multiel_spectra/install_skbeam.py
+-rw-rw-rw-   0        0        0      231 2023-06-13 15:27:34.000000 multiel_spectra-0.0.26/src/multiel_spectra/install_spekpy.py
+-rw-rw-rw-   0        0        0    75340 2023-07-27 10:39:13.000000 multiel_spectra-0.0.26/src/multiel_spectra/multiel_spectra.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:49:44.035097 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/
+-rw-rw-rw-   0        0        0     8263 2023-07-27 10:49:42.000000 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-07-27 10:49:43.000000 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       58 2023-07-27 10:49:42.000000 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-27 10:49:42.000000 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-27 10:49:42.000000 multiel_spectra-0.0.26/src/multiel_spectra.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 10:49:44.042986 multiel_spectra-0.0.26/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/tests/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-06-19 13:58:38.000000 multiel_spectra-0.0.26/tests/test_module1.py
+-rw-rw-rw-   0        0        0      295 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/tox.ini
+-rw-rw-rw-   0        0        0       33 2023-06-13 15:09:48.000000 multiel_spectra-0.0.26/vscode.env
```

### Comparing `multiel_spectra-0.0.25/.github/workflows/release.yml` & `multiel_spectra-0.0.26/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.25/.github/workflows/test.yml` & `multiel_spectra-0.0.26/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.25/.gitignore` & `multiel_spectra-0.0.26/.gitignore`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.25/LICENSE` & `multiel_spectra-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.25/PKG-INFO` & `multiel_spectra-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiel_spectra
-Version: 0.0.25
+Version: 0.0.26
 Summary: Multi-Element Fluorescence Xray Spectra Generator
 Home-page: https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Author: Fernando Garcia-Avello 
 Author-email: fgarciaa@fi.infn.it
 Project-URL: Documentation, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Bug Reports, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Source Code, https://github.com/Fernandogarciagoatcoder/multiel_spectra
```

### Comparing `multiel_spectra-0.0.25/README.md` & `multiel_spectra-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.25/setup.py` & `multiel_spectra-0.0.26/setup.py`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.25/src/multiel_spectra/multiel_spectra.py` & `multiel_spectra-0.0.26/src/multiel_spectra/multiel_spectra.py`

 * *Files 16% similar despite different names*

```diff
@@ -102,22 +102,38 @@
 reduced_lines_l = unziped_l[1]
 peaks_dic  = dict(zip(reduced_lines_l, energies)) 
 
 #incluir algo para introducir uno su propia reduced_list, o los elementos que quieran o todos
 
 def multi_trans_gen(a, Prim_s, bPrim_s):
     """
-    Interesa solo la absorción por lo que no uso el componente fotoelectrico.
-    Se devuelve solo aquello transmitido no lo que excita
+    Simulate X-ray fluorescence (XRF) generation and transmission through a list of elements.
 
-    la lista de las proporciones de los elementos tiene que ser con todos los elementos, es decir, la mayoria 0 excepto algunos, 
-    hacer en manera random el orden de los estratos. Porque de momento están ordenados por Z. 
+    XRF Generation and Transmission through the elements given in 'a', using the Primary spectrum 
+    given by 'Prim_s' with the background (bremsstrahlung) component given by 'bPrim_s'. The spectra transmission 
+    goes from the last element of the 'a' array until the first. That is, the first element has no 
+    transmission, and the last element is transmitted through the whole list given in 'a'. 
 
-    """
-  
+    Args:
+        a (list): A list of element indices representing the elements through which XRF generation and 
+                  transmission are to be simulated.
+        Prim_s (tuple): Tuple containing two arrays representing the primary peaks and their corresponding probabilities.
+        bPrim_s (tuple): Tuple containing two arrays representing the bremsstrahlung primary peaks and their corresponding probabilities.
+
+    Returns:
+        tuple: A tuple containing three elements:
+               - air_spectra (array): The transmitted spectrum after XRF generation and absorption through the elements.
+               - peaks_pos (array): A binary array indicating the presence of peaks in the spectrum.
+               - c (array): A probability distribution representing the composition of the material.
+
+    Note: The function simulates XRF generation and transmission through the specified elements and computes the transmitted spectrum.
+          It considers the effect of XRF generation, absorption through the elements, and air absorption in the final transmitted spectrum.
+          The function relies on other helper functions like 'sum_prima' and 'material_mu'.
+          The 'air_density' variable is assumed to be defined elsewhere in the code.
+    """  
     mask = [b not in a for b in np.arange(0,41,1)]
     c = np.random.random(len(reduced_list)) #/np.sum(c) para normalizar
     c = c/np.sum(c)
     c[mask]=0
     n = c[c> 0] 
     el_list = []
     peaks_pos = np.zeros(len(peaks_dic))
@@ -155,20 +171,37 @@
 
     air_spectra = Narea(final_spectra* np.exp(-q_air))
 
     return air_spectra, peaks_pos, c  # c es reduced list con elementos 0s y 1s. 
 
 def ind_trans_gen(N, Prim_s, bPrim_s):
     """
-    Interesa solo la absorción por lo que no uso el componente fotoelectrico.
-    Se devuelve solo aquello transmitido no lo que excita
+    Simulate the transmission of X-rays through a single element and generate the transmitted spectrum after absorption.
+
+    Only the absorption component is considered, and the photoelectric component is not used. The function
+    returns only the transmitted spectrum, not the exciting spectrum.
 
-    la lista de las proporciones de los elementos tiene que ser con todos los elementos, es decir, la mayoria 0 excepto algunos, 
-    hacer en manera random el orden de los estratos. Porque de momento están ordenados por Z. 
+    The list of proportions of the elements ('c') should contain all the elements, but most of them should have
+    a proportion of 0 except for the specified element represented by the index 'N'.
+
+    Args:
+        N (int): The index of the element to simulate the transmission through.
+        Prim_s (tuple): Tuple containing two arrays representing the primary peaks and their corresponding probabilities.
+        bPrim_s (tuple): Tuple containing two arrays representing the background primary peaks and their corresponding probabilities.
 
+    Returns:
+        tuple: A tuple containing three elements:
+               - air_spectra (array): The transmitted spectrum after absorption through the specified element.
+               - peaks_pos (array): A binary array indicating the presence of peaks in the spectrum.
+               - c (array): A probability distribution representing the composition of the material.
+
+    Note: The function simulates the absorption of X-rays through the specified element and computes the transmitted spectrum.
+          It also considers the effect of air absorption in the final transmitted spectrum.
+          The function relies on other helper functions like 'sum_prima' and 'material_mu'.
+          The 'air_density' variable is assumed to be defined elsewhere in the code.
     """
     c = np.zeros(len(reduced_list))
     c[N]=1  
     el_list = []
     el_list.append(reduced_list[N]) 
 
     peaks_pos = np.zeros(len(peaks_dic))
@@ -185,19 +218,38 @@
 
     air_spectra =  Narea(prod_s*np.exp(-q_air))
 
     return air_spectra, peaks_pos, c  #la verdad que para lo que hace se podria omitir el ultimo calculo.
 
 def pair_trans_gen(a, Prim_s, bPrim_s ):
     """
-    Interesa solo la absorción por lo que no uso el componente fotoelectrico.
-    Se devuelve solo aquello transmitido no lo que excita
+    Simulate the transmission of X-rays through a material and generate the transmitted spectrum after absorption.
+
+    Only the absorption component is considered, and the photoelectric component is not used. The function
+    returns only the transmitted spectrum, not the exciting spectrum.
 
-    la lista de las proporciones de los elementos tiene que ser con todos los elementos, es decir, la mayoria 0 excepto algunos, 
-    hacer en manera random el orden de los estratos. Porque de momento están ordenados por Z. 
+    The list of proportions of the elements ('a') should contain all the elements, but most of them should have
+    a proportion of 0 except for some elements. The order of the elements should be randomized since they are 
+    currently ordered by Z.
+
+    Args:
+        a (list): A list of element indices representing the material's composition.
+        Prim_s (tuple): Tuple containing two arrays representing the primary peaks and their corresponding probabilities.
+        bPrim_s (tuple): Tuple containing two arrays representing the background primary peaks and their corresponding probabilities.
+
+    Returns:
+        tuple: A tuple containing three elements:
+               - air_spectra (array): The transmitted spectrum after absorption through the material.
+               - peaks_pos (array): A binary array indicating the presence of peaks in the spectrum.
+               - c (array): A probability distribution representing the composition of the material.
+
+    Note: The function simulates the absorption of X-rays through the material and computes the transmitted spectrum.
+          It also considers the effect of air absorption in the final transmitted spectrum.
+          The function relies on other helper functions like 'sum_prima' and 'material_mu'.
+          The 'air_density' variable is assumed to be defined elsewhere in the code.
     """
     mask = [b not in a for b in np.arange(0,41,1)]
     c = np.random.random(len(reduced_list)) #/np.sum(c) para normalizar
     c = c/np.sum(c)
     c[mask]=0
     n = c[c> 0] 
     el_list = []
@@ -233,23 +285,62 @@
     q_air = np.array(material_mu("air",  np.arange(0,30,0.05)*1000 )*air_density*air_z*1000*factor)
 
     air_spectra = Narea(final_spectra*np.exp(-q_air))
   
     return air_spectra, peaks_pos, c  
 
 def Narea(array):
+    """
+    Normalize an array to create a probability distribution.
+
+    The function takes an input array and normalizes it to create a probability distribution. 
+    The normalization is performed by dividing each element of the array by its maximum value and then 
+    dividing the resulting array by the sum of all elements.
+
+    Args:
+        array (array): The input array to be normalized.
+
+    Returns:
+        array: The normalized array representing a probability distribution.
+
+    Note: The normalized array will have values between 0 and 1, and the sum of all elements in the 
+          normalized array will be equal to 1, making it a probability distribution.
+    """
     a = array/np.max(array) 
     return a/np.sum(a)
 
-def escape_peaks(spectra, peaks_pos,c): # he quitado c porque no lo he usado, podria usarlo para seleccionar solo algun pico de algun elemento.
+def escape_peaks(spectra, peaks_pos,c): 
     """
-    En este caso hay que coger la linea de un pico (deberia ser uno de los más grandes) y restarle la Ka1 del silicio 1.73998 KeV (que depende del detector pero casi todos son de silicio). 
-    para crear un nuevo pico con esa energia. 
-    Faltaria meter la probabilidad de que se dieran escape peaks en funcion de la intensidad y la energia de los picos. 
+    Generate escape peaks given a histogram representing the spectra from which to add the escape peaks (spectra),
+    the energy position of the peaks (peaks_pos), and the elements present in the spectra (c).
+
+    Escape peaks are generated when the detector is excited by the X-ray radiation. Only the first line of Si 
+    is considered (at 1.73 KeV).
+
+    Args:
+        spectra (array): A histogram representing the spectra from which escape peaks are to be added.
+        peaks_pos (array): Energy positions of the peaks in the spectrum.
+        c (array): Elements present in the spectra.
+
+    Returns:
+        tuple: A tuple containing three elements:
+               - f_spectra (array): The spectra with the escape peaks added.
+               - peaks_pos (array): Energy positions of the peaks in the spectrum.
+               - c (array): Elements present in the spectra.
+
+    Note: This function simulates the creation of escape peaks for a histogram representing the spectra.
+          Escape peaks are generated by taking the line of a peak (typically one of the largest peaks)
+          and subtracting the Ka1 line of silicon at 1.73998 KeV to create a new peak with that energy.
+          The probability of generating escape peaks can be related to the intensity and energy of the peaks.
     """
+
+    #En este caso hay que coger la linea de un pico (deberia ser uno de los más grandes) y restarle la Ka1 del silicio 1.73998 KeV (que depende del detector pero casi todos son de silicio). 
+    #para crear un nuevo pico con esa energia. 
+    #Faltaria meter la probabilidad de que se dieran escape peaks en funcion de la intensidad y la energia de los picos. 
+
     #LA PROBABILIDAD DE QUE SE DE ESTO SERIA LA CROSS SECTION DE LA KA1 DEL SILICO POR EL PICO DE ENERGIA NO ????? 
     x = np.arange(0,30,0.05)
     area = 0.05 * np.sqrt(2 * np.pi)
     els = list(np.array(reduced_list)[c.astype(bool)])
     import scipy 
     peaks = scipy.signal.find_peaks(spectra, prominence = np.max(spectra)/15)
     prominences = sorted((zip(peaks[1]["prominences"], peaks[0])))
@@ -270,16 +361,37 @@
             f_spectra += gaussian(np.arange(0, 30, 0.05), np.sqrt(2 * np.pi)*0.1, x[pos]-1.73998, 0.1) * y_alt *perc
 
   
     return f_spectra, peaks_pos,c
 
 def sum_peaks(spectra, peaks_pos,c):
     """
-    Simplemente hay que sumar dos picos, es decir coger dos lineas de dos elementos y sumarlas para crear otro pico. 
+    Generate sum peaks given a histogram representing the spectra from which to add the escape peaks,
+    the energy position of the peaks, and the elements present in the spectra.
+
+    Sum peaks represent the situation when two photons arrive at the detector in a period of time 
+    shorter than the detector resolution, hence summing their energies.
+
+    Args:
+        spectra (array): A histogram representing the spectra from which to add escape peaks.
+        peaks_pos (array): Energy positions of the peaks in the spectrum.
+        c (array): Elements present in the spectra.
+
+    Returns:
+        tuple: A tuple containing three elements:
+               - f_spectra (array): The spectra with the sum peaks added.
+               - peaks_pos (array): Energy positions of the peaks in the spectrum.
+               - c (array): Elements present in the spectra.
+
+    Note: This function simulates the creation of sum peaks by taking two peaks and adding them together.
+          The prominence of the peaks is used to determine which peaks to select for summing.
+          The function also applies random factors to control the intensity of the sum peaks.
     """
+    #Simplemente hay que sumar dos picos, es decir coger dos lineas de dos elementos y sumarlas para crear otro pico. 
+
     x = np.arange(0,30,0.05)
     area = 0.05 * np.sqrt(2 * np.pi)
     els = list(np.array(reduced_list)[c.astype(bool)])
     import scipy 
     peaks = scipy.signal.find_peaks(spectra, prominence = np.max(spectra)/15)
     prominences = sorted((zip(peaks[1]["prominences"], peaks[0])))
     proms = list(zip(*prominences))[0]
@@ -304,15 +416,31 @@
             f_spectra -= gaussian(np.arange(0, 30, 0.05), area, x[pos2], 0.05) * y_alt *perc/2
             f_spectra += gaussian(np.arange(0, 30, 0.05), area, x[pos1] + x[pos2], 0.1) * y_alt *perc
 
     return f_spectra, peaks_pos,c
 
 def decalibration(spectra, params = []):
     """
-    El objetivo es descalibrar el espectro con transformaciones no solo lineales sino tambien no lineales ligeramente.  
+    Simulate decalibration effects in a spectrum. The decalibration is mainly linear 
+    with a small quadratic component. A spectrum for decalibration must be provided,
+    and the parameters for the transformation are optional.
+
+    Args:
+        spectra (array): The spectrum to be decalibrated.
+        params (list, optional): List of parameters [a, b, c] for the decalibration transformation.
+                                 If not provided, random values within certain ranges will be used.
+
+    Returns:
+        tuple: A tuple containing two elements:
+               - decalibrated_spectrum (array): The decalibrated spectrum after applying the transformation.
+               - params (list): List of parameters [a, b, c] used for the decalibration transformation.
+
+    Note: The decalibration transformation is represented as: x_tr = a + (1 + b) * x + c * x^2
+          Where 'x' is the energy range, and 'a', 'b', and 'c' are the decalibration parameters.
+          The function uses scipy's interp1d to perform the transformation.
     """
     from scipy.interpolate import interp1d
     x = np.arange(0,30,0.05)
     if params ==[]:
         a = np.random.uniform(low=-0.03, high=0.03)
         b = np.random.uniform(low=-0.03, high=0.03)
         c = np.random.uniform(low=-0.05, high=0.05)*10**(-3)
@@ -325,16 +453,30 @@
     return decal(x), [a,b,c]
 
 
 copia_inter = interp1d(x_c, y_c, bounds_error = False, fill_value = 0 )
 eff_inter = copia_inter(np.arange(0,30,0.05)) #modificar esto para que no sea un estandard
 
 def detector_eff(spectra_y, spectra_x, alpha = "", beta = ""):
-    """
-    Crear ventana de eficiencia de la red Neuronal. 
+    """_Function that simulates the efficiency window of a detector. That is the loss of 
+    counts due to the limited resolution of the x-ray detector window. For the moment per default the
+    efficiency of the LABEC (INFN-FLorence) efficiency window is taken and multiplied by a sigmoid function 
+    of parameters alpha and beta in order to modify slightly. _
+
+    Args:
+        spectra_y (_np.array_): _Y comonent of the Spectra _
+        spectra_x (_np.array_): _X comonent of the Spectra _
+        alpha (str, optional): _Alpha parameter of the sigma transformation. If not given it will be randomly generated_. Defaults to "".
+        beta (str, optional): _Beta parameter of the sigma transformation. If not given it will be randomly generated _. Defaults to "".
+
+    Raises:
+        ValueError: _X and Y components of the spectra must have same dimension _
+
+    Returns:
+        _type_: _A new Y component of the spectra representin the spectra that has been passed by the detector._
     """
     try:
         np.testing.assert_array_equal(np.shape(spectra_x), np.shape(spectra_y))
         if alpha =="": 
             alpha = np.random.uniform(low = 0.01 , high = 40 )# de vez en cuando podria dar un uno y un 0, que es como no tener eficiencia. 
         if beta =="": 
             beta = np.random.uniform(low = 0.01 , high = 40)
@@ -351,38 +493,77 @@
         return eff * spectra_y
     
     except AssertionError:
         raise ValueError("Arrays do not have the same dimensions.")
     
 
 def sigmoid(x, a, b):
-    """_summary_
+    """_Sigmoid function of a and b parameters_
 
     Args:
-        x (_type_): _description_
-        a (_type_): _description_
-        b (_type_): _description_
+        x (_np.array_): _Array to apply the transformation to_
+        a (_float_): _exponential parameter_
+        b (_flaat_): _linear parameter_
 
     Returns:
         _type_: _description_
     """
     if type(x) != np.ndarray: 
         x = np.array(x)
     return 1/(1 + b*np.exp(-x*a)) 
 
 def select_values(array, dictionary):
+    """
+    Select values and keys from a dictionary based on an array of conditions.
+
+    Args:
+        array (list): A list of values to act as conditions for selecting values and keys.
+        dictionary (dict): A dictionary from which values and keys will be selected.
+
+    Returns:
+        tuple: A tuple containing two lists - selected_values and selected_keys.
+               - selected_values (list): A list of values from the dictionary that correspond to the True elements in the 'array'.
+               - selected_keys (list): A list of keys from the dictionary that correspond to the True elements in the 'array'.
+    """
     mask = [value == 1 for value in array]
     selected_keys = [key for i, key in enumerate(dictionary.keys()) if mask[i]]
     selected_values = [value for i, value in enumerate(dictionary.values()) if mask[i]]
     
     return selected_values, selected_keys
 
 def spectra_gen(a, Prim, brems, s_counts = 30000,n_counts = 2000, b_counts = 3000, c_counts = 3000,plot = True,  escape = True, sum = True, decal = True, char_r = 15, brem_r = 5,noise_f = 1000, prop = "" ):
     #convertir a en numeros en caso de que sean los nombres de los elementos: 
+    """
+    Generate a spectrum with various components based on input parameters.
+
+    Args:
+        a (str or list): Element(s) or spectrum to be processed. If it's a str, convert it to numerical values representing elements.
+        Prim (tuple): Tuple containing two arrays representing primary peaks and their corresponding probabilities.
+        brems (tuple): Tuple containing two arrays representing bremsstrahlung peaks and their corresponding probabilities.
+        s_counts (int): Number of counts in the main spectrum.
+        n_counts (int): Number of counts in the noise spectrum.
+        b_counts (int): Number of counts in the bremsstrahlung spectrum.
+        c_counts (int): Number of counts in the characteristic spectrum.
+        plot (bool): If True, plot the generated spectrum using Bokeh.
+        escape (bool): If True, apply escape peak correction to the spectrum.
+        sum (bool): If True, sum the peaks in the spectrum.
+        decal (bool): If True, apply decalibration to the spectrum.
+        char_r (float): Characteristic peak range.
+        brem_r (float): Bremsstrahlung peak range.
+        noise_f (int): Factor to control the noise level in the spectrum.
+        prop (float): Proportion parameter for adjusting the contribution of certain components.
 
+    Returns:
+        tuple: A tuple containing two elements:
+               - final_d (array): The generated spectrum with various components combined.
+               - params (dict): Dictionary containing parameters related to the generated spectrum.
+
+    Note: Some functions like multi_trans_gen, escape_peaks, sum_peaks, decalibration, and detector_eff are assumed
+          to be defined elsewhere and used in this function.
+    """
     spec, peaks, els = multi_trans_gen( a, Prim,brems)
     if escape == True: 
         spec = escape_peaks(spec,peaks, els)[0]
     if sum == True:
         spec = sum_peaks(spec,peaks, els)[0]
     if decal == True: 
         spec, params = decalibration(spec)
@@ -402,15 +583,15 @@
         from bokeh.plotting import figure, show
         from bokeh.models import HoverTool, ColumnDataSource
         from bokeh.io import output_notebook
 
         output_notebook()
 
         es, names = select_values(peaks, peaks_dic)
-        box_indices = np.digitize(es, np.arange(0,30,0.05))
+        box_indices = np.digitize(es, np.arange(0,30,0.05))-1 # si no da error en el 600 
         xs = np.arange(0, 30, 0.05)[box_indices]
         ys = spec[box_indices]
 
         source = ColumnDataSource(data=dict(xs=xs, ys=ys, y0=np.zeros_like(es), names=names))
         # Create a figure object
         p = figure()
```

### Comparing `multiel_spectra-0.0.25/src/multiel_spectra.egg-info/PKG-INFO` & `multiel_spectra-0.0.26/src/multiel_spectra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiel-spectra
-Version: 0.0.25
+Version: 0.0.26
 Summary: Multi-Element Fluorescence Xray Spectra Generator
 Home-page: https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Author: Fernando Garcia-Avello 
 Author-email: fgarciaa@fi.infn.it
 Project-URL: Documentation, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Bug Reports, https://github.com/Fernandogarciagoatcoder/multiel_spectra
 Project-URL: Source Code, https://github.com/Fernandogarciagoatcoder/multiel_spectra
```

### Comparing `multiel_spectra-0.0.25/src/multiel_spectra.egg-info/SOURCES.txt` & `multiel_spectra-0.0.26/src/multiel_spectra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiel_spectra-0.0.25/tests/test_module1.py` & `multiel_spectra-0.0.26/tests/test_module1.py`

 * *Files identical despite different names*

