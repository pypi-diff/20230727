# Comparing `tmp/ciditel_utilities-0.2.1.tar.gz` & `tmp/ciditel_utilities-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciditel_utilities-0.2.1.tar", last modified: Thu Mar 16 17:53:53 2023, max compression
+gzip compressed data, was "ciditel_utilities-0.3.tar", last modified: Wed Jul 26 22:02:55 2023, max compression
```

## Comparing `ciditel_utilities-0.2.1.tar` & `ciditel_utilities-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 verushkab  (1000) verushkab  (1000)        0 2023-03-16 17:53:53.334206 ciditel_utilities-0.2.1/
--rw-r--r--   0 verushkab  (1000) verushkab  (1000)     1067 2023-02-18 22:29:27.000000 ciditel_utilities-0.2.1/LICENSE.txt
--rw-rw-r--   0 verushkab  (1000) verushkab  (1000)      106 2023-03-16 17:53:53.334206 ciditel_utilities-0.2.1/PKG-INFO
--rw-r--r--   0 verushkab  (1000) verushkab  (1000)     1123 2023-02-28 19:11:32.000000 ciditel_utilities-0.2.1/README.md
-drwxrwxr-x   0 verushkab  (1000) verushkab  (1000)        0 2023-03-16 17:53:53.334206 ciditel_utilities-0.2.1/ciditel_utilities/
--rw-r--r--   0 verushkab  (1000) verushkab  (1000)        0 2023-02-20 23:36:21.000000 ciditel_utilities-0.2.1/ciditel_utilities/__init__.py
--rw-r--r--   0 verushkab  (1000) verushkab  (1000)     2518 2023-02-28 18:47:07.000000 ciditel_utilities-0.2.1/ciditel_utilities/strings.py
--rw-rw-r--   0 verushkab  (1000) verushkab  (1000)     2109 2023-03-16 17:43:21.000000 ciditel_utilities-0.2.1/ciditel_utilities/validate.py
-drwxrwxr-x   0 verushkab  (1000) verushkab  (1000)        0 2023-03-16 17:53:53.334206 ciditel_utilities-0.2.1/ciditel_utilities.egg-info/
--rw-rw-r--   0 verushkab  (1000) verushkab  (1000)      106 2023-03-16 17:53:53.000000 ciditel_utilities-0.2.1/ciditel_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 verushkab  (1000) verushkab  (1000)      293 2023-03-16 17:53:53.000000 ciditel_utilities-0.2.1/ciditel_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 verushkab  (1000) verushkab  (1000)        1 2023-03-16 17:53:53.000000 ciditel_utilities-0.2.1/ciditel_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 verushkab  (1000) verushkab  (1000)       18 2023-03-16 17:53:53.000000 ciditel_utilities-0.2.1/ciditel_utilities.egg-info/top_level.txt
--rw-r--r--   0 verushkab  (1000) verushkab  (1000)       79 2023-03-16 17:53:53.334206 ciditel_utilities-0.2.1/setup.cfg
--rw-r--r--   0 verushkab  (1000) verushkab  (1000)      167 2023-03-16 17:44:51.000000 ciditel_utilities-0.2.1/setup.py
+drwxrwxr-x   0 verushkab  (1000) verushkab  (1000)        0 2023-07-26 22:02:55.948455 ciditel_utilities-0.3/
+-rw-r--r--   0 verushkab  (1000) verushkab  (1000)     1067 2023-02-18 22:29:27.000000 ciditel_utilities-0.3/LICENSE.txt
+-rw-rw-r--   0 verushkab  (1000) verushkab  (1000)      104 2023-07-26 22:02:55.948455 ciditel_utilities-0.3/PKG-INFO
+-rw-r--r--   0 verushkab  (1000) verushkab  (1000)     1123 2023-02-28 19:11:32.000000 ciditel_utilities-0.3/README.md
+drwxrwxr-x   0 verushkab  (1000) verushkab  (1000)        0 2023-07-26 22:02:55.948455 ciditel_utilities-0.3/ciditel_utilities/
+-rw-r--r--   0 verushkab  (1000) verushkab  (1000)        0 2023-02-20 23:36:21.000000 ciditel_utilities-0.3/ciditel_utilities/__init__.py
+-rw-r--r--   0 verushkab  (1000) verushkab  (1000)     2518 2023-02-28 18:47:07.000000 ciditel_utilities-0.3/ciditel_utilities/strings.py
+-rw-rw-r--   0 verushkab  (1000) verushkab  (1000)     2419 2023-07-26 20:58:02.000000 ciditel_utilities-0.3/ciditel_utilities/validate.py
+drwxrwxr-x   0 verushkab  (1000) verushkab  (1000)        0 2023-07-26 22:02:55.948455 ciditel_utilities-0.3/ciditel_utilities.egg-info/
+-rw-rw-r--   0 verushkab  (1000) verushkab  (1000)      104 2023-07-26 22:02:55.000000 ciditel_utilities-0.3/ciditel_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 verushkab  (1000) verushkab  (1000)      293 2023-07-26 22:02:55.000000 ciditel_utilities-0.3/ciditel_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 verushkab  (1000) verushkab  (1000)        1 2023-07-26 22:02:55.000000 ciditel_utilities-0.3/ciditel_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 verushkab  (1000) verushkab  (1000)       18 2023-07-26 22:02:55.000000 ciditel_utilities-0.3/ciditel_utilities.egg-info/top_level.txt
+-rw-r--r--   0 verushkab  (1000) verushkab  (1000)       79 2023-07-26 22:02:55.952455 ciditel_utilities-0.3/setup.cfg
+-rw-r--r--   0 verushkab  (1000) verushkab  (1000)      166 2023-07-26 22:02:39.000000 ciditel_utilities-0.3/setup.py
```

### Comparing `ciditel_utilities-0.2.1/LICENSE.txt` & `ciditel_utilities-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ciditel_utilities-0.2.1/README.md` & `ciditel_utilities-0.3/README.md`

 * *Files identical despite different names*

### Comparing `ciditel_utilities-0.2.1/ciditel_utilities/strings.py` & `ciditel_utilities-0.3/ciditel_utilities/strings.py`

 * *Files identical despite different names*

### Comparing `ciditel_utilities-0.2.1/ciditel_utilities/validate.py` & `ciditel_utilities-0.3/ciditel_utilities/validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,37 +38,44 @@
     cont = 0
     string = string.upper()
     #CURP contiene 18 caracteres
     #4 letras (nombre)
     #6 numeros (fecha de nacimiento)
     #1 letra (genero H-M-N)
     #5 letras (lugar de nacimiento)
-    #2 numeros al final 
+    #1 DIGITO ALFANUMERICO
+    #1 numero al final 
 
     if cantidad ==18:
             string = list(string)
             for i in string:
                 cont += 1
                 if (cont <=4):
                     p = i.isalpha()
                     if not p:
                         return False
-                elif (cont == 11 and i not in ['H','N','M']):
+                elif (cont == 11 and i not in ['H','M']):
                     return False
                 else:
                     if cont in range(5,11):
                         p = i.isdigit()
                         if not p:
                             return False
                     elif (cont in range(11,17)):
                         p = i.isalpha()
                         if not p:
                             return False
                     else:
-                        if cont in range(17,19):
+                        if cont in range(17,18):
                             p = i.isdigit()
-                            if not p:
-                                return False
+                            if not p :
+                                p = i.isalpha()
+                                if not p :
+                                    return False
+                        elif cont in range(18,19):
+                                p = i.isdigit()
+                                if not p :
+                                    return False
     else:
         return False
 
-    return True
+    return True
```

