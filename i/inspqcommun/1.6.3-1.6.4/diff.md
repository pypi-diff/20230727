# Comparing `tmp/inspqcommun-1.6.3.tar.gz` & `tmp/inspqcommun-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspqcommun-1.6.3.tar", last modified: Wed May 31 15:48:17 2023, max compression
+gzip compressed data, was "inspqcommun-1.6.4.tar", last modified: Thu Jul 27 17:22:13 2023, max compression
```

## Comparing `inspqcommun-1.6.3.tar` & `inspqcommun-1.6.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:17.916043 inspqcommun-1.6.3/
--rw-r--r--   0 jenkins    (114) jenkins    (119)    12567 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/LICENSE
--rw-r--r--   0 jenkins    (114) jenkins    (119)      790 2023-05-31 15:48:17.916043 inspqcommun-1.6.3/PKG-INFO
--rw-r--r--   0 jenkins    (114) jenkins    (119)      509 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/README.md
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:17.912043 inspqcommun-1.6.3/inspqcommun/
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:17.912043 inspqcommun-1.6.3/inspqcommun/hl7/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/hl7/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)   115322 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/hl7/fhir.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:17.912043 inspqcommun-1.6.3/inspqcommun/identity/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/identity/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)   164019 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/identity/keycloak.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1413 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/identity/keycloak_token.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     6729 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/identity/keycloak_tools.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:17.912043 inspqcommun-1.6.3/inspqcommun/kafka/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/kafka/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     7943 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/kafka/consommateur.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     5280 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/kafka/producteur.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:17.912043 inspqcommun-1.6.3/inspqcommun/userprovisioning/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/userprovisioning/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     9944 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/inspqcommun/userprovisioning/scim.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:17.912043 inspqcommun-1.6.3/inspqcommun.egg-info/
--rw-r--r--   0 jenkins    (114) jenkins    (119)      790 2023-05-31 15:48:17.000000 inspqcommun-1.6.3/inspqcommun.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (114) jenkins    (119)      717 2023-05-31 15:48:17.000000 inspqcommun-1.6.3/inspqcommun.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)        1 2023-05-31 15:48:17.000000 inspqcommun-1.6.3/inspqcommun.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)      104 2023-05-31 15:48:17.000000 inspqcommun-1.6.3/inspqcommun.egg-info/requires.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)       12 2023-05-31 15:48:17.000000 inspqcommun-1.6.3/inspqcommun.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)       38 2023-05-31 15:48:17.916043 inspqcommun-1.6.3/setup.cfg
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1412 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/setup.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-05-31 15:48:17.912043 inspqcommun-1.6.3/tests/
--rw-r--r--   0 jenkins    (114) jenkins    (119)   263660 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/tests/test_fhir.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    21724 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/tests/test_integration_fhir.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     3932 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/tests/test_integration_keycloak.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     3154 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/tests/test_kafka.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    17366 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/tests/test_keycloak.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    20775 2023-05-31 15:48:00.000000 inspqcommun-1.6.3/tests/test_scim.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:22:13.447197 inspqcommun-1.6.4/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    12567 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/LICENSE
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      790 2023-07-27 17:22:13.447197 inspqcommun-1.6.4/PKG-INFO
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      509 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/README.md
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:22:13.443197 inspqcommun-1.6.4/inspqcommun/
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:22:13.443197 inspqcommun-1.6.4/inspqcommun/hl7/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/hl7/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)   115190 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/hl7/fhir.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:22:13.447197 inspqcommun-1.6.4/inspqcommun/identity/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/identity/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)   164019 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/identity/keycloak.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1413 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/identity/keycloak_token.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     6729 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/identity/keycloak_tools.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:22:13.447197 inspqcommun-1.6.4/inspqcommun/kafka/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/kafka/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     7943 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/kafka/consommateur.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5280 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/kafka/producteur.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:22:13.447197 inspqcommun-1.6.4/inspqcommun/userprovisioning/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/userprovisioning/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     9944 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/inspqcommun/userprovisioning/scim.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:22:13.443197 inspqcommun-1.6.4/inspqcommun.egg-info/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      790 2023-07-27 17:22:13.000000 inspqcommun-1.6.4/inspqcommun.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      717 2023-07-27 17:22:13.000000 inspqcommun-1.6.4/inspqcommun.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        1 2023-07-27 17:22:13.000000 inspqcommun-1.6.4/inspqcommun.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      104 2023-07-27 17:22:13.000000 inspqcommun-1.6.4/inspqcommun.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)       12 2023-07-27 17:22:13.000000 inspqcommun-1.6.4/inspqcommun.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)       38 2023-07-27 17:22:13.447197 inspqcommun-1.6.4/setup.cfg
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1412 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/setup.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2023-07-27 17:22:13.447197 inspqcommun-1.6.4/tests/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)   263660 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/tests/test_fhir.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    21724 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/tests/test_integration_fhir.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     3932 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/tests/test_integration_keycloak.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     3154 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/tests/test_kafka.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    17366 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/tests/test_keycloak.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    20775 2023-07-27 17:21:54.000000 inspqcommun-1.6.4/tests/test_scim.py
```

### Comparing `inspqcommun-1.6.3/LICENSE` & `inspqcommun-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/PKG-INFO` & `inspqcommun-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspqcommun
-Version: 1.6.3
+Version: 1.6.4
 Summary: Librairies communes de INSPQ
 Home-page: https://gitlab.forge.gouv.qc.ca/inspq/commun/python/inspqcommun.git
 Author: Philippe Gauthier
 Author-email: philippe.gauthier@inspq.qc.ca
 License: LiLiQ
 License-File: LICENSE
```

### Comparing `inspqcommun-1.6.3/inspqcommun/hl7/fhir.py` & `inspqcommun-1.6.4/inspqcommun/hl7/fhir.py`

 * *Files 0% similar despite different names*

```diff
@@ -1486,5723 +1486,5715 @@
 00005cd0: 656e 5f68 6561 6465 723d 746f 6b65 6e5f  en_header=token_
 00005ce0: 6865 6164 6572 290a 2020 2020 2020 2020  header).        
 00005cf0: 7365 6c66 2e76 616c 6964 6174 655f 6365  self.validate_ce
 00005d00: 7274 7320 3d20 7661 6c69 6461 7465 5f63  rts = validate_c
 00005d10: 6572 7473 0a20 2020 2020 2020 2069 6620  erts.        if 
 00005d20: 696d 6d5f 6469 6374 2069 7320 4e6f 6e65  imm_dict is None
 00005d30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00005d40: 6c66 2e63 7265 6174 696f 6e5f 6461 7465  lf.creation_date
-00005d50: 203d 2064 6174 652e 746f 6461 7928 290a   = date.today().
-00005d60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005d70: 2e6c 6173 745f 7570 6461 7465 6420 3d20  .last_updated = 
-00005d80: 6461 7465 7469 6d65 2e6e 6f77 2829 0a20  datetime.now(). 
-00005d90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005da0: 6461 7465 203d 2064 6174 6574 696d 652e  date = datetime.
-00005db0: 6e6f 7728 290a 2020 2020 2020 2020 2020  now().          
-00005dc0: 2020 7365 6c66 2e66 6869 725f 7265 736f    self.fhir_reso
-00005dd0: 7572 6365 203d 2073 656c 662e 746f 5f66  urce = self.to_f
-00005de0: 6869 725f 7265 736f 7572 6365 2829 0a20  hir_resource(). 
-00005df0: 2020 2020 2020 2065 6c73 653a 200a 2020         else: .  
-00005e00: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-00005e10: 726f 6d5f 6469 6374 2869 6d6d 5f64 6963  rom_dict(imm_dic
-00005e20: 743d 696d 6d5f 6469 6374 290a 0a0a 2020  t=imm_dict)...  
-00005e30: 2020 6465 6620 7365 745f 6964 2873 656c    def set_id(sel
-00005e40: 662c 2069 6d6d 756e 697a 6174 696f 6e3d  f, immunization=
-00005e50: 4e6f 6e65 2c20 6964 3d4e 6f6e 6529 3a0a  None, id=None):.
-00005e60: 2020 2020 2020 2020 6966 2069 6d6d 756e          if immun
-00005e70: 697a 6174 696f 6e20 6973 204e 6f6e 653a  ization is None:
-00005e80: 0a20 2020 2020 2020 2020 2020 2069 6d6d  .            imm
-00005e90: 756e 697a 6174 696f 6e20 3d20 7365 6c66  unization = self
-00005ea0: 2e66 6869 725f 7265 736f 7572 6365 0a20  .fhir_resource. 
-00005eb0: 2020 2020 2020 2069 6620 6964 2069 7320         if id is 
-00005ec0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00005ed0: 2020 2020 2020 7365 6c66 2e69 6420 3d20        self.id = 
-00005ee0: 6964 0a20 2020 2020 2020 2069 6d6d 756e  id.        immun
-00005ef0: 697a 6174 696f 6e2e 6964 203d 2073 656c  ization.id = sel
-00005f00: 662e 6964 0a0a 2020 2020 6465 6620 6765  f.id..    def ge
-00005f10: 745f 6964 2873 656c 662c 2069 6d6d 756e  t_id(self, immun
-00005f20: 697a 6174 696f 6e3d 4e6f 6e65 293a 0a20  ization=None):. 
-00005f30: 2020 2020 2020 2069 6620 696d 6d75 6e69         if immuni
-00005f40: 7a61 7469 6f6e 2069 7320 4e6f 6e65 3a0a  zation is None:.
-00005f50: 2020 2020 2020 2020 2020 2020 696d 6d75              immu
-00005f60: 6e69 7a61 7469 6f6e 203d 2073 656c 662e  nization = self.
-00005f70: 6668 6972 5f72 6573 6f75 7263 650a 0a20  fhir_resource.. 
-00005f80: 2020 2020 2020 2072 6574 7572 6e20 696d         return im
-00005f90: 6d75 6e69 7a61 7469 6f6e 2e69 640a 2020  munization.id.  
-00005fa0: 2020 2020 2020 0a20 2020 2064 6566 2067        .    def g
-00005fb0: 6574 5f6d 6574 615f 7570 6461 7465 645f  et_meta_updated_
-00005fc0: 6279 2873 656c 662c 2069 6d6d 756e 697a  by(self, immuniz
-00005fd0: 6174 696f 6e3d 4e6f 6e65 293a 0a20 2020  ation=None):.   
-00005fe0: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
-00005ff0: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-00006000: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
-00006010: 7a61 7469 6f6e 203d 2073 656c 662e 6668  zation = self.fh
-00006020: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
-00006030: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
-00006040: 696f 6e20 6973 204e 6f6e 6520 6f72 2069  ion is None or i
-00006050: 6d6d 756e 697a 6174 696f 6e2e 6d65 7461  mmunization.meta
-00006060: 2069 7320 4e6f 6e65 206f 7220 696d 6d75   is None or immu
-00006070: 6e69 7a61 7469 6f6e 2e6d 6574 612e 6578  nization.meta.ex
-00006080: 7465 6e73 696f 6e20 6973 204e 6f6e 653a  tension is None:
-00006090: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000060a0: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-000060b0: 2066 6f72 2065 7874 656e 7369 6f6e 2069   for extension i
-000060c0: 6e20 696d 6d75 6e69 7a61 7469 6f6e 2e6d  n immunization.m
-000060d0: 6574 612e 6578 7465 6e73 696f 6e3a 0a20  eta.extension:. 
-000060e0: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
-000060f0: 7465 6e73 696f 6e2e 7572 6c20 3d3d 2073  tension.url == s
-00006100: 656c 662e 7570 6461 7465 645f 6279 5f75  elf.updated_by_u
-00006110: 726c 3a0a 2020 2020 2020 2020 2020 2020  rl:.            
-00006120: 2020 2020 7265 7475 726e 2065 7874 656e      return exten
-00006130: 7369 6f6e 2e76 616c 7565 5374 7269 6e67  sion.valueString
-00006140: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006150: 4e6f 6e65 0a0a 2020 2020 6465 6620 6765  None..    def ge
-00006160: 745f 6d65 7461 5f63 7265 6174 6564 5f62  t_meta_created_b
-00006170: 7928 7365 6c66 2c20 696d 6d75 6e69 7a61  y(self, immuniza
-00006180: 7469 6f6e 3d4e 6f6e 6529 3a0a 2020 2020  tion=None):.    
-00006190: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
-000061a0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-000061b0: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
-000061c0: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
-000061d0: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
-000061e0: 2020 2069 6620 696d 6d75 6e69 7a61 7469     if immunizati
-000061f0: 6f6e 2069 7320 4e6f 6e65 206f 7220 696d  on is None or im
-00006200: 6d75 6e69 7a61 7469 6f6e 2e6d 6574 6120  munization.meta 
-00006210: 6973 204e 6f6e 6520 6f72 2069 6d6d 756e  is None or immun
-00006220: 697a 6174 696f 6e2e 6d65 7461 2e65 7874  ization.meta.ext
-00006230: 656e 7369 6f6e 2069 7320 4e6f 6e65 3a0a  ension is None:.
-00006240: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006250: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
-00006260: 666f 7220 6578 7465 6e73 696f 6e20 696e  for extension in
-00006270: 2069 6d6d 756e 697a 6174 696f 6e2e 6d65   immunization.me
-00006280: 7461 2e65 7874 656e 7369 6f6e 3a0a 2020  ta.extension:.  
-00006290: 2020 2020 2020 2020 2020 6966 2065 7874            if ext
-000062a0: 656e 7369 6f6e 2e75 726c 203d 3d20 7365  ension.url == se
-000062b0: 6c66 2e63 7265 6174 6564 5f62 795f 7572  lf.created_by_ur
-000062c0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
-000062d0: 2020 2072 6574 7572 6e20 6578 7465 6e73     return extens
-000062e0: 696f 6e2e 7661 6c75 6553 7472 696e 670a  ion.valueString.
-000062f0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00006300: 6f6e 650a 0a20 2020 2064 6566 2067 6574  one..    def get
-00006310: 5f6d 6574 615f 6372 6561 7469 6f6e 5f64  _meta_creation_d
-00006320: 6174 6528 7365 6c66 2c20 696d 6d75 6e69  ate(self, immuni
-00006330: 7a61 7469 6f6e 3d4e 6f6e 6529 3a0a 2020  zation=None):.  
-00006340: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
-00006350: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
-00006360: 2020 2020 2020 2020 2020 2069 6d6d 756e             immun
-00006370: 697a 6174 696f 6e20 3d20 7365 6c66 2e66  ization = self.f
-00006380: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
-00006390: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
-000063a0: 7469 6f6e 2069 7320 4e6f 6e65 206f 7220  tion is None or 
-000063b0: 696d 6d75 6e69 7a61 7469 6f6e 2e6d 6574  immunization.met
-000063c0: 6120 6973 204e 6f6e 6520 6f72 2069 6d6d  a is None or imm
-000063d0: 756e 697a 6174 696f 6e2e 6d65 7461 2e65  unization.meta.e
-000063e0: 7874 656e 7369 6f6e 2069 7320 4e6f 6e65  xtension is None
-000063f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00006400: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-00006410: 2020 666f 7220 6578 7465 6e73 696f 6e20    for extension 
-00006420: 696e 2069 6d6d 756e 697a 6174 696f 6e2e  in immunization.
-00006430: 6d65 7461 2e65 7874 656e 7369 6f6e 3a0a  meta.extension:.
-00006440: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-00006450: 7874 656e 7369 6f6e 2e75 726c 203d 3d20  xtension.url == 
-00006460: 7365 6c66 2e63 7265 6174 696f 6e5f 6461  self.creation_da
-00006470: 7465 5f75 726c 3a0a 2020 2020 2020 2020  te_url:.        
-00006480: 2020 2020 2020 2020 7265 7475 726e 2065          return e
-00006490: 7874 656e 7369 6f6e 2e76 616c 7565 4461  xtension.valueDa
-000064a0: 7465 0a20 2020 2020 2020 2072 6574 7572  te.        retur
-000064b0: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
-000064c0: 6765 745f 6d65 7461 5f76 6572 7369 6f6e  get_meta_version
-000064d0: 5f69 6428 7365 6c66 2c20 696d 6d75 6e69  _id(self, immuni
-000064e0: 7a61 7469 6f6e 3d4e 6f6e 6529 3a0a 2020  zation=None):.  
-000064f0: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
-00006500: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
-00006510: 2020 2020 2020 2020 2020 2069 6d6d 756e             immun
-00006520: 697a 6174 696f 6e20 3d20 7365 6c66 2e66  ization = self.f
-00006530: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
-00006540: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
-00006550: 7469 6f6e 2069 7320 4e6f 6e65 206f 7220  tion is None or 
-00006560: 696d 6d75 6e69 7a61 7469 6f6e 2e6d 6574  immunization.met
-00006570: 6120 6973 204e 6f6e 653a 0a20 2020 2020  a is None:.     
-00006580: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00006590: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
-000065a0: 6e20 696d 6d75 6e69 7a61 7469 6f6e 2e6d  n immunization.m
-000065b0: 6574 612e 7665 7273 696f 6e49 640a 0a20  eta.versionId.. 
-000065c0: 2020 2064 6566 2067 6574 5f6d 6574 615f     def get_meta_
-000065d0: 6c61 7374 5f75 7064 6174 6564 2873 656c  last_updated(sel
-000065e0: 662c 2069 6d6d 756e 697a 6174 696f 6e3d  f, immunization=
-000065f0: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
-00006600: 6620 696d 6d75 6e69 7a61 7469 6f6e 2069  f immunization i
-00006610: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00006620: 2020 2020 696d 6d75 6e69 7a61 7469 6f6e      immunization
-00006630: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
-00006640: 6f75 7263 650a 2020 2020 2020 2020 6966  ource.        if
-00006650: 2069 6d6d 756e 697a 6174 696f 6e20 6973   immunization is
-00006660: 204e 6f6e 6520 6f72 2069 6d6d 756e 697a   None or immuniz
-00006670: 6174 696f 6e2e 6d65 7461 2069 7320 4e6f  ation.meta is No
-00006680: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00006690: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-000066a0: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
-000066b0: 696f 6e2e 6d65 7461 2e6c 6173 7455 7064  ion.meta.lastUpd
-000066c0: 6174 6564 2069 7320 6e6f 7420 4e6f 6e65  ated is not None
-000066d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000066e0: 7475 726e 2069 6d6d 756e 697a 6174 696f  turn immunizatio
-000066f0: 6e2e 6d65 7461 2e6c 6173 7455 7064 6174  n.meta.lastUpdat
-00006700: 6564 2e69 736f 7374 7269 6e67 0a20 2020  ed.isostring.   
-00006710: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00006720: 2020 2020 2020 2072 6574 7572 6e20 696d         return im
-00006730: 6d75 6e69 7a61 7469 6f6e 2e6d 6574 612e  munization.meta.
-00006740: 6c61 7374 5570 6461 7465 640a 0a20 2020  lastUpdated..   
-00006750: 2064 6566 2067 6574 5f6d 6574 615f 7072   def get_meta_pr
-00006760: 6f66 696c 6528 7365 6c66 2c20 696d 6d75  ofile(self, immu
-00006770: 6e69 7a61 7469 6f6e 3d4e 6f6e 6529 3a0a  nization=None):.
-00006780: 2020 2020 2020 2020 6966 2069 6d6d 756e          if immun
-00006790: 697a 6174 696f 6e20 6973 204e 6f6e 653a  ization is None:
-000067a0: 0a20 2020 2020 2020 2020 2020 2069 6d6d  .            imm
-000067b0: 756e 697a 6174 696f 6e20 3d20 7365 6c66  unization = self
-000067c0: 2e66 6869 725f 7265 736f 7572 6365 0a20  .fhir_resource. 
-000067d0: 2020 2020 2020 2069 6620 696d 6d75 6e69         if immuni
-000067e0: 7a61 7469 6f6e 2069 7320 4e6f 6e65 206f  zation is None o
-000067f0: 7220 696d 6d75 6e69 7a61 7469 6f6e 2e6d  r immunization.m
-00006800: 6574 6120 6973 204e 6f6e 653a 0a20 2020  eta is None:.   
-00006810: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00006820: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
-00006830: 7572 6e20 696d 6d75 6e69 7a61 7469 6f6e  urn immunization
-00006840: 2e6d 6574 612e 7072 6f66 696c 650a 0a20  .meta.profile.. 
-00006850: 2020 2064 6566 2073 6574 5f6d 6574 6128     def set_meta(
-00006860: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
-00006870: 6f6e 3d4e 6f6e 652c 2076 6572 7369 6f6e  on=None, version
-00006880: 5f69 643d 4e6f 6e65 2c20 6c61 7374 5f75  _id=None, last_u
-00006890: 7064 6174 6564 3d4e 6f6e 652c 2070 726f  pdated=None, pro
-000068a0: 6669 6c65 3d4e 6f6e 652c 2075 7064 6174  file=None, updat
-000068b0: 6564 5f62 793d 4e6f 6e65 2c20 6372 6561  ed_by=None, crea
-000068c0: 7469 6f6e 5f64 6174 653d 4e6f 6e65 2c20  tion_date=None, 
-000068d0: 6372 6561 7465 645f 6279 3d4e 6f6e 6529  created_by=None)
-000068e0: 3a0a 2020 2020 2020 2020 6966 2069 6d6d  :.        if imm
-000068f0: 756e 697a 6174 696f 6e20 6973 204e 6f6e  unization is Non
-00006900: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00006910: 6d6d 756e 697a 6174 696f 6e20 3d20 7365  mmunization = se
-00006920: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
-00006930: 0a20 2020 2020 2020 2069 6620 7665 7273  .        if vers
-00006940: 696f 6e5f 6964 2069 7320 6e6f 7420 4e6f  ion_id is not No
-00006950: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00006960: 7365 6c66 2e76 6572 7369 6f6e 5f69 6420  self.version_id 
-00006970: 3d20 7665 7273 696f 6e5f 6964 0a20 2020  = version_id.   
-00006980: 2020 2020 2069 6620 6c61 7374 5f75 7064       if last_upd
-00006990: 6174 6564 2069 7320 6e6f 7420 4e6f 6e65  ated is not None
-000069a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000069b0: 6c66 2e6c 6173 745f 7570 6461 7465 6420  lf.last_updated 
-000069c0: 3d20 6c61 7374 5f75 7064 6174 6564 0a20  = last_updated. 
-000069d0: 2020 2020 2020 2069 6620 7072 6f66 696c         if profil
-000069e0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-000069f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006a00: 7072 6f66 696c 6520 3d20 7072 6f66 696c  profile = profil
-00006a10: 650a 2020 2020 2020 2020 6966 2075 7064  e.        if upd
-00006a20: 6174 6564 5f62 7920 6973 206e 6f74 204e  ated_by is not N
-00006a30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00006a40: 2073 656c 662e 7570 6461 7465 645f 6279   self.updated_by
-00006a50: 203d 2075 7064 6174 6564 5f62 790a 2020   = updated_by.  
-00006a60: 2020 2020 2020 6966 2063 7265 6174 696f        if creatio
-00006a70: 6e5f 6461 7465 2069 7320 6e6f 7420 4e6f  n_date is not No
-00006a80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00006a90: 7365 6c66 2e63 7265 6174 696f 6e5f 6461  self.creation_da
-00006aa0: 7465 203d 2063 7265 6174 696f 6e5f 6461  te = creation_da
-00006ab0: 7465 0a20 2020 2020 2020 2069 6620 6372  te.        if cr
-00006ac0: 6561 7465 645f 6279 2069 7320 6e6f 7420  eated_by is not 
-00006ad0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006ae0: 2020 7365 6c66 2e63 7265 6174 6564 5f62    self.created_b
-00006af0: 7920 3d20 6372 6561 7465 645f 6279 0a20  y = created_by. 
-00006b00: 2020 2020 2020 2069 6620 696d 6d75 6e69         if immuni
-00006b10: 7a61 7469 6f6e 2e6d 6574 6120 6973 204e  zation.meta is N
-00006b20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00006b30: 2069 6d6d 756e 697a 6174 696f 6e2e 6d65   immunization.me
-00006b40: 7461 203d 204d 6574 6128 290a 2020 2020  ta = Meta().    
-00006b50: 2020 2020 696d 6d75 6e69 7a61 7469 6f6e      immunization
-00006b60: 2e6d 6574 612e 7665 7273 696f 6e49 6420  .meta.versionId 
-00006b70: 3d20 7365 6c66 2e76 6572 7369 6f6e 5f69  = self.version_i
-00006b80: 640a 2020 2020 2020 2020 696d 6d75 6e69  d.        immuni
-00006b90: 7a61 7469 6f6e 2e6d 6574 612e 6c61 7374  zation.meta.last
-00006ba0: 5570 6461 7465 6420 3d20 7365 6c66 2e6c  Updated = self.l
-00006bb0: 6173 745f 7570 6461 7465 640a 2020 2020  ast_updated.    
-00006bc0: 2020 2020 696d 6d75 6e69 7a61 7469 6f6e      immunization
-00006bd0: 2e6d 6574 612e 7072 6f66 696c 6520 3d20  .meta.profile = 
-00006be0: 7365 6c66 2e70 726f 6669 6c65 0a20 2020  self.profile.   
-00006bf0: 2020 2020 2069 6620 7365 6c66 2e75 7064       if self.upd
-00006c00: 6174 6564 5f62 7920 6973 206e 6f74 204e  ated_by is not N
-00006c10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00006c20: 2075 7064 6174 6564 5f62 795f 6578 7420   updated_by_ext 
-00006c30: 3d20 4578 7465 6e73 696f 6e28 290a 2020  = Extension().  
-00006c40: 2020 2020 2020 2020 2020 7570 6461 7465            update
-00006c50: 645f 6279 5f65 7874 2e75 726c 203d 2073  d_by_ext.url = s
-00006c60: 656c 662e 7570 6461 7465 645f 6279 5f75  elf.updated_by_u
-00006c70: 726c 0a20 2020 2020 2020 2020 2020 2075  rl.            u
-00006c80: 7064 6174 6564 5f62 795f 6578 742e 7661  pdated_by_ext.va
-00006c90: 6c75 6553 7472 696e 6720 3d20 7365 6c66  lueString = self
-00006ca0: 2e75 7064 6174 6564 5f62 790a 2020 2020  .updated_by.    
-00006cb0: 2020 2020 2020 2020 696d 6d75 6e69 7a61          immuniza
-00006cc0: 7469 6f6e 2e6d 6574 612e 6578 7465 6e73  tion.meta.extens
-00006cd0: 696f 6e20 3d20 7375 7065 7228 292e 6164  ion = super().ad
-00006ce0: 645f 6f72 5f75 7064 6174 655f 6578 7465  d_or_update_exte
-00006cf0: 6e73 696f 6e5f 746f 5f65 7874 656e 7369  nsion_to_extensi
-00006d00: 6f6e 7328 6578 7465 6e73 696f 6e3d 7570  ons(extension=up
-00006d10: 6461 7465 645f 6279 5f65 7874 2c20 6578  dated_by_ext, ex
-00006d20: 7465 6e73 696f 6e73 3d69 6d6d 756e 697a  tensions=immuniz
-00006d30: 6174 696f 6e2e 6d65 7461 2e65 7874 656e  ation.meta.exten
-00006d40: 7369 6f6e 290a 2020 2020 2020 2020 6966  sion).        if
-00006d50: 2073 656c 662e 6372 6561 7469 6f6e 5f64   self.creation_d
-00006d60: 6174 6520 6973 206e 6f74 204e 6f6e 6520  ate is not None 
-00006d70: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
-00006d80: 2020 7479 7065 2873 656c 662e 6372 6561    type(self.crea
-00006d90: 7469 6f6e 5f64 6174 6529 2069 7320 6461  tion_date) is da
-00006da0: 7465 206f 720a 2020 2020 2020 2020 2020  te or.          
-00006db0: 2020 7479 7065 2873 656c 662e 6372 6561    type(self.crea
-00006dc0: 7469 6f6e 5f64 6174 6529 2069 7320 4648  tion_date) is FH
-00006dd0: 4952 4461 7465 206f 7220 0a20 2020 2020  IRDate or .     
-00006de0: 2020 2020 2020 2074 7970 6528 7365 6c66         type(self
-00006df0: 2e63 7265 6174 696f 6e5f 6461 7465 2920  .creation_date) 
-00006e00: 6973 2073 7472 293a 0a0a 2020 2020 2020  is str):..      
-00006e10: 2020 2020 2020 6372 6561 7469 6f6e 5f64        creation_d
-00006e20: 6174 655f 6578 7420 3d20 4578 7465 6e73  ate_ext = Extens
-00006e30: 696f 6e28 290a 2020 2020 2020 2020 2020  ion().          
-00006e40: 2020 6372 6561 7469 6f6e 5f64 6174 655f    creation_date_
-00006e50: 6578 742e 7572 6c20 3d20 7365 6c66 2e63  ext.url = self.c
-00006e60: 7265 6174 696f 6e5f 6461 7465 5f75 726c  reation_date_url
-00006e70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00006e80: 7479 7065 2873 656c 662e 6372 6561 7469  type(self.creati
-00006e90: 6f6e 5f64 6174 6529 2069 7320 7374 723a  on_date) is str:
-00006ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006eb0: 2063 7265 6174 696f 6e5f 6461 7465 5f65   creation_date_e
-00006ec0: 7874 2e76 616c 7565 4461 7465 203d 2064  xt.valueDate = d
-00006ed0: 6174 6574 696d 652e 7374 7266 7469 6d65  atetime.strftime
-00006ee0: 2873 656c 662e 6372 6561 7469 6f6e 5f64  (self.creation_d
-00006ef0: 6174 652c 2022 2559 2d25 6d2d 2564 5425  ate, "%Y-%m-%dT%
-00006f00: 483a 254d 3a25 5325 7a22 290a 2020 2020  H:%M:%S%z").    
-00006f10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00006f20: 2020 2020 2020 2020 2020 2020 2020 6372                cr
-00006f30: 6561 7469 6f6e 5f64 6174 655f 6578 742e  eation_date_ext.
-00006f40: 7661 6c75 6544 6174 6520 3d20 7365 6c66  valueDate = self
-00006f50: 2e63 7265 6174 696f 6e5f 6461 7465 0a20  .creation_date. 
-00006f60: 2020 2020 2020 2020 2020 2069 6d6d 756e             immun
-00006f70: 697a 6174 696f 6e2e 6d65 7461 2e65 7874  ization.meta.ext
-00006f80: 656e 7369 6f6e 203d 2073 7570 6572 2829  ension = super()
-00006f90: 2e61 6464 5f6f 725f 7570 6461 7465 5f65  .add_or_update_e
-00006fa0: 7874 656e 7369 6f6e 5f74 6f5f 6578 7465  xtension_to_exte
-00006fb0: 6e73 696f 6e73 2865 7874 656e 7369 6f6e  nsions(extension
-00006fc0: 3d63 7265 6174 696f 6e5f 6461 7465 5f65  =creation_date_e
-00006fd0: 7874 2c20 6578 7465 6e73 696f 6e73 3d69  xt, extensions=i
-00006fe0: 6d6d 756e 697a 6174 696f 6e2e 6d65 7461  mmunization.meta
-00006ff0: 2e65 7874 656e 7369 6f6e 290a 2020 2020  .extension).    
-00007000: 2020 2020 6966 2073 656c 662e 6372 6561      if self.crea
-00007010: 7465 645f 6279 2069 7320 6e6f 7420 4e6f  ted_by is not No
-00007020: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00007030: 6372 6561 7465 645f 6279 5f65 7874 203d  created_by_ext =
-00007040: 2045 7874 656e 7369 6f6e 2829 0a20 2020   Extension().   
-00007050: 2020 2020 2020 2020 2063 7265 6174 6564           created
-00007060: 5f62 795f 6578 742e 7572 6c20 3d20 7365  _by_ext.url = se
-00007070: 6c66 2e63 7265 6174 6564 5f62 795f 7572  lf.created_by_ur
-00007080: 6c0a 2020 2020 2020 2020 2020 2020 6372  l.            cr
-00007090: 6561 7465 645f 6279 5f65 7874 2e76 616c  eated_by_ext.val
-000070a0: 7565 5374 7269 6e67 203d 2073 656c 662e  ueString = self.
-000070b0: 6372 6561 7465 645f 6279 0a20 2020 2020  created_by.     
-000070c0: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
-000070d0: 696f 6e2e 6d65 7461 2e65 7874 656e 7369  ion.meta.extensi
-000070e0: 6f6e 203d 2073 7570 6572 2829 2e61 6464  on = super().add
-000070f0: 5f6f 725f 7570 6461 7465 5f65 7874 656e  _or_update_exten
-00007100: 7369 6f6e 5f74 6f5f 6578 7465 6e73 696f  sion_to_extensio
-00007110: 6e73 2865 7874 656e 7369 6f6e 3d63 7265  ns(extension=cre
-00007120: 6174 6564 5f62 795f 6578 742c 2065 7874  ated_by_ext, ext
-00007130: 656e 7369 6f6e 733d 696d 6d75 6e69 7a61  ensions=immuniza
-00007140: 7469 6f6e 2e6d 6574 612e 6578 7465 6e73  tion.meta.extens
-00007150: 696f 6e29 0a0a 2020 2020 6465 6620 6765  ion)..    def ge
-00007160: 745f 6f76 6572 7269 6465 5f73 7461 7475  t_override_statu
-00007170: 7328 7365 6c66 2c20 696d 6d75 6e69 7a61  s(self, immuniza
-00007180: 7469 6f6e 3d4e 6f6e 6529 3a0a 2020 2020  tion=None):.    
-00007190: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
-000071a0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-000071b0: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
-000071c0: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
-000071d0: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
-000071e0: 2020 206f 7665 7272 6964 655f 7374 6174     override_stat
-000071f0: 7573 5f65 7874 656e 7369 6f6e 203d 204e  us_extension = N
-00007200: 6f6e 650a 2020 2020 2020 2020 6966 2069  one.        if i
-00007210: 6d6d 756e 697a 6174 696f 6e2e 6578 7465  mmunization.exte
-00007220: 6e73 696f 6e20 6973 206e 6f74 204e 6f6e  nsion is not Non
-00007230: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-00007240: 6f72 2065 7874 2069 6e20 696d 6d75 6e69  or ext in immuni
-00007250: 7a61 7469 6f6e 2e65 7874 656e 7369 6f6e  zation.extension
-00007260: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007270: 2020 6966 2065 7874 2e75 726c 203d 3d20    if ext.url == 
-00007280: 7365 6c66 2e6f 7665 7272 6964 655f 7374  self.override_st
-00007290: 6174 7573 5f75 726c 3a0a 2020 2020 2020  atus_url:.      
-000072a0: 2020 2020 2020 2020 2020 2020 2020 6f76                ov
-000072b0: 6572 7269 6465 5f73 7461 7475 735f 6578  erride_status_ex
-000072c0: 7465 6e73 696f 6e20 3d20 6578 740a 2020  tension = ext.  
-000072d0: 2020 2020 2020 7265 7475 726e 206f 7665        return ove
-000072e0: 7272 6964 655f 7374 6174 7573 5f65 7874  rride_status_ext
-000072f0: 656e 7369 6f6e 0a0a 2020 2020 6465 6620  ension..    def 
-00007300: 7365 745f 6f76 6572 7269 6465 5f73 7461  set_override_sta
-00007310: 7475 7328 7365 6c66 2c20 696d 6d75 6e69  tus(self, immuni
-00007320: 7a61 7469 6f6e 3d4e 6f6e 652c 2073 7461  zation=None, sta
-00007330: 7475 735f 636f 6465 3d4e 6f6e 652c 2073  tus_code=None, s
-00007340: 7461 7475 735f 6469 7370 6c61 793d 4e6f  tatus_display=No
-00007350: 6e65 2c20 7374 6174 7573 5f69 643d 4e6f  ne, status_id=No
-00007360: 6e65 2c20 636f 6469 6e67 5f73 7973 7465  ne, coding_syste
-00007370: 6d3d 4e6f 6e65 2c20 636f 6469 6e67 5f76  m=None, coding_v
-00007380: 6572 7369 6f6e 3d4e 6f6e 6529 3a0a 2020  ersion=None):.  
-00007390: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
-000073a0: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
-000073b0: 2020 2020 2020 2020 2020 2069 6d6d 756e             immun
-000073c0: 697a 6174 696f 6e20 3d20 7365 6c66 2e66  ization = self.f
-000073d0: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
-000073e0: 2020 2020 2069 6620 7374 6174 7573 5f63       if status_c
-000073f0: 6f64 6520 6973 206e 6f74 204e 6f6e 6520  ode is not None 
-00007400: 616e 6420 7374 6174 7573 5f64 6973 706c  and status_displ
-00007410: 6179 2069 7320 6e6f 7420 4e6f 6e65 2061  ay is not None a
-00007420: 6e64 2073 7461 7475 735f 6964 2069 7320  nd status_id is 
-00007430: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00007440: 2020 2020 2020 7365 6c66 2e6f 7665 7272        self.overr
-00007450: 6964 655f 7374 6174 7573 5f63 6f64 6520  ide_status_code 
-00007460: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
-00007470: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
-00007480: 7665 7272 6964 655f 7374 6174 7573 5f64  verride_status_d
-00007490: 6973 706c 6179 203d 2073 7461 7475 735f  isplay = status_
-000074a0: 6469 7370 6c61 790a 2020 2020 2020 2020  display.        
-000074b0: 2020 2020 7365 6c66 2e6f 7665 7272 6964      self.overrid
-000074c0: 655f 7374 6174 7573 5f69 6420 3d20 7374  e_status_id = st
-000074d0: 6174 7573 5f69 640a 2020 2020 2020 2020  atus_id.        
-000074e0: 7374 6174 7573 5f63 6f64 6561 626c 655f  status_codeable_
-000074f0: 636f 6e63 6570 7420 3d20 7365 6c66 2e74  concept = self.t
-00007500: 6f5f 636f 6465 6162 6c65 5f63 6f6e 6365  o_codeable_conce
-00007510: 7074 280a 2020 2020 2020 2020 2020 2020  pt(.            
-00007520: 636f 6465 3d73 656c 662e 6f76 6572 7269  code=self.overri
-00007530: 6465 5f73 7461 7475 735f 636f 6465 2c0a  de_status_code,.
-00007540: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-00007550: 6c61 793d 7365 6c66 2e6f 7665 7272 6964  lay=self.overrid
-00007560: 655f 7374 6174 7573 5f64 6973 706c 6179  e_status_display
-00007570: 2c0a 2020 2020 2020 2020 2020 2020 6964  ,.            id
-00007580: 3d73 656c 662e 6f76 6572 7269 6465 5f73  =self.override_s
-00007590: 7461 7475 735f 6964 2c0a 2020 2020 2020  tatus_id,.      
-000075a0: 2020 2020 2020 636f 6469 6e67 5f73 7973        coding_sys
-000075b0: 7465 6d3d 636f 6469 6e67 5f73 7973 7465  tem=coding_syste
-000075c0: 6d2c 0a20 2020 2020 2020 2020 2020 2063  m,.            c
-000075d0: 6f64 696e 675f 7665 7273 696f 6e3d 636f  oding_version=co
-000075e0: 6469 6e67 5f76 6572 7369 6f6e 290a 2020  ding_version).  
-000075f0: 2020 2020 2020 6e65 775f 6578 7420 3d20        new_ext = 
-00007600: 4578 7465 6e73 696f 6e28 290a 2020 2020  Extension().    
-00007610: 2020 2020 6e65 775f 6578 742e 7572 6c20      new_ext.url 
-00007620: 3d20 7365 6c66 2e6f 7665 7272 6964 655f  = self.override_
-00007630: 7374 6174 7573 5f75 726c 0a20 2020 2020  status_url.     
-00007640: 2020 206e 6577 5f65 7874 2e76 616c 7565     new_ext.value
-00007650: 436f 6465 6162 6c65 436f 6e63 6570 7420  CodeableConcept 
-00007660: 3d20 7374 6174 7573 5f63 6f64 6561 626c  = status_codeabl
-00007670: 655f 636f 6e63 6570 740a 2020 2020 2020  e_concept.      
-00007680: 2020 696d 6d75 6e69 7a61 7469 6f6e 2e65    immunization.e
-00007690: 7874 656e 7369 6f6e 203d 2073 7570 6572  xtension = super
-000076a0: 2829 2e61 6464 5f6f 725f 7570 6461 7465  ().add_or_update
-000076b0: 5f65 7874 656e 7369 6f6e 5f74 6f5f 6578  _extension_to_ex
-000076c0: 7465 6e73 696f 6e73 2865 7874 656e 7369  tensions(extensi
-000076d0: 6f6e 3d6e 6577 5f65 7874 2c20 6578 7465  on=new_ext, exte
-000076e0: 6e73 696f 6e73 3d69 6d6d 756e 697a 6174  nsions=immunizat
-000076f0: 696f 6e2e 6578 7465 6e73 696f 6e29 0a0a  ion.extension)..
-00007700: 2020 2020 6465 6620 7365 745f 616e 7469      def set_anti
-00007710: 6765 6e5f 7374 6174 7573 280a 2020 2020  gen_status(.    
-00007720: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00007730: 2020 696d 6d75 6e69 7a61 7469 6f6e 3d4e    immunization=N
-00007740: 6f6e 652c 0a20 2020 2020 2020 2061 6e74  one,.        ant
-00007750: 6967 656e 5f63 6f64 653d 4e6f 6e65 2c0a  igen_code=None,.
-00007760: 2020 2020 2020 2020 616e 7469 6765 6e5f          antigen_
-00007770: 6964 3d4e 6f6e 652c 0a20 2020 2020 2020  id=None,.       
-00007780: 2061 6e74 6967 656e 5f64 6973 706c 6179   antigen_display
-00007790: 3d4e 6f6e 652c 0a20 2020 2020 2020 2064  =None,.        d
-000077a0: 6f73 655f 6e75 6d62 6572 3d4e 6f6e 652c  ose_number=None,
-000077b0: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
-000077c0: 636f 6465 3d4e 6f6e 652c 0a20 2020 2020  code=None,.     
-000077d0: 2020 2073 7461 7475 735f 6964 3d4e 6f6e     status_id=Non
-000077e0: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
-000077f0: 735f 6469 7370 6c61 793d 4e6f 6e65 2c0a  s_display=None,.
-00007800: 2020 2020 2020 2020 636f 6469 6e67 5f73          coding_s
-00007810: 7973 7465 6d3d 4e6f 6e65 2c0a 2020 2020  ystem=None,.    
-00007820: 2020 2020 636f 6469 6e67 5f76 6572 7369      coding_versi
-00007830: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
-00007840: 2020 6966 2069 6d6d 756e 697a 6174 696f    if immunizatio
-00007850: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-00007860: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
-00007870: 696f 6e20 3d20 7365 6c66 2e66 6869 725f  ion = self.fhir_
-00007880: 7265 736f 7572 6365 0a0a 2020 2020 2020  resource..      
-00007890: 2020 616e 7469 6765 6e5f 7374 6174 7573    antigen_status
-000078a0: 5f65 7874 203d 2045 7874 656e 7369 6f6e  _ext = Extension
-000078b0: 2829 0a20 2020 2020 2020 2061 6e74 6967  ().        antig
-000078c0: 656e 5f73 7461 7475 735f 6578 742e 7572  en_status_ext.ur
-000078d0: 6c20 3d20 7365 6c66 2e61 6e74 6967 656e  l = self.antigen
-000078e0: 5f73 7461 7475 735f 7572 6c0a 0a20 2020  _status_url..   
-000078f0: 2020 2020 2069 6620 616e 7469 6765 6e5f       if antigen_
-00007900: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-00007910: 2061 6e64 2061 6e74 6967 656e 5f69 6420   and antigen_id 
-00007920: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-00007930: 616e 7469 6765 6e5f 6469 7370 6c61 7920  antigen_display 
-00007940: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00007950: 2020 2020 2020 2020 2073 656c 662e 616e           self.an
-00007960: 7469 6765 6e5f 6469 7370 6c61 7920 3d20  tigen_display = 
-00007970: 616e 7469 6765 6e5f 6469 7370 6c61 790a  antigen_display.
-00007980: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007990: 2e61 6e74 6967 656e 5f63 6f64 6520 3d20  .antigen_code = 
-000079a0: 616e 7469 6765 6e5f 636f 6465 0a20 2020  antigen_code.   
-000079b0: 2020 2020 2020 2020 2073 656c 662e 616e           self.an
-000079c0: 7469 6765 6e5f 6964 203d 2061 6e74 6967  tigen_id = antig
-000079d0: 656e 5f69 640a 2020 2020 2020 2020 616e  en_id.        an
-000079e0: 7469 6765 6e5f 636f 6465 6162 6c65 5f63  tigen_codeable_c
-000079f0: 6f6e 6365 7074 203d 2073 656c 662e 746f  oncept = self.to
-00007a00: 5f63 6f64 6561 626c 655f 636f 6e63 6570  _codeable_concep
-00007a10: 7428 0a20 2020 2020 2020 2020 2020 2063  t(.            c
-00007a20: 6f64 653d 7365 6c66 2e61 6e74 6967 656e  ode=self.antigen
-00007a30: 5f63 6f64 652c 0a20 2020 2020 2020 2020  _code,.         
-00007a40: 2020 2064 6973 706c 6179 3d73 656c 662e     display=self.
-00007a50: 616e 7469 6765 6e5f 6469 7370 6c61 792c  antigen_display,
-00007a60: 0a20 2020 2020 2020 2020 2020 2069 643d  .            id=
-00007a70: 7365 6c66 2e61 6e74 6967 656e 5f69 642c  self.antigen_id,
-00007a80: 0a20 2020 2020 2020 2020 2020 2063 6f64  .            cod
-00007a90: 696e 675f 7379 7374 656d 3d63 6f64 696e  ing_system=codin
-00007aa0: 675f 7379 7374 656d 2c0a 2020 2020 2020  g_system,.      
-00007ab0: 2020 2020 2020 636f 6469 6e67 5f76 6572        coding_ver
-00007ac0: 7369 6f6e 3d63 6f64 696e 675f 7665 7273  sion=coding_vers
-00007ad0: 696f 6e29 0a20 2020 2020 2020 2061 6e74  ion).        ant
-00007ae0: 6967 656e 5f65 7874 203d 2045 7874 656e  igen_ext = Exten
-00007af0: 7369 6f6e 2829 0a20 2020 2020 2020 2061  sion().        a
-00007b00: 6e74 6967 656e 5f65 7874 2e75 726c 203d  ntigen_ext.url =
-00007b10: 2027 616e 7469 6765 6e27 0a20 2020 2020   'antigen'.     
-00007b20: 2020 2061 6e74 6967 656e 5f65 7874 2e76     antigen_ext.v
-00007b30: 616c 7565 436f 6465 6162 6c65 436f 6e63  alueCodeableConc
-00007b40: 6570 7420 3d20 616e 7469 6765 6e5f 636f  ept = antigen_co
-00007b50: 6465 6162 6c65 5f63 6f6e 6365 7074 0a20  deable_concept. 
-00007b60: 2020 2020 2020 2061 6e74 6967 656e 5f73         antigen_s
-00007b70: 7461 7475 735f 6578 742e 6578 7465 6e73  tatus_ext.extens
-00007b80: 696f 6e20 3d20 7375 7065 7228 292e 6164  ion = super().ad
-00007b90: 645f 6f72 5f75 7064 6174 655f 6578 7465  d_or_update_exte
-00007ba0: 6e73 696f 6e5f 746f 5f65 7874 656e 7369  nsion_to_extensi
-00007bb0: 6f6e 7328 6578 7465 6e73 696f 6e3d 616e  ons(extension=an
-00007bc0: 7469 6765 6e5f 6578 742c 2065 7874 656e  tigen_ext, exten
-00007bd0: 7369 6f6e 733d 616e 7469 6765 6e5f 7374  sions=antigen_st
-00007be0: 6174 7573 5f65 7874 2e65 7874 656e 7369  atus_ext.extensi
-00007bf0: 6f6e 290a 0a20 2020 2020 2020 2069 6620  on)..        if 
-00007c00: 646f 7365 5f6e 756d 6265 7220 6973 206e  dose_number is n
-00007c10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00007c20: 2020 2020 2073 656c 662e 616e 7469 6765       self.antige
-00007c30: 6e5f 646f 7365 5f6e 756d 6265 7220 3d20  n_dose_number = 
-00007c40: 646f 7365 5f6e 756d 6265 720a 2020 2020  dose_number.    
-00007c50: 2020 2020 646f 7365 5f6e 756d 6265 725f      dose_number_
-00007c60: 6578 7420 3d20 4578 7465 6e73 696f 6e28  ext = Extension(
-00007c70: 290a 2020 2020 2020 2020 646f 7365 5f6e  ).        dose_n
-00007c80: 756d 6265 725f 6578 742e 7572 6c20 3d20  umber_ext.url = 
-00007c90: 2764 6f73 654e 756d 6265 7227 0a20 2020  'doseNumber'.   
-00007ca0: 2020 2020 2064 6f73 655f 6e75 6d62 6572       dose_number
-00007cb0: 5f65 7874 2e76 616c 7565 496e 7465 6765  _ext.valueIntege
-00007cc0: 7220 3d20 7365 6c66 2e61 6e74 6967 656e  r = self.antigen
-00007cd0: 5f64 6f73 655f 6e75 6d62 6572 0a20 2020  _dose_number.   
-00007ce0: 2020 2020 2061 6e74 6967 656e 5f73 7461       antigen_sta
-00007cf0: 7475 735f 6578 742e 6578 7465 6e73 696f  tus_ext.extensio
-00007d00: 6e20 3d20 7375 7065 7228 292e 6164 645f  n = super().add_
-00007d10: 6f72 5f75 7064 6174 655f 6578 7465 6e73  or_update_extens
-00007d20: 696f 6e5f 746f 5f65 7874 656e 7369 6f6e  ion_to_extension
-00007d30: 7328 6578 7465 6e73 696f 6e3d 646f 7365  s(extension=dose
-00007d40: 5f6e 756d 6265 725f 6578 742c 2065 7874  _number_ext, ext
-00007d50: 656e 7369 6f6e 733d 616e 7469 6765 6e5f  ensions=antigen_
-00007d60: 7374 6174 7573 5f65 7874 2e65 7874 656e  status_ext.exten
-00007d70: 7369 6f6e 290a 0a20 2020 2020 2020 2069  sion)..        i
-00007d80: 6620 7374 6174 7573 5f63 6f64 6520 6973  f status_code is
-00007d90: 206e 6f74 204e 6f6e 6520 616e 6420 7374   not None and st
-00007da0: 6174 7573 5f69 6420 6973 206e 6f74 204e  atus_id is not N
-00007db0: 6f6e 6520 616e 6420 7374 6174 7573 5f64  one and status_d
-00007dc0: 6973 706c 6179 2069 7320 6e6f 7420 4e6f  isplay is not No
-00007dd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00007de0: 7365 6c66 2e61 6e74 6967 656e 5f73 7461  self.antigen_sta
-00007df0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
-00007e00: 735f 636f 6465 0a20 2020 2020 2020 2020  s_code.         
-00007e10: 2020 2073 656c 662e 616e 7469 6765 6e5f     self.antigen_
-00007e20: 7374 6174 7573 5f64 6973 706c 6179 203d  status_display =
-00007e30: 2073 7461 7475 735f 6469 7370 6c61 790a   status_display.
-00007e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007e50: 2e61 6e74 6967 656e 5f73 7461 7475 735f  .antigen_status_
-00007e60: 6964 203d 2073 7461 7475 735f 6964 0a20  id = status_id. 
-00007e70: 2020 2020 2020 2073 7461 7475 735f 636f         status_co
-00007e80: 6465 6162 6c65 5f63 6f6e 6365 7074 203d  deable_concept =
-00007e90: 2073 656c 662e 746f 5f63 6f64 6561 626c   self.to_codeabl
-00007ea0: 655f 636f 6e63 6570 7428 0a20 2020 2020  e_concept(.     
-00007eb0: 2020 2020 2020 2063 6f64 6520 3d20 7365         code = se
-00007ec0: 6c66 2e61 6e74 6967 656e 5f73 7461 7475  lf.antigen_statu
-00007ed0: 735f 636f 6465 2c0a 2020 2020 2020 2020  s_code,.        
-00007ee0: 2020 2020 6964 203d 2073 656c 662e 616e      id = self.an
-00007ef0: 7469 6765 6e5f 7374 6174 7573 5f69 642c  tigen_status_id,
-00007f00: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00007f10: 706c 6179 3d73 656c 662e 616e 7469 6765  play=self.antige
-00007f20: 6e5f 7374 6174 7573 5f64 6973 706c 6179  n_status_display
-00007f30: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
-00007f40: 6469 6e67 5f73 7973 7465 6d3d 636f 6469  ding_system=codi
-00007f50: 6e67 5f73 7973 7465 6d2c 0a20 2020 2020  ng_system,.     
-00007f60: 2020 2020 2020 2063 6f64 696e 675f 7665         coding_ve
-00007f70: 7273 696f 6e3d 636f 6469 6e67 5f76 6572  rsion=coding_ver
-00007f80: 7369 6f6e 0a20 2020 2020 2020 2029 0a20  sion.        ). 
-00007f90: 2020 2020 2020 2073 7461 7475 735f 6578         status_ex
-00007fa0: 7420 3d20 4578 7465 6e73 696f 6e28 290a  t = Extension().
-00007fb0: 2020 2020 2020 2020 7374 6174 7573 5f65          status_e
-00007fc0: 7874 2e75 726c 203d 2027 7374 6174 7573  xt.url = 'status
-00007fd0: 270a 2020 2020 2020 2020 7374 6174 7573  '.        status
-00007fe0: 5f65 7874 2e76 616c 7565 436f 6465 6162  _ext.valueCodeab
-00007ff0: 6c65 436f 6e63 6570 7420 3d20 7374 6174  leConcept = stat
-00008000: 7573 5f63 6f64 6561 626c 655f 636f 6e63  us_codeable_conc
-00008010: 6570 740a 2020 2020 2020 2020 616e 7469  ept.        anti
-00008020: 6765 6e5f 7374 6174 7573 5f65 7874 2e65  gen_status_ext.e
-00008030: 7874 656e 7369 6f6e 203d 2073 7570 6572  xtension = super
-00008040: 2829 2e61 6464 5f6f 725f 7570 6461 7465  ().add_or_update
-00008050: 5f65 7874 656e 7369 6f6e 5f74 6f5f 6578  _extension_to_ex
-00008060: 7465 6e73 696f 6e73 2865 7874 656e 7369  tensions(extensi
-00008070: 6f6e 3d73 7461 7475 735f 6578 742c 2065  on=status_ext, e
-00008080: 7874 656e 7369 6f6e 733d 616e 7469 6765  xtensions=antige
-00008090: 6e5f 7374 6174 7573 5f65 7874 2e65 7874  n_status_ext.ext
-000080a0: 656e 7369 6f6e 290a 0a20 2020 2020 2020  ension)..       
-000080b0: 2069 6d6d 756e 697a 6174 696f 6e2e 6578   immunization.ex
-000080c0: 7465 6e73 696f 6e20 3d20 7375 7065 7228  tension = super(
-000080d0: 292e 6164 645f 6f72 5f75 7064 6174 655f  ).add_or_update_
-000080e0: 6578 7465 6e73 696f 6e5f 746f 5f65 7874  extension_to_ext
-000080f0: 656e 7369 6f6e 7328 6578 7465 6e73 696f  ensions(extensio
-00008100: 6e3d 616e 7469 6765 6e5f 7374 6174 7573  n=antigen_status
-00008110: 5f65 7874 2c20 6578 7465 6e73 696f 6e73  _ext, extensions
-00008120: 3d69 6d6d 756e 697a 6174 696f 6e2e 6578  =immunization.ex
-00008130: 7465 6e73 696f 6e29 0a0a 2020 2020 6465  tension)..    de
-00008140: 6620 6765 745f 616e 7469 6765 6e5f 7374  f get_antigen_st
-00008150: 6174 7573 2873 656c 662c 2069 6d6d 756e  atus(self, immun
-00008160: 697a 6174 696f 6e3d 4e6f 6e65 293a 0a20  ization=None):. 
-00008170: 2020 2020 2020 2069 6620 696d 6d75 6e69         if immuni
-00008180: 7a61 7469 6f6e 2069 7320 4e6f 6e65 3a0a  zation is None:.
-00008190: 2020 2020 2020 2020 2020 2020 696d 6d75              immu
-000081a0: 6e69 7a61 7469 6f6e 203d 2073 656c 662e  nization = self.
-000081b0: 6668 6972 5f72 6573 6f75 7263 650a 2020  fhir_resource.  
-000081c0: 2020 2020 2020 616e 7469 6765 6e5f 7374        antigen_st
-000081d0: 6174 7573 5f65 7874 656e 7369 6f6e 203d  atus_extension =
-000081e0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-000081f0: 2069 6d6d 756e 697a 6174 696f 6e2e 6578   immunization.ex
-00008200: 7465 6e73 696f 6e20 6973 206e 6f74 204e  tension is not N
-00008210: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00008220: 2066 6f72 2065 7874 2069 6e20 696d 6d75   for ext in immu
-00008230: 6e69 7a61 7469 6f6e 2e65 7874 656e 7369  nization.extensi
-00008240: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00008250: 2020 2020 6966 2065 7874 2e75 726c 203d      if ext.url =
-00008260: 3d20 7365 6c66 2e61 6e74 6967 656e 5f73  = self.antigen_s
-00008270: 7461 7475 735f 7572 6c3a 0a20 2020 2020  tatus_url:.     
-00008280: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00008290: 6e74 6967 656e 5f73 7461 7475 735f 6578  ntigen_status_ex
-000082a0: 7465 6e73 696f 6e20 3d20 6578 740a 2020  tension = ext.  
-000082b0: 2020 2020 2020 7265 7475 726e 2061 6e74        return ant
-000082c0: 6967 656e 5f73 7461 7475 735f 6578 7465  igen_status_exte
-000082d0: 6e73 696f 6e0a 0a20 2020 2064 6566 2067  nsion..    def g
-000082e0: 6574 5f61 6e74 6967 656e 5f73 7461 7475  et_antigen_statu
-000082f0: 735f 616e 7469 6765 6e28 7365 6c66 2c20  s_antigen(self, 
-00008300: 696d 6d75 6e69 7a61 7469 6f6e 3d4e 6f6e  immunization=Non
-00008310: 6529 3a0a 2020 2020 2020 2020 616e 7469  e):.        anti
-00008320: 6765 6e5f 7374 6174 7573 5f65 7874 656e  gen_status_exten
-00008330: 7369 6f6e 203d 2073 656c 662e 6765 745f  sion = self.get_
-00008340: 616e 7469 6765 6e5f 7374 6174 7573 2869  antigen_status(i
-00008350: 6d6d 756e 697a 6174 696f 6e3d 696d 6d75  mmunization=immu
-00008360: 6e69 7a61 7469 6f6e 290a 2020 2020 2020  nization).      
-00008370: 2020 616e 7469 6765 6e5f 6578 7465 6e73    antigen_extens
-00008380: 696f 6e20 3d20 4e6f 6e65 0a20 2020 2020  ion = None.     
-00008390: 2020 2069 6620 616e 7469 6765 6e5f 7374     if antigen_st
-000083a0: 6174 7573 5f65 7874 656e 7369 6f6e 2069  atus_extension i
-000083b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000083c0: 2020 2020 2020 2020 666f 7220 616e 7469          for anti
-000083d0: 6765 6e5f 6578 7465 6e73 696f 6e20 696e  gen_extension in
-000083e0: 2061 6e74 6967 656e 5f73 7461 7475 735f   antigen_status_
-000083f0: 6578 7465 6e73 696f 6e2e 6578 7465 6e73  extension.extens
-00008400: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-00008410: 2020 2020 2069 6620 616e 7469 6765 6e5f       if antigen_
-00008420: 6578 7465 6e73 696f 6e2e 7572 6c20 3d3d  extension.url ==
-00008430: 2027 616e 7469 6765 6e27 3a0a 2020 2020   'antigen':.    
-00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008450: 6272 6561 6b0a 2020 2020 2020 2020 7265  break.        re
-00008460: 7475 726e 2061 6e74 6967 656e 5f65 7874  turn antigen_ext
-00008470: 656e 7369 6f6e 0a0a 2020 2020 6465 6620  ension..    def 
-00008480: 6765 745f 616e 7469 6765 6e5f 7374 6174  get_antigen_stat
-00008490: 7573 5f64 6f73 655f 6e75 6d62 6572 2873  us_dose_number(s
-000084a0: 656c 662c 2069 6d6d 756e 697a 6174 696f  elf, immunizatio
-000084b0: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
-000084c0: 2061 6e74 6967 656e 5f73 7461 7475 735f   antigen_status_
-000084d0: 6578 7465 6e73 696f 6e20 3d20 7365 6c66  extension = self
-000084e0: 2e67 6574 5f61 6e74 6967 656e 5f73 7461  .get_antigen_sta
-000084f0: 7475 7328 696d 6d75 6e69 7a61 7469 6f6e  tus(immunization
-00008500: 3d69 6d6d 756e 697a 6174 696f 6e29 0a20  =immunization). 
-00008510: 2020 2020 2020 2061 6e74 6967 656e 5f65         antigen_e
-00008520: 7874 656e 7369 6f6e 203d 204e 6f6e 650a  xtension = None.
-00008530: 2020 2020 2020 2020 6966 2061 6e74 6967          if antig
-00008540: 656e 5f73 7461 7475 735f 6578 7465 6e73  en_status_extens
-00008550: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-00008560: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00008570: 2061 6e74 6967 656e 5f65 7874 656e 7369   antigen_extensi
-00008580: 6f6e 2069 6e20 616e 7469 6765 6e5f 7374  on in antigen_st
-00008590: 6174 7573 5f65 7874 656e 7369 6f6e 2e65  atus_extension.e
-000085a0: 7874 656e 7369 6f6e 3a0a 2020 2020 2020  xtension:.      
-000085b0: 2020 2020 2020 2020 2020 6966 2061 6e74            if ant
-000085c0: 6967 656e 5f65 7874 656e 7369 6f6e 2e75  igen_extension.u
-000085d0: 726c 203d 3d20 2764 6f73 654e 756d 6265  rl == 'doseNumbe
-000085e0: 7227 3a0a 2020 2020 2020 2020 2020 2020  r':.            
-000085f0: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
-00008600: 2020 2020 2020 7265 7475 726e 2061 6e74        return ant
-00008610: 6967 656e 5f65 7874 656e 7369 6f6e 0a0a  igen_extension..
-00008620: 2020 2020 6465 6620 6765 745f 616e 7469      def get_anti
-00008630: 6765 6e5f 7374 6174 7573 5f73 7461 7475  gen_status_statu
-00008640: 7328 7365 6c66 2c20 696d 6d75 6e69 7a61  s(self, immuniza
-00008650: 7469 6f6e 3d4e 6f6e 6529 3a0a 2020 2020  tion=None):.    
-00008660: 2020 2020 616e 7469 6765 6e5f 7374 6174      antigen_stat
-00008670: 7573 5f65 7874 656e 7369 6f6e 203d 2073  us_extension = s
-00008680: 656c 662e 6765 745f 616e 7469 6765 6e5f  elf.get_antigen_
-00008690: 7374 6174 7573 2869 6d6d 756e 697a 6174  status(immunizat
-000086a0: 696f 6e3d 696d 6d75 6e69 7a61 7469 6f6e  ion=immunization
-000086b0: 290a 2020 2020 2020 2020 616e 7469 6765  ).        antige
-000086c0: 6e5f 6578 7465 6e73 696f 6e20 3d20 4e6f  n_extension = No
-000086d0: 6e65 0a20 2020 2020 2020 2069 6620 616e  ne.        if an
-000086e0: 7469 6765 6e5f 7374 6174 7573 5f65 7874  tigen_status_ext
-000086f0: 656e 7369 6f6e 2069 7320 6e6f 7420 4e6f  ension is not No
-00008700: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00008710: 666f 7220 616e 7469 6765 6e5f 6578 7465  for antigen_exte
-00008720: 6e73 696f 6e20 696e 2061 6e74 6967 656e  nsion in antigen
-00008730: 5f73 7461 7475 735f 6578 7465 6e73 696f  _status_extensio
-00008740: 6e2e 6578 7465 6e73 696f 6e3a 0a20 2020  n.extension:.   
-00008750: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00008760: 616e 7469 6765 6e5f 6578 7465 6e73 696f  antigen_extensio
-00008770: 6e2e 7572 6c20 3d3d 2027 7374 6174 7573  n.url == 'status
-00008780: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00008790: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-000087a0: 2020 2020 2072 6574 7572 6e20 616e 7469       return anti
-000087b0: 6765 6e5f 6578 7465 6e73 696f 6e0a 0a20  gen_extension.. 
-000087c0: 2020 2064 6566 2067 6574 5f63 6f64 6561     def get_codea
-000087d0: 626c 655f 636f 6e63 6570 745f 636f 6469  ble_concept_codi
-000087e0: 6e67 2873 656c 662c 2063 6f64 6561 626c  ng(self, codeabl
-000087f0: 655f 636f 6e63 6570 743d 4e6f 6e65 2c20  e_concept=None, 
-00008800: 636f 6469 6e67 5f73 7973 7465 6d3d 4e6f  coding_system=No
-00008810: 6e65 2c20 636f 6469 6e67 5f76 6572 7369  ne, coding_versi
-00008820: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
-00008830: 2020 636f 6469 6e67 5f73 7973 7465 6d20    coding_system 
-00008840: 3d20 636f 6469 6e67 5f73 7973 7465 6d20  = coding_system 
-00008850: 6966 2063 6f64 696e 675f 7379 7374 656d  if coding_system
-00008860: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-00008870: 6520 7365 6c66 2e63 6f64 696e 675f 7379  e self.coding_sy
-00008880: 7374 656d 0a20 2020 2020 2020 2063 6f64  stem.        cod
-00008890: 696e 675f 7665 7273 696f 6e20 3d20 636f  ing_version = co
-000088a0: 6469 6e67 5f76 6572 7369 6f6e 2069 6620  ding_version if 
-000088b0: 636f 6469 6e67 5f76 6572 7369 6f6e 2069  coding_version i
-000088c0: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-000088d0: 7365 6c66 2e63 6f64 696e 675f 7665 7273  self.coding_vers
-000088e0: 696f 6e0a 2020 2020 2020 2020 0a20 2020  ion.        .   
-000088f0: 2020 2020 2063 6f64 696e 6720 3d20 4e6f       coding = No
-00008900: 6e65 0a20 2020 2020 2020 2069 6620 636f  ne.        if co
-00008910: 6465 6162 6c65 5f63 6f6e 6365 7074 2069  deable_concept i
-00008920: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2063  s not None and c
-00008930: 6f64 6561 626c 655f 636f 6e63 6570 742e  odeable_concept.
-00008940: 636f 6469 6e67 2069 7320 6e6f 7420 4e6f  coding is not No
-00008950: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00008960: 666f 7220 636f 6469 6e67 2069 6e20 636f  for coding in co
-00008970: 6465 6162 6c65 5f63 6f6e 6365 7074 2e63  deable_concept.c
-00008980: 6f64 696e 673a 0a20 2020 2020 2020 2020  oding:.         
-00008990: 2020 2020 2020 2069 6620 636f 6469 6e67         if coding
-000089a0: 2e73 7973 7465 6d20 3d3d 2063 6f64 696e  .system == codin
-000089b0: 675f 7379 7374 656d 2061 6e64 2063 6f64  g_system and cod
-000089c0: 696e 672e 7665 7273 696f 6e20 3d3d 2063  ing.version == c
-000089d0: 6f64 696e 675f 7665 7273 696f 6e3a 0a20  oding_version:. 
-000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089f0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00008a00: 2072 6574 7572 6e20 636f 6469 6e67 0a20   return coding. 
-00008a10: 2020 200a 2020 2020 6465 6620 746f 5f63     .    def to_c
-00008a20: 6f64 6561 626c 655f 636f 6e63 6570 7428  odeable_concept(
-00008a30: 7365 6c66 2c20 636f 6465 3d4e 6f6e 652c  self, code=None,
-00008a40: 2064 6973 706c 6179 3d4e 6f6e 652c 2069   display=None, i
-00008a50: 643d 4e6f 6e65 2c20 636f 6469 6e67 5f73  d=None, coding_s
-00008a60: 7973 7465 6d3d 4e6f 6e65 2c20 636f 6469  ystem=None, codi
-00008a70: 6e67 5f76 6572 7369 6f6e 3d4e 6f6e 6529  ng_version=None)
-00008a80: 3a0a 2020 2020 2020 2020 636f 6469 6e67  :.        coding
-00008a90: 5f73 7973 7465 6d20 3d20 636f 6469 6e67  _system = coding
-00008aa0: 5f73 7973 7465 6d20 6966 2063 6f64 696e  _system if codin
-00008ab0: 675f 7379 7374 656d 2069 7320 6e6f 7420  g_system is not 
-00008ac0: 4e6f 6e65 2065 6c73 6520 7365 6c66 2e63  None else self.c
-00008ad0: 6f64 696e 675f 7379 7374 656d 0a20 2020  oding_system.   
-00008ae0: 2020 2020 2063 6f64 696e 675f 7665 7273       coding_vers
-00008af0: 696f 6e20 3d20 636f 6469 6e67 5f76 6572  ion = coding_ver
-00008b00: 7369 6f6e 2069 6620 636f 6469 6e67 5f76  sion if coding_v
-00008b10: 6572 7369 6f6e 2069 7320 6e6f 7420 4e6f  ersion is not No
-00008b20: 6e65 2065 6c73 6520 7365 6c66 2e63 6f64  ne else self.cod
-00008b30: 696e 675f 7665 7273 696f 6e0a 2020 2020  ing_version.    
-00008b40: 2020 2020 636f 6469 6e67 203d 2043 6f64      coding = Cod
-00008b50: 696e 6728 290a 2020 2020 2020 2020 636f  ing().        co
-00008b60: 6469 6e67 2e63 6f64 6520 3d20 636f 6465  ding.code = code
-00008b70: 0a20 2020 2020 2020 2063 6f64 696e 672e  .        coding.
-00008b80: 6469 7370 6c61 7920 3d20 6469 7370 6c61  display = displa
-00008b90: 790a 2020 2020 2020 2020 636f 6469 6e67  y.        coding
-00008ba0: 2e69 6420 3d20 6964 0a20 2020 2020 2020  .id = id.       
-00008bb0: 2063 6f64 696e 672e 7665 7273 696f 6e20   coding.version 
-00008bc0: 3d20 636f 6469 6e67 5f73 7973 7465 6d0a  = coding_system.
-00008bd0: 2020 2020 2020 2020 636f 6469 6e67 2e73          coding.s
-00008be0: 7973 7465 6d20 3d20 636f 6469 6e67 5f73  ystem = coding_s
-00008bf0: 7973 7465 6d0a 2020 2020 2020 2020 636f  ystem.        co
-00008c00: 6465 6162 6c65 5f63 6f6e 6365 7074 203d  deable_concept =
-00008c10: 2043 6f64 6561 626c 6543 6f6e 6365 7074   CodeableConcept
-00008c20: 2829 0a20 2020 2020 2020 2063 6f64 6561  ().        codea
-00008c30: 626c 655f 636f 6e63 6570 742e 636f 6469  ble_concept.codi
-00008c40: 6e67 203d 205b 636f 6469 6e67 5d0a 2020  ng = [coding].  
-00008c50: 2020 2020 2020 7265 7475 726e 2063 6f64        return cod
-00008c60: 6561 626c 655f 636f 6e63 6570 740a 0a20  eable_concept.. 
-00008c70: 2020 2064 6566 2067 6574 5f6c 6f74 5f69     def get_lot_i
-00008c80: 6428 7365 6c66 2c20 696d 6d75 6e69 7a61  d(self, immuniza
-00008c90: 7469 6f6e 3d4e 6f6e 6529 3a0a 2020 2020  tion=None):.    
-00008ca0: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
-00008cb0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-00008cc0: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
-00008cd0: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
-00008ce0: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
-00008cf0: 2020 2069 6620 696d 6d75 6e69 7a61 7469     if immunizati
-00008d00: 6f6e 2069 7320 4e6f 6e65 206f 7220 696d  on is None or im
-00008d10: 6d75 6e69 7a61 7469 6f6e 2e65 7874 656e  munization.exten
-00008d20: 7369 6f6e 2069 7320 4e6f 6e65 3a0a 2020  sion is None:.  
-00008d30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008d40: 204e 6f6e 650a 2020 2020 2020 2020 6c6f   None.        lo
-00008d50: 745f 6964 203d 204e 6f6e 650a 2020 2020  t_id = None.    
-00008d60: 2020 2020 666f 7220 6578 7465 6e73 696f      for extensio
-00008d70: 6e20 696e 2069 6d6d 756e 697a 6174 696f  n in immunizatio
-00008d80: 6e2e 6578 7465 6e73 696f 6e3a 0a20 2020  n.extension:.   
-00008d90: 2020 2020 2020 2020 2069 6620 6578 7465           if exte
-00008da0: 6e73 696f 6e2e 7572 6c20 3d3d 2073 656c  nsion.url == sel
-00008db0: 662e 6c6f 745f 6964 5f75 726c 3a0a 2020  f.lot_id_url:.  
-00008dc0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00008dd0: 745f 6964 203d 2065 7874 656e 7369 6f6e  t_id = extension
-00008de0: 2e76 616c 7565 5374 7269 6e67 0a20 2020  .valueString.   
-00008df0: 2020 2020 2072 6574 7572 6e20 6c6f 745f       return lot_
-00008e00: 6964 0a20 2020 200a 2020 2020 6465 6620  id.    .    def 
-00008e10: 7365 745f 6c6f 745f 6964 2873 656c 662c  set_lot_id(self,
-00008e20: 2069 6d6d 756e 697a 6174 696f 6e3d 4e6f   immunization=No
-00008e30: 6e65 2c20 6c6f 745f 6964 3d4e 6f6e 6529  ne, lot_id=None)
-00008e40: 3a0a 2020 2020 2020 2020 6966 2069 6d6d  :.        if imm
-00008e50: 756e 697a 6174 696f 6e20 6973 204e 6f6e  unization is Non
-00008e60: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00008e70: 6d6d 756e 697a 6174 696f 6e20 3d20 7365  mmunization = se
-00008e80: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
-00008e90: 0a20 2020 2020 2020 2069 6620 6c6f 745f  .        if lot_
-00008ea0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00008eb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008ec0: 2e6c 6f74 5f69 6420 3d20 6c6f 745f 6964  .lot_id = lot_id
-00008ed0: 0a20 2020 2020 2020 206c 6f74 5f69 645f  .        lot_id_
-00008ee0: 6578 7420 3d20 4578 7465 6e73 696f 6e28  ext = Extension(
-00008ef0: 290a 2020 2020 2020 2020 6c6f 745f 6964  ).        lot_id
-00008f00: 5f65 7874 2e75 726c 203d 2073 656c 662e  _ext.url = self.
-00008f10: 6c6f 745f 6964 5f75 726c 0a20 2020 2020  lot_id_url.     
-00008f20: 2020 206c 6f74 5f69 645f 6578 742e 7661     lot_id_ext.va
-00008f30: 6c75 6553 7472 696e 6720 3d20 7365 6c66  lueString = self
-00008f40: 2e6c 6f74 5f69 640a 2020 2020 2020 2020  .lot_id.        
-00008f50: 696d 6d75 6e69 7a61 7469 6f6e 2e65 7874  immunization.ext
-00008f60: 656e 7369 6f6e 203d 2073 7570 6572 2829  ension = super()
-00008f70: 2e61 6464 5f6f 725f 7570 6461 7465 5f65  .add_or_update_e
-00008f80: 7874 656e 7369 6f6e 5f74 6f5f 6578 7465  xtension_to_exte
-00008f90: 6e73 696f 6e73 2865 7874 656e 7369 6f6e  nsions(extension
-00008fa0: 3d6c 6f74 5f69 645f 6578 742c 2065 7874  =lot_id_ext, ext
-00008fb0: 656e 7369 6f6e 733d 696d 6d75 6e69 7a61  ensions=immuniza
-00008fc0: 7469 6f6e 2e65 7874 656e 7369 6f6e 290a  tion.extension).
-00008fd0: 0a20 2020 2064 6566 2067 6574 5f74 7261  .    def get_tra
-00008fe0: 6465 5f6e 616d 6528 7365 6c66 2c20 696d  de_name(self, im
-00008ff0: 6d75 6e69 7a61 7469 6f6e 3d4e 6f6e 6529  munization=None)
-00009000: 3a0a 2020 2020 2020 2020 6966 2069 6d6d  :.        if imm
-00009010: 756e 697a 6174 696f 6e20 6973 204e 6f6e  unization is Non
-00009020: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00009030: 6d6d 756e 697a 6174 696f 6e20 3d20 7365  mmunization = se
-00009040: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
-00009050: 0a20 2020 2020 2020 2069 6620 696d 6d75  .        if immu
-00009060: 6e69 7a61 7469 6f6e 2069 7320 4e6f 6e65  nization is None
-00009070: 206f 7220 696d 6d75 6e69 7a61 7469 6f6e   or immunization
-00009080: 2e65 7874 656e 7369 6f6e 2069 7320 4e6f  .extension is No
-00009090: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000090a0: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-000090b0: 2020 2020 7472 6164 655f 6e61 6d65 203d      trade_name =
-000090c0: 204e 6f6e 650a 2020 2020 2020 2020 666f   None.        fo
-000090d0: 7220 6578 7465 6e73 696f 6e20 696e 2069  r extension in i
-000090e0: 6d6d 756e 697a 6174 696f 6e2e 6578 7465  mmunization.exte
-000090f0: 6e73 696f 6e3a 0a20 2020 2020 2020 2020  nsion:.         
-00009100: 2020 2069 6620 6578 7465 6e73 696f 6e2e     if extension.
-00009110: 7572 6c20 3d3d 2073 656c 662e 7472 6164  url == self.trad
-00009120: 655f 6e61 6d65 5f75 726c 3a0a 2020 2020  e_name_url:.    
-00009130: 2020 2020 2020 2020 2020 2020 7472 6164              trad
-00009140: 655f 6e61 6d65 203d 2065 7874 656e 7369  e_name = extensi
-00009150: 6f6e 2e76 616c 7565 5374 7269 6e67 0a20  on.valueString. 
-00009160: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
-00009170: 6164 655f 6e61 6d65 0a0a 2020 2020 6465  ade_name..    de
-00009180: 6620 7365 745f 7472 6164 655f 6e61 6d65  f set_trade_name
-00009190: 2873 656c 662c 2069 6d6d 756e 697a 6174  (self, immunizat
-000091a0: 696f 6e3d 4e6f 6e65 2c20 7472 6164 655f  ion=None, trade_
-000091b0: 6e61 6d65 3d4e 6f6e 6529 3a0a 2020 2020  name=None):.    
-000091c0: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
-000091d0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-000091e0: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
-000091f0: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
-00009200: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
-00009210: 2020 2069 6620 7472 6164 655f 6e61 6d65     if trade_name
-00009220: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00009230: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00009240: 7261 6465 5f6e 616d 6520 3d20 7472 6164  rade_name = trad
-00009250: 655f 6e61 6d65 0a20 2020 2020 2020 2074  e_name.        t
-00009260: 7261 6465 5f6e 616d 655f 6578 7420 3d20  rade_name_ext = 
-00009270: 4578 7465 6e73 696f 6e28 290a 2020 2020  Extension().    
-00009280: 2020 2020 7472 6164 655f 6e61 6d65 5f65      trade_name_e
-00009290: 7874 2e75 726c 203d 2073 656c 662e 7472  xt.url = self.tr
-000092a0: 6164 655f 6e61 6d65 5f75 726c 0a20 2020  ade_name_url.   
-000092b0: 2020 2020 2074 7261 6465 5f6e 616d 655f       trade_name_
-000092c0: 6578 742e 7661 6c75 6553 7472 696e 6720  ext.valueString 
-000092d0: 3d20 7365 6c66 2e74 7261 6465 5f6e 616d  = self.trade_nam
-000092e0: 650a 2020 2020 2020 2020 696d 6d75 6e69  e.        immuni
-000092f0: 7a61 7469 6f6e 2e65 7874 656e 7369 6f6e  zation.extension
-00009300: 203d 2073 7570 6572 2829 2e61 6464 5f6f   = super().add_o
-00009310: 725f 7570 6461 7465 5f65 7874 656e 7369  r_update_extensi
-00009320: 6f6e 5f74 6f5f 6578 7465 6e73 696f 6e73  on_to_extensions
-00009330: 2865 7874 656e 7369 6f6e 3d74 7261 6465  (extension=trade
-00009340: 5f6e 616d 655f 6578 742c 2065 7874 656e  _name_ext, exten
-00009350: 7369 6f6e 733d 696d 6d75 6e69 7a61 7469  sions=immunizati
-00009360: 6f6e 2e65 7874 656e 7369 6f6e 290a 0a20  on.extension).. 
-00009370: 2020 2064 6566 2067 6574 5f63 6f6e 7461     def get_conta
-00009380: 696e 6564 5f6f 7267 616e 697a 6174 696f  ined_organizatio
-00009390: 6e28 7365 6c66 2c20 696d 6d75 6e69 7a61  n(self, immuniza
-000093a0: 7469 6f6e 3d4e 6f6e 6529 3a0a 2020 2020  tion=None):.    
-000093b0: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
-000093c0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-000093d0: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
-000093e0: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
-000093f0: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
-00009400: 2020 2069 6620 696d 6d75 6e69 7a61 7469     if immunizati
-00009410: 6f6e 2e63 6f6e 7461 696e 6564 2069 7320  on.contained is 
-00009420: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00009430: 2020 2020 2020 666f 7220 636f 6e74 6169        for contai
-00009440: 6e65 6420 696e 2069 6d6d 756e 697a 6174  ned in immunizat
-00009450: 696f 6e2e 636f 6e74 6169 6e65 643a 0a20  ion.contained:. 
-00009460: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00009470: 6620 7479 7065 2863 6f6e 7461 696e 6564  f type(contained
-00009480: 2920 6973 204f 7267 616e 697a 6174 696f  ) is Organizatio
-00009490: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
-000094a0: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
-000094b0: 6e74 6169 6e65 640a 2020 2020 2020 2020  ntained.        
-000094c0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-000094d0: 2064 6566 2073 6574 5f63 6f6e 7461 696e   def set_contain
-000094e0: 6564 5f6f 7267 616e 697a 6174 696f 6e28  ed_organization(
-000094f0: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
-00009500: 6f6e 3d4e 6f6e 652c 206f 7267 616e 697a  on=None, organiz
-00009510: 6174 696f 6e3d 4e6f 6e65 293a 0a20 2020  ation=None):.   
-00009520: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
-00009530: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-00009540: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
-00009550: 7a61 7469 6f6e 203d 2073 656c 662e 6668  zation = self.fh
-00009560: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
-00009570: 2020 2020 6966 206f 7267 616e 697a 6174      if organizat
-00009580: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-00009590: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000095a0: 662e 6f72 6761 6e69 7a61 7469 6f6e 203d  f.organization =
-000095b0: 206f 7267 616e 697a 6174 696f 6e0a 2020   organization.  
-000095c0: 2020 2020 2020 636f 6e74 6169 6e65 645f        contained_
-000095d0: 6f72 6761 6e69 7a61 7469 6f6e 203d 204e  organization = N
-000095e0: 6f6e 650a 2020 2020 2020 2020 6966 2074  one.        if t
-000095f0: 7970 6528 7365 6c66 2e6f 7267 616e 697a  ype(self.organiz
-00009600: 6174 696f 6e29 2069 7320 6469 6374 3a0a  ation) is dict:.
+00005d40: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+00005d50: 203d 2073 656c 662e 746f 5f66 6869 725f   = self.to_fhir_
+00005d60: 7265 736f 7572 6365 2829 0a20 2020 2020  resource().     
+00005d70: 2020 2065 6c73 653a 200a 2020 2020 2020     else: .      
+00005d80: 2020 2020 2020 7365 6c66 2e66 726f 6d5f        self.from_
+00005d90: 6469 6374 2869 6d6d 5f64 6963 743d 696d  dict(imm_dict=im
+00005da0: 6d5f 6469 6374 290a 0a0a 2020 2020 6465  m_dict)...    de
+00005db0: 6620 7365 745f 6964 2873 656c 662c 2069  f set_id(self, i
+00005dc0: 6d6d 756e 697a 6174 696f 6e3d 4e6f 6e65  mmunization=None
+00005dd0: 2c20 6964 3d4e 6f6e 6529 3a0a 2020 2020  , id=None):.    
+00005de0: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
+00005df0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
+00005e00: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
+00005e10: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
+00005e20: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
+00005e30: 2020 2069 6620 6964 2069 7320 6e6f 7420     if id is not 
+00005e40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00005e50: 2020 7365 6c66 2e69 6420 3d20 6964 0a20    self.id = id. 
+00005e60: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
+00005e70: 696f 6e2e 6964 203d 2073 656c 662e 6964  ion.id = self.id
+00005e80: 0a0a 2020 2020 6465 6620 6765 745f 6964  ..    def get_id
+00005e90: 2873 656c 662c 2069 6d6d 756e 697a 6174  (self, immunizat
+00005ea0: 696f 6e3d 4e6f 6e65 293a 0a20 2020 2020  ion=None):.     
+00005eb0: 2020 2069 6620 696d 6d75 6e69 7a61 7469     if immunizati
+00005ec0: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00005ed0: 2020 2020 2020 2020 696d 6d75 6e69 7a61          immuniza
+00005ee0: 7469 6f6e 203d 2073 656c 662e 6668 6972  tion = self.fhir
+00005ef0: 5f72 6573 6f75 7263 650a 0a20 2020 2020  _resource..     
+00005f00: 2020 2072 6574 7572 6e20 696d 6d75 6e69     return immuni
+00005f10: 7a61 7469 6f6e 2e69 640a 2020 2020 2020  zation.id.      
+00005f20: 2020 0a20 2020 2064 6566 2067 6574 5f6d    .    def get_m
+00005f30: 6574 615f 7570 6461 7465 645f 6279 2873  eta_updated_by(s
+00005f40: 656c 662c 2069 6d6d 756e 697a 6174 696f  elf, immunizatio
+00005f50: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
+00005f60: 2069 6620 696d 6d75 6e69 7a61 7469 6f6e   if immunization
+00005f70: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00005f80: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
+00005f90: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
+00005fa0: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
+00005fb0: 6966 2069 6d6d 756e 697a 6174 696f 6e20  if immunization 
+00005fc0: 6973 204e 6f6e 6520 6f72 2069 6d6d 756e  is None or immun
+00005fd0: 697a 6174 696f 6e2e 6d65 7461 2069 7320  ization.meta is 
+00005fe0: 4e6f 6e65 206f 7220 696d 6d75 6e69 7a61  None or immuniza
+00005ff0: 7469 6f6e 2e6d 6574 612e 6578 7465 6e73  tion.meta.extens
+00006000: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
+00006010: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006020: 4e6f 6e65 0a20 2020 2020 2020 2066 6f72  None.        for
+00006030: 2065 7874 656e 7369 6f6e 2069 6e20 696d   extension in im
+00006040: 6d75 6e69 7a61 7469 6f6e 2e6d 6574 612e  munization.meta.
+00006050: 6578 7465 6e73 696f 6e3a 0a20 2020 2020  extension:.     
+00006060: 2020 2020 2020 2069 6620 6578 7465 6e73         if extens
+00006070: 696f 6e2e 7572 6c20 3d3d 2073 656c 662e  ion.url == self.
+00006080: 7570 6461 7465 645f 6279 5f75 726c 3a0a  updated_by_url:.
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060a0: 7265 7475 726e 2065 7874 656e 7369 6f6e  return extension
+000060b0: 2e76 616c 7565 5374 7269 6e67 0a20 2020  .valueString.   
+000060c0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000060d0: 0a0a 2020 2020 6465 6620 6765 745f 6d65  ..    def get_me
+000060e0: 7461 5f63 7265 6174 6564 5f62 7928 7365  ta_created_by(se
+000060f0: 6c66 2c20 696d 6d75 6e69 7a61 7469 6f6e  lf, immunization
+00006100: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00006110: 6966 2069 6d6d 756e 697a 6174 696f 6e20  if immunization 
+00006120: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00006130: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
+00006140: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
+00006150: 736f 7572 6365 0a20 2020 2020 2020 2069  source.        i
+00006160: 6620 696d 6d75 6e69 7a61 7469 6f6e 2069  f immunization i
+00006170: 7320 4e6f 6e65 206f 7220 696d 6d75 6e69  s None or immuni
+00006180: 7a61 7469 6f6e 2e6d 6574 6120 6973 204e  zation.meta is N
+00006190: 6f6e 6520 6f72 2069 6d6d 756e 697a 6174  one or immunizat
+000061a0: 696f 6e2e 6d65 7461 2e65 7874 656e 7369  ion.meta.extensi
+000061b0: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+000061c0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+000061d0: 6f6e 650a 2020 2020 2020 2020 666f 7220  one.        for 
+000061e0: 6578 7465 6e73 696f 6e20 696e 2069 6d6d  extension in imm
+000061f0: 756e 697a 6174 696f 6e2e 6d65 7461 2e65  unization.meta.e
+00006200: 7874 656e 7369 6f6e 3a0a 2020 2020 2020  xtension:.      
+00006210: 2020 2020 2020 6966 2065 7874 656e 7369        if extensi
+00006220: 6f6e 2e75 726c 203d 3d20 7365 6c66 2e63  on.url == self.c
+00006230: 7265 6174 6564 5f62 795f 7572 6c3a 0a20  reated_by_url:. 
+00006240: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00006250: 6574 7572 6e20 6578 7465 6e73 696f 6e2e  eturn extension.
+00006260: 7661 6c75 6553 7472 696e 670a 2020 2020  valueString.    
+00006270: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00006280: 0a20 2020 2064 6566 2067 6574 5f6d 6574  .    def get_met
+00006290: 615f 6372 6561 7469 6f6e 5f64 6174 6528  a_creation_date(
+000062a0: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
+000062b0: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
+000062c0: 2020 6966 2069 6d6d 756e 697a 6174 696f    if immunizatio
+000062d0: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+000062e0: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
+000062f0: 696f 6e20 3d20 7365 6c66 2e66 6869 725f  ion = self.fhir_
+00006300: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
+00006310: 2069 6620 696d 6d75 6e69 7a61 7469 6f6e   if immunization
+00006320: 2069 7320 4e6f 6e65 206f 7220 696d 6d75   is None or immu
+00006330: 6e69 7a61 7469 6f6e 2e6d 6574 6120 6973  nization.meta is
+00006340: 204e 6f6e 6520 6f72 2069 6d6d 756e 697a   None or immuniz
+00006350: 6174 696f 6e2e 6d65 7461 2e65 7874 656e  ation.meta.exten
+00006360: 7369 6f6e 2069 7320 4e6f 6e65 3a0a 2020  sion is None:.  
+00006370: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00006380: 204e 6f6e 650a 2020 2020 2020 2020 666f   None.        fo
+00006390: 7220 6578 7465 6e73 696f 6e20 696e 2069  r extension in i
+000063a0: 6d6d 756e 697a 6174 696f 6e2e 6d65 7461  mmunization.meta
+000063b0: 2e65 7874 656e 7369 6f6e 3a0a 2020 2020  .extension:.    
+000063c0: 2020 2020 2020 2020 6966 2065 7874 656e          if exten
+000063d0: 7369 6f6e 2e75 726c 203d 3d20 7365 6c66  sion.url == self
+000063e0: 2e63 7265 6174 696f 6e5f 6461 7465 5f75  .creation_date_u
+000063f0: 726c 3a0a 2020 2020 2020 2020 2020 2020  rl:.            
+00006400: 2020 2020 7265 7475 726e 2065 7874 656e      return exten
+00006410: 7369 6f6e 2e76 616c 7565 4461 7465 0a20  sion.valueDate. 
+00006420: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00006430: 6e65 0a0a 2020 2020 6465 6620 6765 745f  ne..    def get_
+00006440: 6d65 7461 5f76 6572 7369 6f6e 5f69 6428  meta_version_id(
+00006450: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
+00006460: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
+00006470: 2020 6966 2069 6d6d 756e 697a 6174 696f    if immunizatio
+00006480: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+00006490: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
+000064a0: 696f 6e20 3d20 7365 6c66 2e66 6869 725f  ion = self.fhir_
+000064b0: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
+000064c0: 2069 6620 696d 6d75 6e69 7a61 7469 6f6e   if immunization
+000064d0: 2069 7320 4e6f 6e65 206f 7220 696d 6d75   is None or immu
+000064e0: 6e69 7a61 7469 6f6e 2e6d 6574 6120 6973  nization.meta is
+000064f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00006500: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00006510: 2020 2020 2020 2072 6574 7572 6e20 696d         return im
+00006520: 6d75 6e69 7a61 7469 6f6e 2e6d 6574 612e  munization.meta.
+00006530: 7665 7273 696f 6e49 640a 0a20 2020 2064  versionId..    d
+00006540: 6566 2067 6574 5f6d 6574 615f 6c61 7374  ef get_meta_last
+00006550: 5f75 7064 6174 6564 2873 656c 662c 2069  _updated(self, i
+00006560: 6d6d 756e 697a 6174 696f 6e3d 4e6f 6e65  mmunization=None
+00006570: 293a 0a20 2020 2020 2020 2069 6620 696d  ):.        if im
+00006580: 6d75 6e69 7a61 7469 6f6e 2069 7320 4e6f  munization is No
+00006590: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000065a0: 696d 6d75 6e69 7a61 7469 6f6e 203d 2073  immunization = s
+000065b0: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+000065c0: 650a 2020 2020 2020 2020 6966 2069 6d6d  e.        if imm
+000065d0: 756e 697a 6174 696f 6e20 6973 204e 6f6e  unization is Non
+000065e0: 6520 6f72 2069 6d6d 756e 697a 6174 696f  e or immunizatio
+000065f0: 6e2e 6d65 7461 2069 7320 4e6f 6e65 3a0a  n.meta is None:.
+00006600: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00006610: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
+00006620: 6966 2069 6d6d 756e 697a 6174 696f 6e2e  if immunization.
+00006630: 6d65 7461 2e6c 6173 7455 7064 6174 6564  meta.lastUpdated
+00006640: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00006650: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00006660: 2069 6d6d 756e 697a 6174 696f 6e2e 6d65   immunization.me
+00006670: 7461 2e6c 6173 7455 7064 6174 6564 2e69  ta.lastUpdated.i
+00006680: 736f 7374 7269 6e67 0a20 2020 2020 2020  sostring.       
+00006690: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000066a0: 2020 2072 6574 7572 6e20 696d 6d75 6e69     return immuni
+000066b0: 7a61 7469 6f6e 2e6d 6574 612e 6c61 7374  zation.meta.last
+000066c0: 5570 6461 7465 640a 0a20 2020 2064 6566  Updated..    def
+000066d0: 2067 6574 5f6d 6574 615f 7072 6f66 696c   get_meta_profil
+000066e0: 6528 7365 6c66 2c20 696d 6d75 6e69 7a61  e(self, immuniza
+000066f0: 7469 6f6e 3d4e 6f6e 6529 3a0a 2020 2020  tion=None):.    
+00006700: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
+00006710: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
+00006720: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
+00006730: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
+00006740: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
+00006750: 2020 2069 6620 696d 6d75 6e69 7a61 7469     if immunizati
+00006760: 6f6e 2069 7320 4e6f 6e65 206f 7220 696d  on is None or im
+00006770: 6d75 6e69 7a61 7469 6f6e 2e6d 6574 6120  munization.meta 
+00006780: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00006790: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000067a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000067b0: 696d 6d75 6e69 7a61 7469 6f6e 2e6d 6574  immunization.met
+000067c0: 612e 7072 6f66 696c 650a 0a20 2020 2064  a.profile..    d
+000067d0: 6566 2073 6574 5f6d 6574 6128 7365 6c66  ef set_meta(self
+000067e0: 2c20 696d 6d75 6e69 7a61 7469 6f6e 3d4e  , immunization=N
+000067f0: 6f6e 652c 2076 6572 7369 6f6e 5f69 643d  one, version_id=
+00006800: 4e6f 6e65 2c20 6c61 7374 5f75 7064 6174  None, last_updat
+00006810: 6564 3d4e 6f6e 652c 2070 726f 6669 6c65  ed=None, profile
+00006820: 3d4e 6f6e 652c 2075 7064 6174 6564 5f62  =None, updated_b
+00006830: 793d 4e6f 6e65 2c20 6372 6561 7469 6f6e  y=None, creation
+00006840: 5f64 6174 653d 4e6f 6e65 2c20 6372 6561  _date=None, crea
+00006850: 7465 645f 6279 3d4e 6f6e 6529 3a0a 2020  ted_by=None):.  
+00006860: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
+00006870: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
+00006880: 2020 2020 2020 2020 2020 2069 6d6d 756e             immun
+00006890: 697a 6174 696f 6e20 3d20 7365 6c66 2e66  ization = self.f
+000068a0: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
+000068b0: 2020 2020 2069 6620 7665 7273 696f 6e5f       if version_
+000068c0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000068d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000068e0: 2e76 6572 7369 6f6e 5f69 6420 3d20 7665  .version_id = ve
+000068f0: 7273 696f 6e5f 6964 0a20 2020 2020 2020  rsion_id.       
+00006900: 2069 6620 6c61 7374 5f75 7064 6174 6564   if last_updated
+00006910: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00006920: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00006930: 6173 745f 7570 6461 7465 6420 3d20 6c61  ast_updated = la
+00006940: 7374 5f75 7064 6174 6564 0a20 2020 2020  st_updated.     
+00006950: 2020 2069 6620 7072 6f66 696c 6520 6973     if profile is
+00006960: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00006970: 2020 2020 2020 2073 656c 662e 7072 6f66         self.prof
+00006980: 696c 6520 3d20 7072 6f66 696c 650a 2020  ile = profile.  
+00006990: 2020 2020 2020 6966 2075 7064 6174 6564        if updated
+000069a0: 5f62 7920 6973 206e 6f74 204e 6f6e 653a  _by is not None:
+000069b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000069c0: 662e 7570 6461 7465 645f 6279 203d 2075  f.updated_by = u
+000069d0: 7064 6174 6564 5f62 790a 2020 2020 2020  pdated_by.      
+000069e0: 2020 6966 2063 7265 6174 696f 6e5f 6461    if creation_da
+000069f0: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  te is not None:.
+00006a00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006a10: 2e63 7265 6174 696f 6e5f 6461 7465 203d  .creation_date =
+00006a20: 2063 7265 6174 696f 6e5f 6461 7465 0a20   creation_date. 
+00006a30: 2020 2020 2020 2069 6620 6372 6561 7465         if create
+00006a40: 645f 6279 2069 7320 6e6f 7420 4e6f 6e65  d_by is not None
+00006a50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00006a60: 6c66 2e63 7265 6174 6564 5f62 7920 3d20  lf.created_by = 
+00006a70: 6372 6561 7465 645f 6279 0a20 2020 2020  created_by.     
+00006a80: 2020 2069 6620 696d 6d75 6e69 7a61 7469     if immunizati
+00006a90: 6f6e 2e6d 6574 6120 6973 204e 6f6e 653a  on.meta is None:
+00006aa0: 0a20 2020 2020 2020 2020 2020 2069 6d6d  .            imm
+00006ab0: 756e 697a 6174 696f 6e2e 6d65 7461 203d  unization.meta =
+00006ac0: 204d 6574 6128 290a 2020 2020 2020 2020   Meta().        
+00006ad0: 696d 6d75 6e69 7a61 7469 6f6e 2e6d 6574  immunization.met
+00006ae0: 612e 7665 7273 696f 6e49 6420 3d20 7365  a.versionId = se
+00006af0: 6c66 2e76 6572 7369 6f6e 5f69 640a 2020  lf.version_id.  
+00006b00: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
+00006b10: 6f6e 2e6d 6574 612e 6c61 7374 5570 6461  on.meta.lastUpda
+00006b20: 7465 6420 3d20 7365 6c66 2e6c 6173 745f  ted = self.last_
+00006b30: 7570 6461 7465 640a 2020 2020 2020 2020  updated.        
+00006b40: 696d 6d75 6e69 7a61 7469 6f6e 2e6d 6574  immunization.met
+00006b50: 612e 7072 6f66 696c 6520 3d20 7365 6c66  a.profile = self
+00006b60: 2e70 726f 6669 6c65 0a20 2020 2020 2020  .profile.       
+00006b70: 2069 6620 7365 6c66 2e75 7064 6174 6564   if self.updated
+00006b80: 5f62 7920 6973 206e 6f74 204e 6f6e 653a  _by is not None:
+00006b90: 0a20 2020 2020 2020 2020 2020 2075 7064  .            upd
+00006ba0: 6174 6564 5f62 795f 6578 7420 3d20 4578  ated_by_ext = Ex
+00006bb0: 7465 6e73 696f 6e28 290a 2020 2020 2020  tension().      
+00006bc0: 2020 2020 2020 7570 6461 7465 645f 6279        updated_by
+00006bd0: 5f65 7874 2e75 726c 203d 2073 656c 662e  _ext.url = self.
+00006be0: 7570 6461 7465 645f 6279 5f75 726c 0a20  updated_by_url. 
+00006bf0: 2020 2020 2020 2020 2020 2075 7064 6174             updat
+00006c00: 6564 5f62 795f 6578 742e 7661 6c75 6553  ed_by_ext.valueS
+00006c10: 7472 696e 6720 3d20 7365 6c66 2e75 7064  tring = self.upd
+00006c20: 6174 6564 5f62 790a 2020 2020 2020 2020  ated_by.        
+00006c30: 2020 2020 696d 6d75 6e69 7a61 7469 6f6e      immunization
+00006c40: 2e6d 6574 612e 6578 7465 6e73 696f 6e20  .meta.extension 
+00006c50: 3d20 7375 7065 7228 292e 6164 645f 6f72  = super().add_or
+00006c60: 5f75 7064 6174 655f 6578 7465 6e73 696f  _update_extensio
+00006c70: 6e5f 746f 5f65 7874 656e 7369 6f6e 7328  n_to_extensions(
+00006c80: 6578 7465 6e73 696f 6e3d 7570 6461 7465  extension=update
+00006c90: 645f 6279 5f65 7874 2c20 6578 7465 6e73  d_by_ext, extens
+00006ca0: 696f 6e73 3d69 6d6d 756e 697a 6174 696f  ions=immunizatio
+00006cb0: 6e2e 6d65 7461 2e65 7874 656e 7369 6f6e  n.meta.extension
+00006cc0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00006cd0: 662e 6372 6561 7469 6f6e 5f64 6174 6520  f.creation_date 
+00006ce0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00006cf0: 280a 2020 2020 2020 2020 2020 2020 7479  (.            ty
+00006d00: 7065 2873 656c 662e 6372 6561 7469 6f6e  pe(self.creation
+00006d10: 5f64 6174 6529 2069 7320 6461 7465 206f  _date) is date o
+00006d20: 720a 2020 2020 2020 2020 2020 2020 7479  r.            ty
+00006d30: 7065 2873 656c 662e 6372 6561 7469 6f6e  pe(self.creation
+00006d40: 5f64 6174 6529 2069 7320 4648 4952 4461  _date) is FHIRDa
+00006d50: 7465 206f 7220 0a20 2020 2020 2020 2020  te or .         
+00006d60: 2020 2074 7970 6528 7365 6c66 2e63 7265     type(self.cre
+00006d70: 6174 696f 6e5f 6461 7465 2920 6973 2073  ation_date) is s
+00006d80: 7472 293a 0a0a 2020 2020 2020 2020 2020  tr):..          
+00006d90: 2020 6372 6561 7469 6f6e 5f64 6174 655f    creation_date_
+00006da0: 6578 7420 3d20 4578 7465 6e73 696f 6e28  ext = Extension(
+00006db0: 290a 2020 2020 2020 2020 2020 2020 6372  ).            cr
+00006dc0: 6561 7469 6f6e 5f64 6174 655f 6578 742e  eation_date_ext.
+00006dd0: 7572 6c20 3d20 7365 6c66 2e63 7265 6174  url = self.creat
+00006de0: 696f 6e5f 6461 7465 5f75 726c 0a20 2020  ion_date_url.   
+00006df0: 2020 2020 2020 2020 2069 6620 7479 7065           if type
+00006e00: 2873 656c 662e 6372 6561 7469 6f6e 5f64  (self.creation_d
+00006e10: 6174 6529 2069 7320 7374 723a 0a20 2020  ate) is str:.   
+00006e20: 2020 2020 2020 2020 2020 2020 2063 7265               cre
+00006e30: 6174 696f 6e5f 6461 7465 5f65 7874 2e76  ation_date_ext.v
+00006e40: 616c 7565 4461 7465 203d 2064 6174 6574  alueDate = datet
+00006e50: 696d 652e 7374 7266 7469 6d65 2873 656c  ime.strftime(sel
+00006e60: 662e 6372 6561 7469 6f6e 5f64 6174 652c  f.creation_date,
+00006e70: 2022 2559 2d25 6d2d 2564 5425 483a 254d   "%Y-%m-%dT%H:%M
+00006e80: 3a25 5325 7a22 290a 2020 2020 2020 2020  :%S%z").        
+00006e90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00006ea0: 2020 2020 2020 2020 2020 6372 6561 7469            creati
+00006eb0: 6f6e 5f64 6174 655f 6578 742e 7661 6c75  on_date_ext.valu
+00006ec0: 6544 6174 6520 3d20 7365 6c66 2e63 7265  eDate = self.cre
+00006ed0: 6174 696f 6e5f 6461 7465 0a20 2020 2020  ation_date.     
+00006ee0: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
+00006ef0: 696f 6e2e 6d65 7461 2e65 7874 656e 7369  ion.meta.extensi
+00006f00: 6f6e 203d 2073 7570 6572 2829 2e61 6464  on = super().add
+00006f10: 5f6f 725f 7570 6461 7465 5f65 7874 656e  _or_update_exten
+00006f20: 7369 6f6e 5f74 6f5f 6578 7465 6e73 696f  sion_to_extensio
+00006f30: 6e73 2865 7874 656e 7369 6f6e 3d63 7265  ns(extension=cre
+00006f40: 6174 696f 6e5f 6461 7465 5f65 7874 2c20  ation_date_ext, 
+00006f50: 6578 7465 6e73 696f 6e73 3d69 6d6d 756e  extensions=immun
+00006f60: 697a 6174 696f 6e2e 6d65 7461 2e65 7874  ization.meta.ext
+00006f70: 656e 7369 6f6e 290a 2020 2020 2020 2020  ension).        
+00006f80: 6966 2073 656c 662e 6372 6561 7465 645f  if self.created_
+00006f90: 6279 2069 7320 6e6f 7420 4e6f 6e65 3a0a  by is not None:.
+00006fa0: 2020 2020 2020 2020 2020 2020 6372 6561              crea
+00006fb0: 7465 645f 6279 5f65 7874 203d 2045 7874  ted_by_ext = Ext
+00006fc0: 656e 7369 6f6e 2829 0a20 2020 2020 2020  ension().       
+00006fd0: 2020 2020 2063 7265 6174 6564 5f62 795f       created_by_
+00006fe0: 6578 742e 7572 6c20 3d20 7365 6c66 2e63  ext.url = self.c
+00006ff0: 7265 6174 6564 5f62 795f 7572 6c0a 2020  reated_by_url.  
+00007000: 2020 2020 2020 2020 2020 6372 6561 7465            create
+00007010: 645f 6279 5f65 7874 2e76 616c 7565 5374  d_by_ext.valueSt
+00007020: 7269 6e67 203d 2073 656c 662e 6372 6561  ring = self.crea
+00007030: 7465 645f 6279 0a20 2020 2020 2020 2020  ted_by.         
+00007040: 2020 2069 6d6d 756e 697a 6174 696f 6e2e     immunization.
+00007050: 6d65 7461 2e65 7874 656e 7369 6f6e 203d  meta.extension =
+00007060: 2073 7570 6572 2829 2e61 6464 5f6f 725f   super().add_or_
+00007070: 7570 6461 7465 5f65 7874 656e 7369 6f6e  update_extension
+00007080: 5f74 6f5f 6578 7465 6e73 696f 6e73 2865  _to_extensions(e
+00007090: 7874 656e 7369 6f6e 3d63 7265 6174 6564  xtension=created
+000070a0: 5f62 795f 6578 742c 2065 7874 656e 7369  _by_ext, extensi
+000070b0: 6f6e 733d 696d 6d75 6e69 7a61 7469 6f6e  ons=immunization
+000070c0: 2e6d 6574 612e 6578 7465 6e73 696f 6e29  .meta.extension)
+000070d0: 0a0a 2020 2020 6465 6620 6765 745f 6f76  ..    def get_ov
+000070e0: 6572 7269 6465 5f73 7461 7475 7328 7365  erride_status(se
+000070f0: 6c66 2c20 696d 6d75 6e69 7a61 7469 6f6e  lf, immunization
+00007100: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00007110: 6966 2069 6d6d 756e 697a 6174 696f 6e20  if immunization 
+00007120: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00007130: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
+00007140: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
+00007150: 736f 7572 6365 0a20 2020 2020 2020 206f  source.        o
+00007160: 7665 7272 6964 655f 7374 6174 7573 5f65  verride_status_e
+00007170: 7874 656e 7369 6f6e 203d 204e 6f6e 650a  xtension = None.
+00007180: 2020 2020 2020 2020 6966 2069 6d6d 756e          if immun
+00007190: 697a 6174 696f 6e2e 6578 7465 6e73 696f  ization.extensio
+000071a0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+000071b0: 2020 2020 2020 2020 2020 2066 6f72 2065             for e
+000071c0: 7874 2069 6e20 696d 6d75 6e69 7a61 7469  xt in immunizati
+000071d0: 6f6e 2e65 7874 656e 7369 6f6e 3a0a 2020  on.extension:.  
+000071e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000071f0: 2065 7874 2e75 726c 203d 3d20 7365 6c66   ext.url == self
+00007200: 2e6f 7665 7272 6964 655f 7374 6174 7573  .override_status
+00007210: 5f75 726c 3a0a 2020 2020 2020 2020 2020  _url:.          
+00007220: 2020 2020 2020 2020 2020 6f76 6572 7269            overri
+00007230: 6465 5f73 7461 7475 735f 6578 7465 6e73  de_status_extens
+00007240: 696f 6e20 3d20 6578 740a 2020 2020 2020  ion = ext.      
+00007250: 2020 7265 7475 726e 206f 7665 7272 6964    return overrid
+00007260: 655f 7374 6174 7573 5f65 7874 656e 7369  e_status_extensi
+00007270: 6f6e 0a0a 2020 2020 6465 6620 7365 745f  on..    def set_
+00007280: 6f76 6572 7269 6465 5f73 7461 7475 7328  override_status(
+00007290: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
+000072a0: 6f6e 3d4e 6f6e 652c 2073 7461 7475 735f  on=None, status_
+000072b0: 636f 6465 3d4e 6f6e 652c 2073 7461 7475  code=None, statu
+000072c0: 735f 6469 7370 6c61 793d 4e6f 6e65 2c20  s_display=None, 
+000072d0: 7374 6174 7573 5f69 643d 4e6f 6e65 2c20  status_id=None, 
+000072e0: 636f 6469 6e67 5f73 7973 7465 6d3d 4e6f  coding_system=No
+000072f0: 6e65 2c20 636f 6469 6e67 5f76 6572 7369  ne, coding_versi
+00007300: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
+00007310: 2020 6966 2069 6d6d 756e 697a 6174 696f    if immunizatio
+00007320: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+00007330: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
+00007340: 696f 6e20 3d20 7365 6c66 2e66 6869 725f  ion = self.fhir_
+00007350: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
+00007360: 2069 6620 7374 6174 7573 5f63 6f64 6520   if status_code 
+00007370: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00007380: 7374 6174 7573 5f64 6973 706c 6179 2069  status_display i
+00007390: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
+000073a0: 7461 7475 735f 6964 2069 7320 6e6f 7420  tatus_id is not 
+000073b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000073c0: 2020 7365 6c66 2e6f 7665 7272 6964 655f    self.override_
+000073d0: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+000073e0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+000073f0: 2020 2020 2020 7365 6c66 2e6f 7665 7272        self.overr
+00007400: 6964 655f 7374 6174 7573 5f64 6973 706c  ide_status_displ
+00007410: 6179 203d 2073 7461 7475 735f 6469 7370  ay = status_disp
+00007420: 6c61 790a 2020 2020 2020 2020 2020 2020  lay.            
+00007430: 7365 6c66 2e6f 7665 7272 6964 655f 7374  self.override_st
+00007440: 6174 7573 5f69 6420 3d20 7374 6174 7573  atus_id = status
+00007450: 5f69 640a 2020 2020 2020 2020 7374 6174  _id.        stat
+00007460: 7573 5f63 6f64 6561 626c 655f 636f 6e63  us_codeable_conc
+00007470: 6570 7420 3d20 7365 6c66 2e74 6f5f 636f  ept = self.to_co
+00007480: 6465 6162 6c65 5f63 6f6e 6365 7074 280a  deable_concept(.
+00007490: 2020 2020 2020 2020 2020 2020 636f 6465              code
+000074a0: 3d73 656c 662e 6f76 6572 7269 6465 5f73  =self.override_s
+000074b0: 7461 7475 735f 636f 6465 2c0a 2020 2020  tatus_code,.    
+000074c0: 2020 2020 2020 2020 6469 7370 6c61 793d          display=
+000074d0: 7365 6c66 2e6f 7665 7272 6964 655f 7374  self.override_st
+000074e0: 6174 7573 5f64 6973 706c 6179 2c0a 2020  atus_display,.  
+000074f0: 2020 2020 2020 2020 2020 6964 3d73 656c            id=sel
+00007500: 662e 6f76 6572 7269 6465 5f73 7461 7475  f.override_statu
+00007510: 735f 6964 2c0a 2020 2020 2020 2020 2020  s_id,.          
+00007520: 2020 636f 6469 6e67 5f73 7973 7465 6d3d    coding_system=
+00007530: 636f 6469 6e67 5f73 7973 7465 6d2c 0a20  coding_system,. 
+00007540: 2020 2020 2020 2020 2020 2063 6f64 696e             codin
+00007550: 675f 7665 7273 696f 6e3d 636f 6469 6e67  g_version=coding
+00007560: 5f76 6572 7369 6f6e 290a 2020 2020 2020  _version).      
+00007570: 2020 6e65 775f 6578 7420 3d20 4578 7465    new_ext = Exte
+00007580: 6e73 696f 6e28 290a 2020 2020 2020 2020  nsion().        
+00007590: 6e65 775f 6578 742e 7572 6c20 3d20 7365  new_ext.url = se
+000075a0: 6c66 2e6f 7665 7272 6964 655f 7374 6174  lf.override_stat
+000075b0: 7573 5f75 726c 0a20 2020 2020 2020 206e  us_url.        n
+000075c0: 6577 5f65 7874 2e76 616c 7565 436f 6465  ew_ext.valueCode
+000075d0: 6162 6c65 436f 6e63 6570 7420 3d20 7374  ableConcept = st
+000075e0: 6174 7573 5f63 6f64 6561 626c 655f 636f  atus_codeable_co
+000075f0: 6e63 6570 740a 2020 2020 2020 2020 696d  ncept.        im
+00007600: 6d75 6e69 7a61 7469 6f6e 2e65 7874 656e  munization.exten
+00007610: 7369 6f6e 203d 2073 7570 6572 2829 2e61  sion = super().a
+00007620: 6464 5f6f 725f 7570 6461 7465 5f65 7874  dd_or_update_ext
+00007630: 656e 7369 6f6e 5f74 6f5f 6578 7465 6e73  ension_to_extens
+00007640: 696f 6e73 2865 7874 656e 7369 6f6e 3d6e  ions(extension=n
+00007650: 6577 5f65 7874 2c20 6578 7465 6e73 696f  ew_ext, extensio
+00007660: 6e73 3d69 6d6d 756e 697a 6174 696f 6e2e  ns=immunization.
+00007670: 6578 7465 6e73 696f 6e29 0a0a 2020 2020  extension)..    
+00007680: 6465 6620 7365 745f 616e 7469 6765 6e5f  def set_antigen_
+00007690: 7374 6174 7573 280a 2020 2020 2020 2020  status(.        
+000076a0: 7365 6c66 2c0a 2020 2020 2020 2020 696d  self,.        im
+000076b0: 6d75 6e69 7a61 7469 6f6e 3d4e 6f6e 652c  munization=None,
+000076c0: 0a20 2020 2020 2020 2061 6e74 6967 656e  .        antigen
+000076d0: 5f63 6f64 653d 4e6f 6e65 2c0a 2020 2020  _code=None,.    
+000076e0: 2020 2020 616e 7469 6765 6e5f 6964 3d4e      antigen_id=N
+000076f0: 6f6e 652c 0a20 2020 2020 2020 2061 6e74  one,.        ant
+00007700: 6967 656e 5f64 6973 706c 6179 3d4e 6f6e  igen_display=Non
+00007710: 652c 0a20 2020 2020 2020 2064 6f73 655f  e,.        dose_
+00007720: 6e75 6d62 6572 3d4e 6f6e 652c 0a20 2020  number=None,.   
+00007730: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
+00007740: 3d4e 6f6e 652c 0a20 2020 2020 2020 2073  =None,.        s
+00007750: 7461 7475 735f 6964 3d4e 6f6e 652c 0a20  tatus_id=None,. 
+00007760: 2020 2020 2020 2073 7461 7475 735f 6469         status_di
+00007770: 7370 6c61 793d 4e6f 6e65 2c0a 2020 2020  splay=None,.    
+00007780: 2020 2020 636f 6469 6e67 5f73 7973 7465      coding_syste
+00007790: 6d3d 4e6f 6e65 2c0a 2020 2020 2020 2020  m=None,.        
+000077a0: 636f 6469 6e67 5f76 6572 7369 6f6e 3d4e  coding_version=N
+000077b0: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
+000077c0: 2069 6d6d 756e 697a 6174 696f 6e20 6973   immunization is
+000077d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000077e0: 2020 2069 6d6d 756e 697a 6174 696f 6e20     immunization 
+000077f0: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
+00007800: 7572 6365 0a0a 2020 2020 2020 2020 616e  urce..        an
+00007810: 7469 6765 6e5f 7374 6174 7573 5f65 7874  tigen_status_ext
+00007820: 203d 2045 7874 656e 7369 6f6e 2829 0a20   = Extension(). 
+00007830: 2020 2020 2020 2061 6e74 6967 656e 5f73         antigen_s
+00007840: 7461 7475 735f 6578 742e 7572 6c20 3d20  tatus_ext.url = 
+00007850: 7365 6c66 2e61 6e74 6967 656e 5f73 7461  self.antigen_sta
+00007860: 7475 735f 7572 6c0a 0a20 2020 2020 2020  tus_url..       
+00007870: 2069 6620 616e 7469 6765 6e5f 636f 6465   if antigen_code
+00007880: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00007890: 2061 6e74 6967 656e 5f69 6420 6973 206e   antigen_id is n
+000078a0: 6f74 204e 6f6e 6520 616e 6420 616e 7469  ot None and anti
+000078b0: 6765 6e5f 6469 7370 6c61 7920 6973 206e  gen_display is n
+000078c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000078d0: 2020 2020 2073 656c 662e 616e 7469 6765       self.antige
+000078e0: 6e5f 6469 7370 6c61 7920 3d20 616e 7469  n_display = anti
+000078f0: 6765 6e5f 6469 7370 6c61 790a 2020 2020  gen_display.    
+00007900: 2020 2020 2020 2020 7365 6c66 2e61 6e74          self.ant
+00007910: 6967 656e 5f63 6f64 6520 3d20 616e 7469  igen_code = anti
+00007920: 6765 6e5f 636f 6465 0a20 2020 2020 2020  gen_code.       
+00007930: 2020 2020 2073 656c 662e 616e 7469 6765       self.antige
+00007940: 6e5f 6964 203d 2061 6e74 6967 656e 5f69  n_id = antigen_i
+00007950: 640a 2020 2020 2020 2020 616e 7469 6765  d.        antige
+00007960: 6e5f 636f 6465 6162 6c65 5f63 6f6e 6365  n_codeable_conce
+00007970: 7074 203d 2073 656c 662e 746f 5f63 6f64  pt = self.to_cod
+00007980: 6561 626c 655f 636f 6e63 6570 7428 0a20  eable_concept(. 
+00007990: 2020 2020 2020 2020 2020 2063 6f64 653d             code=
+000079a0: 7365 6c66 2e61 6e74 6967 656e 5f63 6f64  self.antigen_cod
+000079b0: 652c 0a20 2020 2020 2020 2020 2020 2064  e,.            d
+000079c0: 6973 706c 6179 3d73 656c 662e 616e 7469  isplay=self.anti
+000079d0: 6765 6e5f 6469 7370 6c61 792c 0a20 2020  gen_display,.   
+000079e0: 2020 2020 2020 2020 2069 643d 7365 6c66           id=self
+000079f0: 2e61 6e74 6967 656e 5f69 642c 0a20 2020  .antigen_id,.   
+00007a00: 2020 2020 2020 2020 2063 6f64 696e 675f           coding_
+00007a10: 7379 7374 656d 3d63 6f64 696e 675f 7379  system=coding_sy
+00007a20: 7374 656d 2c0a 2020 2020 2020 2020 2020  stem,.          
+00007a30: 2020 636f 6469 6e67 5f76 6572 7369 6f6e    coding_version
+00007a40: 3d63 6f64 696e 675f 7665 7273 696f 6e29  =coding_version)
+00007a50: 0a20 2020 2020 2020 2061 6e74 6967 656e  .        antigen
+00007a60: 5f65 7874 203d 2045 7874 656e 7369 6f6e  _ext = Extension
+00007a70: 2829 0a20 2020 2020 2020 2061 6e74 6967  ().        antig
+00007a80: 656e 5f65 7874 2e75 726c 203d 2027 616e  en_ext.url = 'an
+00007a90: 7469 6765 6e27 0a20 2020 2020 2020 2061  tigen'.        a
+00007aa0: 6e74 6967 656e 5f65 7874 2e76 616c 7565  ntigen_ext.value
+00007ab0: 436f 6465 6162 6c65 436f 6e63 6570 7420  CodeableConcept 
+00007ac0: 3d20 616e 7469 6765 6e5f 636f 6465 6162  = antigen_codeab
+00007ad0: 6c65 5f63 6f6e 6365 7074 0a20 2020 2020  le_concept.     
+00007ae0: 2020 2061 6e74 6967 656e 5f73 7461 7475     antigen_statu
+00007af0: 735f 6578 742e 6578 7465 6e73 696f 6e20  s_ext.extension 
+00007b00: 3d20 7375 7065 7228 292e 6164 645f 6f72  = super().add_or
+00007b10: 5f75 7064 6174 655f 6578 7465 6e73 696f  _update_extensio
+00007b20: 6e5f 746f 5f65 7874 656e 7369 6f6e 7328  n_to_extensions(
+00007b30: 6578 7465 6e73 696f 6e3d 616e 7469 6765  extension=antige
+00007b40: 6e5f 6578 742c 2065 7874 656e 7369 6f6e  n_ext, extension
+00007b50: 733d 616e 7469 6765 6e5f 7374 6174 7573  s=antigen_status
+00007b60: 5f65 7874 2e65 7874 656e 7369 6f6e 290a  _ext.extension).
+00007b70: 0a20 2020 2020 2020 2069 6620 646f 7365  .        if dose
+00007b80: 5f6e 756d 6265 7220 6973 206e 6f74 204e  _number is not N
+00007b90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007ba0: 2073 656c 662e 616e 7469 6765 6e5f 646f   self.antigen_do
+00007bb0: 7365 5f6e 756d 6265 7220 3d20 646f 7365  se_number = dose
+00007bc0: 5f6e 756d 6265 720a 2020 2020 2020 2020  _number.        
+00007bd0: 646f 7365 5f6e 756d 6265 725f 6578 7420  dose_number_ext 
+00007be0: 3d20 4578 7465 6e73 696f 6e28 290a 2020  = Extension().  
+00007bf0: 2020 2020 2020 646f 7365 5f6e 756d 6265        dose_numbe
+00007c00: 725f 6578 742e 7572 6c20 3d20 2764 6f73  r_ext.url = 'dos
+00007c10: 654e 756d 6265 7227 0a20 2020 2020 2020  eNumber'.       
+00007c20: 2064 6f73 655f 6e75 6d62 6572 5f65 7874   dose_number_ext
+00007c30: 2e76 616c 7565 496e 7465 6765 7220 3d20  .valueInteger = 
+00007c40: 7365 6c66 2e61 6e74 6967 656e 5f64 6f73  self.antigen_dos
+00007c50: 655f 6e75 6d62 6572 0a20 2020 2020 2020  e_number.       
+00007c60: 2061 6e74 6967 656e 5f73 7461 7475 735f   antigen_status_
+00007c70: 6578 742e 6578 7465 6e73 696f 6e20 3d20  ext.extension = 
+00007c80: 7375 7065 7228 292e 6164 645f 6f72 5f75  super().add_or_u
+00007c90: 7064 6174 655f 6578 7465 6e73 696f 6e5f  pdate_extension_
+00007ca0: 746f 5f65 7874 656e 7369 6f6e 7328 6578  to_extensions(ex
+00007cb0: 7465 6e73 696f 6e3d 646f 7365 5f6e 756d  tension=dose_num
+00007cc0: 6265 725f 6578 742c 2065 7874 656e 7369  ber_ext, extensi
+00007cd0: 6f6e 733d 616e 7469 6765 6e5f 7374 6174  ons=antigen_stat
+00007ce0: 7573 5f65 7874 2e65 7874 656e 7369 6f6e  us_ext.extension
+00007cf0: 290a 0a20 2020 2020 2020 2069 6620 7374  )..        if st
+00007d00: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
+00007d10: 204e 6f6e 6520 616e 6420 7374 6174 7573   None and status
+00007d20: 5f69 6420 6973 206e 6f74 204e 6f6e 6520  _id is not None 
+00007d30: 616e 6420 7374 6174 7573 5f64 6973 706c  and status_displ
+00007d40: 6179 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ay is not None:.
+00007d50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007d60: 2e61 6e74 6967 656e 5f73 7461 7475 735f  .antigen_status_
+00007d70: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00007d80: 6465 0a20 2020 2020 2020 2020 2020 2073  de.            s
+00007d90: 656c 662e 616e 7469 6765 6e5f 7374 6174  elf.antigen_stat
+00007da0: 7573 5f64 6973 706c 6179 203d 2073 7461  us_display = sta
+00007db0: 7475 735f 6469 7370 6c61 790a 2020 2020  tus_display.    
+00007dc0: 2020 2020 2020 2020 7365 6c66 2e61 6e74          self.ant
+00007dd0: 6967 656e 5f73 7461 7475 735f 6964 203d  igen_status_id =
+00007de0: 2073 7461 7475 735f 6964 0a20 2020 2020   status_id.     
+00007df0: 2020 2073 7461 7475 735f 636f 6465 6162     status_codeab
+00007e00: 6c65 5f63 6f6e 6365 7074 203d 2073 656c  le_concept = sel
+00007e10: 662e 746f 5f63 6f64 6561 626c 655f 636f  f.to_codeable_co
+00007e20: 6e63 6570 7428 0a20 2020 2020 2020 2020  ncept(.         
+00007e30: 2020 2063 6f64 6520 3d20 7365 6c66 2e61     code = self.a
+00007e40: 6e74 6967 656e 5f73 7461 7475 735f 636f  ntigen_status_co
+00007e50: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
+00007e60: 6964 203d 2073 656c 662e 616e 7469 6765  id = self.antige
+00007e70: 6e5f 7374 6174 7573 5f69 642c 0a20 2020  n_status_id,.   
+00007e80: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00007e90: 3d73 656c 662e 616e 7469 6765 6e5f 7374  =self.antigen_st
+00007ea0: 6174 7573 5f64 6973 706c 6179 2c0a 2020  atus_display,.  
+00007eb0: 2020 2020 2020 2020 2020 636f 6469 6e67            coding
+00007ec0: 5f73 7973 7465 6d3d 636f 6469 6e67 5f73  _system=coding_s
+00007ed0: 7973 7465 6d2c 0a20 2020 2020 2020 2020  ystem,.         
+00007ee0: 2020 2063 6f64 696e 675f 7665 7273 696f     coding_versio
+00007ef0: 6e3d 636f 6469 6e67 5f76 6572 7369 6f6e  n=coding_version
+00007f00: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00007f10: 2020 2073 7461 7475 735f 6578 7420 3d20     status_ext = 
+00007f20: 4578 7465 6e73 696f 6e28 290a 2020 2020  Extension().    
+00007f30: 2020 2020 7374 6174 7573 5f65 7874 2e75      status_ext.u
+00007f40: 726c 203d 2027 7374 6174 7573 270a 2020  rl = 'status'.  
+00007f50: 2020 2020 2020 7374 6174 7573 5f65 7874        status_ext
+00007f60: 2e76 616c 7565 436f 6465 6162 6c65 436f  .valueCodeableCo
+00007f70: 6e63 6570 7420 3d20 7374 6174 7573 5f63  ncept = status_c
+00007f80: 6f64 6561 626c 655f 636f 6e63 6570 740a  odeable_concept.
+00007f90: 2020 2020 2020 2020 616e 7469 6765 6e5f          antigen_
+00007fa0: 7374 6174 7573 5f65 7874 2e65 7874 656e  status_ext.exten
+00007fb0: 7369 6f6e 203d 2073 7570 6572 2829 2e61  sion = super().a
+00007fc0: 6464 5f6f 725f 7570 6461 7465 5f65 7874  dd_or_update_ext
+00007fd0: 656e 7369 6f6e 5f74 6f5f 6578 7465 6e73  ension_to_extens
+00007fe0: 696f 6e73 2865 7874 656e 7369 6f6e 3d73  ions(extension=s
+00007ff0: 7461 7475 735f 6578 742c 2065 7874 656e  tatus_ext, exten
+00008000: 7369 6f6e 733d 616e 7469 6765 6e5f 7374  sions=antigen_st
+00008010: 6174 7573 5f65 7874 2e65 7874 656e 7369  atus_ext.extensi
+00008020: 6f6e 290a 0a20 2020 2020 2020 2069 6d6d  on)..        imm
+00008030: 756e 697a 6174 696f 6e2e 6578 7465 6e73  unization.extens
+00008040: 696f 6e20 3d20 7375 7065 7228 292e 6164  ion = super().ad
+00008050: 645f 6f72 5f75 7064 6174 655f 6578 7465  d_or_update_exte
+00008060: 6e73 696f 6e5f 746f 5f65 7874 656e 7369  nsion_to_extensi
+00008070: 6f6e 7328 6578 7465 6e73 696f 6e3d 616e  ons(extension=an
+00008080: 7469 6765 6e5f 7374 6174 7573 5f65 7874  tigen_status_ext
+00008090: 2c20 6578 7465 6e73 696f 6e73 3d69 6d6d  , extensions=imm
+000080a0: 756e 697a 6174 696f 6e2e 6578 7465 6e73  unization.extens
+000080b0: 696f 6e29 0a0a 2020 2020 6465 6620 6765  ion)..    def ge
+000080c0: 745f 616e 7469 6765 6e5f 7374 6174 7573  t_antigen_status
+000080d0: 2873 656c 662c 2069 6d6d 756e 697a 6174  (self, immunizat
+000080e0: 696f 6e3d 4e6f 6e65 293a 0a20 2020 2020  ion=None):.     
+000080f0: 2020 2069 6620 696d 6d75 6e69 7a61 7469     if immunizati
+00008100: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00008110: 2020 2020 2020 2020 696d 6d75 6e69 7a61          immuniza
+00008120: 7469 6f6e 203d 2073 656c 662e 6668 6972  tion = self.fhir
+00008130: 5f72 6573 6f75 7263 650a 2020 2020 2020  _resource.      
+00008140: 2020 616e 7469 6765 6e5f 7374 6174 7573    antigen_status
+00008150: 5f65 7874 656e 7369 6f6e 203d 204e 6f6e  _extension = Non
+00008160: 650a 2020 2020 2020 2020 6966 2069 6d6d  e.        if imm
+00008170: 756e 697a 6174 696f 6e2e 6578 7465 6e73  unization.extens
+00008180: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+00008190: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000081a0: 2065 7874 2069 6e20 696d 6d75 6e69 7a61   ext in immuniza
+000081b0: 7469 6f6e 2e65 7874 656e 7369 6f6e 3a0a  tion.extension:.
+000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081d0: 6966 2065 7874 2e75 726c 203d 3d20 7365  if ext.url == se
+000081e0: 6c66 2e61 6e74 6967 656e 5f73 7461 7475  lf.antigen_statu
+000081f0: 735f 7572 6c3a 0a20 2020 2020 2020 2020  s_url:.         
+00008200: 2020 2020 2020 2020 2020 2061 6e74 6967             antig
+00008210: 656e 5f73 7461 7475 735f 6578 7465 6e73  en_status_extens
+00008220: 696f 6e20 3d20 6578 740a 2020 2020 2020  ion = ext.      
+00008230: 2020 7265 7475 726e 2061 6e74 6967 656e    return antigen
+00008240: 5f73 7461 7475 735f 6578 7465 6e73 696f  _status_extensio
+00008250: 6e0a 0a20 2020 2064 6566 2067 6574 5f61  n..    def get_a
+00008260: 6e74 6967 656e 5f73 7461 7475 735f 616e  ntigen_status_an
+00008270: 7469 6765 6e28 7365 6c66 2c20 696d 6d75  tigen(self, immu
+00008280: 6e69 7a61 7469 6f6e 3d4e 6f6e 6529 3a0a  nization=None):.
+00008290: 2020 2020 2020 2020 616e 7469 6765 6e5f          antigen_
+000082a0: 7374 6174 7573 5f65 7874 656e 7369 6f6e  status_extension
+000082b0: 203d 2073 656c 662e 6765 745f 616e 7469   = self.get_anti
+000082c0: 6765 6e5f 7374 6174 7573 2869 6d6d 756e  gen_status(immun
+000082d0: 697a 6174 696f 6e3d 696d 6d75 6e69 7a61  ization=immuniza
+000082e0: 7469 6f6e 290a 2020 2020 2020 2020 616e  tion).        an
+000082f0: 7469 6765 6e5f 6578 7465 6e73 696f 6e20  tigen_extension 
+00008300: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+00008310: 6620 616e 7469 6765 6e5f 7374 6174 7573  f antigen_status
+00008320: 5f65 7874 656e 7369 6f6e 2069 7320 6e6f  _extension is no
+00008330: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00008340: 2020 2020 666f 7220 616e 7469 6765 6e5f      for antigen_
+00008350: 6578 7465 6e73 696f 6e20 696e 2061 6e74  extension in ant
+00008360: 6967 656e 5f73 7461 7475 735f 6578 7465  igen_status_exte
+00008370: 6e73 696f 6e2e 6578 7465 6e73 696f 6e3a  nsion.extension:
+00008380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008390: 2069 6620 616e 7469 6765 6e5f 6578 7465   if antigen_exte
+000083a0: 6e73 696f 6e2e 7572 6c20 3d3d 2027 616e  nsion.url == 'an
+000083b0: 7469 6765 6e27 3a0a 2020 2020 2020 2020  tigen':.        
+000083c0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+000083d0: 6b0a 2020 2020 2020 2020 7265 7475 726e  k.        return
+000083e0: 2061 6e74 6967 656e 5f65 7874 656e 7369   antigen_extensi
+000083f0: 6f6e 0a0a 2020 2020 6465 6620 6765 745f  on..    def get_
+00008400: 616e 7469 6765 6e5f 7374 6174 7573 5f64  antigen_status_d
+00008410: 6f73 655f 6e75 6d62 6572 2873 656c 662c  ose_number(self,
+00008420: 2069 6d6d 756e 697a 6174 696f 6e3d 4e6f   immunization=No
+00008430: 6e65 293a 0a20 2020 2020 2020 2061 6e74  ne):.        ant
+00008440: 6967 656e 5f73 7461 7475 735f 6578 7465  igen_status_exte
+00008450: 6e73 696f 6e20 3d20 7365 6c66 2e67 6574  nsion = self.get
+00008460: 5f61 6e74 6967 656e 5f73 7461 7475 7328  _antigen_status(
+00008470: 696d 6d75 6e69 7a61 7469 6f6e 3d69 6d6d  immunization=imm
+00008480: 756e 697a 6174 696f 6e29 0a20 2020 2020  unization).     
+00008490: 2020 2061 6e74 6967 656e 5f65 7874 656e     antigen_exten
+000084a0: 7369 6f6e 203d 204e 6f6e 650a 2020 2020  sion = None.    
+000084b0: 2020 2020 6966 2061 6e74 6967 656e 5f73      if antigen_s
+000084c0: 7461 7475 735f 6578 7465 6e73 696f 6e20  tatus_extension 
+000084d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000084e0: 2020 2020 2020 2020 2066 6f72 2061 6e74           for ant
+000084f0: 6967 656e 5f65 7874 656e 7369 6f6e 2069  igen_extension i
+00008500: 6e20 616e 7469 6765 6e5f 7374 6174 7573  n antigen_status
+00008510: 5f65 7874 656e 7369 6f6e 2e65 7874 656e  _extension.exten
+00008520: 7369 6f6e 3a0a 2020 2020 2020 2020 2020  sion:.          
+00008530: 2020 2020 2020 6966 2061 6e74 6967 656e        if antigen
+00008540: 5f65 7874 656e 7369 6f6e 2e75 726c 203d  _extension.url =
+00008550: 3d20 2764 6f73 654e 756d 6265 7227 3a0a  = 'doseNumber':.
+00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008570: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00008580: 2020 7265 7475 726e 2061 6e74 6967 656e    return antigen
+00008590: 5f65 7874 656e 7369 6f6e 0a0a 2020 2020  _extension..    
+000085a0: 6465 6620 6765 745f 616e 7469 6765 6e5f  def get_antigen_
+000085b0: 7374 6174 7573 5f73 7461 7475 7328 7365  status_status(se
+000085c0: 6c66 2c20 696d 6d75 6e69 7a61 7469 6f6e  lf, immunization
+000085d0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+000085e0: 616e 7469 6765 6e5f 7374 6174 7573 5f65  antigen_status_e
+000085f0: 7874 656e 7369 6f6e 203d 2073 656c 662e  xtension = self.
+00008600: 6765 745f 616e 7469 6765 6e5f 7374 6174  get_antigen_stat
+00008610: 7573 2869 6d6d 756e 697a 6174 696f 6e3d  us(immunization=
+00008620: 696d 6d75 6e69 7a61 7469 6f6e 290a 2020  immunization).  
+00008630: 2020 2020 2020 616e 7469 6765 6e5f 6578        antigen_ex
+00008640: 7465 6e73 696f 6e20 3d20 4e6f 6e65 0a20  tension = None. 
+00008650: 2020 2020 2020 2069 6620 616e 7469 6765         if antige
+00008660: 6e5f 7374 6174 7573 5f65 7874 656e 7369  n_status_extensi
+00008670: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
+00008680: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00008690: 616e 7469 6765 6e5f 6578 7465 6e73 696f  antigen_extensio
+000086a0: 6e20 696e 2061 6e74 6967 656e 5f73 7461  n in antigen_sta
+000086b0: 7475 735f 6578 7465 6e73 696f 6e2e 6578  tus_extension.ex
+000086c0: 7465 6e73 696f 6e3a 0a20 2020 2020 2020  tension:.       
+000086d0: 2020 2020 2020 2020 2069 6620 616e 7469           if anti
+000086e0: 6765 6e5f 6578 7465 6e73 696f 6e2e 7572  gen_extension.ur
+000086f0: 6c20 3d3d 2027 7374 6174 7573 273a 0a20  l == 'status':. 
+00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008710: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00008720: 2072 6574 7572 6e20 616e 7469 6765 6e5f   return antigen_
+00008730: 6578 7465 6e73 696f 6e0a 0a20 2020 2064  extension..    d
+00008740: 6566 2067 6574 5f63 6f64 6561 626c 655f  ef get_codeable_
+00008750: 636f 6e63 6570 745f 636f 6469 6e67 2873  concept_coding(s
+00008760: 656c 662c 2063 6f64 6561 626c 655f 636f  elf, codeable_co
+00008770: 6e63 6570 743d 4e6f 6e65 2c20 636f 6469  ncept=None, codi
+00008780: 6e67 5f73 7973 7465 6d3d 4e6f 6e65 2c20  ng_system=None, 
+00008790: 636f 6469 6e67 5f76 6572 7369 6f6e 3d4e  coding_version=N
+000087a0: 6f6e 6529 3a0a 2020 2020 2020 2020 636f  one):.        co
+000087b0: 6469 6e67 5f73 7973 7465 6d20 3d20 636f  ding_system = co
+000087c0: 6469 6e67 5f73 7973 7465 6d20 6966 2063  ding_system if c
+000087d0: 6f64 696e 675f 7379 7374 656d 2069 7320  oding_system is 
+000087e0: 6e6f 7420 4e6f 6e65 2065 6c73 6520 7365  not None else se
+000087f0: 6c66 2e63 6f64 696e 675f 7379 7374 656d  lf.coding_system
+00008800: 0a20 2020 2020 2020 2063 6f64 696e 675f  .        coding_
+00008810: 7665 7273 696f 6e20 3d20 636f 6469 6e67  version = coding
+00008820: 5f76 6572 7369 6f6e 2069 6620 636f 6469  _version if codi
+00008830: 6e67 5f76 6572 7369 6f6e 2069 7320 6e6f  ng_version is no
+00008840: 7420 4e6f 6e65 2065 6c73 6520 7365 6c66  t None else self
+00008850: 2e63 6f64 696e 675f 7665 7273 696f 6e0a  .coding_version.
+00008860: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008870: 2063 6f64 696e 6720 3d20 4e6f 6e65 0a20   coding = None. 
+00008880: 2020 2020 2020 2069 6620 636f 6465 6162         if codeab
+00008890: 6c65 5f63 6f6e 6365 7074 2069 7320 6e6f  le_concept is no
+000088a0: 7420 4e6f 6e65 2061 6e64 2063 6f64 6561  t None and codea
+000088b0: 626c 655f 636f 6e63 6570 742e 636f 6469  ble_concept.codi
+000088c0: 6e67 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ng is not None:.
+000088d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000088e0: 636f 6469 6e67 2069 6e20 636f 6465 6162  coding in codeab
+000088f0: 6c65 5f63 6f6e 6365 7074 2e63 6f64 696e  le_concept.codin
+00008900: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
+00008910: 2020 2069 6620 636f 6469 6e67 2e73 7973     if coding.sys
+00008920: 7465 6d20 3d3d 2063 6f64 696e 675f 7379  tem == coding_sy
+00008930: 7374 656d 2061 6e64 2063 6f64 696e 672e  stem and coding.
+00008940: 7665 7273 696f 6e20 3d3d 2063 6f64 696e  version == codin
+00008950: 675f 7665 7273 696f 6e3a 0a20 2020 2020  g_version:.     
+00008960: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00008970: 7265 616b 0a20 2020 2020 2020 2072 6574  reak.        ret
+00008980: 7572 6e20 636f 6469 6e67 0a20 2020 200a  urn coding.    .
+00008990: 2020 2020 6465 6620 746f 5f63 6f64 6561      def to_codea
+000089a0: 626c 655f 636f 6e63 6570 7428 7365 6c66  ble_concept(self
+000089b0: 2c20 636f 6465 3d4e 6f6e 652c 2064 6973  , code=None, dis
+000089c0: 706c 6179 3d4e 6f6e 652c 2069 643d 4e6f  play=None, id=No
+000089d0: 6e65 2c20 636f 6469 6e67 5f73 7973 7465  ne, coding_syste
+000089e0: 6d3d 4e6f 6e65 2c20 636f 6469 6e67 5f76  m=None, coding_v
+000089f0: 6572 7369 6f6e 3d4e 6f6e 6529 3a0a 2020  ersion=None):.  
+00008a00: 2020 2020 2020 636f 6469 6e67 5f73 7973        coding_sys
+00008a10: 7465 6d20 3d20 636f 6469 6e67 5f73 7973  tem = coding_sys
+00008a20: 7465 6d20 6966 2063 6f64 696e 675f 7379  tem if coding_sy
+00008a30: 7374 656d 2069 7320 6e6f 7420 4e6f 6e65  stem is not None
+00008a40: 2065 6c73 6520 7365 6c66 2e63 6f64 696e   else self.codin
+00008a50: 675f 7379 7374 656d 0a20 2020 2020 2020  g_system.       
+00008a60: 2063 6f64 696e 675f 7665 7273 696f 6e20   coding_version 
+00008a70: 3d20 636f 6469 6e67 5f76 6572 7369 6f6e  = coding_version
+00008a80: 2069 6620 636f 6469 6e67 5f76 6572 7369   if coding_versi
+00008a90: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 2065  on is not None e
+00008aa0: 6c73 6520 7365 6c66 2e63 6f64 696e 675f  lse self.coding_
+00008ab0: 7665 7273 696f 6e0a 2020 2020 2020 2020  version.        
+00008ac0: 636f 6469 6e67 203d 2043 6f64 696e 6728  coding = Coding(
+00008ad0: 290a 2020 2020 2020 2020 636f 6469 6e67  ).        coding
+00008ae0: 2e63 6f64 6520 3d20 636f 6465 0a20 2020  .code = code.   
+00008af0: 2020 2020 2063 6f64 696e 672e 6469 7370       coding.disp
+00008b00: 6c61 7920 3d20 6469 7370 6c61 790a 2020  lay = display.  
+00008b10: 2020 2020 2020 636f 6469 6e67 2e69 6420        coding.id 
+00008b20: 3d20 6964 0a20 2020 2020 2020 2063 6f64  = id.        cod
+00008b30: 696e 672e 7665 7273 696f 6e20 3d20 636f  ing.version = co
+00008b40: 6469 6e67 5f73 7973 7465 6d0a 2020 2020  ding_system.    
+00008b50: 2020 2020 636f 6469 6e67 2e73 7973 7465      coding.syste
+00008b60: 6d20 3d20 636f 6469 6e67 5f73 7973 7465  m = coding_syste
+00008b70: 6d0a 2020 2020 2020 2020 636f 6465 6162  m.        codeab
+00008b80: 6c65 5f63 6f6e 6365 7074 203d 2043 6f64  le_concept = Cod
+00008b90: 6561 626c 6543 6f6e 6365 7074 2829 0a20  eableConcept(). 
+00008ba0: 2020 2020 2020 2063 6f64 6561 626c 655f         codeable_
+00008bb0: 636f 6e63 6570 742e 636f 6469 6e67 203d  concept.coding =
+00008bc0: 205b 636f 6469 6e67 5d0a 2020 2020 2020   [coding].      
+00008bd0: 2020 7265 7475 726e 2063 6f64 6561 626c    return codeabl
+00008be0: 655f 636f 6e63 6570 740a 0a20 2020 2064  e_concept..    d
+00008bf0: 6566 2067 6574 5f6c 6f74 5f69 6428 7365  ef get_lot_id(se
+00008c00: 6c66 2c20 696d 6d75 6e69 7a61 7469 6f6e  lf, immunization
+00008c10: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00008c20: 6966 2069 6d6d 756e 697a 6174 696f 6e20  if immunization 
+00008c30: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00008c40: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
+00008c50: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
+00008c60: 736f 7572 6365 0a20 2020 2020 2020 2069  source.        i
+00008c70: 6620 696d 6d75 6e69 7a61 7469 6f6e 2069  f immunization i
+00008c80: 7320 4e6f 6e65 206f 7220 696d 6d75 6e69  s None or immuni
+00008c90: 7a61 7469 6f6e 2e65 7874 656e 7369 6f6e  zation.extension
+00008ca0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00008cb0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00008cc0: 650a 2020 2020 2020 2020 6c6f 745f 6964  e.        lot_id
+00008cd0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00008ce0: 666f 7220 6578 7465 6e73 696f 6e20 696e  for extension in
+00008cf0: 2069 6d6d 756e 697a 6174 696f 6e2e 6578   immunization.ex
+00008d00: 7465 6e73 696f 6e3a 0a20 2020 2020 2020  tension:.       
+00008d10: 2020 2020 2069 6620 6578 7465 6e73 696f       if extensio
+00008d20: 6e2e 7572 6c20 3d3d 2073 656c 662e 6c6f  n.url == self.lo
+00008d30: 745f 6964 5f75 726c 3a0a 2020 2020 2020  t_id_url:.      
+00008d40: 2020 2020 2020 2020 2020 6c6f 745f 6964            lot_id
+00008d50: 203d 2065 7874 656e 7369 6f6e 2e76 616c   = extension.val
+00008d60: 7565 5374 7269 6e67 0a20 2020 2020 2020  ueString.       
+00008d70: 2072 6574 7572 6e20 6c6f 745f 6964 0a20   return lot_id. 
+00008d80: 2020 200a 2020 2020 6465 6620 7365 745f     .    def set_
+00008d90: 6c6f 745f 6964 2873 656c 662c 2069 6d6d  lot_id(self, imm
+00008da0: 756e 697a 6174 696f 6e3d 4e6f 6e65 2c20  unization=None, 
+00008db0: 6c6f 745f 6964 3d4e 6f6e 6529 3a0a 2020  lot_id=None):.  
+00008dc0: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
+00008dd0: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
+00008de0: 2020 2020 2020 2020 2020 2069 6d6d 756e             immun
+00008df0: 697a 6174 696f 6e20 3d20 7365 6c66 2e66  ization = self.f
+00008e00: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
+00008e10: 2020 2020 2069 6620 6c6f 745f 6964 2069       if lot_id i
+00008e20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00008e30: 2020 2020 2020 2020 7365 6c66 2e6c 6f74          self.lot
+00008e40: 5f69 6420 3d20 6c6f 745f 6964 0a20 2020  _id = lot_id.   
+00008e50: 2020 2020 206c 6f74 5f69 645f 6578 7420       lot_id_ext 
+00008e60: 3d20 4578 7465 6e73 696f 6e28 290a 2020  = Extension().  
+00008e70: 2020 2020 2020 6c6f 745f 6964 5f65 7874        lot_id_ext
+00008e80: 2e75 726c 203d 2073 656c 662e 6c6f 745f  .url = self.lot_
+00008e90: 6964 5f75 726c 0a20 2020 2020 2020 206c  id_url.        l
+00008ea0: 6f74 5f69 645f 6578 742e 7661 6c75 6553  ot_id_ext.valueS
+00008eb0: 7472 696e 6720 3d20 7365 6c66 2e6c 6f74  tring = self.lot
+00008ec0: 5f69 640a 2020 2020 2020 2020 696d 6d75  _id.        immu
+00008ed0: 6e69 7a61 7469 6f6e 2e65 7874 656e 7369  nization.extensi
+00008ee0: 6f6e 203d 2073 7570 6572 2829 2e61 6464  on = super().add
+00008ef0: 5f6f 725f 7570 6461 7465 5f65 7874 656e  _or_update_exten
+00008f00: 7369 6f6e 5f74 6f5f 6578 7465 6e73 696f  sion_to_extensio
+00008f10: 6e73 2865 7874 656e 7369 6f6e 3d6c 6f74  ns(extension=lot
+00008f20: 5f69 645f 6578 742c 2065 7874 656e 7369  _id_ext, extensi
+00008f30: 6f6e 733d 696d 6d75 6e69 7a61 7469 6f6e  ons=immunization
+00008f40: 2e65 7874 656e 7369 6f6e 290a 0a20 2020  .extension)..   
+00008f50: 2064 6566 2067 6574 5f74 7261 6465 5f6e   def get_trade_n
+00008f60: 616d 6528 7365 6c66 2c20 696d 6d75 6e69  ame(self, immuni
+00008f70: 7a61 7469 6f6e 3d4e 6f6e 6529 3a0a 2020  zation=None):.  
+00008f80: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
+00008f90: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
+00008fa0: 2020 2020 2020 2020 2020 2069 6d6d 756e             immun
+00008fb0: 697a 6174 696f 6e20 3d20 7365 6c66 2e66  ization = self.f
+00008fc0: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
+00008fd0: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
+00008fe0: 7469 6f6e 2069 7320 4e6f 6e65 206f 7220  tion is None or 
+00008ff0: 696d 6d75 6e69 7a61 7469 6f6e 2e65 7874  immunization.ext
+00009000: 656e 7369 6f6e 2069 7320 4e6f 6e65 3a0a  ension is None:.
+00009010: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009020: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
+00009030: 7472 6164 655f 6e61 6d65 203d 204e 6f6e  trade_name = Non
+00009040: 650a 2020 2020 2020 2020 666f 7220 6578  e.        for ex
+00009050: 7465 6e73 696f 6e20 696e 2069 6d6d 756e  tension in immun
+00009060: 697a 6174 696f 6e2e 6578 7465 6e73 696f  ization.extensio
+00009070: 6e3a 0a20 2020 2020 2020 2020 2020 2069  n:.            i
+00009080: 6620 6578 7465 6e73 696f 6e2e 7572 6c20  f extension.url 
+00009090: 3d3d 2073 656c 662e 7472 6164 655f 6e61  == self.trade_na
+000090a0: 6d65 5f75 726c 3a0a 2020 2020 2020 2020  me_url:.        
+000090b0: 2020 2020 2020 2020 7472 6164 655f 6e61          trade_na
+000090c0: 6d65 203d 2065 7874 656e 7369 6f6e 2e76  me = extension.v
+000090d0: 616c 7565 5374 7269 6e67 0a20 2020 2020  alueString.     
+000090e0: 2020 2072 6574 7572 6e20 7472 6164 655f     return trade_
+000090f0: 6e61 6d65 0a0a 2020 2020 6465 6620 7365  name..    def se
+00009100: 745f 7472 6164 655f 6e61 6d65 2873 656c  t_trade_name(sel
+00009110: 662c 2069 6d6d 756e 697a 6174 696f 6e3d  f, immunization=
+00009120: 4e6f 6e65 2c20 7472 6164 655f 6e61 6d65  None, trade_name
+00009130: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00009140: 6966 2069 6d6d 756e 697a 6174 696f 6e20  if immunization 
+00009150: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00009160: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
+00009170: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
+00009180: 736f 7572 6365 0a20 2020 2020 2020 2069  source.        i
+00009190: 6620 7472 6164 655f 6e61 6d65 2069 7320  f trade_name is 
+000091a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000091b0: 2020 2020 2020 7365 6c66 2e74 7261 6465        self.trade
+000091c0: 5f6e 616d 6520 3d20 7472 6164 655f 6e61  _name = trade_na
+000091d0: 6d65 0a20 2020 2020 2020 2074 7261 6465  me.        trade
+000091e0: 5f6e 616d 655f 6578 7420 3d20 4578 7465  _name_ext = Exte
+000091f0: 6e73 696f 6e28 290a 2020 2020 2020 2020  nsion().        
+00009200: 7472 6164 655f 6e61 6d65 5f65 7874 2e75  trade_name_ext.u
+00009210: 726c 203d 2073 656c 662e 7472 6164 655f  rl = self.trade_
+00009220: 6e61 6d65 5f75 726c 0a20 2020 2020 2020  name_url.       
+00009230: 2074 7261 6465 5f6e 616d 655f 6578 742e   trade_name_ext.
+00009240: 7661 6c75 6553 7472 696e 6720 3d20 7365  valueString = se
+00009250: 6c66 2e74 7261 6465 5f6e 616d 650a 2020  lf.trade_name.  
+00009260: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
+00009270: 6f6e 2e65 7874 656e 7369 6f6e 203d 2073  on.extension = s
+00009280: 7570 6572 2829 2e61 6464 5f6f 725f 7570  uper().add_or_up
+00009290: 6461 7465 5f65 7874 656e 7369 6f6e 5f74  date_extension_t
+000092a0: 6f5f 6578 7465 6e73 696f 6e73 2865 7874  o_extensions(ext
+000092b0: 656e 7369 6f6e 3d74 7261 6465 5f6e 616d  ension=trade_nam
+000092c0: 655f 6578 742c 2065 7874 656e 7369 6f6e  e_ext, extension
+000092d0: 733d 696d 6d75 6e69 7a61 7469 6f6e 2e65  s=immunization.e
+000092e0: 7874 656e 7369 6f6e 290a 0a20 2020 2064  xtension)..    d
+000092f0: 6566 2067 6574 5f63 6f6e 7461 696e 6564  ef get_contained
+00009300: 5f6f 7267 616e 697a 6174 696f 6e28 7365  _organization(se
+00009310: 6c66 2c20 696d 6d75 6e69 7a61 7469 6f6e  lf, immunization
+00009320: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00009330: 6966 2069 6d6d 756e 697a 6174 696f 6e20  if immunization 
+00009340: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00009350: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
+00009360: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
+00009370: 736f 7572 6365 0a20 2020 2020 2020 2069  source.        i
+00009380: 6620 696d 6d75 6e69 7a61 7469 6f6e 2e63  f immunization.c
+00009390: 6f6e 7461 696e 6564 2069 7320 6e6f 7420  ontained is not 
+000093a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000093b0: 2020 666f 7220 636f 6e74 6169 6e65 6420    for contained 
+000093c0: 696e 2069 6d6d 756e 697a 6174 696f 6e2e  in immunization.
+000093d0: 636f 6e74 6169 6e65 643a 0a20 2020 2020  contained:.     
+000093e0: 2020 2020 2020 2020 2020 2069 6620 7479             if ty
+000093f0: 7065 2863 6f6e 7461 696e 6564 2920 6973  pe(contained) is
+00009400: 204f 7267 616e 697a 6174 696f 6e3a 0a20   Organization:. 
+00009410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009420: 2020 2072 6574 7572 6e20 636f 6e74 6169     return contai
+00009430: 6e65 640a 2020 2020 2020 2020 7265 7475  ned.        retu
+00009440: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
+00009450: 2073 6574 5f63 6f6e 7461 696e 6564 5f6f   set_contained_o
+00009460: 7267 616e 697a 6174 696f 6e28 7365 6c66  rganization(self
+00009470: 2c20 696d 6d75 6e69 7a61 7469 6f6e 3d4e  , immunization=N
+00009480: 6f6e 652c 206f 7267 616e 697a 6174 696f  one, organizatio
+00009490: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
+000094a0: 2069 6620 696d 6d75 6e69 7a61 7469 6f6e   if immunization
+000094b0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000094c0: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
+000094d0: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
+000094e0: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
+000094f0: 6966 206f 7267 616e 697a 6174 696f 6e20  if organization 
+00009500: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00009510: 2020 2020 2020 2020 2073 656c 662e 6f72           self.or
+00009520: 6761 6e69 7a61 7469 6f6e 203d 206f 7267  ganization = org
+00009530: 616e 697a 6174 696f 6e0a 2020 2020 2020  anization.      
+00009540: 2020 636f 6e74 6169 6e65 645f 6f72 6761    contained_orga
+00009550: 6e69 7a61 7469 6f6e 203d 204e 6f6e 650a  nization = None.
+00009560: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+00009570: 7365 6c66 2e6f 7267 616e 697a 6174 696f  self.organizatio
+00009580: 6e29 2069 7320 6469 6374 3a0a 2020 2020  n) is dict:.    
+00009590: 2020 2020 2020 2020 636f 6e74 6169 6e65          containe
+000095a0: 645f 6f72 6761 6e69 7a61 7469 6f6e 203d  d_organization =
+000095b0: 204f 7267 616e 697a 6174 696f 6e28 6a73   Organization(js
+000095c0: 6f6e 6469 6374 3d73 656c 662e 6f72 6761  ondict=self.orga
+000095d0: 6e69 7a61 7469 6f6e 290a 2020 2020 2020  nization).      
+000095e0: 2020 656c 6966 2074 7970 6528 7365 6c66    elif type(self
+000095f0: 2e6f 7267 616e 697a 6174 696f 6e29 2069  .organization) i
+00009600: 7320 4f72 6761 6e69 7a61 7469 6f6e 3a0a  s Organization:.
 00009610: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
 00009620: 6169 6e65 645f 6f72 6761 6e69 7a61 7469  ained_organizati
-00009630: 6f6e 203d 204f 7267 616e 697a 6174 696f  on = Organizatio
-00009640: 6e28 6a73 6f6e 6469 6374 3d73 656c 662e  n(jsondict=self.
-00009650: 6f72 6761 6e69 7a61 7469 6f6e 290a 2020  organization).  
-00009660: 2020 2020 2020 656c 6966 2074 7970 6528        elif type(
-00009670: 7365 6c66 2e6f 7267 616e 697a 6174 696f  self.organizatio
-00009680: 6e29 2069 7320 4f72 6761 6e69 7a61 7469  n) is Organizati
-00009690: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-000096a0: 636f 6e74 6169 6e65 645f 6f72 6761 6e69  contained_organi
-000096b0: 7a61 7469 6f6e 203d 2073 656c 662e 6f72  zation = self.or
-000096c0: 6761 6e69 7a61 7469 6f6e 0a20 2020 2020  ganization.     
-000096d0: 2020 2069 6620 636f 6e74 6169 6e65 645f     if contained_
-000096e0: 6f72 6761 6e69 7a61 7469 6f6e 2069 7320  organization is 
-000096f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00009700: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
-00009710: 6174 696f 6e2e 636f 6e74 6169 6e65 6420  ation.contained 
-00009720: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00009730: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
-00009740: 6174 696f 6e2e 636f 6e74 6169 6e65 6420  ation.contained 
-00009750: 3d20 5b63 6f6e 7461 696e 6564 5f6f 7267  = [contained_org
-00009760: 616e 697a 6174 696f 6e5d 0a20 2020 2020  anization].     
-00009770: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00009780: 2020 2020 2020 2020 2020 2020 206f 7267               org
-00009790: 5f66 6f75 6e64 203d 2046 616c 7365 0a20  _found = False. 
-000097a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000097b0: 6f72 2063 6f6e 7461 696e 6564 2069 6e20  or contained in 
-000097c0: 696d 6d75 6e69 7a61 7469 6f6e 2e63 6f6e  immunization.con
-000097d0: 7461 696e 6564 3a0a 2020 2020 2020 2020  tained:.        
-000097e0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-000097f0: 7970 6528 636f 6e74 6169 6e65 6429 2069  ype(contained) i
-00009800: 7320 4f72 6761 6e69 7a61 7469 6f6e 3a0a  s Organization:.
+00009630: 6f6e 203d 2073 656c 662e 6f72 6761 6e69  on = self.organi
+00009640: 7a61 7469 6f6e 0a20 2020 2020 2020 2069  zation.        i
+00009650: 6620 636f 6e74 6169 6e65 645f 6f72 6761  f contained_orga
+00009660: 6e69 7a61 7469 6f6e 2069 7320 6e6f 7420  nization is not 
+00009670: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00009680: 2020 6966 2069 6d6d 756e 697a 6174 696f    if immunizatio
+00009690: 6e2e 636f 6e74 6169 6e65 6420 6973 204e  n.contained is N
+000096a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000096b0: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
+000096c0: 6e2e 636f 6e74 6169 6e65 6420 3d20 5b63  n.contained = [c
+000096d0: 6f6e 7461 696e 6564 5f6f 7267 616e 697a  ontained_organiz
+000096e0: 6174 696f 6e5d 0a20 2020 2020 2020 2020  ation].         
+000096f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00009700: 2020 2020 2020 2020 206f 7267 5f66 6f75           org_fou
+00009710: 6e64 203d 2046 616c 7365 0a20 2020 2020  nd = False.     
+00009720: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00009730: 6f6e 7461 696e 6564 2069 6e20 696d 6d75  ontained in immu
+00009740: 6e69 7a61 7469 6f6e 2e63 6f6e 7461 696e  nization.contain
+00009750: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+00009760: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+00009770: 636f 6e74 6169 6e65 6429 2069 7320 4f72  contained) is Or
+00009780: 6761 6e69 7a61 7469 6f6e 3a0a 2020 2020  ganization:.    
+00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097a0: 2020 2020 636f 6e74 6169 6e65 6420 3d20      contained = 
+000097b0: 7365 6c66 2e6f 7267 616e 697a 6174 696f  self.organizatio
+000097c0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000097d0: 2020 2020 2020 2020 2020 6f72 675f 666f            org_fo
+000097e0: 756e 6420 3d20 5472 7565 0a20 2020 2020  und = True.     
+000097f0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00009800: 7420 6f72 675f 666f 756e 643a 0a20 2020  t org_found:.   
 00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009820: 2020 2020 2020 2020 636f 6e74 6169 6e65          containe
-00009830: 6420 3d20 7365 6c66 2e6f 7267 616e 697a  d = self.organiz
-00009840: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
-00009850: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-00009860: 675f 666f 756e 6420 3d20 5472 7565 0a20  g_found = True. 
-00009870: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00009880: 6620 6e6f 7420 6f72 675f 666f 756e 643a  f not org_found:
-00009890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000098a0: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
-000098b0: 6e2e 636f 6e74 6169 6e65 642e 6170 7065  n.contained.appe
-000098c0: 6e64 2873 656c 662e 6f72 6761 6e69 7a61  nd(self.organiza
-000098d0: 7469 6f6e 290a 2020 2020 0a20 2020 2064  tion).    .    d
-000098e0: 6566 2067 6574 5f76 6163 6369 6e65 5f63  ef get_vaccine_c
-000098f0: 6f64 6528 7365 6c66 2c20 696d 6d75 6e69  ode(self, immuni
-00009900: 7a61 7469 6f6e 3d4e 6f6e 652c 2063 6f64  zation=None, cod
-00009910: 696e 675f 7379 7374 656d 3d4e 6f6e 652c  ing_system=None,
-00009920: 2063 6f64 696e 675f 7665 7273 696f 6e3d   coding_version=
-00009930: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
-00009940: 6620 696d 6d75 6e69 7a61 7469 6f6e 2069  f immunization i
-00009950: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00009960: 2020 2020 696d 6d75 6e69 7a61 7469 6f6e      immunization
-00009970: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
-00009980: 6f75 7263 650a 2020 2020 2020 2020 7661  ource.        va
-00009990: 6363 696e 655f 636f 6465 203d 2073 656c  ccine_code = sel
-000099a0: 662e 6765 745f 636f 6465 6162 6c65 5f63  f.get_codeable_c
-000099b0: 6f6e 6365 7074 5f63 6f64 696e 6728 0a20  oncept_coding(. 
-000099c0: 2020 2020 2020 2020 2020 2063 6f64 6561             codea
-000099d0: 626c 655f 636f 6e63 6570 743d 696d 6d75  ble_concept=immu
-000099e0: 6e69 7a61 7469 6f6e 2e76 6163 6369 6e65  nization.vaccine
-000099f0: 436f 6465 2c0a 2020 2020 2020 2020 2020  Code,.          
-00009a00: 2020 636f 6469 6e67 5f73 7973 7465 6d3d    coding_system=
-00009a10: 636f 6469 6e67 5f73 7973 7465 6d2c 0a20  coding_system,. 
-00009a20: 2020 2020 2020 2020 2020 2063 6f64 696e             codin
-00009a30: 675f 7665 7273 696f 6e3d 636f 6469 6e67  g_version=coding
-00009a40: 5f76 6572 7369 6f6e 290a 2020 2020 2020  _version).      
-00009a50: 2020 7265 7475 726e 2076 6163 6369 6e65    return vaccine
-00009a60: 5f63 6f64 650a 0a20 2020 2064 6566 2073  _code..    def s
-00009a70: 6574 5f76 6163 6369 6e65 5f63 6f64 6528  et_vaccine_code(
-00009a80: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
-00009a90: 6f6e 3d4e 6f6e 652c 2076 6163 6369 6e65  on=None, vaccine
-00009aa0: 5f63 6f64 653d 4e6f 6e65 2c20 7661 6363  _code=None, vacc
-00009ab0: 696e 655f 6964 3d4e 6f6e 652c 2076 6163  ine_id=None, vac
-00009ac0: 6369 6e65 5f64 6973 706c 6179 3d4e 6f6e  cine_display=Non
-00009ad0: 652c 2063 6f64 696e 675f 7379 7374 656d  e, coding_system
-00009ae0: 3d4e 6f6e 652c 2063 6f64 696e 675f 7665  =None, coding_ve
-00009af0: 7273 696f 6e3d 4e6f 6e65 293a 0a20 2020  rsion=None):.   
-00009b00: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
-00009b10: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-00009b20: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
-00009b30: 7a61 7469 6f6e 203d 2073 656c 662e 6668  zation = self.fh
-00009b40: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
-00009b50: 2020 2020 6966 2076 6163 6369 6e65 5f69      if vaccine_i
-00009b60: 6420 6973 206e 6f74 204e 6f6e 6520 616e  d is not None an
-00009b70: 6420 7661 6363 696e 655f 636f 6465 2069  d vaccine_code i
-00009b80: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2076  s not None and v
-00009b90: 6163 6369 6e65 5f64 6973 706c 6179 2069  accine_display i
-00009ba0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00009bb0: 2020 2020 2020 2020 7365 6c66 2e76 6163          self.vac
-00009bc0: 6369 6e65 5f63 6f64 655f 636f 6465 203d  cine_code_code =
-00009bd0: 2076 6163 6369 6e65 5f63 6f64 650a 2020   vaccine_code.  
-00009be0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-00009bf0: 6163 6369 6e65 5f63 6f64 655f 6469 7370  accine_code_disp
-00009c00: 6c61 7920 3d20 7661 6363 696e 655f 6469  lay = vaccine_di
-00009c10: 7370 6c61 790a 2020 2020 2020 2020 2020  splay.          
-00009c20: 2020 7365 6c66 2e76 6163 6369 6e65 5f63    self.vaccine_c
-00009c30: 6f64 655f 6964 203d 2076 6163 6369 6e65  ode_id = vaccine
-00009c40: 5f69 640a 0a20 2020 2020 2020 2076 6163  _id..        vac
-00009c50: 6369 6e65 5f63 6f64 6561 626c 655f 636f  cine_codeable_co
-00009c60: 6e63 6570 7420 3d20 7365 6c66 2e74 6f5f  ncept = self.to_
-00009c70: 636f 6465 6162 6c65 5f63 6f6e 6365 7074  codeable_concept
-00009c80: 280a 2020 2020 2020 2020 2020 2020 636f  (.            co
-00009c90: 6465 3d73 656c 662e 7661 6363 696e 655f  de=self.vaccine_
-00009ca0: 636f 6465 5f63 6f64 652c 0a20 2020 2020  code_code,.     
-00009cb0: 2020 2020 2020 2064 6973 706c 6179 3d73         display=s
-00009cc0: 656c 662e 7661 6363 696e 655f 636f 6465  elf.vaccine_code
-00009cd0: 5f64 6973 706c 6179 2c0a 2020 2020 2020  _display,.      
-00009ce0: 2020 2020 2020 6964 3d73 656c 662e 7661        id=self.va
-00009cf0: 6363 696e 655f 636f 6465 5f69 642c 0a20  ccine_code_id,. 
-00009d00: 2020 2020 2020 2020 2020 2063 6f64 696e             codin
-00009d10: 675f 7379 7374 656d 3d63 6f64 696e 675f  g_system=coding_
-00009d20: 7379 7374 656d 2c0a 2020 2020 2020 2020  system,.        
-00009d30: 2020 2020 636f 6469 6e67 5f76 6572 7369      coding_versi
-00009d40: 6f6e 3d63 6f64 696e 675f 7665 7273 696f  on=coding_versio
-00009d50: 6e29 0a20 2020 2020 2020 2069 6d6d 756e  n).        immun
-00009d60: 697a 6174 696f 6e2e 7661 6363 696e 6543  ization.vaccineC
-00009d70: 6f64 6520 3d20 7661 6363 696e 655f 636f  ode = vaccine_co
-00009d80: 6465 6162 6c65 5f63 6f6e 6365 7074 0a0a  deable_concept..
-00009d90: 2020 2020 6465 6620 6765 745f 7061 7469      def get_pati
-00009da0: 656e 7428 7365 6c66 2c20 696d 6d75 6e69  ent(self, immuni
-00009db0: 7a61 7469 6f6e 3d4e 6f6e 6529 3a0a 2020  zation=None):.  
-00009dc0: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
-00009dd0: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
-00009de0: 2020 2020 2020 2020 2020 2069 6d6d 756e             immun
-00009df0: 697a 6174 696f 6e20 3d20 7365 6c66 2e66  ization = self.f
-00009e00: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
-00009e10: 2020 2020 200a 2020 2020 2020 2020 6966       .        if
-00009e20: 2074 7970 6528 696d 6d75 6e69 7a61 7469   type(immunizati
-00009e30: 6f6e 2e70 6174 6965 6e74 2920 6973 2050  on.patient) is P
-00009e40: 6174 6965 6e74 3a0a 2020 2020 2020 2020  atient:.        
-00009e50: 2020 2020 7061 7469 656e 7420 3d20 5061      patient = Pa
-00009e60: 7469 656e 7446 4849 5228 7061 7469 656e  tientFHIR(patien
-00009e70: 745f 7265 736f 7572 6365 5f64 6963 743d  t_resource_dict=
-00009e80: 696d 6d75 6e69 7a61 7469 6f6e 2e70 6174  immunization.pat
-00009e90: 6965 6e74 2e61 735f 6a73 6f6e 2829 290a  ient.as_json()).
-00009ea0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009eb0: 726e 2070 6174 6965 6e74 0a20 2020 2020  rn patient.     
-00009ec0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-00009ed0: 2020 2020 6465 6620 6765 745f 7061 7469      def get_pati
-00009ee0: 656e 745f 7265 6665 7265 6e63 6528 7365  ent_reference(se
-00009ef0: 6c66 2c20 696d 6d75 6e69 7a61 7469 6f6e  lf, immunization
-00009f00: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00009f10: 6966 2069 6d6d 756e 697a 6174 696f 6e20  if immunization 
-00009f20: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00009f30: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
-00009f40: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
-00009f50: 736f 7572 6365 0a20 2020 2020 2020 200a  source.        .
-00009f60: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-00009f70: 696d 6d75 6e69 7a61 7469 6f6e 2e70 6174  immunization.pat
-00009f80: 6965 6e74 2920 6973 2046 4849 5252 6566  ient) is FHIRRef
-00009f90: 6572 656e 6365 3a0a 2020 2020 2020 2020  erence:.        
-00009fa0: 2020 2020 7265 7475 726e 2069 6d6d 756e      return immun
-00009fb0: 697a 6174 696f 6e2e 7061 7469 656e 742e  ization.patient.
-00009fc0: 7265 6665 7265 6e63 650a 2020 2020 2020  reference.      
-00009fd0: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00009fe0: 2020 0a20 2020 2064 6566 2073 6574 5f70    .    def set_p
-00009ff0: 6174 6965 6e74 2873 656c 662c 2069 6d6d  atient(self, imm
-0000a000: 756e 697a 6174 696f 6e3d 4e6f 6e65 2c20  unization=None, 
-0000a010: 7061 7469 656e 745f 7265 6665 7265 6e63  patient_referenc
-0000a020: 653d 4e6f 6e65 2c20 7061 7469 656e 743d  e=None, patient=
-0000a030: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
-0000a040: 6620 696d 6d75 6e69 7a61 7469 6f6e 2069  f immunization i
-0000a050: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000a060: 2020 2020 696d 6d75 6e69 7a61 7469 6f6e      immunization
-0000a070: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
-0000a080: 6f75 7263 650a 0a20 2020 2020 2020 2069  ource..        i
-0000a090: 6620 7061 7469 656e 745f 7265 6665 7265  f patient_refere
-0000a0a0: 6e63 6520 6973 206e 6f74 204e 6f6e 653a  nce is not None:
-0000a0b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000a0c0: 662e 7061 7469 656e 745f 7265 6665 7265  f.patient_refere
-0000a0d0: 6e63 6520 3d20 7061 7469 656e 745f 7265  nce = patient_re
-0000a0e0: 6665 7265 6e63 650a 0a20 2020 2020 2020  ference..       
-0000a0f0: 2069 6620 7061 7469 656e 7420 6973 206e   if patient is n
-0000a100: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000a110: 2020 2020 2073 656c 662e 7061 7469 656e       self.patien
-0000a120: 7420 3d20 7061 7469 656e 740a 0a20 2020  t = patient..   
-0000a130: 2020 2020 2069 6620 7365 6c66 2e70 6174       if self.pat
-0000a140: 6965 6e74 2069 7320 6e6f 7420 4e6f 6e65  ient is not None
-0000a150: 2061 6e64 2073 656c 662e 7061 7469 656e   and self.patien
-0000a160: 745f 7265 6665 7265 6e63 6520 6973 204e  t_reference is N
-0000a170: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000a180: 2070 6174 6965 6e74 5f6d 6f64 656c 203d   patient_model =
-0000a190: 2050 6174 6965 6e74 286a 736f 6e64 6963   Patient(jsondic
-0000a1a0: 743d 7365 6c66 2e70 6174 6965 6e74 2e67  t=self.patient.g
-0000a1b0: 6574 4668 6972 5265 736f 7572 6365 2829  etFhirResource()
-0000a1c0: 290a 2020 2020 2020 2020 2020 2020 696d  ).            im
-0000a1d0: 6d75 6e69 7a61 7469 6f6e 2e70 6174 6965  munization.patie
-0000a1e0: 6e74 203d 2070 6174 6965 6e74 5f6d 6f64  nt = patient_mod
-0000a1f0: 656c 0a20 2020 2020 2020 2065 6c69 6620  el.        elif 
-0000a200: 7365 6c66 2e70 6174 6965 6e74 5f72 6566  self.patient_ref
-0000a210: 6572 656e 6365 2069 7320 6e6f 7420 4e6f  erence is not No
-0000a220: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000a230: 7265 6665 7265 6e63 6520 3d20 4648 4952  reference = FHIR
-0000a240: 5265 6665 7265 6e63 6528 290a 2020 2020  Reference().    
-0000a250: 2020 2020 2020 2020 7265 6665 7265 6e63          referenc
-0000a260: 652e 7265 6665 7265 6e63 6520 3d20 7365  e.reference = se
-0000a270: 6c66 2e70 6174 6965 6e74 5f72 6566 6572  lf.patient_refer
-0000a280: 656e 6365 0a20 2020 2020 2020 2020 2020  ence.           
-0000a290: 2069 6d6d 756e 697a 6174 696f 6e2e 7061   immunization.pa
-0000a2a0: 7469 656e 7420 3d20 7265 6665 7265 6e63  tient = referenc
-0000a2b0: 650a 0a20 2020 2064 6566 2067 6574 5f70  e..    def get_p
-0000a2c0: 6572 666f 726d 6572 2873 656c 662c 2069  erformer(self, i
-0000a2d0: 6d6d 756e 697a 6174 696f 6e3d 4e6f 6e65  mmunization=None
-0000a2e0: 293a 0a20 2020 2020 2020 2069 6620 696d  ):.        if im
-0000a2f0: 6d75 6e69 7a61 7469 6f6e 2069 7320 4e6f  munization is No
-0000a300: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000a310: 696d 6d75 6e69 7a61 7469 6f6e 203d 2073  immunization = s
-0000a320: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
-0000a330: 650a 0a20 2020 2020 2020 2069 6620 696d  e..        if im
-0000a340: 6d75 6e69 7a61 7469 6f6e 2e70 6572 666f  munization.perfo
-0000a350: 726d 6572 2069 7320 6e6f 7420 4e6f 6e65  rmer is not None
-0000a360: 2061 6e64 2074 7970 6528 696d 6d75 6e69   and type(immuni
-0000a370: 7a61 7469 6f6e 2e70 6572 666f 726d 6572  zation.performer
-0000a380: 2920 6973 2050 7261 6374 6974 696f 6e65  ) is Practitione
-0000a390: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
-0000a3a0: 6574 7572 6e20 696d 6d75 6e69 7a61 7469  eturn immunizati
-0000a3b0: 6f6e 2e70 6572 666f 726d 6572 0a20 2020  on.performer.   
-0000a3c0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-0000a3d0: 0a0a 2020 2020 6465 6620 6765 745f 7065  ..    def get_pe
-0000a3e0: 7266 6f72 6d65 725f 7265 6665 7265 6e63  rformer_referenc
-0000a3f0: 6528 7365 6c66 2c20 696d 6d75 6e69 7a61  e(self, immuniza
-0000a400: 7469 6f6e 3d4e 6f6e 6529 3a0a 2020 2020  tion=None):.    
-0000a410: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
-0000a420: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-0000a430: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
-0000a440: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
-0000a450: 725f 7265 736f 7572 6365 0a0a 2020 2020  r_resource..    
-0000a460: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
-0000a470: 696f 6e2e 7065 7266 6f72 6d65 7220 6973  ion.performer is
-0000a480: 206e 6f74 204e 6f6e 6520 616e 6420 7479   not None and ty
-0000a490: 7065 2869 6d6d 756e 697a 6174 696f 6e2e  pe(immunization.
-0000a4a0: 7065 7266 6f72 6d65 7229 2069 7320 4648  performer) is FH
-0000a4b0: 4952 5265 6665 7265 6e63 653a 0a20 2020  IRReference:.   
-0000a4c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000a4d0: 696d 6d75 6e69 7a61 7469 6f6e 2e70 6572  immunization.per
-0000a4e0: 666f 726d 6572 0a20 2020 2020 2020 2072  former.        r
-0000a4f0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-0000a500: 6465 6620 7365 745f 7065 7266 6f72 6d65  def set_performe
-0000a510: 7228 7365 6c66 2c20 696d 6d75 6e69 7a61  r(self, immuniza
-0000a520: 7469 6f6e 3d4e 6f6e 652c 2070 6572 666f  tion=None, perfo
-0000a530: 726d 6572 3d4e 6f6e 652c 2070 6572 666f  rmer=None, perfo
-0000a540: 726d 6572 5f72 6566 6572 656e 6365 3d4e  rmer_reference=N
-0000a550: 6f6e 652c 2070 6572 666f 726d 6572 5f64  one, performer_d
-0000a560: 6973 706c 6179 3d4e 6f6e 6529 3a0a 2020  isplay=None):.  
-0000a570: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
-0000a580: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
-0000a590: 2020 2020 2020 2020 2020 2069 6d6d 756e             immun
-0000a5a0: 697a 6174 696f 6e20 3d20 7365 6c66 2e66  ization = self.f
-0000a5b0: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
-0000a5c0: 2020 2020 2069 6620 7065 7266 6f72 6d65       if performe
-0000a5d0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-0000a5e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a5f0: 7065 7266 6f72 6d65 7220 3d20 7065 7266  performer = perf
-0000a600: 6f72 6d65 720a 2020 2020 2020 2020 6966  ormer.        if
-0000a610: 2070 6572 666f 726d 6572 5f72 6566 6572   performer_refer
-0000a620: 656e 6365 2069 7320 6e6f 7420 4e6f 6e65  ence is not None
-0000a630: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000a640: 6c66 2e70 6572 666f 726d 6572 5f72 6566  lf.performer_ref
-0000a650: 6572 656e 6365 203d 2070 6572 666f 726d  erence = perform
-0000a660: 6572 5f72 6566 6572 656e 6365 0a20 2020  er_reference.   
-0000a670: 2020 2020 2069 6620 7065 7266 6f72 6d65       if performe
-0000a680: 725f 6469 7370 6c61 7920 6973 206e 6f74  r_display is not
+00009820: 2069 6d6d 756e 697a 6174 696f 6e2e 636f   immunization.co
+00009830: 6e74 6169 6e65 642e 6170 7065 6e64 2873  ntained.append(s
+00009840: 656c 662e 6f72 6761 6e69 7a61 7469 6f6e  elf.organization
+00009850: 290a 2020 2020 0a20 2020 2064 6566 2067  ).    .    def g
+00009860: 6574 5f76 6163 6369 6e65 5f63 6f64 6528  et_vaccine_code(
+00009870: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
+00009880: 6f6e 3d4e 6f6e 652c 2063 6f64 696e 675f  on=None, coding_
+00009890: 7379 7374 656d 3d4e 6f6e 652c 2063 6f64  system=None, cod
+000098a0: 696e 675f 7665 7273 696f 6e3d 4e6f 6e65  ing_version=None
+000098b0: 293a 0a20 2020 2020 2020 2069 6620 696d  ):.        if im
+000098c0: 6d75 6e69 7a61 7469 6f6e 2069 7320 4e6f  munization is No
+000098d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000098e0: 696d 6d75 6e69 7a61 7469 6f6e 203d 2073  immunization = s
+000098f0: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+00009900: 650a 2020 2020 2020 2020 7661 6363 696e  e.        vaccin
+00009910: 655f 636f 6465 203d 2073 656c 662e 6765  e_code = self.ge
+00009920: 745f 636f 6465 6162 6c65 5f63 6f6e 6365  t_codeable_conce
+00009930: 7074 5f63 6f64 696e 6728 0a20 2020 2020  pt_coding(.     
+00009940: 2020 2020 2020 2063 6f64 6561 626c 655f         codeable_
+00009950: 636f 6e63 6570 743d 696d 6d75 6e69 7a61  concept=immuniza
+00009960: 7469 6f6e 2e76 6163 6369 6e65 436f 6465  tion.vaccineCode
+00009970: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+00009980: 6469 6e67 5f73 7973 7465 6d3d 636f 6469  ding_system=codi
+00009990: 6e67 5f73 7973 7465 6d2c 0a20 2020 2020  ng_system,.     
+000099a0: 2020 2020 2020 2063 6f64 696e 675f 7665         coding_ve
+000099b0: 7273 696f 6e3d 636f 6469 6e67 5f76 6572  rsion=coding_ver
+000099c0: 7369 6f6e 290a 2020 2020 2020 2020 7265  sion).        re
+000099d0: 7475 726e 2076 6163 6369 6e65 5f63 6f64  turn vaccine_cod
+000099e0: 650a 0a20 2020 2064 6566 2073 6574 5f76  e..    def set_v
+000099f0: 6163 6369 6e65 5f63 6f64 6528 7365 6c66  accine_code(self
+00009a00: 2c20 696d 6d75 6e69 7a61 7469 6f6e 3d4e  , immunization=N
+00009a10: 6f6e 652c 2076 6163 6369 6e65 5f63 6f64  one, vaccine_cod
+00009a20: 653d 4e6f 6e65 2c20 7661 6363 696e 655f  e=None, vaccine_
+00009a30: 6964 3d4e 6f6e 652c 2076 6163 6369 6e65  id=None, vaccine
+00009a40: 5f64 6973 706c 6179 3d4e 6f6e 652c 2063  _display=None, c
+00009a50: 6f64 696e 675f 7379 7374 656d 3d4e 6f6e  oding_system=Non
+00009a60: 652c 2063 6f64 696e 675f 7665 7273 696f  e, coding_versio
+00009a70: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
+00009a80: 2069 6620 696d 6d75 6e69 7a61 7469 6f6e   if immunization
+00009a90: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00009aa0: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
+00009ab0: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
+00009ac0: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
+00009ad0: 6966 2076 6163 6369 6e65 5f69 6420 6973  if vaccine_id is
+00009ae0: 206e 6f74 204e 6f6e 6520 616e 6420 7661   not None and va
+00009af0: 6363 696e 655f 636f 6465 2069 7320 6e6f  ccine_code is no
+00009b00: 7420 4e6f 6e65 2061 6e64 2076 6163 6369  t None and vacci
+00009b10: 6e65 5f64 6973 706c 6179 2069 7320 6e6f  ne_display is no
+00009b20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00009b30: 2020 2020 7365 6c66 2e76 6163 6369 6e65      self.vaccine
+00009b40: 5f63 6f64 655f 636f 6465 203d 2076 6163  _code_code = vac
+00009b50: 6369 6e65 5f63 6f64 650a 2020 2020 2020  cine_code.      
+00009b60: 2020 2020 2020 7365 6c66 2e76 6163 6369        self.vacci
+00009b70: 6e65 5f63 6f64 655f 6469 7370 6c61 7920  ne_code_display 
+00009b80: 3d20 7661 6363 696e 655f 6469 7370 6c61  = vaccine_displa
+00009b90: 790a 2020 2020 2020 2020 2020 2020 7365  y.            se
+00009ba0: 6c66 2e76 6163 6369 6e65 5f63 6f64 655f  lf.vaccine_code_
+00009bb0: 6964 203d 2076 6163 6369 6e65 5f69 640a  id = vaccine_id.
+00009bc0: 0a20 2020 2020 2020 2076 6163 6369 6e65  .        vaccine
+00009bd0: 5f63 6f64 6561 626c 655f 636f 6e63 6570  _codeable_concep
+00009be0: 7420 3d20 7365 6c66 2e74 6f5f 636f 6465  t = self.to_code
+00009bf0: 6162 6c65 5f63 6f6e 6365 7074 280a 2020  able_concept(.  
+00009c00: 2020 2020 2020 2020 2020 636f 6465 3d73            code=s
+00009c10: 656c 662e 7661 6363 696e 655f 636f 6465  elf.vaccine_code
+00009c20: 5f63 6f64 652c 0a20 2020 2020 2020 2020  _code,.         
+00009c30: 2020 2064 6973 706c 6179 3d73 656c 662e     display=self.
+00009c40: 7661 6363 696e 655f 636f 6465 5f64 6973  vaccine_code_dis
+00009c50: 706c 6179 2c0a 2020 2020 2020 2020 2020  play,.          
+00009c60: 2020 6964 3d73 656c 662e 7661 6363 696e    id=self.vaccin
+00009c70: 655f 636f 6465 5f69 642c 0a20 2020 2020  e_code_id,.     
+00009c80: 2020 2020 2020 2063 6f64 696e 675f 7379         coding_sy
+00009c90: 7374 656d 3d63 6f64 696e 675f 7379 7374  stem=coding_syst
+00009ca0: 656d 2c0a 2020 2020 2020 2020 2020 2020  em,.            
+00009cb0: 636f 6469 6e67 5f76 6572 7369 6f6e 3d63  coding_version=c
+00009cc0: 6f64 696e 675f 7665 7273 696f 6e29 0a20  oding_version). 
+00009cd0: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
+00009ce0: 696f 6e2e 7661 6363 696e 6543 6f64 6520  ion.vaccineCode 
+00009cf0: 3d20 7661 6363 696e 655f 636f 6465 6162  = vaccine_codeab
+00009d00: 6c65 5f63 6f6e 6365 7074 0a0a 2020 2020  le_concept..    
+00009d10: 6465 6620 6765 745f 7061 7469 656e 7428  def get_patient(
+00009d20: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
+00009d30: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
+00009d40: 2020 6966 2069 6d6d 756e 697a 6174 696f    if immunizatio
+00009d50: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+00009d60: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
+00009d70: 696f 6e20 3d20 7365 6c66 2e66 6869 725f  ion = self.fhir_
+00009d80: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
+00009d90: 200a 2020 2020 2020 2020 6966 2074 7970   .        if typ
+00009da0: 6528 696d 6d75 6e69 7a61 7469 6f6e 2e70  e(immunization.p
+00009db0: 6174 6965 6e74 2920 6973 2050 6174 6965  atient) is Patie
+00009dc0: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
+00009dd0: 7061 7469 656e 7420 3d20 5061 7469 656e  patient = Patien
+00009de0: 7446 4849 5228 7061 7469 656e 745f 7265  tFHIR(patient_re
+00009df0: 736f 7572 6365 5f64 6963 743d 696d 6d75  source_dict=immu
+00009e00: 6e69 7a61 7469 6f6e 2e70 6174 6965 6e74  nization.patient
+00009e10: 2e61 735f 6a73 6f6e 2829 290a 2020 2020  .as_json()).    
+00009e20: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+00009e30: 6174 6965 6e74 0a20 2020 2020 2020 2072  atient.        r
+00009e40: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
+00009e50: 6465 6620 6765 745f 7061 7469 656e 745f  def get_patient_
+00009e60: 7265 6665 7265 6e63 6528 7365 6c66 2c20  reference(self, 
+00009e70: 696d 6d75 6e69 7a61 7469 6f6e 3d4e 6f6e  immunization=Non
+00009e80: 6529 3a0a 2020 2020 2020 2020 6966 2069  e):.        if i
+00009e90: 6d6d 756e 697a 6174 696f 6e20 6973 204e  mmunization is N
+00009ea0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00009eb0: 2069 6d6d 756e 697a 6174 696f 6e20 3d20   immunization = 
+00009ec0: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
+00009ed0: 6365 0a20 2020 2020 2020 200a 2020 2020  ce.        .    
+00009ee0: 2020 2020 6966 2074 7970 6528 696d 6d75      if type(immu
+00009ef0: 6e69 7a61 7469 6f6e 2e70 6174 6965 6e74  nization.patient
+00009f00: 2920 6973 2046 4849 5252 6566 6572 656e  ) is FHIRReferen
+00009f10: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
+00009f20: 7265 7475 726e 2069 6d6d 756e 697a 6174  return immunizat
+00009f30: 696f 6e2e 7061 7469 656e 742e 7265 6665  ion.patient.refe
+00009f40: 7265 6e63 650a 2020 2020 2020 2020 7265  rence.        re
+00009f50: 7475 726e 204e 6f6e 650a 2020 2020 0a20  turn None.    . 
+00009f60: 2020 2064 6566 2073 6574 5f70 6174 6965     def set_patie
+00009f70: 6e74 2873 656c 662c 2069 6d6d 756e 697a  nt(self, immuniz
+00009f80: 6174 696f 6e3d 4e6f 6e65 2c20 7061 7469  ation=None, pati
+00009f90: 656e 745f 7265 6665 7265 6e63 653d 4e6f  ent_reference=No
+00009fa0: 6e65 2c20 7061 7469 656e 743d 4e6f 6e65  ne, patient=None
+00009fb0: 293a 0a20 2020 2020 2020 2069 6620 696d  ):.        if im
+00009fc0: 6d75 6e69 7a61 7469 6f6e 2069 7320 4e6f  munization is No
+00009fd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00009fe0: 696d 6d75 6e69 7a61 7469 6f6e 203d 2073  immunization = s
+00009ff0: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+0000a000: 650a 0a20 2020 2020 2020 2069 6620 7061  e..        if pa
+0000a010: 7469 656e 745f 7265 6665 7265 6e63 6520  tient_reference 
+0000a020: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000a030: 2020 2020 2020 2020 2073 656c 662e 7061           self.pa
+0000a040: 7469 656e 745f 7265 6665 7265 6e63 6520  tient_reference 
+0000a050: 3d20 7061 7469 656e 745f 7265 6665 7265  = patient_refere
+0000a060: 6e63 650a 0a20 2020 2020 2020 2069 6620  nce..        if 
+0000a070: 7061 7469 656e 7420 6973 206e 6f74 204e  patient is not N
+0000a080: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000a090: 2073 656c 662e 7061 7469 656e 7420 3d20   self.patient = 
+0000a0a0: 7061 7469 656e 740a 0a20 2020 2020 2020  patient..       
+0000a0b0: 2069 6620 7365 6c66 2e70 6174 6965 6e74   if self.patient
+0000a0c0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0000a0d0: 2073 656c 662e 7061 7469 656e 745f 7265   self.patient_re
+0000a0e0: 6665 7265 6e63 6520 6973 204e 6f6e 653a  ference is None:
+0000a0f0: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+0000a100: 6965 6e74 5f6d 6f64 656c 203d 2050 6174  ient_model = Pat
+0000a110: 6965 6e74 286a 736f 6e64 6963 743d 7365  ient(jsondict=se
+0000a120: 6c66 2e70 6174 6965 6e74 2e67 6574 4668  lf.patient.getFh
+0000a130: 6972 5265 736f 7572 6365 2829 290a 2020  irResource()).  
+0000a140: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
+0000a150: 7a61 7469 6f6e 2e70 6174 6965 6e74 203d  zation.patient =
+0000a160: 2070 6174 6965 6e74 5f6d 6f64 656c 0a20   patient_model. 
+0000a170: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+0000a180: 2e70 6174 6965 6e74 5f72 6566 6572 656e  .patient_referen
+0000a190: 6365 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ce is not None:.
+0000a1a0: 2020 2020 2020 2020 2020 2020 7265 6665              refe
+0000a1b0: 7265 6e63 6520 3d20 4648 4952 5265 6665  rence = FHIRRefe
+0000a1c0: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
+0000a1d0: 2020 2020 7265 6665 7265 6e63 652e 7265      reference.re
+0000a1e0: 6665 7265 6e63 6520 3d20 7365 6c66 2e70  ference = self.p
+0000a1f0: 6174 6965 6e74 5f72 6566 6572 656e 6365  atient_reference
+0000a200: 0a20 2020 2020 2020 2020 2020 2069 6d6d  .            imm
+0000a210: 756e 697a 6174 696f 6e2e 7061 7469 656e  unization.patien
+0000a220: 7420 3d20 7265 6665 7265 6e63 650a 0a20  t = reference.. 
+0000a230: 2020 2064 6566 2067 6574 5f70 6572 666f     def get_perfo
+0000a240: 726d 6572 2873 656c 662c 2069 6d6d 756e  rmer(self, immun
+0000a250: 697a 6174 696f 6e3d 4e6f 6e65 293a 0a20  ization=None):. 
+0000a260: 2020 2020 2020 2069 6620 696d 6d75 6e69         if immuni
+0000a270: 7a61 7469 6f6e 2069 7320 4e6f 6e65 3a0a  zation is None:.
+0000a280: 2020 2020 2020 2020 2020 2020 696d 6d75              immu
+0000a290: 6e69 7a61 7469 6f6e 203d 2073 656c 662e  nization = self.
+0000a2a0: 6668 6972 5f72 6573 6f75 7263 650a 0a20  fhir_resource.. 
+0000a2b0: 2020 2020 2020 2069 6620 696d 6d75 6e69         if immuni
+0000a2c0: 7a61 7469 6f6e 2e70 6572 666f 726d 6572  zation.performer
+0000a2d0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0000a2e0: 2074 7970 6528 696d 6d75 6e69 7a61 7469   type(immunizati
+0000a2f0: 6f6e 2e70 6572 666f 726d 6572 2920 6973  on.performer) is
+0000a300: 2050 7261 6374 6974 696f 6e65 723a 0a20   Practitioner:. 
+0000a310: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a320: 6e20 696d 6d75 6e69 7a61 7469 6f6e 2e70  n immunization.p
+0000a330: 6572 666f 726d 6572 0a20 2020 2020 2020  erformer.       
+0000a340: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+0000a350: 2020 6465 6620 6765 745f 7065 7266 6f72    def get_perfor
+0000a360: 6d65 725f 7265 6665 7265 6e63 6528 7365  mer_reference(se
+0000a370: 6c66 2c20 696d 6d75 6e69 7a61 7469 6f6e  lf, immunization
+0000a380: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0000a390: 6966 2069 6d6d 756e 697a 6174 696f 6e20  if immunization 
+0000a3a0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000a3b0: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
+0000a3c0: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
+0000a3d0: 736f 7572 6365 0a0a 2020 2020 2020 2020  source..        
+0000a3e0: 6966 2069 6d6d 756e 697a 6174 696f 6e2e  if immunization.
+0000a3f0: 7065 7266 6f72 6d65 7220 6973 206e 6f74  performer is not
+0000a400: 204e 6f6e 6520 616e 6420 7479 7065 2869   None and type(i
+0000a410: 6d6d 756e 697a 6174 696f 6e2e 7065 7266  mmunization.perf
+0000a420: 6f72 6d65 7229 2069 7320 4648 4952 5265  ormer) is FHIRRe
+0000a430: 6665 7265 6e63 653a 0a20 2020 2020 2020  ference:.       
+0000a440: 2020 2020 2072 6574 7572 6e20 696d 6d75       return immu
+0000a450: 6e69 7a61 7469 6f6e 2e70 6572 666f 726d  nization.perform
+0000a460: 6572 0a20 2020 2020 2020 2072 6574 7572  er.        retur
+0000a470: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
+0000a480: 7365 745f 7065 7266 6f72 6d65 7228 7365  set_performer(se
+0000a490: 6c66 2c20 696d 6d75 6e69 7a61 7469 6f6e  lf, immunization
+0000a4a0: 3d4e 6f6e 652c 2070 6572 666f 726d 6572  =None, performer
+0000a4b0: 3d4e 6f6e 652c 2070 6572 666f 726d 6572  =None, performer
+0000a4c0: 5f72 6566 6572 656e 6365 3d4e 6f6e 652c  _reference=None,
+0000a4d0: 2070 6572 666f 726d 6572 5f64 6973 706c   performer_displ
+0000a4e0: 6179 3d4e 6f6e 6529 3a0a 2020 2020 2020  ay=None):.      
+0000a4f0: 2020 6966 2069 6d6d 756e 697a 6174 696f    if immunizatio
+0000a500: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+0000a510: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
+0000a520: 696f 6e20 3d20 7365 6c66 2e66 6869 725f  ion = self.fhir_
+0000a530: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
+0000a540: 2069 6620 7065 7266 6f72 6d65 7220 6973   if performer is
+0000a550: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000a560: 2020 2020 2020 2073 656c 662e 7065 7266         self.perf
+0000a570: 6f72 6d65 7220 3d20 7065 7266 6f72 6d65  ormer = performe
+0000a580: 720a 2020 2020 2020 2020 6966 2070 6572  r.        if per
+0000a590: 666f 726d 6572 5f72 6566 6572 656e 6365  former_reference
+0000a5a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000a5b0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000a5c0: 6572 666f 726d 6572 5f72 6566 6572 656e  erformer_referen
+0000a5d0: 6365 203d 2070 6572 666f 726d 6572 5f72  ce = performer_r
+0000a5e0: 6566 6572 656e 6365 0a20 2020 2020 2020  eference.       
+0000a5f0: 2069 6620 7065 7266 6f72 6d65 725f 6469   if performer_di
+0000a600: 7370 6c61 7920 6973 206e 6f74 204e 6f6e  splay is not Non
+0000a610: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000a620: 656c 662e 7065 7266 6f72 6d65 725f 6469  elf.performer_di
+0000a630: 7370 6c61 7920 3d20 7065 7266 6f72 6d65  splay = performe
+0000a640: 725f 6469 7370 6c61 790a 0a20 2020 2020  r_display..     
+0000a650: 2020 2069 6620 7365 6c66 2e70 6572 666f     if self.perfo
+0000a660: 726d 6572 2069 7320 6e6f 7420 4e6f 6e65  rmer is not None
+0000a670: 2061 6e64 2073 656c 662e 7065 7266 6f72   and self.perfor
+0000a680: 6d65 725f 7265 6665 7265 6e63 6520 6973  mer_reference is
 0000a690: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000a6a0: 2020 2073 656c 662e 7065 7266 6f72 6d65     self.performe
-0000a6b0: 725f 6469 7370 6c61 7920 3d20 7065 7266  r_display = perf
-0000a6c0: 6f72 6d65 725f 6469 7370 6c61 790a 0a20  ormer_display.. 
-0000a6d0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000a6e0: 6572 666f 726d 6572 2069 7320 6e6f 7420  erformer is not 
-0000a6f0: 4e6f 6e65 2061 6e64 2073 656c 662e 7065  None and self.pe
-0000a700: 7266 6f72 6d65 725f 7265 6665 7265 6e63  rformer_referenc
-0000a710: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-0000a720: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
-0000a730: 696f 6e2e 7065 7266 6f72 6d65 7220 3d20  ion.performer = 
-0000a740: 7365 6c66 2e70 6572 666f 726d 6572 0a20  self.performer. 
-0000a750: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-0000a760: 2e70 6572 666f 726d 6572 5f72 6566 6572  .performer_refer
-0000a770: 656e 6365 2069 7320 6e6f 7420 4e6f 6e65  ence is not None
-0000a780: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000a790: 6620 3d20 4648 4952 5265 6665 7265 6e63  f = FHIRReferenc
-0000a7a0: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000a7b0: 7265 662e 7265 6665 7265 6e63 6520 3d20  ref.reference = 
-0000a7c0: 7365 6c66 2e70 6572 666f 726d 6572 5f72  self.performer_r
-0000a7d0: 6566 6572 656e 6365 0a20 2020 2020 2020  eference.       
-0000a7e0: 2020 2020 2072 6566 2e64 6973 706c 6179       ref.display
-0000a7f0: 203d 2073 656c 662e 7065 7266 6f72 6d65   = self.performe
-0000a800: 725f 6469 7370 6c61 790a 2020 2020 2020  r_display.      
-0000a810: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
-0000a820: 6f6e 2e70 6572 666f 726d 6572 203d 2072  on.performer = r
-0000a830: 6566 0a0a 2020 2020 6465 6620 6765 745f  ef..    def get_
-0000a840: 6c6f 6361 7469 6f6e 2873 656c 662c 2069  location(self, i
-0000a850: 6d6d 756e 697a 6174 696f 6e3d 4e6f 6e65  mmunization=None
-0000a860: 293a 0a20 2020 2020 2020 2069 6620 696d  ):.        if im
-0000a870: 6d75 6e69 7a61 7469 6f6e 2069 7320 4e6f  munization is No
-0000a880: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000a890: 696d 6d75 6e69 7a61 7469 6f6e 203d 2073  immunization = s
-0000a8a0: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
-0000a8b0: 650a 2020 2020 2020 2020 6966 2069 6d6d  e.        if imm
-0000a8c0: 756e 697a 6174 696f 6e2e 6c6f 6361 7469  unization.locati
-0000a8d0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 2061  on is not None a
-0000a8e0: 6e64 2074 7970 6528 696d 6d75 6e69 7a61  nd type(immuniza
-0000a8f0: 7469 6f6e 2e6c 6f63 6174 696f 6e29 2069  tion.location) i
-0000a900: 7320 4c6f 6361 7469 6f6e 3a0a 2020 2020  s Location:.    
-0000a910: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-0000a920: 6d6d 756e 697a 6174 696f 6e2e 6c6f 6361  mmunization.loca
-0000a930: 7469 6f6e 0a20 2020 2020 2020 2072 6574  tion.        ret
-0000a940: 7572 6e20 4e6f 6e65 0a0a 2020 2020 6465  urn None..    de
-0000a950: 6620 6765 745f 6c6f 6361 7469 6f6e 5f72  f get_location_r
-0000a960: 6566 6572 656e 6365 2873 656c 662c 2069  eference(self, i
-0000a970: 6d6d 756e 697a 6174 696f 6e3d 4e6f 6e65  mmunization=None
-0000a980: 293a 0a20 2020 2020 2020 2069 6620 696d  ):.        if im
-0000a990: 6d75 6e69 7a61 7469 6f6e 2069 7320 4e6f  munization is No
-0000a9a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000a9b0: 696d 6d75 6e69 7a61 7469 6f6e 203d 2073  immunization = s
-0000a9c0: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
-0000a9d0: 650a 2020 2020 2020 2020 6966 2069 6d6d  e.        if imm
-0000a9e0: 756e 697a 6174 696f 6e2e 6c6f 6361 7469  unization.locati
-0000a9f0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 2061  on is not None a
-0000aa00: 6e64 2074 7970 6528 696d 6d75 6e69 7a61  nd type(immuniza
-0000aa10: 7469 6f6e 2e6c 6f63 6174 696f 6e29 2069  tion.location) i
-0000aa20: 7320 4648 4952 5265 6665 7265 6e63 653a  s FHIRReference:
-0000aa30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000aa40: 7572 6e20 696d 6d75 6e69 7a61 7469 6f6e  urn immunization
-0000aa50: 2e6c 6f63 6174 696f 6e0a 2020 2020 2020  .location.      
-0000aa60: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-0000aa70: 2020 2064 6566 2073 6574 5f6c 6f63 6174     def set_locat
-0000aa80: 696f 6e28 7365 6c66 2c20 696d 6d75 6e69  ion(self, immuni
-0000aa90: 7a61 7469 6f6e 3d4e 6f6e 652c 206c 6f63  zation=None, loc
-0000aaa0: 6174 696f 6e3d 4e6f 6e65 2c20 6c6f 6361  ation=None, loca
-0000aab0: 7469 6f6e 5f72 6566 6572 656e 6365 3d4e  tion_reference=N
-0000aac0: 6f6e 652c 206c 6f63 6174 696f 6e5f 6469  one, location_di
-0000aad0: 7370 6c61 793d 4e6f 6e65 293a 0a20 2020  splay=None):.   
-0000aae0: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
-0000aaf0: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-0000ab00: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
-0000ab10: 7a61 7469 6f6e 203d 2073 656c 662e 6668  zation = self.fh
-0000ab20: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
-0000ab30: 2020 2020 6966 206c 6f63 6174 696f 6e20      if location 
-0000ab40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000ab50: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-0000ab60: 6361 7469 6f6e 3d6c 6f63 6174 696f 6e0a  cation=location.
-0000ab70: 2020 2020 2020 2020 6966 206c 6f63 6174          if locat
-0000ab80: 696f 6e5f 7265 6665 7265 6e63 6520 6973  ion_reference is
-0000ab90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000aba0: 2020 2020 2020 2073 656c 662e 6c6f 6361         self.loca
-0000abb0: 7469 6f6e 5f72 6566 6572 656e 6365 203d  tion_reference =
-0000abc0: 206c 6f63 6174 696f 6e5f 7265 6665 7265   location_refere
-0000abd0: 6e63 650a 2020 2020 2020 2020 6966 206c  nce.        if l
-0000abe0: 6f63 6174 696f 6e5f 6469 7370 6c61 7920  ocation_display 
-0000abf0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000ac00: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-0000ac10: 6361 7469 6f6e 5f64 6973 706c 6179 203d  cation_display =
-0000ac20: 206c 6f63 6174 696f 6e5f 6469 7370 6c61   location_displa
-0000ac30: 790a 0a20 2020 2020 2020 2069 6620 7365  y..        if se
-0000ac40: 6c66 2e6c 6f63 6174 696f 6e20 6973 206e  lf.location is n
-0000ac50: 6f74 204e 6f6e 6520 616e 6420 7365 6c66  ot None and self
-0000ac60: 2e6c 6f63 6174 696f 6e5f 7265 6665 7265  .location_refere
-0000ac70: 6e63 6520 6973 204e 6f6e 653a 0a20 2020  nce is None:.   
-0000ac80: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
-0000ac90: 6174 696f 6e2e 6c6f 6361 7469 6f6e 203d  ation.location =
-0000aca0: 2073 656c 662e 6c6f 6361 7469 6f6e 0a20   self.location. 
-0000acb0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-0000acc0: 2e6c 6f63 6174 696f 6e5f 7265 6665 7265  .location_refere
-0000acd0: 6e63 6520 6973 206e 6f74 204e 6f6e 653a  nce is not None:
-0000ace0: 0a20 2020 2020 2020 2020 2020 2072 6566  .            ref
-0000acf0: 203d 2046 4849 5252 6566 6572 656e 6365   = FHIRReference
-0000ad00: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
-0000ad10: 6566 2e72 6566 6572 656e 6365 203d 2073  ef.reference = s
-0000ad20: 656c 662e 6c6f 6361 7469 6f6e 5f72 6566  elf.location_ref
-0000ad30: 6572 656e 6365 0a20 2020 2020 2020 2020  erence.         
-0000ad40: 2020 2072 6566 2e64 6973 706c 6179 203d     ref.display =
-0000ad50: 2073 656c 662e 6c6f 6361 7469 6f6e 5f64   self.location_d
-0000ad60: 6973 706c 6179 0a20 2020 2020 2020 2020  isplay.         
-0000ad70: 2020 2069 6d6d 756e 697a 6174 696f 6e2e     immunization.
-0000ad80: 6c6f 6361 7469 6f6e 203d 2072 6566 0a0a  location = ref..
-0000ad90: 2020 2020 6465 6620 6765 745f 6c6f 745f      def get_lot_
-0000ada0: 6e75 6d62 6572 2873 656c 662c 2069 6d6d  number(self, imm
-0000adb0: 756e 697a 6174 696f 6e3d 4e6f 6e65 293a  unization=None):
-0000adc0: 0a20 2020 2020 2020 2069 6620 696d 6d75  .        if immu
-0000add0: 6e69 7a61 7469 6f6e 2069 7320 4e6f 6e65  nization is None
-0000ade0: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
-0000adf0: 6d75 6e69 7a61 7469 6f6e 203d 2073 656c  munization = sel
-0000ae00: 662e 6668 6972 5f72 6573 6f75 7263 650a  f.fhir_resource.
-0000ae10: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-0000ae20: 6d6d 756e 697a 6174 696f 6e2e 6c6f 744e  mmunization.lotN
-0000ae30: 756d 6265 720a 0a20 2020 2064 6566 2073  umber..    def s
-0000ae40: 6574 5f6c 6f74 5f6e 756d 6265 7228 7365  et_lot_number(se
-0000ae50: 6c66 2c20 696d 6d75 6e69 7a61 7469 6f6e  lf, immunization
-0000ae60: 3d4e 6f6e 652c 206c 6f74 5f6e 756d 6265  =None, lot_numbe
-0000ae70: 723d 4e6f 6e65 293a 0a20 2020 2020 2020  r=None):.       
-0000ae80: 2069 6620 696d 6d75 6e69 7a61 7469 6f6e   if immunization
-0000ae90: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000aea0: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
-0000aeb0: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
-0000aec0: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
-0000aed0: 6966 206c 6f74 5f6e 756d 6265 7220 6973  if lot_number is
-0000aee0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000aef0: 2020 2020 2020 2073 656c 662e 6c6f 745f         self.lot_
-0000af00: 6e75 6d62 6572 203d 206c 6f74 5f6e 756d  number = lot_num
-0000af10: 6265 720a 2020 2020 2020 2020 696d 6d75  ber.        immu
-0000af20: 6e69 7a61 7469 6f6e 2e6c 6f74 4e75 6d62  nization.lotNumb
-0000af30: 6572 203d 2073 656c 662e 6c6f 745f 6e75  er = self.lot_nu
-0000af40: 6d62 6572 0a0a 2020 2020 6465 6620 6765  mber..    def ge
-0000af50: 745f 6578 7069 7261 7469 6f6e 5f64 6174  t_expiration_dat
-0000af60: 6528 7365 6c66 2c20 696d 6d75 6e69 7a61  e(self, immuniza
-0000af70: 7469 6f6e 3d4e 6f6e 6529 3a0a 2020 2020  tion=None):.    
-0000af80: 2020 2020 6966 2069 6d6d 756e 697a 6174      if immunizat
-0000af90: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-0000afa0: 2020 2020 2020 2020 2069 6d6d 756e 697a           immuniz
-0000afb0: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
-0000afc0: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
-0000afd0: 2020 2069 6620 696d 6d75 6e69 7a61 7469     if immunizati
-0000afe0: 6f6e 2e65 7870 6972 6174 696f 6e44 6174  on.expirationDat
-0000aff0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-0000b000: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b010: 6e20 696d 6d75 6e69 7a61 7469 6f6e 2e65  n immunization.e
-0000b020: 7870 6972 6174 696f 6e44 6174 652e 6973  xpirationDate.is
-0000b030: 6f73 7472 696e 670a 0a20 2020 2064 6566  ostring..    def
-0000b040: 2073 6574 5f65 7870 6972 6174 696f 6e5f   set_expiration_
-0000b050: 6461 7465 2873 656c 662c 2069 6d6d 756e  date(self, immun
-0000b060: 697a 6174 696f 6e3d 4e6f 6e65 2c20 6578  ization=None, ex
-0000b070: 7069 7261 7469 6f6e 5f64 6174 653d 4e6f  piration_date=No
-0000b080: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
-0000b090: 696d 6d75 6e69 7a61 7469 6f6e 2069 7320  immunization is 
-0000b0a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000b0b0: 2020 696d 6d75 6e69 7a61 7469 6f6e 203d    immunization =
-0000b0c0: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
-0000b0d0: 7263 650a 2020 2020 2020 2020 6966 2065  rce.        if e
-0000b0e0: 7870 6972 6174 696f 6e5f 6461 7465 2069  xpiration_date i
-0000b0f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000b100: 2020 2020 2020 2020 7365 6c66 2e65 7870          self.exp
-0000b110: 6972 6174 696f 6e5f 6461 7465 203d 2065  iration_date = e
-0000b120: 7870 6972 6174 696f 6e5f 6461 7465 0a20  xpiration_date. 
-0000b130: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-0000b140: 7870 6972 6174 696f 6e5f 6461 7465 2069  xpiration_date i
-0000b150: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000b160: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-0000b170: 7365 6c66 2e65 7870 6972 6174 696f 6e5f  self.expiration_
-0000b180: 6461 7465 2920 6973 2073 7472 3a0a 2020  date) is str:.  
-0000b190: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0000b1a0: 6d75 6e69 7a61 7469 6f6e 2e65 7870 6972  munization.expir
-0000b1b0: 6174 696f 6e44 6174 6520 3d20 6461 7465  ationDate = date
-0000b1c0: 7469 6d65 2e73 7472 7074 696d 6528 7365  time.strptime(se
-0000b1d0: 6c66 2e65 7870 6972 6174 696f 6e5f 6461  lf.expiration_da
-0000b1e0: 7465 2c20 2225 592d 256d 2d25 6422 290a  te, "%Y-%m-%d").
-0000b1f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000b200: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b210: 2020 696d 6d75 6e69 7a61 7469 6f6e 2e65    immunization.e
-0000b220: 7870 6972 6174 696f 6e44 6174 6520 3d20  xpirationDate = 
-0000b230: 7365 6c66 2e65 7870 6972 6174 696f 6e5f  self.expiration_
-0000b240: 6461 7465 0a0a 2020 2020 6465 6620 6765  date..    def ge
-0000b250: 745f 7369 7465 2873 656c 662c 2069 6d6d  t_site(self, imm
-0000b260: 756e 697a 6174 696f 6e3d 4e6f 6e65 2c20  unization=None, 
-0000b270: 636f 6469 6e67 5f73 7973 7465 6d3d 4e6f  coding_system=No
-0000b280: 6e65 2c20 636f 6469 6e67 5f76 6572 7369  ne, coding_versi
-0000b290: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
-0000b2a0: 2020 6966 2069 6d6d 756e 697a 6174 696f    if immunizatio
-0000b2b0: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-0000b2c0: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
-0000b2d0: 696f 6e20 3d20 7365 6c66 2e66 6869 725f  ion = self.fhir_
-0000b2e0: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
-0000b2f0: 2069 6620 696d 6d75 6e69 7a61 7469 6f6e   if immunization
-0000b300: 2e73 6974 6520 6973 206e 6f74 204e 6f6e  .site is not Non
-0000b310: 6520 616e 6420 7479 7065 2869 6d6d 756e  e and type(immun
-0000b320: 697a 6174 696f 6e2e 7369 7465 2920 6973  ization.site) is
-0000b330: 2043 6f64 6561 626c 6543 6f6e 6365 7074   CodeableConcept
-0000b340: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-0000b350: 6469 6e67 203d 2073 656c 662e 6765 745f  ding = self.get_
-0000b360: 636f 6465 6162 6c65 5f63 6f6e 6365 7074  codeable_concept
-0000b370: 5f63 6f64 696e 6728 0a20 2020 2020 2020  _coding(.       
-0000b380: 2020 2020 2020 2020 2063 6f64 6561 626c           codeabl
-0000b390: 655f 636f 6e63 6570 743d 696d 6d75 6e69  e_concept=immuni
-0000b3a0: 7a61 7469 6f6e 2e73 6974 652c 0a20 2020  zation.site,.   
-0000b3b0: 2020 2020 2020 2020 2020 2020 2063 6f64               cod
-0000b3c0: 696e 675f 7379 7374 656d 3d63 6f64 696e  ing_system=codin
-0000b3d0: 675f 7379 7374 656d 2c0a 2020 2020 2020  g_system,.      
-0000b3e0: 2020 2020 2020 2020 2020 636f 6469 6e67            coding
-0000b3f0: 5f76 6572 7369 6f6e 3d63 6f64 696e 675f  _version=coding_
-0000b400: 7665 7273 696f 6e29 0a20 2020 2020 2020  version).       
-0000b410: 2020 2020 2072 6574 7572 6e20 636f 6469       return codi
-0000b420: 6e67 0a20 2020 2020 2020 2072 6574 7572  ng.        retur
-0000b430: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
-0000b440: 7365 745f 7369 7465 2873 656c 662c 2069  set_site(self, i
-0000b450: 6d6d 756e 697a 6174 696f 6e3d 4e6f 6e65  mmunization=None
-0000b460: 2c20 7369 7465 5f63 6f64 653d 4e6f 6e65  , site_code=None
-0000b470: 2c20 7369 7465 5f69 643d 4e6f 6e65 2c20  , site_id=None, 
-0000b480: 7369 7465 5f64 6973 706c 6179 3d4e 6f6e  site_display=Non
-0000b490: 652c 2063 6f64 696e 675f 7379 7374 656d  e, coding_system
-0000b4a0: 3d4e 6f6e 652c 2063 6f64 696e 675f 7665  =None, coding_ve
-0000b4b0: 7273 696f 6e3d 4e6f 6e65 293a 0a20 2020  rsion=None):.   
-0000b4c0: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
-0000b4d0: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-0000b4e0: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
-0000b4f0: 7a61 7469 6f6e 203d 2073 656c 662e 6668  zation = self.fh
-0000b500: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
-0000b510: 2020 2020 6966 2073 6974 655f 636f 6465      if site_code
-0000b520: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000b530: 2073 6974 655f 6964 2069 7320 6e6f 7420   site_id is not 
-0000b540: 4e6f 6e65 2061 6e64 2073 6974 655f 6469  None and site_di
-0000b550: 7370 6c61 7920 6973 206e 6f74 204e 6f6e  splay is not Non
-0000b560: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000b570: 656c 662e 7369 7465 5f63 6f64 6520 3d20  elf.site_code = 
-0000b580: 7369 7465 5f63 6f64 650a 2020 2020 2020  site_code.      
-0000b590: 2020 2020 2020 7365 6c66 2e73 6974 655f        self.site_
-0000b5a0: 6469 7370 6c61 7920 3d20 7369 7465 5f64  display = site_d
-0000b5b0: 6973 706c 6179 0a20 2020 2020 2020 2020  isplay.         
-0000b5c0: 2020 2073 656c 662e 7369 7465 5f69 6420     self.site_id 
-0000b5d0: 3d20 7369 7465 5f69 640a 2020 2020 2020  = site_id.      
-0000b5e0: 2020 7369 7465 203d 2073 656c 662e 746f    site = self.to
-0000b5f0: 5f63 6f64 6561 626c 655f 636f 6e63 6570  _codeable_concep
-0000b600: 7428 0a20 2020 2020 2020 2020 2020 2063  t(.            c
-0000b610: 6f64 653d 7365 6c66 2e73 6974 655f 636f  ode=self.site_co
-0000b620: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
-0000b630: 6469 7370 6c61 793d 7365 6c66 2e73 6974  display=self.sit
-0000b640: 655f 6469 7370 6c61 792c 0a20 2020 2020  e_display,.     
-0000b650: 2020 2020 2020 2069 643d 7365 6c66 2e73         id=self.s
-0000b660: 6974 655f 6964 2c0a 2020 2020 2020 2020  ite_id,.        
-0000b670: 2020 2020 636f 6469 6e67 5f73 7973 7465      coding_syste
-0000b680: 6d3d 636f 6469 6e67 5f73 7973 7465 6d2c  m=coding_system,
-0000b690: 0a20 2020 2020 2020 2020 2020 2063 6f64  .            cod
-0000b6a0: 696e 675f 7665 7273 696f 6e3d 636f 6469  ing_version=codi
-0000b6b0: 6e67 5f76 6572 7369 6f6e 0a20 2020 2020  ng_version.     
-0000b6c0: 2020 2029 0a20 2020 2020 2020 2069 6d6d     ).        imm
-0000b6d0: 756e 697a 6174 696f 6e2e 7369 7465 203d  unization.site =
-0000b6e0: 2073 6974 650a 0a20 2020 2064 6566 2067   site..    def g
-0000b6f0: 6574 5f64 6f73 655f 7175 616e 7469 7479  et_dose_quantity
-0000b700: 2873 656c 662c 2069 6d6d 756e 697a 6174  (self, immunizat
-0000b710: 696f 6e3d 4e6f 6e65 293a 0a20 2020 2020  ion=None):.     
-0000b720: 2020 2069 6620 696d 6d75 6e69 7a61 7469     if immunizati
-0000b730: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-0000b740: 2020 2020 2020 2020 696d 6d75 6e69 7a61          immuniza
-0000b750: 7469 6f6e 203d 2073 656c 662e 6668 6972  tion = self.fhir
-0000b760: 5f72 6573 6f75 7263 650a 2020 2020 2020  _resource.      
-0000b770: 2020 7265 7475 726e 2069 6d6d 756e 697a    return immuniz
-0000b780: 6174 696f 6e2e 646f 7365 5175 616e 7469  ation.doseQuanti
-0000b790: 7479 0a20 2020 2020 2020 2020 2020 200a  ty.            .
-0000b7a0: 2020 2020 0a20 2020 2064 6566 2073 6574      .    def set
-0000b7b0: 5f64 6f73 655f 7175 616e 7469 7479 2873  _dose_quantity(s
-0000b7c0: 656c 662c 2069 6d6d 756e 697a 6174 696f  elf, immunizatio
-0000b7d0: 6e3d 4e6f 6e65 2c20 7175 616e 7469 7479  n=None, quantity
-0000b7e0: 3d4e 6f6e 652c 2071 7561 6e74 6974 795f  =None, quantity_
-0000b7f0: 636f 6465 3d4e 6f6e 652c 2071 7561 6e74  code=None, quant
-0000b800: 6974 795f 756e 6974 3d4e 6f6e 652c 2071  ity_unit=None, q
-0000b810: 7561 6e74 6974 795f 7661 6c75 653d 4e6f  uantity_value=No
-0000b820: 6e65 2c20 7175 616e 7469 7479 5f73 7973  ne, quantity_sys
-0000b830: 7465 6d3d 4e6f 6e65 293a 0a20 2020 2020  tem=None):.     
-0000b840: 2020 2069 6620 696d 6d75 6e69 7a61 7469     if immunizati
-0000b850: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-0000b860: 2020 2020 2020 2020 696d 6d75 6e69 7a61          immuniza
-0000b870: 7469 6f6e 203d 2073 656c 662e 6668 6972  tion = self.fhir
-0000b880: 5f72 6573 6f75 7263 650a 2020 2020 2020  _resource.      
-0000b890: 2020 6966 2071 7561 6e74 6974 795f 7379    if quantity_sy
-0000b8a0: 7374 656d 2069 7320 4e6f 6e65 3a0a 2020  stem is None:.  
-0000b8b0: 2020 2020 2020 2020 2020 7175 616e 7469            quanti
-0000b8c0: 7479 5f73 7973 7465 6d20 3d20 7365 6c66  ty_system = self
-0000b8d0: 2e63 6f64 696e 675f 7379 7374 656d 0a20  .coding_system. 
-0000b8e0: 2020 2020 2020 2069 6620 7175 616e 7469         if quanti
-0000b8f0: 7479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ty is not None:.
-0000b900: 2020 2020 2020 2020 2020 2020 646f 7365              dose
-0000b910: 5f71 7561 6e74 6974 7920 3d20 7175 616e  _quantity = quan
-0000b920: 7469 7479 0a20 2020 2020 2020 2020 2020  tity.           
-0000b930: 2073 656c 662e 646f 7365 5f71 7561 6e74   self.dose_quant
-0000b940: 6974 795f 636f 6465 203d 2064 6f73 655f  ity_code = dose_
-0000b950: 7175 616e 7469 7479 2e63 6f64 650a 2020  quantity.code.  
-0000b960: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0000b970: 6f73 655f 7175 616e 7469 7479 5f75 6e69  ose_quantity_uni
-0000b980: 7420 3d20 646f 7365 5f71 7561 6e74 6974  t = dose_quantit
-0000b990: 792e 756e 6974 0a20 2020 2020 2020 2020  y.unit.         
-0000b9a0: 2020 2073 656c 662e 646f 7365 5f71 7561     self.dose_qua
-0000b9b0: 6e74 6974 795f 7661 6c75 6520 3d20 646f  ntity_value = do
-0000b9c0: 7365 5f71 7561 6e74 6974 792e 7661 6c75  se_quantity.valu
-0000b9d0: 650a 2020 2020 2020 2020 656c 7365 3a0a  e.        else:.
-0000b9e0: 2020 2020 2020 2020 2020 2020 6966 2071              if q
-0000b9f0: 7561 6e74 6974 795f 756e 6974 2069 7320  uantity_unit is 
-0000ba00: 6e6f 7420 4e6f 6e65 2061 6e64 2071 7561  not None and qua
-0000ba10: 6e74 6974 795f 7661 6c75 6520 6973 206e  ntity_value is n
-0000ba20: 6f74 204e 6f6e 6520 616e 6420 7175 616e  ot None and quan
-0000ba30: 7469 7479 5f63 6f64 6520 6973 206e 6f74  tity_code is not
-0000ba40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000ba50: 2020 2020 2020 2073 656c 662e 646f 7365         self.dose
-0000ba60: 5f71 7561 6e74 6974 795f 636f 6465 203d  _quantity_code =
-0000ba70: 2071 7561 6e74 6974 795f 636f 6465 0a20   quantity_code. 
-0000ba80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ba90: 656c 662e 646f 7365 5f71 7561 6e74 6974  elf.dose_quantit
-0000baa0: 795f 756e 6974 203d 2071 7561 6e74 6974  y_unit = quantit
-0000bab0: 795f 756e 6974 0a20 2020 2020 2020 2020  y_unit.         
-0000bac0: 2020 2020 2020 2073 656c 662e 646f 7365         self.dose
-0000bad0: 5f71 7561 6e74 6974 795f 7661 6c75 6520  _quantity_value 
-0000bae0: 3d20 7175 616e 7469 7479 5f76 616c 7565  = quantity_value
-0000baf0: 0a20 2020 2020 2020 2020 2020 2064 6f73  .            dos
-0000bb00: 655f 7175 616e 7469 7479 203d 2051 7561  e_quantity = Qua
-0000bb10: 6e74 6974 7928 290a 2020 2020 2020 2020  ntity().        
-0000bb20: 2020 2020 646f 7365 5f71 7561 6e74 6974      dose_quantit
-0000bb30: 792e 636f 6465 203d 2073 656c 662e 646f  y.code = self.do
-0000bb40: 7365 5f71 7561 6e74 6974 795f 636f 6465  se_quantity_code
-0000bb50: 0a20 2020 2020 2020 2020 2020 2064 6f73  .            dos
-0000bb60: 655f 7175 616e 7469 7479 2e73 7973 7465  e_quantity.syste
-0000bb70: 6d20 3d20 7175 616e 7469 7479 5f73 7973  m = quantity_sys
-0000bb80: 7465 6d0a 2020 2020 2020 2020 2020 2020  tem.            
-0000bb90: 646f 7365 5f71 7561 6e74 6974 792e 756e  dose_quantity.un
-0000bba0: 6974 203d 2073 656c 662e 646f 7365 5f71  it = self.dose_q
-0000bbb0: 7561 6e74 6974 795f 756e 6974 0a20 2020  uantity_unit.   
-0000bbc0: 2020 2020 2020 2020 2064 6f73 655f 7175           dose_qu
-0000bbd0: 616e 7469 7479 2e76 616c 7565 203d 2073  antity.value = s
-0000bbe0: 656c 662e 646f 7365 5f71 7561 6e74 6974  elf.dose_quantit
-0000bbf0: 795f 7661 6c75 650a 0a20 2020 2020 2020  y_value..       
-0000bc00: 2069 6d6d 756e 697a 6174 696f 6e2e 646f   immunization.do
-0000bc10: 7365 5175 616e 7469 7479 203d 2064 6f73  seQuantity = dos
-0000bc20: 655f 7175 616e 7469 7479 0a0a 2020 2020  e_quantity..    
-0000bc30: 6465 6620 6765 745f 7265 6173 6f6e 7328  def get_reasons(
-0000bc40: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
-0000bc50: 6f6e 3d4e 6f6e 652c 2063 6f64 696e 675f  on=None, coding_
-0000bc60: 7379 7374 656d 3d4e 6f6e 652c 2063 6f64  system=None, cod
-0000bc70: 696e 675f 7665 7273 696f 6e3d 4e6f 6e65  ing_version=None
-0000bc80: 293a 0a20 2020 2020 2020 2069 6620 696d  ):.        if im
-0000bc90: 6d75 6e69 7a61 7469 6f6e 2069 7320 4e6f  munization is No
-0000bca0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000bcb0: 696d 6d75 6e69 7a61 7469 6f6e 2020 3d20  immunization  = 
-0000bcc0: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
-0000bcd0: 6365 0a20 2020 2020 2020 2069 6620 696d  ce.        if im
-0000bce0: 6d75 6e69 7a61 7469 6f6e 2e65 7870 6c61  munization.expla
-0000bcf0: 6e61 7469 6f6e 2069 7320 6e6f 7420 4e6f  nation is not No
-0000bd00: 6e65 2061 6e64 2069 6d6d 756e 697a 6174  ne and immunizat
-0000bd10: 696f 6e2e 6578 706c 616e 6174 696f 6e2e  ion.explanation.
-0000bd20: 7265 6173 6f6e 2069 7320 6e6f 7420 4e6f  reason is not No
-0000bd30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000bd40: 7265 6173 6f6e 7320 3d20 5b5d 0a20 2020  reasons = [].   
-0000bd50: 2020 2020 2020 2020 2066 6f72 2072 6561           for rea
-0000bd60: 736f 6e20 696e 2069 6d6d 756e 697a 6174  son in immunizat
-0000bd70: 696f 6e2e 6578 706c 616e 6174 696f 6e2e  ion.explanation.
-0000bd80: 7265 6173 6f6e 3a0a 2020 2020 2020 2020  reason:.        
-0000bd90: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-0000bda0: 7265 6173 6f6e 2920 6973 2043 6f64 6561  reason) is Codea
-0000bdb0: 626c 6543 6f6e 6365 7074 3a0a 2020 2020  bleConcept:.    
-0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdd0: 7265 6173 6f6e 5f63 6f64 696e 6720 3d20  reason_coding = 
-0000bde0: 7365 6c66 2e67 6574 5f63 6f64 6561 626c  self.get_codeabl
-0000bdf0: 655f 636f 6e63 6570 745f 636f 6469 6e67  e_concept_coding
-0000be00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000be10: 2020 2020 2020 2020 2020 636f 6465 6162            codeab
-0000be20: 6c65 5f63 6f6e 6365 7074 3d72 6561 736f  le_concept=reaso
-0000be30: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-0000be40: 2020 2020 2020 2020 2020 2063 6f64 696e             codin
-0000be50: 675f 7379 7374 656d 3d63 6f64 696e 675f  g_system=coding_
-0000be60: 7379 7374 656d 2c0a 2020 2020 2020 2020  system,.        
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be80: 636f 6469 6e67 5f76 6572 7369 6f6e 3d63  coding_version=c
-0000be90: 6f64 696e 675f 7665 7273 696f 6e29 0a20  oding_version). 
-0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000beb0: 2020 2072 6561 736f 6e73 2e61 7070 656e     reasons.appen
-0000bec0: 6428 7265 6173 6f6e 5f63 6f64 696e 672e  d(reason_coding.
-0000bed0: 6173 5f6a 736f 6e28 2929 0a20 2020 2020  as_json()).     
-0000bee0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000bef0: 7479 7065 2872 6561 736f 6e29 2069 7320  type(reason) is 
-0000bf00: 436f 6469 6e67 3a0a 2020 2020 2020 2020  Coding:.        
-0000bf10: 2020 2020 2020 2020 2020 2020 7265 6173              reas
-0000bf20: 6f6e 732e 6170 7065 6e64 2872 6561 736f  ons.append(reaso
-0000bf30: 6e2e 6173 5f6a 736f 6e28 2929 0a20 2020  n.as_json()).   
-0000bf40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000bf50: 7265 6173 6f6e 730a 0a20 2020 2064 6566  reasons..    def
-0000bf60: 2073 6574 5f72 6561 736f 6e28 7365 6c66   set_reason(self
-0000bf70: 2c20 696d 6d75 6e69 7a61 7469 6f6e 3d4e  , immunization=N
-0000bf80: 6f6e 652c 2072 6561 736f 6e73 3d4e 6f6e  one, reasons=Non
-0000bf90: 652c 2063 6f64 696e 675f 7379 7374 656d  e, coding_system
-0000bfa0: 3d4e 6f6e 652c 2063 6f64 696e 675f 7665  =None, coding_ve
-0000bfb0: 7273 696f 6e3d 4e6f 6e65 293a 0a20 2020  rsion=None):.   
-0000bfc0: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
-0000bfd0: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-0000bfe0: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
-0000bff0: 7a61 7469 6f6e 203d 2073 656c 662e 6668  zation = self.fh
-0000c000: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
-0000c010: 2020 2020 636f 6469 6e67 5f73 7973 7465      coding_syste
-0000c020: 6d20 3d20 636f 6469 6e67 5f73 7973 7465  m = coding_syste
-0000c030: 6d20 6966 2063 6f64 696e 675f 7379 7374  m if coding_syst
-0000c040: 656d 2069 7320 6e6f 7420 4e6f 6e65 2065  em is not None e
-0000c050: 6c73 6520 7365 6c66 2e63 6f64 696e 675f  lse self.coding_
-0000c060: 7379 7374 656d 0a20 2020 2020 2020 2063  system.        c
-0000c070: 6f64 696e 675f 7665 7273 696f 6e20 3d20  oding_version = 
-0000c080: 636f 6469 6e67 5f76 6572 7369 6f6e 2069  coding_version i
-0000c090: 6620 636f 6469 6e67 5f76 6572 7369 6f6e  f coding_version
-0000c0a0: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-0000c0b0: 6520 7365 6c66 2e63 6f64 696e 675f 7665  e self.coding_ve
-0000c0c0: 7273 696f 6e0a 2020 2020 2020 2020 6966  rsion.        if
-0000c0d0: 2072 6561 736f 6e73 2069 7320 6e6f 7420   reasons is not 
-0000c0e0: 4e6f 6e65 2061 6e64 206c 656e 2872 6561  None and len(rea
-0000c0f0: 736f 6e73 2920 3e20 303a 0a20 2020 2020  sons) > 0:.     
-0000c100: 2020 2020 2020 2073 656c 662e 7265 6173         self.reas
-0000c110: 6f6e 203d 2072 6561 736f 6e73 0a0a 2020  on = reasons..  
-0000c120: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-0000c130: 6173 6f6e 2069 7320 6e6f 7420 4e6f 6e65  ason is not None
-0000c140: 2061 6e64 206c 656e 2873 656c 662e 7265   and len(self.re
-0000c150: 6173 6f6e 2920 3e20 303a 0a20 2020 2020  ason) > 0:.     
-0000c160: 2020 2020 2020 2069 6d6d 5f65 7870 6c61         imm_expla
-0000c170: 6e61 7469 6f6e 203d 2049 6d6d 756e 697a  nation = Immuniz
-0000c180: 6174 696f 6e45 7870 6c61 6e61 7469 6f6e  ationExplanation
-0000c190: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-0000c1a0: 6d6d 5f65 7870 6c61 6e61 7469 6f6e 2e72  mm_explanation.r
-0000c1b0: 6561 736f 6e20 3d20 5b5d 0a20 2020 2020  eason = [].     
-0000c1c0: 2020 2020 2020 2066 6f72 2072 6561 736f         for reaso
-0000c1d0: 6e20 696e 2073 656c 662e 7265 6173 6f6e  n in self.reason
-0000c1e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c1f0: 2020 7265 6173 6f6e 5f63 6f64 696e 6720    reason_coding 
-0000c200: 3d20 436f 6469 6e67 286a 736f 6e64 6963  = Coding(jsondic
-0000c210: 743d 7265 6173 6f6e 290a 2020 2020 2020  t=reason).      
-0000c220: 2020 2020 2020 2020 2020 7265 6173 6f6e            reason
-0000c230: 5f63 6f64 696e 672e 7665 7273 696f 6e20  _coding.version 
-0000c240: 3d20 636f 6469 6e67 5f76 6572 7369 6f6e  = coding_version
-0000c250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c260: 2072 6561 736f 6e5f 636f 6469 6e67 2e73   reason_coding.s
-0000c270: 7973 7465 6d20 3d20 636f 6469 6e67 5f73  ystem = coding_s
-0000c280: 7973 7465 6d20 0a20 2020 2020 2020 2020  ystem .         
-0000c290: 2020 2020 2020 2069 6d6d 5f65 7870 6c61         imm_expla
-0000c2a0: 6e61 7469 6f6e 2e72 6561 736f 6e2e 6170  nation.reason.ap
-0000c2b0: 7065 6e64 2872 6561 736f 6e5f 636f 6469  pend(reason_codi
-0000c2c0: 6e67 290a 2020 2020 2020 2020 2020 2020  ng).            
-0000c2d0: 696d 6d75 6e69 7a61 7469 6f6e 2e65 7870  immunization.exp
-0000c2e0: 6c61 6e61 7469 6f6e 203d 2069 6d6d 5f65  lanation = imm_e
-0000c2f0: 7870 6c61 6e61 7469 6f6e 0a0a 2020 2020  xplanation..    
-0000c300: 6465 6620 6765 745f 6461 7465 2873 656c  def get_date(sel
-0000c310: 662c 2069 6d6d 756e 697a 6174 696f 6e3d  f, immunization=
-0000c320: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
-0000c330: 6620 696d 6d75 6e69 7a61 7469 6f6e 2069  f immunization i
-0000c340: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000c350: 2020 2020 696d 6d75 6e69 7a61 7469 6f6e      immunization
-0000c360: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
-0000c370: 6f75 7263 650a 2020 2020 2020 2020 7265  ource.        re
-0000c380: 7475 726e 2069 6d6d 756e 697a 6174 696f  turn immunizatio
-0000c390: 6e2e 6461 7465 0a0a 2020 2020 6465 6620  n.date..    def 
-0000c3a0: 7365 745f 6461 7465 2873 656c 662c 2069  set_date(self, i
-0000c3b0: 6d6d 756e 697a 6174 696f 6e3d 4e6f 6e65  mmunization=None
-0000c3c0: 2c20 6461 7465 5f74 6f5f 7365 743d 4e6f  , date_to_set=No
-0000c3d0: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
-0000c3e0: 696d 6d75 6e69 7a61 7469 6f6e 2069 7320  immunization is 
-0000c3f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000c400: 2020 696d 6d75 6e69 7a61 7469 6f6e 203d    immunization =
-0000c410: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
-0000c420: 7263 650a 2020 2020 2020 2020 6966 2064  rce.        if d
-0000c430: 6174 655f 746f 5f73 6574 2069 7320 6e6f  ate_to_set is no
-0000c440: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000c450: 2020 2020 6966 2074 7970 6528 6461 7465      if type(date
-0000c460: 5f74 6f5f 7365 7429 2069 7320 7374 723a  _to_set) is str:
-0000c470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c480: 2073 656c 662e 6461 7465 203d 2064 6174   self.date = dat
-0000c490: 655f 746f 5f73 6574 0a20 2020 2020 2020  e_to_set.       
-0000c4a0: 2020 2020 2065 6c69 6620 7479 7065 2864       elif type(d
-0000c4b0: 6174 655f 746f 5f73 6574 2920 6973 2064  ate_to_set) is d
-0000c4c0: 6174 6520 6f72 2074 7970 6528 6461 7465  ate or type(date
-0000c4d0: 5f74 6f5f 7365 7429 2069 7320 6461 7465  _to_set) is date
-0000c4e0: 7469 6d65 3a0a 2020 2020 2020 2020 2020  time:.          
-0000c4f0: 2020 2020 2020 7365 6c66 2e64 6174 6520        self.date 
-0000c500: 3d20 6461 7465 7469 6d65 2e73 7472 6674  = datetime.strft
-0000c510: 696d 6528 6461 7465 5f74 6f5f 7365 742c  ime(date_to_set,
-0000c520: 2022 2559 2d25 6d2d 2564 5425 483a 254d   "%Y-%m-%dT%H:%M
-0000c530: 3a25 5322 290a 2020 2020 2020 2020 6966  :%S").        if
-0000c540: 2074 7970 6528 7365 6c66 2e64 6174 6529   type(self.date)
-0000c550: 2069 7320 6461 7465 206f 7220 7479 7065   is date or type
-0000c560: 2873 656c 662e 6461 7465 2920 6973 2064  (self.date) is d
-0000c570: 6174 6574 696d 653a 0a20 2020 2020 2020  atetime:.       
-0000c580: 2020 2020 2073 656c 662e 6461 7465 203d       self.date =
-0000c590: 2064 6174 6574 696d 652e 7374 7266 7469   datetime.strfti
-0000c5a0: 6d65 2873 656c 662e 6461 7465 2c22 2559  me(self.date,"%Y
-0000c5b0: 2d25 6d2d 2564 5425 483a 254d 3a25 5322  -%m-%dT%H:%M:%S"
-0000c5c0: 290a 2020 2020 2020 2020 696d 6d75 6e69  ).        immuni
-0000c5d0: 7a61 7469 6f6e 2e64 6174 6520 3d20 4648  zation.date = FH
-0000c5e0: 4952 4461 7465 286a 736f 6e76 616c 3d73  IRDate(jsonval=s
-0000c5f0: 656c 662e 6461 7465 2920 6966 2073 656c  elf.date) if sel
-0000c600: 662e 6461 7465 2069 7320 6e6f 7420 4e6f  f.date is not No
-0000c610: 6e65 2065 6c73 6520 4e6f 6e65 0a20 2020  ne else None.   
-0000c620: 2020 2020 200a 0a20 2020 2064 6566 2067       ..    def g
-0000c630: 6574 5f73 7461 7475 7328 7365 6c66 2c20  et_status(self, 
-0000c640: 696d 6d75 6e69 7a61 7469 6f6e 3d4e 6f6e  immunization=Non
-0000c650: 6529 3a0a 2020 2020 2020 2020 6966 2069  e):.        if i
-0000c660: 6d6d 756e 697a 6174 696f 6e20 6973 204e  mmunization is N
-0000c670: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000c680: 2069 6d6d 756e 697a 6174 696f 6e20 3d20   immunization = 
-0000c690: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
-0000c6a0: 6365 0a20 2020 2020 2020 2072 6574 7572  ce.        retur
-0000c6b0: 6e20 696d 6d75 6e69 7a61 7469 6f6e 2e73  n immunization.s
-0000c6c0: 7461 7475 730a 0a20 2020 2064 6566 2073  tatus..    def s
-0000c6d0: 6574 5f73 7461 7475 7328 7365 6c66 2c20  et_status(self, 
-0000c6e0: 696d 6d75 6e69 7a61 7469 6f6e 3d4e 6f6e  immunization=Non
-0000c6f0: 652c 2073 7461 7475 733d 4e6f 6e65 293a  e, status=None):
-0000c700: 0a20 2020 2020 2020 2069 6620 696d 6d75  .        if immu
-0000c710: 6e69 7a61 7469 6f6e 2069 7320 4e6f 6e65  nization is None
-0000c720: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
-0000c730: 6d75 6e69 7a61 7469 6f6e 203d 2073 656c  munization = sel
-0000c740: 662e 6668 6972 5f72 6573 6f75 7263 650a  f.fhir_resource.
-0000c750: 2020 2020 2020 2020 6966 2073 7461 7475          if statu
-0000c760: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-0000c770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000c780: 7374 6174 7573 203d 2073 7461 7475 730a  status = status.
-0000c790: 2020 2020 2020 2020 696d 6d75 6e69 7a61          immuniza
-0000c7a0: 7469 6f6e 2e73 7461 7475 7320 3d20 7365  tion.status = se
-0000c7b0: 6c66 2e73 7461 7475 730a 0a20 2020 2064  lf.status..    d
-0000c7c0: 6566 2074 6f5f 6668 6972 5f72 6573 6f75  ef to_fhir_resou
-0000c7d0: 7263 6528 7365 6c66 2c20 696d 6d75 6e69  rce(self, immuni
-0000c7e0: 7a61 7469 6f6e 3d4e 6f6e 6529 3a0a 2020  zation=None):.  
-0000c7f0: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
-0000c800: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
-0000c810: 2020 2020 2020 2020 2020 2069 6d6d 756e             immun
-0000c820: 697a 6174 696f 6e20 3d20 496d 6d75 6e69  ization = Immuni
-0000c830: 7a61 7469 6f6e 2829 0a20 2020 2020 2020  zation().       
-0000c840: 2073 656c 662e 7365 745f 6964 2869 6d6d   self.set_id(imm
-0000c850: 756e 697a 6174 696f 6e3d 696d 6d75 6e69  unization=immuni
-0000c860: 7a61 7469 6f6e 290a 2020 2020 2020 2020  zation).        
-0000c870: 7365 6c66 2e73 6574 5f6d 6574 6128 696d  self.set_meta(im
-0000c880: 6d75 6e69 7a61 7469 6f6e 3d69 6d6d 756e  munization=immun
-0000c890: 697a 6174 696f 6e29 0a20 2020 2020 2020  ization).       
-0000c8a0: 2073 656c 662e 7365 745f 636f 6e74 6169   self.set_contai
-0000c8b0: 6e65 645f 6f72 6761 6e69 7a61 7469 6f6e  ned_organization
-0000c8c0: 2869 6d6d 756e 697a 6174 696f 6e3d 696d  (immunization=im
-0000c8d0: 6d75 6e69 7a61 7469 6f6e 290a 2020 2020  munization).    
-0000c8e0: 2020 2020 7365 6c66 2e73 6574 5f6f 7665      self.set_ove
-0000c8f0: 7272 6964 655f 7374 6174 7573 2869 6d6d  rride_status(imm
-0000c900: 756e 697a 6174 696f 6e3d 696d 6d75 6e69  unization=immuni
-0000c910: 7a61 7469 6f6e 290a 2020 2020 2020 2020  zation).        
-0000c920: 7365 6c66 2e73 6574 5f6c 6f74 5f69 6428  self.set_lot_id(
-0000c930: 696d 6d75 6e69 7a61 7469 6f6e 3d69 6d6d  immunization=imm
-0000c940: 756e 697a 6174 696f 6e29 0a20 2020 2020  unization).     
-0000c950: 2020 2073 656c 662e 7365 745f 616e 7469     self.set_anti
-0000c960: 6765 6e5f 7374 6174 7573 2869 6d6d 756e  gen_status(immun
-0000c970: 697a 6174 696f 6e3d 696d 6d75 6e69 7a61  ization=immuniza
-0000c980: 7469 6f6e 290a 2020 2020 2020 2020 7365  tion).        se
-0000c990: 6c66 2e73 6574 5f74 7261 6465 5f6e 616d  lf.set_trade_nam
-0000c9a0: 6528 696d 6d75 6e69 7a61 7469 6f6e 3d69  e(immunization=i
-0000c9b0: 6d6d 756e 697a 6174 696f 6e29 0a20 2020  mmunization).   
-0000c9c0: 2020 2020 2073 656c 662e 7365 745f 7661       self.set_va
-0000c9d0: 6363 696e 655f 636f 6465 2869 6d6d 756e  ccine_code(immun
-0000c9e0: 697a 6174 696f 6e3d 696d 6d75 6e69 7a61  ization=immuniza
-0000c9f0: 7469 6f6e 290a 2020 2020 2020 2020 7365  tion).        se
-0000ca00: 6c66 2e73 6574 5f70 6174 6965 6e74 2869  lf.set_patient(i
-0000ca10: 6d6d 756e 697a 6174 696f 6e3d 696d 6d75  mmunization=immu
-0000ca20: 6e69 7a61 7469 6f6e 290a 2020 2020 2020  nization).      
-0000ca30: 2020 7365 6c66 2e73 6574 5f70 6572 666f    self.set_perfo
-0000ca40: 726d 6572 2869 6d6d 756e 697a 6174 696f  rmer(immunizatio
-0000ca50: 6e3d 696d 6d75 6e69 7a61 7469 6f6e 290a  n=immunization).
-0000ca60: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000ca70: 5f6c 6f63 6174 696f 6e28 696d 6d75 6e69  _location(immuni
-0000ca80: 7a61 7469 6f6e 3d69 6d6d 756e 697a 6174  zation=immunizat
-0000ca90: 696f 6e29 0a20 2020 2020 2020 2073 656c  ion).        sel
-0000caa0: 662e 7365 745f 6c6f 745f 6e75 6d62 6572  f.set_lot_number
-0000cab0: 2869 6d6d 756e 697a 6174 696f 6e3d 696d  (immunization=im
-0000cac0: 6d75 6e69 7a61 7469 6f6e 290a 2020 2020  munization).    
-0000cad0: 2020 2020 7365 6c66 2e73 6574 5f65 7870      self.set_exp
-0000cae0: 6972 6174 696f 6e5f 6461 7465 2869 6d6d  iration_date(imm
-0000caf0: 756e 697a 6174 696f 6e3d 696d 6d75 6e69  unization=immuni
-0000cb00: 7a61 7469 6f6e 290a 2020 2020 2020 2020  zation).        
-0000cb10: 7365 6c66 2e73 6574 5f73 6974 6528 696d  self.set_site(im
-0000cb20: 6d75 6e69 7a61 7469 6f6e 3d69 6d6d 756e  munization=immun
-0000cb30: 697a 6174 696f 6e29 0a20 2020 2020 2020  ization).       
-0000cb40: 2073 656c 662e 7365 745f 646f 7365 5f71   self.set_dose_q
-0000cb50: 7561 6e74 6974 7928 696d 6d75 6e69 7a61  uantity(immuniza
-0000cb60: 7469 6f6e 3d69 6d6d 756e 697a 6174 696f  tion=immunizatio
-0000cb70: 6e29 0a20 2020 2020 2020 2073 656c 662e  n).        self.
-0000cb80: 7365 745f 7265 6173 6f6e 2869 6d6d 756e  set_reason(immun
-0000cb90: 697a 6174 696f 6e3d 696d 6d75 6e69 7a61  ization=immuniza
-0000cba0: 7469 6f6e 290a 2020 2020 2020 2020 7365  tion).        se
-0000cbb0: 6c66 2e73 6574 5f64 6174 6528 696d 6d75  lf.set_date(immu
-0000cbc0: 6e69 7a61 7469 6f6e 3d69 6d6d 756e 697a  nization=immuniz
-0000cbd0: 6174 696f 6e29 0a20 2020 2020 2020 2073  ation).        s
-0000cbe0: 656c 662e 7365 745f 7374 6174 7573 2869  elf.set_status(i
-0000cbf0: 6d6d 756e 697a 6174 696f 6e3d 696d 6d75  mmunization=immu
-0000cc00: 6e69 7a61 7469 6f6e 290a 2020 2020 2020  nization).      
-0000cc10: 2020 7265 7475 726e 2069 6d6d 756e 697a    return immuniz
-0000cc20: 6174 696f 6e0a 0a20 2020 2064 6566 2067  ation..    def g
-0000cc30: 6574 4668 6972 5265 736f 7572 6365 2873  etFhirResource(s
-0000cc40: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-0000cc50: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
-0000cc60: 203d 2073 656c 662e 746f 5f66 6869 725f   = self.to_fhir_
-0000cc70: 7265 736f 7572 6365 2829 0a20 2020 2020  resource().     
-0000cc80: 2020 2072 6573 6f75 7263 6520 3d20 7365     resource = se
-0000cc90: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
-0000cca0: 2e61 735f 6a73 6f6e 2829 0a20 2020 2020  .as_json().     
-0000ccb0: 2020 2072 6574 7572 6e20 7265 736f 7572     return resour
-0000ccc0: 6365 0a20 2020 2020 2020 200a 2020 2020  ce.        .    
-0000ccd0: 6465 6620 6672 6f6d 5f64 6963 7428 7365  def from_dict(se
-0000cce0: 6c66 2c20 696d 6d5f 6469 6374 3d4e 6f6e  lf, imm_dict=Non
-0000ccf0: 6529 3a0a 2020 2020 2020 2020 6966 2069  e):.        if i
-0000cd00: 6d6d 5f64 6963 7420 6973 204e 6f6e 653a  mm_dict is None:
-0000cd10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000cd20: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-0000cd30: 2069 6d6d 5f72 6573 6f75 7263 6520 3d20   imm_resource = 
-0000cd40: 496d 6d75 6e69 7a61 7469 6f6e 286a 736f  Immunization(jso
-0000cd50: 6e64 6963 743d 696d 6d5f 6469 6374 290a  ndict=imm_dict).
-0000cd60: 2020 2020 2020 2020 7365 6c66 2e66 726f          self.fro
-0000cd70: 6d5f 6668 6972 5f72 6573 6f75 7263 6528  m_fhir_resource(
-0000cd80: 696d 6d75 6e69 7a61 7469 6f6e 3d69 6d6d  immunization=imm
-0000cd90: 5f72 6573 6f75 7263 6529 0a0a 2020 2020  _resource)..    
-0000cda0: 6465 6620 6672 6f6d 5f66 6869 725f 7265  def from_fhir_re
-0000cdb0: 736f 7572 6365 2873 656c 662c 2069 6d6d  source(self, imm
-0000cdc0: 756e 697a 6174 696f 6e3d 4e6f 6e65 2c20  unization=None, 
-0000cdd0: 636f 6469 6e67 5f73 7973 7465 6d3d 4e6f  coding_system=No
-0000cde0: 6e65 2c20 636f 6469 6e67 5f76 6572 7369  ne, coding_versi
-0000cdf0: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
-0000ce00: 2020 6966 2069 6d6d 756e 697a 6174 696f    if immunizatio
-0000ce10: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-0000ce20: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
-0000ce30: 696f 6e20 3d20 7365 6c66 2e66 6869 725f  ion = self.fhir_
-0000ce40: 7265 736f 7572 6365 0a0a 2020 2020 2020  resource..      
-0000ce50: 2020 7365 6c66 2e66 6869 725f 7265 736f    self.fhir_reso
-0000ce60: 7572 6365 203d 2069 6d6d 756e 697a 6174  urce = immunizat
-0000ce70: 696f 6e0a 2020 2020 2020 2020 7365 6c66  ion.        self
-0000ce80: 2e69 6420 3d20 7365 6c66 2e67 6574 5f69  .id = self.get_i
-0000ce90: 6428 290a 2020 2020 2020 2020 616e 7469  d().        anti
-0000cea0: 6765 6e20 3d20 7365 6c66 2e67 6574 5f61  gen = self.get_a
-0000ceb0: 6e74 6967 656e 5f73 7461 7475 735f 616e  ntigen_status_an
-0000cec0: 7469 6765 6e28 290a 2020 2020 2020 2020  tigen().        
-0000ced0: 616e 7469 6765 6e5f 636f 6469 6e67 203d  antigen_coding =
-0000cee0: 2073 656c 662e 6765 745f 636f 6465 6162   self.get_codeab
-0000cef0: 6c65 5f63 6f6e 6365 7074 5f63 6f64 696e  le_concept_codin
-0000cf00: 6728 0a20 2020 2020 2020 2020 2020 2063  g(.            c
-0000cf10: 6f64 6561 626c 655f 636f 6e63 6570 743d  odeable_concept=
-0000cf20: 616e 7469 6765 6e2e 7661 6c75 6543 6f64  antigen.valueCod
-0000cf30: 6561 626c 6543 6f6e 6365 7074 2c0a 2020  eableConcept,.  
-0000cf40: 2020 2020 2020 2020 2020 636f 6469 6e67            coding
-0000cf50: 5f73 7973 7465 6d3d 636f 6469 6e67 5f73  _system=coding_s
-0000cf60: 7973 7465 6d2c 0a20 2020 2020 2020 2020  ystem,.         
-0000cf70: 2020 2063 6f64 696e 675f 7665 7273 696f     coding_versio
-0000cf80: 6e3d 636f 6469 6e67 5f76 6572 7369 6f6e  n=coding_version
-0000cf90: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000cfa0: 6e74 6967 656e 5f63 6f64 6520 3d20 616e  ntigen_code = an
-0000cfb0: 7469 6765 6e5f 636f 6469 6e67 2e63 6f64  tigen_coding.cod
-0000cfc0: 650a 2020 2020 2020 2020 7365 6c66 2e61  e.        self.a
-0000cfd0: 6e74 6967 656e 5f64 6973 706c 6179 203d  ntigen_display =
-0000cfe0: 2061 6e74 6967 656e 5f63 6f64 696e 672e   antigen_coding.
-0000cff0: 6469 7370 6c61 790a 2020 2020 2020 2020  display.        
-0000d000: 7365 6c66 2e61 6e74 6967 656e 5f69 6420  self.antigen_id 
-0000d010: 3d20 616e 7469 6765 6e5f 636f 6469 6e67  = antigen_coding
-0000d020: 2e69 640a 2020 2020 2020 2020 646f 7365  .id.        dose
-0000d030: 5f6e 756d 6265 7220 3d20 7365 6c66 2e67  _number = self.g
-0000d040: 6574 5f61 6e74 6967 656e 5f73 7461 7475  et_antigen_statu
-0000d050: 735f 646f 7365 5f6e 756d 6265 7228 290a  s_dose_number().
-0000d060: 2020 2020 2020 2020 7365 6c66 2e61 6e74          self.ant
-0000d070: 6967 656e 5f64 6f73 655f 6e75 6d62 6572  igen_dose_number
-0000d080: 203d 2064 6f73 655f 6e75 6d62 6572 2e76   = dose_number.v
-0000d090: 616c 7565 496e 7465 6765 720a 2020 2020  alueInteger.    
-0000d0a0: 2020 2020 616e 7469 6765 6e5f 7374 6174      antigen_stat
-0000d0b0: 7573 203d 2073 656c 662e 6765 745f 616e  us = self.get_an
-0000d0c0: 7469 6765 6e5f 7374 6174 7573 5f73 7461  tigen_status_sta
-0000d0d0: 7475 7328 290a 2020 2020 2020 2020 616e  tus().        an
-0000d0e0: 7469 6765 6e5f 7374 6174 7573 5f63 6f64  tigen_status_cod
-0000d0f0: 6520 3d20 7365 6c66 2e67 6574 5f63 6f64  e = self.get_cod
-0000d100: 6561 626c 655f 636f 6e63 6570 745f 636f  eable_concept_co
-0000d110: 6469 6e67 280a 2020 2020 2020 2020 2020  ding(.          
-0000d120: 2020 636f 6465 6162 6c65 5f63 6f6e 6365    codeable_conce
-0000d130: 7074 3d61 6e74 6967 656e 5f73 7461 7475  pt=antigen_statu
-0000d140: 732e 7661 6c75 6543 6f64 6561 626c 6543  s.valueCodeableC
-0000d150: 6f6e 6365 7074 2c0a 2020 2020 2020 2020  oncept,.        
-0000d160: 2020 2020 636f 6469 6e67 5f73 7973 7465      coding_syste
-0000d170: 6d3d 636f 6469 6e67 5f73 7973 7465 6d2c  m=coding_system,
-0000d180: 0a20 2020 2020 2020 2020 2020 2063 6f64  .            cod
-0000d190: 696e 675f 7665 7273 696f 6e3d 636f 6469  ing_version=codi
-0000d1a0: 6e67 5f76 6572 7369 6f6e 290a 2020 2020  ng_version).    
-0000d1b0: 2020 2020 7365 6c66 2e61 6e74 6967 656e      self.antigen
-0000d1c0: 5f73 7461 7475 735f 636f 6465 203d 2061  _status_code = a
-0000d1d0: 6e74 6967 656e 5f73 7461 7475 735f 636f  ntigen_status_co
-0000d1e0: 6465 2e63 6f64 650a 2020 2020 2020 2020  de.code.        
-0000d1f0: 7365 6c66 2e61 6e74 6967 656e 5f73 7461  self.antigen_sta
-0000d200: 7475 735f 6469 7370 6c61 7920 3d20 616e  tus_display = an
-0000d210: 7469 6765 6e5f 7374 6174 7573 5f63 6f64  tigen_status_cod
-0000d220: 652e 6469 7370 6c61 790a 2020 2020 2020  e.display.      
-0000d230: 2020 7365 6c66 2e61 6e74 6967 656e 5f73    self.antigen_s
-0000d240: 7461 7475 735f 6964 203d 2061 6e74 6967  tatus_id = antig
-0000d250: 656e 5f73 7461 7475 735f 636f 6465 2e69  en_status_code.i
-0000d260: 640a 2020 2020 2020 2020 7365 6c66 2e75  d.        self.u
-0000d270: 7064 6174 6564 5f62 7920 3d20 7365 6c66  pdated_by = self
-0000d280: 2e67 6574 5f6d 6574 615f 7570 6461 7465  .get_meta_update
-0000d290: 645f 6279 2829 0a20 2020 2020 2020 2073  d_by().        s
-0000d2a0: 656c 662e 6372 6561 7465 645f 6279 203d  elf.created_by =
-0000d2b0: 2073 656c 662e 6765 745f 6d65 7461 5f63   self.get_meta_c
-0000d2c0: 7265 6174 6564 5f62 7928 290a 2020 2020  reated_by().    
-0000d2d0: 2020 2020 7365 6c66 2e63 7265 6174 696f      self.creatio
-0000d2e0: 6e5f 6461 7465 203d 2073 656c 662e 6765  n_date = self.ge
-0000d2f0: 745f 6d65 7461 5f63 7265 6174 696f 6e5f  t_meta_creation_
-0000d300: 6461 7465 2829 2e69 736f 7374 7269 6e67  date().isostring
-0000d310: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-0000d320: 7273 696f 6e5f 6964 203d 2073 656c 662e  rsion_id = self.
-0000d330: 6765 745f 6d65 7461 5f76 6572 7369 6f6e  get_meta_version
-0000d340: 5f69 6428 290a 2020 2020 2020 2020 7365  _id().        se
-0000d350: 6c66 2e6c 6173 745f 7570 6461 7465 6420  lf.last_updated 
-0000d360: 3d20 7365 6c66 2e67 6574 5f6d 6574 615f  = self.get_meta_
-0000d370: 6c61 7374 5f75 7064 6174 6564 2829 0a20  last_updated(). 
-0000d380: 2020 2020 2020 2073 656c 662e 7072 6f66         self.prof
-0000d390: 696c 6520 3d20 7365 6c66 2e67 6574 5f6d  ile = self.get_m
-0000d3a0: 6574 615f 7072 6f66 696c 6528 290a 2020  eta_profile().  
-0000d3b0: 2020 2020 2020 7365 6c66 2e6f 7267 616e        self.organ
-0000d3c0: 697a 6174 696f 6e20 3d20 7365 6c66 2e67  ization = self.g
-0000d3d0: 6574 5f63 6f6e 7461 696e 6564 5f6f 7267  et_contained_org
-0000d3e0: 616e 697a 6174 696f 6e28 290a 2020 2020  anization().    
-0000d3f0: 2020 2020 6f76 6572 7269 6465 5f73 7461      override_sta
-0000d400: 7475 735f 6578 7465 6e73 696f 6e20 3d20  tus_extension = 
-0000d410: 7365 6c66 2e67 6574 5f6f 7665 7272 6964  self.get_overrid
-0000d420: 655f 7374 6174 7573 2829 0a20 2020 2020  e_status().     
-0000d430: 2020 2069 6620 6f76 6572 7269 6465 5f73     if override_s
-0000d440: 7461 7475 735f 6578 7465 6e73 696f 6e20  tatus_extension 
-0000d450: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000d460: 2020 2020 2020 2020 206f 7665 7272 6964           overrid
-0000d470: 655f 7374 6174 7573 5f63 6f64 696e 6720  e_status_coding 
-0000d480: 3d20 7365 6c66 2e67 6574 5f63 6f64 6561  = self.get_codea
-0000d490: 626c 655f 636f 6e63 6570 745f 636f 6469  ble_concept_codi
-0000d4a0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
-0000d4b0: 2020 2020 636f 6465 6162 6c65 5f63 6f6e      codeable_con
-0000d4c0: 6365 7074 3d6f 7665 7272 6964 655f 7374  cept=override_st
-0000d4d0: 6174 7573 5f65 7874 656e 7369 6f6e 2e76  atus_extension.v
-0000d4e0: 616c 7565 436f 6465 6162 6c65 436f 6e63  alueCodeableConc
-0000d4f0: 6570 742c 0a20 2020 2020 2020 2020 2020  ept,.           
-0000d500: 2020 2020 2063 6f64 696e 675f 7379 7374       coding_syst
-0000d510: 656d 3d63 6f64 696e 675f 7379 7374 656d  em=coding_system
-0000d520: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d530: 2020 636f 6469 6e67 5f76 6572 7369 6f6e    coding_version
-0000d540: 3d63 6f64 696e 675f 7665 7273 696f 6e29  =coding_version)
-0000d550: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d560: 662e 6f76 6572 7269 6465 5f73 7461 7475  f.override_statu
-0000d570: 735f 636f 6465 203d 206f 7665 7272 6964  s_code = overrid
-0000d580: 655f 7374 6174 7573 5f63 6f64 696e 672e  e_status_coding.
-0000d590: 636f 6465 0a20 2020 2020 2020 2020 2020  code.           
-0000d5a0: 2073 656c 662e 6f76 6572 7269 6465 5f73   self.override_s
-0000d5b0: 7461 7475 735f 6469 7370 6c61 7920 3d20  tatus_display = 
-0000d5c0: 6f76 6572 7269 6465 5f73 7461 7475 735f  override_status_
-0000d5d0: 636f 6469 6e67 2e64 6973 706c 6179 0a20  coding.display. 
-0000d5e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d5f0: 6f76 6572 7269 6465 5f73 7461 7475 735f  override_status_
-0000d600: 6964 203d 206f 7665 7272 6964 655f 7374  id = override_st
-0000d610: 6174 7573 5f63 6f64 696e 672e 6964 0a20  atus_coding.id. 
-0000d620: 2020 2020 2020 2073 656c 662e 6c6f 745f         self.lot_
-0000d630: 6964 203d 2073 656c 662e 6765 745f 6c6f  id = self.get_lo
-0000d640: 745f 6964 2829 0a20 2020 2020 2020 2073  t_id().        s
-0000d650: 656c 662e 7472 6164 655f 6e61 6d65 203d  elf.trade_name =
-0000d660: 2073 656c 662e 6765 745f 7472 6164 655f   self.get_trade_
-0000d670: 6e61 6d65 2829 0a20 2020 2020 2020 2073  name().        s
-0000d680: 656c 662e 7374 6174 7573 203d 2073 656c  elf.status = sel
-0000d690: 662e 6765 745f 7374 6174 7573 2829 0a20  f.get_status(). 
-0000d6a0: 2020 2020 2020 2073 656c 662e 6461 7465         self.date
-0000d6b0: 203d 2073 656c 662e 6765 745f 6461 7465   = self.get_date
-0000d6c0: 2829 2e69 736f 7374 7269 6e67 0a20 2020  ().isostring.   
-0000d6d0: 2020 2020 2076 6163 6369 6e65 5f63 6f64       vaccine_cod
-0000d6e0: 6520 3d20 7365 6c66 2e67 6574 5f76 6163  e = self.get_vac
-0000d6f0: 6369 6e65 5f63 6f64 6528 0a20 2020 2020  cine_code(.     
-0000d700: 2020 2020 2020 2063 6f64 696e 675f 7379         coding_sy
-0000d710: 7374 656d 3d63 6f64 696e 675f 7379 7374  stem=coding_syst
-0000d720: 656d 2c0a 2020 2020 2020 2020 2020 2020  em,.            
-0000d730: 636f 6469 6e67 5f76 6572 7369 6f6e 3d63  coding_version=c
-0000d740: 6f64 696e 675f 7665 7273 696f 6e29 0a20  oding_version). 
-0000d750: 2020 2020 2020 2073 656c 662e 7661 6363         self.vacc
-0000d760: 696e 655f 636f 6465 5f63 6f64 6520 3d20  ine_code_code = 
-0000d770: 7661 6363 696e 655f 636f 6465 2e63 6f64  vaccine_code.cod
-0000d780: 650a 2020 2020 2020 2020 7365 6c66 2e76  e.        self.v
-0000d790: 6163 6369 6e65 5f63 6f64 655f 6469 7370  accine_code_disp
-0000d7a0: 6c61 7920 3d20 7661 6363 696e 655f 636f  lay = vaccine_co
-0000d7b0: 6465 2e64 6973 706c 6179 0a20 2020 2020  de.display.     
-0000d7c0: 2020 2073 656c 662e 7661 6363 696e 655f     self.vaccine_
-0000d7d0: 636f 6465 5f69 6420 3d20 7661 6363 696e  code_id = vaccin
-0000d7e0: 655f 636f 6465 2e69 640a 2020 2020 2020  e_code.id.      
-0000d7f0: 2020 7365 6c66 2e70 6174 6965 6e74 203d    self.patient =
-0000d800: 2073 656c 662e 6765 745f 7061 7469 656e   self.get_patien
-0000d810: 7428 696d 6d75 6e69 7a61 7469 6f6e 3d69  t(immunization=i
-0000d820: 6d6d 756e 697a 6174 696f 6e29 0a20 2020  mmunization).   
-0000d830: 2020 2020 2073 656c 662e 7061 7469 656e       self.patien
-0000d840: 745f 7265 6665 7265 6e63 6520 3d20 7365  t_reference = se
-0000d850: 6c66 2e67 6574 5f70 6174 6965 6e74 5f72  lf.get_patient_r
-0000d860: 6566 6572 656e 6365 2869 6d6d 756e 697a  eference(immuniz
-0000d870: 6174 696f 6e3d 696d 6d75 6e69 7a61 7469  ation=immunizati
-0000d880: 6f6e 290a 2020 2020 2020 2020 7065 7266  on).        perf
-0000d890: 6f72 6d65 725f 7265 6665 7265 6e63 6520  ormer_reference 
-0000d8a0: 3d20 7365 6c66 2e67 6574 5f70 6572 666f  = self.get_perfo
-0000d8b0: 726d 6572 5f72 6566 6572 656e 6365 2869  rmer_reference(i
-0000d8c0: 6d6d 756e 697a 6174 696f 6e3d 696d 6d75  mmunization=immu
-0000d8d0: 6e69 7a61 7469 6f6e 290a 2020 2020 2020  nization).      
-0000d8e0: 2020 6966 2070 6572 666f 726d 6572 5f72    if performer_r
-0000d8f0: 6566 6572 656e 6365 2069 7320 6e6f 7420  eference is not 
-0000d900: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000d910: 2020 7365 6c66 2e70 6572 666f 726d 6572    self.performer
-0000d920: 5f72 6566 6572 656e 6365 203d 2070 6572  _reference = per
-0000d930: 666f 726d 6572 5f72 6566 6572 656e 6365  former_reference
-0000d940: 2e72 6566 6572 656e 6365 0a20 2020 2020  .reference.     
-0000d950: 2020 2020 2020 2073 656c 662e 7065 7266         self.perf
-0000d960: 6f72 6d65 725f 6469 7370 6c61 7920 3d20  ormer_display = 
-0000d970: 7065 7266 6f72 6d65 725f 7265 6665 7265  performer_refere
-0000d980: 6e63 652e 6469 7370 6c61 790a 2020 2020  nce.display.    
-0000d990: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000d9a0: 2020 2020 2020 7365 6c66 2e70 6572 666f        self.perfo
-0000d9b0: 726d 6572 203d 2073 656c 662e 6765 745f  rmer = self.get_
-0000d9c0: 7065 7266 6f72 6d65 7228 696d 6d75 6e69  performer(immuni
-0000d9d0: 7a61 7469 6f6e 3d69 6d6d 756e 697a 6174  zation=immunizat
-0000d9e0: 696f 6e29 0a0a 2020 2020 2020 2020 7365  ion)..        se
-0000d9f0: 6c66 2e6c 6f63 6174 696f 6e20 3d20 7365  lf.location = se
-0000da00: 6c66 2e67 6574 5f6c 6f63 6174 696f 6e28  lf.get_location(
-0000da10: 696d 6d75 6e69 7a61 7469 6f6e 3d69 6d6d  immunization=imm
-0000da20: 756e 697a 6174 696f 6e29 0a20 2020 2020  unization).     
-0000da30: 2020 206c 6f63 6174 696f 6e5f 7265 6620     location_ref 
-0000da40: 3d20 7365 6c66 2e67 6574 5f6c 6f63 6174  = self.get_locat
-0000da50: 696f 6e5f 7265 6665 7265 6e63 6528 696d  ion_reference(im
-0000da60: 6d75 6e69 7a61 7469 6f6e 3d69 6d6d 756e  munization=immun
-0000da70: 697a 6174 696f 6e29 0a20 2020 2020 2020  ization).       
-0000da80: 2069 6620 6c6f 6361 7469 6f6e 5f72 6566   if location_ref
-0000da90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000daa0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-0000dab0: 6f63 6174 696f 6e5f 7265 6665 7265 6e63  ocation_referenc
-0000dac0: 6520 3d20 6c6f 6361 7469 6f6e 5f72 6566  e = location_ref
-0000dad0: 2e72 6566 6572 656e 6365 0a20 2020 2020  .reference.     
-0000dae0: 2020 2020 2020 2073 656c 662e 6c6f 6361         self.loca
-0000daf0: 7469 6f6e 5f64 6973 706c 6179 203d 206c  tion_display = l
-0000db00: 6f63 6174 696f 6e5f 7265 662e 6469 7370  ocation_ref.disp
-0000db10: 6c61 790a 2020 2020 2020 2020 7365 6c66  lay.        self
-0000db20: 2e6c 6f74 5f6e 756d 6265 7220 3d20 7365  .lot_number = se
-0000db30: 6c66 2e67 6574 5f6c 6f74 5f6e 756d 6265  lf.get_lot_numbe
-0000db40: 7228 696d 6d75 6e69 7a61 7469 6f6e 3d69  r(immunization=i
-0000db50: 6d6d 756e 697a 6174 696f 6e29 0a20 2020  mmunization).   
-0000db60: 2020 2020 2073 656c 662e 6578 7069 7261       self.expira
-0000db70: 7469 6f6e 5f64 6174 6520 3d20 7365 6c66  tion_date = self
-0000db80: 2e67 6574 5f65 7870 6972 6174 696f 6e5f  .get_expiration_
-0000db90: 6461 7465 2869 6d6d 756e 697a 6174 696f  date(immunizatio
-0000dba0: 6e3d 696d 6d75 6e69 7a61 7469 6f6e 290a  n=immunization).
-0000dbb0: 2020 2020 2020 2020 7369 7465 203d 2073          site = s
-0000dbc0: 656c 662e 6765 745f 7369 7465 280a 2020  elf.get_site(.  
-0000dbd0: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
-0000dbe0: 7a61 7469 6f6e 3d69 6d6d 756e 697a 6174  zation=immunizat
-0000dbf0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-0000dc00: 2063 6f64 696e 675f 7379 7374 656d 3d63   coding_system=c
-0000dc10: 6f64 696e 675f 7379 7374 656d 2c0a 2020  oding_system,.  
-0000dc20: 2020 2020 2020 2020 2020 636f 6469 6e67            coding
-0000dc30: 5f76 6572 7369 6f6e 3d63 6f64 696e 675f  _version=coding_
-0000dc40: 7665 7273 696f 6e29 0a20 2020 2020 2020  version).       
-0000dc50: 2069 6620 7369 7465 2069 7320 6e6f 7420   if site is not 
-0000dc60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000dc70: 2020 7365 6c66 2e73 6974 655f 636f 6465    self.site_code
-0000dc80: 203d 2073 6974 652e 636f 6465 0a20 2020   = site.code.   
-0000dc90: 2020 2020 2020 2020 2073 656c 662e 7369           self.si
-0000dca0: 7465 5f64 6973 706c 6179 203d 2073 6974  te_display = sit
-0000dcb0: 652e 6469 7370 6c61 790a 2020 2020 2020  e.display.      
-0000dcc0: 2020 2020 2020 7365 6c66 2e73 6974 655f        self.site_
-0000dcd0: 6964 203d 2073 6974 652e 6964 0a20 2020  id = site.id.   
-0000dce0: 2020 2020 2072 6f75 7465 5f63 6f64 696e       route_codin
-0000dcf0: 6720 3d20 7365 6c66 2e67 6574 5f63 6f64  g = self.get_cod
-0000dd00: 6561 626c 655f 636f 6e63 6570 745f 636f  eable_concept_co
-0000dd10: 6469 6e67 280a 2020 2020 2020 2020 2020  ding(.          
-0000dd20: 2020 696d 6d75 6e69 7a61 7469 6f6e 2e72    immunization.r
-0000dd30: 6f75 7465 2c0a 2020 2020 2020 2020 2020  oute,.          
-0000dd40: 2020 636f 6469 6e67 5f73 7973 7465 6d3d    coding_system=
-0000dd50: 636f 6469 6e67 5f73 7973 7465 6d2c 0a20  coding_system,. 
-0000dd60: 2020 2020 2020 2020 2020 2063 6f64 696e             codin
-0000dd70: 675f 7665 7273 696f 6e3d 636f 6469 6e67  g_version=coding
-0000dd80: 5f76 6572 7369 6f6e 290a 2020 2020 2020  _version).      
-0000dd90: 2020 7365 6c66 2e72 6f75 7465 5f63 6f64    self.route_cod
-0000dda0: 6520 3d20 726f 7574 655f 636f 6469 6e67  e = route_coding
-0000ddb0: 2e63 6f64 650a 2020 2020 2020 2020 7365  .code.        se
-0000ddc0: 6c66 2e72 6f75 7465 5f64 6973 706c 6179  lf.route_display
-0000ddd0: 203d 2072 6f75 7465 5f63 6f64 696e 672e   = route_coding.
-0000dde0: 6469 7370 6c61 790a 2020 2020 2020 2020  display.        
-0000ddf0: 7365 6c66 2e72 6f75 7465 5f69 6420 3d20  self.route_id = 
-0000de00: 726f 7574 655f 636f 6469 6e67 2e69 640a  route_coding.id.
-0000de10: 2020 2020 2020 2020 646f 7365 5f71 7561          dose_qua
-0000de20: 6e74 6974 7920 3d20 7365 6c66 2e67 6574  ntity = self.get
-0000de30: 5f64 6f73 655f 7175 616e 7469 7479 2869  _dose_quantity(i
-0000de40: 6d6d 756e 697a 6174 696f 6e3d 696d 6d75  mmunization=immu
-0000de50: 6e69 7a61 7469 6f6e 290a 2020 2020 2020  nization).      
-0000de60: 2020 6966 2064 6f73 655f 7175 616e 7469    if dose_quanti
-0000de70: 7479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ty is not None:.
-0000de80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000de90: 2e64 6f73 655f 7175 616e 7469 7479 5f63  .dose_quantity_c
-0000dea0: 6f64 6520 3d20 646f 7365 5f71 7561 6e74  ode = dose_quant
-0000deb0: 6974 792e 636f 6465 0a20 2020 2020 2020  ity.code.       
-0000dec0: 2020 2020 2073 656c 662e 646f 7365 5f71       self.dose_q
-0000ded0: 7561 6e74 6974 795f 756e 6974 203d 2064  uantity_unit = d
-0000dee0: 6f73 655f 7175 616e 7469 7479 2e75 6e69  ose_quantity.uni
-0000def0: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
-0000df00: 6c66 2e64 6f73 655f 7175 616e 7469 7479  lf.dose_quantity
-0000df10: 5f76 616c 7565 203d 2064 6f73 655f 7175  _value = dose_qu
-0000df20: 616e 7469 7479 2e76 616c 7565 0a20 2020  antity.value.   
-0000df30: 2020 2020 2073 656c 662e 7265 6173 6f6e       self.reason
-0000df40: 203d 2073 656c 662e 6765 745f 7265 6173   = self.get_reas
-0000df50: 6f6e 7328 696d 6d75 6e69 7a61 7469 6f6e  ons(immunization
-0000df60: 3d69 6d6d 756e 697a 6174 696f 6e2c 636f  =immunization,co
-0000df70: 6469 6e67 5f73 7973 7465 6d3d 636f 6469  ding_system=codi
-0000df80: 6e67 5f73 7973 7465 6d2c 2063 6f64 696e  ng_system, codin
-0000df90: 675f 7665 7273 696f 6e3d 636f 6469 6e67  g_version=coding
-0000dfa0: 5f76 6572 7369 6f6e 290a 0a63 6c61 7373  _version)..class
-0000dfb0: 2050 6174 6965 6e74 4648 4952 2842 6173   PatientFHIR(Bas
-0000dfc0: 6546 4849 5229 3a0a 2020 2020 7265 736f  eFHIR):.    reso
-0000dfd0: 7572 6365 5f74 7970 6520 3d20 2750 6174  urce_type = 'Pat
-0000dfe0: 6965 6e74 270a 2020 2020 6465 6661 756c  ient'.    defaul
-0000dff0: 745f 636f 6469 6e67 5f73 7973 7465 6d20  t_coding_system 
-0000e000: 3d20 2768 7474 703a 2f2f 7777 772e 7361  = 'http://www.sa
-0000e010: 6e74 6570 7562 6c69 7175 652e 7274 7373  ntepublique.rtss
-0000e020: 2e71 632e 6361 2f73 6970 6d69 2f66 612f  .qc.ca/sipmi/fa/
-0000e030: 312e 302e 302f 766f 6361 6275 6c61 7279  1.0.0/vocabulary
-0000e040: 270a 2020 2020 6465 6661 756c 745f 636f  '.    default_co
-0000e050: 6469 6e67 5f76 6572 7369 6f6e 203d 2022  ding_version = "
-0000e060: 312e 302e 3022 0a20 2020 206e 616d 5f69  1.0.0".    nam_i
-0000e070: 6465 6e74 6966 6965 725f 6578 7465 6e73  dentifier_extens
-0000e080: 696f 6e5f 7572 6c20 3d20 2268 7474 703a  ion_url = "http:
-0000e090: 2f2f 7777 772e 7361 6e74 6570 7562 6c69  //www.santepubli
-0000e0a0: 7175 652e 7274 7373 2e71 632e 6361 2f73  que.rtss.qc.ca/s
-0000e0b0: 6970 6d69 2f66 612f 312e 302e 302f 6578  ipmi/fa/1.0.0/ex
-0000e0c0: 7465 6e73 696f 6e73 2f23 7061 7469 656e  tensions/#patien
-0000e0d0: 742f 6865 616c 7468 6361 7264 6f72 6967  t/healthcardorig
-0000e0e0: 696e 220a 2020 2020 6e61 6d5f 6964 656e  in".    nam_iden
-0000e0f0: 7469 6669 6572 5f73 7973 7465 6d20 3d20  tifier_system = 
-0000e100: 2268 7474 703a 2f2f 7777 772e 7361 6e74  "http://www.sant
-0000e110: 6570 7562 6c69 7175 652e 7274 7373 2e71  epublique.rtss.q
-0000e120: 632e 6361 2f73 6970 6d69 2f66 612f 312e  c.ca/sipmi/fa/1.
-0000e130: 302e 302f 766f 6361 6275 6c61 7279 2f69  0.0/vocabulary/i
-0000e140: 6465 6e74 6966 6965 7254 7970 653f 636f  dentifierType?co
-0000e150: 6465 3d4e 414d 220a 2020 2020 6e69 755f  de=NAM".    niu_
-0000e160: 6964 656e 7469 6669 6572 5f73 7973 7465  identifier_syste
-0000e170: 6d20 3d20 2268 7474 703a 2f2f 7777 772e  m = "http://www.
-0000e180: 7361 6e74 6570 7562 6c69 7175 652e 7274  santepublique.rt
-0000e190: 7373 2e71 632e 6361 2f73 6970 6d69 2f66  ss.qc.ca/sipmi/f
-0000e1a0: 612f 312e 302e 302f 766f 6361 6275 6c61  a/1.0.0/vocabula
-0000e1b0: 7279 2f69 6465 6e74 6966 6965 7254 7970  ry/identifierTyp
-0000e1c0: 653f 636f 6465 3d4e 4955 5522 0a20 2020  e?code=NIUU".   
-0000e1d0: 2061 7563 756e 5f69 6465 6e74 6966 6965   aucun_identifie
-0000e1e0: 725f 7379 7374 656d 203d 2022 6874 7470  r_system = "http
-0000e1f0: 3a2f 2f77 7777 2e73 616e 7465 7075 626c  ://www.santepubl
-0000e200: 6971 7565 2e72 7473 732e 7163 2e63 612f  ique.rtss.qc.ca/
-0000e210: 7369 706d 692f 6661 2f31 2e30 2e30 2f76  sipmi/fa/1.0.0/v
-0000e220: 6f63 6162 756c 6172 792f 6964 656e 7469  ocabulary/identi
-0000e230: 6669 6572 5479 7065 3f63 6f64 653d 4155  fierType?code=AU
-0000e240: 4355 4e22 0a20 2020 206d 6174 6368 7261  CUN".    matchra
-0000e250: 6d71 5f65 7874 656e 7369 6f6e 5f75 726c  mq_extension_url
-0000e260: 203d 2022 6874 7470 3a2f 2f77 7777 2e73   = "http://www.s
-0000e270: 616e 7465 7075 626c 6971 7565 2e72 7473  antepublique.rts
-0000e280: 732e 7163 2e63 612f 7369 706d 692f 6661  s.qc.ca/sipmi/fa
-0000e290: 2f31 2e30 2e30 2f65 7874 656e 7369 6f6e  /1.0.0/extension
-0000e2a0: 732f 2370 6174 6965 6e74 2f6d 6174 6368  s/#patient/match
-0000e2b0: 7261 6d71 220a 2020 2020 6964 203d 204e  ramq".    id = N
-0000e2c0: 6f6e 650a 2020 2020 7573 6572 5f6e 616d  one.    user_nam
-0000e2d0: 6520 3d20 4e6f 6e65 0a20 2020 2063 7265  e = None.    cre
-0000e2e0: 6174 696f 6e5f 6461 7465 203d 204e 6f6e  ation_date = Non
-0000e2f0: 650a 2020 2020 7570 6461 7465 5f74 696d  e.    update_tim
-0000e300: 6573 7461 6d70 203d 204e 6f6e 650a 2020  estamp = None.  
-0000e310: 2020 6d61 7463 6872 616d 7120 3d20 4e6f    matchramq = No
-0000e320: 6e65 0a20 2020 2061 6374 6976 6520 3d20  ne.    active = 
-0000e330: 5472 7565 0a20 2020 206e 616d 203d 204e  True.    nam = N
-0000e340: 6f6e 650a 2020 2020 6e69 7520 3d20 4e6f  one.    niu = No
-0000e350: 6e65 0a20 2020 2066 616d 696c 795f 6e61  ne.    family_na
-0000e360: 6d65 203d 204e 6f6e 650a 2020 2020 6769  me = None.    gi
-0000e370: 7665 6e5f 6e61 6d65 203d 204e 6f6e 650a  ven_name = None.
-0000e380: 2020 2020 7068 6f6e 655f 6e75 6d62 6572      phone_number
-0000e390: 203d 204e 6f6e 650a 2020 2020 6765 6e64   = None.    gend
-0000e3a0: 6572 203d 204e 6f6e 650a 2020 2020 6269  er = None.    bi
-0000e3b0: 7274 685f 6461 7465 203d 204e 6f6e 650a  rth_date = None.
-0000e3c0: 2020 2020 6465 6365 6173 6564 5f62 6f6f      deceased_boo
-0000e3d0: 6c65 616e 203d 2046 616c 7365 0a20 2020  lean = False.   
-0000e3e0: 2061 6464 7265 7373 5f6c 696e 6520 3d20   address_line = 
-0000e3f0: 4e6f 6e65 0a20 2020 2061 6464 7265 7373  None.    address
-0000e400: 5f63 6974 7920 3d20 4e6f 6e65 0a20 2020  _city = None.   
-0000e410: 2061 6464 7265 7373 5f73 7461 7465 203d   address_state =
-0000e420: 204e 6f6e 650a 2020 2020 6164 6472 6573   None.    addres
-0000e430: 735f 706f 7374 616c 5f63 6f64 6520 3d20  s_postal_code = 
-0000e440: 4e6f 6e65 0a20 2020 2061 6464 7265 7373  None.    address
-0000e450: 5f63 6f75 6e74 7279 203d 204e 6f6e 650a  _country = None.
-0000e460: 2020 2020 6d6f 7468 6572 5f67 6976 656e      mother_given
-0000e470: 5f6e 616d 6520 3d20 4e6f 6e65 0a20 2020  _name = None.   
-0000e480: 206d 6f74 6865 725f 6661 6d69 6c79 5f6e   mother_family_n
-0000e490: 616d 6520 3d20 4e6f 6e65 0a20 2020 2066  ame = None.    f
-0000e4a0: 6174 6865 725f 6769 7665 6e5f 6e61 6d65  ather_given_name
-0000e4b0: 203d 204e 6f6e 650a 2020 2020 6661 7468   = None.    fath
-0000e4c0: 6572 5f66 616d 696c 795f 6e61 6d65 203d  er_family_name =
-0000e4d0: 204e 6f6e 650a 2020 2020 6261 7365 5f75   None.    base_u
-0000e4e0: 726c 203d 2022 220a 2020 2020 7061 7469  rl = "".    pati
-0000e4f0: 656e 745f 656e 6470 6f69 6e74 203d 2022  ent_endpoint = "
-0000e500: 7b30 7d2f 5061 7469 656e 7422 0a20 2020  {0}/Patient".   
-0000e510: 2070 6174 6965 6e74 5f69 645f 656e 6470   patient_id_endp
-0000e520: 6f69 6e74 203d 2022 7b30 7d2f 5061 7469  oint = "{0}/Pati
-0000e530: 656e 742f 7b31 7d22 0a20 2020 2070 6174  ent/{1}".    pat
-0000e540: 6965 6e74 5f6d 6174 6368 5f65 6e64 706f  ient_match_endpo
-0000e550: 696e 7420 3d20 227b 307d 2f50 6174 6965  int = "{0}/Patie
-0000e560: 6e74 2f24 6d61 7463 6822 0a20 2020 2070  nt/$match".    p
-0000e570: 6174 6965 6e74 5f64 6566 696e 6972 5f6e  atient_definir_n
-0000e580: 6975 5f65 6e64 706f 696e 7420 3d20 7061  iu_endpoint = pa
-0000e590: 7469 656e 745f 6964 5f65 6e64 706f 696e  tient_id_endpoin
-0000e5a0: 7420 2b20 222f 2464 6566 696e 6972 2d6e  t + "/$definir-n
-0000e5b0: 6975 220a 0a20 2020 2068 6561 6465 7273  iu"..    headers
-0000e5c0: 203d 207b 7d0a 2020 2020 6668 6972 5f72   = {}.    fhir_r
-0000e5d0: 6573 6f75 7263 6520 3d20 4e6f 6e65 0a20  esource = None. 
-0000e5e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0000e5f0: 7365 6c66 2c20 6261 7365 5f75 726c 3d4e  self, base_url=N
-0000e600: 6f6e 652c 2062 6173 655f 7572 693d 4e6f  one, base_uri=No
-0000e610: 6e65 2c20 7061 7469 656e 745f 6469 6374  ne, patient_dict
-0000e620: 3d4e 6f6e 652c 2074 6f6b 656e 3d4e 6f6e  =None, token=Non
-0000e630: 652c 2070 6174 6965 6e74 5f72 6573 6f75  e, patient_resou
-0000e640: 7263 655f 6469 6374 3d4e 6f6e 652c 2076  rce_dict=None, v
-0000e650: 616c 6964 6174 655f 6365 7274 733d 5472  alidate_certs=Tr
-0000e660: 7565 293a 0a20 2020 2020 2020 2073 7570  ue):.        sup
-0000e670: 6572 2829 2e5f 5f69 6e69 745f 5f28 6261  er().__init__(ba
-0000e680: 7365 5f75 726c 3d62 6173 655f 7572 6c2c  se_url=base_url,
-0000e690: 2062 6173 655f 7572 693d 6261 7365 5f75   base_uri=base_u
-0000e6a0: 7269 290a 2020 2020 2020 2020 7365 6c66  ri).        self
-0000e6b0: 2e76 616c 6964 6174 655f 6365 7274 7320  .validate_certs 
-0000e6c0: 3d20 7661 6c69 6461 7465 5f63 6572 7473  = validate_certs
-0000e6d0: 0a20 2020 2020 2020 2069 6620 7061 7469  .        if pati
-0000e6e0: 656e 745f 7265 736f 7572 6365 5f64 6963  ent_resource_dic
-0000e6f0: 7420 6973 204e 6f6e 6520 616e 6420 7061  t is None and pa
-0000e700: 7469 656e 745f 6469 6374 2069 7320 6e6f  tient_dict is no
-0000e710: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000e720: 2020 2020 7365 6c66 2e66 726f 6d5f 6469      self.from_di
-0000e730: 6374 2870 6174 6965 6e74 5f64 6963 7429  ct(patient_dict)
-0000e740: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e750: 662e 6668 6972 5f72 6573 6f75 7263 6520  f.fhir_resource 
-0000e760: 3d20 7365 6c66 2e70 6174 6965 6e74 5f64  = self.patient_d
-0000e770: 6963 745f 746f 5f66 6869 725f 7061 7469  ict_to_fhir_pati
-0000e780: 656e 7428 7061 7469 656e 745f 6469 6374  ent(patient_dict
-0000e790: 3d70 6174 6965 6e74 5f64 6963 742c 2070  =patient_dict, p
-0000e7a0: 6174 6965 6e74 3d50 6174 6965 6e74 2829  atient=Patient()
-0000e7b0: 290a 2020 2020 2020 2020 656c 6966 2070  ).        elif p
-0000e7c0: 6174 6965 6e74 5f72 6573 6f75 7263 655f  atient_resource_
-0000e7d0: 6469 6374 2069 7320 6e6f 7420 4e6f 6e65  dict is not None
-0000e7e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000e7f0: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
-0000e800: 203d 2050 6174 6965 6e74 286a 736f 6e64   = Patient(jsond
-0000e810: 6963 743d 7061 7469 656e 745f 7265 736f  ict=patient_reso
-0000e820: 7572 6365 5f64 6963 7429 0a20 2020 2020  urce_dict).     
-0000e830: 2020 2020 2020 2073 656c 662e 6672 6f6d         self.from
-0000e840: 5f66 6869 725f 7061 7469 656e 7428 290a  _fhir_patient().
-0000e850: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000e860: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0000e870: 6869 725f 7265 736f 7572 6365 203d 2050  hir_resource = P
-0000e880: 6174 6965 6e74 2829 0a0a 2020 2020 2020  atient()..      
-0000e890: 2020 6966 2062 6173 655f 7572 6c20 6973    if base_url is
-0000e8a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000e8b0: 2020 2020 2020 2073 656c 662e 6261 7365         self.base
-0000e8c0: 5f75 726c 203d 2062 6173 655f 7572 6c0a  _url = base_url.
-0000e8d0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-0000e8e0: 2020 2020 2073 656c 662e 7365 7448 6561       self.setHea
-0000e8f0: 6465 7273 2874 6f6b 656e 3d74 6f6b 656e  ders(token=token
-0000e900: 290a 0a20 2020 2064 6566 2066 726f 6d5f  )..    def from_
-0000e910: 6469 6374 2873 656c 662c 2070 6174 6965  dict(self, patie
-0000e920: 6e74 5f64 6963 7429 3a0a 2020 2020 2020  nt_dict):.      
-0000e930: 2020 7365 6c66 2e69 6420 3d20 7061 7469    self.id = pati
-0000e940: 656e 745f 6469 6374 5b27 6964 275d 2069  ent_dict['id'] i
-0000e950: 6620 2769 6427 2069 6e20 7061 7469 656e  f 'id' in patien
-0000e960: 745f 6469 6374 2065 6c73 6520 4e6f 6e65  t_dict else None
-0000e970: 0a20 2020 2020 2020 2073 656c 662e 6769  .        self.gi
-0000e980: 7665 6e5f 6e61 6d65 203d 2070 6174 6965  ven_name = patie
-0000e990: 6e74 5f64 6963 745b 2767 6976 656e 5f6e  nt_dict['given_n
-0000e9a0: 616d 6527 5d20 6966 2027 6769 7665 6e5f  ame'] if 'given_
-0000e9b0: 6e61 6d65 2720 696e 2070 6174 6965 6e74  name' in patient
-0000e9c0: 5f64 6963 7420 656c 7365 204e 6f6e 650a  _dict else None.
-0000e9d0: 2020 2020 2020 2020 7365 6c66 2e66 616d          self.fam
-0000e9e0: 696c 795f 6e61 6d65 203d 2070 6174 6965  ily_name = patie
-0000e9f0: 6e74 5f64 6963 745b 2766 616d 696c 795f  nt_dict['family_
-0000ea00: 6e61 6d65 275d 2069 6620 2766 616d 696c  name'] if 'famil
-0000ea10: 795f 6e61 6d65 2720 696e 2070 6174 6965  y_name' in patie
-0000ea20: 6e74 5f64 6963 7420 656c 7365 204e 6f6e  nt_dict else Non
-0000ea30: 650a 2020 2020 2020 2020 7365 6c66 2e61  e.        self.a
-0000ea40: 6374 6976 6520 3d20 7061 7469 656e 745f  ctive = patient_
-0000ea50: 6469 6374 5b27 6163 7469 7665 275d 2069  dict['active'] i
-0000ea60: 6620 2761 6374 6976 6527 2069 6e20 7061  f 'active' in pa
-0000ea70: 7469 656e 745f 6469 6374 2065 6c73 6520  tient_dict else 
-0000ea80: 5472 7565 0a20 2020 2020 2020 2073 656c  True.        sel
-0000ea90: 662e 6765 6e64 6572 203d 2070 6174 6965  f.gender = patie
-0000eaa0: 6e74 5f64 6963 745b 2767 656e 6465 7227  nt_dict['gender'
-0000eab0: 5d20 6966 2027 6765 6e64 6572 2720 696e  ] if 'gender' in
-0000eac0: 2070 6174 6965 6e74 5f64 6963 7420 656c   patient_dict el
-0000ead0: 7365 204e 6f6e 650a 2020 2020 2020 2020  se None.        
-0000eae0: 7365 6c66 2e62 6972 7468 5f64 6174 6520  self.birth_date 
-0000eaf0: 3d20 7061 7469 656e 745f 6469 6374 5b27  = patient_dict['
-0000eb00: 6269 7274 685f 6461 7465 275d 2069 6620  birth_date'] if 
-0000eb10: 2762 6972 7468 5f64 6174 6527 2069 6e20  'birth_date' in 
-0000eb20: 7061 7469 656e 745f 6469 6374 2065 6c73  patient_dict els
-0000eb30: 6520 4e6f 6e65 0a20 2020 2020 2020 2073  e None.        s
-0000eb40: 656c 662e 6e69 7520 3d20 7061 7469 656e  elf.niu = patien
-0000eb50: 745f 6469 6374 5b27 6e69 7527 5d20 6966  t_dict['niu'] if
-0000eb60: 2027 6e69 7527 2069 6e20 7061 7469 656e   'niu' in patien
-0000eb70: 745f 6469 6374 2065 6c73 6520 4e6f 6e65  t_dict else None
-0000eb80: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
-0000eb90: 6d20 3d20 7061 7469 656e 745f 6469 6374  m = patient_dict
-0000eba0: 5b27 6e61 6d27 5d20 6966 2027 6e61 6d27  ['nam'] if 'nam'
-0000ebb0: 2069 6e20 7061 7469 656e 745f 6469 6374   in patient_dict
-0000ebc0: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
-0000ebd0: 2020 2073 656c 662e 6164 6472 6573 735f     self.address_
-0000ebe0: 6c69 6e65 203d 2070 6174 6965 6e74 5f64  line = patient_d
-0000ebf0: 6963 745b 2761 6464 7265 7373 5f6c 696e  ict['address_lin
-0000ec00: 6527 5d20 6966 2027 6164 6472 6573 735f  e'] if 'address_
-0000ec10: 6c69 6e65 2720 696e 2070 6174 6965 6e74  line' in patient
-0000ec20: 5f64 6963 7420 656c 7365 204e 6f6e 650a  _dict else None.
-0000ec30: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
-0000ec40: 7265 7373 5f63 6974 7920 3d20 7061 7469  ress_city = pati
-0000ec50: 656e 745f 6469 6374 5b27 6164 6472 6573  ent_dict['addres
-0000ec60: 735f 6369 7479 275d 2069 6620 2761 6464  s_city'] if 'add
-0000ec70: 7265 7373 5f63 6974 7927 2069 6e20 7061  ress_city' in pa
-0000ec80: 7469 656e 745f 6469 6374 2065 6c73 6520  tient_dict else 
-0000ec90: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000eca0: 662e 6164 6472 6573 735f 7374 6174 6520  f.address_state 
-0000ecb0: 3d20 7061 7469 656e 745f 6469 6374 5b27  = patient_dict['
-0000ecc0: 6164 6472 6573 735f 7374 6174 6527 5d20  address_state'] 
-0000ecd0: 6966 2027 6164 6472 6573 735f 7374 6174  if 'address_stat
-0000ece0: 6527 2069 6e20 7061 7469 656e 745f 6469  e' in patient_di
-0000ecf0: 6374 2065 6c73 6520 4e6f 6e65 0a20 2020  ct else None.   
-0000ed00: 2020 2020 2073 656c 662e 6164 6472 6573       self.addres
-0000ed10: 735f 706f 7374 616c 5f63 6f64 6520 3d20  s_postal_code = 
-0000ed20: 7061 7469 656e 745f 6469 6374 5b27 6164  patient_dict['ad
-0000ed30: 6472 6573 735f 706f 7374 616c 5f63 6f64  dress_postal_cod
-0000ed40: 6527 5d20 6966 2027 6164 6472 6573 735f  e'] if 'address_
-0000ed50: 706f 7374 616c 5f63 6f64 6527 2069 6e20  postal_code' in 
-0000ed60: 7061 7469 656e 745f 6469 6374 2065 6c73  patient_dict els
-0000ed70: 6520 4e6f 6e65 0a20 2020 2020 2020 2073  e None.        s
-0000ed80: 656c 662e 6164 6472 6573 735f 636f 756e  elf.address_coun
-0000ed90: 7472 7920 3d20 7061 7469 656e 745f 6469  try = patient_di
-0000eda0: 6374 5b27 6164 6472 6573 735f 636f 756e  ct['address_coun
-0000edb0: 7472 7927 5d20 6966 2027 6164 6472 6573  try'] if 'addres
-0000edc0: 735f 636f 756e 7472 7927 2069 6e20 7061  s_country' in pa
-0000edd0: 7469 656e 745f 6469 6374 2065 6c73 6520  tient_dict else 
-0000ede0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-0000edf0: 662e 6d6f 7468 6572 5f67 6976 656e 5f6e  f.mother_given_n
-0000ee00: 616d 6520 3d20 7061 7469 656e 745f 6469  ame = patient_di
-0000ee10: 6374 5b27 6d6f 7468 6572 5f67 6976 656e  ct['mother_given
-0000ee20: 5f6e 616d 6527 5d20 6966 2027 6d6f 7468  _name'] if 'moth
-0000ee30: 6572 5f67 6976 656e 5f6e 616d 6527 2069  er_given_name' i
-0000ee40: 6e20 7061 7469 656e 745f 6469 6374 2065  n patient_dict e
-0000ee50: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
-0000ee60: 2073 656c 662e 6d6f 7468 6572 5f66 616d   self.mother_fam
-0000ee70: 696c 795f 6e61 6d65 203d 2070 6174 6965  ily_name = patie
-0000ee80: 6e74 5f64 6963 745b 276d 6f74 6865 725f  nt_dict['mother_
-0000ee90: 6661 6d69 6c79 5f6e 616d 6527 5d20 6966  family_name'] if
-0000eea0: 2027 6d6f 7468 6572 5f66 616d 696c 795f   'mother_family_
-0000eeb0: 6e61 6d65 2720 696e 2070 6174 6965 6e74  name' in patient
-0000eec0: 5f64 6963 7420 656c 7365 204e 6f6e 650a  _dict else None.
-0000eed0: 2020 2020 2020 2020 7365 6c66 2e66 6174          self.fat
-0000eee0: 6865 725f 6769 7665 6e5f 6e61 6d65 203d  her_given_name =
-0000eef0: 2070 6174 6965 6e74 5f64 6963 745b 2766   patient_dict['f
-0000ef00: 6174 6865 725f 6769 7665 6e5f 6e61 6d65  ather_given_name
-0000ef10: 275d 2069 6620 2766 6174 6865 725f 6769  '] if 'father_gi
-0000ef20: 7665 6e5f 6e61 6d65 2720 696e 2070 6174  ven_name' in pat
-0000ef30: 6965 6e74 5f64 6963 7420 656c 7365 204e  ient_dict else N
-0000ef40: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
-0000ef50: 2e66 6174 6865 725f 6661 6d69 6c79 5f6e  .father_family_n
-0000ef60: 616d 6520 3d20 7061 7469 656e 745f 6469  ame = patient_di
-0000ef70: 6374 5b27 6661 7468 6572 5f66 616d 696c  ct['father_famil
-0000ef80: 795f 6e61 6d65 275d 2069 6620 2766 6174  y_name'] if 'fat
-0000ef90: 6865 725f 6661 6d69 6c79 5f6e 616d 6527  her_family_name'
-0000efa0: 2069 6e20 7061 7469 656e 745f 6469 6374   in patient_dict
-0000efb0: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
-0000efc0: 2020 2073 656c 662e 7068 6f6e 655f 6e75     self.phone_nu
-0000efd0: 6d62 6572 203d 2070 6174 6965 6e74 5f64  mber = patient_d
-0000efe0: 6963 745b 2770 686f 6e65 5f6e 756d 6265  ict['phone_numbe
-0000eff0: 7227 5d20 6966 2027 7068 6f6e 655f 6e75  r'] if 'phone_nu
-0000f000: 6d62 6572 2720 696e 2070 6174 6965 6e74  mber' in patient
-0000f010: 5f64 6963 7420 656c 7365 204e 6f6e 650a  _dict else None.
-0000f020: 0a20 2020 2064 6566 2066 726f 6d5f 6a73  .    def from_js
-0000f030: 6f6e 2873 656c 662c 2072 6573 6f75 7263  on(self, resourc
-0000f040: 6529 3a0a 2020 2020 2020 2020 6966 2074  e):.        if t
-0000f050: 7970 6528 7265 736f 7572 6365 2920 6973  ype(resource) is
-0000f060: 2073 7472 3a0a 2020 2020 2020 2020 2020   str:.          
-0000f070: 2020 7374 725f 7265 736f 7572 6365 203d    str_resource =
-0000f080: 2072 6573 6f75 7263 650a 2020 2020 2020   resource.      
-0000f090: 2020 2020 2020 7265 736f 7572 6365 203d        resource =
-0000f0a0: 206a 736f 6e2e 6c6f 6164 7328 7374 725f   json.loads(str_
-0000f0b0: 7265 736f 7572 6365 290a 2020 2020 2020  resource).      
-0000f0c0: 2020 7365 6c66 2e66 6869 725f 7265 736f    self.fhir_reso
-0000f0d0: 7572 6365 203d 2050 6174 6965 6e74 286a  urce = Patient(j
-0000f0e0: 736f 6e64 6963 743d 7265 736f 7572 6365  sondict=resource
-0000f0f0: 290a 2020 2020 2020 2020 7365 6c66 2e66  ).        self.f
-0000f100: 726f 6d5f 6668 6972 5f70 6174 6965 6e74  rom_fhir_patient
-0000f110: 2829 0a0a 2020 2020 6465 6620 6765 7446  ()..    def getF
-0000f120: 6869 7252 6573 6f75 7263 6528 7365 6c66  hirResource(self
-0000f130: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0000f140: 746f 5f66 6869 725f 7061 7469 656e 7428  to_fhir_patient(
-0000f150: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000f160: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
-0000f170: 7263 652e 6173 5f6a 736f 6e28 290a 0a20  rce.as_json().. 
-0000f180: 2020 2064 6566 2067 6574 4668 6972 5265     def getFhirRe
-0000f190: 736f 7572 6365 5061 7261 6d65 7465 7228  sourceParameter(
-0000f1a0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-0000f1b0: 656c 662e 746f 5f66 6869 725f 7061 7469  elf.to_fhir_pati
-0000f1c0: 656e 7428 290a 2020 2020 2020 2020 7061  ent().        pa
-0000f1d0: 7261 6d20 3d20 5061 7261 6d65 7465 7246  ram = ParameterF
-0000f1e0: 4849 5228 290a 2020 2020 2020 2020 7061  HIR().        pa
-0000f1f0: 7261 6d2e 6164 645f 7061 7261 6d65 7465  ram.add_paramete
-0000f200: 7228 7365 6c66 2e66 6869 725f 7265 736f  r(self.fhir_reso
-0000f210: 7572 6365 290a 2020 2020 2020 2020 7265  urce).        re
-0000f220: 7475 726e 2070 6172 616d 2e67 6574 4668  turn param.getFh
-0000f230: 6972 5265 736f 7572 6365 2829 0a0a 2020  irResource()..  
-0000f240: 2020 6465 6620 7365 7448 6561 6465 7273    def setHeaders
-0000f250: 2873 656c 662c 2068 6561 6465 7273 3d7b  (self, headers={
-0000f260: 7d2c 2074 6f6b 656e 3d4e 6f6e 6529 3a0a  }, token=None):.
-0000f270: 2020 2020 2020 2020 6e65 7748 6561 6465          newHeade
-0000f280: 7273 203d 207b 2a2a 6865 6164 6572 732c  rs = {**headers,
-0000f290: 202a 2a73 656c 662e 6261 7365 5f68 6561   **self.base_hea
-0000f2a0: 6465 7273 7d0a 2020 2020 2020 2020 6966  ders}.        if
-0000f2b0: 2074 6f6b 656e 2069 7320 6e6f 7420 4e6f   token is not No
-0000f2c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000f2d0: 6966 2027 436f 6e74 656e 742d 7479 7065  if 'Content-type
-0000f2e0: 2720 696e 2074 6f6b 656e 3a0a 2020 2020  ' in token:.    
-0000f2f0: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-0000f300: 746f 6b65 6e5b 2743 6f6e 7465 6e74 2d74  token['Content-t
-0000f310: 7970 6527 5d0a 2020 2020 2020 2020 2020  ype'].          
-0000f320: 2020 6865 6164 6572 7357 6974 6841 7574    headersWithAut
-0000f330: 6820 3d20 7b2a 2a6e 6577 4865 6164 6572  h = {**newHeader
-0000f340: 732c 202a 2a74 6f6b 656e 7d0a 2020 2020  s, **token}.    
-0000f350: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0000f360: 6465 7273 203d 2068 6561 6465 7273 5769  ders = headersWi
-0000f370: 7468 4175 7468 0a20 2020 2020 2020 2065  thAuth.        e
-0000f380: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000f390: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-0000f3a0: 6e65 7748 6561 6465 7273 0a20 2020 2020  newHeaders.     
-0000f3b0: 2020 2072 6574 7572 6e20 7365 6c66 2e68     return self.h
-0000f3c0: 6561 6465 7273 0a0a 2020 2020 6465 6620  eaders..    def 
-0000f3d0: 4372 6561 7465 2873 656c 6629 3a0a 2020  Create(self):.  
-0000f3e0: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
-0000f3f0: 2e67 6574 4668 6972 5265 736f 7572 6365  .getFhirResource
-0000f400: 2829 0a20 2020 2020 2020 2072 6573 706f  ().        respo
-0000f410: 6e73 6520 3d20 7265 7175 6573 7473 2e70  nse = requests.p
-0000f420: 6f73 7428 7572 6c3d 7365 6c66 2e70 6174  ost(url=self.pat
-0000f430: 6965 6e74 5f65 6e64 706f 696e 742e 666f  ient_endpoint.fo
-0000f440: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-0000f450: 2020 7365 6c66 2e67 6574 5f66 6869 725f    self.get_fhir_
-0000f460: 7572 6c28 2929 2c20 6461 7461 3d6a 736f  url()), data=jso
-0000f470: 6e2e 6475 6d70 7328 7265 7329 2c20 6865  n.dumps(res), he
-0000f480: 6164 6572 733d 7365 6c66 2e68 6561 6465  aders=self.heade
-0000f490: 7273 2c20 7665 7269 6679 3d73 656c 662e  rs, verify=self.
-0000f4a0: 7661 6c69 6461 7465 5f63 6572 7473 290a  validate_certs).
-0000f4b0: 2020 2020 2020 2020 7365 6c66 2e66 726f          self.fro
-0000f4c0: 6d5f 6a73 6f6e 2872 6573 6f75 7263 653d  m_json(resource=
-0000f4d0: 7265 7370 6f6e 7365 2e63 6f6e 7465 6e74  response.content
-0000f4e0: 2e64 6563 6f64 6528 2929 0a20 2020 2020  .decode()).     
-0000f4f0: 2020 2069 6620 7365 6c66 2e6e 6975 2069     if self.niu i
-0000f500: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000f510: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-0000f520: 6c66 2e67 6574 4668 6972 5265 736f 7572  lf.getFhirResour
-0000f530: 6365 5061 7261 6d65 7465 7228 290a 2020  ceParameter().  
-0000f540: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-0000f550: 7473 2e70 6f73 7428 7572 6c3d 7365 6c66  ts.post(url=self
-0000f560: 2e70 6174 6965 6e74 5f64 6566 696e 6972  .patient_definir
-0000f570: 5f6e 6975 5f65 6e64 706f 696e 742e 666f  _niu_endpoint.fo
-0000f580: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-0000f590: 2020 2020 2020 7365 6c66 2e67 6574 5f66        self.get_f
-0000f5a0: 6869 725f 7572 6c28 292c 2073 656c 662e  hir_url(), self.
-0000f5b0: 6964 292c 2064 6174 613d 6a73 6f6e 2e64  id), data=json.d
-0000f5c0: 756d 7073 2872 6573 292c 2068 6561 6465  umps(res), heade
-0000f5d0: 7273 3d73 656c 662e 6865 6164 6572 732c  rs=self.headers,
-0000f5e0: 2076 6572 6966 793d 7365 6c66 2e76 616c   verify=self.val
-0000f5f0: 6964 6174 655f 6365 7274 7329 0a20 2020  idate_certs).   
-0000f600: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
-0000f610: 6f6e 7365 0a0a 2020 2020 6465 6620 4765  onse..    def Ge
-0000f620: 7442 7949 6428 7365 6c66 2c20 7061 7469  tById(self, pati
-0000f630: 656e 745f 6964 3d4e 6f6e 6529 3a0a 2020  ent_id=None):.  
-0000f640: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-0000f650: 2072 6571 7565 7374 732e 6765 7428 7572   requests.get(ur
-0000f660: 6c3d 7365 6c66 2e70 6174 6965 6e74 5f69  l=self.patient_i
-0000f670: 645f 656e 6470 6f69 6e74 2e66 6f72 6d61  d_endpoint.forma
-0000f680: 7428 0a20 2020 2020 2020 2020 2020 2073  t(.            s
-0000f690: 656c 662e 6765 745f 6668 6972 5f75 726c  elf.get_fhir_url
-0000f6a0: 2829 2c20 7061 7469 656e 745f 6964 292c  (), patient_id),
-0000f6b0: 2068 6561 6465 7273 3d73 656c 662e 6865   headers=self.he
-0000f6c0: 6164 6572 732c 2076 6572 6966 793d 7365  aders, verify=se
-0000f6d0: 6c66 2e76 616c 6964 6174 655f 6365 7274  lf.validate_cert
-0000f6e0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-0000f6f0: 6672 6f6d 5f6a 736f 6e28 7265 736f 7572  from_json(resour
-0000f700: 6365 3d72 6573 706f 6e73 652e 636f 6e74  ce=response.cont
-0000f710: 656e 742e 6465 636f 6465 2829 290a 2020  ent.decode()).  
-0000f720: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0000f730: 706f 6e73 650a 0a20 2020 2064 6566 204d  ponse..    def M
-0000f740: 6174 6368 2873 656c 6629 3a0a 2020 2020  atch(self):.    
-0000f750: 2020 2020 7265 7320 3d20 7365 6c66 2e67      res = self.g
-0000f760: 6574 4668 6972 5265 736f 7572 6365 5061  etFhirResourcePa
-0000f770: 7261 6d65 7465 7228 290a 2020 2020 2020  rameter().      
-0000f780: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
-0000f790: 7565 7374 732e 706f 7374 2875 726c 3d73  uests.post(url=s
-0000f7a0: 656c 662e 7061 7469 656e 745f 6d61 7463  elf.patient_matc
-0000f7b0: 685f 656e 6470 6f69 6e74 2e66 6f72 6d61  h_endpoint.forma
-0000f7c0: 7428 0a20 2020 2020 2020 2020 2020 2073  t(.            s
-0000f7d0: 656c 662e 6765 745f 6668 6972 5f75 726c  elf.get_fhir_url
-0000f7e0: 2829 292c 2064 6174 613d 6a73 6f6e 2e64  ()), data=json.d
-0000f7f0: 756d 7073 2872 6573 292c 2068 6561 6465  umps(res), heade
-0000f800: 7273 3d73 656c 662e 6865 6164 6572 732c  rs=self.headers,
-0000f810: 2076 6572 6966 793d 7365 6c66 2e76 616c   verify=self.val
-0000f820: 6964 6174 655f 6365 7274 7329 0a20 2020  idate_certs).   
-0000f830: 2020 2020 2069 6620 7265 7370 6f6e 7365       if response
-0000f840: 2e73 7461 7475 735f 636f 6465 203d 3d20  .status_code == 
-0000f850: 3230 303a 0a20 2020 2020 2020 2020 2020  200:.           
-0000f860: 2070 6172 616d 7320 3d20 5061 7261 6d65   params = Parame
-0000f870: 7465 7246 4849 5228 7265 736f 7572 6365  terFHIR(resource
-0000f880: 3d6a 736f 6e2e 6c6f 6164 7328 7265 7370  =json.loads(resp
-0000f890: 6f6e 7365 2e63 6f6e 7465 6e74 2e64 6563  onse.content.dec
-0000f8a0: 6f64 6528 2929 290a 2020 2020 2020 2020  ode())).        
-0000f8b0: 2020 2020 6966 2070 6172 616d 732e 6668      if params.fh
-0000f8c0: 6972 5f72 6573 6f75 7263 6520 6973 206e  ir_resource is n
-0000f8d0: 6f74 204e 6f6e 6520 616e 6420 7061 7261  ot None and para
-0000f8e0: 6d73 2e66 6869 725f 7265 736f 7572 6365  ms.fhir_resource
-0000f8f0: 2e70 6172 616d 6574 6572 2069 7320 6e6f  .parameter is no
-0000f900: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000f910: 2020 2020 2020 2020 666f 7220 7061 7261          for para
-0000f920: 6d20 696e 2070 6172 616d 732e 6668 6972  m in params.fhir
-0000f930: 5f72 6573 6f75 7263 652e 7061 7261 6d65  _resource.parame
-0000f940: 7465 723a 0a20 2020 2020 2020 2020 2020  ter:.           
-0000f950: 2020 2020 2020 2020 2069 6620 7479 7065           if type
-0000f960: 2870 6172 616d 2e72 6573 6f75 7263 6529  (param.resource)
-0000f970: 2069 7320 5061 7469 656e 743a 0a20 2020   is Patient:.   
-0000f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f990: 2020 2020 2073 656c 662e 6668 6972 5f72       self.fhir_r
-0000f9a0: 6573 6f75 7263 6520 3d20 7061 7261 6d2e  esource = param.
-0000f9b0: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
-0000f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9d0: 2073 656c 662e 6672 6f6d 5f66 6869 725f   self.from_fhir_
-0000f9e0: 7061 7469 656e 7428 290a 2020 2020 2020  patient().      
-0000f9f0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-0000fa00: 650a 0a20 2020 2064 6566 2053 6561 7263  e..    def Searc
-0000fa10: 6828 7365 6c66 2c20 6964 656e 7469 6669  h(self, identifi
-0000fa20: 6572 3d4e 6f6e 652c 2067 6976 656e 3d4e  er=None, given=N
-0000fa30: 6f6e 652c 2066 616d 696c 793d 4e6f 6e65  one, family=None
-0000fa40: 2c20 6765 6e64 6572 3d4e 6f6e 652c 2062  , gender=None, b
-0000fa50: 6972 7468 6461 7465 3d4e 6f6e 6529 3a0a  irthdate=None):.
-0000fa60: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-0000fa70: 207b 7d0a 2020 2020 2020 2020 6966 2069   {}.        if i
-0000fa80: 6465 6e74 6966 6965 7220 6973 206e 6f74  dentifier is not
-0000fa90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000faa0: 2020 2070 6172 616d 735b 2769 6465 6e74     params['ident
-0000fab0: 6966 6965 7227 5d20 3d20 6964 656e 7469  ifier'] = identi
-0000fac0: 6669 6572 0a20 2020 2020 2020 2065 6c69  fier.        eli
-0000fad0: 6620 7365 6c66 2e6e 616d 2069 7320 6e6f  f self.nam is no
-0000fae0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000faf0: 2020 2020 7061 7261 6d73 5b27 6964 656e      params['iden
-0000fb00: 7469 6669 6572 275d 203d 2022 636f 6465  tifier'] = "code
-0000fb10: 3d4e 414d 7c7b 7d22 2e66 6f72 6d61 7428  =NAM|{}".format(
-0000fb20: 7365 6c66 2e6e 616d 290a 2020 2020 2020  self.nam).      
-0000fb30: 2020 6966 2067 6976 656e 2069 7320 6e6f    if given is no
-0000fb40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000fb50: 2020 2020 7061 7261 6d73 5b27 6769 7665      params['give
-0000fb60: 6e27 5d20 3d20 6769 7665 6e0a 2020 2020  n'] = given.    
-0000fb70: 2020 2020 656c 6966 2073 656c 662e 6769      elif self.gi
-0000fb80: 7665 6e5f 6e61 6d65 2069 7320 6e6f 7420  ven_name is not 
-0000fb90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000fba0: 2020 7061 7261 6d73 5b27 6769 7665 6e27    params['given'
-0000fbb0: 5d20 3d20 7365 6c66 2e67 6976 656e 5f6e  ] = self.given_n
-0000fbc0: 616d 650a 2020 2020 2020 2020 6966 2066  ame.        if f
-0000fbd0: 616d 696c 7920 6973 206e 6f74 204e 6f6e  amily is not Non
-0000fbe0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-0000fbf0: 6172 616d 735b 2766 616d 696c 7927 5d20  arams['family'] 
-0000fc00: 3d20 6661 6d69 6c79 0a20 2020 2020 2020  = family.       
-0000fc10: 2065 6c69 6620 7365 6c66 2e66 616d 696c   elif self.famil
-0000fc20: 795f 6e61 6d65 2069 7320 6e6f 7420 4e6f  y_name is not No
-0000fc30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000fc40: 7061 7261 6d73 5b27 6661 6d69 6c79 275d  params['family']
-0000fc50: 203d 2073 656c 662e 6661 6d69 6c79 5f6e   = self.family_n
-0000fc60: 616d 650a 2020 2020 2020 2020 6966 2067  ame.        if g
-0000fc70: 656e 6465 7220 6973 206e 6f74 204e 6f6e  ender is not Non
-0000fc80: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-0000fc90: 6172 616d 735b 2767 656e 6465 7227 5d20  arams['gender'] 
-0000fca0: 3d20 6765 6e64 6572 0a20 2020 2020 2020  = gender.       
-0000fcb0: 2065 6c69 6620 7365 6c66 2e67 656e 6465   elif self.gende
-0000fcc0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-0000fcd0: 2020 2020 2020 2020 2020 2070 6172 616d             param
-0000fce0: 735b 2767 656e 6465 7227 5d20 3d20 7365  s['gender'] = se
-0000fcf0: 6c66 2e67 656e 6465 720a 2020 2020 2020  lf.gender.      
-0000fd00: 2020 6966 2062 6972 7468 6461 7465 2069    if birthdate i
-0000fd10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000fd20: 2020 2020 2020 2020 7061 7261 6d73 5b27          params['
-0000fd30: 6269 7274 6864 6174 6527 5d20 3d20 6269  birthdate'] = bi
-0000fd40: 7274 6864 6174 650a 2020 2020 2020 2020  rthdate.        
-0000fd50: 656c 6966 2073 656c 662e 6269 7274 685f  elif self.birth_
-0000fd60: 6461 7465 2069 7320 6e6f 7420 4e6f 6e65  date is not None
-0000fd70: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-0000fd80: 7261 6d73 5b27 6269 7274 6864 6174 6527  rams['birthdate'
-0000fd90: 5d20 3d20 7365 6c66 2e62 6972 7468 5f64  ] = self.birth_d
-0000fda0: 6174 650a 2020 2020 2020 2020 7265 7370  ate.        resp
-0000fdb0: 6f6e 7365 203d 2072 6571 7565 7374 732e  onse = requests.
-0000fdc0: 6765 7428 7572 6c3d 7365 6c66 2e70 6174  get(url=self.pat
-0000fdd0: 6965 6e74 5f65 6e64 706f 696e 742e 666f  ient_endpoint.fo
-0000fde0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-0000fdf0: 2020 7365 6c66 2e67 6574 5f66 6869 725f    self.get_fhir_
-0000fe00: 7572 6c28 2929 2c20 7061 7261 6d73 3d70  url()), params=p
-0000fe10: 6172 616d 732c 2068 6561 6465 7273 3d73  arams, headers=s
-0000fe20: 656c 662e 6865 6164 6572 732c 2076 6572  elf.headers, ver
-0000fe30: 6966 793d 7365 6c66 2e76 616c 6964 6174  ify=self.validat
-0000fe40: 655f 6365 7274 7329 0a0a 2020 2020 2020  e_certs)..      
-0000fe50: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-0000fe60: 650a 0a20 2020 2064 6566 206e 616d 5f74  e..    def nam_t
-0000fe70: 6f5f 6964 656e 7469 6669 6572 2873 656c  o_identifier(sel
-0000fe80: 662c 206e 616d 2c20 636f 6469 6e67 5f73  f, nam, coding_s
-0000fe90: 7973 7465 6d3d 4e6f 6e65 2c20 636f 6469  ystem=None, codi
-0000fea0: 6e67 5f76 6572 7369 6f6e 3d4e 6f6e 6529  ng_version=None)
-0000feb0: 3a0a 2020 2020 2020 2020 6e61 6d5f 636f  :.        nam_co
-0000fec0: 6469 6e67 5f73 7973 7465 6d20 3d20 636f  ding_system = co
-0000fed0: 6469 6e67 5f73 7973 7465 6d20 6966 2063  ding_system if c
-0000fee0: 6f64 696e 675f 7379 7374 656d 2069 7320  oding_system is 
-0000fef0: 6e6f 7420 4e6f 6e65 2065 6c73 6520 7365  not None else se
-0000ff00: 6c66 2e64 6566 6175 6c74 5f63 6f64 696e  lf.default_codin
-0000ff10: 675f 7379 7374 656d 0a20 2020 2020 2020  g_system.       
-0000ff20: 206e 616d 5f63 6f64 696e 675f 7665 7273   nam_coding_vers
-0000ff30: 696f 6e20 3d20 636f 6469 6e67 5f73 7973  ion = coding_sys
-0000ff40: 7465 6d20 6966 2063 6f64 696e 675f 7665  tem if coding_ve
-0000ff50: 7273 696f 6e20 6973 206e 6f74 204e 6f6e  rsion is not Non
-0000ff60: 6520 656c 7365 2073 656c 662e 6465 6661  e else self.defa
-0000ff70: 756c 745f 636f 6469 6e67 5f76 6572 7369  ult_coding_versi
-0000ff80: 6f6e 0a20 2020 2020 2020 206e 616d 5f69  on.        nam_i
-0000ff90: 6465 6e74 6966 6965 7220 3d20 4964 656e  dentifier = Iden
-0000ffa0: 7469 6669 6572 2829 0a20 2020 2020 2020  tifier().       
-0000ffb0: 206e 616d 5f69 6465 6e74 6966 6965 725f   nam_identifier_
-0000ffc0: 6578 7465 6e73 696f 6e20 3d20 4578 7465  extension = Exte
-0000ffd0: 6e73 696f 6e28 290a 2020 2020 2020 2020  nsion().        
-0000ffe0: 6e61 6d5f 6964 656e 7469 6669 6572 5f65  nam_identifier_e
-0000fff0: 7874 656e 7369 6f6e 2e75 726c 203d 2073  xtension.url = s
-00010000: 656c 662e 6e61 6d5f 6964 656e 7469 6669  elf.nam_identifi
-00010010: 6572 5f65 7874 656e 7369 6f6e 5f75 726c  er_extension_url
-00010020: 0a20 2020 2020 2020 206e 616d 5f65 7874  .        nam_ext
-00010030: 5f63 6f64 6162 6c65 5f63 6f6e 6365 7074  _codable_concept
-00010040: 203d 2043 6f64 6561 626c 6543 6f6e 6365   = CodeableConce
-00010050: 7074 2829 0a20 2020 2020 2020 206e 616d  pt().        nam
-00010060: 5f65 7874 5f63 6f64 6162 6c65 5f63 6f6e  _ext_codable_con
-00010070: 6365 7074 2e63 6f64 696e 6720 3d20 5b43  cept.coding = [C
-00010080: 6f64 696e 6728 6a73 6f6e 6469 6374 3d7b  oding(jsondict={
-00010090: 2273 7973 7465 6d22 3a20 6e61 6d5f 636f  "system": nam_co
-000100a0: 6469 6e67 5f73 7973 7465 6d2c 2276 6572  ding_system,"ver
-000100b0: 7369 6f6e 223a 206e 616d 5f63 6f64 696e  sion": nam_codin
-000100c0: 675f 7665 7273 696f 6e2c 2263 6f64 6522  g_version,"code"
-000100d0: 3a20 2251 4322 7d29 5d0a 2020 2020 2020  : "QC"})].      
-000100e0: 2020 6e61 6d5f 6964 656e 7469 6669 6572    nam_identifier
-000100f0: 5f65 7874 656e 7369 6f6e 2e76 616c 7565  _extension.value
-00010100: 436f 6465 6162 6c65 436f 6e63 6570 7420  CodeableConcept 
-00010110: 3d20 6e61 6d5f 6578 745f 636f 6461 626c  = nam_ext_codabl
-00010120: 655f 636f 6e63 6570 740a 2020 2020 2020  e_concept.      
-00010130: 2020 6e61 6d5f 6964 656e 7469 6669 6572    nam_identifier
-00010140: 2e65 7874 656e 7369 6f6e 203d 205b 6e61  .extension = [na
-00010150: 6d5f 6964 656e 7469 6669 6572 5f65 7874  m_identifier_ext
-00010160: 656e 7369 6f6e 5d0a 2020 2020 2020 2020  ension].        
-00010170: 6e61 6d5f 7479 7065 5f63 6f64 6162 6c65  nam_type_codable
-00010180: 5f63 6f6e 6365 7074 203d 2043 6f64 6561  _concept = Codea
-00010190: 626c 6543 6f6e 6365 7074 2829 0a20 2020  bleConcept().   
-000101a0: 2020 2020 206e 616d 5f74 7970 655f 636f       nam_type_co
-000101b0: 6461 626c 655f 636f 6e63 6570 742e 636f  dable_concept.co
-000101c0: 6469 6e67 203d 205b 436f 6469 6e67 286a  ding = [Coding(j
-000101d0: 736f 6e64 6963 743d 7b22 7379 7374 656d  sondict={"system
-000101e0: 223a 206e 616d 5f63 6f64 696e 675f 7379  ": nam_coding_sy
-000101f0: 7374 656d 2c22 7665 7273 696f 6e22 3a20  stem,"version": 
-00010200: 6e61 6d5f 636f 6469 6e67 5f76 6572 7369  nam_coding_versi
-00010210: 6f6e 2c22 636f 6465 223a 2022 4e41 4d22  on,"code": "NAM"
-00010220: 7d29 5d0a 2020 2020 2020 2020 6e61 6d5f  })].        nam_
-00010230: 6964 656e 7469 6669 6572 2e74 7970 6520  identifier.type 
-00010240: 3d20 6e61 6d5f 7479 7065 5f63 6f64 6162  = nam_type_codab
-00010250: 6c65 5f63 6f6e 6365 7074 0a20 2020 2020  le_concept.     
-00010260: 2020 206e 616d 5f69 6465 6e74 6966 6965     nam_identifie
-00010270: 722e 7379 7374 656d 203d 2073 656c 662e  r.system = self.
-00010280: 6e61 6d5f 6964 656e 7469 6669 6572 5f73  nam_identifier_s
-00010290: 7973 7465 6d0a 2020 2020 2020 2020 6e61  ystem.        na
-000102a0: 6d5f 6964 656e 7469 6669 6572 2e76 616c  m_identifier.val
-000102b0: 7565 203d 206e 616d 0a20 2020 2020 2020  ue = nam.       
-000102c0: 2072 6574 7572 6e20 6e61 6d5f 6964 656e   return nam_iden
-000102d0: 7469 6669 6572 0a0a 2020 2020 6465 6620  tifier..    def 
-000102e0: 6e69 755f 746f 5f69 6465 6e74 6966 6965  niu_to_identifie
-000102f0: 7228 7365 6c66 2c20 6e69 752c 2063 6f64  r(self, niu, cod
-00010300: 696e 675f 7379 7374 656d 3d4e 6f6e 652c  ing_system=None,
-00010310: 2063 6f64 696e 675f 7665 7273 696f 6e3d   coding_version=
-00010320: 4e6f 6e65 293a 0a20 2020 2020 2020 206e  None):.        n
-00010330: 6975 5f63 6f64 696e 675f 7379 7374 656d  iu_coding_system
-00010340: 203d 2063 6f64 696e 675f 7379 7374 656d   = coding_system
-00010350: 2069 6620 636f 6469 6e67 5f73 7973 7465   if coding_syste
-00010360: 6d20 6973 206e 6f74 204e 6f6e 6520 656c  m is not None el
-00010370: 7365 2073 656c 662e 6465 6661 756c 745f  se self.default_
-00010380: 636f 6469 6e67 5f73 7973 7465 6d0a 2020  coding_system.  
-00010390: 2020 2020 2020 6e69 755f 636f 6469 6e67        niu_coding
-000103a0: 5f76 6572 7369 6f6e 203d 2063 6f64 696e  _version = codin
-000103b0: 675f 7379 7374 656d 2069 6620 636f 6469  g_system if codi
-000103c0: 6e67 5f76 6572 7369 6f6e 2069 7320 6e6f  ng_version is no
-000103d0: 7420 4e6f 6e65 2065 6c73 6520 7365 6c66  t None else self
-000103e0: 2e64 6566 6175 6c74 5f63 6f64 696e 675f  .default_coding_
-000103f0: 7665 7273 696f 6e0a 2020 2020 2020 2020  version.        
-00010400: 6e69 755f 6964 656e 7469 6669 6572 203d  niu_identifier =
-00010410: 2049 6465 6e74 6966 6965 7228 290a 2020   Identifier().  
-00010420: 2020 2020 2020 6e69 755f 7479 7065 5f63        niu_type_c
-00010430: 6f64 6162 6c65 5f63 6f6e 6365 7074 203d  odable_concept =
-00010440: 2043 6f64 6561 626c 6543 6f6e 6365 7074   CodeableConcept
-00010450: 2829 0a20 2020 2020 2020 206e 6975 5f74  ().        niu_t
-00010460: 7970 655f 636f 6461 626c 655f 636f 6e63  ype_codable_conc
-00010470: 6570 742e 636f 6469 6e67 203d 205b 436f  ept.coding = [Co
-00010480: 6469 6e67 286a 736f 6e64 6963 743d 7b22  ding(jsondict={"
-00010490: 7379 7374 656d 223a 206e 6975 5f63 6f64  system": niu_cod
-000104a0: 696e 675f 7379 7374 656d 2c22 7665 7273  ing_system,"vers
-000104b0: 696f 6e22 3a20 6e69 755f 636f 6469 6e67  ion": niu_coding
-000104c0: 5f76 6572 7369 6f6e 2c22 636f 6465 223a  _version,"code":
-000104d0: 2022 4e49 5555 222c 2264 6973 706c 6179   "NIUU","display
-000104e0: 223a 224e 4955 227d 295d 0a20 2020 2020  ":"NIU"})].     
-000104f0: 2020 206e 6975 5f69 6465 6e74 6966 6965     niu_identifie
-00010500: 722e 7479 7065 203d 206e 6975 5f74 7970  r.type = niu_typ
-00010510: 655f 636f 6461 626c 655f 636f 6e63 6570  e_codable_concep
-00010520: 740a 2020 2020 2020 2020 6e69 755f 6964  t.        niu_id
-00010530: 656e 7469 6669 6572 2e76 616c 7565 203d  entifier.value =
-00010540: 206e 6975 0a20 2020 2020 2020 206e 6975   niu.        niu
-00010550: 5f69 6465 6e74 6966 6965 722e 7379 7374  _identifier.syst
-00010560: 656d 203d 2073 656c 662e 6e69 755f 6964  em = self.niu_id
-00010570: 656e 7469 6669 6572 5f73 7973 7465 6d0a  entifier_system.
-00010580: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-00010590: 6975 5f69 6465 6e74 6966 6965 720a 0a20  iu_identifier.. 
-000105a0: 2020 2064 6566 2061 7563 756e 5f69 6465     def aucun_ide
-000105b0: 6e74 6966 6961 6e74 5f74 6f5f 6964 656e  ntifiant_to_iden
-000105c0: 7469 6669 6572 2873 656c 662c 2063 6f64  tifier(self, cod
-000105d0: 696e 675f 7379 7374 656d 3d4e 6f6e 652c  ing_system=None,
-000105e0: 2063 6f64 696e 675f 7665 7273 696f 6e3d   coding_version=
-000105f0: 4e6f 6e65 293a 0a20 2020 2020 2020 2063  None):.        c
-00010600: 6f64 696e 675f 7379 7374 656d 203d 2063  oding_system = c
-00010610: 6f64 696e 675f 7379 7374 656d 2069 6620  oding_system if 
-00010620: 636f 6469 6e67 5f73 7973 7465 6d20 6973  coding_system is
-00010630: 206e 6f74 204e 6f6e 6520 656c 7365 2073   not None else s
-00010640: 656c 662e 6465 6661 756c 745f 636f 6469  elf.default_codi
-00010650: 6e67 5f73 7973 7465 6d0a 2020 2020 2020  ng_system.      
-00010660: 2020 636f 6469 6e67 5f76 6572 7369 6f6e    coding_version
-00010670: 203d 2063 6f64 696e 675f 7379 7374 656d   = coding_system
-00010680: 2069 6620 636f 6469 6e67 5f76 6572 7369   if coding_versi
-00010690: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 2065  on is not None e
-000106a0: 6c73 6520 7365 6c66 2e64 6566 6175 6c74  lse self.default
-000106b0: 5f63 6f64 696e 675f 7665 7273 696f 6e0a  _coding_version.
-000106c0: 2020 2020 2020 2020 6175 6375 6e5f 6964          aucun_id
-000106d0: 656e 7469 6669 6572 203d 2049 6465 6e74  entifier = Ident
-000106e0: 6966 6965 7228 290a 2020 2020 2020 2020  ifier().        
-000106f0: 6175 6375 6e5f 7479 7065 5f63 6f64 6162  aucun_type_codab
-00010700: 6c65 5f63 6f6e 6365 7074 203d 2043 6f64  le_concept = Cod
-00010710: 6561 626c 6543 6f6e 6365 7074 2829 0a20  eableConcept(). 
-00010720: 2020 2020 2020 2061 7563 756e 5f74 7970         aucun_typ
-00010730: 655f 636f 6461 626c 655f 636f 6e63 6570  e_codable_concep
-00010740: 742e 636f 6469 6e67 203d 205b 436f 6469  t.coding = [Codi
-00010750: 6e67 286a 736f 6e64 6963 743d 7b22 7379  ng(jsondict={"sy
-00010760: 7374 656d 223a 2063 6f64 696e 675f 7379  stem": coding_sy
-00010770: 7374 656d 2c22 7665 7273 696f 6e22 3a20  stem,"version": 
-00010780: 636f 6469 6e67 5f76 6572 7369 6f6e 2c22  coding_version,"
-00010790: 636f 6465 223a 2022 4155 4355 4e22 2c22  code": "AUCUN","
-000107a0: 6469 7370 6c61 7922 3a22 4175 6375 6e20  display":"Aucun 
-000107b0: 6964 656e 7469 6669 616e 7422 7d29 5d0a  identifiant"})].
-000107c0: 2020 2020 2020 2020 6175 6375 6e5f 6964          aucun_id
-000107d0: 656e 7469 6669 6572 2e74 7970 6520 3d20  entifier.type = 
-000107e0: 6175 6375 6e5f 7479 7065 5f63 6f64 6162  aucun_type_codab
-000107f0: 6c65 5f63 6f6e 6365 7074 0a20 2020 2020  le_concept.     
-00010800: 2020 2061 7563 756e 5f69 6465 6e74 6966     aucun_identif
-00010810: 6965 722e 7379 7374 656d 203d 2073 656c  ier.system = sel
-00010820: 662e 6175 6375 6e5f 6964 656e 7469 6669  f.aucun_identifi
-00010830: 6572 5f73 7973 7465 6d0a 2020 2020 2020  er_system.      
-00010840: 2020 7265 7475 726e 2061 7563 756e 5f69    return aucun_i
-00010850: 6465 6e74 6966 6965 720a 0a20 2020 2064  dentifier..    d
-00010860: 6566 2067 6976 656e 5f66 616d 696c 795f  ef given_family_
-00010870: 746f 5f68 756d 616e 5f6e 616d 6528 7365  to_human_name(se
-00010880: 6c66 2c20 6769 7665 6e5f 6e61 6d65 3d4e  lf, given_name=N
-00010890: 6f6e 652c 2066 616d 696c 795f 6e61 6d65  one, family_name
-000108a0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-000108b0: 686e 203d 2048 756d 616e 4e61 6d65 2829  hn = HumanName()
-000108c0: 0a20 2020 2020 2020 2068 6e2e 6769 7665  .        hn.give
-000108d0: 6e20 3d20 5b67 6976 656e 5f6e 616d 655d  n = [given_name]
-000108e0: 0a20 2020 2020 2020 2068 6e2e 6661 6d69  .        hn.fami
-000108f0: 6c79 203d 205b 6661 6d69 6c79 5f6e 616d  ly = [family_nam
-00010900: 655d 0a20 2020 2020 2020 2072 6574 7572  e].        retur
-00010910: 6e20 686e 0a0a 2020 2020 6465 6620 7374  n hn..    def st
-00010920: 725f 6461 7465 5f74 6f5f 6668 6972 5f64  r_date_to_fhir_d
-00010930: 6174 6528 7365 6c66 2c20 7374 725f 6461  ate(self, str_da
-00010940: 7465 293a 0a20 2020 2020 2020 2066 6869  te):.        fhi
-00010950: 725f 6461 7465 2020 3d20 4648 4952 4461  r_date  = FHIRDa
-00010960: 7465 2829 0a20 2020 2020 2020 2066 6869  te().        fhi
-00010970: 725f 6461 7465 2e64 6174 6520 3d20 6461  r_date.date = da
-00010980: 7465 7469 6d65 2e73 7472 7074 696d 6528  tetime.strptime(
-00010990: 7374 725f 6461 7465 2c20 2725 592d 256d  str_date, '%Y-%m
-000109a0: 2d25 6427 292e 6461 7465 2829 0a20 2020  -%d').date().   
-000109b0: 2020 2020 2072 6574 7572 6e20 6668 6972       return fhir
-000109c0: 5f64 6174 650a 0a20 2020 2064 6566 2066  _date..    def f
-000109d0: 6869 725f 6461 7465 5f74 6f5f 7374 725f  hir_date_to_str_
-000109e0: 6461 7465 2873 656c 662c 2066 6869 725f  date(self, fhir_
-000109f0: 6461 7465 293a 0a20 2020 2020 2020 2073  date):.        s
-00010a00: 7472 5f64 6174 6520 3d20 4e6f 6e65 0a20  tr_date = None. 
-00010a10: 2020 2020 2020 2069 6620 6668 6972 5f64         if fhir_d
-00010a20: 6174 6520 6973 206e 6f74 204e 6f6e 6520  ate is not None 
-00010a30: 616e 6420 6668 6972 5f64 6174 652e 6461  and fhir_date.da
-00010a40: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  te is not None:.
-00010a50: 2020 2020 2020 2020 2020 2020 7374 725f              str_
-00010a60: 6461 7465 203d 2066 6869 725f 6461 7465  date = fhir_date
-00010a70: 2e69 736f 7374 7269 6e67 0a20 2020 2020  .isostring.     
-00010a80: 2020 2072 6574 7572 6e20 7374 725f 6461     return str_da
-00010a90: 7465 0a0a 2020 2020 6465 6620 7365 745f  te..    def set_
-00010aa0: 6964 2873 656c 662c 2069 642c 2070 6174  id(self, id, pat
-00010ab0: 6965 6e74 3d4e 6f6e 6529 3a0a 2020 2020  ient=None):.    
-00010ac0: 2020 2020 6966 2070 6174 6965 6e74 2069      if patient i
-00010ad0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00010ae0: 2020 2020 7061 7469 656e 7420 3d20 7365      patient = se
-00010af0: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
-00010b00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010b10: 662e 6964 203d 2069 640a 2020 2020 2020  f.id = id.      
-00010b20: 2020 7061 7469 656e 742e 6964 203d 2069    patient.id = i
-00010b30: 640a 0a20 2020 2064 6566 2067 6574 5f69  d..    def get_i
-00010b40: 6428 7365 6c66 2c20 7061 7469 656e 743d  d(self, patient=
-00010b50: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
-00010b60: 6620 7061 7469 656e 7420 6973 204e 6f6e  f patient is Non
-00010b70: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-00010b80: 6174 6965 6e74 203d 2073 656c 662e 6668  atient = self.fh
-00010b90: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
-00010ba0: 2020 2020 7265 7475 726e 2070 6174 6965      return patie
-00010bb0: 6e74 2e69 640a 0a20 2020 2064 6566 2073  nt.id..    def s
-00010bc0: 6574 5f6d 6174 6368 7261 6d71 2873 656c  et_matchramq(sel
-00010bd0: 662c 206d 6174 6368 7261 6d71 3d46 616c  f, matchramq=Fal
-00010be0: 7365 2c20 7061 7469 656e 743d 4e6f 6e65  se, patient=None
-00010bf0: 293a 0a20 2020 2020 2020 2069 6620 7479  ):.        if ty
-00010c00: 7065 286d 6174 6368 7261 6d71 2920 6973  pe(matchramq) is
-00010c10: 2062 6f6f 6c3a 0a20 2020 2020 2020 2020   bool:.         
-00010c20: 2020 2062 6f6f 6c5f 6d61 7463 6872 616d     bool_matchram
-00010c30: 7120 3d20 6d61 7463 6872 616d 710a 2020  q = matchramq.  
-00010c40: 2020 2020 2020 656c 6966 2074 7970 6528        elif type(
-00010c50: 6d61 7463 6872 616d 7129 2069 7320 7374  matchramq) is st
-00010c60: 723a 0a20 2020 2020 2020 2020 2020 2062  r:.            b
-00010c70: 6f6f 6c5f 6d61 7463 6872 616d 7120 3d20  ool_matchramq = 
-00010c80: 626f 6f6c 2873 7472 3262 6f6f 6c28 6d61  bool(str2bool(ma
-00010c90: 7463 6872 616d 7129 290a 2020 2020 2020  tchramq)).      
-00010ca0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00010cb0: 2020 2020 626f 6f6c 5f6d 6174 6368 7261      bool_matchra
-00010cc0: 6d71 203d 2046 616c 7365 0a20 2020 2020  mq = False.     
-00010cd0: 2020 2069 6620 7061 7469 656e 7420 6973     if patient is
-00010ce0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00010cf0: 2020 2070 6174 6965 6e74 203d 2073 656c     patient = sel
-00010d00: 662e 6668 6972 5f72 6573 6f75 7263 650a  f.fhir_resource.
-00010d10: 2020 2020 2020 2020 6d61 7463 6872 616d          matchram
-00010d20: 715f 6578 7465 6e73 696f 6e20 3d20 4578  q_extension = Ex
-00010d30: 7465 6e73 696f 6e28 290a 2020 2020 2020  tension().      
-00010d40: 2020 6d61 7463 6872 616d 715f 6578 7465    matchramq_exte
-00010d50: 6e73 696f 6e2e 7572 6c20 3d20 7365 6c66  nsion.url = self
-00010d60: 2e6d 6174 6368 7261 6d71 5f65 7874 656e  .matchramq_exten
-00010d70: 7369 6f6e 5f75 726c 0a20 2020 2020 2020  sion_url.       
-00010d80: 206d 6174 6368 7261 6d71 5f65 7874 656e   matchramq_exten
-00010d90: 7369 6f6e 2e76 616c 7565 426f 6f6c 6561  sion.valueBoolea
-00010da0: 6e20 3d20 626f 6f6c 5f6d 6174 6368 7261  n = bool_matchra
-00010db0: 6d71 0a0a 2020 2020 2020 2020 6966 2070  mq..        if p
-00010dc0: 6174 6965 6e74 2e65 7874 656e 7369 6f6e  atient.extension
-00010dd0: 2069 7320 4e6f 6e65 3a20 2020 200a 2020   is None:    .  
-00010de0: 2020 2020 2020 2020 2020 7061 7469 656e            patien
-00010df0: 742e 6578 7465 6e73 696f 6e20 3d20 5b6d  t.extension = [m
-00010e00: 6174 6368 7261 6d71 5f65 7874 656e 7369  atchramq_extensi
-00010e10: 6f6e 5d0a 2020 2020 2020 2020 656c 7365  on].        else
-00010e20: 3a0a 2020 2020 2020 2020 2020 2020 6578  :.            ex
-00010e30: 7465 6e73 696f 6e5f 666f 756e 6420 3d20  tension_found = 
-00010e40: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00010e50: 2020 666f 7220 6578 7420 696e 2070 6174    for ext in pat
-00010e60: 6965 6e74 2e65 7874 656e 7369 6f6e 3a0a  ient.extension:.
-00010e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e80: 6966 2065 7874 2e75 726c 203d 3d20 7365  if ext.url == se
-00010e90: 6c66 2e6d 6174 6368 7261 6d71 5f65 7874  lf.matchramq_ext
-00010ea0: 656e 7369 6f6e 5f75 726c 3a0a 2020 2020  ension_url:.    
-00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ec0: 6578 7465 6e73 696f 6e5f 666f 756e 6420  extension_found 
-00010ed0: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-00010ee0: 2020 2020 2020 2020 2020 2065 7874 2e76             ext.v
-00010ef0: 616c 7565 426f 6f6c 6561 6e20 3d20 626f  alueBoolean = bo
-00010f00: 6f6c 5f6d 6174 6368 7261 6d71 0a20 2020  ol_matchramq.   
-00010f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f20: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-00010f30: 2020 2069 6620 6e6f 7420 6578 7465 6e73     if not extens
-00010f40: 696f 6e5f 666f 756e 643a 0a20 2020 2020  ion_found:.     
-00010f50: 2020 2020 2020 2020 2020 2070 6174 6965             patie
-00010f60: 6e74 2e65 7874 656e 7369 6f6e 2e61 7070  nt.extension.app
-00010f70: 656e 6428 6d61 7463 6872 616d 715f 6578  end(matchramq_ex
-00010f80: 7465 6e73 696f 6e29 0a0a 2020 2020 6465  tension)..    de
-00010f90: 6620 6765 745f 6d61 7463 6872 616d 7128  f get_matchramq(
-00010fa0: 7365 6c66 2c20 7061 7469 656e 743d 4e6f  self, patient=No
-00010fb0: 6e65 293a 0a20 2020 2020 2020 206d 6174  ne):.        mat
-00010fc0: 6368 7261 6d71 203d 2046 616c 7365 0a20  chramq = False. 
-00010fd0: 2020 2020 2020 2069 6620 7061 7469 656e         if patien
-00010fe0: 742e 6578 7465 6e73 696f 6e20 6973 206e  t.extension is n
-00010ff0: 6f74 204e 6f6e 653a 2020 2020 0a20 2020  ot None:    .   
-00011000: 2020 2020 2020 2020 2066 6f72 2065 7874           for ext
-00011010: 2069 6e20 7061 7469 656e 742e 6578 7465   in patient.exte
-00011020: 6e73 696f 6e3a 0a20 2020 2020 2020 2020  nsion:.         
-00011030: 2020 2020 2020 2069 6620 6578 742e 7572         if ext.ur
-00011040: 6c20 3d3d 2073 656c 662e 6d61 7463 6872  l == self.matchr
-00011050: 616d 715f 6578 7465 6e73 696f 6e5f 7572  amq_extension_ur
-00011060: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
-00011070: 2020 2020 2020 2072 6574 7572 6e20 6578         return ex
-00011080: 742e 7661 6c75 6542 6f6f 6c65 616e 0a20  t.valueBoolean. 
-00011090: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
-000110a0: 7463 6872 616d 7120 2020 2020 2020 200a  tchramq        .
-000110b0: 0a20 2020 2064 6566 2073 6574 5f61 6374  .    def set_act
-000110c0: 6976 6528 7365 6c66 2c20 6163 7469 7665  ive(self, active
-000110d0: 2c20 7061 7469 656e 743d 4e6f 6e65 293a  , patient=None):
-000110e0: 0a20 2020 2020 2020 2069 6620 7061 7469  .        if pati
-000110f0: 656e 7420 6973 204e 6f6e 653a 0a20 2020  ent is None:.   
-00011100: 2020 2020 2020 2020 2070 6174 6965 6e74           patient
-00011110: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
-00011120: 6f75 7263 650a 2020 2020 2020 2020 2020  ource.          
-00011130: 2020 7365 6c66 2e61 6374 6976 6520 3d20    self.active = 
-00011140: 6163 7469 7665 0a20 2020 2020 2020 2070  active.        p
-00011150: 6174 6965 6e74 2e61 6374 6976 6520 3d20  atient.active = 
-00011160: 6163 7469 7665 0a0a 2020 2020 6465 6620  active..    def 
-00011170: 6765 745f 6163 7469 7665 2873 656c 662c  get_active(self,
-00011180: 2070 6174 6965 6e74 3d4e 6f6e 6529 3a0a   patient=None):.
-00011190: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
-000111a0: 6e74 2069 7320 4e6f 6e65 3a0a 2020 2020  nt is None:.    
-000111b0: 2020 2020 2020 2020 7061 7469 656e 7420          patient 
-000111c0: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
-000111d0: 7572 6365 0a20 2020 2020 2020 2072 6574  urce.        ret
-000111e0: 7572 6e20 7061 7469 656e 742e 6163 7469  urn patient.acti
-000111f0: 7665 0a0a 2020 2020 6465 6620 7365 745f  ve..    def set_
-00011200: 6e61 6d65 2873 656c 662c 2067 6976 656e  name(self, given
-00011210: 5f6e 616d 653d 4e6f 6e65 2c20 6661 6d69  _name=None, fami
-00011220: 6c79 5f6e 616d 653d 4e6f 6e65 2c20 7061  ly_name=None, pa
-00011230: 7469 656e 743d 4e6f 6e65 293a 0a20 2020  tient=None):.   
-00011240: 2020 2020 2069 6620 7061 7469 656e 7420       if patient 
-00011250: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00011260: 2020 2020 2070 6174 6965 6e74 203d 2073       patient = s
-00011270: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
-00011280: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
-00011290: 6c66 2e67 6976 656e 5f6e 616d 6520 3d20  lf.given_name = 
-000112a0: 6769 7665 6e5f 6e61 6d65 0a20 2020 2020  given_name.     
-000112b0: 2020 2020 2020 2073 656c 662e 6661 6d69         self.fami
-000112c0: 6c79 5f6e 616d 6520 3d20 6661 6d69 6c79  ly_name = family
-000112d0: 5f6e 616d 650a 2020 2020 2020 2020 686e  _name.        hn
-000112e0: 203d 2073 656c 662e 6769 7665 6e5f 6661   = self.given_fa
-000112f0: 6d69 6c79 5f74 6f5f 6875 6d61 6e5f 6e61  mily_to_human_na
-00011300: 6d65 2867 6976 656e 5f6e 616d 653d 6769  me(given_name=gi
-00011310: 7665 6e5f 6e61 6d65 2c20 6661 6d69 6c79  ven_name, family
-00011320: 5f6e 616d 653d 6661 6d69 6c79 5f6e 616d  _name=family_nam
-00011330: 6529 0a20 2020 2020 2020 2069 6620 7061  e).        if pa
-00011340: 7469 656e 742e 6e61 6d65 2069 7320 4e6f  tient.name is No
-00011350: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00011360: 7061 7469 656e 742e 6e61 6d65 203d 205b  patient.name = [
-00011370: 686e 5d0a 0a20 2020 2064 6566 2067 6574  hn]..    def get
-00011380: 5f6e 616d 6528 7365 6c66 2c20 696e 6465  _name(self, inde
-00011390: 783d 302c 2070 6174 6965 6e74 3d4e 6f6e  x=0, patient=Non
-000113a0: 6529 3a0a 2020 2020 2020 2020 6966 2070  e):.        if p
-000113b0: 6174 6965 6e74 2069 7320 4e6f 6e65 3a0a  atient is None:.
-000113c0: 2020 2020 2020 2020 2020 2020 7061 7469              pati
-000113d0: 656e 7420 3d20 7365 6c66 2e66 6869 725f  ent = self.fhir_
-000113e0: 7265 736f 7572 6365 0a0a 2020 2020 2020  resource..      
-000113f0: 2020 7265 7475 726e 2070 6174 6965 6e74    return patient
-00011400: 2e6e 616d 655b 696e 6465 785d 0a0a 2020  .name[index]..  
-00011410: 2020 6465 6620 6765 745f 6769 7665 6e5f    def get_given_
-00011420: 6e61 6d65 2873 656c 662c 2069 6e64 6578  name(self, index
-00011430: 3d30 2c20 7061 7469 656e 743d 4e6f 6e65  =0, patient=None
-00011440: 293a 0a20 2020 2020 2020 2069 6620 7061  ):.        if pa
-00011450: 7469 656e 7420 6973 204e 6f6e 653a 0a20  tient is None:. 
-00011460: 2020 2020 2020 2020 2020 2070 6174 6965             patie
-00011470: 6e74 203d 2073 656c 662e 6668 6972 5f72  nt = self.fhir_r
-00011480: 6573 6f75 7263 650a 0a20 2020 2020 2020  esource..       
-00011490: 2067 6976 656e 5f6e 616d 6520 3d20 4e6f   given_name = No
-000114a0: 6e65 0a20 2020 2020 2020 2069 6620 7061  ne.        if pa
-000114b0: 7469 656e 742e 6e61 6d65 2069 7320 6e6f  tient.name is no
-000114c0: 7420 4e6f 6e65 2061 6e64 206c 656e 2870  t None and len(p
-000114d0: 6174 6965 6e74 2e6e 616d 6529 203e 2030  atient.name) > 0
-000114e0: 2061 6e64 206c 656e 2870 6174 6965 6e74   and len(patient
-000114f0: 2e6e 616d 655b 696e 6465 785d 2e67 6976  .name[index].giv
-00011500: 656e 2920 3e20 303a 0a20 2020 2020 2020  en) > 0:.       
-00011510: 2020 2020 2067 6976 656e 5f6e 616d 6520       given_name 
-00011520: 3d20 7061 7469 656e 742e 6e61 6d65 5b69  = patient.name[i
-00011530: 6e64 6578 5d2e 6769 7665 6e5b 696e 6465  ndex].given[inde
-00011540: 785d 0a20 2020 2020 2020 2072 6574 7572  x].        retur
-00011550: 6e20 6769 7665 6e5f 6e61 6d65 0a0a 2020  n given_name..  
-00011560: 2020 6465 6620 6765 745f 6661 6d69 6c79    def get_family
-00011570: 5f6e 616d 6528 7365 6c66 2c20 696e 6465  _name(self, inde
-00011580: 783d 302c 2070 6174 6965 6e74 3d4e 6f6e  x=0, patient=Non
-00011590: 6529 3a0a 2020 2020 2020 2020 6966 2070  e):.        if p
-000115a0: 6174 6965 6e74 2069 7320 4e6f 6e65 3a0a  atient is None:.
-000115b0: 2020 2020 2020 2020 2020 2020 7061 7469              pati
-000115c0: 656e 7420 3d20 7365 6c66 2e66 6869 725f  ent = self.fhir_
-000115d0: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
-000115e0: 2066 616d 696c 795f 6e61 6d65 203d 204e   family_name = N
-000115f0: 6f6e 650a 2020 2020 2020 2020 6966 2070  one.        if p
-00011600: 6174 6965 6e74 2e6e 616d 6520 6973 206e  atient.name is n
-00011610: 6f74 204e 6f6e 6520 616e 6420 6c65 6e28  ot None and len(
-00011620: 7061 7469 656e 742e 6e61 6d65 2920 3e20  patient.name) > 
-00011630: 3020 616e 6420 6c65 6e28 7061 7469 656e  0 and len(patien
-00011640: 742e 6e61 6d65 5b69 6e64 6578 5d2e 6661  t.name[index].fa
-00011650: 6d69 6c79 2920 3e20 303a 0a20 2020 2020  mily) > 0:.     
-00011660: 2020 2020 2020 2066 616d 696c 795f 6e61         family_na
-00011670: 6d65 203d 2070 6174 6965 6e74 2e6e 616d  me = patient.nam
-00011680: 655b 696e 6465 785d 2e66 616d 696c 795b  e[index].family[
-00011690: 696e 6465 785d 0a20 2020 2020 2020 2072  index].        r
-000116a0: 6574 7572 6e20 6661 6d69 6c79 5f6e 616d  eturn family_nam
-000116b0: 650a 0a20 2020 2064 6566 2073 6574 5f67  e..    def set_g
-000116c0: 656e 6465 7228 7365 6c66 2c20 6765 6e64  ender(self, gend
-000116d0: 6572 2c20 7061 7469 656e 743d 4e6f 6e65  er, patient=None
-000116e0: 293a 0a20 2020 2020 2020 2069 6620 7061  ):.        if pa
-000116f0: 7469 656e 7420 6973 204e 6f6e 653a 0a20  tient is None:. 
-00011700: 2020 2020 2020 2020 2020 2070 6174 6965             patie
-00011710: 6e74 203d 2073 656c 662e 6668 6972 5f72  nt = self.fhir_r
-00011720: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
-00011730: 2020 2020 7365 6c66 2e67 656e 6465 7220      self.gender 
-00011740: 3d20 6765 6e64 6572 0a0a 2020 2020 2020  = gender..      
-00011750: 2020 7061 7469 656e 742e 6765 6e64 6572    patient.gender
-00011760: 203d 2067 656e 6465 720a 0a20 2020 2064   = gender..    d
-00011770: 6566 2067 6574 5f67 656e 6465 7228 7365  ef get_gender(se
-00011780: 6c66 2c20 7061 7469 656e 743d 4e6f 6e65  lf, patient=None
-00011790: 293a 0a20 2020 2020 2020 2069 6620 7061  ):.        if pa
-000117a0: 7469 656e 7420 6973 204e 6f6e 653a 0a20  tient is None:. 
-000117b0: 2020 2020 2020 2020 2020 2070 6174 6965             patie
-000117c0: 6e74 203d 2073 656c 662e 6668 6972 5f72  nt = self.fhir_r
-000117d0: 6573 6f75 7263 650a 0a20 2020 2020 2020  esource..       
-000117e0: 2072 6574 7572 6e20 7061 7469 656e 742e   return patient.
-000117f0: 6765 6e64 6572 0a0a 2020 2020 6465 6620  gender..    def 
-00011800: 7365 745f 6e61 6d28 7365 6c66 2c20 6e61  set_nam(self, na
-00011810: 6d2c 2070 6174 6965 6e74 3d4e 6f6e 652c  m, patient=None,
-00011820: 2063 6f64 696e 675f 7379 7374 656d 3d4e   coding_system=N
-00011830: 6f6e 652c 2063 6f64 696e 675f 7665 7273  one, coding_vers
-00011840: 696f 6e3d 4e6f 6e65 293a 0a20 2020 2020  ion=None):.     
-00011850: 2020 2069 6620 7061 7469 656e 7420 6973     if patient is
-00011860: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00011870: 2020 2070 6174 6965 6e74 203d 2073 656c     patient = sel
-00011880: 662e 6668 6972 5f72 6573 6f75 7263 650a  f.fhir_resource.
-00011890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000118a0: 2e6e 616d 203d 206e 616d 0a20 2020 2020  .nam = nam.     
-000118b0: 2020 206e 616d 5f69 6465 6e74 6966 6965     nam_identifie
-000118c0: 7220 3d20 7365 6c66 2e6e 616d 5f74 6f5f  r = self.nam_to_
-000118d0: 6964 656e 7469 6669 6572 286e 616d 3d6e  identifier(nam=n
-000118e0: 616d 2c20 636f 6469 6e67 5f73 7973 7465  am, coding_syste
-000118f0: 6d3d 636f 6469 6e67 5f73 7973 7465 6d2c  m=coding_system,
-00011900: 2063 6f64 696e 675f 7665 7273 696f 6e3d   coding_version=
-00011910: 636f 6469 6e67 5f76 6572 7369 6f6e 290a  coding_version).
-00011920: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
-00011930: 6e74 2e69 6465 6e74 6966 6965 7220 6973  nt.identifier is
-00011940: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00011950: 2020 2070 6174 6965 6e74 2e69 6465 6e74     patient.ident
-00011960: 6966 6965 7220 3d20 5b6e 616d 5f69 6465  ifier = [nam_ide
-00011970: 6e74 6966 6965 725d 0a20 2020 2020 2020  ntifier].       
-00011980: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00011990: 2020 206e 616d 5f69 6465 6e74 6966 6965     nam_identifie
-000119a0: 725f 666f 756e 6420 3d20 4661 6c73 650a  r_found = False.
-000119b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000119c0: 6964 656e 7469 6669 6572 2069 6e20 7061  identifier in pa
-000119d0: 7469 656e 742e 6964 656e 7469 6669 6572  tient.identifier
-000119e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000119f0: 2020 6966 2069 6465 6e74 6966 6965 722e    if identifier.
-00011a00: 7379 7374 656d 203d 3d20 7365 6c66 2e6e  system == self.n
-00011a10: 616d 5f69 6465 6e74 6966 6965 725f 7379  am_identifier_sy
-00011a20: 7374 656d 3a0a 2020 2020 2020 2020 2020  stem:.          
-00011a30: 2020 2020 2020 2020 2020 6964 656e 7469            identi
-00011a40: 6669 6572 2e76 616c 7565 203d 206e 616d  fier.value = nam
-00011a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011a60: 2020 2020 206e 616d 5f69 6465 6e74 6966       nam_identif
-00011a70: 6965 725f 666f 756e 6420 3d20 5472 7565  ier_found = True
-00011a80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011a90: 6e6f 7420 6e61 6d5f 6964 656e 7469 6669  not nam_identifi
-00011aa0: 6572 5f66 6f75 6e64 2061 6e64 206e 616d  er_found and nam
-00011ab0: 5f69 6465 6e74 6966 6965 7220 6973 206e  _identifier is n
-00011ac0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00011ad0: 2020 2020 2020 2020 2070 6174 6965 6e74           patient
-00011ae0: 2e69 6465 6e74 6966 6965 722e 6170 7065  .identifier.appe
-00011af0: 6e64 286e 616d 5f69 6465 6e74 6966 6965  nd(nam_identifie
-00011b00: 7229 0a0a 2020 2020 6465 6620 6765 745f  r)..    def get_
-00011b10: 6e61 6d28 7365 6c66 2c20 7061 7469 656e  nam(self, patien
-00011b20: 743d 4e6f 6e65 293a 0a20 2020 2020 2020  t=None):.       
-00011b30: 206e 616d 203d 204e 6f6e 650a 2020 2020   nam = None.    
-00011b40: 2020 2020 6966 2070 6174 6965 6e74 2069      if patient i
-00011b50: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00011b60: 2020 2020 7061 7469 656e 7420 3d20 7365      patient = se
-00011b70: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
-00011b80: 0a20 2020 2020 2020 2069 6620 7061 7469  .        if pati
-00011b90: 656e 742e 6964 656e 7469 6669 6572 2069  ent.identifier i
-00011ba0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00011bb0: 2020 2020 2020 2020 666f 7220 6964 656e          for iden
-00011bc0: 7469 6669 6572 2069 6e20 7061 7469 656e  tifier in patien
-00011bd0: 742e 6964 656e 7469 6669 6572 3a0a 2020  t.identifier:.  
-00011be0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011bf0: 2069 6465 6e74 6966 6965 722e 7379 7374   identifier.syst
-00011c00: 656d 203d 3d20 7365 6c66 2e6e 616d 5f69  em == self.nam_i
-00011c10: 6465 6e74 6966 6965 725f 7379 7374 656d  dentifier_system
-00011c20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011c30: 2020 2020 2020 6e61 6d20 3d20 6964 656e        nam = iden
-00011c40: 7469 6669 6572 2e76 616c 7565 0a20 2020  tifier.value.   
-00011c50: 2020 2020 2072 6574 7572 6e20 6e61 6d0a       return nam.
-00011c60: 0a20 2020 2064 6566 2073 6574 5f6e 6975  .    def set_niu
-00011c70: 2873 656c 662c 206e 6975 2c20 7061 7469  (self, niu, pati
-00011c80: 656e 743d 4e6f 6e65 2c20 636f 6469 6e67  ent=None, coding
-00011c90: 5f73 7973 7465 6d3d 4e6f 6e65 2c20 636f  _system=None, co
-00011ca0: 6469 6e67 5f76 6572 7369 6f6e 3d4e 6f6e  ding_version=Non
-00011cb0: 6529 3a0a 2020 2020 2020 2020 6966 2070  e):.        if p
-00011cc0: 6174 6965 6e74 2069 7320 4e6f 6e65 3a0a  atient is None:.
-00011cd0: 2020 2020 2020 2020 2020 2020 7061 7469              pati
-00011ce0: 656e 7420 3d20 7365 6c66 2e66 6869 725f  ent = self.fhir_
-00011cf0: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
-00011d00: 2020 2020 2073 656c 662e 6e69 7520 3d20       self.niu = 
-00011d10: 6e69 750a 0a20 2020 2020 2020 206e 6975  niu..        niu
-00011d20: 5f69 6465 6e74 6966 6965 7220 3d20 7365  _identifier = se
-00011d30: 6c66 2e6e 6975 5f74 6f5f 6964 656e 7469  lf.niu_to_identi
-00011d40: 6669 6572 286e 6975 3d6e 6975 2c20 636f  fier(niu=niu, co
-00011d50: 6469 6e67 5f73 7973 7465 6d3d 636f 6469  ding_system=codi
-00011d60: 6e67 5f73 7973 7465 6d2c 2063 6f64 696e  ng_system, codin
-00011d70: 675f 7665 7273 696f 6e3d 636f 6469 6e67  g_version=coding
-00011d80: 5f76 6572 7369 6f6e 290a 2020 2020 2020  _version).      
-00011d90: 2020 6966 2070 6174 6965 6e74 2e69 6465    if patient.ide
-00011da0: 6e74 6966 6965 7220 6973 204e 6f6e 653a  ntifier is None:
-00011db0: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
-00011dc0: 6965 6e74 2e69 6465 6e74 6966 6965 7220  ient.identifier 
-00011dd0: 3d20 5b6e 6975 5f69 6465 6e74 6966 6965  = [niu_identifie
-00011de0: 725d 0a20 2020 2020 2020 2065 6c73 653a  r].        else:
-00011df0: 0a20 2020 2020 2020 2020 2020 206e 6975  .            niu
-00011e00: 5f69 6465 6e74 6966 6965 725f 666f 756e  _identifier_foun
-00011e10: 6420 3d20 4661 6c73 650a 2020 2020 2020  d = False.      
-00011e20: 2020 2020 2020 666f 7220 6964 656e 7469        for identi
-00011e30: 6669 6572 2069 6e20 7061 7469 656e 742e  fier in patient.
-00011e40: 6964 656e 7469 6669 6572 3a0a 2020 2020  identifier:.    
-00011e50: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00011e60: 6465 6e74 6966 6965 722e 7379 7374 656d  dentifier.system
-00011e70: 203d 3d20 7365 6c66 2e6e 6975 5f69 6465   == self.niu_ide
-00011e80: 6e74 6966 6965 725f 7379 7374 656d 3a0a  ntifier_system:.
-00011e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ea0: 2020 2020 6964 656e 7469 6669 6572 2e76      identifier.v
-00011eb0: 616c 7565 203d 206e 6975 0a20 2020 2020  alue = niu.     
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00011ed0: 6975 5f69 6465 6e74 6966 6965 725f 666f  iu_identifier_fo
-00011ee0: 756e 6420 3d20 5472 7565 0a20 2020 2020  und = True.     
-00011ef0: 2020 2020 2020 2069 6620 6e6f 7420 6e69         if not ni
-00011f00: 755f 6964 656e 7469 6669 6572 5f66 6f75  u_identifier_fou
-00011f10: 6e64 2061 6e64 206e 6975 5f69 6465 6e74  nd and niu_ident
-00011f20: 6966 6965 7220 6973 206e 6f74 204e 6f6e  ifier is not Non
-00011f30: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00011f40: 2020 2070 6174 6965 6e74 2e69 6465 6e74     patient.ident
-00011f50: 6966 6965 722e 6170 7065 6e64 286e 6975  ifier.append(niu
-00011f60: 5f69 6465 6e74 6966 6965 7229 0a0a 2020  _identifier)..  
-00011f70: 2020 6465 6620 6765 745f 6e69 7528 7365    def get_niu(se
-00011f80: 6c66 2c20 7061 7469 656e 743d 4e6f 6e65  lf, patient=None
-00011f90: 293a 0a20 2020 2020 2020 206e 6975 203d  ):.        niu =
-00011fa0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-00011fb0: 2070 6174 6965 6e74 2069 7320 4e6f 6e65   patient is None
-00011fc0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00011fd0: 7469 656e 7420 3d20 7365 6c66 2e66 6869  tient = self.fhi
-00011fe0: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
-00011ff0: 2020 2069 6620 7061 7469 656e 742e 6964     if patient.id
-00012000: 656e 7469 6669 6572 2069 7320 6e6f 7420  entifier is not 
-00012010: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00012020: 2020 666f 7220 6964 656e 7469 6669 6572    for identifier
-00012030: 2069 6e20 7061 7469 656e 742e 6964 656e   in patient.iden
-00012040: 7469 6669 6572 3a0a 2020 2020 2020 2020  tifier:.        
-00012050: 2020 2020 2020 2020 6966 2069 6465 6e74          if ident
-00012060: 6966 6965 722e 7379 7374 656d 203d 3d20  ifier.system == 
-00012070: 7365 6c66 2e6e 6975 5f69 6465 6e74 6966  self.niu_identif
-00012080: 6965 725f 7379 7374 656d 3a0a 2020 2020  ier_system:.    
-00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120a0: 6e69 7520 3d20 6964 656e 7469 6669 6572  niu = identifier
-000120b0: 2e76 616c 7565 0a20 2020 2020 2020 2072  .value.        r
-000120c0: 6574 7572 6e20 6e69 750a 0a20 2020 2064  eturn niu..    d
-000120d0: 6566 2073 6574 5f61 7563 756e 5f69 6465  ef set_aucun_ide
-000120e0: 6e74 6966 6961 6e74 2873 656c 662c 2070  ntifiant(self, p
-000120f0: 6174 6965 6e74 3d4e 6f6e 652c 2063 6f64  atient=None, cod
-00012100: 696e 675f 7379 7374 656d 3d4e 6f6e 652c  ing_system=None,
-00012110: 2063 6f64 696e 675f 7665 7273 696f 6e3d   coding_version=
-00012120: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
-00012130: 6620 7061 7469 656e 7420 6973 204e 6f6e  f patient is Non
-00012140: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-00012150: 6174 6965 6e74 203d 2073 656c 662e 6668  atient = self.fh
-00012160: 6972 5f72 6573 6f75 7263 650a 0a20 2020  ir_resource..   
-00012170: 2020 2020 2061 7563 756e 5f69 6465 6e74       aucun_ident
-00012180: 6966 6965 7220 3d20 7365 6c66 2e61 7563  ifier = self.auc
-00012190: 756e 5f69 6465 6e74 6966 6961 6e74 5f74  un_identifiant_t
-000121a0: 6f5f 6964 656e 7469 6669 6572 2863 6f64  o_identifier(cod
-000121b0: 696e 675f 7379 7374 656d 3d63 6f64 696e  ing_system=codin
-000121c0: 675f 7379 7374 656d 2c20 636f 6469 6e67  g_system, coding
-000121d0: 5f76 6572 7369 6f6e 3d63 6f64 696e 675f  _version=coding_
-000121e0: 7665 7273 696f 6e29 0a20 2020 2020 2020  version).       
-000121f0: 2070 6174 6965 6e74 2e69 6465 6e74 6966   patient.identif
-00012200: 6965 7220 3d20 5b61 7563 756e 5f69 6465  ier = [aucun_ide
-00012210: 6e74 6966 6965 725d 0a0a 2020 2020 6465  ntifier]..    de
-00012220: 6620 7365 745f 6269 7274 685f 6461 7465  f set_birth_date
-00012230: 2873 656c 662c 2073 7472 5f64 6174 652c  (self, str_date,
-00012240: 2070 6174 6965 6e74 3d4e 6f6e 6529 3a0a   patient=None):.
-00012250: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
-00012260: 6e74 2069 7320 4e6f 6e65 3a0a 2020 2020  nt is None:.    
-00012270: 2020 2020 2020 2020 7061 7469 656e 7420          patient 
-00012280: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
-00012290: 7572 6365 0a20 2020 2020 2020 2020 2020  urce.           
-000122a0: 2073 656c 662e 6269 7274 685f 6461 7465   self.birth_date
-000122b0: 203d 2073 7472 5f64 6174 650a 2020 2020   = str_date.    
-000122c0: 2020 2020 7061 7469 656e 742e 6269 7274      patient.birt
-000122d0: 6844 6174 6520 3d20 7365 6c66 2e73 7472  hDate = self.str
-000122e0: 5f64 6174 655f 746f 5f66 6869 725f 6461  _date_to_fhir_da
-000122f0: 7465 2873 7472 5f64 6174 6529 0a0a 2020  te(str_date)..  
-00012300: 2020 6465 6620 6765 745f 6269 7274 685f    def get_birth_
-00012310: 6461 7465 2873 656c 662c 2070 6174 6965  date(self, patie
-00012320: 6e74 3d4e 6f6e 6529 3a0a 2020 2020 2020  nt=None):.      
-00012330: 2020 6966 2070 6174 6965 6e74 2069 7320    if patient is 
-00012340: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00012350: 2020 7061 7469 656e 7420 3d20 7365 6c66    patient = self
-00012360: 2e66 6869 725f 7265 736f 7572 6365 0a20  .fhir_resource. 
-00012370: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00012380: 6c66 2e66 6869 725f 6461 7465 5f74 6f5f  lf.fhir_date_to_
-00012390: 7374 725f 6461 7465 2866 6869 725f 6461  str_date(fhir_da
-000123a0: 7465 3d70 6174 6965 6e74 2e62 6972 7468  te=patient.birth
-000123b0: 4461 7465 290a 0a20 2020 2064 6566 2073  Date)..    def s
-000123c0: 6574 5f61 6464 7265 7373 2873 656c 662c  et_address(self,
-000123d0: 2061 6464 7265 7373 5f6c 696e 653d 4e6f   address_line=No
-000123e0: 6e65 2c20 6164 6472 6573 735f 6369 7479  ne, address_city
-000123f0: 3d4e 6f6e 652c 2061 6464 7265 7373 5f73  =None, address_s
-00012400: 7461 7465 3d4e 6f6e 652c 2061 6464 7265  tate=None, addre
-00012410: 7373 5f70 6f73 7461 6c5f 636f 6465 3d4e  ss_postal_code=N
-00012420: 6f6e 652c 2061 6464 7265 7373 5f63 6f75  one, address_cou
-00012430: 6e74 7279 3d4e 6f6e 652c 2070 6174 6965  ntry=None, patie
-00012440: 6e74 3d4e 6f6e 6529 3a0a 2020 2020 2020  nt=None):.      
-00012450: 2020 6966 2070 6174 6965 6e74 2069 7320    if patient is 
-00012460: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00012470: 2020 7061 7469 656e 7420 3d20 7365 6c66    patient = self
-00012480: 2e66 6869 725f 7265 736f 7572 6365 0a20  .fhir_resource. 
-00012490: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000124a0: 6164 6472 6573 735f 6369 7479 203d 2061  address_city = a
-000124b0: 6464 7265 7373 5f63 6974 790a 2020 2020  ddress_city.    
-000124c0: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
-000124d0: 7265 7373 5f63 6f75 6e74 7279 203d 2061  ress_country = a
-000124e0: 6464 7265 7373 5f63 6f75 6e74 7279 0a20  ddress_country. 
-000124f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012500: 6164 6472 6573 735f 6c69 6e65 203d 2061  address_line = a
-00012510: 6464 7265 7373 5f6c 696e 650a 2020 2020  ddress_line.    
-00012520: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
-00012530: 7265 7373 5f70 6f73 7461 6c5f 636f 6465  ress_postal_code
-00012540: 203d 2061 6464 7265 7373 5f70 6f73 7461   = address_posta
-00012550: 6c5f 636f 6465 0a20 2020 2020 2020 2020  l_code.         
-00012560: 2020 2073 656c 662e 6164 6472 6573 735f     self.address_
-00012570: 7374 6174 6520 3d20 6164 6472 6573 735f  state = address_
-00012580: 7374 6174 650a 2020 2020 2020 2020 6164  state.        ad
-00012590: 6472 6573 7320 3d20 4164 6472 6573 7328  dress = Address(
-000125a0: 290a 2020 2020 2020 2020 6164 6472 6573  ).        addres
-000125b0: 732e 6369 7479 203d 2061 6464 7265 7373  s.city = address
-000125c0: 5f63 6974 790a 2020 2020 2020 2020 6164  _city.        ad
-000125d0: 6472 6573 732e 636f 756e 7472 7920 3d20  dress.country = 
-000125e0: 6164 6472 6573 735f 636f 756e 7472 790a  address_country.
-000125f0: 2020 2020 2020 2020 6164 6472 6573 732e          address.
-00012600: 7374 6174 6520 3d20 6164 6472 6573 735f  state = address_
-00012610: 7374 6174 650a 2020 2020 2020 2020 6164  state.        ad
-00012620: 6472 6573 732e 706f 7374 616c 436f 6465  dress.postalCode
-00012630: 203d 2061 6464 7265 7373 5f70 6f73 7461   = address_posta
-00012640: 6c5f 636f 6465 0a20 2020 2020 2020 2061  l_code.        a
-00012650: 6464 7265 7373 2e6c 696e 6520 3d20 5b61  ddress.line = [a
-00012660: 6464 7265 7373 5f6c 696e 655d 0a20 2020  ddress_line].   
-00012670: 2020 2020 2070 6174 6965 6e74 2e61 6464       patient.add
-00012680: 7265 7373 203d 205b 6164 6472 6573 735d  ress = [address]
-00012690: 0a0a 2020 2020 6465 6620 6765 745f 6164  ..    def get_ad
-000126a0: 6472 6573 7328 7365 6c66 2c20 7061 7469  dress(self, pati
-000126b0: 656e 743d 4e6f 6e65 2c20 696e 6465 783d  ent=None, index=
-000126c0: 3029 3a0a 2020 2020 2020 2020 6966 2070  0):.        if p
-000126d0: 6174 6965 6e74 2069 7320 4e6f 6e65 3a0a  atient is None:.
-000126e0: 2020 2020 2020 2020 2020 2020 7061 7469              pati
-000126f0: 656e 7420 3d20 7365 6c66 2e66 6869 725f  ent = self.fhir_
-00012700: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
-00012710: 2069 6620 7061 7469 656e 742e 6164 6472   if patient.addr
-00012720: 6573 7320 6973 206e 6f74 204e 6f6e 6520  ess is not None 
-00012730: 616e 6420 6c65 6e28 7061 7469 656e 742e  and len(patient.
-00012740: 6164 6472 6573 7329 203e 2069 6e64 6578  address) > index
-00012750: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00012760: 7475 726e 2070 6174 6965 6e74 2e61 6464  turn patient.add
-00012770: 7265 7373 5b69 6e64 6578 5d0a 2020 2020  ress[index].    
-00012780: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00012790: 0a20 2020 2064 6566 2073 6574 5f6d 6f74  .    def set_mot
-000127a0: 6865 725f 6e61 6d65 2873 656c 662c 206d  her_name(self, m
-000127b0: 6f74 6865 725f 6769 7665 6e5f 6e61 6d65  other_given_name
-000127c0: 3d4e 6f6e 652c 206d 6f74 6865 725f 6661  =None, mother_fa
-000127d0: 6d69 6c79 5f6e 616d 653d 4e6f 6e65 2c20  mily_name=None, 
-000127e0: 7061 7469 656e 743d 4e6f 6e65 2c20 636f  patient=None, co
-000127f0: 6469 6e67 5f73 7973 7465 6d3d 4e6f 6e65  ding_system=None
-00012800: 2c20 636f 6469 6e67 5f76 6572 7369 6f6e  , coding_version
-00012810: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00012820: 6966 2070 6174 6965 6e74 2069 7320 4e6f  if patient is No
-00012830: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00012840: 7061 7469 656e 7420 3d20 7365 6c66 2e66  patient = self.f
-00012850: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
-00012860: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
-00012870: 7468 6572 5f66 616d 696c 795f 6e61 6d65  ther_family_name
-00012880: 203d 206d 6f74 6865 725f 6661 6d69 6c79   = mother_family
-00012890: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
-000128a0: 2020 7365 6c66 2e6d 6f74 6865 725f 6769    self.mother_gi
-000128b0: 7665 6e5f 6e61 6d65 203d 206d 6f74 6865  ven_name = mothe
-000128c0: 725f 6769 7665 6e5f 6e61 6d65 0a20 2020  r_given_name.   
-000128d0: 2020 2020 206d 6f74 6865 725f 636f 6469       mother_codi
-000128e0: 6e67 5f73 7973 7465 6d20 3d20 636f 6469  ng_system = codi
-000128f0: 6e67 5f73 7973 7465 6d20 6966 2063 6f64  ng_system if cod
-00012900: 696e 675f 7379 7374 656d 2069 7320 6e6f  ing_system is no
-00012910: 7420 4e6f 6e65 2065 6c73 6520 7365 6c66  t None else self
-00012920: 2e64 6566 6175 6c74 5f63 6f64 696e 675f  .default_coding_
-00012930: 7379 7374 656d 0a20 2020 2020 2020 206d  system.        m
-00012940: 6f74 6865 725f 636f 6469 6e67 5f76 6572  other_coding_ver
-00012950: 7369 6f6e 203d 2063 6f64 696e 675f 7379  sion = coding_sy
-00012960: 7374 656d 2069 6620 636f 6469 6e67 5f76  stem if coding_v
-00012970: 6572 7369 6f6e 2069 7320 6e6f 7420 4e6f  ersion is not No
-00012980: 6e65 2065 6c73 6520 7365 6c66 2e64 6566  ne else self.def
-00012990: 6175 6c74 5f63 6f64 696e 675f 7665 7273  ault_coding_vers
-000129a0: 696f 6e0a 2020 2020 2020 2020 636f 6e74  ion.        cont
-000129b0: 6163 7420 3d20 5061 7469 656e 7443 6f6e  act = PatientCon
-000129c0: 7461 6374 2829 0a20 2020 2020 2020 2068  tact().        h
-000129d0: 6e20 3d20 7365 6c66 2e67 6976 656e 5f66  n = self.given_f
-000129e0: 616d 696c 795f 746f 5f68 756d 616e 5f6e  amily_to_human_n
-000129f0: 616d 6528 6769 7665 6e5f 6e61 6d65 3d6d  ame(given_name=m
-00012a00: 6f74 6865 725f 6769 7665 6e5f 6e61 6d65  other_given_name
-00012a10: 2c20 6661 6d69 6c79 5f6e 616d 653d 6d6f  , family_name=mo
-00012a20: 7468 6572 5f66 616d 696c 795f 6e61 6d65  ther_family_name
-00012a30: 290a 2020 2020 2020 2020 636f 6e74 6163  ).        contac
-00012a40: 742e 6e61 6d65 203d 2068 6e0a 2020 2020  t.name = hn.    
-00012a50: 2020 2020 6d6f 7468 6572 5f63 6f64 6162      mother_codab
-00012a60: 6c65 5f63 6f6e 6365 7074 203d 2043 6f64  le_concept = Cod
-00012a70: 6561 626c 6543 6f6e 6365 7074 2829 0a20  eableConcept(). 
-00012a80: 2020 2020 2020 206d 6f74 6865 725f 636f         mother_co
-00012a90: 6461 626c 655f 636f 6e63 6570 742e 636f  dable_concept.co
-00012aa0: 6469 6e67 203d 205b 0a20 2020 2020 2020  ding = [.       
-00012ab0: 2020 2020 2043 6f64 696e 6728 0a20 2020       Coding(.   
-00012ac0: 2020 2020 2020 2020 2020 2020 206a 736f               jso
-00012ad0: 6e64 6963 743d 7b0a 2020 2020 2020 2020  ndict={.        
-00012ae0: 2020 2020 2020 2020 2020 2020 2273 7973              "sys
-00012af0: 7465 6d22 3a20 6d6f 7468 6572 5f63 6f64  tem": mother_cod
-00012b00: 696e 675f 7379 7374 656d 2c0a 2020 2020  ing_system,.    
-00012b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b20: 2276 6572 7369 6f6e 223a 206d 6f74 6865  "version": mothe
-00012b30: 725f 636f 6469 6e67 5f76 6572 7369 6f6e  r_coding_version
-00012b40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00012b50: 2020 2020 2020 2263 6f64 6522 3a20 224d        "code": "M
-00012b60: 4552 4522 2c0a 2020 2020 2020 2020 2020  ERE",.          
-00012b70: 2020 2020 2020 2020 2020 2264 6973 706c            "displ
-00012b80: 6179 223a 2022 4dc3 a872 6522 0a20 2020  ay": "M..re".   
-00012b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ba0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00012bb0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00012bc0: 205d 0a20 2020 2020 2020 2063 6f6e 7461   ].        conta
-00012bd0: 6374 2e72 656c 6174 696f 6e73 6869 7020  ct.relationship 
-00012be0: 3d20 5b6d 6f74 6865 725f 636f 6461 626c  = [mother_codabl
-00012bf0: 655f 636f 6e63 6570 745d 0a20 2020 2020  e_concept].     
-00012c00: 2020 2069 6620 7061 7469 656e 742e 636f     if patient.co
-00012c10: 6e74 6163 7420 6973 204e 6f6e 653a 0a20  ntact is None:. 
-00012c20: 2020 2020 2020 2020 2020 2070 6174 6965             patie
-00012c30: 6e74 2e63 6f6e 7461 6374 203d 205b 636f  nt.contact = [co
-00012c40: 6e74 6163 745d 0a20 2020 2020 2020 2065  ntact].        e
-00012c50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00012c60: 2063 6f6e 7461 6374 5f66 6f75 6e64 203d   contact_found =
-00012c70: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00012c80: 2020 2066 6f72 2070 6174 6965 6e74 5f63     for patient_c
-00012c90: 6f6e 7461 6374 2069 6e20 7061 7469 656e  ontact in patien
-00012ca0: 742e 636f 6e74 6163 743a 0a20 2020 2020  t.contact:.     
-00012cb0: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
-00012cc0: 656c 6174 696f 6e73 6869 7020 696e 2070  elationship in p
-00012cd0: 6174 6965 6e74 5f63 6f6e 7461 6374 2e72  atient_contact.r
-00012ce0: 656c 6174 696f 6e73 6869 703a 0a20 2020  elationship:.   
-00012cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d00: 2066 6f72 2063 6f64 696e 6720 696e 2072   for coding in r
-00012d10: 656c 6174 696f 6e73 6869 702e 636f 6469  elationship.codi
-00012d20: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-00012d30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00012d40: 6d6f 7468 6572 5f63 6f64 6162 6c65 5f63  mother_codable_c
-00012d50: 6f6e 6365 7074 5f63 6f64 696e 6720 696e  oncept_coding in
-00012d60: 206d 6f74 6865 725f 636f 6461 626c 655f   mother_codable_
-00012d70: 636f 6e63 6570 742e 636f 6469 6e67 3a0a  concept.coding:.
-00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d90: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00012da0: 6f64 696e 672e 636f 6465 203d 3d20 6d6f  oding.code == mo
-00012db0: 7468 6572 5f63 6f64 6162 6c65 5f63 6f6e  ther_codable_con
-00012dc0: 6365 7074 5f63 6f64 696e 672e 636f 6465  cept_coding.code
-00012dd0: 2061 6e64 2063 6f64 696e 672e 7379 7374   and coding.syst
-00012de0: 656d 203d 3d20 6d6f 7468 6572 5f63 6f64  em == mother_cod
-00012df0: 6162 6c65 5f63 6f6e 6365 7074 5f63 6f64  able_concept_cod
-00012e00: 696e 6720 616e 6420 636f 6469 6e67 2e76  ing and coding.v
-00012e10: 6572 7369 6f6e 2061 6e64 206d 6f74 6865  ersion and mothe
-00012e20: 725f 636f 6461 626c 655f 636f 6e63 6570  r_codable_concep
-00012e30: 745f 636f 6469 6e67 2e76 6572 7369 6f6e  t_coding.version
-00012e40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e60: 2020 7061 7469 656e 745f 636f 6e74 6163    patient_contac
-00012e70: 7420 3d20 636f 6e74 6163 740a 2020 2020  t = contact.    
+0000a6a0: 2020 2069 6d6d 756e 697a 6174 696f 6e2e     immunization.
+0000a6b0: 7065 7266 6f72 6d65 7220 3d20 7365 6c66  performer = self
+0000a6c0: 2e70 6572 666f 726d 6572 0a20 2020 2020  .performer.     
+0000a6d0: 2020 2065 6c69 6620 7365 6c66 2e70 6572     elif self.per
+0000a6e0: 666f 726d 6572 5f72 6566 6572 656e 6365  former_reference
+0000a6f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000a700: 2020 2020 2020 2020 2020 7265 6620 3d20            ref = 
+0000a710: 4648 4952 5265 6665 7265 6e63 6528 290a  FHIRReference().
+0000a720: 2020 2020 2020 2020 2020 2020 7265 662e              ref.
+0000a730: 7265 6665 7265 6e63 6520 3d20 7365 6c66  reference = self
+0000a740: 2e70 6572 666f 726d 6572 5f72 6566 6572  .performer_refer
+0000a750: 656e 6365 0a20 2020 2020 2020 2020 2020  ence.           
+0000a760: 2072 6566 2e64 6973 706c 6179 203d 2073   ref.display = s
+0000a770: 656c 662e 7065 7266 6f72 6d65 725f 6469  elf.performer_di
+0000a780: 7370 6c61 790a 2020 2020 2020 2020 2020  splay.          
+0000a790: 2020 696d 6d75 6e69 7a61 7469 6f6e 2e70    immunization.p
+0000a7a0: 6572 666f 726d 6572 203d 2072 6566 0a0a  erformer = ref..
+0000a7b0: 2020 2020 6465 6620 6765 745f 6c6f 6361      def get_loca
+0000a7c0: 7469 6f6e 2873 656c 662c 2069 6d6d 756e  tion(self, immun
+0000a7d0: 697a 6174 696f 6e3d 4e6f 6e65 293a 0a20  ization=None):. 
+0000a7e0: 2020 2020 2020 2069 6620 696d 6d75 6e69         if immuni
+0000a7f0: 7a61 7469 6f6e 2069 7320 4e6f 6e65 3a0a  zation is None:.
+0000a800: 2020 2020 2020 2020 2020 2020 696d 6d75              immu
+0000a810: 6e69 7a61 7469 6f6e 203d 2073 656c 662e  nization = self.
+0000a820: 6668 6972 5f72 6573 6f75 7263 650a 2020  fhir_resource.  
+0000a830: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
+0000a840: 6174 696f 6e2e 6c6f 6361 7469 6f6e 2069  ation.location i
+0000a850: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2074  s not None and t
+0000a860: 7970 6528 696d 6d75 6e69 7a61 7469 6f6e  ype(immunization
+0000a870: 2e6c 6f63 6174 696f 6e29 2069 7320 4c6f  .location) is Lo
+0000a880: 6361 7469 6f6e 3a0a 2020 2020 2020 2020  cation:.        
+0000a890: 2020 2020 7265 7475 726e 2069 6d6d 756e      return immun
+0000a8a0: 697a 6174 696f 6e2e 6c6f 6361 7469 6f6e  ization.location
+0000a8b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000a8c0: 4e6f 6e65 0a0a 2020 2020 6465 6620 6765  None..    def ge
+0000a8d0: 745f 6c6f 6361 7469 6f6e 5f72 6566 6572  t_location_refer
+0000a8e0: 656e 6365 2873 656c 662c 2069 6d6d 756e  ence(self, immun
+0000a8f0: 697a 6174 696f 6e3d 4e6f 6e65 293a 0a20  ization=None):. 
+0000a900: 2020 2020 2020 2069 6620 696d 6d75 6e69         if immuni
+0000a910: 7a61 7469 6f6e 2069 7320 4e6f 6e65 3a0a  zation is None:.
+0000a920: 2020 2020 2020 2020 2020 2020 696d 6d75              immu
+0000a930: 6e69 7a61 7469 6f6e 203d 2073 656c 662e  nization = self.
+0000a940: 6668 6972 5f72 6573 6f75 7263 650a 2020  fhir_resource.  
+0000a950: 2020 2020 2020 6966 2069 6d6d 756e 697a        if immuniz
+0000a960: 6174 696f 6e2e 6c6f 6361 7469 6f6e 2069  ation.location i
+0000a970: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2074  s not None and t
+0000a980: 7970 6528 696d 6d75 6e69 7a61 7469 6f6e  ype(immunization
+0000a990: 2e6c 6f63 6174 696f 6e29 2069 7320 4648  .location) is FH
+0000a9a0: 4952 5265 6665 7265 6e63 653a 0a20 2020  IRReference:.   
+0000a9b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000a9c0: 696d 6d75 6e69 7a61 7469 6f6e 2e6c 6f63  immunization.loc
+0000a9d0: 6174 696f 6e0a 2020 2020 2020 2020 7265  ation.        re
+0000a9e0: 7475 726e 204e 6f6e 650a 0a20 2020 2064  turn None..    d
+0000a9f0: 6566 2073 6574 5f6c 6f63 6174 696f 6e28  ef set_location(
+0000aa00: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
+0000aa10: 6f6e 3d4e 6f6e 652c 206c 6f63 6174 696f  on=None, locatio
+0000aa20: 6e3d 4e6f 6e65 2c20 6c6f 6361 7469 6f6e  n=None, location
+0000aa30: 5f72 6566 6572 656e 6365 3d4e 6f6e 652c  _reference=None,
+0000aa40: 206c 6f63 6174 696f 6e5f 6469 7370 6c61   location_displa
+0000aa50: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
+0000aa60: 2069 6620 696d 6d75 6e69 7a61 7469 6f6e   if immunization
+0000aa70: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000aa80: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
+0000aa90: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
+0000aaa0: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
+0000aab0: 6966 206c 6f63 6174 696f 6e20 6973 206e  if location is n
+0000aac0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000aad0: 2020 2020 2073 656c 662e 6c6f 6361 7469       self.locati
+0000aae0: 6f6e 3d6c 6f63 6174 696f 6e0a 2020 2020  on=location.    
+0000aaf0: 2020 2020 6966 206c 6f63 6174 696f 6e5f      if location_
+0000ab00: 7265 6665 7265 6e63 6520 6973 206e 6f74  reference is not
+0000ab10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000ab20: 2020 2073 656c 662e 6c6f 6361 7469 6f6e     self.location
+0000ab30: 5f72 6566 6572 656e 6365 203d 206c 6f63  _reference = loc
+0000ab40: 6174 696f 6e5f 7265 6665 7265 6e63 650a  ation_reference.
+0000ab50: 2020 2020 2020 2020 6966 206c 6f63 6174          if locat
+0000ab60: 696f 6e5f 6469 7370 6c61 7920 6973 206e  ion_display is n
+0000ab70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000ab80: 2020 2020 2073 656c 662e 6c6f 6361 7469       self.locati
+0000ab90: 6f6e 5f64 6973 706c 6179 203d 206c 6f63  on_display = loc
+0000aba0: 6174 696f 6e5f 6469 7370 6c61 790a 0a20  ation_display.. 
+0000abb0: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+0000abc0: 6f63 6174 696f 6e20 6973 206e 6f74 204e  ocation is not N
+0000abd0: 6f6e 6520 616e 6420 7365 6c66 2e6c 6f63  one and self.loc
+0000abe0: 6174 696f 6e5f 7265 6665 7265 6e63 6520  ation_reference 
+0000abf0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000ac00: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
+0000ac10: 6e2e 6c6f 6361 7469 6f6e 203d 2073 656c  n.location = sel
+0000ac20: 662e 6c6f 6361 7469 6f6e 0a20 2020 2020  f.location.     
+0000ac30: 2020 2065 6c69 6620 7365 6c66 2e6c 6f63     elif self.loc
+0000ac40: 6174 696f 6e5f 7265 6665 7265 6e63 6520  ation_reference 
+0000ac50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000ac60: 2020 2020 2020 2020 2072 6566 203d 2046           ref = F
+0000ac70: 4849 5252 6566 6572 656e 6365 2829 0a20  HIRReference(). 
+0000ac80: 2020 2020 2020 2020 2020 2072 6566 2e72             ref.r
+0000ac90: 6566 6572 656e 6365 203d 2073 656c 662e  eference = self.
+0000aca0: 6c6f 6361 7469 6f6e 5f72 6566 6572 656e  location_referen
+0000acb0: 6365 0a20 2020 2020 2020 2020 2020 2072  ce.            r
+0000acc0: 6566 2e64 6973 706c 6179 203d 2073 656c  ef.display = sel
+0000acd0: 662e 6c6f 6361 7469 6f6e 5f64 6973 706c  f.location_displ
+0000ace0: 6179 0a20 2020 2020 2020 2020 2020 2069  ay.            i
+0000acf0: 6d6d 756e 697a 6174 696f 6e2e 6c6f 6361  mmunization.loca
+0000ad00: 7469 6f6e 203d 2072 6566 0a0a 2020 2020  tion = ref..    
+0000ad10: 6465 6620 6765 745f 6c6f 745f 6e75 6d62  def get_lot_numb
+0000ad20: 6572 2873 656c 662c 2069 6d6d 756e 697a  er(self, immuniz
+0000ad30: 6174 696f 6e3d 4e6f 6e65 293a 0a20 2020  ation=None):.   
+0000ad40: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
+0000ad50: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
+0000ad60: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
+0000ad70: 7a61 7469 6f6e 203d 2073 656c 662e 6668  zation = self.fh
+0000ad80: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
+0000ad90: 2020 2020 7265 7475 726e 2069 6d6d 756e      return immun
+0000ada0: 697a 6174 696f 6e2e 6c6f 744e 756d 6265  ization.lotNumbe
+0000adb0: 720a 0a20 2020 2064 6566 2073 6574 5f6c  r..    def set_l
+0000adc0: 6f74 5f6e 756d 6265 7228 7365 6c66 2c20  ot_number(self, 
+0000add0: 696d 6d75 6e69 7a61 7469 6f6e 3d4e 6f6e  immunization=Non
+0000ade0: 652c 206c 6f74 5f6e 756d 6265 723d 4e6f  e, lot_number=No
+0000adf0: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
+0000ae00: 696d 6d75 6e69 7a61 7469 6f6e 2069 7320  immunization is 
+0000ae10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000ae20: 2020 696d 6d75 6e69 7a61 7469 6f6e 203d    immunization =
+0000ae30: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
+0000ae40: 7263 650a 2020 2020 2020 2020 6966 206c  rce.        if l
+0000ae50: 6f74 5f6e 756d 6265 7220 6973 206e 6f74  ot_number is not
+0000ae60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000ae70: 2020 2073 656c 662e 6c6f 745f 6e75 6d62     self.lot_numb
+0000ae80: 6572 203d 206c 6f74 5f6e 756d 6265 720a  er = lot_number.
+0000ae90: 2020 2020 2020 2020 696d 6d75 6e69 7a61          immuniza
+0000aea0: 7469 6f6e 2e6c 6f74 4e75 6d62 6572 203d  tion.lotNumber =
+0000aeb0: 2073 656c 662e 6c6f 745f 6e75 6d62 6572   self.lot_number
+0000aec0: 0a0a 2020 2020 6465 6620 6765 745f 6578  ..    def get_ex
+0000aed0: 7069 7261 7469 6f6e 5f64 6174 6528 7365  piration_date(se
+0000aee0: 6c66 2c20 696d 6d75 6e69 7a61 7469 6f6e  lf, immunization
+0000aef0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0000af00: 6966 2069 6d6d 756e 697a 6174 696f 6e20  if immunization 
+0000af10: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000af20: 2020 2020 2069 6d6d 756e 697a 6174 696f       immunizatio
+0000af30: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
+0000af40: 736f 7572 6365 0a20 2020 2020 2020 2069  source.        i
+0000af50: 6620 696d 6d75 6e69 7a61 7469 6f6e 2e65  f immunization.e
+0000af60: 7870 6972 6174 696f 6e44 6174 6520 6973  xpirationDate is
+0000af70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000af80: 2020 2020 2020 2072 6574 7572 6e20 696d         return im
+0000af90: 6d75 6e69 7a61 7469 6f6e 2e65 7870 6972  munization.expir
+0000afa0: 6174 696f 6e44 6174 652e 6973 6f73 7472  ationDate.isostr
+0000afb0: 696e 670a 0a20 2020 2064 6566 2073 6574  ing..    def set
+0000afc0: 5f65 7870 6972 6174 696f 6e5f 6461 7465  _expiration_date
+0000afd0: 2873 656c 662c 2069 6d6d 756e 697a 6174  (self, immunizat
+0000afe0: 696f 6e3d 4e6f 6e65 2c20 6578 7069 7261  ion=None, expira
+0000aff0: 7469 6f6e 5f64 6174 653d 4e6f 6e65 293a  tion_date=None):
+0000b000: 0a20 2020 2020 2020 2069 6620 696d 6d75  .        if immu
+0000b010: 6e69 7a61 7469 6f6e 2069 7320 4e6f 6e65  nization is None
+0000b020: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
+0000b030: 6d75 6e69 7a61 7469 6f6e 203d 2073 656c  munization = sel
+0000b040: 662e 6668 6972 5f72 6573 6f75 7263 650a  f.fhir_resource.
+0000b050: 2020 2020 2020 2020 6966 2065 7870 6972          if expir
+0000b060: 6174 696f 6e5f 6461 7465 2069 7320 6e6f  ation_date is no
+0000b070: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000b080: 2020 2020 7365 6c66 2e65 7870 6972 6174      self.expirat
+0000b090: 696f 6e5f 6461 7465 203d 2065 7870 6972  ion_date = expir
+0000b0a0: 6174 696f 6e5f 6461 7465 0a20 2020 2020  ation_date.     
+0000b0b0: 2020 2069 6620 7365 6c66 2e65 7870 6972     if self.expir
+0000b0c0: 6174 696f 6e5f 6461 7465 2069 7320 6e6f  ation_date is no
+0000b0d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000b0e0: 2020 2020 6966 2074 7970 6528 7365 6c66      if type(self
+0000b0f0: 2e65 7870 6972 6174 696f 6e5f 6461 7465  .expiration_date
+0000b100: 2920 6973 2073 7472 3a0a 2020 2020 2020  ) is str:.      
+0000b110: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
+0000b120: 7a61 7469 6f6e 2e65 7870 6972 6174 696f  zation.expiratio
+0000b130: 6e44 6174 6520 3d20 6461 7465 7469 6d65  nDate = datetime
+0000b140: 2e73 7472 7074 696d 6528 7365 6c66 2e65  .strptime(self.e
+0000b150: 7870 6972 6174 696f 6e5f 6461 7465 2c20  xpiration_date, 
+0000b160: 2225 592d 256d 2d25 6422 290a 2020 2020  "%Y-%m-%d").    
+0000b170: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000b180: 2020 2020 2020 2020 2020 2020 2020 696d                im
+0000b190: 6d75 6e69 7a61 7469 6f6e 2e65 7870 6972  munization.expir
+0000b1a0: 6174 696f 6e44 6174 6520 3d20 7365 6c66  ationDate = self
+0000b1b0: 2e65 7870 6972 6174 696f 6e5f 6461 7465  .expiration_date
+0000b1c0: 0a0a 2020 2020 6465 6620 6765 745f 7369  ..    def get_si
+0000b1d0: 7465 2873 656c 662c 2069 6d6d 756e 697a  te(self, immuniz
+0000b1e0: 6174 696f 6e3d 4e6f 6e65 2c20 636f 6469  ation=None, codi
+0000b1f0: 6e67 5f73 7973 7465 6d3d 4e6f 6e65 2c20  ng_system=None, 
+0000b200: 636f 6469 6e67 5f76 6572 7369 6f6e 3d4e  coding_version=N
+0000b210: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
+0000b220: 2069 6d6d 756e 697a 6174 696f 6e20 6973   immunization is
+0000b230: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000b240: 2020 2069 6d6d 756e 697a 6174 696f 6e20     immunization 
+0000b250: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
+0000b260: 7572 6365 0a20 2020 2020 2020 2069 6620  urce.        if 
+0000b270: 696d 6d75 6e69 7a61 7469 6f6e 2e73 6974  immunization.sit
+0000b280: 6520 6973 206e 6f74 204e 6f6e 6520 616e  e is not None an
+0000b290: 6420 7479 7065 2869 6d6d 756e 697a 6174  d type(immunizat
+0000b2a0: 696f 6e2e 7369 7465 2920 6973 2043 6f64  ion.site) is Cod
+0000b2b0: 6561 626c 6543 6f6e 6365 7074 3a0a 2020  eableConcept:.  
+0000b2c0: 2020 2020 2020 2020 2020 636f 6469 6e67            coding
+0000b2d0: 203d 2073 656c 662e 6765 745f 636f 6465   = self.get_code
+0000b2e0: 6162 6c65 5f63 6f6e 6365 7074 5f63 6f64  able_concept_cod
+0000b2f0: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+0000b300: 2020 2020 2063 6f64 6561 626c 655f 636f       codeable_co
+0000b310: 6e63 6570 743d 696d 6d75 6e69 7a61 7469  ncept=immunizati
+0000b320: 6f6e 2e73 6974 652c 0a20 2020 2020 2020  on.site,.       
+0000b330: 2020 2020 2020 2020 2063 6f64 696e 675f           coding_
+0000b340: 7379 7374 656d 3d63 6f64 696e 675f 7379  system=coding_sy
+0000b350: 7374 656d 2c0a 2020 2020 2020 2020 2020  stem,.          
+0000b360: 2020 2020 2020 636f 6469 6e67 5f76 6572        coding_ver
+0000b370: 7369 6f6e 3d63 6f64 696e 675f 7665 7273  sion=coding_vers
+0000b380: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
+0000b390: 2072 6574 7572 6e20 636f 6469 6e67 0a20   return coding. 
+0000b3a0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0000b3b0: 6e65 0a0a 2020 2020 6465 6620 7365 745f  ne..    def set_
+0000b3c0: 7369 7465 2873 656c 662c 2069 6d6d 756e  site(self, immun
+0000b3d0: 697a 6174 696f 6e3d 4e6f 6e65 2c20 7369  ization=None, si
+0000b3e0: 7465 5f63 6f64 653d 4e6f 6e65 2c20 7369  te_code=None, si
+0000b3f0: 7465 5f69 643d 4e6f 6e65 2c20 7369 7465  te_id=None, site
+0000b400: 5f64 6973 706c 6179 3d4e 6f6e 652c 2063  _display=None, c
+0000b410: 6f64 696e 675f 7379 7374 656d 3d4e 6f6e  oding_system=Non
+0000b420: 652c 2063 6f64 696e 675f 7665 7273 696f  e, coding_versio
+0000b430: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
+0000b440: 2069 6620 696d 6d75 6e69 7a61 7469 6f6e   if immunization
+0000b450: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000b460: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
+0000b470: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
+0000b480: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
+0000b490: 6966 2073 6974 655f 636f 6465 2069 7320  if site_code is 
+0000b4a0: 6e6f 7420 4e6f 6e65 2061 6e64 2073 6974  not None and sit
+0000b4b0: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+0000b4c0: 2061 6e64 2073 6974 655f 6469 7370 6c61   and site_displa
+0000b4d0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0000b4e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b4f0: 7369 7465 5f63 6f64 6520 3d20 7369 7465  site_code = site
+0000b500: 5f63 6f64 650a 2020 2020 2020 2020 2020  _code.          
+0000b510: 2020 7365 6c66 2e73 6974 655f 6469 7370    self.site_disp
+0000b520: 6c61 7920 3d20 7369 7465 5f64 6973 706c  lay = site_displ
+0000b530: 6179 0a20 2020 2020 2020 2020 2020 2073  ay.            s
+0000b540: 656c 662e 7369 7465 5f69 6420 3d20 7369  elf.site_id = si
+0000b550: 7465 5f69 640a 2020 2020 2020 2020 7369  te_id.        si
+0000b560: 7465 203d 2073 656c 662e 746f 5f63 6f64  te = self.to_cod
+0000b570: 6561 626c 655f 636f 6e63 6570 7428 0a20  eable_concept(. 
+0000b580: 2020 2020 2020 2020 2020 2063 6f64 653d             code=
+0000b590: 7365 6c66 2e73 6974 655f 636f 6465 2c0a  self.site_code,.
+0000b5a0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+0000b5b0: 6c61 793d 7365 6c66 2e73 6974 655f 6469  lay=self.site_di
+0000b5c0: 7370 6c61 792c 0a20 2020 2020 2020 2020  splay,.         
+0000b5d0: 2020 2069 643d 7365 6c66 2e73 6974 655f     id=self.site_
+0000b5e0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0000b5f0: 636f 6469 6e67 5f73 7973 7465 6d3d 636f  coding_system=co
+0000b600: 6469 6e67 5f73 7973 7465 6d2c 0a20 2020  ding_system,.   
+0000b610: 2020 2020 2020 2020 2063 6f64 696e 675f           coding_
+0000b620: 7665 7273 696f 6e3d 636f 6469 6e67 5f76  version=coding_v
+0000b630: 6572 7369 6f6e 0a20 2020 2020 2020 2029  ersion.        )
+0000b640: 0a20 2020 2020 2020 2069 6d6d 756e 697a  .        immuniz
+0000b650: 6174 696f 6e2e 7369 7465 203d 2073 6974  ation.site = sit
+0000b660: 650a 0a20 2020 2064 6566 2067 6574 5f64  e..    def get_d
+0000b670: 6f73 655f 7175 616e 7469 7479 2873 656c  ose_quantity(sel
+0000b680: 662c 2069 6d6d 756e 697a 6174 696f 6e3d  f, immunization=
+0000b690: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
+0000b6a0: 6620 696d 6d75 6e69 7a61 7469 6f6e 2069  f immunization i
+0000b6b0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000b6c0: 2020 2020 696d 6d75 6e69 7a61 7469 6f6e      immunization
+0000b6d0: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
+0000b6e0: 6f75 7263 650a 2020 2020 2020 2020 7265  ource.        re
+0000b6f0: 7475 726e 2069 6d6d 756e 697a 6174 696f  turn immunizatio
+0000b700: 6e2e 646f 7365 5175 616e 7469 7479 0a20  n.doseQuantity. 
+0000b710: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0000b720: 0a20 2020 2064 6566 2073 6574 5f64 6f73  .    def set_dos
+0000b730: 655f 7175 616e 7469 7479 2873 656c 662c  e_quantity(self,
+0000b740: 2069 6d6d 756e 697a 6174 696f 6e3d 4e6f   immunization=No
+0000b750: 6e65 2c20 7175 616e 7469 7479 3d4e 6f6e  ne, quantity=Non
+0000b760: 652c 2071 7561 6e74 6974 795f 636f 6465  e, quantity_code
+0000b770: 3d4e 6f6e 652c 2071 7561 6e74 6974 795f  =None, quantity_
+0000b780: 756e 6974 3d4e 6f6e 652c 2071 7561 6e74  unit=None, quant
+0000b790: 6974 795f 7661 6c75 653d 4e6f 6e65 2c20  ity_value=None, 
+0000b7a0: 7175 616e 7469 7479 5f73 7973 7465 6d3d  quantity_system=
+0000b7b0: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
+0000b7c0: 6620 696d 6d75 6e69 7a61 7469 6f6e 2069  f immunization i
+0000b7d0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000b7e0: 2020 2020 696d 6d75 6e69 7a61 7469 6f6e      immunization
+0000b7f0: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
+0000b800: 6f75 7263 650a 2020 2020 2020 2020 6966  ource.        if
+0000b810: 2071 7561 6e74 6974 795f 7379 7374 656d   quantity_system
+0000b820: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000b830: 2020 2020 2020 7175 616e 7469 7479 5f73        quantity_s
+0000b840: 7973 7465 6d20 3d20 7365 6c66 2e63 6f64  ystem = self.cod
+0000b850: 696e 675f 7379 7374 656d 0a20 2020 2020  ing_system.     
+0000b860: 2020 2069 6620 7175 616e 7469 7479 2069     if quantity i
+0000b870: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000b880: 2020 2020 2020 2020 646f 7365 5f71 7561          dose_qua
+0000b890: 6e74 6974 7920 3d20 7175 616e 7469 7479  ntity = quantity
+0000b8a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000b8b0: 662e 646f 7365 5f71 7561 6e74 6974 795f  f.dose_quantity_
+0000b8c0: 636f 6465 203d 2064 6f73 655f 7175 616e  code = dose_quan
+0000b8d0: 7469 7479 2e63 6f64 650a 2020 2020 2020  tity.code.      
+0000b8e0: 2020 2020 2020 7365 6c66 2e64 6f73 655f        self.dose_
+0000b8f0: 7175 616e 7469 7479 5f75 6e69 7420 3d20  quantity_unit = 
+0000b900: 646f 7365 5f71 7561 6e74 6974 792e 756e  dose_quantity.un
+0000b910: 6974 0a20 2020 2020 2020 2020 2020 2073  it.            s
+0000b920: 656c 662e 646f 7365 5f71 7561 6e74 6974  elf.dose_quantit
+0000b930: 795f 7661 6c75 6520 3d20 646f 7365 5f71  y_value = dose_q
+0000b940: 7561 6e74 6974 792e 7661 6c75 650a 2020  uantity.value.  
+0000b950: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000b960: 2020 2020 2020 2020 6966 2071 7561 6e74          if quant
+0000b970: 6974 795f 756e 6974 2069 7320 6e6f 7420  ity_unit is not 
+0000b980: 4e6f 6e65 2061 6e64 2071 7561 6e74 6974  None and quantit
+0000b990: 795f 7661 6c75 6520 6973 206e 6f74 204e  y_value is not N
+0000b9a0: 6f6e 6520 616e 6420 7175 616e 7469 7479  one and quantity
+0000b9b0: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+0000b9c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000b9d0: 2020 2073 656c 662e 646f 7365 5f71 7561     self.dose_qua
+0000b9e0: 6e74 6974 795f 636f 6465 203d 2071 7561  ntity_code = qua
+0000b9f0: 6e74 6974 795f 636f 6465 0a20 2020 2020  ntity_code.     
+0000ba00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ba10: 646f 7365 5f71 7561 6e74 6974 795f 756e  dose_quantity_un
+0000ba20: 6974 203d 2071 7561 6e74 6974 795f 756e  it = quantity_un
+0000ba30: 6974 0a20 2020 2020 2020 2020 2020 2020  it.             
+0000ba40: 2020 2073 656c 662e 646f 7365 5f71 7561     self.dose_qua
+0000ba50: 6e74 6974 795f 7661 6c75 6520 3d20 7175  ntity_value = qu
+0000ba60: 616e 7469 7479 5f76 616c 7565 0a20 2020  antity_value.   
+0000ba70: 2020 2020 2020 2020 2064 6f73 655f 7175           dose_qu
+0000ba80: 616e 7469 7479 203d 2051 7561 6e74 6974  antity = Quantit
+0000ba90: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
+0000baa0: 646f 7365 5f71 7561 6e74 6974 792e 636f  dose_quantity.co
+0000bab0: 6465 203d 2073 656c 662e 646f 7365 5f71  de = self.dose_q
+0000bac0: 7561 6e74 6974 795f 636f 6465 0a20 2020  uantity_code.   
+0000bad0: 2020 2020 2020 2020 2064 6f73 655f 7175           dose_qu
+0000bae0: 616e 7469 7479 2e73 7973 7465 6d20 3d20  antity.system = 
+0000baf0: 7175 616e 7469 7479 5f73 7973 7465 6d0a  quantity_system.
+0000bb00: 2020 2020 2020 2020 2020 2020 646f 7365              dose
+0000bb10: 5f71 7561 6e74 6974 792e 756e 6974 203d  _quantity.unit =
+0000bb20: 2073 656c 662e 646f 7365 5f71 7561 6e74   self.dose_quant
+0000bb30: 6974 795f 756e 6974 0a20 2020 2020 2020  ity_unit.       
+0000bb40: 2020 2020 2064 6f73 655f 7175 616e 7469       dose_quanti
+0000bb50: 7479 2e76 616c 7565 203d 2073 656c 662e  ty.value = self.
+0000bb60: 646f 7365 5f71 7561 6e74 6974 795f 7661  dose_quantity_va
+0000bb70: 6c75 650a 0a20 2020 2020 2020 2069 6d6d  lue..        imm
+0000bb80: 756e 697a 6174 696f 6e2e 646f 7365 5175  unization.doseQu
+0000bb90: 616e 7469 7479 203d 2064 6f73 655f 7175  antity = dose_qu
+0000bba0: 616e 7469 7479 0a0a 2020 2020 6465 6620  antity..    def 
+0000bbb0: 6765 745f 7265 6173 6f6e 7328 7365 6c66  get_reasons(self
+0000bbc0: 2c20 696d 6d75 6e69 7a61 7469 6f6e 3d4e  , immunization=N
+0000bbd0: 6f6e 652c 2063 6f64 696e 675f 7379 7374  one, coding_syst
+0000bbe0: 656d 3d4e 6f6e 652c 2063 6f64 696e 675f  em=None, coding_
+0000bbf0: 7665 7273 696f 6e3d 4e6f 6e65 293a 0a20  version=None):. 
+0000bc00: 2020 2020 2020 2069 6620 696d 6d75 6e69         if immuni
+0000bc10: 7a61 7469 6f6e 2069 7320 4e6f 6e65 3a0a  zation is None:.
+0000bc20: 2020 2020 2020 2020 2020 2020 696d 6d75              immu
+0000bc30: 6e69 7a61 7469 6f6e 2020 3d20 7365 6c66  nization  = self
+0000bc40: 2e66 6869 725f 7265 736f 7572 6365 0a20  .fhir_resource. 
+0000bc50: 2020 2020 2020 2069 6620 696d 6d75 6e69         if immuni
+0000bc60: 7a61 7469 6f6e 2e65 7870 6c61 6e61 7469  zation.explanati
+0000bc70: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 2061  on is not None a
+0000bc80: 6e64 2069 6d6d 756e 697a 6174 696f 6e2e  nd immunization.
+0000bc90: 6578 706c 616e 6174 696f 6e2e 7265 6173  explanation.reas
+0000bca0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
+0000bcb0: 2020 2020 2020 2020 2020 2020 7265 6173              reas
+0000bcc0: 6f6e 7320 3d20 5b5d 0a20 2020 2020 2020  ons = [].       
+0000bcd0: 2020 2020 2066 6f72 2072 6561 736f 6e20       for reason 
+0000bce0: 696e 2069 6d6d 756e 697a 6174 696f 6e2e  in immunization.
+0000bcf0: 6578 706c 616e 6174 696f 6e2e 7265 6173  explanation.reas
+0000bd00: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+0000bd10: 2020 2020 6966 2074 7970 6528 7265 6173      if type(reas
+0000bd20: 6f6e 2920 6973 2043 6f64 6561 626c 6543  on) is CodeableC
+0000bd30: 6f6e 6365 7074 3a0a 2020 2020 2020 2020  oncept:.        
+0000bd40: 2020 2020 2020 2020 2020 2020 7265 6173              reas
+0000bd50: 6f6e 5f63 6f64 696e 6720 3d20 7365 6c66  on_coding = self
+0000bd60: 2e67 6574 5f63 6f64 6561 626c 655f 636f  .get_codeable_co
+0000bd70: 6e63 6570 745f 636f 6469 6e67 280a 2020  ncept_coding(.  
+0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd90: 2020 2020 2020 636f 6465 6162 6c65 5f63        codeable_c
+0000bda0: 6f6e 6365 7074 3d72 6561 736f 6e2c 0a20  oncept=reason,. 
+0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdc0: 2020 2020 2020 2063 6f64 696e 675f 7379         coding_sy
+0000bdd0: 7374 656d 3d63 6f64 696e 675f 7379 7374  stem=coding_syst
+0000bde0: 656d 2c0a 2020 2020 2020 2020 2020 2020  em,.            
+0000bdf0: 2020 2020 2020 2020 2020 2020 636f 6469              codi
+0000be00: 6e67 5f76 6572 7369 6f6e 3d63 6f64 696e  ng_version=codin
+0000be10: 675f 7665 7273 696f 6e29 0a20 2020 2020  g_version).     
+0000be20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000be30: 6561 736f 6e73 2e61 7070 656e 6428 7265  easons.append(re
+0000be40: 6173 6f6e 5f63 6f64 696e 672e 6173 5f6a  ason_coding.as_j
+0000be50: 736f 6e28 2929 0a20 2020 2020 2020 2020  son()).         
+0000be60: 2020 2020 2020 2065 6c69 6620 7479 7065         elif type
+0000be70: 2872 6561 736f 6e29 2069 7320 436f 6469  (reason) is Codi
+0000be80: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+0000be90: 2020 2020 2020 2020 7265 6173 6f6e 732e          reasons.
+0000bea0: 6170 7065 6e64 2872 6561 736f 6e2e 6173  append(reason.as
+0000beb0: 5f6a 736f 6e28 2929 0a20 2020 2020 2020  _json()).       
+0000bec0: 2020 2020 2072 6574 7572 6e20 7265 6173       return reas
+0000bed0: 6f6e 730a 0a20 2020 2064 6566 2073 6574  ons..    def set
+0000bee0: 5f72 6561 736f 6e28 7365 6c66 2c20 696d  _reason(self, im
+0000bef0: 6d75 6e69 7a61 7469 6f6e 3d4e 6f6e 652c  munization=None,
+0000bf00: 2072 6561 736f 6e73 3d4e 6f6e 652c 2063   reasons=None, c
+0000bf10: 6f64 696e 675f 7379 7374 656d 3d4e 6f6e  oding_system=Non
+0000bf20: 652c 2063 6f64 696e 675f 7665 7273 696f  e, coding_versio
+0000bf30: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
+0000bf40: 2069 6620 696d 6d75 6e69 7a61 7469 6f6e   if immunization
+0000bf50: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000bf60: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
+0000bf70: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
+0000bf80: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
+0000bf90: 636f 6469 6e67 5f73 7973 7465 6d20 3d20  coding_system = 
+0000bfa0: 636f 6469 6e67 5f73 7973 7465 6d20 6966  coding_system if
+0000bfb0: 2063 6f64 696e 675f 7379 7374 656d 2069   coding_system i
+0000bfc0: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+0000bfd0: 7365 6c66 2e63 6f64 696e 675f 7379 7374  self.coding_syst
+0000bfe0: 656d 0a20 2020 2020 2020 2063 6f64 696e  em.        codin
+0000bff0: 675f 7665 7273 696f 6e20 3d20 636f 6469  g_version = codi
+0000c000: 6e67 5f76 6572 7369 6f6e 2069 6620 636f  ng_version if co
+0000c010: 6469 6e67 5f76 6572 7369 6f6e 2069 7320  ding_version is 
+0000c020: 6e6f 7420 4e6f 6e65 2065 6c73 6520 7365  not None else se
+0000c030: 6c66 2e63 6f64 696e 675f 7665 7273 696f  lf.coding_versio
+0000c040: 6e0a 2020 2020 2020 2020 6966 2072 6561  n.        if rea
+0000c050: 736f 6e73 2069 7320 6e6f 7420 4e6f 6e65  sons is not None
+0000c060: 2061 6e64 206c 656e 2872 6561 736f 6e73   and len(reasons
+0000c070: 2920 3e20 303a 0a20 2020 2020 2020 2020  ) > 0:.         
+0000c080: 2020 2073 656c 662e 7265 6173 6f6e 203d     self.reason =
+0000c090: 2072 6561 736f 6e73 0a0a 2020 2020 2020   reasons..      
+0000c0a0: 2020 6966 2073 656c 662e 7265 6173 6f6e    if self.reason
+0000c0b0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0000c0c0: 206c 656e 2873 656c 662e 7265 6173 6f6e   len(self.reason
+0000c0d0: 2920 3e20 303a 0a20 2020 2020 2020 2020  ) > 0:.         
+0000c0e0: 2020 2069 6d6d 5f65 7870 6c61 6e61 7469     imm_explanati
+0000c0f0: 6f6e 203d 2049 6d6d 756e 697a 6174 696f  on = Immunizatio
+0000c100: 6e45 7870 6c61 6e61 7469 6f6e 2829 0a20  nExplanation(). 
+0000c110: 2020 2020 2020 2020 2020 2069 6d6d 5f65             imm_e
+0000c120: 7870 6c61 6e61 7469 6f6e 2e72 6561 736f  xplanation.reaso
+0000c130: 6e20 3d20 5b5d 0a20 2020 2020 2020 2020  n = [].         
+0000c140: 2020 2066 6f72 2072 6561 736f 6e20 696e     for reason in
+0000c150: 2073 656c 662e 7265 6173 6f6e 3a0a 2020   self.reason:.  
+0000c160: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000c170: 6173 6f6e 5f63 6f64 696e 6720 3d20 436f  ason_coding = Co
+0000c180: 6469 6e67 286a 736f 6e64 6963 743d 7265  ding(jsondict=re
+0000c190: 6173 6f6e 290a 2020 2020 2020 2020 2020  ason).          
+0000c1a0: 2020 2020 2020 7265 6173 6f6e 5f63 6f64        reason_cod
+0000c1b0: 696e 672e 7665 7273 696f 6e20 3d20 636f  ing.version = co
+0000c1c0: 6469 6e67 5f76 6572 7369 6f6e 0a20 2020  ding_version.   
+0000c1d0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+0000c1e0: 736f 6e5f 636f 6469 6e67 2e73 7973 7465  son_coding.syste
+0000c1f0: 6d20 3d20 636f 6469 6e67 5f73 7973 7465  m = coding_syste
+0000c200: 6d20 0a20 2020 2020 2020 2020 2020 2020  m .             
+0000c210: 2020 2069 6d6d 5f65 7870 6c61 6e61 7469     imm_explanati
+0000c220: 6f6e 2e72 6561 736f 6e2e 6170 7065 6e64  on.reason.append
+0000c230: 2872 6561 736f 6e5f 636f 6469 6e67 290a  (reason_coding).
+0000c240: 2020 2020 2020 2020 2020 2020 696d 6d75              immu
+0000c250: 6e69 7a61 7469 6f6e 2e65 7870 6c61 6e61  nization.explana
+0000c260: 7469 6f6e 203d 2069 6d6d 5f65 7870 6c61  tion = imm_expla
+0000c270: 6e61 7469 6f6e 0a0a 2020 2020 6465 6620  nation..    def 
+0000c280: 6765 745f 6461 7465 2873 656c 662c 2069  get_date(self, i
+0000c290: 6d6d 756e 697a 6174 696f 6e3d 4e6f 6e65  mmunization=None
+0000c2a0: 293a 0a20 2020 2020 2020 2069 6620 696d  ):.        if im
+0000c2b0: 6d75 6e69 7a61 7469 6f6e 2069 7320 4e6f  munization is No
+0000c2c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000c2d0: 696d 6d75 6e69 7a61 7469 6f6e 203d 2073  immunization = s
+0000c2e0: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+0000c2f0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+0000c300: 2069 6d6d 756e 697a 6174 696f 6e2e 6461   immunization.da
+0000c310: 7465 0a0a 2020 2020 6465 6620 7365 745f  te..    def set_
+0000c320: 6461 7465 2873 656c 662c 2069 6d6d 756e  date(self, immun
+0000c330: 697a 6174 696f 6e3d 4e6f 6e65 2c20 6461  ization=None, da
+0000c340: 7465 5f74 6f5f 7365 743d 4e6f 6e65 293a  te_to_set=None):
+0000c350: 0a20 2020 2020 2020 2069 6620 696d 6d75  .        if immu
+0000c360: 6e69 7a61 7469 6f6e 2069 7320 4e6f 6e65  nization is None
+0000c370: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
+0000c380: 6d75 6e69 7a61 7469 6f6e 203d 2073 656c  munization = sel
+0000c390: 662e 6668 6972 5f72 6573 6f75 7263 650a  f.fhir_resource.
+0000c3a0: 2020 2020 2020 2020 6966 2064 6174 655f          if date_
+0000c3b0: 746f 5f73 6574 2069 7320 6e6f 7420 4e6f  to_set is not No
+0000c3c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000c3d0: 6966 2074 7970 6528 6461 7465 5f74 6f5f  if type(date_to_
+0000c3e0: 7365 7429 2069 7320 7374 723a 0a20 2020  set) is str:.   
+0000c3f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c400: 662e 6461 7465 203d 2064 6174 655f 746f  f.date = date_to
+0000c410: 5f73 6574 0a20 2020 2020 2020 2020 2020  _set.           
+0000c420: 2065 6c69 6620 7479 7065 2864 6174 655f   elif type(date_
+0000c430: 746f 5f73 6574 2920 6973 2064 6174 6520  to_set) is date 
+0000c440: 6f72 2074 7970 6528 6461 7465 5f74 6f5f  or type(date_to_
+0000c450: 7365 7429 2069 7320 6461 7465 7469 6d65  set) is datetime
+0000c460: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c470: 2020 7365 6c66 2e64 6174 6520 3d20 6461    self.date = da
+0000c480: 7465 7469 6d65 2e73 7472 6674 696d 6528  tetime.strftime(
+0000c490: 6461 7465 5f74 6f5f 7365 742c 2022 2559  date_to_set, "%Y
+0000c4a0: 2d25 6d2d 2564 5425 483a 254d 3a25 5322  -%m-%dT%H:%M:%S"
+0000c4b0: 290a 2020 2020 2020 2020 6966 2074 7970  ).        if typ
+0000c4c0: 6528 7365 6c66 2e64 6174 6529 2069 7320  e(self.date) is 
+0000c4d0: 6461 7465 206f 7220 7479 7065 2873 656c  date or type(sel
+0000c4e0: 662e 6461 7465 2920 6973 2064 6174 6574  f.date) is datet
+0000c4f0: 696d 653a 0a20 2020 2020 2020 2020 2020  ime:.           
+0000c500: 2073 656c 662e 6461 7465 203d 2064 6174   self.date = dat
+0000c510: 6574 696d 652e 7374 7266 7469 6d65 2873  etime.strftime(s
+0000c520: 656c 662e 6461 7465 2c22 2559 2d25 6d2d  elf.date,"%Y-%m-
+0000c530: 2564 5425 483a 254d 3a25 5322 290a 2020  %dT%H:%M:%S").  
+0000c540: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
+0000c550: 6f6e 2e64 6174 6520 3d20 4648 4952 4461  on.date = FHIRDa
+0000c560: 7465 286a 736f 6e76 616c 3d73 656c 662e  te(jsonval=self.
+0000c570: 6461 7465 2920 6966 2073 656c 662e 6461  date) if self.da
+0000c580: 7465 2069 7320 6e6f 7420 4e6f 6e65 2065  te is not None e
+0000c590: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
+0000c5a0: 200a 0a20 2020 2064 6566 2067 6574 5f73   ..    def get_s
+0000c5b0: 7461 7475 7328 7365 6c66 2c20 696d 6d75  tatus(self, immu
+0000c5c0: 6e69 7a61 7469 6f6e 3d4e 6f6e 6529 3a0a  nization=None):.
+0000c5d0: 2020 2020 2020 2020 6966 2069 6d6d 756e          if immun
+0000c5e0: 697a 6174 696f 6e20 6973 204e 6f6e 653a  ization is None:
+0000c5f0: 0a20 2020 2020 2020 2020 2020 2069 6d6d  .            imm
+0000c600: 756e 697a 6174 696f 6e20 3d20 7365 6c66  unization = self
+0000c610: 2e66 6869 725f 7265 736f 7572 6365 0a20  .fhir_resource. 
+0000c620: 2020 2020 2020 2072 6574 7572 6e20 696d         return im
+0000c630: 6d75 6e69 7a61 7469 6f6e 2e73 7461 7475  munization.statu
+0000c640: 730a 0a20 2020 2064 6566 2073 6574 5f73  s..    def set_s
+0000c650: 7461 7475 7328 7365 6c66 2c20 696d 6d75  tatus(self, immu
+0000c660: 6e69 7a61 7469 6f6e 3d4e 6f6e 652c 2073  nization=None, s
+0000c670: 7461 7475 733d 4e6f 6e65 293a 0a20 2020  tatus=None):.   
+0000c680: 2020 2020 2069 6620 696d 6d75 6e69 7a61       if immuniza
+0000c690: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
+0000c6a0: 2020 2020 2020 2020 2020 696d 6d75 6e69            immuni
+0000c6b0: 7a61 7469 6f6e 203d 2073 656c 662e 6668  zation = self.fh
+0000c6c0: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
+0000c6d0: 2020 2020 6966 2073 7461 7475 7320 6973      if status is
+0000c6e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000c6f0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0000c700: 7573 203d 2073 7461 7475 730a 2020 2020  us = status.    
+0000c710: 2020 2020 696d 6d75 6e69 7a61 7469 6f6e      immunization
+0000c720: 2e73 7461 7475 7320 3d20 7365 6c66 2e73  .status = self.s
+0000c730: 7461 7475 730a 0a20 2020 2064 6566 2074  tatus..    def t
+0000c740: 6f5f 6668 6972 5f72 6573 6f75 7263 6528  o_fhir_resource(
+0000c750: 7365 6c66 2c20 696d 6d75 6e69 7a61 7469  self, immunizati
+0000c760: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
+0000c770: 2020 6966 2069 6d6d 756e 697a 6174 696f    if immunizatio
+0000c780: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+0000c790: 2020 2020 2020 2069 6d6d 756e 697a 6174         immunizat
+0000c7a0: 696f 6e20 3d20 496d 6d75 6e69 7a61 7469  ion = Immunizati
+0000c7b0: 6f6e 2829 0a20 2020 2020 2020 2073 656c  on().        sel
+0000c7c0: 662e 7365 745f 6964 2869 6d6d 756e 697a  f.set_id(immuniz
+0000c7d0: 6174 696f 6e3d 696d 6d75 6e69 7a61 7469  ation=immunizati
+0000c7e0: 6f6e 290a 2020 2020 2020 2020 7365 6c66  on).        self
+0000c7f0: 2e73 6574 5f6d 6574 6128 696d 6d75 6e69  .set_meta(immuni
+0000c800: 7a61 7469 6f6e 3d69 6d6d 756e 697a 6174  zation=immunizat
+0000c810: 696f 6e29 0a20 2020 2020 2020 2073 656c  ion).        sel
+0000c820: 662e 7365 745f 636f 6e74 6169 6e65 645f  f.set_contained_
+0000c830: 6f72 6761 6e69 7a61 7469 6f6e 2869 6d6d  organization(imm
+0000c840: 756e 697a 6174 696f 6e3d 696d 6d75 6e69  unization=immuni
+0000c850: 7a61 7469 6f6e 290a 2020 2020 2020 2020  zation).        
+0000c860: 7365 6c66 2e73 6574 5f6f 7665 7272 6964  self.set_overrid
+0000c870: 655f 7374 6174 7573 2869 6d6d 756e 697a  e_status(immuniz
+0000c880: 6174 696f 6e3d 696d 6d75 6e69 7a61 7469  ation=immunizati
+0000c890: 6f6e 290a 2020 2020 2020 2020 7365 6c66  on).        self
+0000c8a0: 2e73 6574 5f6c 6f74 5f69 6428 696d 6d75  .set_lot_id(immu
+0000c8b0: 6e69 7a61 7469 6f6e 3d69 6d6d 756e 697a  nization=immuniz
+0000c8c0: 6174 696f 6e29 0a20 2020 2020 2020 2073  ation).        s
+0000c8d0: 656c 662e 7365 745f 616e 7469 6765 6e5f  elf.set_antigen_
+0000c8e0: 7374 6174 7573 2869 6d6d 756e 697a 6174  status(immunizat
+0000c8f0: 696f 6e3d 696d 6d75 6e69 7a61 7469 6f6e  ion=immunization
+0000c900: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000c910: 6574 5f74 7261 6465 5f6e 616d 6528 696d  et_trade_name(im
+0000c920: 6d75 6e69 7a61 7469 6f6e 3d69 6d6d 756e  munization=immun
+0000c930: 697a 6174 696f 6e29 0a20 2020 2020 2020  ization).       
+0000c940: 2073 656c 662e 7365 745f 7661 6363 696e   self.set_vaccin
+0000c950: 655f 636f 6465 2869 6d6d 756e 697a 6174  e_code(immunizat
+0000c960: 696f 6e3d 696d 6d75 6e69 7a61 7469 6f6e  ion=immunization
+0000c970: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000c980: 6574 5f70 6174 6965 6e74 2869 6d6d 756e  et_patient(immun
+0000c990: 697a 6174 696f 6e3d 696d 6d75 6e69 7a61  ization=immuniza
+0000c9a0: 7469 6f6e 290a 2020 2020 2020 2020 7365  tion).        se
+0000c9b0: 6c66 2e73 6574 5f70 6572 666f 726d 6572  lf.set_performer
+0000c9c0: 2869 6d6d 756e 697a 6174 696f 6e3d 696d  (immunization=im
+0000c9d0: 6d75 6e69 7a61 7469 6f6e 290a 2020 2020  munization).    
+0000c9e0: 2020 2020 7365 6c66 2e73 6574 5f6c 6f63      self.set_loc
+0000c9f0: 6174 696f 6e28 696d 6d75 6e69 7a61 7469  ation(immunizati
+0000ca00: 6f6e 3d69 6d6d 756e 697a 6174 696f 6e29  on=immunization)
+0000ca10: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000ca20: 745f 6c6f 745f 6e75 6d62 6572 2869 6d6d  t_lot_number(imm
+0000ca30: 756e 697a 6174 696f 6e3d 696d 6d75 6e69  unization=immuni
+0000ca40: 7a61 7469 6f6e 290a 2020 2020 2020 2020  zation).        
+0000ca50: 7365 6c66 2e73 6574 5f65 7870 6972 6174  self.set_expirat
+0000ca60: 696f 6e5f 6461 7465 2869 6d6d 756e 697a  ion_date(immuniz
+0000ca70: 6174 696f 6e3d 696d 6d75 6e69 7a61 7469  ation=immunizati
+0000ca80: 6f6e 290a 2020 2020 2020 2020 7365 6c66  on).        self
+0000ca90: 2e73 6574 5f73 6974 6528 696d 6d75 6e69  .set_site(immuni
+0000caa0: 7a61 7469 6f6e 3d69 6d6d 756e 697a 6174  zation=immunizat
+0000cab0: 696f 6e29 0a20 2020 2020 2020 2073 656c  ion).        sel
+0000cac0: 662e 7365 745f 646f 7365 5f71 7561 6e74  f.set_dose_quant
+0000cad0: 6974 7928 696d 6d75 6e69 7a61 7469 6f6e  ity(immunization
+0000cae0: 3d69 6d6d 756e 697a 6174 696f 6e29 0a20  =immunization). 
+0000caf0: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+0000cb00: 7265 6173 6f6e 2869 6d6d 756e 697a 6174  reason(immunizat
+0000cb10: 696f 6e3d 696d 6d75 6e69 7a61 7469 6f6e  ion=immunization
+0000cb20: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000cb30: 6574 5f64 6174 6528 696d 6d75 6e69 7a61  et_date(immuniza
+0000cb40: 7469 6f6e 3d69 6d6d 756e 697a 6174 696f  tion=immunizatio
+0000cb50: 6e29 0a20 2020 2020 2020 2073 656c 662e  n).        self.
+0000cb60: 7365 745f 7374 6174 7573 2869 6d6d 756e  set_status(immun
+0000cb70: 697a 6174 696f 6e3d 696d 6d75 6e69 7a61  ization=immuniza
+0000cb80: 7469 6f6e 290a 2020 2020 2020 2020 7265  tion).        re
+0000cb90: 7475 726e 2069 6d6d 756e 697a 6174 696f  turn immunizatio
+0000cba0: 6e0a 0a20 2020 2064 6566 2067 6574 4668  n..    def getFh
+0000cbb0: 6972 5265 736f 7572 6365 2873 656c 6629  irResource(self)
+0000cbc0: 3a0a 2020 2020 2020 2020 7365 6c66 2e66  :.        self.f
+0000cbd0: 6869 725f 7265 736f 7572 6365 203d 2073  hir_resource = s
+0000cbe0: 656c 662e 746f 5f66 6869 725f 7265 736f  elf.to_fhir_reso
+0000cbf0: 7572 6365 2829 0a20 2020 2020 2020 2072  urce().        r
+0000cc00: 6573 6f75 7263 6520 3d20 7365 6c66 2e66  esource = self.f
+0000cc10: 6869 725f 7265 736f 7572 6365 2e61 735f  hir_resource.as_
+0000cc20: 6a73 6f6e 2829 0a20 2020 2020 2020 2072  json().        r
+0000cc30: 6574 7572 6e20 7265 736f 7572 6365 0a20  eturn resource. 
+0000cc40: 2020 2020 2020 200a 2020 2020 6465 6620         .    def 
+0000cc50: 6672 6f6d 5f64 6963 7428 7365 6c66 2c20  from_dict(self, 
+0000cc60: 696d 6d5f 6469 6374 3d4e 6f6e 6529 3a0a  imm_dict=None):.
+0000cc70: 2020 2020 2020 2020 6966 2069 6d6d 5f64          if imm_d
+0000cc80: 6963 7420 6973 204e 6f6e 653a 0a20 2020  ict is None:.   
+0000cc90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000cca0: 4e6f 6e65 0a20 2020 2020 2020 2069 6d6d  None.        imm
+0000ccb0: 5f72 6573 6f75 7263 6520 3d20 496d 6d75  _resource = Immu
+0000ccc0: 6e69 7a61 7469 6f6e 286a 736f 6e64 6963  nization(jsondic
+0000ccd0: 743d 696d 6d5f 6469 6374 290a 2020 2020  t=imm_dict).    
+0000cce0: 2020 2020 7365 6c66 2e66 726f 6d5f 6668      self.from_fh
+0000ccf0: 6972 5f72 6573 6f75 7263 6528 696d 6d75  ir_resource(immu
+0000cd00: 6e69 7a61 7469 6f6e 3d69 6d6d 5f72 6573  nization=imm_res
+0000cd10: 6f75 7263 6529 0a0a 2020 2020 6465 6620  ource)..    def 
+0000cd20: 6672 6f6d 5f66 6869 725f 7265 736f 7572  from_fhir_resour
+0000cd30: 6365 2873 656c 662c 2069 6d6d 756e 697a  ce(self, immuniz
+0000cd40: 6174 696f 6e3d 4e6f 6e65 2c20 636f 6469  ation=None, codi
+0000cd50: 6e67 5f73 7973 7465 6d3d 4e6f 6e65 2c20  ng_system=None, 
+0000cd60: 636f 6469 6e67 5f76 6572 7369 6f6e 3d4e  coding_version=N
+0000cd70: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
+0000cd80: 2069 6d6d 756e 697a 6174 696f 6e20 6973   immunization is
+0000cd90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000cda0: 2020 2069 6d6d 756e 697a 6174 696f 6e20     immunization 
+0000cdb0: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
+0000cdc0: 7572 6365 0a0a 2020 2020 2020 2020 7365  urce..        se
+0000cdd0: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+0000cde0: 203d 2069 6d6d 756e 697a 6174 696f 6e0a   = immunization.
+0000cdf0: 2020 2020 2020 2020 7365 6c66 2e69 6420          self.id 
+0000ce00: 3d20 7365 6c66 2e67 6574 5f69 6428 290a  = self.get_id().
+0000ce10: 2020 2020 2020 2020 616e 7469 6765 6e20          antigen 
+0000ce20: 3d20 7365 6c66 2e67 6574 5f61 6e74 6967  = self.get_antig
+0000ce30: 656e 5f73 7461 7475 735f 616e 7469 6765  en_status_antige
+0000ce40: 6e28 290a 2020 2020 2020 2020 616e 7469  n().        anti
+0000ce50: 6765 6e5f 636f 6469 6e67 203d 2073 656c  gen_coding = sel
+0000ce60: 662e 6765 745f 636f 6465 6162 6c65 5f63  f.get_codeable_c
+0000ce70: 6f6e 6365 7074 5f63 6f64 696e 6728 0a20  oncept_coding(. 
+0000ce80: 2020 2020 2020 2020 2020 2063 6f64 6561             codea
+0000ce90: 626c 655f 636f 6e63 6570 743d 616e 7469  ble_concept=anti
+0000cea0: 6765 6e2e 7661 6c75 6543 6f64 6561 626c  gen.valueCodeabl
+0000ceb0: 6543 6f6e 6365 7074 2c0a 2020 2020 2020  eConcept,.      
+0000cec0: 2020 2020 2020 636f 6469 6e67 5f73 7973        coding_sys
+0000ced0: 7465 6d3d 636f 6469 6e67 5f73 7973 7465  tem=coding_syste
+0000cee0: 6d2c 0a20 2020 2020 2020 2020 2020 2063  m,.            c
+0000cef0: 6f64 696e 675f 7665 7273 696f 6e3d 636f  oding_version=co
+0000cf00: 6469 6e67 5f76 6572 7369 6f6e 290a 2020  ding_version).  
+0000cf10: 2020 2020 2020 7365 6c66 2e61 6e74 6967        self.antig
+0000cf20: 656e 5f63 6f64 6520 3d20 616e 7469 6765  en_code = antige
+0000cf30: 6e5f 636f 6469 6e67 2e63 6f64 650a 2020  n_coding.code.  
+0000cf40: 2020 2020 2020 7365 6c66 2e61 6e74 6967        self.antig
+0000cf50: 656e 5f64 6973 706c 6179 203d 2061 6e74  en_display = ant
+0000cf60: 6967 656e 5f63 6f64 696e 672e 6469 7370  igen_coding.disp
+0000cf70: 6c61 790a 2020 2020 2020 2020 7365 6c66  lay.        self
+0000cf80: 2e61 6e74 6967 656e 5f69 6420 3d20 616e  .antigen_id = an
+0000cf90: 7469 6765 6e5f 636f 6469 6e67 2e69 640a  tigen_coding.id.
+0000cfa0: 2020 2020 2020 2020 646f 7365 5f6e 756d          dose_num
+0000cfb0: 6265 7220 3d20 7365 6c66 2e67 6574 5f61  ber = self.get_a
+0000cfc0: 6e74 6967 656e 5f73 7461 7475 735f 646f  ntigen_status_do
+0000cfd0: 7365 5f6e 756d 6265 7228 290a 2020 2020  se_number().    
+0000cfe0: 2020 2020 7365 6c66 2e61 6e74 6967 656e      self.antigen
+0000cff0: 5f64 6f73 655f 6e75 6d62 6572 203d 2064  _dose_number = d
+0000d000: 6f73 655f 6e75 6d62 6572 2e76 616c 7565  ose_number.value
+0000d010: 496e 7465 6765 720a 2020 2020 2020 2020  Integer.        
+0000d020: 616e 7469 6765 6e5f 7374 6174 7573 203d  antigen_status =
+0000d030: 2073 656c 662e 6765 745f 616e 7469 6765   self.get_antige
+0000d040: 6e5f 7374 6174 7573 5f73 7461 7475 7328  n_status_status(
+0000d050: 290a 2020 2020 2020 2020 616e 7469 6765  ).        antige
+0000d060: 6e5f 7374 6174 7573 5f63 6f64 6520 3d20  n_status_code = 
+0000d070: 7365 6c66 2e67 6574 5f63 6f64 6561 626c  self.get_codeabl
+0000d080: 655f 636f 6e63 6570 745f 636f 6469 6e67  e_concept_coding
+0000d090: 280a 2020 2020 2020 2020 2020 2020 636f  (.            co
+0000d0a0: 6465 6162 6c65 5f63 6f6e 6365 7074 3d61  deable_concept=a
+0000d0b0: 6e74 6967 656e 5f73 7461 7475 732e 7661  ntigen_status.va
+0000d0c0: 6c75 6543 6f64 6561 626c 6543 6f6e 6365  lueCodeableConce
+0000d0d0: 7074 2c0a 2020 2020 2020 2020 2020 2020  pt,.            
+0000d0e0: 636f 6469 6e67 5f73 7973 7465 6d3d 636f  coding_system=co
+0000d0f0: 6469 6e67 5f73 7973 7465 6d2c 0a20 2020  ding_system,.   
+0000d100: 2020 2020 2020 2020 2063 6f64 696e 675f           coding_
+0000d110: 7665 7273 696f 6e3d 636f 6469 6e67 5f76  version=coding_v
+0000d120: 6572 7369 6f6e 290a 2020 2020 2020 2020  ersion).        
+0000d130: 7365 6c66 2e61 6e74 6967 656e 5f73 7461  self.antigen_sta
+0000d140: 7475 735f 636f 6465 203d 2061 6e74 6967  tus_code = antig
+0000d150: 656e 5f73 7461 7475 735f 636f 6465 2e63  en_status_code.c
+0000d160: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
+0000d170: 2e61 6e74 6967 656e 5f73 7461 7475 735f  .antigen_status_
+0000d180: 6469 7370 6c61 7920 3d20 616e 7469 6765  display = antige
+0000d190: 6e5f 7374 6174 7573 5f63 6f64 652e 6469  n_status_code.di
+0000d1a0: 7370 6c61 790a 2020 2020 2020 2020 7365  splay.        se
+0000d1b0: 6c66 2e61 6e74 6967 656e 5f73 7461 7475  lf.antigen_statu
+0000d1c0: 735f 6964 203d 2061 6e74 6967 656e 5f73  s_id = antigen_s
+0000d1d0: 7461 7475 735f 636f 6465 2e69 640a 2020  tatus_code.id.  
+0000d1e0: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
+0000d1f0: 6564 5f62 7920 3d20 7365 6c66 2e67 6574  ed_by = self.get
+0000d200: 5f6d 6574 615f 7570 6461 7465 645f 6279  _meta_updated_by
+0000d210: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000d220: 6372 6561 7465 645f 6279 203d 2073 656c  created_by = sel
+0000d230: 662e 6765 745f 6d65 7461 5f63 7265 6174  f.get_meta_creat
+0000d240: 6564 5f62 7928 290a 2020 2020 2020 2020  ed_by().        
+0000d250: 7365 6c66 2e63 7265 6174 696f 6e5f 6461  self.creation_da
+0000d260: 7465 203d 2073 656c 662e 6765 745f 6d65  te = self.get_me
+0000d270: 7461 5f63 7265 6174 696f 6e5f 6461 7465  ta_creation_date
+0000d280: 2829 2e69 736f 7374 7269 6e67 0a20 2020  ().isostring.   
+0000d290: 2020 2020 2073 656c 662e 7665 7273 696f       self.versio
+0000d2a0: 6e5f 6964 203d 2073 656c 662e 6765 745f  n_id = self.get_
+0000d2b0: 6d65 7461 5f76 6572 7369 6f6e 5f69 6428  meta_version_id(
+0000d2c0: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+0000d2d0: 6173 745f 7570 6461 7465 6420 3d20 7365  ast_updated = se
+0000d2e0: 6c66 2e67 6574 5f6d 6574 615f 6c61 7374  lf.get_meta_last
+0000d2f0: 5f75 7064 6174 6564 2829 0a20 2020 2020  _updated().     
+0000d300: 2020 2073 656c 662e 7072 6f66 696c 6520     self.profile 
+0000d310: 3d20 7365 6c66 2e67 6574 5f6d 6574 615f  = self.get_meta_
+0000d320: 7072 6f66 696c 6528 290a 2020 2020 2020  profile().      
+0000d330: 2020 7365 6c66 2e6f 7267 616e 697a 6174    self.organizat
+0000d340: 696f 6e20 3d20 7365 6c66 2e67 6574 5f63  ion = self.get_c
+0000d350: 6f6e 7461 696e 6564 5f6f 7267 616e 697a  ontained_organiz
+0000d360: 6174 696f 6e28 290a 2020 2020 2020 2020  ation().        
+0000d370: 6f76 6572 7269 6465 5f73 7461 7475 735f  override_status_
+0000d380: 6578 7465 6e73 696f 6e20 3d20 7365 6c66  extension = self
+0000d390: 2e67 6574 5f6f 7665 7272 6964 655f 7374  .get_override_st
+0000d3a0: 6174 7573 2829 0a20 2020 2020 2020 2069  atus().        i
+0000d3b0: 6620 6f76 6572 7269 6465 5f73 7461 7475  f override_statu
+0000d3c0: 735f 6578 7465 6e73 696f 6e20 6973 206e  s_extension is n
+0000d3d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000d3e0: 2020 2020 206f 7665 7272 6964 655f 7374       override_st
+0000d3f0: 6174 7573 5f63 6f64 696e 6720 3d20 7365  atus_coding = se
+0000d400: 6c66 2e67 6574 5f63 6f64 6561 626c 655f  lf.get_codeable_
+0000d410: 636f 6e63 6570 745f 636f 6469 6e67 280a  concept_coding(.
+0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d430: 636f 6465 6162 6c65 5f63 6f6e 6365 7074  codeable_concept
+0000d440: 3d6f 7665 7272 6964 655f 7374 6174 7573  =override_status
+0000d450: 5f65 7874 656e 7369 6f6e 2e76 616c 7565  _extension.value
+0000d460: 436f 6465 6162 6c65 436f 6e63 6570 742c  CodeableConcept,
+0000d470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d480: 2063 6f64 696e 675f 7379 7374 656d 3d63   coding_system=c
+0000d490: 6f64 696e 675f 7379 7374 656d 2c0a 2020  oding_system,.  
+0000d4a0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000d4b0: 6469 6e67 5f76 6572 7369 6f6e 3d63 6f64  ding_version=cod
+0000d4c0: 696e 675f 7665 7273 696f 6e29 0a20 2020  ing_version).   
+0000d4d0: 2020 2020 2020 2020 2073 656c 662e 6f76           self.ov
+0000d4e0: 6572 7269 6465 5f73 7461 7475 735f 636f  erride_status_co
+0000d4f0: 6465 203d 206f 7665 7272 6964 655f 7374  de = override_st
+0000d500: 6174 7573 5f63 6f64 696e 672e 636f 6465  atus_coding.code
+0000d510: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d520: 662e 6f76 6572 7269 6465 5f73 7461 7475  f.override_statu
+0000d530: 735f 6469 7370 6c61 7920 3d20 6f76 6572  s_display = over
+0000d540: 7269 6465 5f73 7461 7475 735f 636f 6469  ride_status_codi
+0000d550: 6e67 2e64 6973 706c 6179 0a20 2020 2020  ng.display.     
+0000d560: 2020 2020 2020 2073 656c 662e 6f76 6572         self.over
+0000d570: 7269 6465 5f73 7461 7475 735f 6964 203d  ride_status_id =
+0000d580: 206f 7665 7272 6964 655f 7374 6174 7573   override_status
+0000d590: 5f63 6f64 696e 672e 6964 0a20 2020 2020  _coding.id.     
+0000d5a0: 2020 2073 656c 662e 6c6f 745f 6964 203d     self.lot_id =
+0000d5b0: 2073 656c 662e 6765 745f 6c6f 745f 6964   self.get_lot_id
+0000d5c0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000d5d0: 7472 6164 655f 6e61 6d65 203d 2073 656c  trade_name = sel
+0000d5e0: 662e 6765 745f 7472 6164 655f 6e61 6d65  f.get_trade_name
+0000d5f0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000d600: 7374 6174 7573 203d 2073 656c 662e 6765  status = self.ge
+0000d610: 745f 7374 6174 7573 2829 0a20 2020 2020  t_status().     
+0000d620: 2020 2073 656c 662e 6461 7465 203d 2073     self.date = s
+0000d630: 656c 662e 6765 745f 6461 7465 2829 2e69  elf.get_date().i
+0000d640: 736f 7374 7269 6e67 0a20 2020 2020 2020  sostring.       
+0000d650: 2076 6163 6369 6e65 5f63 6f64 6520 3d20   vaccine_code = 
+0000d660: 7365 6c66 2e67 6574 5f76 6163 6369 6e65  self.get_vaccine
+0000d670: 5f63 6f64 6528 0a20 2020 2020 2020 2020  _code(.         
+0000d680: 2020 2063 6f64 696e 675f 7379 7374 656d     coding_system
+0000d690: 3d63 6f64 696e 675f 7379 7374 656d 2c0a  =coding_system,.
+0000d6a0: 2020 2020 2020 2020 2020 2020 636f 6469              codi
+0000d6b0: 6e67 5f76 6572 7369 6f6e 3d63 6f64 696e  ng_version=codin
+0000d6c0: 675f 7665 7273 696f 6e29 0a20 2020 2020  g_version).     
+0000d6d0: 2020 2073 656c 662e 7661 6363 696e 655f     self.vaccine_
+0000d6e0: 636f 6465 5f63 6f64 6520 3d20 7661 6363  code_code = vacc
+0000d6f0: 696e 655f 636f 6465 2e63 6f64 650a 2020  ine_code.code.  
+0000d700: 2020 2020 2020 7365 6c66 2e76 6163 6369        self.vacci
+0000d710: 6e65 5f63 6f64 655f 6469 7370 6c61 7920  ne_code_display 
+0000d720: 3d20 7661 6363 696e 655f 636f 6465 2e64  = vaccine_code.d
+0000d730: 6973 706c 6179 0a20 2020 2020 2020 2073  isplay.        s
+0000d740: 656c 662e 7661 6363 696e 655f 636f 6465  elf.vaccine_code
+0000d750: 5f69 6420 3d20 7661 6363 696e 655f 636f  _id = vaccine_co
+0000d760: 6465 2e69 640a 2020 2020 2020 2020 7365  de.id.        se
+0000d770: 6c66 2e70 6174 6965 6e74 203d 2073 656c  lf.patient = sel
+0000d780: 662e 6765 745f 7061 7469 656e 7428 696d  f.get_patient(im
+0000d790: 6d75 6e69 7a61 7469 6f6e 3d69 6d6d 756e  munization=immun
+0000d7a0: 697a 6174 696f 6e29 0a20 2020 2020 2020  ization).       
+0000d7b0: 2073 656c 662e 7061 7469 656e 745f 7265   self.patient_re
+0000d7c0: 6665 7265 6e63 6520 3d20 7365 6c66 2e67  ference = self.g
+0000d7d0: 6574 5f70 6174 6965 6e74 5f72 6566 6572  et_patient_refer
+0000d7e0: 656e 6365 2869 6d6d 756e 697a 6174 696f  ence(immunizatio
+0000d7f0: 6e3d 696d 6d75 6e69 7a61 7469 6f6e 290a  n=immunization).
+0000d800: 2020 2020 2020 2020 7065 7266 6f72 6d65          performe
+0000d810: 725f 7265 6665 7265 6e63 6520 3d20 7365  r_reference = se
+0000d820: 6c66 2e67 6574 5f70 6572 666f 726d 6572  lf.get_performer
+0000d830: 5f72 6566 6572 656e 6365 2869 6d6d 756e  _reference(immun
+0000d840: 697a 6174 696f 6e3d 696d 6d75 6e69 7a61  ization=immuniza
+0000d850: 7469 6f6e 290a 2020 2020 2020 2020 6966  tion).        if
+0000d860: 2070 6572 666f 726d 6572 5f72 6566 6572   performer_refer
+0000d870: 656e 6365 2069 7320 6e6f 7420 4e6f 6e65  ence is not None
+0000d880: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000d890: 6c66 2e70 6572 666f 726d 6572 5f72 6566  lf.performer_ref
+0000d8a0: 6572 656e 6365 203d 2070 6572 666f 726d  erence = perform
+0000d8b0: 6572 5f72 6566 6572 656e 6365 2e72 6566  er_reference.ref
+0000d8c0: 6572 656e 6365 0a20 2020 2020 2020 2020  erence.         
+0000d8d0: 2020 2073 656c 662e 7065 7266 6f72 6d65     self.performe
+0000d8e0: 725f 6469 7370 6c61 7920 3d20 7065 7266  r_display = perf
+0000d8f0: 6f72 6d65 725f 7265 6665 7265 6e63 652e  ormer_reference.
+0000d900: 6469 7370 6c61 790a 2020 2020 2020 2020  display.        
+0000d910: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000d920: 2020 7365 6c66 2e70 6572 666f 726d 6572    self.performer
+0000d930: 203d 2073 656c 662e 6765 745f 7065 7266   = self.get_perf
+0000d940: 6f72 6d65 7228 696d 6d75 6e69 7a61 7469  ormer(immunizati
+0000d950: 6f6e 3d69 6d6d 756e 697a 6174 696f 6e29  on=immunization)
+0000d960: 0a0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+0000d970: 6f63 6174 696f 6e20 3d20 7365 6c66 2e67  ocation = self.g
+0000d980: 6574 5f6c 6f63 6174 696f 6e28 696d 6d75  et_location(immu
+0000d990: 6e69 7a61 7469 6f6e 3d69 6d6d 756e 697a  nization=immuniz
+0000d9a0: 6174 696f 6e29 0a20 2020 2020 2020 206c  ation).        l
+0000d9b0: 6f63 6174 696f 6e5f 7265 6620 3d20 7365  ocation_ref = se
+0000d9c0: 6c66 2e67 6574 5f6c 6f63 6174 696f 6e5f  lf.get_location_
+0000d9d0: 7265 6665 7265 6e63 6528 696d 6d75 6e69  reference(immuni
+0000d9e0: 7a61 7469 6f6e 3d69 6d6d 756e 697a 6174  zation=immunizat
+0000d9f0: 696f 6e29 0a20 2020 2020 2020 2069 6620  ion).        if 
+0000da00: 6c6f 6361 7469 6f6e 5f72 6566 2069 7320  location_ref is 
+0000da10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000da20: 2020 2020 2020 7365 6c66 2e6c 6f63 6174        self.locat
+0000da30: 696f 6e5f 7265 6665 7265 6e63 6520 3d20  ion_reference = 
+0000da40: 6c6f 6361 7469 6f6e 5f72 6566 2e72 6566  location_ref.ref
+0000da50: 6572 656e 6365 0a20 2020 2020 2020 2020  erence.         
+0000da60: 2020 2073 656c 662e 6c6f 6361 7469 6f6e     self.location
+0000da70: 5f64 6973 706c 6179 203d 206c 6f63 6174  _display = locat
+0000da80: 696f 6e5f 7265 662e 6469 7370 6c61 790a  ion_ref.display.
+0000da90: 2020 2020 2020 2020 7365 6c66 2e6c 6f74          self.lot
+0000daa0: 5f6e 756d 6265 7220 3d20 7365 6c66 2e67  _number = self.g
+0000dab0: 6574 5f6c 6f74 5f6e 756d 6265 7228 696d  et_lot_number(im
+0000dac0: 6d75 6e69 7a61 7469 6f6e 3d69 6d6d 756e  munization=immun
+0000dad0: 697a 6174 696f 6e29 0a20 2020 2020 2020  ization).       
+0000dae0: 2073 656c 662e 6578 7069 7261 7469 6f6e   self.expiration
+0000daf0: 5f64 6174 6520 3d20 7365 6c66 2e67 6574  _date = self.get
+0000db00: 5f65 7870 6972 6174 696f 6e5f 6461 7465  _expiration_date
+0000db10: 2869 6d6d 756e 697a 6174 696f 6e3d 696d  (immunization=im
+0000db20: 6d75 6e69 7a61 7469 6f6e 290a 2020 2020  munization).    
+0000db30: 2020 2020 7369 7465 203d 2073 656c 662e      site = self.
+0000db40: 6765 745f 7369 7465 280a 2020 2020 2020  get_site(.      
+0000db50: 2020 2020 2020 696d 6d75 6e69 7a61 7469        immunizati
+0000db60: 6f6e 3d69 6d6d 756e 697a 6174 696f 6e2c  on=immunization,
+0000db70: 0a20 2020 2020 2020 2020 2020 2063 6f64  .            cod
+0000db80: 696e 675f 7379 7374 656d 3d63 6f64 696e  ing_system=codin
+0000db90: 675f 7379 7374 656d 2c0a 2020 2020 2020  g_system,.      
+0000dba0: 2020 2020 2020 636f 6469 6e67 5f76 6572        coding_ver
+0000dbb0: 7369 6f6e 3d63 6f64 696e 675f 7665 7273  sion=coding_vers
+0000dbc0: 696f 6e29 0a20 2020 2020 2020 2069 6620  ion).        if 
+0000dbd0: 7369 7465 2069 7320 6e6f 7420 4e6f 6e65  site is not None
+0000dbe0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000dbf0: 6c66 2e73 6974 655f 636f 6465 203d 2073  lf.site_code = s
+0000dc00: 6974 652e 636f 6465 0a20 2020 2020 2020  ite.code.       
+0000dc10: 2020 2020 2073 656c 662e 7369 7465 5f64       self.site_d
+0000dc20: 6973 706c 6179 203d 2073 6974 652e 6469  isplay = site.di
+0000dc30: 7370 6c61 790a 2020 2020 2020 2020 2020  splay.          
+0000dc40: 2020 7365 6c66 2e73 6974 655f 6964 203d    self.site_id =
+0000dc50: 2073 6974 652e 6964 0a20 2020 2020 2020   site.id.       
+0000dc60: 2072 6f75 7465 5f63 6f64 696e 6720 3d20   route_coding = 
+0000dc70: 7365 6c66 2e67 6574 5f63 6f64 6561 626c  self.get_codeabl
+0000dc80: 655f 636f 6e63 6570 745f 636f 6469 6e67  e_concept_coding
+0000dc90: 280a 2020 2020 2020 2020 2020 2020 696d  (.            im
+0000dca0: 6d75 6e69 7a61 7469 6f6e 2e72 6f75 7465  munization.route
+0000dcb0: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+0000dcc0: 6469 6e67 5f73 7973 7465 6d3d 636f 6469  ding_system=codi
+0000dcd0: 6e67 5f73 7973 7465 6d2c 0a20 2020 2020  ng_system,.     
+0000dce0: 2020 2020 2020 2063 6f64 696e 675f 7665         coding_ve
+0000dcf0: 7273 696f 6e3d 636f 6469 6e67 5f76 6572  rsion=coding_ver
+0000dd00: 7369 6f6e 290a 2020 2020 2020 2020 7365  sion).        se
+0000dd10: 6c66 2e72 6f75 7465 5f63 6f64 6520 3d20  lf.route_code = 
+0000dd20: 726f 7574 655f 636f 6469 6e67 2e63 6f64  route_coding.cod
+0000dd30: 650a 2020 2020 2020 2020 7365 6c66 2e72  e.        self.r
+0000dd40: 6f75 7465 5f64 6973 706c 6179 203d 2072  oute_display = r
+0000dd50: 6f75 7465 5f63 6f64 696e 672e 6469 7370  oute_coding.disp
+0000dd60: 6c61 790a 2020 2020 2020 2020 7365 6c66  lay.        self
+0000dd70: 2e72 6f75 7465 5f69 6420 3d20 726f 7574  .route_id = rout
+0000dd80: 655f 636f 6469 6e67 2e69 640a 2020 2020  e_coding.id.    
+0000dd90: 2020 2020 646f 7365 5f71 7561 6e74 6974      dose_quantit
+0000dda0: 7920 3d20 7365 6c66 2e67 6574 5f64 6f73  y = self.get_dos
+0000ddb0: 655f 7175 616e 7469 7479 2869 6d6d 756e  e_quantity(immun
+0000ddc0: 697a 6174 696f 6e3d 696d 6d75 6e69 7a61  ization=immuniza
+0000ddd0: 7469 6f6e 290a 2020 2020 2020 2020 6966  tion).        if
+0000dde0: 2064 6f73 655f 7175 616e 7469 7479 2069   dose_quantity i
+0000ddf0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000de00: 2020 2020 2020 2020 7365 6c66 2e64 6f73          self.dos
+0000de10: 655f 7175 616e 7469 7479 5f63 6f64 6520  e_quantity_code 
+0000de20: 3d20 646f 7365 5f71 7561 6e74 6974 792e  = dose_quantity.
+0000de30: 636f 6465 0a20 2020 2020 2020 2020 2020  code.           
+0000de40: 2073 656c 662e 646f 7365 5f71 7561 6e74   self.dose_quant
+0000de50: 6974 795f 756e 6974 203d 2064 6f73 655f  ity_unit = dose_
+0000de60: 7175 616e 7469 7479 2e75 6e69 740a 2020  quantity.unit.  
+0000de70: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000de80: 6f73 655f 7175 616e 7469 7479 5f76 616c  ose_quantity_val
+0000de90: 7565 203d 2064 6f73 655f 7175 616e 7469  ue = dose_quanti
+0000dea0: 7479 2e76 616c 7565 0a20 2020 2020 2020  ty.value.       
+0000deb0: 2073 656c 662e 7265 6173 6f6e 203d 2073   self.reason = s
+0000dec0: 656c 662e 6765 745f 7265 6173 6f6e 7328  elf.get_reasons(
+0000ded0: 696d 6d75 6e69 7a61 7469 6f6e 3d69 6d6d  immunization=imm
+0000dee0: 756e 697a 6174 696f 6e2c 636f 6469 6e67  unization,coding
+0000def0: 5f73 7973 7465 6d3d 636f 6469 6e67 5f73  _system=coding_s
+0000df00: 7973 7465 6d2c 2063 6f64 696e 675f 7665  ystem, coding_ve
+0000df10: 7273 696f 6e3d 636f 6469 6e67 5f76 6572  rsion=coding_ver
+0000df20: 7369 6f6e 290a 0a63 6c61 7373 2050 6174  sion)..class Pat
+0000df30: 6965 6e74 4648 4952 2842 6173 6546 4849  ientFHIR(BaseFHI
+0000df40: 5229 3a0a 2020 2020 7265 736f 7572 6365  R):.    resource
+0000df50: 5f74 7970 6520 3d20 2750 6174 6965 6e74  _type = 'Patient
+0000df60: 270a 2020 2020 6465 6661 756c 745f 636f  '.    default_co
+0000df70: 6469 6e67 5f73 7973 7465 6d20 3d20 2768  ding_system = 'h
+0000df80: 7474 703a 2f2f 7777 772e 7361 6e74 6570  ttp://www.santep
+0000df90: 7562 6c69 7175 652e 7274 7373 2e71 632e  ublique.rtss.qc.
+0000dfa0: 6361 2f73 6970 6d69 2f66 612f 312e 302e  ca/sipmi/fa/1.0.
+0000dfb0: 302f 766f 6361 6275 6c61 7279 270a 2020  0/vocabulary'.  
+0000dfc0: 2020 6465 6661 756c 745f 636f 6469 6e67    default_coding
+0000dfd0: 5f76 6572 7369 6f6e 203d 2022 312e 302e  _version = "1.0.
+0000dfe0: 3022 0a20 2020 206e 616d 5f69 6465 6e74  0".    nam_ident
+0000dff0: 6966 6965 725f 6578 7465 6e73 696f 6e5f  ifier_extension_
+0000e000: 7572 6c20 3d20 2268 7474 703a 2f2f 7777  url = "http://ww
+0000e010: 772e 7361 6e74 6570 7562 6c69 7175 652e  w.santepublique.
+0000e020: 7274 7373 2e71 632e 6361 2f73 6970 6d69  rtss.qc.ca/sipmi
+0000e030: 2f66 612f 312e 302e 302f 6578 7465 6e73  /fa/1.0.0/extens
+0000e040: 696f 6e73 2f23 7061 7469 656e 742f 6865  ions/#patient/he
+0000e050: 616c 7468 6361 7264 6f72 6967 696e 220a  althcardorigin".
+0000e060: 2020 2020 6e61 6d5f 6964 656e 7469 6669      nam_identifi
+0000e070: 6572 5f73 7973 7465 6d20 3d20 2268 7474  er_system = "htt
+0000e080: 703a 2f2f 7777 772e 7361 6e74 6570 7562  p://www.santepub
+0000e090: 6c69 7175 652e 7274 7373 2e71 632e 6361  lique.rtss.qc.ca
+0000e0a0: 2f73 6970 6d69 2f66 612f 312e 302e 302f  /sipmi/fa/1.0.0/
+0000e0b0: 766f 6361 6275 6c61 7279 2f69 6465 6e74  vocabulary/ident
+0000e0c0: 6966 6965 7254 7970 653f 636f 6465 3d4e  ifierType?code=N
+0000e0d0: 414d 220a 2020 2020 6e69 755f 6964 656e  AM".    niu_iden
+0000e0e0: 7469 6669 6572 5f73 7973 7465 6d20 3d20  tifier_system = 
+0000e0f0: 2268 7474 703a 2f2f 7777 772e 7361 6e74  "http://www.sant
+0000e100: 6570 7562 6c69 7175 652e 7274 7373 2e71  epublique.rtss.q
+0000e110: 632e 6361 2f73 6970 6d69 2f66 612f 312e  c.ca/sipmi/fa/1.
+0000e120: 302e 302f 766f 6361 6275 6c61 7279 2f69  0.0/vocabulary/i
+0000e130: 6465 6e74 6966 6965 7254 7970 653f 636f  dentifierType?co
+0000e140: 6465 3d4e 4955 5522 0a20 2020 2061 7563  de=NIUU".    auc
+0000e150: 756e 5f69 6465 6e74 6966 6965 725f 7379  un_identifier_sy
+0000e160: 7374 656d 203d 2022 6874 7470 3a2f 2f77  stem = "http://w
+0000e170: 7777 2e73 616e 7465 7075 626c 6971 7565  ww.santepublique
+0000e180: 2e72 7473 732e 7163 2e63 612f 7369 706d  .rtss.qc.ca/sipm
+0000e190: 692f 6661 2f31 2e30 2e30 2f76 6f63 6162  i/fa/1.0.0/vocab
+0000e1a0: 756c 6172 792f 6964 656e 7469 6669 6572  ulary/identifier
+0000e1b0: 5479 7065 3f63 6f64 653d 4155 4355 4e22  Type?code=AUCUN"
+0000e1c0: 0a20 2020 206d 6174 6368 7261 6d71 5f65  .    matchramq_e
+0000e1d0: 7874 656e 7369 6f6e 5f75 726c 203d 2022  xtension_url = "
+0000e1e0: 6874 7470 3a2f 2f77 7777 2e73 616e 7465  http://www.sante
+0000e1f0: 7075 626c 6971 7565 2e72 7473 732e 7163  publique.rtss.qc
+0000e200: 2e63 612f 7369 706d 692f 6661 2f31 2e30  .ca/sipmi/fa/1.0
+0000e210: 2e30 2f65 7874 656e 7369 6f6e 732f 2370  .0/extensions/#p
+0000e220: 6174 6965 6e74 2f6d 6174 6368 7261 6d71  atient/matchramq
+0000e230: 220a 2020 2020 6964 203d 204e 6f6e 650a  ".    id = None.
+0000e240: 2020 2020 7573 6572 5f6e 616d 6520 3d20      user_name = 
+0000e250: 4e6f 6e65 0a20 2020 2063 7265 6174 696f  None.    creatio
+0000e260: 6e5f 6461 7465 203d 204e 6f6e 650a 2020  n_date = None.  
+0000e270: 2020 7570 6461 7465 5f74 696d 6573 7461    update_timesta
+0000e280: 6d70 203d 204e 6f6e 650a 2020 2020 6d61  mp = None.    ma
+0000e290: 7463 6872 616d 7120 3d20 4e6f 6e65 0a20  tchramq = None. 
+0000e2a0: 2020 2061 6374 6976 6520 3d20 5472 7565     active = True
+0000e2b0: 0a20 2020 206e 616d 203d 204e 6f6e 650a  .    nam = None.
+0000e2c0: 2020 2020 6e69 7520 3d20 4e6f 6e65 0a20      niu = None. 
+0000e2d0: 2020 2066 616d 696c 795f 6e61 6d65 203d     family_name =
+0000e2e0: 204e 6f6e 650a 2020 2020 6769 7665 6e5f   None.    given_
+0000e2f0: 6e61 6d65 203d 204e 6f6e 650a 2020 2020  name = None.    
+0000e300: 7068 6f6e 655f 6e75 6d62 6572 203d 204e  phone_number = N
+0000e310: 6f6e 650a 2020 2020 6765 6e64 6572 203d  one.    gender =
+0000e320: 204e 6f6e 650a 2020 2020 6269 7274 685f   None.    birth_
+0000e330: 6461 7465 203d 204e 6f6e 650a 2020 2020  date = None.    
+0000e340: 6465 6365 6173 6564 5f62 6f6f 6c65 616e  deceased_boolean
+0000e350: 203d 2046 616c 7365 0a20 2020 2061 6464   = False.    add
+0000e360: 7265 7373 5f6c 696e 6520 3d20 4e6f 6e65  ress_line = None
+0000e370: 0a20 2020 2061 6464 7265 7373 5f63 6974  .    address_cit
+0000e380: 7920 3d20 4e6f 6e65 0a20 2020 2061 6464  y = None.    add
+0000e390: 7265 7373 5f73 7461 7465 203d 204e 6f6e  ress_state = Non
+0000e3a0: 650a 2020 2020 6164 6472 6573 735f 706f  e.    address_po
+0000e3b0: 7374 616c 5f63 6f64 6520 3d20 4e6f 6e65  stal_code = None
+0000e3c0: 0a20 2020 2061 6464 7265 7373 5f63 6f75  .    address_cou
+0000e3d0: 6e74 7279 203d 204e 6f6e 650a 2020 2020  ntry = None.    
+0000e3e0: 6d6f 7468 6572 5f67 6976 656e 5f6e 616d  mother_given_nam
+0000e3f0: 6520 3d20 4e6f 6e65 0a20 2020 206d 6f74  e = None.    mot
+0000e400: 6865 725f 6661 6d69 6c79 5f6e 616d 6520  her_family_name 
+0000e410: 3d20 4e6f 6e65 0a20 2020 2066 6174 6865  = None.    fathe
+0000e420: 725f 6769 7665 6e5f 6e61 6d65 203d 204e  r_given_name = N
+0000e430: 6f6e 650a 2020 2020 6661 7468 6572 5f66  one.    father_f
+0000e440: 616d 696c 795f 6e61 6d65 203d 204e 6f6e  amily_name = Non
+0000e450: 650a 2020 2020 6261 7365 5f75 726c 203d  e.    base_url =
+0000e460: 2022 220a 2020 2020 7061 7469 656e 745f   "".    patient_
+0000e470: 656e 6470 6f69 6e74 203d 2022 7b30 7d2f  endpoint = "{0}/
+0000e480: 5061 7469 656e 7422 0a20 2020 2070 6174  Patient".    pat
+0000e490: 6965 6e74 5f69 645f 656e 6470 6f69 6e74  ient_id_endpoint
+0000e4a0: 203d 2022 7b30 7d2f 5061 7469 656e 742f   = "{0}/Patient/
+0000e4b0: 7b31 7d22 0a20 2020 2070 6174 6965 6e74  {1}".    patient
+0000e4c0: 5f6d 6174 6368 5f65 6e64 706f 696e 7420  _match_endpoint 
+0000e4d0: 3d20 227b 307d 2f50 6174 6965 6e74 2f24  = "{0}/Patient/$
+0000e4e0: 6d61 7463 6822 0a20 2020 2070 6174 6965  match".    patie
+0000e4f0: 6e74 5f64 6566 696e 6972 5f6e 6975 5f65  nt_definir_niu_e
+0000e500: 6e64 706f 696e 7420 3d20 7061 7469 656e  ndpoint = patien
+0000e510: 745f 6964 5f65 6e64 706f 696e 7420 2b20  t_id_endpoint + 
+0000e520: 222f 2464 6566 696e 6972 2d6e 6975 220a  "/$definir-niu".
+0000e530: 0a20 2020 2068 6561 6465 7273 203d 207b  .    headers = {
+0000e540: 7d0a 2020 2020 6668 6972 5f72 6573 6f75  }.    fhir_resou
+0000e550: 7263 6520 3d20 4e6f 6e65 0a20 2020 2064  rce = None.    d
+0000e560: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0000e570: 2c20 6261 7365 5f75 726c 3d4e 6f6e 652c  , base_url=None,
+0000e580: 2062 6173 655f 7572 693d 4e6f 6e65 2c20   base_uri=None, 
+0000e590: 7061 7469 656e 745f 6469 6374 3d4e 6f6e  patient_dict=Non
+0000e5a0: 652c 2074 6f6b 656e 3d4e 6f6e 652c 2070  e, token=None, p
+0000e5b0: 6174 6965 6e74 5f72 6573 6f75 7263 655f  atient_resource_
+0000e5c0: 6469 6374 3d4e 6f6e 652c 2076 616c 6964  dict=None, valid
+0000e5d0: 6174 655f 6365 7274 733d 5472 7565 293a  ate_certs=True):
+0000e5e0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+0000e5f0: 2e5f 5f69 6e69 745f 5f28 6261 7365 5f75  .__init__(base_u
+0000e600: 726c 3d62 6173 655f 7572 6c2c 2062 6173  rl=base_url, bas
+0000e610: 655f 7572 693d 6261 7365 5f75 7269 290a  e_uri=base_uri).
+0000e620: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+0000e630: 6964 6174 655f 6365 7274 7320 3d20 7661  idate_certs = va
+0000e640: 6c69 6461 7465 5f63 6572 7473 0a20 2020  lidate_certs.   
+0000e650: 2020 2020 2069 6620 7061 7469 656e 745f       if patient_
+0000e660: 7265 736f 7572 6365 5f64 6963 7420 6973  resource_dict is
+0000e670: 204e 6f6e 6520 616e 6420 7061 7469 656e   None and patien
+0000e680: 745f 6469 6374 2069 7320 6e6f 7420 4e6f  t_dict is not No
+0000e690: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000e6a0: 7365 6c66 2e66 726f 6d5f 6469 6374 2870  self.from_dict(p
+0000e6b0: 6174 6965 6e74 5f64 6963 7429 0a20 2020  atient_dict).   
+0000e6c0: 2020 2020 2020 2020 2073 656c 662e 6668           self.fh
+0000e6d0: 6972 5f72 6573 6f75 7263 6520 3d20 7365  ir_resource = se
+0000e6e0: 6c66 2e70 6174 6965 6e74 5f64 6963 745f  lf.patient_dict_
+0000e6f0: 746f 5f66 6869 725f 7061 7469 656e 7428  to_fhir_patient(
+0000e700: 7061 7469 656e 745f 6469 6374 3d70 6174  patient_dict=pat
+0000e710: 6965 6e74 5f64 6963 742c 2070 6174 6965  ient_dict, patie
+0000e720: 6e74 3d50 6174 6965 6e74 2829 290a 2020  nt=Patient()).  
+0000e730: 2020 2020 2020 656c 6966 2070 6174 6965        elif patie
+0000e740: 6e74 5f72 6573 6f75 7263 655f 6469 6374  nt_resource_dict
+0000e750: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000e760: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+0000e770: 6869 725f 7265 736f 7572 6365 203d 2050  hir_resource = P
+0000e780: 6174 6965 6e74 286a 736f 6e64 6963 743d  atient(jsondict=
+0000e790: 7061 7469 656e 745f 7265 736f 7572 6365  patient_resource
+0000e7a0: 5f64 6963 7429 0a20 2020 2020 2020 2020  _dict).         
+0000e7b0: 2020 2073 656c 662e 6672 6f6d 5f66 6869     self.from_fhi
+0000e7c0: 725f 7061 7469 656e 7428 290a 2020 2020  r_patient().    
+0000e7d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000e7e0: 2020 2020 2020 7365 6c66 2e66 6869 725f        self.fhir_
+0000e7f0: 7265 736f 7572 6365 203d 2050 6174 6965  resource = Patie
+0000e800: 6e74 2829 0a0a 2020 2020 2020 2020 6966  nt()..        if
+0000e810: 2062 6173 655f 7572 6c20 6973 206e 6f74   base_url is not
+0000e820: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000e830: 2020 2073 656c 662e 6261 7365 5f75 726c     self.base_url
+0000e840: 203d 2062 6173 655f 7572 6c0a 2020 2020   = base_url.    
+0000e850: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000e860: 2073 656c 662e 7365 7448 6561 6465 7273   self.setHeaders
+0000e870: 2874 6f6b 656e 3d74 6f6b 656e 290a 0a20  (token=token).. 
+0000e880: 2020 2064 6566 2066 726f 6d5f 6469 6374     def from_dict
+0000e890: 2873 656c 662c 2070 6174 6965 6e74 5f64  (self, patient_d
+0000e8a0: 6963 7429 3a0a 2020 2020 2020 2020 7365  ict):.        se
+0000e8b0: 6c66 2e69 6420 3d20 7061 7469 656e 745f  lf.id = patient_
+0000e8c0: 6469 6374 5b27 6964 275d 2069 6620 2769  dict['id'] if 'i
+0000e8d0: 6427 2069 6e20 7061 7469 656e 745f 6469  d' in patient_di
+0000e8e0: 6374 2065 6c73 6520 4e6f 6e65 0a20 2020  ct else None.   
+0000e8f0: 2020 2020 2073 656c 662e 6769 7665 6e5f       self.given_
+0000e900: 6e61 6d65 203d 2070 6174 6965 6e74 5f64  name = patient_d
+0000e910: 6963 745b 2767 6976 656e 5f6e 616d 6527  ict['given_name'
+0000e920: 5d20 6966 2027 6769 7665 6e5f 6e61 6d65  ] if 'given_name
+0000e930: 2720 696e 2070 6174 6965 6e74 5f64 6963  ' in patient_dic
+0000e940: 7420 656c 7365 204e 6f6e 650a 2020 2020  t else None.    
+0000e950: 2020 2020 7365 6c66 2e66 616d 696c 795f      self.family_
+0000e960: 6e61 6d65 203d 2070 6174 6965 6e74 5f64  name = patient_d
+0000e970: 6963 745b 2766 616d 696c 795f 6e61 6d65  ict['family_name
+0000e980: 275d 2069 6620 2766 616d 696c 795f 6e61  '] if 'family_na
+0000e990: 6d65 2720 696e 2070 6174 6965 6e74 5f64  me' in patient_d
+0000e9a0: 6963 7420 656c 7365 204e 6f6e 650a 2020  ict else None.  
+0000e9b0: 2020 2020 2020 7365 6c66 2e61 6374 6976        self.activ
+0000e9c0: 6520 3d20 7061 7469 656e 745f 6469 6374  e = patient_dict
+0000e9d0: 5b27 6163 7469 7665 275d 2069 6620 2761  ['active'] if 'a
+0000e9e0: 6374 6976 6527 2069 6e20 7061 7469 656e  ctive' in patien
+0000e9f0: 745f 6469 6374 2065 6c73 6520 5472 7565  t_dict else True
+0000ea00: 0a20 2020 2020 2020 2073 656c 662e 6765  .        self.ge
+0000ea10: 6e64 6572 203d 2070 6174 6965 6e74 5f64  nder = patient_d
+0000ea20: 6963 745b 2767 656e 6465 7227 5d20 6966  ict['gender'] if
+0000ea30: 2027 6765 6e64 6572 2720 696e 2070 6174   'gender' in pat
+0000ea40: 6965 6e74 5f64 6963 7420 656c 7365 204e  ient_dict else N
+0000ea50: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+0000ea60: 2e62 6972 7468 5f64 6174 6520 3d20 7061  .birth_date = pa
+0000ea70: 7469 656e 745f 6469 6374 5b27 6269 7274  tient_dict['birt
+0000ea80: 685f 6461 7465 275d 2069 6620 2762 6972  h_date'] if 'bir
+0000ea90: 7468 5f64 6174 6527 2069 6e20 7061 7469  th_date' in pati
+0000eaa0: 656e 745f 6469 6374 2065 6c73 6520 4e6f  ent_dict else No
+0000eab0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000eac0: 6e69 7520 3d20 7061 7469 656e 745f 6469  niu = patient_di
+0000ead0: 6374 5b27 6e69 7527 5d20 6966 2027 6e69  ct['niu'] if 'ni
+0000eae0: 7527 2069 6e20 7061 7469 656e 745f 6469  u' in patient_di
+0000eaf0: 6374 2065 6c73 6520 4e6f 6e65 0a20 2020  ct else None.   
+0000eb00: 2020 2020 2073 656c 662e 6e61 6d20 3d20       self.nam = 
+0000eb10: 7061 7469 656e 745f 6469 6374 5b27 6e61  patient_dict['na
+0000eb20: 6d27 5d20 6966 2027 6e61 6d27 2069 6e20  m'] if 'nam' in 
+0000eb30: 7061 7469 656e 745f 6469 6374 2065 6c73  patient_dict els
+0000eb40: 6520 4e6f 6e65 0a20 2020 2020 2020 2073  e None.        s
+0000eb50: 656c 662e 6164 6472 6573 735f 6c69 6e65  elf.address_line
+0000eb60: 203d 2070 6174 6965 6e74 5f64 6963 745b   = patient_dict[
+0000eb70: 2761 6464 7265 7373 5f6c 696e 6527 5d20  'address_line'] 
+0000eb80: 6966 2027 6164 6472 6573 735f 6c69 6e65  if 'address_line
+0000eb90: 2720 696e 2070 6174 6965 6e74 5f64 6963  ' in patient_dic
+0000eba0: 7420 656c 7365 204e 6f6e 650a 2020 2020  t else None.    
+0000ebb0: 2020 2020 7365 6c66 2e61 6464 7265 7373      self.address
+0000ebc0: 5f63 6974 7920 3d20 7061 7469 656e 745f  _city = patient_
+0000ebd0: 6469 6374 5b27 6164 6472 6573 735f 6369  dict['address_ci
+0000ebe0: 7479 275d 2069 6620 2761 6464 7265 7373  ty'] if 'address
+0000ebf0: 5f63 6974 7927 2069 6e20 7061 7469 656e  _city' in patien
+0000ec00: 745f 6469 6374 2065 6c73 6520 4e6f 6e65  t_dict else None
+0000ec10: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+0000ec20: 6472 6573 735f 7374 6174 6520 3d20 7061  dress_state = pa
+0000ec30: 7469 656e 745f 6469 6374 5b27 6164 6472  tient_dict['addr
+0000ec40: 6573 735f 7374 6174 6527 5d20 6966 2027  ess_state'] if '
+0000ec50: 6164 6472 6573 735f 7374 6174 6527 2069  address_state' i
+0000ec60: 6e20 7061 7469 656e 745f 6469 6374 2065  n patient_dict e
+0000ec70: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
+0000ec80: 2073 656c 662e 6164 6472 6573 735f 706f   self.address_po
+0000ec90: 7374 616c 5f63 6f64 6520 3d20 7061 7469  stal_code = pati
+0000eca0: 656e 745f 6469 6374 5b27 6164 6472 6573  ent_dict['addres
+0000ecb0: 735f 706f 7374 616c 5f63 6f64 6527 5d20  s_postal_code'] 
+0000ecc0: 6966 2027 6164 6472 6573 735f 706f 7374  if 'address_post
+0000ecd0: 616c 5f63 6f64 6527 2069 6e20 7061 7469  al_code' in pati
+0000ece0: 656e 745f 6469 6374 2065 6c73 6520 4e6f  ent_dict else No
+0000ecf0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
+0000ed00: 6164 6472 6573 735f 636f 756e 7472 7920  address_country 
+0000ed10: 3d20 7061 7469 656e 745f 6469 6374 5b27  = patient_dict['
+0000ed20: 6164 6472 6573 735f 636f 756e 7472 7927  address_country'
+0000ed30: 5d20 6966 2027 6164 6472 6573 735f 636f  ] if 'address_co
+0000ed40: 756e 7472 7927 2069 6e20 7061 7469 656e  untry' in patien
+0000ed50: 745f 6469 6374 2065 6c73 6520 4e6f 6e65  t_dict else None
+0000ed60: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
+0000ed70: 7468 6572 5f67 6976 656e 5f6e 616d 6520  ther_given_name 
+0000ed80: 3d20 7061 7469 656e 745f 6469 6374 5b27  = patient_dict['
+0000ed90: 6d6f 7468 6572 5f67 6976 656e 5f6e 616d  mother_given_nam
+0000eda0: 6527 5d20 6966 2027 6d6f 7468 6572 5f67  e'] if 'mother_g
+0000edb0: 6976 656e 5f6e 616d 6527 2069 6e20 7061  iven_name' in pa
+0000edc0: 7469 656e 745f 6469 6374 2065 6c73 6520  tient_dict else 
+0000edd0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
+0000ede0: 662e 6d6f 7468 6572 5f66 616d 696c 795f  f.mother_family_
+0000edf0: 6e61 6d65 203d 2070 6174 6965 6e74 5f64  name = patient_d
+0000ee00: 6963 745b 276d 6f74 6865 725f 6661 6d69  ict['mother_fami
+0000ee10: 6c79 5f6e 616d 6527 5d20 6966 2027 6d6f  ly_name'] if 'mo
+0000ee20: 7468 6572 5f66 616d 696c 795f 6e61 6d65  ther_family_name
+0000ee30: 2720 696e 2070 6174 6965 6e74 5f64 6963  ' in patient_dic
+0000ee40: 7420 656c 7365 204e 6f6e 650a 2020 2020  t else None.    
+0000ee50: 2020 2020 7365 6c66 2e66 6174 6865 725f      self.father_
+0000ee60: 6769 7665 6e5f 6e61 6d65 203d 2070 6174  given_name = pat
+0000ee70: 6965 6e74 5f64 6963 745b 2766 6174 6865  ient_dict['fathe
+0000ee80: 725f 6769 7665 6e5f 6e61 6d65 275d 2069  r_given_name'] i
+0000ee90: 6620 2766 6174 6865 725f 6769 7665 6e5f  f 'father_given_
+0000eea0: 6e61 6d65 2720 696e 2070 6174 6965 6e74  name' in patient
+0000eeb0: 5f64 6963 7420 656c 7365 204e 6f6e 650a  _dict else None.
+0000eec0: 2020 2020 2020 2020 7365 6c66 2e66 6174          self.fat
+0000eed0: 6865 725f 6661 6d69 6c79 5f6e 616d 6520  her_family_name 
+0000eee0: 3d20 7061 7469 656e 745f 6469 6374 5b27  = patient_dict['
+0000eef0: 6661 7468 6572 5f66 616d 696c 795f 6e61  father_family_na
+0000ef00: 6d65 275d 2069 6620 2766 6174 6865 725f  me'] if 'father_
+0000ef10: 6661 6d69 6c79 5f6e 616d 6527 2069 6e20  family_name' in 
+0000ef20: 7061 7469 656e 745f 6469 6374 2065 6c73  patient_dict els
+0000ef30: 6520 4e6f 6e65 0a20 2020 2020 2020 2073  e None.        s
+0000ef40: 656c 662e 7068 6f6e 655f 6e75 6d62 6572  elf.phone_number
+0000ef50: 203d 2070 6174 6965 6e74 5f64 6963 745b   = patient_dict[
+0000ef60: 2770 686f 6e65 5f6e 756d 6265 7227 5d20  'phone_number'] 
+0000ef70: 6966 2027 7068 6f6e 655f 6e75 6d62 6572  if 'phone_number
+0000ef80: 2720 696e 2070 6174 6965 6e74 5f64 6963  ' in patient_dic
+0000ef90: 7420 656c 7365 204e 6f6e 650a 0a20 2020  t else None..   
+0000efa0: 2064 6566 2066 726f 6d5f 6a73 6f6e 2873   def from_json(s
+0000efb0: 656c 662c 2072 6573 6f75 7263 6529 3a0a  elf, resource):.
+0000efc0: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+0000efd0: 7265 736f 7572 6365 2920 6973 2073 7472  resource) is str
+0000efe0: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
+0000eff0: 725f 7265 736f 7572 6365 203d 2072 6573  r_resource = res
+0000f000: 6f75 7263 650a 2020 2020 2020 2020 2020  ource.          
+0000f010: 2020 7265 736f 7572 6365 203d 206a 736f    resource = jso
+0000f020: 6e2e 6c6f 6164 7328 7374 725f 7265 736f  n.loads(str_reso
+0000f030: 7572 6365 290a 2020 2020 2020 2020 7365  urce).        se
+0000f040: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+0000f050: 203d 2050 6174 6965 6e74 286a 736f 6e64   = Patient(jsond
+0000f060: 6963 743d 7265 736f 7572 6365 290a 2020  ict=resource).  
+0000f070: 2020 2020 2020 7365 6c66 2e66 726f 6d5f        self.from_
+0000f080: 6668 6972 5f70 6174 6965 6e74 2829 0a0a  fhir_patient()..
+0000f090: 2020 2020 6465 6620 6765 7446 6869 7252      def getFhirR
+0000f0a0: 6573 6f75 7263 6528 7365 6c66 293a 0a20  esource(self):. 
+0000f0b0: 2020 2020 2020 2073 656c 662e 746f 5f66         self.to_f
+0000f0c0: 6869 725f 7061 7469 656e 7428 290a 2020  hir_patient().  
+0000f0d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000f0e0: 662e 6668 6972 5f72 6573 6f75 7263 652e  f.fhir_resource.
+0000f0f0: 6173 5f6a 736f 6e28 290a 0a20 2020 2064  as_json()..    d
+0000f100: 6566 2067 6574 4668 6972 5265 736f 7572  ef getFhirResour
+0000f110: 6365 5061 7261 6d65 7465 7228 7365 6c66  ceParameter(self
+0000f120: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000f130: 746f 5f66 6869 725f 7061 7469 656e 7428  to_fhir_patient(
+0000f140: 290a 2020 2020 2020 2020 7061 7261 6d20  ).        param 
+0000f150: 3d20 5061 7261 6d65 7465 7246 4849 5228  = ParameterFHIR(
+0000f160: 290a 2020 2020 2020 2020 7061 7261 6d2e  ).        param.
+0000f170: 6164 645f 7061 7261 6d65 7465 7228 7365  add_parameter(se
+0000f180: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+0000f190: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000f1a0: 2070 6172 616d 2e67 6574 4668 6972 5265   param.getFhirRe
+0000f1b0: 736f 7572 6365 2829 0a0a 2020 2020 6465  source()..    de
+0000f1c0: 6620 7365 7448 6561 6465 7273 2873 656c  f setHeaders(sel
+0000f1d0: 662c 2068 6561 6465 7273 3d7b 7d2c 2074  f, headers={}, t
+0000f1e0: 6f6b 656e 3d4e 6f6e 6529 3a0a 2020 2020  oken=None):.    
+0000f1f0: 2020 2020 6e65 7748 6561 6465 7273 203d      newHeaders =
+0000f200: 207b 2a2a 6865 6164 6572 732c 202a 2a73   {**headers, **s
+0000f210: 656c 662e 6261 7365 5f68 6561 6465 7273  elf.base_headers
+0000f220: 7d0a 2020 2020 2020 2020 6966 2074 6f6b  }.        if tok
+0000f230: 656e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  en is not None:.
+0000f240: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+0000f250: 436f 6e74 656e 742d 7479 7065 2720 696e  Content-type' in
+0000f260: 2074 6f6b 656e 3a0a 2020 2020 2020 2020   token:.        
+0000f270: 2020 2020 2020 2020 6465 6c20 746f 6b65          del toke
+0000f280: 6e5b 2743 6f6e 7465 6e74 2d74 7970 6527  n['Content-type'
+0000f290: 5d0a 2020 2020 2020 2020 2020 2020 6865  ].            he
+0000f2a0: 6164 6572 7357 6974 6841 7574 6820 3d20  adersWithAuth = 
+0000f2b0: 7b2a 2a6e 6577 4865 6164 6572 732c 202a  {**newHeaders, *
+0000f2c0: 2a74 6f6b 656e 7d0a 2020 2020 2020 2020  *token}.        
+0000f2d0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+0000f2e0: 203d 2068 6561 6465 7273 5769 7468 4175   = headersWithAu
+0000f2f0: 7468 0a20 2020 2020 2020 2065 6c73 653a  th.        else:
+0000f300: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f310: 662e 6865 6164 6572 7320 3d20 6e65 7748  f.headers = newH
+0000f320: 6561 6465 7273 0a20 2020 2020 2020 2072  eaders.        r
+0000f330: 6574 7572 6e20 7365 6c66 2e68 6561 6465  eturn self.heade
+0000f340: 7273 0a0a 2020 2020 6465 6620 4372 6561  rs..    def Crea
+0000f350: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0000f360: 2020 7265 7320 3d20 7365 6c66 2e67 6574    res = self.get
+0000f370: 4668 6972 5265 736f 7572 6365 2829 0a20  FhirResource(). 
+0000f380: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+0000f390: 3d20 7265 7175 6573 7473 2e70 6f73 7428  = requests.post(
+0000f3a0: 7572 6c3d 7365 6c66 2e70 6174 6965 6e74  url=self.patient
+0000f3b0: 5f65 6e64 706f 696e 742e 666f 726d 6174  _endpoint.format
+0000f3c0: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000f3d0: 6c66 2e67 6574 5f66 6869 725f 7572 6c28  lf.get_fhir_url(
+0000f3e0: 2929 2c20 6461 7461 3d6a 736f 6e2e 6475  )), data=json.du
+0000f3f0: 6d70 7328 7265 7329 2c20 6865 6164 6572  mps(res), header
+0000f400: 733d 7365 6c66 2e68 6561 6465 7273 2c20  s=self.headers, 
+0000f410: 7665 7269 6679 3d73 656c 662e 7661 6c69  verify=self.vali
+0000f420: 6461 7465 5f63 6572 7473 290a 2020 2020  date_certs).    
+0000f430: 2020 2020 7365 6c66 2e66 726f 6d5f 6a73      self.from_js
+0000f440: 6f6e 2872 6573 6f75 7263 653d 7265 7370  on(resource=resp
+0000f450: 6f6e 7365 2e63 6f6e 7465 6e74 2e64 6563  onse.content.dec
+0000f460: 6f64 6528 2929 0a20 2020 2020 2020 2069  ode()).        i
+0000f470: 6620 7365 6c66 2e6e 6975 2069 7320 6e6f  f self.niu is no
+0000f480: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000f490: 2020 2020 7265 7320 3d20 7365 6c66 2e67      res = self.g
+0000f4a0: 6574 4668 6972 5265 736f 7572 6365 5061  etFhirResourcePa
+0000f4b0: 7261 6d65 7465 7228 290a 2020 2020 2020  rameter().      
+0000f4c0: 2020 2020 2020 7265 7175 6573 7473 2e70        requests.p
+0000f4d0: 6f73 7428 7572 6c3d 7365 6c66 2e70 6174  ost(url=self.pat
+0000f4e0: 6965 6e74 5f64 6566 696e 6972 5f6e 6975  ient_definir_niu
+0000f4f0: 5f65 6e64 706f 696e 742e 666f 726d 6174  _endpoint.format
+0000f500: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000f510: 2020 7365 6c66 2e67 6574 5f66 6869 725f    self.get_fhir_
+0000f520: 7572 6c28 292c 2073 656c 662e 6964 292c  url(), self.id),
+0000f530: 2064 6174 613d 6a73 6f6e 2e64 756d 7073   data=json.dumps
+0000f540: 2872 6573 292c 2068 6561 6465 7273 3d73  (res), headers=s
+0000f550: 656c 662e 6865 6164 6572 732c 2076 6572  elf.headers, ver
+0000f560: 6966 793d 7365 6c66 2e76 616c 6964 6174  ify=self.validat
+0000f570: 655f 6365 7274 7329 0a20 2020 2020 2020  e_certs).       
+0000f580: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+0000f590: 0a0a 2020 2020 6465 6620 4765 7442 7949  ..    def GetByI
+0000f5a0: 6428 7365 6c66 2c20 7061 7469 656e 745f  d(self, patient_
+0000f5b0: 6964 3d4e 6f6e 6529 3a0a 2020 2020 2020  id=None):.      
+0000f5c0: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
+0000f5d0: 7565 7374 732e 6765 7428 7572 6c3d 7365  uests.get(url=se
+0000f5e0: 6c66 2e70 6174 6965 6e74 5f69 645f 656e  lf.patient_id_en
+0000f5f0: 6470 6f69 6e74 2e66 6f72 6d61 7428 0a20  dpoint.format(. 
+0000f600: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f610: 6765 745f 6668 6972 5f75 726c 2829 2c20  get_fhir_url(), 
+0000f620: 7061 7469 656e 745f 6964 292c 2068 6561  patient_id), hea
+0000f630: 6465 7273 3d73 656c 662e 6865 6164 6572  ders=self.header
+0000f640: 732c 2076 6572 6966 793d 7365 6c66 2e76  s, verify=self.v
+0000f650: 616c 6964 6174 655f 6365 7274 7329 0a20  alidate_certs). 
+0000f660: 2020 2020 2020 2073 656c 662e 6672 6f6d         self.from
+0000f670: 5f6a 736f 6e28 7265 736f 7572 6365 3d72  _json(resource=r
+0000f680: 6573 706f 6e73 652e 636f 6e74 656e 742e  esponse.content.
+0000f690: 6465 636f 6465 2829 290a 2020 2020 2020  decode()).      
+0000f6a0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+0000f6b0: 650a 0a20 2020 2064 6566 204d 6174 6368  e..    def Match
+0000f6c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000f6d0: 7265 7320 3d20 7365 6c66 2e67 6574 4668  res = self.getFh
+0000f6e0: 6972 5265 736f 7572 6365 5061 7261 6d65  irResourceParame
+0000f6f0: 7465 7228 290a 2020 2020 2020 2020 7265  ter().        re
+0000f700: 7370 6f6e 7365 203d 2072 6571 7565 7374  sponse = request
+0000f710: 732e 706f 7374 2875 726c 3d73 656c 662e  s.post(url=self.
+0000f720: 7061 7469 656e 745f 6d61 7463 685f 656e  patient_match_en
+0000f730: 6470 6f69 6e74 2e66 6f72 6d61 7428 0a20  dpoint.format(. 
+0000f740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f750: 6765 745f 6668 6972 5f75 726c 2829 292c  get_fhir_url()),
+0000f760: 2064 6174 613d 6a73 6f6e 2e64 756d 7073   data=json.dumps
+0000f770: 2872 6573 292c 2068 6561 6465 7273 3d73  (res), headers=s
+0000f780: 656c 662e 6865 6164 6572 732c 2076 6572  elf.headers, ver
+0000f790: 6966 793d 7365 6c66 2e76 616c 6964 6174  ify=self.validat
+0000f7a0: 655f 6365 7274 7329 0a20 2020 2020 2020  e_certs).       
+0000f7b0: 2069 6620 7265 7370 6f6e 7365 2e73 7461   if response.sta
+0000f7c0: 7475 735f 636f 6465 203d 3d20 3230 303a  tus_code == 200:
+0000f7d0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+0000f7e0: 616d 7320 3d20 5061 7261 6d65 7465 7246  ams = ParameterF
+0000f7f0: 4849 5228 7265 736f 7572 6365 3d6a 736f  HIR(resource=jso
+0000f800: 6e2e 6c6f 6164 7328 7265 7370 6f6e 7365  n.loads(response
+0000f810: 2e63 6f6e 7465 6e74 2e64 6563 6f64 6528  .content.decode(
+0000f820: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+0000f830: 6966 2070 6172 616d 732e 6668 6972 5f72  if params.fhir_r
+0000f840: 6573 6f75 7263 6520 6973 206e 6f74 204e  esource is not N
+0000f850: 6f6e 6520 616e 6420 7061 7261 6d73 2e66  one and params.f
+0000f860: 6869 725f 7265 736f 7572 6365 2e70 6172  hir_resource.par
+0000f870: 616d 6574 6572 2069 7320 6e6f 7420 4e6f  ameter is not No
+0000f880: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000f890: 2020 2020 666f 7220 7061 7261 6d20 696e      for param in
+0000f8a0: 2070 6172 616d 732e 6668 6972 5f72 6573   params.fhir_res
+0000f8b0: 6f75 7263 652e 7061 7261 6d65 7465 723a  ource.parameter:
+0000f8c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f8d0: 2020 2020 2069 6620 7479 7065 2870 6172       if type(par
+0000f8e0: 616d 2e72 6573 6f75 7263 6529 2069 7320  am.resource) is 
+0000f8f0: 5061 7469 656e 743a 0a20 2020 2020 2020  Patient:.       
+0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f910: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
+0000f920: 7263 6520 3d20 7061 7261 6d2e 7265 736f  rce = param.reso
+0000f930: 7572 6365 0a20 2020 2020 2020 2020 2020  urce.           
+0000f940: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f950: 662e 6672 6f6d 5f66 6869 725f 7061 7469  f.from_fhir_pati
+0000f960: 656e 7428 290a 2020 2020 2020 2020 7265  ent().        re
+0000f970: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+0000f980: 2020 2064 6566 2053 6561 7263 6828 7365     def Search(se
+0000f990: 6c66 2c20 6964 656e 7469 6669 6572 3d4e  lf, identifier=N
+0000f9a0: 6f6e 652c 2067 6976 656e 3d4e 6f6e 652c  one, given=None,
+0000f9b0: 2066 616d 696c 793d 4e6f 6e65 2c20 6765   family=None, ge
+0000f9c0: 6e64 6572 3d4e 6f6e 652c 2062 6972 7468  nder=None, birth
+0000f9d0: 6461 7465 3d4e 6f6e 6529 3a0a 2020 2020  date=None):.    
+0000f9e0: 2020 2020 7061 7261 6d73 203d 207b 7d0a      params = {}.
+0000f9f0: 2020 2020 2020 2020 6966 2069 6465 6e74          if ident
+0000fa00: 6966 6965 7220 6973 206e 6f74 204e 6f6e  ifier is not Non
+0000fa10: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+0000fa20: 6172 616d 735b 2769 6465 6e74 6966 6965  arams['identifie
+0000fa30: 7227 5d20 3d20 6964 656e 7469 6669 6572  r'] = identifier
+0000fa40: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
+0000fa50: 6c66 2e6e 616d 2069 7320 6e6f 7420 4e6f  lf.nam is not No
+0000fa60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000fa70: 7061 7261 6d73 5b27 6964 656e 7469 6669  params['identifi
+0000fa80: 6572 275d 203d 2022 636f 6465 3d4e 414d  er'] = "code=NAM
+0000fa90: 7c7b 7d22 2e66 6f72 6d61 7428 7365 6c66  |{}".format(self
+0000faa0: 2e6e 616d 290a 2020 2020 2020 2020 6966  .nam).        if
+0000fab0: 2067 6976 656e 2069 7320 6e6f 7420 4e6f   given is not No
+0000fac0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000fad0: 7061 7261 6d73 5b27 6769 7665 6e27 5d20  params['given'] 
+0000fae0: 3d20 6769 7665 6e0a 2020 2020 2020 2020  = given.        
+0000faf0: 656c 6966 2073 656c 662e 6769 7665 6e5f  elif self.given_
+0000fb00: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
+0000fb10: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+0000fb20: 7261 6d73 5b27 6769 7665 6e27 5d20 3d20  rams['given'] = 
+0000fb30: 7365 6c66 2e67 6976 656e 5f6e 616d 650a  self.given_name.
+0000fb40: 2020 2020 2020 2020 6966 2066 616d 696c          if famil
+0000fb50: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0000fb60: 2020 2020 2020 2020 2020 2070 6172 616d             param
+0000fb70: 735b 2766 616d 696c 7927 5d20 3d20 6661  s['family'] = fa
+0000fb80: 6d69 6c79 0a20 2020 2020 2020 2065 6c69  mily.        eli
+0000fb90: 6620 7365 6c66 2e66 616d 696c 795f 6e61  f self.family_na
+0000fba0: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+0000fbb0: 2020 2020 2020 2020 2020 2020 7061 7261              para
+0000fbc0: 6d73 5b27 6661 6d69 6c79 275d 203d 2073  ms['family'] = s
+0000fbd0: 656c 662e 6661 6d69 6c79 5f6e 616d 650a  elf.family_name.
+0000fbe0: 2020 2020 2020 2020 6966 2067 656e 6465          if gende
+0000fbf0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+0000fc00: 2020 2020 2020 2020 2020 2070 6172 616d             param
+0000fc10: 735b 2767 656e 6465 7227 5d20 3d20 6765  s['gender'] = ge
+0000fc20: 6e64 6572 0a20 2020 2020 2020 2065 6c69  nder.        eli
+0000fc30: 6620 7365 6c66 2e67 656e 6465 7220 6973  f self.gender is
+0000fc40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000fc50: 2020 2020 2020 2070 6172 616d 735b 2767         params['g
+0000fc60: 656e 6465 7227 5d20 3d20 7365 6c66 2e67  ender'] = self.g
+0000fc70: 656e 6465 720a 2020 2020 2020 2020 6966  ender.        if
+0000fc80: 2062 6972 7468 6461 7465 2069 7320 6e6f   birthdate is no
+0000fc90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000fca0: 2020 2020 7061 7261 6d73 5b27 6269 7274      params['birt
+0000fcb0: 6864 6174 6527 5d20 3d20 6269 7274 6864  hdate'] = birthd
+0000fcc0: 6174 650a 2020 2020 2020 2020 656c 6966  ate.        elif
+0000fcd0: 2073 656c 662e 6269 7274 685f 6461 7465   self.birth_date
+0000fce0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000fcf0: 2020 2020 2020 2020 2020 7061 7261 6d73            params
+0000fd00: 5b27 6269 7274 6864 6174 6527 5d20 3d20  ['birthdate'] = 
+0000fd10: 7365 6c66 2e62 6972 7468 5f64 6174 650a  self.birth_date.
+0000fd20: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+0000fd30: 203d 2072 6571 7565 7374 732e 6765 7428   = requests.get(
+0000fd40: 7572 6c3d 7365 6c66 2e70 6174 6965 6e74  url=self.patient
+0000fd50: 5f65 6e64 706f 696e 742e 666f 726d 6174  _endpoint.format
+0000fd60: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000fd70: 6c66 2e67 6574 5f66 6869 725f 7572 6c28  lf.get_fhir_url(
+0000fd80: 2929 2c20 7061 7261 6d73 3d70 6172 616d  )), params=param
+0000fd90: 732c 2068 6561 6465 7273 3d73 656c 662e  s, headers=self.
+0000fda0: 6865 6164 6572 732c 2076 6572 6966 793d  headers, verify=
+0000fdb0: 7365 6c66 2e76 616c 6964 6174 655f 6365  self.validate_ce
+0000fdc0: 7274 7329 0a0a 2020 2020 2020 2020 7265  rts)..        re
+0000fdd0: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+0000fde0: 2020 2064 6566 206e 616d 5f74 6f5f 6964     def nam_to_id
+0000fdf0: 656e 7469 6669 6572 2873 656c 662c 206e  entifier(self, n
+0000fe00: 616d 2c20 636f 6469 6e67 5f73 7973 7465  am, coding_syste
+0000fe10: 6d3d 4e6f 6e65 2c20 636f 6469 6e67 5f76  m=None, coding_v
+0000fe20: 6572 7369 6f6e 3d4e 6f6e 6529 3a0a 2020  ersion=None):.  
+0000fe30: 2020 2020 2020 6e61 6d5f 636f 6469 6e67        nam_coding
+0000fe40: 5f73 7973 7465 6d20 3d20 636f 6469 6e67  _system = coding
+0000fe50: 5f73 7973 7465 6d20 6966 2063 6f64 696e  _system if codin
+0000fe60: 675f 7379 7374 656d 2069 7320 6e6f 7420  g_system is not 
+0000fe70: 4e6f 6e65 2065 6c73 6520 7365 6c66 2e64  None else self.d
+0000fe80: 6566 6175 6c74 5f63 6f64 696e 675f 7379  efault_coding_sy
+0000fe90: 7374 656d 0a20 2020 2020 2020 206e 616d  stem.        nam
+0000fea0: 5f63 6f64 696e 675f 7665 7273 696f 6e20  _coding_version 
+0000feb0: 3d20 636f 6469 6e67 5f73 7973 7465 6d20  = coding_system 
+0000fec0: 6966 2063 6f64 696e 675f 7665 7273 696f  if coding_versio
+0000fed0: 6e20 6973 206e 6f74 204e 6f6e 6520 656c  n is not None el
+0000fee0: 7365 2073 656c 662e 6465 6661 756c 745f  se self.default_
+0000fef0: 636f 6469 6e67 5f76 6572 7369 6f6e 0a20  coding_version. 
+0000ff00: 2020 2020 2020 206e 616d 5f69 6465 6e74         nam_ident
+0000ff10: 6966 6965 7220 3d20 4964 656e 7469 6669  ifier = Identifi
+0000ff20: 6572 2829 0a20 2020 2020 2020 206e 616d  er().        nam
+0000ff30: 5f69 6465 6e74 6966 6965 725f 6578 7465  _identifier_exte
+0000ff40: 6e73 696f 6e20 3d20 4578 7465 6e73 696f  nsion = Extensio
+0000ff50: 6e28 290a 2020 2020 2020 2020 6e61 6d5f  n().        nam_
+0000ff60: 6964 656e 7469 6669 6572 5f65 7874 656e  identifier_exten
+0000ff70: 7369 6f6e 2e75 726c 203d 2073 656c 662e  sion.url = self.
+0000ff80: 6e61 6d5f 6964 656e 7469 6669 6572 5f65  nam_identifier_e
+0000ff90: 7874 656e 7369 6f6e 5f75 726c 0a20 2020  xtension_url.   
+0000ffa0: 2020 2020 206e 616d 5f65 7874 5f63 6f64       nam_ext_cod
+0000ffb0: 6162 6c65 5f63 6f6e 6365 7074 203d 2043  able_concept = C
+0000ffc0: 6f64 6561 626c 6543 6f6e 6365 7074 2829  odeableConcept()
+0000ffd0: 0a20 2020 2020 2020 206e 616d 5f65 7874  .        nam_ext
+0000ffe0: 5f63 6f64 6162 6c65 5f63 6f6e 6365 7074  _codable_concept
+0000fff0: 2e63 6f64 696e 6720 3d20 5b43 6f64 696e  .coding = [Codin
+00010000: 6728 6a73 6f6e 6469 6374 3d7b 2273 7973  g(jsondict={"sys
+00010010: 7465 6d22 3a20 6e61 6d5f 636f 6469 6e67  tem": nam_coding
+00010020: 5f73 7973 7465 6d2c 2276 6572 7369 6f6e  _system,"version
+00010030: 223a 206e 616d 5f63 6f64 696e 675f 7665  ": nam_coding_ve
+00010040: 7273 696f 6e2c 2263 6f64 6522 3a20 2251  rsion,"code": "Q
+00010050: 4322 7d29 5d0a 2020 2020 2020 2020 6e61  C"})].        na
+00010060: 6d5f 6964 656e 7469 6669 6572 5f65 7874  m_identifier_ext
+00010070: 656e 7369 6f6e 2e76 616c 7565 436f 6465  ension.valueCode
+00010080: 6162 6c65 436f 6e63 6570 7420 3d20 6e61  ableConcept = na
+00010090: 6d5f 6578 745f 636f 6461 626c 655f 636f  m_ext_codable_co
+000100a0: 6e63 6570 740a 2020 2020 2020 2020 6e61  ncept.        na
+000100b0: 6d5f 6964 656e 7469 6669 6572 2e65 7874  m_identifier.ext
+000100c0: 656e 7369 6f6e 203d 205b 6e61 6d5f 6964  ension = [nam_id
+000100d0: 656e 7469 6669 6572 5f65 7874 656e 7369  entifier_extensi
+000100e0: 6f6e 5d0a 2020 2020 2020 2020 6e61 6d5f  on].        nam_
+000100f0: 7479 7065 5f63 6f64 6162 6c65 5f63 6f6e  type_codable_con
+00010100: 6365 7074 203d 2043 6f64 6561 626c 6543  cept = CodeableC
+00010110: 6f6e 6365 7074 2829 0a20 2020 2020 2020  oncept().       
+00010120: 206e 616d 5f74 7970 655f 636f 6461 626c   nam_type_codabl
+00010130: 655f 636f 6e63 6570 742e 636f 6469 6e67  e_concept.coding
+00010140: 203d 205b 436f 6469 6e67 286a 736f 6e64   = [Coding(jsond
+00010150: 6963 743d 7b22 7379 7374 656d 223a 206e  ict={"system": n
+00010160: 616d 5f63 6f64 696e 675f 7379 7374 656d  am_coding_system
+00010170: 2c22 7665 7273 696f 6e22 3a20 6e61 6d5f  ,"version": nam_
+00010180: 636f 6469 6e67 5f76 6572 7369 6f6e 2c22  coding_version,"
+00010190: 636f 6465 223a 2022 4e41 4d22 7d29 5d0a  code": "NAM"})].
+000101a0: 2020 2020 2020 2020 6e61 6d5f 6964 656e          nam_iden
+000101b0: 7469 6669 6572 2e74 7970 6520 3d20 6e61  tifier.type = na
+000101c0: 6d5f 7479 7065 5f63 6f64 6162 6c65 5f63  m_type_codable_c
+000101d0: 6f6e 6365 7074 0a20 2020 2020 2020 206e  oncept.        n
+000101e0: 616d 5f69 6465 6e74 6966 6965 722e 7379  am_identifier.sy
+000101f0: 7374 656d 203d 2073 656c 662e 6e61 6d5f  stem = self.nam_
+00010200: 6964 656e 7469 6669 6572 5f73 7973 7465  identifier_syste
+00010210: 6d0a 2020 2020 2020 2020 6e61 6d5f 6964  m.        nam_id
+00010220: 656e 7469 6669 6572 2e76 616c 7565 203d  entifier.value =
+00010230: 206e 616d 0a20 2020 2020 2020 2072 6574   nam.        ret
+00010240: 7572 6e20 6e61 6d5f 6964 656e 7469 6669  urn nam_identifi
+00010250: 6572 0a0a 2020 2020 6465 6620 6e69 755f  er..    def niu_
+00010260: 746f 5f69 6465 6e74 6966 6965 7228 7365  to_identifier(se
+00010270: 6c66 2c20 6e69 752c 2063 6f64 696e 675f  lf, niu, coding_
+00010280: 7379 7374 656d 3d4e 6f6e 652c 2063 6f64  system=None, cod
+00010290: 696e 675f 7665 7273 696f 6e3d 4e6f 6e65  ing_version=None
+000102a0: 293a 0a20 2020 2020 2020 206e 6975 5f63  ):.        niu_c
+000102b0: 6f64 696e 675f 7379 7374 656d 203d 2063  oding_system = c
+000102c0: 6f64 696e 675f 7379 7374 656d 2069 6620  oding_system if 
+000102d0: 636f 6469 6e67 5f73 7973 7465 6d20 6973  coding_system is
+000102e0: 206e 6f74 204e 6f6e 6520 656c 7365 2073   not None else s
+000102f0: 656c 662e 6465 6661 756c 745f 636f 6469  elf.default_codi
+00010300: 6e67 5f73 7973 7465 6d0a 2020 2020 2020  ng_system.      
+00010310: 2020 6e69 755f 636f 6469 6e67 5f76 6572    niu_coding_ver
+00010320: 7369 6f6e 203d 2063 6f64 696e 675f 7379  sion = coding_sy
+00010330: 7374 656d 2069 6620 636f 6469 6e67 5f76  stem if coding_v
+00010340: 6572 7369 6f6e 2069 7320 6e6f 7420 4e6f  ersion is not No
+00010350: 6e65 2065 6c73 6520 7365 6c66 2e64 6566  ne else self.def
+00010360: 6175 6c74 5f63 6f64 696e 675f 7665 7273  ault_coding_vers
+00010370: 696f 6e0a 2020 2020 2020 2020 6e69 755f  ion.        niu_
+00010380: 6964 656e 7469 6669 6572 203d 2049 6465  identifier = Ide
+00010390: 6e74 6966 6965 7228 290a 2020 2020 2020  ntifier().      
+000103a0: 2020 6e69 755f 7479 7065 5f63 6f64 6162    niu_type_codab
+000103b0: 6c65 5f63 6f6e 6365 7074 203d 2043 6f64  le_concept = Cod
+000103c0: 6561 626c 6543 6f6e 6365 7074 2829 0a20  eableConcept(). 
+000103d0: 2020 2020 2020 206e 6975 5f74 7970 655f         niu_type_
+000103e0: 636f 6461 626c 655f 636f 6e63 6570 742e  codable_concept.
+000103f0: 636f 6469 6e67 203d 205b 436f 6469 6e67  coding = [Coding
+00010400: 286a 736f 6e64 6963 743d 7b22 7379 7374  (jsondict={"syst
+00010410: 656d 223a 206e 6975 5f63 6f64 696e 675f  em": niu_coding_
+00010420: 7379 7374 656d 2c22 7665 7273 696f 6e22  system,"version"
+00010430: 3a20 6e69 755f 636f 6469 6e67 5f76 6572  : niu_coding_ver
+00010440: 7369 6f6e 2c22 636f 6465 223a 2022 4e49  sion,"code": "NI
+00010450: 5555 222c 2264 6973 706c 6179 223a 224e  UU","display":"N
+00010460: 4955 227d 295d 0a20 2020 2020 2020 206e  IU"})].        n
+00010470: 6975 5f69 6465 6e74 6966 6965 722e 7479  iu_identifier.ty
+00010480: 7065 203d 206e 6975 5f74 7970 655f 636f  pe = niu_type_co
+00010490: 6461 626c 655f 636f 6e63 6570 740a 2020  dable_concept.  
+000104a0: 2020 2020 2020 6e69 755f 6964 656e 7469        niu_identi
+000104b0: 6669 6572 2e76 616c 7565 203d 206e 6975  fier.value = niu
+000104c0: 0a20 2020 2020 2020 206e 6975 5f69 6465  .        niu_ide
+000104d0: 6e74 6966 6965 722e 7379 7374 656d 203d  ntifier.system =
+000104e0: 2073 656c 662e 6e69 755f 6964 656e 7469   self.niu_identi
+000104f0: 6669 6572 5f73 7973 7465 6d0a 2020 2020  fier_system.    
+00010500: 2020 2020 7265 7475 726e 206e 6975 5f69      return niu_i
+00010510: 6465 6e74 6966 6965 720a 0a20 2020 2064  dentifier..    d
+00010520: 6566 2061 7563 756e 5f69 6465 6e74 6966  ef aucun_identif
+00010530: 6961 6e74 5f74 6f5f 6964 656e 7469 6669  iant_to_identifi
+00010540: 6572 2873 656c 662c 2063 6f64 696e 675f  er(self, coding_
+00010550: 7379 7374 656d 3d4e 6f6e 652c 2063 6f64  system=None, cod
+00010560: 696e 675f 7665 7273 696f 6e3d 4e6f 6e65  ing_version=None
+00010570: 293a 0a20 2020 2020 2020 2063 6f64 696e  ):.        codin
+00010580: 675f 7379 7374 656d 203d 2063 6f64 696e  g_system = codin
+00010590: 675f 7379 7374 656d 2069 6620 636f 6469  g_system if codi
+000105a0: 6e67 5f73 7973 7465 6d20 6973 206e 6f74  ng_system is not
+000105b0: 204e 6f6e 6520 656c 7365 2073 656c 662e   None else self.
+000105c0: 6465 6661 756c 745f 636f 6469 6e67 5f73  default_coding_s
+000105d0: 7973 7465 6d0a 2020 2020 2020 2020 636f  ystem.        co
+000105e0: 6469 6e67 5f76 6572 7369 6f6e 203d 2063  ding_version = c
+000105f0: 6f64 696e 675f 7379 7374 656d 2069 6620  oding_system if 
+00010600: 636f 6469 6e67 5f76 6572 7369 6f6e 2069  coding_version i
+00010610: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00010620: 7365 6c66 2e64 6566 6175 6c74 5f63 6f64  self.default_cod
+00010630: 696e 675f 7665 7273 696f 6e0a 2020 2020  ing_version.    
+00010640: 2020 2020 6175 6375 6e5f 6964 656e 7469      aucun_identi
+00010650: 6669 6572 203d 2049 6465 6e74 6966 6965  fier = Identifie
+00010660: 7228 290a 2020 2020 2020 2020 6175 6375  r().        aucu
+00010670: 6e5f 7479 7065 5f63 6f64 6162 6c65 5f63  n_type_codable_c
+00010680: 6f6e 6365 7074 203d 2043 6f64 6561 626c  oncept = Codeabl
+00010690: 6543 6f6e 6365 7074 2829 0a20 2020 2020  eConcept().     
+000106a0: 2020 2061 7563 756e 5f74 7970 655f 636f     aucun_type_co
+000106b0: 6461 626c 655f 636f 6e63 6570 742e 636f  dable_concept.co
+000106c0: 6469 6e67 203d 205b 436f 6469 6e67 286a  ding = [Coding(j
+000106d0: 736f 6e64 6963 743d 7b22 7379 7374 656d  sondict={"system
+000106e0: 223a 2063 6f64 696e 675f 7379 7374 656d  ": coding_system
+000106f0: 2c22 7665 7273 696f 6e22 3a20 636f 6469  ,"version": codi
+00010700: 6e67 5f76 6572 7369 6f6e 2c22 636f 6465  ng_version,"code
+00010710: 223a 2022 4155 4355 4e22 2c22 6469 7370  ": "AUCUN","disp
+00010720: 6c61 7922 3a22 4175 6375 6e20 6964 656e  lay":"Aucun iden
+00010730: 7469 6669 616e 7422 7d29 5d0a 2020 2020  tifiant"})].    
+00010740: 2020 2020 6175 6375 6e5f 6964 656e 7469      aucun_identi
+00010750: 6669 6572 2e74 7970 6520 3d20 6175 6375  fier.type = aucu
+00010760: 6e5f 7479 7065 5f63 6f64 6162 6c65 5f63  n_type_codable_c
+00010770: 6f6e 6365 7074 0a20 2020 2020 2020 2061  oncept.        a
+00010780: 7563 756e 5f69 6465 6e74 6966 6965 722e  ucun_identifier.
+00010790: 7379 7374 656d 203d 2073 656c 662e 6175  system = self.au
+000107a0: 6375 6e5f 6964 656e 7469 6669 6572 5f73  cun_identifier_s
+000107b0: 7973 7465 6d0a 2020 2020 2020 2020 7265  ystem.        re
+000107c0: 7475 726e 2061 7563 756e 5f69 6465 6e74  turn aucun_ident
+000107d0: 6966 6965 720a 0a20 2020 2064 6566 2067  ifier..    def g
+000107e0: 6976 656e 5f66 616d 696c 795f 746f 5f68  iven_family_to_h
+000107f0: 756d 616e 5f6e 616d 6528 7365 6c66 2c20  uman_name(self, 
+00010800: 6769 7665 6e5f 6e61 6d65 3d4e 6f6e 652c  given_name=None,
+00010810: 2066 616d 696c 795f 6e61 6d65 3d4e 6f6e   family_name=Non
+00010820: 6529 3a0a 2020 2020 2020 2020 686e 203d  e):.        hn =
+00010830: 2048 756d 616e 4e61 6d65 2829 0a20 2020   HumanName().   
+00010840: 2020 2020 2068 6e2e 6769 7665 6e20 3d20       hn.given = 
+00010850: 5b67 6976 656e 5f6e 616d 655d 0a20 2020  [given_name].   
+00010860: 2020 2020 2068 6e2e 6661 6d69 6c79 203d       hn.family =
+00010870: 205b 6661 6d69 6c79 5f6e 616d 655d 0a20   [family_name]. 
+00010880: 2020 2020 2020 2072 6574 7572 6e20 686e         return hn
+00010890: 0a0a 2020 2020 6465 6620 7374 725f 6461  ..    def str_da
+000108a0: 7465 5f74 6f5f 6668 6972 5f64 6174 6528  te_to_fhir_date(
+000108b0: 7365 6c66 2c20 7374 725f 6461 7465 293a  self, str_date):
+000108c0: 0a20 2020 2020 2020 2066 6869 725f 6461  .        fhir_da
+000108d0: 7465 2020 3d20 4648 4952 4461 7465 2829  te  = FHIRDate()
+000108e0: 0a20 2020 2020 2020 2066 6869 725f 6461  .        fhir_da
+000108f0: 7465 2e64 6174 6520 3d20 6461 7465 7469  te.date = dateti
+00010900: 6d65 2e73 7472 7074 696d 6528 7374 725f  me.strptime(str_
+00010910: 6461 7465 2c20 2725 592d 256d 2d25 6427  date, '%Y-%m-%d'
+00010920: 292e 6461 7465 2829 0a20 2020 2020 2020  ).date().       
+00010930: 2072 6574 7572 6e20 6668 6972 5f64 6174   return fhir_dat
+00010940: 650a 0a20 2020 2064 6566 2066 6869 725f  e..    def fhir_
+00010950: 6461 7465 5f74 6f5f 7374 725f 6461 7465  date_to_str_date
+00010960: 2873 656c 662c 2066 6869 725f 6461 7465  (self, fhir_date
+00010970: 293a 0a20 2020 2020 2020 2073 7472 5f64  ):.        str_d
+00010980: 6174 6520 3d20 4e6f 6e65 0a20 2020 2020  ate = None.     
+00010990: 2020 2069 6620 6668 6972 5f64 6174 6520     if fhir_date 
+000109a0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+000109b0: 6668 6972 5f64 6174 652e 6461 7465 2069  fhir_date.date i
+000109c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000109d0: 2020 2020 2020 2020 7374 725f 6461 7465          str_date
+000109e0: 203d 2066 6869 725f 6461 7465 2e69 736f   = fhir_date.iso
+000109f0: 7374 7269 6e67 0a20 2020 2020 2020 2072  string.        r
+00010a00: 6574 7572 6e20 7374 725f 6461 7465 0a0a  eturn str_date..
+00010a10: 2020 2020 6465 6620 7365 745f 6964 2873      def set_id(s
+00010a20: 656c 662c 2069 642c 2070 6174 6965 6e74  elf, id, patient
+00010a30: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00010a40: 6966 2070 6174 6965 6e74 2069 7320 4e6f  if patient is No
+00010a50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00010a60: 7061 7469 656e 7420 3d20 7365 6c66 2e66  patient = self.f
+00010a70: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
+00010a80: 2020 2020 2020 2020 2073 656c 662e 6964           self.id
+00010a90: 203d 2069 640a 2020 2020 2020 2020 7061   = id.        pa
+00010aa0: 7469 656e 742e 6964 203d 2069 640a 0a20  tient.id = id.. 
+00010ab0: 2020 2064 6566 2067 6574 5f69 6428 7365     def get_id(se
+00010ac0: 6c66 2c20 7061 7469 656e 743d 4e6f 6e65  lf, patient=None
+00010ad0: 293a 0a20 2020 2020 2020 2069 6620 7061  ):.        if pa
+00010ae0: 7469 656e 7420 6973 204e 6f6e 653a 0a20  tient is None:. 
+00010af0: 2020 2020 2020 2020 2020 2070 6174 6965             patie
+00010b00: 6e74 203d 2073 656c 662e 6668 6972 5f72  nt = self.fhir_r
+00010b10: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
+00010b20: 7265 7475 726e 2070 6174 6965 6e74 2e69  return patient.i
+00010b30: 640a 0a20 2020 2064 6566 2073 6574 5f6d  d..    def set_m
+00010b40: 6174 6368 7261 6d71 2873 656c 662c 206d  atchramq(self, m
+00010b50: 6174 6368 7261 6d71 3d46 616c 7365 2c20  atchramq=False, 
+00010b60: 7061 7469 656e 743d 4e6f 6e65 293a 0a20  patient=None):. 
+00010b70: 2020 2020 2020 2069 6620 7479 7065 286d         if type(m
+00010b80: 6174 6368 7261 6d71 2920 6973 2062 6f6f  atchramq) is boo
+00010b90: 6c3a 0a20 2020 2020 2020 2020 2020 2062  l:.            b
+00010ba0: 6f6f 6c5f 6d61 7463 6872 616d 7120 3d20  ool_matchramq = 
+00010bb0: 6d61 7463 6872 616d 710a 2020 2020 2020  matchramq.      
+00010bc0: 2020 656c 6966 2074 7970 6528 6d61 7463    elif type(matc
+00010bd0: 6872 616d 7129 2069 7320 7374 723a 0a20  hramq) is str:. 
+00010be0: 2020 2020 2020 2020 2020 2062 6f6f 6c5f             bool_
+00010bf0: 6d61 7463 6872 616d 7120 3d20 626f 6f6c  matchramq = bool
+00010c00: 2873 7472 3262 6f6f 6c28 6d61 7463 6872  (str2bool(matchr
+00010c10: 616d 7129 290a 2020 2020 2020 2020 656c  amq)).        el
+00010c20: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00010c30: 626f 6f6c 5f6d 6174 6368 7261 6d71 203d  bool_matchramq =
+00010c40: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
+00010c50: 6620 7061 7469 656e 7420 6973 204e 6f6e  f patient is Non
+00010c60: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00010c70: 6174 6965 6e74 203d 2073 656c 662e 6668  atient = self.fh
+00010c80: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
+00010c90: 2020 2020 6d61 7463 6872 616d 715f 6578      matchramq_ex
+00010ca0: 7465 6e73 696f 6e20 3d20 4578 7465 6e73  tension = Extens
+00010cb0: 696f 6e28 290a 2020 2020 2020 2020 6d61  ion().        ma
+00010cc0: 7463 6872 616d 715f 6578 7465 6e73 696f  tchramq_extensio
+00010cd0: 6e2e 7572 6c20 3d20 7365 6c66 2e6d 6174  n.url = self.mat
+00010ce0: 6368 7261 6d71 5f65 7874 656e 7369 6f6e  chramq_extension
+00010cf0: 5f75 726c 0a20 2020 2020 2020 206d 6174  _url.        mat
+00010d00: 6368 7261 6d71 5f65 7874 656e 7369 6f6e  chramq_extension
+00010d10: 2e76 616c 7565 426f 6f6c 6561 6e20 3d20  .valueBoolean = 
+00010d20: 626f 6f6c 5f6d 6174 6368 7261 6d71 0a0a  bool_matchramq..
+00010d30: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
+00010d40: 6e74 2e65 7874 656e 7369 6f6e 2069 7320  nt.extension is 
+00010d50: 4e6f 6e65 3a20 2020 200a 2020 2020 2020  None:    .      
+00010d60: 2020 2020 2020 7061 7469 656e 742e 6578        patient.ex
+00010d70: 7465 6e73 696f 6e20 3d20 5b6d 6174 6368  tension = [match
+00010d80: 7261 6d71 5f65 7874 656e 7369 6f6e 5d0a  ramq_extension].
+00010d90: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00010da0: 2020 2020 2020 2020 2020 6578 7465 6e73            extens
+00010db0: 696f 6e5f 666f 756e 6420 3d20 4661 6c73  ion_found = Fals
+00010dc0: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
+00010dd0: 7220 6578 7420 696e 2070 6174 6965 6e74  r ext in patient
+00010de0: 2e65 7874 656e 7369 6f6e 3a0a 2020 2020  .extension:.    
+00010df0: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+00010e00: 7874 2e75 726c 203d 3d20 7365 6c66 2e6d  xt.url == self.m
+00010e10: 6174 6368 7261 6d71 5f65 7874 656e 7369  atchramq_extensi
+00010e20: 6f6e 5f75 726c 3a0a 2020 2020 2020 2020  on_url:.        
+00010e30: 2020 2020 2020 2020 2020 2020 6578 7465              exte
+00010e40: 6e73 696f 6e5f 666f 756e 6420 3d20 5472  nsion_found = Tr
+00010e50: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00010e60: 2020 2020 2020 2065 7874 2e76 616c 7565         ext.value
+00010e70: 426f 6f6c 6561 6e20 3d20 626f 6f6c 5f6d  Boolean = bool_m
+00010e80: 6174 6368 7261 6d71 0a20 2020 2020 2020  atchramq.       
+00010e90: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00010ea0: 616b 0a20 2020 2020 2020 2020 2020 2069  ak.            i
+00010eb0: 6620 6e6f 7420 6578 7465 6e73 696f 6e5f  f not extension_
+00010ec0: 666f 756e 643a 0a20 2020 2020 2020 2020  found:.         
+00010ed0: 2020 2020 2020 2070 6174 6965 6e74 2e65         patient.e
+00010ee0: 7874 656e 7369 6f6e 2e61 7070 656e 6428  xtension.append(
+00010ef0: 6d61 7463 6872 616d 715f 6578 7465 6e73  matchramq_extens
+00010f00: 696f 6e29 0a0a 2020 2020 6465 6620 6765  ion)..    def ge
+00010f10: 745f 6d61 7463 6872 616d 7128 7365 6c66  t_matchramq(self
+00010f20: 2c20 7061 7469 656e 743d 4e6f 6e65 293a  , patient=None):
+00010f30: 0a20 2020 2020 2020 206d 6174 6368 7261  .        matchra
+00010f40: 6d71 203d 2046 616c 7365 0a20 2020 2020  mq = False.     
+00010f50: 2020 2069 6620 7061 7469 656e 742e 6578     if patient.ex
+00010f60: 7465 6e73 696f 6e20 6973 206e 6f74 204e  tension is not N
+00010f70: 6f6e 653a 2020 2020 0a20 2020 2020 2020  one:    .       
+00010f80: 2020 2020 2066 6f72 2065 7874 2069 6e20       for ext in 
+00010f90: 7061 7469 656e 742e 6578 7465 6e73 696f  patient.extensio
+00010fa0: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
+00010fb0: 2020 2069 6620 6578 742e 7572 6c20 3d3d     if ext.url ==
+00010fc0: 2073 656c 662e 6d61 7463 6872 616d 715f   self.matchramq_
+00010fd0: 6578 7465 6e73 696f 6e5f 7572 6c3a 0a20  extension_url:. 
+00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ff0: 2020 2072 6574 7572 6e20 6578 742e 7661     return ext.va
+00011000: 6c75 6542 6f6f 6c65 616e 0a20 2020 2020  lueBoolean.     
+00011010: 2020 2072 6574 7572 6e20 6d61 7463 6872     return matchr
+00011020: 616d 7120 2020 2020 2020 200a 0a20 2020  amq        ..   
+00011030: 2064 6566 2073 6574 5f61 6374 6976 6528   def set_active(
+00011040: 7365 6c66 2c20 6163 7469 7665 2c20 7061  self, active, pa
+00011050: 7469 656e 743d 4e6f 6e65 293a 0a20 2020  tient=None):.   
+00011060: 2020 2020 2069 6620 7061 7469 656e 7420       if patient 
+00011070: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00011080: 2020 2020 2070 6174 6965 6e74 203d 2073       patient = s
+00011090: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+000110a0: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+000110b0: 6c66 2e61 6374 6976 6520 3d20 6163 7469  lf.active = acti
+000110c0: 7665 0a20 2020 2020 2020 2070 6174 6965  ve.        patie
+000110d0: 6e74 2e61 6374 6976 6520 3d20 6163 7469  nt.active = acti
+000110e0: 7665 0a0a 2020 2020 6465 6620 6765 745f  ve..    def get_
+000110f0: 6163 7469 7665 2873 656c 662c 2070 6174  active(self, pat
+00011100: 6965 6e74 3d4e 6f6e 6529 3a0a 2020 2020  ient=None):.    
+00011110: 2020 2020 6966 2070 6174 6965 6e74 2069      if patient i
+00011120: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00011130: 2020 2020 7061 7469 656e 7420 3d20 7365      patient = se
+00011140: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+00011150: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011160: 7061 7469 656e 742e 6163 7469 7665 0a0a  patient.active..
+00011170: 2020 2020 6465 6620 7365 745f 6e61 6d65      def set_name
+00011180: 2873 656c 662c 2067 6976 656e 5f6e 616d  (self, given_nam
+00011190: 653d 4e6f 6e65 2c20 6661 6d69 6c79 5f6e  e=None, family_n
+000111a0: 616d 653d 4e6f 6e65 2c20 7061 7469 656e  ame=None, patien
+000111b0: 743d 4e6f 6e65 293a 0a20 2020 2020 2020  t=None):.       
+000111c0: 2069 6620 7061 7469 656e 7420 6973 204e   if patient is N
+000111d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000111e0: 2070 6174 6965 6e74 203d 2073 656c 662e   patient = self.
+000111f0: 6668 6972 5f72 6573 6f75 7263 650a 2020  fhir_resource.  
+00011200: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00011210: 6976 656e 5f6e 616d 6520 3d20 6769 7665  iven_name = give
+00011220: 6e5f 6e61 6d65 0a20 2020 2020 2020 2020  n_name.         
+00011230: 2020 2073 656c 662e 6661 6d69 6c79 5f6e     self.family_n
+00011240: 616d 6520 3d20 6661 6d69 6c79 5f6e 616d  ame = family_nam
+00011250: 650a 2020 2020 2020 2020 686e 203d 2073  e.        hn = s
+00011260: 656c 662e 6769 7665 6e5f 6661 6d69 6c79  elf.given_family
+00011270: 5f74 6f5f 6875 6d61 6e5f 6e61 6d65 2867  _to_human_name(g
+00011280: 6976 656e 5f6e 616d 653d 6769 7665 6e5f  iven_name=given_
+00011290: 6e61 6d65 2c20 6661 6d69 6c79 5f6e 616d  name, family_nam
+000112a0: 653d 6661 6d69 6c79 5f6e 616d 6529 0a20  e=family_name). 
+000112b0: 2020 2020 2020 2069 6620 7061 7469 656e         if patien
+000112c0: 742e 6e61 6d65 2069 7320 4e6f 6e65 3a0a  t.name is None:.
+000112d0: 2020 2020 2020 2020 2020 2020 7061 7469              pati
+000112e0: 656e 742e 6e61 6d65 203d 205b 686e 5d0a  ent.name = [hn].
+000112f0: 0a20 2020 2064 6566 2067 6574 5f6e 616d  .    def get_nam
+00011300: 6528 7365 6c66 2c20 696e 6465 783d 302c  e(self, index=0,
+00011310: 2070 6174 6965 6e74 3d4e 6f6e 6529 3a0a   patient=None):.
+00011320: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
+00011330: 6e74 2069 7320 4e6f 6e65 3a0a 2020 2020  nt is None:.    
+00011340: 2020 2020 2020 2020 7061 7469 656e 7420          patient 
+00011350: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
+00011360: 7572 6365 0a0a 2020 2020 2020 2020 7265  urce..        re
+00011370: 7475 726e 2070 6174 6965 6e74 2e6e 616d  turn patient.nam
+00011380: 655b 696e 6465 785d 0a0a 2020 2020 6465  e[index]..    de
+00011390: 6620 6765 745f 6769 7665 6e5f 6e61 6d65  f get_given_name
+000113a0: 2873 656c 662c 2069 6e64 6578 3d30 2c20  (self, index=0, 
+000113b0: 7061 7469 656e 743d 4e6f 6e65 293a 0a20  patient=None):. 
+000113c0: 2020 2020 2020 2069 6620 7061 7469 656e         if patien
+000113d0: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+000113e0: 2020 2020 2020 2070 6174 6965 6e74 203d         patient =
+000113f0: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
+00011400: 7263 650a 0a20 2020 2020 2020 2067 6976  rce..        giv
+00011410: 656e 5f6e 616d 6520 3d20 4e6f 6e65 0a20  en_name = None. 
+00011420: 2020 2020 2020 2069 6620 7061 7469 656e         if patien
+00011430: 742e 6e61 6d65 2069 7320 6e6f 7420 4e6f  t.name is not No
+00011440: 6e65 2061 6e64 206c 656e 2870 6174 6965  ne and len(patie
+00011450: 6e74 2e6e 616d 6529 203e 2030 2061 6e64  nt.name) > 0 and
+00011460: 206c 656e 2870 6174 6965 6e74 2e6e 616d   len(patient.nam
+00011470: 655b 696e 6465 785d 2e67 6976 656e 2920  e[index].given) 
+00011480: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+00011490: 2067 6976 656e 5f6e 616d 6520 3d20 7061   given_name = pa
+000114a0: 7469 656e 742e 6e61 6d65 5b69 6e64 6578  tient.name[index
+000114b0: 5d2e 6769 7665 6e5b 696e 6465 785d 0a20  ].given[index]. 
+000114c0: 2020 2020 2020 2072 6574 7572 6e20 6769         return gi
+000114d0: 7665 6e5f 6e61 6d65 0a0a 2020 2020 6465  ven_name..    de
+000114e0: 6620 6765 745f 6661 6d69 6c79 5f6e 616d  f get_family_nam
+000114f0: 6528 7365 6c66 2c20 696e 6465 783d 302c  e(self, index=0,
+00011500: 2070 6174 6965 6e74 3d4e 6f6e 6529 3a0a   patient=None):.
+00011510: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
+00011520: 6e74 2069 7320 4e6f 6e65 3a0a 2020 2020  nt is None:.    
+00011530: 2020 2020 2020 2020 7061 7469 656e 7420          patient 
+00011540: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
+00011550: 7572 6365 0a20 2020 2020 2020 2066 616d  urce.        fam
+00011560: 696c 795f 6e61 6d65 203d 204e 6f6e 650a  ily_name = None.
+00011570: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
+00011580: 6e74 2e6e 616d 6520 6973 206e 6f74 204e  nt.name is not N
+00011590: 6f6e 6520 616e 6420 6c65 6e28 7061 7469  one and len(pati
+000115a0: 656e 742e 6e61 6d65 2920 3e20 3020 616e  ent.name) > 0 an
+000115b0: 6420 6c65 6e28 7061 7469 656e 742e 6e61  d len(patient.na
+000115c0: 6d65 5b69 6e64 6578 5d2e 6661 6d69 6c79  me[index].family
+000115d0: 2920 3e20 303a 0a20 2020 2020 2020 2020  ) > 0:.         
+000115e0: 2020 2066 616d 696c 795f 6e61 6d65 203d     family_name =
+000115f0: 2070 6174 6965 6e74 2e6e 616d 655b 696e   patient.name[in
+00011600: 6465 785d 2e66 616d 696c 795b 696e 6465  dex].family[inde
+00011610: 785d 0a20 2020 2020 2020 2072 6574 7572  x].        retur
+00011620: 6e20 6661 6d69 6c79 5f6e 616d 650a 0a20  n family_name.. 
+00011630: 2020 2064 6566 2073 6574 5f67 656e 6465     def set_gende
+00011640: 7228 7365 6c66 2c20 6765 6e64 6572 2c20  r(self, gender, 
+00011650: 7061 7469 656e 743d 4e6f 6e65 293a 0a20  patient=None):. 
+00011660: 2020 2020 2020 2069 6620 7061 7469 656e         if patien
+00011670: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+00011680: 2020 2020 2020 2070 6174 6965 6e74 203d         patient =
+00011690: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
+000116a0: 7263 650a 2020 2020 2020 2020 2020 2020  rce.            
+000116b0: 7365 6c66 2e67 656e 6465 7220 3d20 6765  self.gender = ge
+000116c0: 6e64 6572 0a0a 2020 2020 2020 2020 7061  nder..        pa
+000116d0: 7469 656e 742e 6765 6e64 6572 203d 2067  tient.gender = g
+000116e0: 656e 6465 720a 0a20 2020 2064 6566 2067  ender..    def g
+000116f0: 6574 5f67 656e 6465 7228 7365 6c66 2c20  et_gender(self, 
+00011700: 7061 7469 656e 743d 4e6f 6e65 293a 0a20  patient=None):. 
+00011710: 2020 2020 2020 2069 6620 7061 7469 656e         if patien
+00011720: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+00011730: 2020 2020 2020 2070 6174 6965 6e74 203d         patient =
+00011740: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
+00011750: 7263 650a 0a20 2020 2020 2020 2072 6574  rce..        ret
+00011760: 7572 6e20 7061 7469 656e 742e 6765 6e64  urn patient.gend
+00011770: 6572 0a0a 2020 2020 6465 6620 7365 745f  er..    def set_
+00011780: 6e61 6d28 7365 6c66 2c20 6e61 6d2c 2070  nam(self, nam, p
+00011790: 6174 6965 6e74 3d4e 6f6e 652c 2063 6f64  atient=None, cod
+000117a0: 696e 675f 7379 7374 656d 3d4e 6f6e 652c  ing_system=None,
+000117b0: 2063 6f64 696e 675f 7665 7273 696f 6e3d   coding_version=
+000117c0: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
+000117d0: 6620 7061 7469 656e 7420 6973 204e 6f6e  f patient is Non
+000117e0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+000117f0: 6174 6965 6e74 203d 2073 656c 662e 6668  atient = self.fh
+00011800: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
+00011810: 2020 2020 2020 2020 7365 6c66 2e6e 616d          self.nam
+00011820: 203d 206e 616d 0a20 2020 2020 2020 206e   = nam.        n
+00011830: 616d 5f69 6465 6e74 6966 6965 7220 3d20  am_identifier = 
+00011840: 7365 6c66 2e6e 616d 5f74 6f5f 6964 656e  self.nam_to_iden
+00011850: 7469 6669 6572 286e 616d 3d6e 616d 2c20  tifier(nam=nam, 
+00011860: 636f 6469 6e67 5f73 7973 7465 6d3d 636f  coding_system=co
+00011870: 6469 6e67 5f73 7973 7465 6d2c 2063 6f64  ding_system, cod
+00011880: 696e 675f 7665 7273 696f 6e3d 636f 6469  ing_version=codi
+00011890: 6e67 5f76 6572 7369 6f6e 290a 2020 2020  ng_version).    
+000118a0: 2020 2020 6966 2070 6174 6965 6e74 2e69      if patient.i
+000118b0: 6465 6e74 6966 6965 7220 6973 204e 6f6e  dentifier is Non
+000118c0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+000118d0: 6174 6965 6e74 2e69 6465 6e74 6966 6965  atient.identifie
+000118e0: 7220 3d20 5b6e 616d 5f69 6465 6e74 6966  r = [nam_identif
+000118f0: 6965 725d 0a20 2020 2020 2020 2065 6c73  ier].        els
+00011900: 653a 0a20 2020 2020 2020 2020 2020 206e  e:.            n
+00011910: 616d 5f69 6465 6e74 6966 6965 725f 666f  am_identifier_fo
+00011920: 756e 6420 3d20 4661 6c73 650a 2020 2020  und = False.    
+00011930: 2020 2020 2020 2020 666f 7220 6964 656e          for iden
+00011940: 7469 6669 6572 2069 6e20 7061 7469 656e  tifier in patien
+00011950: 742e 6964 656e 7469 6669 6572 3a0a 2020  t.identifier:.  
+00011960: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011970: 2069 6465 6e74 6966 6965 722e 7379 7374   identifier.syst
+00011980: 656d 203d 3d20 7365 6c66 2e6e 616d 5f69  em == self.nam_i
+00011990: 6465 6e74 6966 6965 725f 7379 7374 656d  dentifier_system
+000119a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000119b0: 2020 2020 2020 6964 656e 7469 6669 6572        identifier
+000119c0: 2e76 616c 7565 203d 206e 616d 0a20 2020  .value = nam.   
+000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119e0: 206e 616d 5f69 6465 6e74 6966 6965 725f   nam_identifier_
+000119f0: 666f 756e 6420 3d20 5472 7565 0a20 2020  found = True.   
+00011a00: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00011a10: 6e61 6d5f 6964 656e 7469 6669 6572 5f66  nam_identifier_f
+00011a20: 6f75 6e64 2061 6e64 206e 616d 5f69 6465  ound and nam_ide
+00011a30: 6e74 6966 6965 7220 6973 206e 6f74 204e  ntifier is not N
+00011a40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00011a50: 2020 2020 2070 6174 6965 6e74 2e69 6465       patient.ide
+00011a60: 6e74 6966 6965 722e 6170 7065 6e64 286e  ntifier.append(n
+00011a70: 616d 5f69 6465 6e74 6966 6965 7229 0a0a  am_identifier)..
+00011a80: 2020 2020 6465 6620 6765 745f 6e61 6d28      def get_nam(
+00011a90: 7365 6c66 2c20 7061 7469 656e 743d 4e6f  self, patient=No
+00011aa0: 6e65 293a 0a20 2020 2020 2020 206e 616d  ne):.        nam
+00011ab0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00011ac0: 6966 2070 6174 6965 6e74 2069 7320 4e6f  if patient is No
+00011ad0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00011ae0: 7061 7469 656e 7420 3d20 7365 6c66 2e66  patient = self.f
+00011af0: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
+00011b00: 2020 2020 2069 6620 7061 7469 656e 742e       if patient.
+00011b10: 6964 656e 7469 6669 6572 2069 7320 6e6f  identifier is no
+00011b20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00011b30: 2020 2020 666f 7220 6964 656e 7469 6669      for identifi
+00011b40: 6572 2069 6e20 7061 7469 656e 742e 6964  er in patient.id
+00011b50: 656e 7469 6669 6572 3a0a 2020 2020 2020  entifier:.      
+00011b60: 2020 2020 2020 2020 2020 6966 2069 6465            if ide
+00011b70: 6e74 6966 6965 722e 7379 7374 656d 203d  ntifier.system =
+00011b80: 3d20 7365 6c66 2e6e 616d 5f69 6465 6e74  = self.nam_ident
+00011b90: 6966 6965 725f 7379 7374 656d 3a0a 2020  ifier_system:.  
+00011ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bb0: 2020 6e61 6d20 3d20 6964 656e 7469 6669    nam = identifi
+00011bc0: 6572 2e76 616c 7565 0a20 2020 2020 2020  er.value.       
+00011bd0: 2072 6574 7572 6e20 6e61 6d0a 0a20 2020   return nam..   
+00011be0: 2064 6566 2073 6574 5f6e 6975 2873 656c   def set_niu(sel
+00011bf0: 662c 206e 6975 2c20 7061 7469 656e 743d  f, niu, patient=
+00011c00: 4e6f 6e65 2c20 636f 6469 6e67 5f73 7973  None, coding_sys
+00011c10: 7465 6d3d 4e6f 6e65 2c20 636f 6469 6e67  tem=None, coding
+00011c20: 5f76 6572 7369 6f6e 3d4e 6f6e 6529 3a0a  _version=None):.
+00011c30: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
+00011c40: 6e74 2069 7320 4e6f 6e65 3a0a 2020 2020  nt is None:.    
+00011c50: 2020 2020 2020 2020 7061 7469 656e 7420          patient 
+00011c60: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
+00011c70: 7572 6365 0a20 2020 2020 2020 2020 2020  urce.           
+00011c80: 2073 656c 662e 6e69 7520 3d20 6e69 750a   self.niu = niu.
+00011c90: 0a20 2020 2020 2020 206e 6975 5f69 6465  .        niu_ide
+00011ca0: 6e74 6966 6965 7220 3d20 7365 6c66 2e6e  ntifier = self.n
+00011cb0: 6975 5f74 6f5f 6964 656e 7469 6669 6572  iu_to_identifier
+00011cc0: 286e 6975 3d6e 6975 2c20 636f 6469 6e67  (niu=niu, coding
+00011cd0: 5f73 7973 7465 6d3d 636f 6469 6e67 5f73  _system=coding_s
+00011ce0: 7973 7465 6d2c 2063 6f64 696e 675f 7665  ystem, coding_ve
+00011cf0: 7273 696f 6e3d 636f 6469 6e67 5f76 6572  rsion=coding_ver
+00011d00: 7369 6f6e 290a 2020 2020 2020 2020 6966  sion).        if
+00011d10: 2070 6174 6965 6e74 2e69 6465 6e74 6966   patient.identif
+00011d20: 6965 7220 6973 204e 6f6e 653a 0a20 2020  ier is None:.   
+00011d30: 2020 2020 2020 2020 2070 6174 6965 6e74           patient
+00011d40: 2e69 6465 6e74 6966 6965 7220 3d20 5b6e  .identifier = [n
+00011d50: 6975 5f69 6465 6e74 6966 6965 725d 0a20  iu_identifier]. 
+00011d60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00011d70: 2020 2020 2020 2020 206e 6975 5f69 6465           niu_ide
+00011d80: 6e74 6966 6965 725f 666f 756e 6420 3d20  ntifier_found = 
+00011d90: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00011da0: 2020 666f 7220 6964 656e 7469 6669 6572    for identifier
+00011db0: 2069 6e20 7061 7469 656e 742e 6964 656e   in patient.iden
+00011dc0: 7469 6669 6572 3a0a 2020 2020 2020 2020  tifier:.        
+00011dd0: 2020 2020 2020 2020 6966 2069 6465 6e74          if ident
+00011de0: 6966 6965 722e 7379 7374 656d 203d 3d20  ifier.system == 
+00011df0: 7365 6c66 2e6e 6975 5f69 6465 6e74 6966  self.niu_identif
+00011e00: 6965 725f 7379 7374 656d 3a0a 2020 2020  ier_system:.    
+00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e20: 6964 656e 7469 6669 6572 2e76 616c 7565  identifier.value
+00011e30: 203d 206e 6975 0a20 2020 2020 2020 2020   = niu.         
+00011e40: 2020 2020 2020 2020 2020 206e 6975 5f69             niu_i
+00011e50: 6465 6e74 6966 6965 725f 666f 756e 6420  dentifier_found 
+00011e60: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
+00011e70: 2020 2069 6620 6e6f 7420 6e69 755f 6964     if not niu_id
+00011e80: 656e 7469 6669 6572 5f66 6f75 6e64 2061  entifier_found a
+00011e90: 6e64 206e 6975 5f69 6465 6e74 6966 6965  nd niu_identifie
+00011ea0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+00011eb0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00011ec0: 6174 6965 6e74 2e69 6465 6e74 6966 6965  atient.identifie
+00011ed0: 722e 6170 7065 6e64 286e 6975 5f69 6465  r.append(niu_ide
+00011ee0: 6e74 6966 6965 7229 0a0a 2020 2020 6465  ntifier)..    de
+00011ef0: 6620 6765 745f 6e69 7528 7365 6c66 2c20  f get_niu(self, 
+00011f00: 7061 7469 656e 743d 4e6f 6e65 293a 0a20  patient=None):. 
+00011f10: 2020 2020 2020 206e 6975 203d 204e 6f6e         niu = Non
+00011f20: 650a 2020 2020 2020 2020 6966 2070 6174  e.        if pat
+00011f30: 6965 6e74 2069 7320 4e6f 6e65 3a0a 2020  ient is None:.  
+00011f40: 2020 2020 2020 2020 2020 7061 7469 656e            patien
+00011f50: 7420 3d20 7365 6c66 2e66 6869 725f 7265  t = self.fhir_re
+00011f60: 736f 7572 6365 0a20 2020 2020 2020 2069  source.        i
+00011f70: 6620 7061 7469 656e 742e 6964 656e 7469  f patient.identi
+00011f80: 6669 6572 2069 7320 6e6f 7420 4e6f 6e65  fier is not None
+00011f90: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00011fa0: 7220 6964 656e 7469 6669 6572 2069 6e20  r identifier in 
+00011fb0: 7061 7469 656e 742e 6964 656e 7469 6669  patient.identifi
+00011fc0: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
+00011fd0: 2020 2020 6966 2069 6465 6e74 6966 6965      if identifie
+00011fe0: 722e 7379 7374 656d 203d 3d20 7365 6c66  r.system == self
+00011ff0: 2e6e 6975 5f69 6465 6e74 6966 6965 725f  .niu_identifier_
+00012000: 7379 7374 656d 3a0a 2020 2020 2020 2020  system:.        
+00012010: 2020 2020 2020 2020 2020 2020 6e69 7520              niu 
+00012020: 3d20 6964 656e 7469 6669 6572 2e76 616c  = identifier.val
+00012030: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00012040: 6e20 6e69 750a 0a20 2020 2064 6566 2073  n niu..    def s
+00012050: 6574 5f61 7563 756e 5f69 6465 6e74 6966  et_aucun_identif
+00012060: 6961 6e74 2873 656c 662c 2070 6174 6965  iant(self, patie
+00012070: 6e74 3d4e 6f6e 652c 2063 6f64 696e 675f  nt=None, coding_
+00012080: 7379 7374 656d 3d4e 6f6e 652c 2063 6f64  system=None, cod
+00012090: 696e 675f 7665 7273 696f 6e3d 4e6f 6e65  ing_version=None
+000120a0: 293a 0a20 2020 2020 2020 2069 6620 7061  ):.        if pa
+000120b0: 7469 656e 7420 6973 204e 6f6e 653a 0a20  tient is None:. 
+000120c0: 2020 2020 2020 2020 2020 2070 6174 6965             patie
+000120d0: 6e74 203d 2073 656c 662e 6668 6972 5f72  nt = self.fhir_r
+000120e0: 6573 6f75 7263 650a 0a20 2020 2020 2020  esource..       
+000120f0: 2061 7563 756e 5f69 6465 6e74 6966 6965   aucun_identifie
+00012100: 7220 3d20 7365 6c66 2e61 7563 756e 5f69  r = self.aucun_i
+00012110: 6465 6e74 6966 6961 6e74 5f74 6f5f 6964  dentifiant_to_id
+00012120: 656e 7469 6669 6572 2863 6f64 696e 675f  entifier(coding_
+00012130: 7379 7374 656d 3d63 6f64 696e 675f 7379  system=coding_sy
+00012140: 7374 656d 2c20 636f 6469 6e67 5f76 6572  stem, coding_ver
+00012150: 7369 6f6e 3d63 6f64 696e 675f 7665 7273  sion=coding_vers
+00012160: 696f 6e29 0a20 2020 2020 2020 2070 6174  ion).        pat
+00012170: 6965 6e74 2e69 6465 6e74 6966 6965 7220  ient.identifier 
+00012180: 3d20 5b61 7563 756e 5f69 6465 6e74 6966  = [aucun_identif
+00012190: 6965 725d 0a0a 2020 2020 6465 6620 7365  ier]..    def se
+000121a0: 745f 6269 7274 685f 6461 7465 2873 656c  t_birth_date(sel
+000121b0: 662c 2073 7472 5f64 6174 652c 2070 6174  f, str_date, pat
+000121c0: 6965 6e74 3d4e 6f6e 6529 3a0a 2020 2020  ient=None):.    
+000121d0: 2020 2020 6966 2070 6174 6965 6e74 2069      if patient i
+000121e0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000121f0: 2020 2020 7061 7469 656e 7420 3d20 7365      patient = se
+00012200: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+00012210: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00012220: 662e 6269 7274 685f 6461 7465 203d 2073  f.birth_date = s
+00012230: 7472 5f64 6174 650a 2020 2020 2020 2020  tr_date.        
+00012240: 7061 7469 656e 742e 6269 7274 6844 6174  patient.birthDat
+00012250: 6520 3d20 7365 6c66 2e73 7472 5f64 6174  e = self.str_dat
+00012260: 655f 746f 5f66 6869 725f 6461 7465 2873  e_to_fhir_date(s
+00012270: 7472 5f64 6174 6529 0a0a 2020 2020 6465  tr_date)..    de
+00012280: 6620 6765 745f 6269 7274 685f 6461 7465  f get_birth_date
+00012290: 2873 656c 662c 2070 6174 6965 6e74 3d4e  (self, patient=N
+000122a0: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
+000122b0: 2070 6174 6965 6e74 2069 7320 4e6f 6e65   patient is None
+000122c0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+000122d0: 7469 656e 7420 3d20 7365 6c66 2e66 6869  tient = self.fhi
+000122e0: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
+000122f0: 2020 2072 6574 7572 6e20 7365 6c66 2e66     return self.f
+00012300: 6869 725f 6461 7465 5f74 6f5f 7374 725f  hir_date_to_str_
+00012310: 6461 7465 2866 6869 725f 6461 7465 3d70  date(fhir_date=p
+00012320: 6174 6965 6e74 2e62 6972 7468 4461 7465  atient.birthDate
+00012330: 290a 0a20 2020 2064 6566 2073 6574 5f61  )..    def set_a
+00012340: 6464 7265 7373 2873 656c 662c 2061 6464  ddress(self, add
+00012350: 7265 7373 5f6c 696e 653d 4e6f 6e65 2c20  ress_line=None, 
+00012360: 6164 6472 6573 735f 6369 7479 3d4e 6f6e  address_city=Non
+00012370: 652c 2061 6464 7265 7373 5f73 7461 7465  e, address_state
+00012380: 3d4e 6f6e 652c 2061 6464 7265 7373 5f70  =None, address_p
+00012390: 6f73 7461 6c5f 636f 6465 3d4e 6f6e 652c  ostal_code=None,
+000123a0: 2061 6464 7265 7373 5f63 6f75 6e74 7279   address_country
+000123b0: 3d4e 6f6e 652c 2070 6174 6965 6e74 3d4e  =None, patient=N
+000123c0: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
+000123d0: 2070 6174 6965 6e74 2069 7320 4e6f 6e65   patient is None
+000123e0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+000123f0: 7469 656e 7420 3d20 7365 6c66 2e66 6869  tient = self.fhi
+00012400: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
+00012410: 2020 2020 2020 2073 656c 662e 6164 6472         self.addr
+00012420: 6573 735f 6369 7479 203d 2061 6464 7265  ess_city = addre
+00012430: 7373 5f63 6974 790a 2020 2020 2020 2020  ss_city.        
+00012440: 2020 2020 7365 6c66 2e61 6464 7265 7373      self.address
+00012450: 5f63 6f75 6e74 7279 203d 2061 6464 7265  _country = addre
+00012460: 7373 5f63 6f75 6e74 7279 0a20 2020 2020  ss_country.     
+00012470: 2020 2020 2020 2073 656c 662e 6164 6472         self.addr
+00012480: 6573 735f 6c69 6e65 203d 2061 6464 7265  ess_line = addre
+00012490: 7373 5f6c 696e 650a 2020 2020 2020 2020  ss_line.        
+000124a0: 2020 2020 7365 6c66 2e61 6464 7265 7373      self.address
+000124b0: 5f70 6f73 7461 6c5f 636f 6465 203d 2061  _postal_code = a
+000124c0: 6464 7265 7373 5f70 6f73 7461 6c5f 636f  ddress_postal_co
+000124d0: 6465 0a20 2020 2020 2020 2020 2020 2073  de.            s
+000124e0: 656c 662e 6164 6472 6573 735f 7374 6174  elf.address_stat
+000124f0: 6520 3d20 6164 6472 6573 735f 7374 6174  e = address_stat
+00012500: 650a 2020 2020 2020 2020 6164 6472 6573  e.        addres
+00012510: 7320 3d20 4164 6472 6573 7328 290a 2020  s = Address().  
+00012520: 2020 2020 2020 6164 6472 6573 732e 6369        address.ci
+00012530: 7479 203d 2061 6464 7265 7373 5f63 6974  ty = address_cit
+00012540: 790a 2020 2020 2020 2020 6164 6472 6573  y.        addres
+00012550: 732e 636f 756e 7472 7920 3d20 6164 6472  s.country = addr
+00012560: 6573 735f 636f 756e 7472 790a 2020 2020  ess_country.    
+00012570: 2020 2020 6164 6472 6573 732e 7374 6174      address.stat
+00012580: 6520 3d20 6164 6472 6573 735f 7374 6174  e = address_stat
+00012590: 650a 2020 2020 2020 2020 6164 6472 6573  e.        addres
+000125a0: 732e 706f 7374 616c 436f 6465 203d 2061  s.postalCode = a
+000125b0: 6464 7265 7373 5f70 6f73 7461 6c5f 636f  ddress_postal_co
+000125c0: 6465 0a20 2020 2020 2020 2061 6464 7265  de.        addre
+000125d0: 7373 2e6c 696e 6520 3d20 5b61 6464 7265  ss.line = [addre
+000125e0: 7373 5f6c 696e 655d 0a20 2020 2020 2020  ss_line].       
+000125f0: 2070 6174 6965 6e74 2e61 6464 7265 7373   patient.address
+00012600: 203d 205b 6164 6472 6573 735d 0a0a 2020   = [address]..  
+00012610: 2020 6465 6620 6765 745f 6164 6472 6573    def get_addres
+00012620: 7328 7365 6c66 2c20 7061 7469 656e 743d  s(self, patient=
+00012630: 4e6f 6e65 2c20 696e 6465 783d 3029 3a0a  None, index=0):.
+00012640: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
+00012650: 6e74 2069 7320 4e6f 6e65 3a0a 2020 2020  nt is None:.    
+00012660: 2020 2020 2020 2020 7061 7469 656e 7420          patient 
+00012670: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
+00012680: 7572 6365 0a20 2020 2020 2020 2069 6620  urce.        if 
+00012690: 7061 7469 656e 742e 6164 6472 6573 7320  patient.address 
+000126a0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+000126b0: 6c65 6e28 7061 7469 656e 742e 6164 6472  len(patient.addr
+000126c0: 6573 7329 203e 2069 6e64 6578 3a0a 2020  ess) > index:.  
+000126d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000126e0: 2070 6174 6965 6e74 2e61 6464 7265 7373   patient.address
+000126f0: 5b69 6e64 6578 5d0a 2020 2020 2020 2020  [index].        
+00012700: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+00012710: 2064 6566 2073 6574 5f6d 6f74 6865 725f   def set_mother_
+00012720: 6e61 6d65 2873 656c 662c 206d 6f74 6865  name(self, mothe
+00012730: 725f 6769 7665 6e5f 6e61 6d65 3d4e 6f6e  r_given_name=Non
+00012740: 652c 206d 6f74 6865 725f 6661 6d69 6c79  e, mother_family
+00012750: 5f6e 616d 653d 4e6f 6e65 2c20 7061 7469  _name=None, pati
+00012760: 656e 743d 4e6f 6e65 2c20 636f 6469 6e67  ent=None, coding
+00012770: 5f73 7973 7465 6d3d 4e6f 6e65 2c20 636f  _system=None, co
+00012780: 6469 6e67 5f76 6572 7369 6f6e 3d4e 6f6e  ding_version=Non
+00012790: 6529 3a0a 2020 2020 2020 2020 6966 2070  e):.        if p
+000127a0: 6174 6965 6e74 2069 7320 4e6f 6e65 3a0a  atient is None:.
+000127b0: 2020 2020 2020 2020 2020 2020 7061 7469              pati
+000127c0: 656e 7420 3d20 7365 6c66 2e66 6869 725f  ent = self.fhir_
+000127d0: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
+000127e0: 2020 2020 2073 656c 662e 6d6f 7468 6572       self.mother
+000127f0: 5f66 616d 696c 795f 6e61 6d65 203d 206d  _family_name = m
+00012800: 6f74 6865 725f 6661 6d69 6c79 5f6e 616d  other_family_nam
+00012810: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00012820: 6c66 2e6d 6f74 6865 725f 6769 7665 6e5f  lf.mother_given_
+00012830: 6e61 6d65 203d 206d 6f74 6865 725f 6769  name = mother_gi
+00012840: 7665 6e5f 6e61 6d65 0a20 2020 2020 2020  ven_name.       
+00012850: 206d 6f74 6865 725f 636f 6469 6e67 5f73   mother_coding_s
+00012860: 7973 7465 6d20 3d20 636f 6469 6e67 5f73  ystem = coding_s
+00012870: 7973 7465 6d20 6966 2063 6f64 696e 675f  ystem if coding_
+00012880: 7379 7374 656d 2069 7320 6e6f 7420 4e6f  system is not No
+00012890: 6e65 2065 6c73 6520 7365 6c66 2e64 6566  ne else self.def
+000128a0: 6175 6c74 5f63 6f64 696e 675f 7379 7374  ault_coding_syst
+000128b0: 656d 0a20 2020 2020 2020 206d 6f74 6865  em.        mothe
+000128c0: 725f 636f 6469 6e67 5f76 6572 7369 6f6e  r_coding_version
+000128d0: 203d 2063 6f64 696e 675f 7379 7374 656d   = coding_system
+000128e0: 2069 6620 636f 6469 6e67 5f76 6572 7369   if coding_versi
+000128f0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 2065  on is not None e
+00012900: 6c73 6520 7365 6c66 2e64 6566 6175 6c74  lse self.default
+00012910: 5f63 6f64 696e 675f 7665 7273 696f 6e0a  _coding_version.
+00012920: 2020 2020 2020 2020 636f 6e74 6163 7420          contact 
+00012930: 3d20 5061 7469 656e 7443 6f6e 7461 6374  = PatientContact
+00012940: 2829 0a20 2020 2020 2020 2068 6e20 3d20  ().        hn = 
+00012950: 7365 6c66 2e67 6976 656e 5f66 616d 696c  self.given_famil
+00012960: 795f 746f 5f68 756d 616e 5f6e 616d 6528  y_to_human_name(
+00012970: 6769 7665 6e5f 6e61 6d65 3d6d 6f74 6865  given_name=mothe
+00012980: 725f 6769 7665 6e5f 6e61 6d65 2c20 6661  r_given_name, fa
+00012990: 6d69 6c79 5f6e 616d 653d 6d6f 7468 6572  mily_name=mother
+000129a0: 5f66 616d 696c 795f 6e61 6d65 290a 2020  _family_name).  
+000129b0: 2020 2020 2020 636f 6e74 6163 742e 6e61        contact.na
+000129c0: 6d65 203d 2068 6e0a 2020 2020 2020 2020  me = hn.        
+000129d0: 6d6f 7468 6572 5f63 6f64 6162 6c65 5f63  mother_codable_c
+000129e0: 6f6e 6365 7074 203d 2043 6f64 6561 626c  oncept = Codeabl
+000129f0: 6543 6f6e 6365 7074 2829 0a20 2020 2020  eConcept().     
+00012a00: 2020 206d 6f74 6865 725f 636f 6461 626c     mother_codabl
+00012a10: 655f 636f 6e63 6570 742e 636f 6469 6e67  e_concept.coding
+00012a20: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00012a30: 2043 6f64 696e 6728 0a20 2020 2020 2020   Coding(.       
+00012a40: 2020 2020 2020 2020 206a 736f 6e64 6963           jsondic
+00012a50: 743d 7b0a 2020 2020 2020 2020 2020 2020  t={.            
+00012a60: 2020 2020 2020 2020 2273 7973 7465 6d22          "system"
+00012a70: 3a20 6d6f 7468 6572 5f63 6f64 696e 675f  : mother_coding_
+00012a80: 7379 7374 656d 2c0a 2020 2020 2020 2020  system,.        
+00012a90: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
+00012aa0: 7369 6f6e 223a 206d 6f74 6865 725f 636f  sion": mother_co
+00012ab0: 6469 6e67 5f76 6572 7369 6f6e 2c0a 2020  ding_version,.  
+00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ad0: 2020 2263 6f64 6522 3a20 224d 4552 4522    "code": "MERE"
+00012ae0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012af0: 2020 2020 2020 2264 6973 706c 6179 223a        "display":
+00012b00: 2022 4dc3 a872 6522 0a20 2020 2020 2020   "M..re".       
+00012b10: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00012b20: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00012b30: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+00012b40: 2020 2020 2020 2063 6f6e 7461 6374 2e72         contact.r
+00012b50: 656c 6174 696f 6e73 6869 7020 3d20 5b6d  elationship = [m
+00012b60: 6f74 6865 725f 636f 6461 626c 655f 636f  other_codable_co
+00012b70: 6e63 6570 745d 0a20 2020 2020 2020 2069  ncept].        i
+00012b80: 6620 7061 7469 656e 742e 636f 6e74 6163  f patient.contac
+00012b90: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+00012ba0: 2020 2020 2020 2070 6174 6965 6e74 2e63         patient.c
+00012bb0: 6f6e 7461 6374 203d 205b 636f 6e74 6163  ontact = [contac
+00012bc0: 745d 0a20 2020 2020 2020 2065 6c73 653a  t].        else:
+00012bd0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00012be0: 7461 6374 5f66 6f75 6e64 203d 2046 616c  tact_found = Fal
+00012bf0: 7365 0a20 2020 2020 2020 2020 2020 2066  se.            f
+00012c00: 6f72 2070 6174 6965 6e74 5f63 6f6e 7461  or patient_conta
+00012c10: 6374 2069 6e20 7061 7469 656e 742e 636f  ct in patient.co
+00012c20: 6e74 6163 743a 0a20 2020 2020 2020 2020  ntact:.         
+00012c30: 2020 2020 2020 2066 6f72 2072 656c 6174         for relat
+00012c40: 696f 6e73 6869 7020 696e 2070 6174 6965  ionship in patie
+00012c50: 6e74 5f63 6f6e 7461 6374 2e72 656c 6174  nt_contact.relat
+00012c60: 696f 6e73 6869 703a 0a20 2020 2020 2020  ionship:.       
+00012c70: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00012c80: 2063 6f64 696e 6720 696e 2072 656c 6174   coding in relat
+00012c90: 696f 6e73 6869 702e 636f 6469 6e67 3a0a  ionship.coding:.
+00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cb0: 2020 2020 2020 2020 666f 7220 6d6f 7468          for moth
+00012cc0: 6572 5f63 6f64 6162 6c65 5f63 6f6e 6365  er_codable_conce
+00012cd0: 7074 5f63 6f64 696e 6720 696e 206d 6f74  pt_coding in mot
+00012ce0: 6865 725f 636f 6461 626c 655f 636f 6e63  her_codable_conc
+00012cf0: 6570 742e 636f 6469 6e67 3a0a 2020 2020  ept.coding:.    
+00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d10: 2020 2020 2020 2020 6966 2063 6f64 696e          if codin
+00012d20: 672e 636f 6465 203d 3d20 6d6f 7468 6572  g.code == mother
+00012d30: 5f63 6f64 6162 6c65 5f63 6f6e 6365 7074  _codable_concept
+00012d40: 5f63 6f64 696e 672e 636f 6465 2061 6e64  _coding.code and
+00012d50: 2063 6f64 696e 672e 7379 7374 656d 203d   coding.system =
+00012d60: 3d20 6d6f 7468 6572 5f63 6f64 6162 6c65  = mother_codable
+00012d70: 5f63 6f6e 6365 7074 5f63 6f64 696e 6720  _concept_coding 
+00012d80: 616e 6420 636f 6469 6e67 2e76 6572 7369  and coding.versi
+00012d90: 6f6e 2061 6e64 206d 6f74 6865 725f 636f  on and mother_co
+00012da0: 6461 626c 655f 636f 6e63 6570 745f 636f  dable_concept_co
+00012db0: 6469 6e67 2e76 6572 7369 6f6e 3a0a 2020  ding.version:.  
+00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012dd0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00012de0: 7469 656e 745f 636f 6e74 6163 7420 3d20  tient_contact = 
+00012df0: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
+00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e10: 2020 2020 2020 2020 636f 6e74 6163 745f          contact_
+00012e20: 666f 756e 6420 3d20 5472 7565 0a20 2020  found = True.   
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e40: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00012e50: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+00012e60: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+00012e70: 6e74 6163 745f 666f 756e 643a 0a20 2020  ntact_found:.   
 00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e90: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00012ea0: 6163 745f 666f 756e 6420 3d20 5472 7565  act_found = True
-00012eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ed0: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-00012ee0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012ef0: 6620 636f 6e74 6163 745f 666f 756e 643a  f contact_found:
-00012f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012f10: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00012f20: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
-00012f30: 2020 2020 2020 2069 6620 636f 6e74 6163         if contac
-00012f40: 745f 666f 756e 643a 0a20 2020 2020 2020  t_found:.       
-00012f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f60: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-00012f70: 2020 2020 2020 2069 6620 636f 6e74 6163         if contac
-00012f80: 745f 666f 756e 643a 0a20 2020 2020 2020  t_found:.       
-00012f90: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00012fa0: 616b 0a20 2020 2020 2020 2020 2020 2069  ak.            i
-00012fb0: 6620 6e6f 7420 636f 6e74 6163 745f 666f  f not contact_fo
-00012fc0: 756e 6420 616e 6420 636f 6e74 6163 7420  und and contact 
-00012fd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00012fe0: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-00012ff0: 6965 6e74 2e63 6f6e 7461 6374 2e61 7070  ient.contact.app
-00013000: 656e 6428 636f 6e74 6163 7429 0a0a 2020  end(contact)..  
-00013010: 2020 6465 6620 6765 745f 6d6f 7468 6572    def get_mother
-00013020: 5f6e 616d 6528 7365 6c66 2c20 7061 7469  _name(self, pati
-00013030: 656e 743d 4e6f 6e65 2c20 636f 6469 6e67  ent=None, coding
-00013040: 5f73 7973 7465 6d3d 4e6f 6e65 2c20 636f  _system=None, co
-00013050: 6469 6e67 5f76 6572 7369 6f6e 3d4e 6f6e  ding_version=Non
-00013060: 6529 3a0a 2020 2020 2020 2020 6d6f 7468  e):.        moth
-00013070: 6572 5f63 6f64 696e 675f 7379 7374 656d  er_coding_system
-00013080: 203d 2063 6f64 696e 675f 7379 7374 656d   = coding_system
-00013090: 2069 6620 636f 6469 6e67 5f73 7973 7465   if coding_syste
-000130a0: 6d20 6973 206e 6f74 204e 6f6e 6520 656c  m is not None el
-000130b0: 7365 2073 656c 662e 6465 6661 756c 745f  se self.default_
-000130c0: 636f 6469 6e67 5f73 7973 7465 6d0a 2020  coding_system.  
-000130d0: 2020 2020 2020 6d6f 7468 6572 5f63 6f64        mother_cod
-000130e0: 696e 675f 7665 7273 696f 6e20 3d20 636f  ing_version = co
-000130f0: 6469 6e67 5f73 7973 7465 6d20 6966 2063  ding_system if c
-00013100: 6f64 696e 675f 7665 7273 696f 6e20 6973  oding_version is
-00013110: 206e 6f74 204e 6f6e 6520 656c 7365 2073   not None else s
-00013120: 656c 662e 6465 6661 756c 745f 636f 6469  elf.default_codi
-00013130: 6e67 5f76 6572 7369 6f6e 0a20 2020 2020  ng_version.     
-00013140: 2020 2069 6620 7061 7469 656e 7420 6973     if patient is
-00013150: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00013160: 2020 2070 6174 6965 6e74 203d 2073 656c     patient = sel
-00013170: 662e 6668 6972 5f72 6573 6f75 7263 650a  f.fhir_resource.
-00013180: 2020 2020 2020 2020 6d6f 7468 6572 5f6e          mother_n
-00013190: 616d 6520 3d20 4e6f 6e65 0a20 2020 2020  ame = None.     
-000131a0: 2020 2069 6620 7061 7469 656e 742e 636f     if patient.co
-000131b0: 6e74 6163 7420 6973 206e 6f74 204e 6f6e  ntact is not Non
-000131c0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-000131d0: 6f72 2070 6174 6965 6e74 5f63 6f6e 7461  or patient_conta
-000131e0: 6374 2069 6e20 7061 7469 656e 742e 636f  ct in patient.co
-000131f0: 6e74 6163 743a 0a20 2020 2020 2020 2020  ntact:.         
-00013200: 2020 2020 2020 2066 6f72 2072 656c 6174         for relat
-00013210: 696f 6e73 6869 7020 696e 2070 6174 6965  ionship in patie
-00013220: 6e74 5f63 6f6e 7461 6374 2e72 656c 6174  nt_contact.relat
-00013230: 696f 6e73 6869 703a 0a20 2020 2020 2020  ionship:.       
-00013240: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00013250: 2063 6f64 696e 6720 696e 2072 656c 6174   coding in relat
-00013260: 696f 6e73 6869 702e 636f 6469 6e67 3a0a  ionship.coding:.
-00013270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013280: 2020 2020 2020 2020 6966 2063 6f64 696e          if codin
-00013290: 672e 636f 6465 203d 3d20 274d 4552 4527  g.code == 'MERE'
-000132a0: 2061 6e64 2063 6f64 696e 672e 7379 7374   and coding.syst
-000132b0: 656d 203d 3d20 6d6f 7468 6572 5f63 6f64  em == mother_cod
-000132c0: 696e 675f 7379 7374 656d 2061 6e64 2063  ing_system and c
-000132d0: 6f64 696e 672e 7665 7273 696f 6e20 3d3d  oding.version ==
-000132e0: 206d 6f74 6865 725f 636f 6469 6e67 5f76   mother_coding_v
-000132f0: 6572 7369 6f6e 3a0a 2020 2020 2020 2020  ersion:.        
-00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013310: 2020 2020 6d6f 7468 6572 5f6e 616d 6520      mother_name 
-00013320: 3d20 7061 7469 656e 745f 636f 6e74 6163  = patient_contac
-00013330: 742e 6e61 6d65 0a20 2020 2020 2020 2020  t.name.         
-00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013350: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00013360: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00013370: 6d6f 7468 6572 5f6e 616d 6520 6973 206e  mother_name is n
-00013380: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00013390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133a0: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
-000133b0: 2020 2020 2020 2069 6620 6d6f 7468 6572         if mother
-000133c0: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
-000133d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000133e0: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-000133f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013400: 200a 2020 2020 2020 2020 7265 7475 726e   .        return
-00013410: 206d 6f74 6865 725f 6e61 6d65 0a20 2020   mother_name.   
-00013420: 2020 2020 200a 2020 2020 6465 6620 7365       .    def se
-00013430: 745f 6661 7468 6572 5f6e 616d 6528 7365  t_father_name(se
-00013440: 6c66 2c20 6661 7468 6572 5f67 6976 656e  lf, father_given
-00013450: 5f6e 616d 653d 4e6f 6e65 2c20 6661 7468  _name=None, fath
-00013460: 6572 5f66 616d 696c 795f 6e61 6d65 3d4e  er_family_name=N
-00013470: 6f6e 652c 2070 6174 6965 6e74 3d4e 6f6e  one, patient=Non
-00013480: 652c 2063 6f64 696e 675f 7379 7374 656d  e, coding_system
-00013490: 3d4e 6f6e 652c 2063 6f64 696e 675f 7665  =None, coding_ve
-000134a0: 7273 696f 6e3d 4e6f 6e65 293a 0a20 2020  rsion=None):.   
-000134b0: 2020 2020 2069 6620 7061 7469 656e 7420       if patient 
-000134c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000134d0: 2020 2020 2070 6174 6965 6e74 203d 2073       patient = s
-000134e0: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
-000134f0: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
-00013500: 6c66 2e66 6174 6865 725f 6661 6d69 6c79  lf.father_family
-00013510: 5f6e 616d 6520 3d20 6661 7468 6572 5f66  _name = father_f
-00013520: 616d 696c 795f 6e61 6d65 0a20 2020 2020  amily_name.     
-00013530: 2020 2020 2020 2073 656c 662e 6661 7468         self.fath
-00013540: 6572 5f67 6976 656e 5f6e 616d 6520 3d20  er_given_name = 
-00013550: 6661 7468 6572 5f67 6976 656e 5f6e 616d  father_given_nam
-00013560: 650a 2020 2020 2020 2020 6661 7468 6572  e.        father
-00013570: 5f63 6f64 696e 675f 7379 7374 656d 203d  _coding_system =
-00013580: 2063 6f64 696e 675f 7379 7374 656d 2069   coding_system i
-00013590: 6620 636f 6469 6e67 5f73 7973 7465 6d20  f coding_system 
-000135a0: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
-000135b0: 2073 656c 662e 6465 6661 756c 745f 636f   self.default_co
-000135c0: 6469 6e67 5f73 7973 7465 6d0a 2020 2020  ding_system.    
-000135d0: 2020 2020 6661 7468 6572 5f63 6f64 696e      father_codin
-000135e0: 675f 7665 7273 696f 6e20 3d20 636f 6469  g_version = codi
-000135f0: 6e67 5f73 7973 7465 6d20 6966 2063 6f64  ng_system if cod
-00013600: 696e 675f 7665 7273 696f 6e20 6973 206e  ing_version is n
-00013610: 6f74 204e 6f6e 6520 656c 7365 2073 656c  ot None else sel
-00013620: 662e 6465 6661 756c 745f 636f 6469 6e67  f.default_coding
-00013630: 5f76 6572 7369 6f6e 0a20 2020 2020 2020  _version.       
-00013640: 2063 6f6e 7461 6374 203d 2050 6174 6965   contact = Patie
-00013650: 6e74 436f 6e74 6163 7428 290a 2020 2020  ntContact().    
-00013660: 2020 2020 686e 203d 2073 656c 662e 6769      hn = self.gi
-00013670: 7665 6e5f 6661 6d69 6c79 5f74 6f5f 6875  ven_family_to_hu
-00013680: 6d61 6e5f 6e61 6d65 2867 6976 656e 5f6e  man_name(given_n
-00013690: 616d 653d 6661 7468 6572 5f67 6976 656e  ame=father_given
-000136a0: 5f6e 616d 652c 2066 616d 696c 795f 6e61  _name, family_na
-000136b0: 6d65 3d66 6174 6865 725f 6661 6d69 6c79  me=father_family
-000136c0: 5f6e 616d 6529 0a20 2020 2020 2020 2063  _name).        c
-000136d0: 6f6e 7461 6374 2e6e 616d 6520 3d20 686e  ontact.name = hn
-000136e0: 0a20 2020 2020 2020 2066 6174 6865 725f  .        father_
-000136f0: 636f 6461 626c 655f 636f 6e63 6570 7420  codable_concept 
-00013700: 3d20 436f 6465 6162 6c65 436f 6e63 6570  = CodeableConcep
-00013710: 7428 290a 2020 2020 2020 2020 6661 7468  t().        fath
-00013720: 6572 5f63 6f64 6162 6c65 5f63 6f6e 6365  er_codable_conce
-00013730: 7074 2e63 6f64 696e 6720 3d20 5b0a 2020  pt.coding = [.  
-00013740: 2020 2020 2020 2020 2020 436f 6469 6e67            Coding
-00013750: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00013760: 2020 6a73 6f6e 6469 6374 3d7b 0a20 2020    jsondict={.   
-00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013780: 2022 7379 7374 656d 223a 2066 6174 6865   "system": fathe
-00013790: 725f 636f 6469 6e67 5f73 7973 7465 6d2c  r_coding_system,
-000137a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000137b0: 2020 2020 2022 7665 7273 696f 6e22 3a20       "version": 
-000137c0: 6661 7468 6572 5f63 6f64 696e 675f 7665  father_coding_ve
-000137d0: 7273 696f 6e2c 0a20 2020 2020 2020 2020  rsion,.         
-000137e0: 2020 2020 2020 2020 2020 2022 636f 6465             "code
-000137f0: 223a 2022 5045 5245 222c 0a20 2020 2020  ": "PERE",.     
-00013800: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00013810: 6469 7370 6c61 7922 3a20 2250 c3a8 7265  display": "P..re
-00013820: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00013830: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00013840: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00013850: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00013860: 636f 6e74 6163 742e 7265 6c61 7469 6f6e  contact.relation
-00013870: 7368 6970 203d 205b 6661 7468 6572 5f63  ship = [father_c
-00013880: 6f64 6162 6c65 5f63 6f6e 6365 7074 5d0a  odable_concept].
-00013890: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
-000138a0: 6e74 2e63 6f6e 7461 6374 2069 7320 4e6f  nt.contact is No
-000138b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000138c0: 7061 7469 656e 742e 636f 6e74 6163 7420  patient.contact 
-000138d0: 3d20 5b63 6f6e 7461 6374 5d0a 2020 2020  = [contact].    
-000138e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000138f0: 2020 2020 2020 636f 6e74 6163 745f 666f        contact_fo
-00013900: 756e 6420 3d20 4661 6c73 650a 2020 2020  und = False.    
-00013910: 2020 2020 2020 2020 666f 7220 7061 7469          for pati
-00013920: 656e 745f 636f 6e74 6163 7420 696e 2070  ent_contact in p
-00013930: 6174 6965 6e74 2e63 6f6e 7461 6374 3a0a  atient.contact:.
-00013940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013950: 666f 7220 7265 6c61 7469 6f6e 7368 6970  for relationship
-00013960: 2069 6e20 7061 7469 656e 745f 636f 6e74   in patient_cont
-00013970: 6163 742e 7265 6c61 7469 6f6e 7368 6970  act.relationship
-00013980: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013990: 2020 2020 2020 666f 7220 636f 6469 6e67        for coding
-000139a0: 2069 6e20 7265 6c61 7469 6f6e 7368 6970   in relationship
-000139b0: 2e63 6f64 696e 673a 0a20 2020 2020 2020  .coding:.       
-000139c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139d0: 2066 6f72 2066 6174 6865 725f 636f 6461   for father_coda
-000139e0: 626c 655f 636f 6e63 6570 745f 636f 6469  ble_concept_codi
-000139f0: 6e67 2069 6e20 6661 7468 6572 5f63 6f64  ng in father_cod
-00013a00: 6162 6c65 5f63 6f6e 6365 7074 2e63 6f64  able_concept.cod
-00013a10: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-00013a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a30: 2069 6620 636f 6469 6e67 2e63 6f64 6520   if coding.code 
-00013a40: 3d3d 2066 6174 6865 725f 636f 6461 626c  == father_codabl
-00013a50: 655f 636f 6e63 6570 745f 636f 6469 6e67  e_concept_coding
-00013a60: 2e63 6f64 6520 616e 6420 636f 6469 6e67  .code and coding
-00013a70: 2e73 7973 7465 6d20 3d3d 2066 6174 6865  .system == fathe
-00013a80: 725f 636f 6461 626c 655f 636f 6e63 6570  r_codable_concep
-00013a90: 745f 636f 6469 6e67 2061 6e64 2063 6f64  t_coding and cod
-00013aa0: 696e 672e 7665 7273 696f 6e20 616e 6420  ing.version and 
-00013ab0: 6661 7468 6572 5f63 6f64 6162 6c65 5f63  father_codable_c
-00013ac0: 6f6e 6365 7074 5f63 6f64 696e 672e 7665  oncept_coding.ve
-00013ad0: 7273 696f 6e3a 0a20 2020 2020 2020 2020  rsion:.         
-00013ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013af0: 2020 2020 2020 2070 6174 6965 6e74 5f63         patient_c
-00013b00: 6f6e 7461 6374 203d 2063 6f6e 7461 6374  ontact = contact
-00013b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b30: 2063 6f6e 7461 6374 5f66 6f75 6e64 203d   contact_found =
-00013b40: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-00013b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b60: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00013b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b80: 2020 2020 6966 2063 6f6e 7461 6374 5f66      if contact_f
-00013b90: 6f75 6e64 3a0a 2020 2020 2020 2020 2020  ound:.          
-00013ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bb0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00013bc0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00013bd0: 6f6e 7461 6374 5f66 6f75 6e64 3a0a 2020  ontact_found:.  
-00013be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bf0: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00013c00: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00013c10: 6f6e 7461 6374 5f66 6f75 6e64 3a0a 2020  ontact_found:.  
-00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c30: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00013c40: 2020 2020 6966 206e 6f74 2063 6f6e 7461      if not conta
-00013c50: 6374 5f66 6f75 6e64 2061 6e64 2063 6f6e  ct_found and con
-00013c60: 7461 6374 2069 7320 6e6f 7420 4e6f 6e65  tact is not None
-00013c70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013c80: 2020 7061 7469 656e 742e 636f 6e74 6163    patient.contac
-00013c90: 742e 6170 7065 6e64 2863 6f6e 7461 6374  t.append(contact
-00013ca0: 290a 2020 2020 2020 2020 0a20 2020 2064  ).        .    d
-00013cb0: 6566 2067 6574 5f66 6174 6865 725f 6e61  ef get_father_na
-00013cc0: 6d65 2873 656c 662c 2070 6174 6965 6e74  me(self, patient
-00013cd0: 3d4e 6f6e 652c 2063 6f64 696e 675f 7379  =None, coding_sy
-00013ce0: 7374 656d 3d4e 6f6e 652c 2063 6f64 696e  stem=None, codin
-00013cf0: 675f 7665 7273 696f 6e3d 4e6f 6e65 293a  g_version=None):
-00013d00: 0a20 2020 2020 2020 2069 6620 7061 7469  .        if pati
-00013d10: 656e 7420 6973 204e 6f6e 653a 0a20 2020  ent is None:.   
-00013d20: 2020 2020 2020 2020 2070 6174 6965 6e74           patient
-00013d30: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
-00013d40: 6f75 7263 650a 2020 2020 2020 2020 6661  ource.        fa
-00013d50: 7468 6572 5f63 6f64 696e 675f 7379 7374  ther_coding_syst
-00013d60: 656d 203d 2063 6f64 696e 675f 7379 7374  em = coding_syst
-00013d70: 656d 2069 6620 636f 6469 6e67 5f73 7973  em if coding_sys
-00013d80: 7465 6d20 6973 206e 6f74 204e 6f6e 6520  tem is not None 
-00013d90: 656c 7365 2073 656c 662e 6465 6661 756c  else self.defaul
-00013da0: 745f 636f 6469 6e67 5f73 7973 7465 6d0a  t_coding_system.
-00013db0: 2020 2020 2020 2020 6661 7468 6572 5f63          father_c
-00013dc0: 6f64 696e 675f 7665 7273 696f 6e20 3d20  oding_version = 
-00013dd0: 636f 6469 6e67 5f73 7973 7465 6d20 6966  coding_system if
-00013de0: 2063 6f64 696e 675f 7665 7273 696f 6e20   coding_version 
-00013df0: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
-00013e00: 2073 656c 662e 6465 6661 756c 745f 636f   self.default_co
-00013e10: 6469 6e67 5f76 6572 7369 6f6e 0a20 2020  ding_version.   
-00013e20: 2020 2020 2066 6174 6865 725f 6e61 6d65       father_name
-00013e30: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00013e40: 6966 2070 6174 6965 6e74 2e63 6f6e 7461  if patient.conta
-00013e50: 6374 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ct is not None:.
-00013e60: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00013e70: 7061 7469 656e 745f 636f 6e74 6163 7420  patient_contact 
-00013e80: 696e 2070 6174 6965 6e74 2e63 6f6e 7461  in patient.conta
-00013e90: 6374 3a0a 2020 2020 2020 2020 2020 2020  ct:.            
-00013ea0: 2020 2020 666f 7220 7265 6c61 7469 6f6e      for relation
-00013eb0: 7368 6970 2069 6e20 7061 7469 656e 745f  ship in patient_
-00013ec0: 636f 6e74 6163 742e 7265 6c61 7469 6f6e  contact.relation
-00013ed0: 7368 6970 3a0a 2020 2020 2020 2020 2020  ship:.          
-00013ee0: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-00013ef0: 6469 6e67 2069 6e20 7265 6c61 7469 6f6e  ding in relation
-00013f00: 7368 6970 2e63 6f64 696e 673a 0a20 2020  ship.coding:.   
-00013f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f20: 2020 2020 2069 6620 636f 6469 6e67 2e63       if coding.c
-00013f30: 6f64 6520 3d3d 2027 5045 5245 2720 616e  ode == 'PERE' an
-00013f40: 6420 636f 6469 6e67 2e73 7973 7465 6d20  d coding.system 
-00013f50: 3d3d 2066 6174 6865 725f 636f 6469 6e67  == father_coding
-00013f60: 5f73 7973 7465 6d20 616e 6420 636f 6469  _system and codi
-00013f70: 6e67 2e76 6572 7369 6f6e 203d 3d20 6661  ng.version == fa
-00013f80: 7468 6572 5f63 6f64 696e 675f 7665 7273  ther_coding_vers
-00013f90: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fb0: 2066 6174 6865 725f 6e61 6d65 203d 2070   father_name = p
-00013fc0: 6174 6965 6e74 5f63 6f6e 7461 6374 2e6e  atient_contact.n
-00013fd0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-00013fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ff0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
-00014000: 2020 2020 2020 2020 2020 6966 2066 6174            if fat
-00014010: 6865 725f 6e61 6d65 2069 7320 6e6f 7420  her_name is not 
-00014020: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00014030: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00014040: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
-00014050: 2020 2020 6966 2066 6174 6865 725f 6e61      if father_na
-00014060: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
-00014070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014080: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00014090: 2020 7265 7475 726e 2066 6174 6865 725f    return father_
-000140a0: 6e61 6d65 0a0a 2020 2020 6465 6620 7365  name..    def se
-000140b0: 745f 7068 6f6e 655f 6e75 6d62 6572 2873  t_phone_number(s
-000140c0: 656c 662c 2070 686f 6e65 5f6e 756d 6265  elf, phone_numbe
-000140d0: 722c 2070 6174 6965 6e74 3d4e 6f6e 6529  r, patient=None)
-000140e0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-000140f0: 2070 686f 6e65 5f6e 756d 6265 722e 7374   phone_number.st
-00014100: 6172 7473 7769 7468 2827 2b31 2729 3a0a  artswith('+1'):.
-00014110: 2020 2020 2020 2020 2020 2020 7068 6f6e              phon
-00014120: 655f 6e75 6d62 6572 203d 2027 2b31 7b30  e_number = '+1{0
-00014130: 7d27 2e66 6f72 6d61 7428 7068 6f6e 655f  }'.format(phone_
-00014140: 6e75 6d62 6572 290a 2020 2020 2020 2020  number).        
-00014150: 6966 2070 6174 6965 6e74 2069 7320 4e6f  if patient is No
-00014160: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00014170: 7061 7469 656e 7420 3d20 7365 6c66 2e66  patient = self.f
-00014180: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
-00014190: 2020 2020 2020 2020 2073 656c 662e 7068           self.ph
-000141a0: 6f6e 655f 6e75 6d62 6572 203d 2070 686f  one_number = pho
-000141b0: 6e65 5f6e 756d 6265 720a 2020 2020 2020  ne_number.      
-000141c0: 2020 636f 6e74 6163 745f 706f 696e 7420    contact_point 
-000141d0: 3d20 436f 6e74 6163 7450 6f69 6e74 2829  = ContactPoint()
-000141e0: 0a20 2020 2020 2020 2063 6f6e 7461 6374  .        contact
-000141f0: 5f70 6f69 6e74 2e73 7973 7465 6d20 3d20  _point.system = 
-00014200: 2770 686f 6e65 270a 2020 2020 2020 2020  'phone'.        
-00014210: 636f 6e74 6163 745f 706f 696e 742e 7661  contact_point.va
-00014220: 6c75 6520 3d20 7068 6f6e 655f 6e75 6d62  lue = phone_numb
-00014230: 6572 0a0a 2020 2020 2020 2020 6966 2070  er..        if p
-00014240: 6174 6965 6e74 2e74 656c 6563 6f6d 2069  atient.telecom i
-00014250: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00014260: 2020 2020 7061 7469 656e 742e 7465 6c65      patient.tele
-00014270: 636f 6d20 3d20 5b63 6f6e 7461 6374 5f70  com = [contact_p
-00014280: 6f69 6e74 5d0a 2020 2020 2020 2020 656c  oint].        el
-00014290: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000142a0: 666f 7220 706f 696e 7420 696e 2070 6174  for point in pat
-000142b0: 6965 6e74 2e74 656c 6563 6f6d 3a0a 2020  ient.telecom:.  
-000142c0: 2020 2020 2020 2020 2020 2020 2020 7068                ph
-000142d0: 6f6e 655f 666f 756e 6420 3d20 4661 6c73  one_found = Fals
-000142e0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000142f0: 2020 6966 2070 6f69 6e74 2e73 7973 7465    if point.syste
-00014300: 6d20 3d3d 2027 7068 6f6e 6527 3a0a 2020  m == 'phone':.  
-00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014320: 2020 706f 696e 7420 3d20 636f 6e74 6163    point = contac
-00014330: 745f 706f 696e 740a 2020 2020 2020 2020  t_point.        
-00014340: 2020 2020 2020 2020 2020 2020 7068 6f6e              phon
-00014350: 655f 666f 756e 6420 3d20 5472 7565 0a20  e_found = True. 
-00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014370: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00014380: 2020 2020 2069 6620 6e6f 7420 7068 6f6e       if not phon
-00014390: 655f 666f 756e 6420 616e 6420 636f 6e74  e_found and cont
-000143a0: 6163 745f 706f 696e 7420 6973 206e 6f74  act_point is not
-000143b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000143c0: 2020 2020 2020 2070 6174 6965 6e74 2e74         patient.t
-000143d0: 656c 6563 6f6d 2e61 7070 656e 6428 636f  elecom.append(co
-000143e0: 6e74 6163 745f 706f 696e 7429 0a20 2020  ntact_point).   
-000143f0: 2020 2020 2020 0a20 2020 2064 6566 2067        .    def g
-00014400: 6574 5f70 686f 6e65 5f6e 756d 6265 7228  et_phone_number(
-00014410: 7365 6c66 2c20 7061 7469 656e 743d 4e6f  self, patient=No
-00014420: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
-00014430: 7061 7469 656e 7420 6973 204e 6f6e 653a  patient is None:
-00014440: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
-00014450: 6965 6e74 203d 2073 656c 662e 6668 6972  ient = self.fhir
-00014460: 5f72 6573 6f75 7263 650a 2020 2020 2020  _resource.      
-00014470: 2020 7068 6f6e 655f 6e75 6d62 6572 203d    phone_number =
-00014480: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-00014490: 2070 6174 6965 6e74 2e74 656c 6563 6f6d   patient.telecom
-000144a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000144b0: 2020 2020 2020 2020 2020 666f 7220 706f            for po
-000144c0: 696e 7420 696e 2070 6174 6965 6e74 2e74  int in patient.t
-000144d0: 656c 6563 6f6d 3a0a 2020 2020 2020 2020  elecom:.        
-000144e0: 2020 2020 2020 2020 6966 2070 6f69 6e74          if point
-000144f0: 2e73 7973 7465 6d20 3d3d 2027 7068 6f6e  .system == 'phon
-00014500: 6527 3a0a 2020 2020 2020 2020 2020 2020  e':.            
-00014510: 2020 2020 2020 2020 7068 6f6e 655f 6e75          phone_nu
-00014520: 6d62 6572 203d 2070 6f69 6e74 2e76 616c  mber = point.val
-00014530: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00014540: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00014550: 2020 2020 2072 6574 7572 6e20 7068 6f6e       return phon
-00014560: 655f 6e75 6d62 6572 0a0a 2020 2020 6465  e_number..    de
-00014570: 6620 7061 7469 656e 745f 6469 6374 5f74  f patient_dict_t
-00014580: 6f5f 6668 6972 5f70 6174 6965 6e74 2873  o_fhir_patient(s
-00014590: 656c 662c 2070 6174 6965 6e74 5f64 6963  elf, patient_dic
-000145a0: 743d 4e6f 6e65 2c20 636f 6469 6e67 5f73  t=None, coding_s
-000145b0: 7973 7465 6d3d 4e6f 6e65 2c20 636f 6469  ystem=None, codi
-000145c0: 6e67 5f76 6572 7369 6f6e 3d4e 6f6e 652c  ng_version=None,
-000145d0: 2070 6174 6965 6e74 3d4e 6f6e 6529 3a0a   patient=None):.
-000145e0: 2020 2020 2020 2020 7061 7469 656e 745f          patient_
-000145f0: 636f 6469 6e67 5f73 7973 7465 6d20 3d20  coding_system = 
-00014600: 636f 6469 6e67 5f73 7973 7465 6d20 6966  coding_system if
-00014610: 2063 6f64 696e 675f 7379 7374 656d 2069   coding_system i
-00014620: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-00014630: 7365 6c66 2e64 6566 6175 6c74 5f63 6f64  self.default_cod
-00014640: 696e 675f 7379 7374 656d 0a20 2020 2020  ing_system.     
-00014650: 2020 2070 6174 6965 6e74 5f63 6f64 696e     patient_codin
-00014660: 675f 7665 7273 696f 6e20 3d20 636f 6469  g_version = codi
-00014670: 6e67 5f73 7973 7465 6d20 6966 2063 6f64  ng_system if cod
-00014680: 696e 675f 7665 7273 696f 6e20 6973 206e  ing_version is n
-00014690: 6f74 204e 6f6e 6520 656c 7365 2073 656c  ot None else sel
-000146a0: 662e 6465 6661 756c 745f 636f 6469 6e67  f.default_coding
-000146b0: 5f76 6572 7369 6f6e 0a0a 2020 2020 2020  _version..      
-000146c0: 2020 6966 2070 6174 6965 6e74 5f64 6963    if patient_dic
-000146d0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-000146e0: 2020 2020 2020 2020 2020 2069 6620 276d             if 'm
-000146f0: 6174 6368 7261 6d71 2720 696e 2070 6174  atchramq' in pat
-00014700: 6965 6e74 5f64 6963 7420 616e 6420 7061  ient_dict and pa
-00014710: 7469 656e 745f 6469 6374 5b27 6d61 7463  tient_dict['matc
-00014720: 6872 616d 7127 5d20 6973 206e 6f74 204e  hramq'] is not N
-00014730: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00014740: 2020 2020 2073 656c 662e 7365 745f 6d61       self.set_ma
-00014750: 7463 6872 616d 7128 6d61 7463 6872 616d  tchramq(matchram
-00014760: 713d 7061 7469 656e 745f 6469 6374 5b27  q=patient_dict['
-00014770: 6d61 7463 6872 616d 7127 5d2c 2070 6174  matchramq'], pat
-00014780: 6965 6e74 3d70 6174 6965 6e74 290a 2020  ient=patient).  
-00014790: 2020 2020 2020 2020 2020 6966 2027 6769            if 'gi
-000147a0: 7665 6e5f 6e61 6d65 2720 696e 2070 6174  ven_name' in pat
-000147b0: 6965 6e74 5f64 6963 7420 6f72 2027 6661  ient_dict or 'fa
-000147c0: 6d69 6c79 5f6e 616d 6527 2069 6e20 7061  mily_name' in pa
-000147d0: 7469 656e 745f 6469 6374 3a0a 2020 2020  tient_dict:.    
-000147e0: 2020 2020 2020 2020 2020 2020 6769 7665              give
-000147f0: 6e20 3d20 7061 7469 656e 745f 6469 6374  n = patient_dict
-00014800: 5b27 6769 7665 6e5f 6e61 6d65 275d 2069  ['given_name'] i
-00014810: 6620 2767 6976 656e 5f6e 616d 6527 2069  f 'given_name' i
-00014820: 6e20 7061 7469 656e 745f 6469 6374 2065  n patient_dict e
-00014830: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
-00014840: 2020 2020 2020 2020 2066 616d 696c 7920           family 
-00014850: 3d20 7061 7469 656e 745f 6469 6374 5b27  = patient_dict['
-00014860: 6661 6d69 6c79 5f6e 616d 6527 5d20 6966  family_name'] if
-00014870: 2027 6661 6d69 6c79 5f6e 616d 6527 2069   'family_name' i
-00014880: 6e20 7061 7469 656e 745f 6469 6374 2065  n patient_dict e
-00014890: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
-000148a0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000148b0: 745f 6e61 6d65 2867 6976 656e 5f6e 616d  t_name(given_nam
-000148c0: 653d 6769 7665 6e2c 2066 616d 696c 795f  e=given, family_
-000148d0: 6e61 6d65 3d66 616d 696c 792c 2070 6174  name=family, pat
+00012e90: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012eb0: 2020 2069 6620 636f 6e74 6163 745f 666f     if contact_fo
+00012ec0: 756e 643a 0a20 2020 2020 2020 2020 2020  und:.           
+00012ed0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00012ee0: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+00012ef0: 2020 2069 6620 636f 6e74 6163 745f 666f     if contact_fo
+00012f00: 756e 643a 0a20 2020 2020 2020 2020 2020  und:.           
+00012f10: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+00012f20: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00012f30: 7420 636f 6e74 6163 745f 666f 756e 6420  t contact_found 
+00012f40: 616e 6420 636f 6e74 6163 7420 6973 206e  and contact is n
+00012f50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00012f60: 2020 2020 2020 2020 2070 6174 6965 6e74           patient
+00012f70: 2e63 6f6e 7461 6374 2e61 7070 656e 6428  .contact.append(
+00012f80: 636f 6e74 6163 7429 0a0a 2020 2020 6465  contact)..    de
+00012f90: 6620 6765 745f 6d6f 7468 6572 5f6e 616d  f get_mother_nam
+00012fa0: 6528 7365 6c66 2c20 7061 7469 656e 743d  e(self, patient=
+00012fb0: 4e6f 6e65 2c20 636f 6469 6e67 5f73 7973  None, coding_sys
+00012fc0: 7465 6d3d 4e6f 6e65 2c20 636f 6469 6e67  tem=None, coding
+00012fd0: 5f76 6572 7369 6f6e 3d4e 6f6e 6529 3a0a  _version=None):.
+00012fe0: 2020 2020 2020 2020 6d6f 7468 6572 5f63          mother_c
+00012ff0: 6f64 696e 675f 7379 7374 656d 203d 2063  oding_system = c
+00013000: 6f64 696e 675f 7379 7374 656d 2069 6620  oding_system if 
+00013010: 636f 6469 6e67 5f73 7973 7465 6d20 6973  coding_system is
+00013020: 206e 6f74 204e 6f6e 6520 656c 7365 2073   not None else s
+00013030: 656c 662e 6465 6661 756c 745f 636f 6469  elf.default_codi
+00013040: 6e67 5f73 7973 7465 6d0a 2020 2020 2020  ng_system.      
+00013050: 2020 6d6f 7468 6572 5f63 6f64 696e 675f    mother_coding_
+00013060: 7665 7273 696f 6e20 3d20 636f 6469 6e67  version = coding
+00013070: 5f73 7973 7465 6d20 6966 2063 6f64 696e  _system if codin
+00013080: 675f 7665 7273 696f 6e20 6973 206e 6f74  g_version is not
+00013090: 204e 6f6e 6520 656c 7365 2073 656c 662e   None else self.
+000130a0: 6465 6661 756c 745f 636f 6469 6e67 5f76  default_coding_v
+000130b0: 6572 7369 6f6e 0a20 2020 2020 2020 2069  ersion.        i
+000130c0: 6620 7061 7469 656e 7420 6973 204e 6f6e  f patient is Non
+000130d0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+000130e0: 6174 6965 6e74 203d 2073 656c 662e 6668  atient = self.fh
+000130f0: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
+00013100: 2020 2020 6d6f 7468 6572 5f6e 616d 6520      mother_name 
+00013110: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+00013120: 6620 7061 7469 656e 742e 636f 6e74 6163  f patient.contac
+00013130: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+00013140: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+00013150: 6174 6965 6e74 5f63 6f6e 7461 6374 2069  atient_contact i
+00013160: 6e20 7061 7469 656e 742e 636f 6e74 6163  n patient.contac
+00013170: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00013180: 2020 2066 6f72 2072 656c 6174 696f 6e73     for relations
+00013190: 6869 7020 696e 2070 6174 6965 6e74 5f63  hip in patient_c
+000131a0: 6f6e 7461 6374 2e72 656c 6174 696f 6e73  ontact.relations
+000131b0: 6869 703a 0a20 2020 2020 2020 2020 2020  hip:.           
+000131c0: 2020 2020 2020 2020 2066 6f72 2063 6f64           for cod
+000131d0: 696e 6720 696e 2072 656c 6174 696f 6e73  ing in relations
+000131e0: 6869 702e 636f 6469 6e67 3a0a 2020 2020  hip.coding:.    
+000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013200: 2020 2020 6966 2063 6f64 696e 672e 636f      if coding.co
+00013210: 6465 203d 3d20 274d 4552 4527 2061 6e64  de == 'MERE' and
+00013220: 2063 6f64 696e 672e 7379 7374 656d 203d   coding.system =
+00013230: 3d20 6d6f 7468 6572 5f63 6f64 696e 675f  = mother_coding_
+00013240: 7379 7374 656d 2061 6e64 2063 6f64 696e  system and codin
+00013250: 672e 7665 7273 696f 6e20 3d3d 206d 6f74  g.version == mot
+00013260: 6865 725f 636f 6469 6e67 5f76 6572 7369  her_coding_versi
+00013270: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013290: 6d6f 7468 6572 5f6e 616d 6520 3d20 7061  mother_name = pa
+000132a0: 7469 656e 745f 636f 6e74 6163 742e 6e61  tient_contact.na
+000132b0: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
+000132c0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+000132d0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
+000132e0: 2020 2020 2020 2020 2069 6620 6d6f 7468           if moth
+000132f0: 6572 5f6e 616d 6520 6973 206e 6f74 204e  er_name is not N
+00013300: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013310: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00013320: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+00013330: 2020 2069 6620 6d6f 7468 6572 5f6e 616d     if mother_nam
+00013340: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013360: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00013370: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00013380: 2020 2020 2020 7265 7475 726e 206d 6f74        return mot
+00013390: 6865 725f 6e61 6d65 0a20 2020 2020 2020  her_name.       
+000133a0: 200a 2020 2020 6465 6620 7365 745f 6661   .    def set_fa
+000133b0: 7468 6572 5f6e 616d 6528 7365 6c66 2c20  ther_name(self, 
+000133c0: 6661 7468 6572 5f67 6976 656e 5f6e 616d  father_given_nam
+000133d0: 653d 4e6f 6e65 2c20 6661 7468 6572 5f66  e=None, father_f
+000133e0: 616d 696c 795f 6e61 6d65 3d4e 6f6e 652c  amily_name=None,
+000133f0: 2070 6174 6965 6e74 3d4e 6f6e 652c 2063   patient=None, c
+00013400: 6f64 696e 675f 7379 7374 656d 3d4e 6f6e  oding_system=Non
+00013410: 652c 2063 6f64 696e 675f 7665 7273 696f  e, coding_versio
+00013420: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
+00013430: 2069 6620 7061 7469 656e 7420 6973 204e   if patient is N
+00013440: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013450: 2070 6174 6965 6e74 203d 2073 656c 662e   patient = self.
+00013460: 6668 6972 5f72 6573 6f75 7263 650a 2020  fhir_resource.  
+00013470: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00013480: 6174 6865 725f 6661 6d69 6c79 5f6e 616d  ather_family_nam
+00013490: 6520 3d20 6661 7468 6572 5f66 616d 696c  e = father_famil
+000134a0: 795f 6e61 6d65 0a20 2020 2020 2020 2020  y_name.         
+000134b0: 2020 2073 656c 662e 6661 7468 6572 5f67     self.father_g
+000134c0: 6976 656e 5f6e 616d 6520 3d20 6661 7468  iven_name = fath
+000134d0: 6572 5f67 6976 656e 5f6e 616d 650a 2020  er_given_name.  
+000134e0: 2020 2020 2020 6661 7468 6572 5f63 6f64        father_cod
+000134f0: 696e 675f 7379 7374 656d 203d 2063 6f64  ing_system = cod
+00013500: 696e 675f 7379 7374 656d 2069 6620 636f  ing_system if co
+00013510: 6469 6e67 5f73 7973 7465 6d20 6973 206e  ding_system is n
+00013520: 6f74 204e 6f6e 6520 656c 7365 2073 656c  ot None else sel
+00013530: 662e 6465 6661 756c 745f 636f 6469 6e67  f.default_coding
+00013540: 5f73 7973 7465 6d0a 2020 2020 2020 2020  _system.        
+00013550: 6661 7468 6572 5f63 6f64 696e 675f 7665  father_coding_ve
+00013560: 7273 696f 6e20 3d20 636f 6469 6e67 5f73  rsion = coding_s
+00013570: 7973 7465 6d20 6966 2063 6f64 696e 675f  ystem if coding_
+00013580: 7665 7273 696f 6e20 6973 206e 6f74 204e  version is not N
+00013590: 6f6e 6520 656c 7365 2073 656c 662e 6465  one else self.de
+000135a0: 6661 756c 745f 636f 6469 6e67 5f76 6572  fault_coding_ver
+000135b0: 7369 6f6e 0a20 2020 2020 2020 2063 6f6e  sion.        con
+000135c0: 7461 6374 203d 2050 6174 6965 6e74 436f  tact = PatientCo
+000135d0: 6e74 6163 7428 290a 2020 2020 2020 2020  ntact().        
+000135e0: 686e 203d 2073 656c 662e 6769 7665 6e5f  hn = self.given_
+000135f0: 6661 6d69 6c79 5f74 6f5f 6875 6d61 6e5f  family_to_human_
+00013600: 6e61 6d65 2867 6976 656e 5f6e 616d 653d  name(given_name=
+00013610: 6661 7468 6572 5f67 6976 656e 5f6e 616d  father_given_nam
+00013620: 652c 2066 616d 696c 795f 6e61 6d65 3d66  e, family_name=f
+00013630: 6174 6865 725f 6661 6d69 6c79 5f6e 616d  ather_family_nam
+00013640: 6529 0a20 2020 2020 2020 2063 6f6e 7461  e).        conta
+00013650: 6374 2e6e 616d 6520 3d20 686e 0a20 2020  ct.name = hn.   
+00013660: 2020 2020 2066 6174 6865 725f 636f 6461       father_coda
+00013670: 626c 655f 636f 6e63 6570 7420 3d20 436f  ble_concept = Co
+00013680: 6465 6162 6c65 436f 6e63 6570 7428 290a  deableConcept().
+00013690: 2020 2020 2020 2020 6661 7468 6572 5f63          father_c
+000136a0: 6f64 6162 6c65 5f63 6f6e 6365 7074 2e63  odable_concept.c
+000136b0: 6f64 696e 6720 3d20 5b0a 2020 2020 2020  oding = [.      
+000136c0: 2020 2020 2020 436f 6469 6e67 280a 2020        Coding(.  
+000136d0: 2020 2020 2020 2020 2020 2020 2020 6a73                js
+000136e0: 6f6e 6469 6374 3d7b 0a20 2020 2020 2020  ondict={.       
+000136f0: 2020 2020 2020 2020 2020 2020 2022 7379               "sy
+00013700: 7374 656d 223a 2066 6174 6865 725f 636f  stem": father_co
+00013710: 6469 6e67 5f73 7973 7465 6d2c 0a20 2020  ding_system,.   
+00013720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013730: 2022 7665 7273 696f 6e22 3a20 6661 7468   "version": fath
+00013740: 6572 5f63 6f64 696e 675f 7665 7273 696f  er_coding_versio
+00013750: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+00013760: 2020 2020 2020 2022 636f 6465 223a 2022         "code": "
+00013770: 5045 5245 222c 0a20 2020 2020 2020 2020  PERE",.         
+00013780: 2020 2020 2020 2020 2020 2022 6469 7370             "disp
+00013790: 6c61 7922 3a20 2250 c3a8 7265 220a 2020  lay": "P..re".  
+000137a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137b0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+000137c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+000137d0: 2020 5d0a 2020 2020 2020 2020 636f 6e74    ].        cont
+000137e0: 6163 742e 7265 6c61 7469 6f6e 7368 6970  act.relationship
+000137f0: 203d 205b 6661 7468 6572 5f63 6f64 6162   = [father_codab
+00013800: 6c65 5f63 6f6e 6365 7074 5d0a 2020 2020  le_concept].    
+00013810: 2020 2020 6966 2070 6174 6965 6e74 2e63      if patient.c
+00013820: 6f6e 7461 6374 2069 7320 4e6f 6e65 3a0a  ontact is None:.
+00013830: 2020 2020 2020 2020 2020 2020 7061 7469              pati
+00013840: 656e 742e 636f 6e74 6163 7420 3d20 5b63  ent.contact = [c
+00013850: 6f6e 7461 6374 5d0a 2020 2020 2020 2020  ontact].        
+00013860: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00013870: 2020 636f 6e74 6163 745f 666f 756e 6420    contact_found 
+00013880: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00013890: 2020 2020 666f 7220 7061 7469 656e 745f      for patient_
+000138a0: 636f 6e74 6163 7420 696e 2070 6174 6965  contact in patie
+000138b0: 6e74 2e63 6f6e 7461 6374 3a0a 2020 2020  nt.contact:.    
+000138c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000138d0: 7265 6c61 7469 6f6e 7368 6970 2069 6e20  relationship in 
+000138e0: 7061 7469 656e 745f 636f 6e74 6163 742e  patient_contact.
+000138f0: 7265 6c61 7469 6f6e 7368 6970 3a0a 2020  relationship:.  
+00013900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013910: 2020 666f 7220 636f 6469 6e67 2069 6e20    for coding in 
+00013920: 7265 6c61 7469 6f6e 7368 6970 2e63 6f64  relationship.cod
+00013930: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00013940: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00013950: 2066 6174 6865 725f 636f 6461 626c 655f   father_codable_
+00013960: 636f 6e63 6570 745f 636f 6469 6e67 2069  concept_coding i
+00013970: 6e20 6661 7468 6572 5f63 6f64 6162 6c65  n father_codable
+00013980: 5f63 6f6e 6365 7074 2e63 6f64 696e 673a  _concept.coding:
+00013990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000139a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000139b0: 636f 6469 6e67 2e63 6f64 6520 3d3d 2066  coding.code == f
+000139c0: 6174 6865 725f 636f 6461 626c 655f 636f  ather_codable_co
+000139d0: 6e63 6570 745f 636f 6469 6e67 2e63 6f64  ncept_coding.cod
+000139e0: 6520 616e 6420 636f 6469 6e67 2e73 7973  e and coding.sys
+000139f0: 7465 6d20 3d3d 2066 6174 6865 725f 636f  tem == father_co
+00013a00: 6461 626c 655f 636f 6e63 6570 745f 636f  dable_concept_co
+00013a10: 6469 6e67 2061 6e64 2063 6f64 696e 672e  ding and coding.
+00013a20: 7665 7273 696f 6e20 616e 6420 6661 7468  version and fath
+00013a30: 6572 5f63 6f64 6162 6c65 5f63 6f6e 6365  er_codable_conce
+00013a40: 7074 5f63 6f64 696e 672e 7665 7273 696f  pt_coding.versio
+00013a50: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
+00013a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a70: 2020 2070 6174 6965 6e74 5f63 6f6e 7461     patient_conta
+00013a80: 6374 203d 2063 6f6e 7461 6374 0a20 2020  ct = contact.   
+00013a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013aa0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00013ab0: 7461 6374 5f66 6f75 6e64 203d 2054 7275  tact_found = Tru
+00013ac0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00013ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ae0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+00013af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b00: 6966 2063 6f6e 7461 6374 5f66 6f75 6e64  if contact_found
+00013b10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013b20: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00013b30: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00013b40: 2020 2020 2020 2020 6966 2063 6f6e 7461          if conta
+00013b50: 6374 5f66 6f75 6e64 3a0a 2020 2020 2020  ct_found:.      
+00013b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b70: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+00013b80: 2020 2020 2020 2020 6966 2063 6f6e 7461          if conta
+00013b90: 6374 5f66 6f75 6e64 3a0a 2020 2020 2020  ct_found:.      
+00013ba0: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00013bb0: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
+00013bc0: 6966 206e 6f74 2063 6f6e 7461 6374 5f66  if not contact_f
+00013bd0: 6f75 6e64 2061 6e64 2063 6f6e 7461 6374  ound and contact
+00013be0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00013bf0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00013c00: 7469 656e 742e 636f 6e74 6163 742e 6170  tient.contact.ap
+00013c10: 7065 6e64 2863 6f6e 7461 6374 290a 2020  pend(contact).  
+00013c20: 2020 2020 2020 0a20 2020 2064 6566 2067        .    def g
+00013c30: 6574 5f66 6174 6865 725f 6e61 6d65 2873  et_father_name(s
+00013c40: 656c 662c 2070 6174 6965 6e74 3d4e 6f6e  elf, patient=Non
+00013c50: 652c 2063 6f64 696e 675f 7379 7374 656d  e, coding_system
+00013c60: 3d4e 6f6e 652c 2063 6f64 696e 675f 7665  =None, coding_ve
+00013c70: 7273 696f 6e3d 4e6f 6e65 293a 0a20 2020  rsion=None):.   
+00013c80: 2020 2020 2069 6620 7061 7469 656e 7420       if patient 
+00013c90: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00013ca0: 2020 2020 2070 6174 6965 6e74 203d 2073       patient = s
+00013cb0: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+00013cc0: 650a 2020 2020 2020 2020 6661 7468 6572  e.        father
+00013cd0: 5f63 6f64 696e 675f 7379 7374 656d 203d  _coding_system =
+00013ce0: 2063 6f64 696e 675f 7379 7374 656d 2069   coding_system i
+00013cf0: 6620 636f 6469 6e67 5f73 7973 7465 6d20  f coding_system 
+00013d00: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
+00013d10: 2073 656c 662e 6465 6661 756c 745f 636f   self.default_co
+00013d20: 6469 6e67 5f73 7973 7465 6d0a 2020 2020  ding_system.    
+00013d30: 2020 2020 6661 7468 6572 5f63 6f64 696e      father_codin
+00013d40: 675f 7665 7273 696f 6e20 3d20 636f 6469  g_version = codi
+00013d50: 6e67 5f73 7973 7465 6d20 6966 2063 6f64  ng_system if cod
+00013d60: 696e 675f 7665 7273 696f 6e20 6973 206e  ing_version is n
+00013d70: 6f74 204e 6f6e 6520 656c 7365 2073 656c  ot None else sel
+00013d80: 662e 6465 6661 756c 745f 636f 6469 6e67  f.default_coding
+00013d90: 5f76 6572 7369 6f6e 0a20 2020 2020 2020  _version.       
+00013da0: 2066 6174 6865 725f 6e61 6d65 203d 204e   father_name = N
+00013db0: 6f6e 650a 2020 2020 2020 2020 6966 2070  one.        if p
+00013dc0: 6174 6965 6e74 2e63 6f6e 7461 6374 2069  atient.contact i
+00013dd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00013de0: 2020 2020 2020 2020 666f 7220 7061 7469          for pati
+00013df0: 656e 745f 636f 6e74 6163 7420 696e 2070  ent_contact in p
+00013e00: 6174 6965 6e74 2e63 6f6e 7461 6374 3a0a  atient.contact:.
+00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e20: 666f 7220 7265 6c61 7469 6f6e 7368 6970  for relationship
+00013e30: 2069 6e20 7061 7469 656e 745f 636f 6e74   in patient_cont
+00013e40: 6163 742e 7265 6c61 7469 6f6e 7368 6970  act.relationship
+00013e50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013e60: 2020 2020 2020 666f 7220 636f 6469 6e67        for coding
+00013e70: 2069 6e20 7265 6c61 7469 6f6e 7368 6970   in relationship
+00013e80: 2e63 6f64 696e 673a 0a20 2020 2020 2020  .coding:.       
+00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ea0: 2069 6620 636f 6469 6e67 2e63 6f64 6520   if coding.code 
+00013eb0: 3d3d 2027 5045 5245 2720 616e 6420 636f  == 'PERE' and co
+00013ec0: 6469 6e67 2e73 7973 7465 6d20 3d3d 2066  ding.system == f
+00013ed0: 6174 6865 725f 636f 6469 6e67 5f73 7973  ather_coding_sys
+00013ee0: 7465 6d20 616e 6420 636f 6469 6e67 2e76  tem and coding.v
+00013ef0: 6572 7369 6f6e 203d 3d20 6661 7468 6572  ersion == father
+00013f00: 5f63 6f64 696e 675f 7665 7273 696f 6e3a  _coding_version:
+00013f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013f20: 2020 2020 2020 2020 2020 2020 2066 6174               fat
+00013f30: 6865 725f 6e61 6d65 203d 2070 6174 6965  her_name = patie
+00013f40: 6e74 5f63 6f6e 7461 6374 2e6e 616d 650a  nt_contact.name.
+00013f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f60: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00013f70: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+00013f80: 2020 2020 2020 6966 2066 6174 6865 725f        if father_
+00013f90: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
+00013fa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013fb0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fd0: 6966 2066 6174 6865 725f 6e61 6d65 2069  if father_name i
+00013fe0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00013ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014000: 6272 6561 6b0a 2020 2020 2020 2020 7265  break.        re
+00014010: 7475 726e 2066 6174 6865 725f 6e61 6d65  turn father_name
+00014020: 0a0a 2020 2020 6465 6620 7365 745f 7068  ..    def set_ph
+00014030: 6f6e 655f 6e75 6d62 6572 2873 656c 662c  one_number(self,
+00014040: 2070 686f 6e65 5f6e 756d 6265 722c 2070   phone_number, p
+00014050: 6174 6965 6e74 3d4e 6f6e 6529 3a0a 2020  atient=None):.  
+00014060: 2020 2020 2020 6966 206e 6f74 2070 686f        if not pho
+00014070: 6e65 5f6e 756d 6265 722e 7374 6172 7473  ne_number.starts
+00014080: 7769 7468 2827 2b31 2729 3a0a 2020 2020  with('+1'):.    
+00014090: 2020 2020 2020 2020 7068 6f6e 655f 6e75          phone_nu
+000140a0: 6d62 6572 203d 2027 2b31 7b30 7d27 2e66  mber = '+1{0}'.f
+000140b0: 6f72 6d61 7428 7068 6f6e 655f 6e75 6d62  ormat(phone_numb
+000140c0: 6572 290a 2020 2020 2020 2020 6966 2070  er).        if p
+000140d0: 6174 6965 6e74 2069 7320 4e6f 6e65 3a0a  atient is None:.
+000140e0: 2020 2020 2020 2020 2020 2020 7061 7469              pati
+000140f0: 656e 7420 3d20 7365 6c66 2e66 6869 725f  ent = self.fhir_
+00014100: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
+00014110: 2020 2020 2073 656c 662e 7068 6f6e 655f       self.phone_
+00014120: 6e75 6d62 6572 203d 2070 686f 6e65 5f6e  number = phone_n
+00014130: 756d 6265 720a 2020 2020 2020 2020 636f  umber.        co
+00014140: 6e74 6163 745f 706f 696e 7420 3d20 436f  ntact_point = Co
+00014150: 6e74 6163 7450 6f69 6e74 2829 0a20 2020  ntactPoint().   
+00014160: 2020 2020 2063 6f6e 7461 6374 5f70 6f69       contact_poi
+00014170: 6e74 2e73 7973 7465 6d20 3d20 2770 686f  nt.system = 'pho
+00014180: 6e65 270a 2020 2020 2020 2020 636f 6e74  ne'.        cont
+00014190: 6163 745f 706f 696e 742e 7661 6c75 6520  act_point.value 
+000141a0: 3d20 7068 6f6e 655f 6e75 6d62 6572 0a0a  = phone_number..
+000141b0: 2020 2020 2020 2020 6966 2070 6174 6965          if patie
+000141c0: 6e74 2e74 656c 6563 6f6d 2069 7320 4e6f  nt.telecom is No
+000141d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000141e0: 7061 7469 656e 742e 7465 6c65 636f 6d20  patient.telecom 
+000141f0: 3d20 5b63 6f6e 7461 6374 5f70 6f69 6e74  = [contact_point
+00014200: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
+00014210: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00014220: 706f 696e 7420 696e 2070 6174 6965 6e74  point in patient
+00014230: 2e74 656c 6563 6f6d 3a0a 2020 2020 2020  .telecom:.      
+00014240: 2020 2020 2020 2020 2020 7068 6f6e 655f            phone_
+00014250: 666f 756e 6420 3d20 4661 6c73 650a 2020  found = False.  
+00014260: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00014270: 2070 6f69 6e74 2e73 7973 7465 6d20 3d3d   point.system ==
+00014280: 2027 7068 6f6e 6527 3a0a 2020 2020 2020   'phone':.      
+00014290: 2020 2020 2020 2020 2020 2020 2020 706f                po
+000142a0: 696e 7420 3d20 636f 6e74 6163 745f 706f  int = contact_po
+000142b0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+000142c0: 2020 2020 2020 2020 7068 6f6e 655f 666f          phone_fo
+000142d0: 756e 6420 3d20 5472 7565 0a20 2020 2020  und = True.     
+000142e0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+000142f0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
+00014300: 2069 6620 6e6f 7420 7068 6f6e 655f 666f   if not phone_fo
+00014310: 756e 6420 616e 6420 636f 6e74 6163 745f  und and contact_
+00014320: 706f 696e 7420 6973 206e 6f74 204e 6f6e  point is not Non
+00014330: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00014340: 2020 2070 6174 6965 6e74 2e74 656c 6563     patient.telec
+00014350: 6f6d 2e61 7070 656e 6428 636f 6e74 6163  om.append(contac
+00014360: 745f 706f 696e 7429 0a20 2020 2020 2020  t_point).       
+00014370: 2020 0a20 2020 2064 6566 2067 6574 5f70    .    def get_p
+00014380: 686f 6e65 5f6e 756d 6265 7228 7365 6c66  hone_number(self
+00014390: 2c20 7061 7469 656e 743d 4e6f 6e65 293a  , patient=None):
+000143a0: 0a20 2020 2020 2020 2069 6620 7061 7469  .        if pati
+000143b0: 656e 7420 6973 204e 6f6e 653a 0a20 2020  ent is None:.   
+000143c0: 2020 2020 2020 2020 2070 6174 6965 6e74           patient
+000143d0: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
+000143e0: 6f75 7263 650a 2020 2020 2020 2020 7068  ource.        ph
+000143f0: 6f6e 655f 6e75 6d62 6572 203d 204e 6f6e  one_number = Non
+00014400: 650a 2020 2020 2020 2020 6966 2070 6174  e.        if pat
+00014410: 6965 6e74 2e74 656c 6563 6f6d 2069 7320  ient.telecom is 
+00014420: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00014430: 2020 2020 2020 666f 7220 706f 696e 7420        for point 
+00014440: 696e 2070 6174 6965 6e74 2e74 656c 6563  in patient.telec
+00014450: 6f6d 3a0a 2020 2020 2020 2020 2020 2020  om:.            
+00014460: 2020 2020 6966 2070 6f69 6e74 2e73 7973      if point.sys
+00014470: 7465 6d20 3d3d 2027 7068 6f6e 6527 3a0a  tem == 'phone':.
+00014480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014490: 2020 2020 7068 6f6e 655f 6e75 6d62 6572      phone_number
+000144a0: 203d 2070 6f69 6e74 2e76 616c 7565 0a20   = point.value. 
+000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144c0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+000144d0: 2072 6574 7572 6e20 7068 6f6e 655f 6e75   return phone_nu
+000144e0: 6d62 6572 0a0a 2020 2020 6465 6620 7061  mber..    def pa
+000144f0: 7469 656e 745f 6469 6374 5f74 6f5f 6668  tient_dict_to_fh
+00014500: 6972 5f70 6174 6965 6e74 2873 656c 662c  ir_patient(self,
+00014510: 2070 6174 6965 6e74 5f64 6963 743d 4e6f   patient_dict=No
+00014520: 6e65 2c20 636f 6469 6e67 5f73 7973 7465  ne, coding_syste
+00014530: 6d3d 4e6f 6e65 2c20 636f 6469 6e67 5f76  m=None, coding_v
+00014540: 6572 7369 6f6e 3d4e 6f6e 652c 2070 6174  ersion=None, pat
+00014550: 6965 6e74 3d4e 6f6e 6529 3a0a 2020 2020  ient=None):.    
+00014560: 2020 2020 7061 7469 656e 745f 636f 6469      patient_codi
+00014570: 6e67 5f73 7973 7465 6d20 3d20 636f 6469  ng_system = codi
+00014580: 6e67 5f73 7973 7465 6d20 6966 2063 6f64  ng_system if cod
+00014590: 696e 675f 7379 7374 656d 2069 7320 6e6f  ing_system is no
+000145a0: 7420 4e6f 6e65 2065 6c73 6520 7365 6c66  t None else self
+000145b0: 2e64 6566 6175 6c74 5f63 6f64 696e 675f  .default_coding_
+000145c0: 7379 7374 656d 0a20 2020 2020 2020 2070  system.        p
+000145d0: 6174 6965 6e74 5f63 6f64 696e 675f 7665  atient_coding_ve
+000145e0: 7273 696f 6e20 3d20 636f 6469 6e67 5f73  rsion = coding_s
+000145f0: 7973 7465 6d20 6966 2063 6f64 696e 675f  ystem if coding_
+00014600: 7665 7273 696f 6e20 6973 206e 6f74 204e  version is not N
+00014610: 6f6e 6520 656c 7365 2073 656c 662e 6465  one else self.de
+00014620: 6661 756c 745f 636f 6469 6e67 5f76 6572  fault_coding_ver
+00014630: 7369 6f6e 0a0a 2020 2020 2020 2020 6966  sion..        if
+00014640: 2070 6174 6965 6e74 5f64 6963 7420 6973   patient_dict is
+00014650: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00014660: 2020 2020 2020 2069 6620 276d 6174 6368         if 'match
+00014670: 7261 6d71 2720 696e 2070 6174 6965 6e74  ramq' in patient
+00014680: 5f64 6963 7420 616e 6420 7061 7469 656e  _dict and patien
+00014690: 745f 6469 6374 5b27 6d61 7463 6872 616d  t_dict['matchram
+000146a0: 7127 5d20 6973 206e 6f74 204e 6f6e 653a  q'] is not None:
+000146b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000146c0: 2073 656c 662e 7365 745f 6d61 7463 6872   self.set_matchr
+000146d0: 616d 7128 6d61 7463 6872 616d 713d 7061  amq(matchramq=pa
+000146e0: 7469 656e 745f 6469 6374 5b27 6d61 7463  tient_dict['matc
+000146f0: 6872 616d 7127 5d2c 2070 6174 6965 6e74  hramq'], patient
+00014700: 3d70 6174 6965 6e74 290a 2020 2020 2020  =patient).      
+00014710: 2020 2020 2020 6966 2027 6769 7665 6e5f        if 'given_
+00014720: 6e61 6d65 2720 696e 2070 6174 6965 6e74  name' in patient
+00014730: 5f64 6963 7420 6f72 2027 6661 6d69 6c79  _dict or 'family
+00014740: 5f6e 616d 6527 2069 6e20 7061 7469 656e  _name' in patien
+00014750: 745f 6469 6374 3a0a 2020 2020 2020 2020  t_dict:.        
+00014760: 2020 2020 2020 2020 6769 7665 6e20 3d20          given = 
+00014770: 7061 7469 656e 745f 6469 6374 5b27 6769  patient_dict['gi
+00014780: 7665 6e5f 6e61 6d65 275d 2069 6620 2767  ven_name'] if 'g
+00014790: 6976 656e 5f6e 616d 6527 2069 6e20 7061  iven_name' in pa
+000147a0: 7469 656e 745f 6469 6374 2065 6c73 6520  tient_dict else 
+000147b0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+000147c0: 2020 2020 2066 616d 696c 7920 3d20 7061       family = pa
+000147d0: 7469 656e 745f 6469 6374 5b27 6661 6d69  tient_dict['fami
+000147e0: 6c79 5f6e 616d 6527 5d20 6966 2027 6661  ly_name'] if 'fa
+000147f0: 6d69 6c79 5f6e 616d 6527 2069 6e20 7061  mily_name' in pa
+00014800: 7469 656e 745f 6469 6374 2065 6c73 6520  tient_dict else 
+00014810: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00014820: 2020 2020 2073 656c 662e 7365 745f 6e61       self.set_na
+00014830: 6d65 2867 6976 656e 5f6e 616d 653d 6769  me(given_name=gi
+00014840: 7665 6e2c 2066 616d 696c 795f 6e61 6d65  ven, family_name
+00014850: 3d66 616d 696c 792c 2070 6174 6965 6e74  =family, patient
+00014860: 3d70 6174 6965 6e74 290a 2020 2020 2020  =patient).      
+00014870: 2020 2020 2020 6966 2027 6e61 6d27 206e        if 'nam' n
+00014880: 6f74 2069 6e20 7061 7469 656e 745f 6469  ot in patient_di
+00014890: 6374 2061 6e64 2027 6e69 7527 206e 6f74  ct and 'niu' not
+000148a0: 2069 6e20 7061 7469 656e 745f 6469 6374   in patient_dict
+000148b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000148c0: 2020 7365 6c66 2e73 6574 5f61 7563 756e    self.set_aucun
+000148d0: 5f69 6465 6e74 6966 6961 6e74 2870 6174  _identifiant(pat
 000148e0: 6965 6e74 3d70 6174 6965 6e74 290a 2020  ient=patient).  
-000148f0: 2020 2020 2020 2020 2020 6966 2027 6e61            if 'na
-00014900: 6d27 206e 6f74 2069 6e20 7061 7469 656e  m' not in patien
-00014910: 745f 6469 6374 2061 6e64 2027 6e69 7527  t_dict and 'niu'
-00014920: 206e 6f74 2069 6e20 7061 7469 656e 745f   not in patient_
-00014930: 6469 6374 3a0a 2020 2020 2020 2020 2020  dict:.          
-00014940: 2020 2020 2020 7365 6c66 2e73 6574 5f61        self.set_a
-00014950: 7563 756e 5f69 6465 6e74 6966 6961 6e74  ucun_identifiant
-00014960: 2870 6174 6965 6e74 3d70 6174 6965 6e74  (patient=patient
-00014970: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00014980: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00014990: 2020 2020 6966 2027 6e61 6d27 2069 6e20      if 'nam' in 
-000149a0: 7061 7469 656e 745f 6469 6374 3a0a 2020  patient_dict:.  
-000149b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149c0: 2020 7365 6c66 2e73 6574 5f6e 616d 286e    self.set_nam(n
-000149d0: 616d 3d70 6174 6965 6e74 5f64 6963 745b  am=patient_dict[
-000149e0: 276e 616d 275d 2c20 636f 6469 6e67 5f73  'nam'], coding_s
-000149f0: 7973 7465 6d3d 7061 7469 656e 745f 636f  ystem=patient_co
-00014a00: 6469 6e67 5f73 7973 7465 6d2c 2063 6f64  ding_system, cod
-00014a10: 696e 675f 7665 7273 696f 6e3d 7061 7469  ing_version=pati
-00014a20: 656e 745f 636f 6469 6e67 5f76 6572 7369  ent_coding_versi
-00014a30: 6f6e 2c20 7061 7469 656e 743d 7061 7469  on, patient=pati
-00014a40: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
-00014a50: 2020 2020 2069 6620 276e 6975 2720 696e       if 'niu' in
-00014a60: 2070 6174 6965 6e74 5f64 6963 743a 0a20   patient_dict:. 
-00014a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a80: 2020 2073 656c 662e 7365 745f 6e69 7528     self.set_niu(
-00014a90: 6e69 753d 7061 7469 656e 745f 6469 6374  niu=patient_dict
-00014aa0: 5b27 6e69 7527 5d2c 2063 6f64 696e 675f  ['niu'], coding_
-00014ab0: 7379 7374 656d 3d70 6174 6965 6e74 5f63  system=patient_c
-00014ac0: 6f64 696e 675f 7379 7374 656d 2c20 636f  oding_system, co
-00014ad0: 6469 6e67 5f76 6572 7369 6f6e 3d70 6174  ding_version=pat
-00014ae0: 6965 6e74 5f63 6f64 696e 675f 7665 7273  ient_coding_vers
-00014af0: 696f 6e2c 2070 6174 6965 6e74 3d70 6174  ion, patient=pat
-00014b00: 6965 6e74 290a 2020 2020 2020 2020 2020  ient).          
-00014b10: 2020 6966 2027 6765 6e64 6572 2720 696e    if 'gender' in
-00014b20: 2070 6174 6965 6e74 5f64 6963 743a 0a20   patient_dict:. 
-00014b30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014b40: 656c 662e 7365 745f 6765 6e64 6572 2867  elf.set_gender(g
-00014b50: 656e 6465 723d 7061 7469 656e 745f 6469  ender=patient_di
-00014b60: 6374 5b27 6765 6e64 6572 275d 2c20 7061  ct['gender'], pa
-00014b70: 7469 656e 743d 7061 7469 656e 7429 0a20  tient=patient). 
-00014b80: 2020 2020 2020 2020 2020 2069 6620 2762             if 'b
-00014b90: 6972 7468 5f64 6174 6527 2069 6e20 7061  irth_date' in pa
-00014ba0: 7469 656e 745f 6469 6374 3a0a 2020 2020  tient_dict:.    
-00014bb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014bc0: 2e73 6574 5f62 6972 7468 5f64 6174 6528  .set_birth_date(
-00014bd0: 7374 725f 6461 7465 3d70 6174 6965 6e74  str_date=patient
-00014be0: 5f64 6963 745b 2762 6972 7468 5f64 6174  _dict['birth_dat
-00014bf0: 6527 5d2c 2070 6174 6965 6e74 3d70 6174  e'], patient=pat
-00014c00: 6965 6e74 290a 2020 2020 2020 2020 2020  ient).          
-00014c10: 2020 6966 2027 6964 2720 696e 2070 6174    if 'id' in pat
-00014c20: 6965 6e74 5f64 6963 743a 0a20 2020 2020  ient_dict:.     
-00014c30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014c40: 7365 745f 6964 2869 643d 7061 7469 656e  set_id(id=patien
-00014c50: 745f 6469 6374 5b27 6964 275d 2c20 7061  t_dict['id'], pa
-00014c60: 7469 656e 743d 7061 7469 656e 7429 0a20  tient=patient). 
-00014c70: 2020 2020 2020 2020 2020 2061 6374 6976             activ
-00014c80: 6520 3d20 7061 7469 656e 745f 6469 6374  e = patient_dict
-00014c90: 5b27 6163 7469 7665 275d 2069 6620 2761  ['active'] if 'a
-00014ca0: 6374 6976 6527 2069 6e20 7061 7469 656e  ctive' in patien
-00014cb0: 745f 6469 6374 2065 6c73 6520 5472 7565  t_dict else True
-00014cc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014cd0: 662e 7365 745f 6163 7469 7665 2861 6374  f.set_active(act
-00014ce0: 6976 653d 6163 7469 7665 2c20 7061 7469  ive=active, pati
-00014cf0: 656e 743d 7061 7469 656e 7429 0a20 2020  ent=patient).   
-00014d00: 2020 2020 2020 2020 2069 6620 2761 6464           if 'add
-00014d10: 7265 7373 5f6c 696e 6527 2069 6e20 7061  ress_line' in pa
-00014d20: 7469 656e 745f 6469 6374 206f 7220 2761  tient_dict or 'a
-00014d30: 6464 7265 7373 5f63 6974 7927 2069 6e20  ddress_city' in 
-00014d40: 7061 7469 656e 745f 6469 6374 206f 7220  patient_dict or 
-00014d50: 2761 6464 7265 7373 5f70 6f73 7461 6c5f  'address_postal_
-00014d60: 636f 6465 2720 696e 2070 6174 6965 6e74  code' in patient
-00014d70: 5f64 6963 7420 6f72 2027 6164 6472 6573  _dict or 'addres
-00014d80: 735f 7374 6174 6527 2069 6e20 7061 7469  s_state' in pati
-00014d90: 656e 745f 6469 6374 206f 7220 2761 6464  ent_dict or 'add
-00014da0: 7265 7373 5f63 6f75 6e74 7279 2720 696e  ress_country' in
-00014db0: 2070 6174 6965 6e74 5f64 6963 743a 0a20   patient_dict:. 
-00014dc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00014dd0: 6464 7265 7373 5f6c 696e 6520 3d20 7061  ddress_line = pa
-00014de0: 7469 656e 745f 6469 6374 5b27 6164 6472  tient_dict['addr
-00014df0: 6573 735f 6c69 6e65 275d 2069 6620 2761  ess_line'] if 'a
-00014e00: 6464 7265 7373 5f6c 696e 6527 2069 6e20  ddress_line' in 
-00014e10: 7061 7469 656e 745f 6469 6374 2065 6c73  patient_dict els
-00014e20: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
-00014e30: 2020 2020 2020 2061 6464 7265 7373 5f63         address_c
-00014e40: 6974 7920 3d20 7061 7469 656e 745f 6469  ity = patient_di
-00014e50: 6374 5b27 6164 6472 6573 735f 6369 7479  ct['address_city
-00014e60: 275d 2069 6620 2761 6464 7265 7373 5f63  '] if 'address_c
-00014e70: 6974 7927 2069 6e20 7061 7469 656e 745f  ity' in patient_
-00014e80: 6469 6374 2065 6c73 6520 4e6f 6e65 0a20  dict else None. 
-00014e90: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00014ea0: 6464 7265 7373 5f73 7461 7465 203d 2070  ddress_state = p
-00014eb0: 6174 6965 6e74 5f64 6963 745b 2761 6464  atient_dict['add
-00014ec0: 7265 7373 5f73 7461 7465 275d 2069 6620  ress_state'] if 
-00014ed0: 2761 6464 7265 7373 5f73 7461 7465 2720  'address_state' 
-00014ee0: 696e 2070 6174 6965 6e74 5f64 6963 7420  in patient_dict 
-00014ef0: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
-00014f00: 2020 2020 2020 2020 2020 6164 6472 6573            addres
-00014f10: 735f 706f 7374 616c 5f63 6f64 6520 3d20  s_postal_code = 
-00014f20: 7061 7469 656e 745f 6469 6374 5b27 6164  patient_dict['ad
-00014f30: 6472 6573 735f 706f 7374 616c 5f63 6f64  dress_postal_cod
-00014f40: 6527 5d20 6966 2027 6164 6472 6573 735f  e'] if 'address_
-00014f50: 706f 7374 616c 5f63 6f64 6527 2069 6e20  postal_code' in 
-00014f60: 7061 7469 656e 745f 6469 6374 2065 6c73  patient_dict els
-00014f70: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
-00014f80: 2020 2020 2020 2061 6464 7265 7373 5f63         address_c
-00014f90: 6f75 6e74 7279 203d 2070 6174 6965 6e74  ountry = patient
-00014fa0: 5f64 6963 745b 2761 6464 7265 7373 5f63  _dict['address_c
-00014fb0: 6f75 6e74 7279 275d 2069 6620 2761 6464  ountry'] if 'add
-00014fc0: 7265 7373 5f63 6f75 6e74 7279 2720 696e  ress_country' in
-00014fd0: 2070 6174 6965 6e74 5f64 6963 7420 656c   patient_dict el
-00014fe0: 7365 204e 6f6e 650a 2020 2020 2020 2020  se None.        
-00014ff0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00015000: 5f61 6464 7265 7373 280a 2020 2020 2020  _address(.      
-00015010: 2020 2020 2020 2020 2020 2020 2020 6164                ad
-00015020: 6472 6573 735f 6369 7479 3d61 6464 7265  dress_city=addre
-00015030: 7373 5f63 6974 792c 0a20 2020 2020 2020  ss_city,.       
-00015040: 2020 2020 2020 2020 2020 2020 2061 6464               add
-00015050: 7265 7373 5f63 6f75 6e74 7279 3d61 6464  ress_country=add
-00015060: 7265 7373 5f63 6f75 6e74 7279 2c0a 2020  ress_country,.  
-00015070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015080: 2020 6164 6472 6573 735f 6c69 6e65 3d61    address_line=a
-00015090: 6464 7265 7373 5f6c 696e 652c 0a20 2020  ddress_line,.   
-000150a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150b0: 2061 6464 7265 7373 5f73 7461 7465 3d61   address_state=a
-000150c0: 6464 7265 7373 5f73 7461 7465 2c0a 2020  ddress_state,.  
-000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150e0: 2020 6164 6472 6573 735f 706f 7374 616c    address_postal
-000150f0: 5f63 6f64 653d 6164 6472 6573 735f 706f  _code=address_po
-00015100: 7374 616c 5f63 6f64 652c 0a20 2020 2020  stal_code,.     
-00015110: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00015120: 6174 6965 6e74 3d70 6174 6965 6e74 290a  atient=patient).
-00015130: 2020 2020 2020 2020 2020 2020 6966 2027              if '
-00015140: 6d6f 7468 6572 5f67 6976 656e 5f6e 616d  mother_given_nam
-00015150: 6527 2069 6e20 7061 7469 656e 745f 6469  e' in patient_di
-00015160: 6374 206f 7220 276d 6f74 6865 725f 6661  ct or 'mother_fa
-00015170: 6d69 6c79 5f6e 616d 6527 2069 6e20 7061  mily_name' in pa
-00015180: 7469 656e 745f 6469 6374 3a0a 2020 2020  tient_dict:.    
-00015190: 2020 2020 2020 2020 2020 2020 6d6f 7468              moth
-000151a0: 6572 5f67 6976 656e 5f6e 616d 6520 3d20  er_given_name = 
-000151b0: 7061 7469 656e 745f 6469 6374 5b27 6d6f  patient_dict['mo
-000151c0: 7468 6572 5f67 6976 656e 5f6e 616d 6527  ther_given_name'
-000151d0: 5d20 6966 2027 6d6f 7468 6572 5f67 6976  ] if 'mother_giv
-000151e0: 656e 5f6e 616d 6527 2069 6e20 7061 7469  en_name' in pati
-000151f0: 656e 745f 6469 6374 2065 6c73 6520 4e6f  ent_dict else No
-00015200: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-00015210: 2020 206d 6f74 6865 725f 6661 6d69 6c79     mother_family
-00015220: 5f6e 616d 6520 3d20 7061 7469 656e 745f  _name = patient_
-00015230: 6469 6374 5b27 6d6f 7468 6572 5f66 616d  dict['mother_fam
-00015240: 696c 795f 6e61 6d65 275d 2069 6620 276d  ily_name'] if 'm
-00015250: 6f74 6865 725f 6661 6d69 6c79 5f6e 616d  other_family_nam
-00015260: 6527 2069 6e20 7061 7469 656e 745f 6469  e' in patient_di
-00015270: 6374 2065 6c73 6520 4e6f 6e65 0a20 2020  ct else None.   
-00015280: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015290: 662e 7365 745f 6d6f 7468 6572 5f6e 616d  f.set_mother_nam
-000152a0: 6528 6d6f 7468 6572 5f66 616d 696c 795f  e(mother_family_
-000152b0: 6e61 6d65 3d6d 6f74 6865 725f 6661 6d69  name=mother_fami
-000152c0: 6c79 5f6e 616d 652c 206d 6f74 6865 725f  ly_name, mother_
-000152d0: 6769 7665 6e5f 6e61 6d65 3d6d 6f74 6865  given_name=mothe
-000152e0: 725f 6769 7665 6e5f 6e61 6d65 2c20 7061  r_given_name, pa
-000152f0: 7469 656e 743d 7061 7469 656e 742c 2063  tient=patient, c
-00015300: 6f64 696e 675f 7379 7374 656d 3d70 6174  oding_system=pat
-00015310: 6965 6e74 5f63 6f64 696e 675f 7379 7374  ient_coding_syst
-00015320: 656d 2c20 636f 6469 6e67 5f76 6572 7369  em, coding_versi
-00015330: 6f6e 3d70 6174 6965 6e74 5f63 6f64 696e  on=patient_codin
-00015340: 675f 7665 7273 696f 6e29 0a0a 2020 2020  g_version)..    
-00015350: 2020 2020 2020 2020 6966 2027 6661 7468          if 'fath
-00015360: 6572 5f67 6976 656e 5f6e 616d 6527 2069  er_given_name' i
-00015370: 6e20 7061 7469 656e 745f 6469 6374 206f  n patient_dict o
-00015380: 7220 2766 6174 6865 725f 6661 6d69 6c79  r 'father_family
-00015390: 5f6e 616d 6527 2069 6e20 7061 7469 656e  _name' in patien
-000153a0: 745f 6469 6374 3a0a 2020 2020 2020 2020  t_dict:.        
-000153b0: 2020 2020 2020 2020 6661 7468 6572 5f67          father_g
-000153c0: 6976 656e 5f6e 616d 6520 3d20 7061 7469  iven_name = pati
-000153d0: 656e 745f 6469 6374 5b27 6661 7468 6572  ent_dict['father
-000153e0: 5f67 6976 656e 5f6e 616d 6527 5d20 6966  _given_name'] if
-000153f0: 2027 6661 7468 6572 5f67 6976 656e 5f6e   'father_given_n
-00015400: 616d 6527 2069 6e20 7061 7469 656e 745f  ame' in patient_
-00015410: 6469 6374 2065 6c73 6520 4e6f 6e65 0a20  dict else None. 
-00015420: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00015430: 6174 6865 725f 6661 6d69 6c79 5f6e 616d  ather_family_nam
-00015440: 6520 3d20 7061 7469 656e 745f 6469 6374  e = patient_dict
-00015450: 5b27 6661 7468 6572 5f66 616d 696c 795f  ['father_family_
-00015460: 6e61 6d65 275d 2069 6620 2766 6174 6865  name'] if 'fathe
-00015470: 725f 6661 6d69 6c79 5f6e 616d 6527 2069  r_family_name' i
-00015480: 6e20 7061 7469 656e 745f 6469 6374 2065  n patient_dict e
-00015490: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
-000154a0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000154b0: 745f 6661 7468 6572 5f6e 616d 6528 6661  t_father_name(fa
-000154c0: 7468 6572 5f66 616d 696c 795f 6e61 6d65  ther_family_name
-000154d0: 3d66 6174 6865 725f 6661 6d69 6c79 5f6e  =father_family_n
-000154e0: 616d 652c 2066 6174 6865 725f 6769 7665  ame, father_give
-000154f0: 6e5f 6e61 6d65 3d66 6174 6865 725f 6769  n_name=father_gi
-00015500: 7665 6e5f 6e61 6d65 2c20 7061 7469 656e  ven_name, patien
-00015510: 743d 7061 7469 656e 742c 2063 6f64 696e  t=patient, codin
-00015520: 675f 7379 7374 656d 3d70 6174 6965 6e74  g_system=patient
-00015530: 5f63 6f64 696e 675f 7379 7374 656d 2c20  _coding_system, 
-00015540: 636f 6469 6e67 5f76 6572 7369 6f6e 3d70  coding_version=p
-00015550: 6174 6965 6e74 5f63 6f64 696e 675f 7665  atient_coding_ve
-00015560: 7273 696f 6e29 0a20 2020 2020 2020 2020  rsion).         
-00015570: 2020 2069 6620 2770 686f 6e65 5f6e 756d     if 'phone_num
-00015580: 6265 7227 2069 6e20 7061 7469 656e 745f  ber' in patient_
-00015590: 6469 6374 3a0a 2020 2020 2020 2020 2020  dict:.          
-000155a0: 2020 2020 2020 7365 6c66 2e73 6574 5f70        self.set_p
-000155b0: 686f 6e65 5f6e 756d 6265 7228 7068 6f6e  hone_number(phon
-000155c0: 655f 6e75 6d62 6572 3d70 6174 6965 6e74  e_number=patient
-000155d0: 5f64 6963 745b 2770 686f 6e65 5f6e 756d  _dict['phone_num
-000155e0: 6265 7227 5d2c 2070 6174 6965 6e74 3d70  ber'], patient=p
-000155f0: 6174 6965 6e74 290a 0a20 2020 2020 2020  atient)..       
-00015600: 2072 6574 7572 6e20 7061 7469 656e 740a   return patient.
-00015610: 0a20 2020 2064 6566 2066 726f 6d5f 6668  .    def from_fh
-00015620: 6972 5f70 6174 6965 6e74 2873 656c 662c  ir_patient(self,
-00015630: 2070 6174 6965 6e74 3d4e 6f6e 652c 2063   patient=None, c
-00015640: 6f64 696e 675f 7379 7374 656d 3d4e 6f6e  oding_system=Non
-00015650: 652c 2063 6f64 696e 675f 7665 7273 696f  e, coding_versio
-00015660: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
-00015670: 2069 6620 7061 7469 656e 7420 6973 204e   if patient is N
-00015680: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00015690: 2070 6174 6965 6e74 203d 2073 656c 662e   patient = self.
-000156a0: 6668 6972 5f72 6573 6f75 7263 650a 0a20  fhir_resource.. 
-000156b0: 2020 2020 2020 2073 656c 662e 6964 203d         self.id =
-000156c0: 2073 656c 662e 6765 745f 6964 2870 6174   self.get_id(pat
-000156d0: 6965 6e74 3d70 6174 6965 6e74 290a 2020  ient=patient).  
-000156e0: 2020 2020 2020 7365 6c66 2e6d 6174 6368        self.match
-000156f0: 7261 6d71 203d 2073 656c 662e 6765 745f  ramq = self.get_
-00015700: 6d61 7463 6872 616d 7128 7061 7469 656e  matchramq(patien
-00015710: 743d 7061 7469 656e 7429 0a20 2020 2020  t=patient).     
-00015720: 2020 2073 656c 662e 6e61 6d20 3d20 7365     self.nam = se
-00015730: 6c66 2e67 6574 5f6e 616d 2870 6174 6965  lf.get_nam(patie
-00015740: 6e74 3d70 6174 6965 6e74 290a 2020 2020  nt=patient).    
-00015750: 2020 2020 7365 6c66 2e6e 6975 203d 2073      self.niu = s
-00015760: 656c 662e 6765 745f 6e69 7528 7061 7469  elf.get_niu(pati
-00015770: 656e 743d 7061 7469 656e 7429 0a20 2020  ent=patient).   
-00015780: 2020 2020 2073 656c 662e 6769 7665 6e5f       self.given_
-00015790: 6e61 6d65 203d 2073 656c 662e 6765 745f  name = self.get_
-000157a0: 6769 7665 6e5f 6e61 6d65 2870 6174 6965  given_name(patie
-000157b0: 6e74 3d70 6174 6965 6e74 290a 2020 2020  nt=patient).    
-000157c0: 2020 2020 7365 6c66 2e66 616d 696c 795f      self.family_
-000157d0: 6e61 6d65 203d 2073 656c 662e 6765 745f  name = self.get_
-000157e0: 6661 6d69 6c79 5f6e 616d 6528 7061 7469  family_name(pati
-000157f0: 656e 743d 7061 7469 656e 7429 0a20 2020  ent=patient).   
-00015800: 2020 2020 2073 656c 662e 6163 7469 7665       self.active
-00015810: 203d 2073 656c 662e 6765 745f 6163 7469   = self.get_acti
-00015820: 7665 2870 6174 6965 6e74 3d70 6174 6965  ve(patient=patie
-00015830: 6e74 290a 2020 2020 2020 2020 7365 6c66  nt).        self
-00015840: 2e67 656e 6465 7220 3d20 7365 6c66 2e67  .gender = self.g
-00015850: 6574 5f67 656e 6465 7228 7061 7469 656e  et_gender(patien
-00015860: 743d 7061 7469 656e 7429 0a20 2020 2020  t=patient).     
-00015870: 2020 2073 656c 662e 6269 7274 685f 6461     self.birth_da
-00015880: 7465 203d 2073 656c 662e 6765 745f 6269  te = self.get_bi
-00015890: 7274 685f 6461 7465 2870 6174 6965 6e74  rth_date(patient
-000158a0: 3d70 6174 6965 6e74 290a 2020 2020 2020  =patient).      
-000158b0: 2020 6164 6472 6573 7320 3d20 7365 6c66    address = self
-000158c0: 2e67 6574 5f61 6464 7265 7373 2870 6174  .get_address(pat
-000158d0: 6965 6e74 3d70 6174 6965 6e74 290a 2020  ient=patient).  
-000158e0: 2020 2020 2020 6966 2061 6464 7265 7373        if address
-000158f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00015900: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00015910: 6464 7265 7373 5f6c 696e 6520 3d20 6164  ddress_line = ad
-00015920: 6472 6573 732e 6c69 6e65 0a20 2020 2020  dress.line.     
-00015930: 2020 2020 2020 2073 656c 662e 6164 6472         self.addr
-00015940: 6573 735f 6369 7479 203d 2061 6464 7265  ess_city = addre
-00015950: 7373 2e63 6974 790a 2020 2020 2020 2020  ss.city.        
-00015960: 2020 2020 7365 6c66 2e61 6464 7265 7373      self.address
-00015970: 5f73 7461 7465 203d 2061 6464 7265 7373  _state = address
-00015980: 2e73 7461 7465 0a20 2020 2020 2020 2020  .state.         
-00015990: 2020 2073 656c 662e 6164 6472 6573 735f     self.address_
-000159a0: 706f 7374 616c 5f63 6f64 6520 3d20 6164  postal_code = ad
-000159b0: 6472 6573 732e 706f 7374 616c 436f 6465  dress.postalCode
-000159c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000159d0: 662e 6164 6472 6573 735f 636f 756e 7472  f.address_countr
-000159e0: 7920 3d20 6164 6472 6573 732e 636f 756e  y = address.coun
-000159f0: 7472 790a 2020 2020 2020 2020 6d6f 7468  try.        moth
-00015a00: 6572 5f6e 616d 6520 3d20 2073 656c 662e  er_name =  self.
-00015a10: 6765 745f 6d6f 7468 6572 5f6e 616d 6528  get_mother_name(
-00015a20: 7061 7469 656e 743d 7061 7469 656e 742c  patient=patient,
-00015a30: 2063 6f64 696e 675f 7379 7374 656d 3d63   coding_system=c
-00015a40: 6f64 696e 675f 7379 7374 656d 2c20 636f  oding_system, co
-00015a50: 6469 6e67 5f76 6572 7369 6f6e 3d63 6f64  ding_version=cod
-00015a60: 696e 675f 7665 7273 696f 6e29 0a20 2020  ing_version).   
-00015a70: 2020 2020 2069 6620 6d6f 7468 6572 5f6e       if mother_n
-00015a80: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-00015a90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015aa0: 662e 6d6f 7468 6572 5f67 6976 656e 5f6e  f.mother_given_n
-00015ab0: 616d 6520 3d20 6d6f 7468 6572 5f6e 616d  ame = mother_nam
-00015ac0: 652e 6769 7665 6e0a 2020 2020 2020 2020  e.given.        
-00015ad0: 2020 2020 7365 6c66 2e6d 6f74 6865 725f      self.mother_
-00015ae0: 6661 6d69 6c79 5f6e 616d 6520 3d20 6d6f  family_name = mo
-00015af0: 7468 6572 5f6e 616d 652e 6661 6d69 6c79  ther_name.family
-00015b00: 0a20 2020 2020 2020 2066 6174 6865 725f  .        father_
-00015b10: 6e61 6d65 203d 2073 656c 662e 6765 745f  name = self.get_
-00015b20: 6661 7468 6572 5f6e 616d 6528 7061 7469  father_name(pati
-00015b30: 656e 743d 7061 7469 656e 742c 2063 6f64  ent=patient, cod
-00015b40: 696e 675f 7379 7374 656d 3d63 6f64 696e  ing_system=codin
-00015b50: 675f 7379 7374 656d 2c20 636f 6469 6e67  g_system, coding
-00015b60: 5f76 6572 7369 6f6e 3d63 6f64 696e 675f  _version=coding_
-00015b70: 7665 7273 696f 6e29 0a20 2020 2020 2020  version).       
-00015b80: 2069 6620 6661 7468 6572 5f6e 616d 6520   if father_name 
-00015b90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00015ba0: 2020 2020 2020 2020 2073 656c 662e 6661           self.fa
-00015bb0: 7468 6572 5f67 6976 656e 5f6e 616d 6520  ther_given_name 
-00015bc0: 3d20 6661 7468 6572 5f6e 616d 652e 6769  = father_name.gi
-00015bd0: 7665 6e0a 2020 2020 2020 2020 2020 2020  ven.            
-00015be0: 7365 6c66 2e66 6174 6865 725f 6661 6d69  self.father_fami
-00015bf0: 6c79 5f6e 616d 6520 3d20 6661 7468 6572  ly_name = father
-00015c00: 5f6e 616d 652e 6661 6d69 6c79 0a20 2020  _name.family.   
-00015c10: 2020 2020 2073 656c 662e 7068 6f6e 655f       self.phone_
-00015c20: 6e75 6d62 6572 203d 2073 656c 662e 6765  number = self.ge
-00015c30: 745f 7068 6f6e 655f 6e75 6d62 6572 2870  t_phone_number(p
-00015c40: 6174 6965 6e74 3d70 6174 6965 6e74 290a  atient=patient).
-00015c50: 2020 2020 2020 2020 0a20 2020 2064 6566          .    def
-00015c60: 2074 6f5f 6668 6972 5f70 6174 6965 6e74   to_fhir_patient
-00015c70: 2873 656c 662c 2070 6174 6965 6e74 3d4e  (self, patient=N
-00015c80: 6f6e 652c 2063 6f64 696e 675f 7379 7374  one, coding_syst
-00015c90: 656d 3d4e 6f6e 652c 2063 6f64 696e 675f  em=None, coding_
-00015ca0: 7665 7273 696f 6e3d 4e6f 6e65 293a 0a20  version=None):. 
-00015cb0: 2020 2020 2020 2069 6620 7061 7469 656e         if patien
-00015cc0: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
-00015cd0: 2020 2020 2020 2070 6174 6965 6e74 203d         patient =
-00015ce0: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
-00015cf0: 7263 650a 0a20 2020 2020 2020 2069 6620  rce..        if 
-00015d00: 7365 6c66 2e69 6420 6973 206e 6f74 204e  self.id is not N
-00015d10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00015d20: 2073 656c 662e 7365 745f 6964 2869 643d   self.set_id(id=
-00015d30: 7365 6c66 2e69 642c 2070 6174 6965 6e74  self.id, patient
-00015d40: 3d70 6174 6965 6e74 290a 2020 2020 2020  =patient).      
-00015d50: 2020 6966 2073 656c 662e 6e69 7520 6973    if self.niu is
-00015d60: 204e 6f6e 6520 616e 6420 7365 6c66 2e6e   None and self.n
-00015d70: 616d 2069 7320 4e6f 6e65 3a0a 2020 2020  am is None:.    
-00015d80: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00015d90: 5f61 7563 756e 5f69 6465 6e74 6966 6961  _aucun_identifia
-00015da0: 6e74 2870 6174 6965 6e74 3d70 6174 6965  nt(patient=patie
-00015db0: 6e74 290a 2020 2020 2020 2020 656c 7365  nt).        else
-00015dc0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00015dd0: 2073 656c 662e 6e61 6d20 6973 206e 6f74   self.nam is not
-00015de0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00015df0: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
-00015e00: 6e61 6d28 6e61 6d3d 7365 6c66 2e6e 616d  nam(nam=self.nam
-00015e10: 2c20 7061 7469 656e 743d 7061 7469 656e  , patient=patien
-00015e20: 7429 0a20 2020 2020 2020 2020 2020 2069  t).            i
-00015e30: 6620 7365 6c66 2e6e 6975 2069 7320 6e6f  f self.niu is no
-00015e40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00015e50: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00015e60: 5f6e 6975 286e 6975 3d73 656c 662e 6e69  _niu(niu=self.ni
-00015e70: 752c 2070 6174 6965 6e74 3d70 6174 6965  u, patient=patie
-00015e80: 6e74 290a 2020 2020 2020 2020 7365 6c66  nt).        self
-00015e90: 2e73 6574 5f61 6374 6976 6528 6163 7469  .set_active(acti
-00015ea0: 7665 3d73 656c 662e 6163 7469 7665 2c20  ve=self.active, 
-00015eb0: 7061 7469 656e 743d 7061 7469 656e 7429  patient=patient)
-00015ec0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00015ed0: 745f 6d61 7463 6872 616d 7128 6d61 7463  t_matchramq(matc
-00015ee0: 6872 616d 713d 7365 6c66 2e6d 6174 6368  hramq=self.match
-00015ef0: 7261 6d71 2c20 7061 7469 656e 743d 7061  ramq, patient=pa
-00015f00: 7469 656e 7429 0a20 2020 2020 2020 2069  tient).        i
-00015f10: 6620 7365 6c66 2e61 6464 7265 7373 5f63  f self.address_c
-00015f20: 6974 7920 6973 206e 6f74 204e 6f6e 6520  ity is not None 
-00015f30: 6f72 2073 656c 662e 6164 6472 6573 735f  or self.address_
-00015f40: 636f 756e 7472 7920 6973 206e 6f74 204e  country is not N
-00015f50: 6f6e 6520 6f72 2073 656c 662e 6164 6472  one or self.addr
-00015f60: 6573 735f 6c69 6e65 2069 7320 6e6f 7420  ess_line is not 
-00015f70: 4e6f 6e65 206f 7220 7365 6c66 2e61 6464  None or self.add
-00015f80: 7265 7373 5f70 6f73 7461 6c5f 636f 6465  ress_postal_code
-00015f90: 2069 7320 6e6f 7420 4e6f 6e65 206f 7220   is not None or 
-00015fa0: 7365 6c66 2e61 6464 7265 7373 5f73 7461  self.address_sta
-00015fb0: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  te is not None:.
-00015fc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015fd0: 2e73 6574 5f61 6464 7265 7373 280a 2020  .set_address(.  
-00015fe0: 2020 2020 2020 2020 2020 2020 2020 6164                ad
-00015ff0: 6472 6573 735f 6369 7479 3d73 656c 662e  dress_city=self.
-00016000: 6164 6472 6573 735f 6369 7479 2c0a 2020  address_city,.  
-00016010: 2020 2020 2020 2020 2020 2020 2020 6164                ad
-00016020: 6472 6573 735f 636f 756e 7472 793d 7365  dress_country=se
-00016030: 6c66 2e61 6464 7265 7373 5f63 6f75 6e74  lf.address_count
-00016040: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
-00016050: 2020 2020 6164 6472 6573 735f 6c69 6e65      address_line
-00016060: 3d73 656c 662e 6164 6472 6573 735f 6c69  =self.address_li
-00016070: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00016080: 2020 2020 6164 6472 6573 735f 7374 6174      address_stat
-00016090: 653d 7365 6c66 2e61 6464 7265 7373 5f73  e=self.address_s
-000160a0: 7461 7465 2c0a 2020 2020 2020 2020 2020  tate,.          
-000160b0: 2020 2020 2020 6164 6472 6573 735f 706f        address_po
-000160c0: 7374 616c 5f63 6f64 653d 7365 6c66 2e61  stal_code=self.a
-000160d0: 6464 7265 7373 5f70 6f73 7461 6c5f 636f  ddress_postal_co
-000160e0: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
-000160f0: 2020 2020 7061 7469 656e 743d 7061 7469      patient=pati
-00016100: 656e 7429 2020 2020 2020 2020 2020 2020  ent)            
-00016110: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00016120: 2e62 6972 7468 5f64 6174 6520 6973 206e  .birth_date is n
-00016130: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00016140: 2020 2020 2073 656c 662e 7365 745f 6269       self.set_bi
-00016150: 7274 685f 6461 7465 2873 7472 5f64 6174  rth_date(str_dat
-00016160: 653d 7365 6c66 2e62 6972 7468 5f64 6174  e=self.birth_dat
-00016170: 652c 2070 6174 6965 6e74 3d70 6174 6965  e, patient=patie
-00016180: 6e74 290a 2020 2020 2020 2020 6966 2073  nt).        if s
-00016190: 656c 662e 6661 6d69 6c79 5f6e 616d 6520  elf.family_name 
-000161a0: 6973 206e 6f74 204e 6f6e 6520 6f72 2073  is not None or s
-000161b0: 656c 662e 6769 7665 6e5f 6e61 6d65 2069  elf.given_name i
-000161c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000161d0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-000161e0: 5f6e 616d 6528 6769 7665 6e5f 6e61 6d65  _name(given_name
-000161f0: 3d73 656c 662e 6769 7665 6e5f 6e61 6d65  =self.given_name
-00016200: 2c20 6661 6d69 6c79 5f6e 616d 653d 7365  , family_name=se
-00016210: 6c66 2e66 616d 696c 795f 6e61 6d65 290a  lf.family_name).
-00016220: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00016230: 6661 7468 6572 5f66 616d 696c 795f 6e61  father_family_na
-00016240: 6d65 2069 7320 6e6f 7420 4e6f 6e65 206f  me is not None o
-00016250: 7220 7365 6c66 2e66 6174 6865 725f 6769  r self.father_gi
-00016260: 7665 6e5f 6e61 6d65 2069 7320 6e6f 7420  ven_name is not 
-00016270: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00016280: 2020 7365 6c66 2e73 6574 5f66 6174 6865    self.set_fathe
-00016290: 725f 6e61 6d65 2866 6174 6865 725f 6769  r_name(father_gi
-000162a0: 7665 6e5f 6e61 6d65 3d73 656c 662e 6661  ven_name=self.fa
-000162b0: 7468 6572 5f67 6976 656e 5f6e 616d 652c  ther_given_name,
-000162c0: 2066 6174 6865 725f 6661 6d69 6c79 5f6e   father_family_n
-000162d0: 616d 653d 7365 6c66 2e66 6174 6865 725f  ame=self.father_
-000162e0: 6661 6d69 6c79 5f6e 616d 652c 2063 6f64  family_name, cod
-000162f0: 696e 675f 7379 7374 656d 3d63 6f64 696e  ing_system=codin
-00016300: 675f 7379 7374 656d 2c20 636f 6469 6e67  g_system, coding
-00016310: 5f76 6572 7369 6f6e 3d63 6f64 696e 675f  _version=coding_
-00016320: 7665 7273 696f 6e29 0a20 2020 2020 2020  version).       
-00016330: 2069 6620 7365 6c66 2e6d 6f74 6865 725f   if self.mother_
-00016340: 6661 6d69 6c79 5f6e 616d 6520 6973 206e  family_name is n
-00016350: 6f74 204e 6f6e 6520 6f72 2073 656c 662e  ot None or self.
-00016360: 6d6f 7468 6572 5f67 6976 656e 5f6e 616d  mother_given_nam
-00016370: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00016380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016390: 7365 745f 6d6f 7468 6572 5f6e 616d 6528  set_mother_name(
-000163a0: 6d6f 7468 6572 5f67 6976 656e 5f6e 616d  mother_given_nam
-000163b0: 653d 7365 6c66 2e6d 6f74 6865 725f 6769  e=self.mother_gi
-000163c0: 7665 6e5f 6e61 6d65 2c20 6d6f 7468 6572  ven_name, mother
-000163d0: 5f66 616d 696c 795f 6e61 6d65 3d73 656c  _family_name=sel
-000163e0: 662e 6d6f 7468 6572 5f66 616d 696c 795f  f.mother_family_
-000163f0: 6e61 6d65 2c20 636f 6469 6e67 5f73 7973  name, coding_sys
-00016400: 7465 6d3d 636f 6469 6e67 5f73 7973 7465  tem=coding_syste
-00016410: 6d2c 2063 6f64 696e 675f 7665 7273 696f  m, coding_versio
-00016420: 6e3d 636f 6469 6e67 5f76 6572 7369 6f6e  n=coding_version
-00016430: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00016440: 6574 5f67 656e 6465 7228 6765 6e64 6572  et_gender(gender
-00016450: 3d73 656c 662e 6765 6e64 6572 2c20 7061  =self.gender, pa
-00016460: 7469 656e 743d 7061 7469 656e 7429 0a20  tient=patient). 
-00016470: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00016480: 686f 6e65 5f6e 756d 6265 7220 6973 206e  hone_number is n
-00016490: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000164a0: 2020 2020 2073 656c 662e 7365 745f 7068       self.set_ph
-000164b0: 6f6e 655f 6e75 6d62 6572 2870 686f 6e65  one_number(phone
-000164c0: 5f6e 756d 6265 723d 7365 6c66 2e70 686f  _number=self.pho
-000164d0: 6e65 5f6e 756d 6265 722c 2070 6174 6965  ne_number, patie
-000164e0: 6e74 3d70 6174 6965 6e74 290a 0a63 6c61  nt=patient)..cla
-000164f0: 7373 204f 7267 616e 697a 6174 696f 6e46  ss OrganizationF
-00016500: 4849 5228 4261 7365 4648 4952 293a 0a20  HIR(BaseFHIR):. 
-00016510: 2020 206f 7267 616e 697a 6174 696f 6e5f     organization_
-00016520: 656e 6470 6f69 6e74 203d 2022 7b62 6173  endpoint = "{bas
-00016530: 655f 7572 6c7d 2f4f 7267 616e 697a 6174  e_url}/Organizat
-00016540: 696f 6e22 0a20 2020 2073 6561 7263 685f  ion".    search_
-00016550: 656e 6470 6f69 6e74 203d 206f 7267 616e  endpoint = organ
-00016560: 697a 6174 696f 6e5f 656e 6470 6f69 6e74  ization_endpoint
-00016570: 202b 2022 2f5f 7365 6172 6368 220a 2020   + "/_search".  
-00016580: 2020 6f72 6761 6e69 7a61 7469 6f6e 5f62    organization_b
-00016590: 795f 6964 5f65 6e64 706f 696e 7420 3d20  y_id_endpoint = 
-000165a0: 6f72 6761 6e69 7a61 7469 6f6e 5f65 6e64  organization_end
-000165b0: 706f 696e 7420 2b20 222f 7b69 647d 220a  point + "/{id}".
-000165c0: 2020 2020 7272 7373 5f73 7973 7465 6d20      rrss_system 
-000165d0: 3d20 2768 7474 7073 3a2f 2f70 726f 2e63  = 'https://pro.c
-000165e0: 6f6e 7375 6c74 6174 696f 6e2e 7272 7373  onsultation.rrss
-000165f0: 2e72 7473 732e 7163 2e63 6127 0a20 2020  .rtss.qc.ca'.   
-00016600: 2072 7273 735f 6d6f 745f 636c 655f 6578   rrss_mot_cle_ex
-00016610: 7465 6e73 696f 6e5f 7572 6c20 3d20 2768  tension_url = 'h
-00016620: 7474 703a 2f2f 7777 772e 7361 6e74 6570  ttp://www.santep
-00016630: 7562 6c69 7175 652e 7274 7373 2e71 632e  ublique.rtss.qc.
-00016640: 6361 2f73 6970 6d69 2f72 7273 732f 312e  ca/sipmi/rrss/1.
-00016650: 302e 302f 6578 7465 6e73 696f 6e73 2f23  0.0/extensions/#
-00016660: 6d6f 7473 636c 6573 270a 2020 2020 7065  motscles'.    pe
-00016670: 7269 6f64 5f75 726c 203d 2022 6874 7470  riod_url = "http
-00016680: 3a2f 2f77 7777 2e73 616e 7465 7075 626c  ://www.santepubl
-00016690: 6971 7565 2e72 7473 732e 7163 2e63 612f  ique.rtss.qc.ca/
-000166a0: 7369 706d 692f 7272 7373 2f31 2e30 2e30  sipmi/rrss/1.0.0
-000166b0: 2f65 7874 656e 7369 6f6e 732f 7065 7269  /extensions/peri
-000166c0: 6f64 220a 0a20 2020 2064 6566 205f 5f69  od"..    def __i
-000166d0: 6e69 745f 5f28 7365 6c66 2c20 6261 7365  nit__(self, base
-000166e0: 5f75 726c 3d4e 6f6e 652c 2062 6173 655f  _url=None, base_
-000166f0: 7572 693d 4e6f 6e65 2c20 7265 736f 7572  uri=None, resour
-00016700: 6365 3d4e 6f6e 652c 2074 6f6b 656e 5f68  ce=None, token_h
-00016710: 6561 6465 723d 4e6f 6e65 2c20 7661 6c69  eader=None, vali
-00016720: 6461 7465 5f63 6572 7473 3d54 7275 6529  date_certs=True)
-00016730: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00016740: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-00016750: 5f5f 2862 6173 655f 7572 6c3d 6261 7365  __(base_url=base
-00016760: 5f75 726c 2c20 6261 7365 5f75 7269 3d62  _url, base_uri=b
-00016770: 6173 655f 7572 692c 2074 6f6b 656e 5f68  ase_uri, token_h
-00016780: 6561 6465 723d 746f 6b65 6e5f 6865 6164  eader=token_head
-00016790: 6572 290a 2020 2020 2020 2020 7365 6c66  er).        self
-000167a0: 2e76 616c 6964 6174 655f 6365 7274 7320  .validate_certs 
-000167b0: 3d20 7661 6c69 6461 7465 5f63 6572 7473  = validate_certs
-000167c0: 0a20 2020 2020 2020 2069 6620 7265 736f  .        if reso
-000167d0: 7572 6365 2069 7320 6e6f 7420 4e6f 6e65  urce is not None
-000167e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000167f0: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
-00016800: 203d 204f 7267 616e 697a 6174 696f 6e28   = Organization(
-00016810: 6a73 6f6e 6469 6374 3d72 6573 6f75 7263  jsondict=resourc
-00016820: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
-00016830: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00016840: 662e 6668 6972 5f72 6573 6f75 7263 6520  f.fhir_resource 
-00016850: 3d20 4f72 6761 6e69 7a61 7469 6f6e 2829  = Organization()
-00016860: 0a0a 2020 2020 6465 6620 6765 7446 6869  ..    def getFhi
-00016870: 7252 6573 6f75 7263 6528 7365 6c66 293a  rResource(self):
-00016880: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00016890: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
-000168a0: 6365 2e61 735f 6a73 6f6e 2829 0a0a 2020  ce.as_json()..  
-000168b0: 2020 6465 6620 6765 745f 6964 2873 656c    def get_id(sel
-000168c0: 662c 206f 7267 616e 697a 6174 696f 6e3d  f, organization=
-000168d0: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
-000168e0: 6620 6f72 6761 6e69 7a61 7469 6f6e 2069  f organization i
-000168f0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00016900: 2020 2020 6f72 6761 6e69 7a61 7469 6f6e      organization
-00016910: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
-00016920: 6f75 7263 650a 2020 2020 2020 2020 7265  ource.        re
-00016930: 7475 726e 206f 7267 616e 697a 6174 696f  turn organizatio
-00016940: 6e2e 6964 0a0a 2020 2020 6465 6620 6765  n.id..    def ge
-00016950: 745f 6964 5f72 7273 7328 7365 6c66 2c20  t_id_rrss(self, 
-00016960: 6f72 6761 6e69 7a61 7469 6f6e 3d4e 6f6e  organization=Non
-00016970: 6529 3a0a 2020 2020 2020 2020 6966 206f  e):.        if o
-00016980: 7267 616e 697a 6174 696f 6e20 6973 204e  rganization is N
-00016990: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000169a0: 206f 7267 616e 697a 6174 696f 6e20 3d20   organization = 
-000169b0: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
-000169c0: 6365 0a20 2020 2020 2020 2069 6620 6f72  ce.        if or
-000169d0: 6761 6e69 7a61 7469 6f6e 2e69 6465 6e74  ganization.ident
-000169e0: 6966 6965 7220 6973 206e 6f74 204e 6f6e  ifier is not Non
-000169f0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-00016a00: 6f72 2069 6465 6e74 6966 6965 7220 696e  or identifier in
-00016a10: 206f 7267 616e 697a 6174 696f 6e2e 6964   organization.id
-00016a20: 656e 7469 6669 6572 3a0a 2020 2020 2020  entifier:.      
-00016a30: 2020 2020 2020 2020 2020 6966 2069 6465            if ide
-00016a40: 6e74 6966 6965 722e 7379 7374 656d 203d  ntifier.system =
-00016a50: 3d20 7365 6c66 2e72 7273 735f 7379 7374  = self.rrss_syst
-00016a60: 656d 3a0a 2020 2020 2020 2020 2020 2020  em:.            
-00016a70: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00016a80: 6465 6e74 6966 6965 722e 7661 6c75 650a  dentifier.value.
-00016a90: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00016aa0: 6f6e 650a 0a20 2020 2064 6566 2073 6574  one..    def set
-00016ab0: 5f6e 616d 6528 7365 6c66 2c20 6f72 6761  _name(self, orga
-00016ac0: 6e69 7a61 7469 6f6e 3d4e 6f6e 652c 206e  nization=None, n
-00016ad0: 616d 653d 4e6f 6e65 293a 0a20 2020 2020  ame=None):.     
-00016ae0: 2020 2069 6620 6f72 6761 6e69 7a61 7469     if organizati
-00016af0: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-00016b00: 2020 2020 2020 2020 6f72 6761 6e69 7a61          organiza
-00016b10: 7469 6f6e 203d 2073 656c 662e 6668 6972  tion = self.fhir
-00016b20: 5f72 6573 6f75 7263 650a 0a20 2020 2020  _resource..     
-00016b30: 2020 206f 7267 616e 697a 6174 696f 6e2e     organization.
-00016b40: 6e61 6d65 203d 206e 616d 650a 0a20 2020  name = name..   
-00016b50: 2064 6566 2067 6574 5f6e 616d 6528 7365   def get_name(se
-00016b60: 6c66 2c20 6f72 6761 6e69 7a61 7469 6f6e  lf, organization
-00016b70: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00016b80: 6966 206f 7267 616e 697a 6174 696f 6e20  if organization 
-00016b90: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00016ba0: 2020 2020 206f 7267 616e 697a 6174 696f       organizatio
-00016bb0: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
-00016bc0: 736f 7572 6365 0a20 2020 2020 2020 2072  source.        r
-00016bd0: 6574 7572 6e20 6f72 6761 6e69 7a61 7469  eturn organizati
-00016be0: 6f6e 2e6e 616d 650a 0a20 2020 2064 6566  on.name..    def
-00016bf0: 2068 6176 655f 6d6f 745f 636c 6528 7365   have_mot_cle(se
-00016c00: 6c66 2c20 6f72 6761 6e69 7a61 7469 6f6e  lf, organization
-00016c10: 3d4e 6f6e 652c 206d 6f74 5f63 6c65 3d4e  =None, mot_cle=N
-00016c20: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-00016c30: 206f 7267 616e 697a 6174 696f 6e20 6973   organization is
-00016c40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00016c50: 2020 206f 7267 616e 697a 6174 696f 6e20     organization 
-00016c60: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
-00016c70: 7572 6365 0a20 2020 2020 2020 2069 6620  urce.        if 
-00016c80: 6d6f 745f 636c 6520 6973 206e 6f74 204e  mot_cle is not N
-00016c90: 6f6e 6520 616e 6420 6f72 6761 6e69 7a61  one and organiza
-00016ca0: 7469 6f6e 2e65 7874 656e 7369 6f6e 2069  tion.extension i
-00016cb0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00016cc0: 2020 2020 2020 2020 666f 7220 6578 7465          for exte
-00016cd0: 6e73 696f 6e20 696e 206f 7267 616e 697a  nsion in organiz
-00016ce0: 6174 696f 6e2e 6578 7465 6e73 696f 6e3a  ation.extension:
-00016cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016d00: 2069 6620 6578 7465 6e73 696f 6e2e 7572   if extension.ur
-00016d10: 6c20 3d3d 2073 656c 662e 7272 7373 5f6d  l == self.rrss_m
-00016d20: 6f74 5f63 6c65 5f65 7874 656e 7369 6f6e  ot_cle_extension
-00016d30: 5f75 726c 2061 6e64 2065 7874 656e 7369  _url and extensi
-00016d40: 6f6e 2e76 616c 7565 5374 7269 6e67 203d  on.valueString =
-00016d50: 3d20 6d6f 745f 636c 653a 0a20 2020 2020  = mot_cle:.     
-00016d60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00016d70: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00016d80: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00016d90: 0a20 2020 2064 6566 2067 6574 5f65 6666  .    def get_eff
-00016da0: 6563 7469 7665 5f66 726f 6d28 7365 6c66  ective_from(self
-00016db0: 2c20 6f72 6761 6e69 7a61 7469 6f6e 3d4e  , organization=N
-00016dc0: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-00016dd0: 206f 7267 616e 697a 6174 696f 6e20 6973   organization is
-00016de0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00016df0: 2020 206f 7267 616e 697a 6174 696f 6e20     organization 
-00016e00: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
-00016e10: 7572 6365 0a20 2020 2020 2020 2070 6572  urce.        per
-00016e20: 696f 645f 6578 7420 3d20 7365 6c66 2e67  iod_ext = self.g
-00016e30: 6574 5f70 6572 696f 645f 6578 7428 6f72  et_period_ext(or
-00016e40: 6761 6e69 7a61 7469 6f6e 3d6f 7267 616e  ganization=organ
-00016e50: 697a 6174 696f 6e29 0a20 2020 2020 2020  ization).       
-00016e60: 2069 6620 7065 7269 6f64 5f65 7874 2069   if period_ext i
-00016e70: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2070  s not None and p
-00016e80: 6572 696f 645f 6578 742e 7661 6c75 6550  eriod_ext.valueP
-00016e90: 6572 696f 6420 6973 206e 6f74 204e 6f6e  eriod is not Non
-00016ea0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00016eb0: 2020 2072 6574 7572 6e20 7065 7269 6f64     return period
-00016ec0: 5f65 7874 2e76 616c 7565 5065 7269 6f64  _ext.valuePeriod
-00016ed0: 2e73 7461 7274 0a20 2020 2020 2020 2072  .start.        r
-00016ee0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-00016ef0: 6465 6620 6765 745f 6566 6665 6374 6976  def get_effectiv
-00016f00: 655f 746f 2873 656c 662c 206f 7267 616e  e_to(self, organ
-00016f10: 697a 6174 696f 6e3d 4e6f 6e65 293a 0a20  ization=None):. 
-00016f20: 2020 2020 2020 2069 6620 6f72 6761 6e69         if organi
-00016f30: 7a61 7469 6f6e 2069 7320 4e6f 6e65 3a0a  zation is None:.
-00016f40: 2020 2020 2020 2020 2020 2020 6f72 6761              orga
-00016f50: 6e69 7a61 7469 6f6e 203d 2073 656c 662e  nization = self.
-00016f60: 6668 6972 5f72 6573 6f75 7263 650a 2020  fhir_resource.  
-00016f70: 2020 2020 2020 7065 7269 6f64 5f65 7874        period_ext
-00016f80: 203d 2073 656c 662e 6765 745f 7065 7269   = self.get_peri
-00016f90: 6f64 5f65 7874 286f 7267 616e 697a 6174  od_ext(organizat
-00016fa0: 696f 6e3d 6f72 6761 6e69 7a61 7469 6f6e  ion=organization
-00016fb0: 290a 2020 2020 2020 2020 6966 2070 6572  ).        if per
-00016fc0: 696f 645f 6578 7420 6973 206e 6f74 204e  iod_ext is not N
-00016fd0: 6f6e 6520 616e 6420 7065 7269 6f64 5f65  one and period_e
-00016fe0: 7874 2e76 616c 7565 5065 7269 6f64 2069  xt.valuePeriod i
-00016ff0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00017000: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00017010: 726e 2070 6572 696f 645f 6578 742e 7661  rn period_ext.va
-00017020: 6c75 6550 6572 696f 642e 656e 640a 2020  luePeriod.end.  
-00017030: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00017040: 650a 0a20 2020 2064 6566 2073 6574 5f65  e..    def set_e
-00017050: 6666 6563 7469 7665 5f66 726f 6d28 7365  ffective_from(se
-00017060: 6c66 2c20 6f72 6761 6e69 7a61 7469 6f6e  lf, organization
-00017070: 3d4e 6f6e 652c 2065 6666 6563 7469 7665  =None, effective
-00017080: 5f66 726f 6d3d 4e6f 6e65 293a 0a20 2020  _from=None):.   
-00017090: 2020 2020 2069 6620 6f72 6761 6e69 7a61       if organiza
-000170a0: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-000170b0: 2020 2020 2020 2020 2020 6f72 6761 6e69            organi
-000170c0: 7a61 7469 6f6e 203d 2073 656c 662e 6668  zation = self.fh
-000170d0: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
-000170e0: 2020 2020 6668 6972 5f65 6666 6563 7469      fhir_effecti
-000170f0: 7665 5f66 726f 6d20 3d20 4e6f 6e65 0a20  ve_from = None. 
-00017100: 2020 2020 2020 2069 6620 7479 7065 2865         if type(e
-00017110: 6666 6563 7469 7665 5f66 726f 6d29 2069  ffective_from) i
-00017120: 7320 7374 723a 0a20 2020 2020 2020 2020  s str:.         
-00017130: 2020 2066 6869 725f 6566 6665 6374 6976     fhir_effectiv
-00017140: 655f 6672 6f6d 203d 2046 4849 5244 6174  e_from = FHIRDat
-00017150: 6528 6a73 6f6e 7661 6c3d 6566 6665 6374  e(jsonval=effect
-00017160: 6976 655f 6672 6f6d 290a 2020 2020 2020  ive_from).      
-00017170: 2020 656c 6966 2074 7970 6528 6566 6665    elif type(effe
-00017180: 6374 6976 655f 6672 6f6d 2920 6973 2046  ctive_from) is F
-00017190: 4849 5244 6174 653a 0a20 2020 2020 2020  HIRDate:.       
-000171a0: 2020 2020 2066 6869 725f 6566 6665 6374       fhir_effect
-000171b0: 6976 655f 6672 6f6d 203d 2065 6666 6563  ive_from = effec
-000171c0: 7469 7665 5f66 726f 6d0a 2020 2020 2020  tive_from.      
-000171d0: 2020 7065 7269 6f64 5f65 7874 203d 2073    period_ext = s
-000171e0: 656c 662e 6765 745f 7065 7269 6f64 5f65  elf.get_period_e
-000171f0: 7874 2829 0a20 2020 2020 2020 2069 6620  xt().        if 
-00017200: 7065 7269 6f64 5f65 7874 2069 7320 4e6f  period_ext is No
-00017210: 6e65 206f 7220 7065 7269 6f64 5f65 7874  ne or period_ext
-00017220: 2e76 616c 7565 5065 7269 6f64 2069 7320  .valuePeriod is 
-00017230: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00017240: 2020 7065 7269 6f64 203d 2050 6572 696f    period = Perio
-00017250: 6428 290a 2020 2020 2020 2020 656c 7365  d().        else
-00017260: 3a0a 2020 2020 2020 2020 2020 2020 7065  :.            pe
-00017270: 7269 6f64 203d 2070 6572 696f 645f 6578  riod = period_ex
-00017280: 742e 7661 6c75 6550 6572 696f 640a 2020  t.valuePeriod.  
-00017290: 2020 2020 2020 7065 7269 6f64 2e73 7461        period.sta
-000172a0: 7274 203d 2066 6869 725f 6566 6665 6374  rt = fhir_effect
-000172b0: 6976 655f 6672 6f6d 0a20 2020 2020 2020  ive_from.       
-000172c0: 2073 656c 662e 7365 745f 7065 7269 6f64   self.set_period
-000172d0: 5f65 7874 286f 7267 616e 697a 6174 696f  _ext(organizatio
-000172e0: 6e3d 6f72 6761 6e69 7a61 7469 6f6e 2c20  n=organization, 
-000172f0: 7065 7269 6f64 3d70 6572 696f 6429 0a0a  period=period)..
-00017300: 2020 2020 6465 6620 7365 745f 6566 6665      def set_effe
-00017310: 6374 6976 655f 746f 2873 656c 662c 206f  ctive_to(self, o
-00017320: 7267 616e 697a 6174 696f 6e3d 4e6f 6e65  rganization=None
-00017330: 2c20 6566 6665 6374 6976 655f 746f 3d4e  , effective_to=N
-00017340: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-00017350: 206f 7267 616e 697a 6174 696f 6e20 6973   organization is
-00017360: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00017370: 2020 206f 7267 616e 697a 6174 696f 6e20     organization 
-00017380: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
-00017390: 7572 6365 0a20 2020 2020 2020 2066 6869  urce.        fhi
-000173a0: 725f 6566 6665 6374 6976 655f 746f 203d  r_effective_to =
-000173b0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-000173c0: 2074 7970 6528 6566 6665 6374 6976 655f   type(effective_
-000173d0: 746f 2920 6973 2073 7472 3a0a 2020 2020  to) is str:.    
-000173e0: 2020 2020 2020 2020 6668 6972 5f65 6666          fhir_eff
-000173f0: 6563 7469 7665 5f74 6f20 3d20 4648 4952  ective_to = FHIR
-00017400: 4461 7465 286a 736f 6e76 616c 3d65 6666  Date(jsonval=eff
-00017410: 6563 7469 7665 5f74 6f29 0a20 2020 2020  ective_to).     
-00017420: 2020 2065 6c69 6620 7479 7065 2865 6666     elif type(eff
-00017430: 6563 7469 7665 5f74 6f29 2069 7320 4648  ective_to) is FH
-00017440: 4952 4461 7465 3a0a 2020 2020 2020 2020  IRDate:.        
-00017450: 2020 2020 6668 6972 5f65 6666 6563 7469      fhir_effecti
-00017460: 7665 5f74 6f20 3d20 6566 6665 6374 6976  ve_to = effectiv
-00017470: 655f 746f 0a20 2020 2020 2020 2070 6572  e_to.        per
-00017480: 696f 645f 6578 7420 3d20 7365 6c66 2e67  iod_ext = self.g
-00017490: 6574 5f70 6572 696f 645f 6578 7428 290a  et_period_ext().
-000174a0: 2020 2020 2020 2020 6966 2070 6572 696f          if perio
-000174b0: 645f 6578 7420 6973 204e 6f6e 6520 6f72  d_ext is None or
-000174c0: 2070 6572 696f 645f 6578 742e 7661 6c75   period_ext.valu
-000174d0: 6550 6572 696f 6420 6973 204e 6f6e 653a  ePeriod is None:
-000174e0: 0a20 2020 2020 2020 2020 2020 2070 6572  .            per
-000174f0: 696f 6420 3d20 5065 7269 6f64 2829 0a20  iod = Period(). 
-00017500: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00017510: 2020 2020 2020 2020 2070 6572 696f 6420           period 
-00017520: 3d20 7065 7269 6f64 5f65 7874 2e76 616c  = period_ext.val
-00017530: 7565 5065 7269 6f64 0a20 2020 2020 2020  uePeriod.       
-00017540: 2070 6572 696f 642e 656e 6420 3d20 6668   period.end = fh
-00017550: 6972 5f65 6666 6563 7469 7665 5f74 6f0a  ir_effective_to.
-00017560: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00017570: 5f70 6572 696f 645f 6578 7428 6f72 6761  _period_ext(orga
-00017580: 6e69 7a61 7469 6f6e 3d6f 7267 616e 697a  nization=organiz
-00017590: 6174 696f 6e2c 2070 6572 696f 643d 7065  ation, period=pe
-000175a0: 7269 6f64 290a 0a20 2020 2064 6566 2067  riod)..    def g
-000175b0: 6574 5f70 6572 696f 645f 6578 7428 7365  et_period_ext(se
-000175c0: 6c66 2c20 6f72 6761 6e69 7a61 7469 6f6e  lf, organization
-000175d0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-000175e0: 6966 206f 7267 616e 697a 6174 696f 6e20  if organization 
-000175f0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00017600: 2020 2020 206f 7267 616e 697a 6174 696f       organizatio
-00017610: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
-00017620: 736f 7572 6365 0a20 2020 2020 2020 2069  source.        i
-00017630: 6620 6f72 6761 6e69 7a61 7469 6f6e 2e65  f organization.e
-00017640: 7874 656e 7369 6f6e 2069 7320 6e6f 7420  xtension is not 
-00017650: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00017660: 2020 666f 7220 6578 7420 696e 206f 7267    for ext in org
-00017670: 616e 697a 6174 696f 6e2e 6578 7465 6e73  anization.extens
-00017680: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-00017690: 2020 2020 2069 6620 6578 742e 7572 6c20       if ext.url 
-000176a0: 3d3d 2073 656c 662e 7065 7269 6f64 5f75  == self.period_u
-000176b0: 726c 3a0a 2020 2020 2020 2020 2020 2020  rl:.            
-000176c0: 2020 2020 2020 2020 7265 7475 726e 2065          return e
-000176d0: 7874 0a20 2020 2020 2020 2072 6574 7572  xt.        retur
-000176e0: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
-000176f0: 7365 745f 7065 7269 6f64 5f65 7874 2873  set_period_ext(s
-00017700: 656c 662c 206f 7267 616e 697a 6174 696f  elf, organizatio
-00017710: 6e3d 4e6f 6e65 2c20 7065 7269 6f64 3d4e  n=None, period=N
-00017720: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-00017730: 206f 7267 616e 697a 6174 696f 6e20 6973   organization is
-00017740: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00017750: 2020 206f 7267 616e 697a 6174 696f 6e20     organization 
-00017760: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
-00017770: 7572 6365 0a20 2020 2020 2020 2069 6620  urce.        if 
-00017780: 6f72 6761 6e69 7a61 7469 6f6e 2e65 7874  organization.ext
-00017790: 656e 7369 6f6e 2069 7320 4e6f 6e65 3a0a  ension is None:.
-000177a0: 2020 2020 2020 2020 2020 2020 6f72 6761              orga
-000177b0: 6e69 7a61 7469 6f6e 2e65 7874 656e 7369  nization.extensi
-000177c0: 6f6e 203d 205b 5d0a 2020 2020 2020 2020  on = [].        
-000177d0: 7065 7269 6f64 5f65 7874 203d 2073 656c  period_ext = sel
-000177e0: 662e 6765 745f 7065 7269 6f64 5f65 7874  f.get_period_ext
-000177f0: 286f 7267 616e 697a 6174 696f 6e3d 6f72  (organization=or
-00017800: 6761 6e69 7a61 7469 6f6e 290a 2020 2020  ganization).    
-00017810: 2020 2020 6966 2070 6572 696f 645f 6578      if period_ex
-00017820: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+000148f0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014910: 6966 2027 6e61 6d27 2069 6e20 7061 7469  if 'nam' in pati
+00014920: 656e 745f 6469 6374 3a0a 2020 2020 2020  ent_dict:.      
+00014930: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014940: 6c66 2e73 6574 5f6e 616d 286e 616d 3d70  lf.set_nam(nam=p
+00014950: 6174 6965 6e74 5f64 6963 745b 276e 616d  atient_dict['nam
+00014960: 275d 2c20 636f 6469 6e67 5f73 7973 7465  '], coding_syste
+00014970: 6d3d 7061 7469 656e 745f 636f 6469 6e67  m=patient_coding
+00014980: 5f73 7973 7465 6d2c 2063 6f64 696e 675f  _system, coding_
+00014990: 7665 7273 696f 6e3d 7061 7469 656e 745f  version=patient_
+000149a0: 636f 6469 6e67 5f76 6572 7369 6f6e 2c20  coding_version, 
+000149b0: 7061 7469 656e 743d 7061 7469 656e 7429  patient=patient)
+000149c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000149d0: 2069 6620 276e 6975 2720 696e 2070 6174   if 'niu' in pat
+000149e0: 6965 6e74 5f64 6963 743a 0a20 2020 2020  ient_dict:.     
+000149f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014a00: 656c 662e 7365 745f 6e69 7528 6e69 753d  elf.set_niu(niu=
+00014a10: 7061 7469 656e 745f 6469 6374 5b27 6e69  patient_dict['ni
+00014a20: 7527 5d2c 2063 6f64 696e 675f 7379 7374  u'], coding_syst
+00014a30: 656d 3d70 6174 6965 6e74 5f63 6f64 696e  em=patient_codin
+00014a40: 675f 7379 7374 656d 2c20 636f 6469 6e67  g_system, coding
+00014a50: 5f76 6572 7369 6f6e 3d70 6174 6965 6e74  _version=patient
+00014a60: 5f63 6f64 696e 675f 7665 7273 696f 6e2c  _coding_version,
+00014a70: 2070 6174 6965 6e74 3d70 6174 6965 6e74   patient=patient
+00014a80: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00014a90: 2027 6765 6e64 6572 2720 696e 2070 6174   'gender' in pat
+00014aa0: 6965 6e74 5f64 6963 743a 0a20 2020 2020  ient_dict:.     
+00014ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014ac0: 7365 745f 6765 6e64 6572 2867 656e 6465  set_gender(gende
+00014ad0: 723d 7061 7469 656e 745f 6469 6374 5b27  r=patient_dict['
+00014ae0: 6765 6e64 6572 275d 2c20 7061 7469 656e  gender'], patien
+00014af0: 743d 7061 7469 656e 7429 0a20 2020 2020  t=patient).     
+00014b00: 2020 2020 2020 2069 6620 2762 6972 7468         if 'birth
+00014b10: 5f64 6174 6527 2069 6e20 7061 7469 656e  _date' in patien
+00014b20: 745f 6469 6374 3a0a 2020 2020 2020 2020  t_dict:.        
+00014b30: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00014b40: 5f62 6972 7468 5f64 6174 6528 7374 725f  _birth_date(str_
+00014b50: 6461 7465 3d70 6174 6965 6e74 5f64 6963  date=patient_dic
+00014b60: 745b 2762 6972 7468 5f64 6174 6527 5d2c  t['birth_date'],
+00014b70: 2070 6174 6965 6e74 3d70 6174 6965 6e74   patient=patient
+00014b80: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00014b90: 2027 6964 2720 696e 2070 6174 6965 6e74   'id' in patient
+00014ba0: 5f64 6963 743a 0a20 2020 2020 2020 2020  _dict:.         
+00014bb0: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00014bc0: 6964 2869 643d 7061 7469 656e 745f 6469  id(id=patient_di
+00014bd0: 6374 5b27 6964 275d 2c20 7061 7469 656e  ct['id'], patien
+00014be0: 743d 7061 7469 656e 7429 0a20 2020 2020  t=patient).     
+00014bf0: 2020 2020 2020 2061 6374 6976 6520 3d20         active = 
+00014c00: 7061 7469 656e 745f 6469 6374 5b27 6163  patient_dict['ac
+00014c10: 7469 7665 275d 2069 6620 2761 6374 6976  tive'] if 'activ
+00014c20: 6527 2069 6e20 7061 7469 656e 745f 6469  e' in patient_di
+00014c30: 6374 2065 6c73 6520 5472 7565 0a20 2020  ct else True.   
+00014c40: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00014c50: 745f 6163 7469 7665 2861 6374 6976 653d  t_active(active=
+00014c60: 6163 7469 7665 2c20 7061 7469 656e 743d  active, patient=
+00014c70: 7061 7469 656e 7429 0a20 2020 2020 2020  patient).       
+00014c80: 2020 2020 2069 6620 2761 6464 7265 7373       if 'address
+00014c90: 5f6c 696e 6527 2069 6e20 7061 7469 656e  _line' in patien
+00014ca0: 745f 6469 6374 206f 7220 2761 6464 7265  t_dict or 'addre
+00014cb0: 7373 5f63 6974 7927 2069 6e20 7061 7469  ss_city' in pati
+00014cc0: 656e 745f 6469 6374 206f 7220 2761 6464  ent_dict or 'add
+00014cd0: 7265 7373 5f70 6f73 7461 6c5f 636f 6465  ress_postal_code
+00014ce0: 2720 696e 2070 6174 6965 6e74 5f64 6963  ' in patient_dic
+00014cf0: 7420 6f72 2027 6164 6472 6573 735f 7374  t or 'address_st
+00014d00: 6174 6527 2069 6e20 7061 7469 656e 745f  ate' in patient_
+00014d10: 6469 6374 206f 7220 2761 6464 7265 7373  dict or 'address
+00014d20: 5f63 6f75 6e74 7279 2720 696e 2070 6174  _country' in pat
+00014d30: 6965 6e74 5f64 6963 743a 0a20 2020 2020  ient_dict:.     
+00014d40: 2020 2020 2020 2020 2020 2061 6464 7265             addre
+00014d50: 7373 5f6c 696e 6520 3d20 7061 7469 656e  ss_line = patien
+00014d60: 745f 6469 6374 5b27 6164 6472 6573 735f  t_dict['address_
+00014d70: 6c69 6e65 275d 2069 6620 2761 6464 7265  line'] if 'addre
+00014d80: 7373 5f6c 696e 6527 2069 6e20 7061 7469  ss_line' in pati
+00014d90: 656e 745f 6469 6374 2065 6c73 6520 4e6f  ent_dict else No
+00014da0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00014db0: 2020 2061 6464 7265 7373 5f63 6974 7920     address_city 
+00014dc0: 3d20 7061 7469 656e 745f 6469 6374 5b27  = patient_dict['
+00014dd0: 6164 6472 6573 735f 6369 7479 275d 2069  address_city'] i
+00014de0: 6620 2761 6464 7265 7373 5f63 6974 7927  f 'address_city'
+00014df0: 2069 6e20 7061 7469 656e 745f 6469 6374   in patient_dict
+00014e00: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
+00014e10: 2020 2020 2020 2020 2020 2061 6464 7265             addre
+00014e20: 7373 5f73 7461 7465 203d 2070 6174 6965  ss_state = patie
+00014e30: 6e74 5f64 6963 745b 2761 6464 7265 7373  nt_dict['address
+00014e40: 5f73 7461 7465 275d 2069 6620 2761 6464  _state'] if 'add
+00014e50: 7265 7373 5f73 7461 7465 2720 696e 2070  ress_state' in p
+00014e60: 6174 6965 6e74 5f64 6963 7420 656c 7365  atient_dict else
+00014e70: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00014e80: 2020 2020 2020 6164 6472 6573 735f 706f        address_po
+00014e90: 7374 616c 5f63 6f64 6520 3d20 7061 7469  stal_code = pati
+00014ea0: 656e 745f 6469 6374 5b27 6164 6472 6573  ent_dict['addres
+00014eb0: 735f 706f 7374 616c 5f63 6f64 6527 5d20  s_postal_code'] 
+00014ec0: 6966 2027 6164 6472 6573 735f 706f 7374  if 'address_post
+00014ed0: 616c 5f63 6f64 6527 2069 6e20 7061 7469  al_code' in pati
+00014ee0: 656e 745f 6469 6374 2065 6c73 6520 4e6f  ent_dict else No
+00014ef0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00014f00: 2020 2061 6464 7265 7373 5f63 6f75 6e74     address_count
+00014f10: 7279 203d 2070 6174 6965 6e74 5f64 6963  ry = patient_dic
+00014f20: 745b 2761 6464 7265 7373 5f63 6f75 6e74  t['address_count
+00014f30: 7279 275d 2069 6620 2761 6464 7265 7373  ry'] if 'address
+00014f40: 5f63 6f75 6e74 7279 2720 696e 2070 6174  _country' in pat
+00014f50: 6965 6e74 5f64 6963 7420 656c 7365 204e  ient_dict else N
+00014f60: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00014f70: 2020 2020 7365 6c66 2e73 6574 5f61 6464      self.set_add
+00014f80: 7265 7373 280a 2020 2020 2020 2020 2020  ress(.          
+00014f90: 2020 2020 2020 2020 2020 6164 6472 6573            addres
+00014fa0: 735f 6369 7479 3d61 6464 7265 7373 5f63  s_city=address_c
+00014fb0: 6974 792c 0a20 2020 2020 2020 2020 2020  ity,.           
+00014fc0: 2020 2020 2020 2020 2061 6464 7265 7373           address
+00014fd0: 5f63 6f75 6e74 7279 3d61 6464 7265 7373  _country=address
+00014fe0: 5f63 6f75 6e74 7279 2c0a 2020 2020 2020  _country,.      
+00014ff0: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+00015000: 6472 6573 735f 6c69 6e65 3d61 6464 7265  dress_line=addre
+00015010: 7373 5f6c 696e 652c 0a20 2020 2020 2020  ss_line,.       
+00015020: 2020 2020 2020 2020 2020 2020 2061 6464               add
+00015030: 7265 7373 5f73 7461 7465 3d61 6464 7265  ress_state=addre
+00015040: 7373 5f73 7461 7465 2c0a 2020 2020 2020  ss_state,.      
+00015050: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+00015060: 6472 6573 735f 706f 7374 616c 5f63 6f64  dress_postal_cod
+00015070: 653d 6164 6472 6573 735f 706f 7374 616c  e=address_postal
+00015080: 5f63 6f64 652c 0a20 2020 2020 2020 2020  _code,.         
+00015090: 2020 2020 2020 2020 2020 2070 6174 6965             patie
+000150a0: 6e74 3d70 6174 6965 6e74 290a 2020 2020  nt=patient).    
+000150b0: 2020 2020 2020 2020 6966 2027 6d6f 7468          if 'moth
+000150c0: 6572 5f67 6976 656e 5f6e 616d 6527 2069  er_given_name' i
+000150d0: 6e20 7061 7469 656e 745f 6469 6374 206f  n patient_dict o
+000150e0: 7220 276d 6f74 6865 725f 6661 6d69 6c79  r 'mother_family
+000150f0: 5f6e 616d 6527 2069 6e20 7061 7469 656e  _name' in patien
+00015100: 745f 6469 6374 3a0a 2020 2020 2020 2020  t_dict:.        
+00015110: 2020 2020 2020 2020 6d6f 7468 6572 5f67          mother_g
+00015120: 6976 656e 5f6e 616d 6520 3d20 7061 7469  iven_name = pati
+00015130: 656e 745f 6469 6374 5b27 6d6f 7468 6572  ent_dict['mother
+00015140: 5f67 6976 656e 5f6e 616d 6527 5d20 6966  _given_name'] if
+00015150: 2027 6d6f 7468 6572 5f67 6976 656e 5f6e   'mother_given_n
+00015160: 616d 6527 2069 6e20 7061 7469 656e 745f  ame' in patient_
+00015170: 6469 6374 2065 6c73 6520 4e6f 6e65 0a20  dict else None. 
+00015180: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00015190: 6f74 6865 725f 6661 6d69 6c79 5f6e 616d  other_family_nam
+000151a0: 6520 3d20 7061 7469 656e 745f 6469 6374  e = patient_dict
+000151b0: 5b27 6d6f 7468 6572 5f66 616d 696c 795f  ['mother_family_
+000151c0: 6e61 6d65 275d 2069 6620 276d 6f74 6865  name'] if 'mothe
+000151d0: 725f 6661 6d69 6c79 5f6e 616d 6527 2069  r_family_name' i
+000151e0: 6e20 7061 7469 656e 745f 6469 6374 2065  n patient_dict e
+000151f0: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
+00015200: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00015210: 745f 6d6f 7468 6572 5f6e 616d 6528 6d6f  t_mother_name(mo
+00015220: 7468 6572 5f66 616d 696c 795f 6e61 6d65  ther_family_name
+00015230: 3d6d 6f74 6865 725f 6661 6d69 6c79 5f6e  =mother_family_n
+00015240: 616d 652c 206d 6f74 6865 725f 6769 7665  ame, mother_give
+00015250: 6e5f 6e61 6d65 3d6d 6f74 6865 725f 6769  n_name=mother_gi
+00015260: 7665 6e5f 6e61 6d65 2c20 7061 7469 656e  ven_name, patien
+00015270: 743d 7061 7469 656e 742c 2063 6f64 696e  t=patient, codin
+00015280: 675f 7379 7374 656d 3d70 6174 6965 6e74  g_system=patient
+00015290: 5f63 6f64 696e 675f 7379 7374 656d 2c20  _coding_system, 
+000152a0: 636f 6469 6e67 5f76 6572 7369 6f6e 3d70  coding_version=p
+000152b0: 6174 6965 6e74 5f63 6f64 696e 675f 7665  atient_coding_ve
+000152c0: 7273 696f 6e29 0a0a 2020 2020 2020 2020  rsion)..        
+000152d0: 2020 2020 6966 2027 6661 7468 6572 5f67      if 'father_g
+000152e0: 6976 656e 5f6e 616d 6527 2069 6e20 7061  iven_name' in pa
+000152f0: 7469 656e 745f 6469 6374 206f 7220 2766  tient_dict or 'f
+00015300: 6174 6865 725f 6661 6d69 6c79 5f6e 616d  ather_family_nam
+00015310: 6527 2069 6e20 7061 7469 656e 745f 6469  e' in patient_di
+00015320: 6374 3a0a 2020 2020 2020 2020 2020 2020  ct:.            
+00015330: 2020 2020 6661 7468 6572 5f67 6976 656e      father_given
+00015340: 5f6e 616d 6520 3d20 7061 7469 656e 745f  _name = patient_
+00015350: 6469 6374 5b27 6661 7468 6572 5f67 6976  dict['father_giv
+00015360: 656e 5f6e 616d 6527 5d20 6966 2027 6661  en_name'] if 'fa
+00015370: 7468 6572 5f67 6976 656e 5f6e 616d 6527  ther_given_name'
+00015380: 2069 6e20 7061 7469 656e 745f 6469 6374   in patient_dict
+00015390: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
+000153a0: 2020 2020 2020 2020 2020 2066 6174 6865             fathe
+000153b0: 725f 6661 6d69 6c79 5f6e 616d 6520 3d20  r_family_name = 
+000153c0: 7061 7469 656e 745f 6469 6374 5b27 6661  patient_dict['fa
+000153d0: 7468 6572 5f66 616d 696c 795f 6e61 6d65  ther_family_name
+000153e0: 275d 2069 6620 2766 6174 6865 725f 6661  '] if 'father_fa
+000153f0: 6d69 6c79 5f6e 616d 6527 2069 6e20 7061  mily_name' in pa
+00015400: 7469 656e 745f 6469 6374 2065 6c73 6520  tient_dict else 
+00015410: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00015420: 2020 2020 2073 656c 662e 7365 745f 6661       self.set_fa
+00015430: 7468 6572 5f6e 616d 6528 6661 7468 6572  ther_name(father
+00015440: 5f66 616d 696c 795f 6e61 6d65 3d66 6174  _family_name=fat
+00015450: 6865 725f 6661 6d69 6c79 5f6e 616d 652c  her_family_name,
+00015460: 2066 6174 6865 725f 6769 7665 6e5f 6e61   father_given_na
+00015470: 6d65 3d66 6174 6865 725f 6769 7665 6e5f  me=father_given_
+00015480: 6e61 6d65 2c20 7061 7469 656e 743d 7061  name, patient=pa
+00015490: 7469 656e 742c 2063 6f64 696e 675f 7379  tient, coding_sy
+000154a0: 7374 656d 3d70 6174 6965 6e74 5f63 6f64  stem=patient_cod
+000154b0: 696e 675f 7379 7374 656d 2c20 636f 6469  ing_system, codi
+000154c0: 6e67 5f76 6572 7369 6f6e 3d70 6174 6965  ng_version=patie
+000154d0: 6e74 5f63 6f64 696e 675f 7665 7273 696f  nt_coding_versio
+000154e0: 6e29 0a20 2020 2020 2020 2020 2020 2069  n).            i
+000154f0: 6620 2770 686f 6e65 5f6e 756d 6265 7227  f 'phone_number'
+00015500: 2069 6e20 7061 7469 656e 745f 6469 6374   in patient_dict
+00015510: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015520: 2020 7365 6c66 2e73 6574 5f70 686f 6e65    self.set_phone
+00015530: 5f6e 756d 6265 7228 7068 6f6e 655f 6e75  _number(phone_nu
+00015540: 6d62 6572 3d70 6174 6965 6e74 5f64 6963  mber=patient_dic
+00015550: 745b 2770 686f 6e65 5f6e 756d 6265 7227  t['phone_number'
+00015560: 5d2c 2070 6174 6965 6e74 3d70 6174 6965  ], patient=patie
+00015570: 6e74 290a 0a20 2020 2020 2020 2072 6574  nt)..        ret
+00015580: 7572 6e20 7061 7469 656e 740a 0a20 2020  urn patient..   
+00015590: 2064 6566 2066 726f 6d5f 6668 6972 5f70   def from_fhir_p
+000155a0: 6174 6965 6e74 2873 656c 662c 2070 6174  atient(self, pat
+000155b0: 6965 6e74 3d4e 6f6e 652c 2063 6f64 696e  ient=None, codin
+000155c0: 675f 7379 7374 656d 3d4e 6f6e 652c 2063  g_system=None, c
+000155d0: 6f64 696e 675f 7665 7273 696f 6e3d 4e6f  oding_version=No
+000155e0: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
+000155f0: 7061 7469 656e 7420 6973 204e 6f6e 653a  patient is None:
+00015600: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
+00015610: 6965 6e74 203d 2073 656c 662e 6668 6972  ient = self.fhir
+00015620: 5f72 6573 6f75 7263 650a 0a20 2020 2020  _resource..     
+00015630: 2020 2073 656c 662e 6964 203d 2073 656c     self.id = sel
+00015640: 662e 6765 745f 6964 2870 6174 6965 6e74  f.get_id(patient
+00015650: 3d70 6174 6965 6e74 290a 2020 2020 2020  =patient).      
+00015660: 2020 7365 6c66 2e6d 6174 6368 7261 6d71    self.matchramq
+00015670: 203d 2073 656c 662e 6765 745f 6d61 7463   = self.get_matc
+00015680: 6872 616d 7128 7061 7469 656e 743d 7061  hramq(patient=pa
+00015690: 7469 656e 7429 0a20 2020 2020 2020 2073  tient).        s
+000156a0: 656c 662e 6e61 6d20 3d20 7365 6c66 2e67  elf.nam = self.g
+000156b0: 6574 5f6e 616d 2870 6174 6965 6e74 3d70  et_nam(patient=p
+000156c0: 6174 6965 6e74 290a 2020 2020 2020 2020  atient).        
+000156d0: 7365 6c66 2e6e 6975 203d 2073 656c 662e  self.niu = self.
+000156e0: 6765 745f 6e69 7528 7061 7469 656e 743d  get_niu(patient=
+000156f0: 7061 7469 656e 7429 0a20 2020 2020 2020  patient).       
+00015700: 2073 656c 662e 6769 7665 6e5f 6e61 6d65   self.given_name
+00015710: 203d 2073 656c 662e 6765 745f 6769 7665   = self.get_give
+00015720: 6e5f 6e61 6d65 2870 6174 6965 6e74 3d70  n_name(patient=p
+00015730: 6174 6965 6e74 290a 2020 2020 2020 2020  atient).        
+00015740: 7365 6c66 2e66 616d 696c 795f 6e61 6d65  self.family_name
+00015750: 203d 2073 656c 662e 6765 745f 6661 6d69   = self.get_fami
+00015760: 6c79 5f6e 616d 6528 7061 7469 656e 743d  ly_name(patient=
+00015770: 7061 7469 656e 7429 0a20 2020 2020 2020  patient).       
+00015780: 2073 656c 662e 6163 7469 7665 203d 2073   self.active = s
+00015790: 656c 662e 6765 745f 6163 7469 7665 2870  elf.get_active(p
+000157a0: 6174 6965 6e74 3d70 6174 6965 6e74 290a  atient=patient).
+000157b0: 2020 2020 2020 2020 7365 6c66 2e67 656e          self.gen
+000157c0: 6465 7220 3d20 7365 6c66 2e67 6574 5f67  der = self.get_g
+000157d0: 656e 6465 7228 7061 7469 656e 743d 7061  ender(patient=pa
+000157e0: 7469 656e 7429 0a20 2020 2020 2020 2073  tient).        s
+000157f0: 656c 662e 6269 7274 685f 6461 7465 203d  elf.birth_date =
+00015800: 2073 656c 662e 6765 745f 6269 7274 685f   self.get_birth_
+00015810: 6461 7465 2870 6174 6965 6e74 3d70 6174  date(patient=pat
+00015820: 6965 6e74 290a 2020 2020 2020 2020 6164  ient).        ad
+00015830: 6472 6573 7320 3d20 7365 6c66 2e67 6574  dress = self.get
+00015840: 5f61 6464 7265 7373 2870 6174 6965 6e74  _address(patient
+00015850: 3d70 6174 6965 6e74 290a 2020 2020 2020  =patient).      
+00015860: 2020 6966 2061 6464 7265 7373 2069 7320    if address is 
+00015870: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00015880: 2020 2020 2020 7365 6c66 2e61 6464 7265        self.addre
+00015890: 7373 5f6c 696e 6520 3d20 6164 6472 6573  ss_line = addres
+000158a0: 732e 6c69 6e65 0a20 2020 2020 2020 2020  s.line.         
+000158b0: 2020 2073 656c 662e 6164 6472 6573 735f     self.address_
+000158c0: 6369 7479 203d 2061 6464 7265 7373 2e63  city = address.c
+000158d0: 6974 790a 2020 2020 2020 2020 2020 2020  ity.            
+000158e0: 7365 6c66 2e61 6464 7265 7373 5f73 7461  self.address_sta
+000158f0: 7465 203d 2061 6464 7265 7373 2e73 7461  te = address.sta
+00015900: 7465 0a20 2020 2020 2020 2020 2020 2073  te.            s
+00015910: 656c 662e 6164 6472 6573 735f 706f 7374  elf.address_post
+00015920: 616c 5f63 6f64 6520 3d20 6164 6472 6573  al_code = addres
+00015930: 732e 706f 7374 616c 436f 6465 0a20 2020  s.postalCode.   
+00015940: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
+00015950: 6472 6573 735f 636f 756e 7472 7920 3d20  dress_country = 
+00015960: 6164 6472 6573 732e 636f 756e 7472 790a  address.country.
+00015970: 2020 2020 2020 2020 6d6f 7468 6572 5f6e          mother_n
+00015980: 616d 6520 3d20 2073 656c 662e 6765 745f  ame =  self.get_
+00015990: 6d6f 7468 6572 5f6e 616d 6528 7061 7469  mother_name(pati
+000159a0: 656e 743d 7061 7469 656e 742c 2063 6f64  ent=patient, cod
+000159b0: 696e 675f 7379 7374 656d 3d63 6f64 696e  ing_system=codin
+000159c0: 675f 7379 7374 656d 2c20 636f 6469 6e67  g_system, coding
+000159d0: 5f76 6572 7369 6f6e 3d63 6f64 696e 675f  _version=coding_
+000159e0: 7665 7273 696f 6e29 0a20 2020 2020 2020  version).       
+000159f0: 2069 6620 6d6f 7468 6572 5f6e 616d 6520   if mother_name 
+00015a00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00015a10: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
+00015a20: 7468 6572 5f67 6976 656e 5f6e 616d 6520  ther_given_name 
+00015a30: 3d20 6d6f 7468 6572 5f6e 616d 652e 6769  = mother_name.gi
+00015a40: 7665 6e0a 2020 2020 2020 2020 2020 2020  ven.            
+00015a50: 7365 6c66 2e6d 6f74 6865 725f 6661 6d69  self.mother_fami
+00015a60: 6c79 5f6e 616d 6520 3d20 6d6f 7468 6572  ly_name = mother
+00015a70: 5f6e 616d 652e 6661 6d69 6c79 0a20 2020  _name.family.   
+00015a80: 2020 2020 2066 6174 6865 725f 6e61 6d65       father_name
+00015a90: 203d 2073 656c 662e 6765 745f 6661 7468   = self.get_fath
+00015aa0: 6572 5f6e 616d 6528 7061 7469 656e 743d  er_name(patient=
+00015ab0: 7061 7469 656e 742c 2063 6f64 696e 675f  patient, coding_
+00015ac0: 7379 7374 656d 3d63 6f64 696e 675f 7379  system=coding_sy
+00015ad0: 7374 656d 2c20 636f 6469 6e67 5f76 6572  stem, coding_ver
+00015ae0: 7369 6f6e 3d63 6f64 696e 675f 7665 7273  sion=coding_vers
+00015af0: 696f 6e29 0a20 2020 2020 2020 2069 6620  ion).        if 
+00015b00: 6661 7468 6572 5f6e 616d 6520 6973 206e  father_name is n
+00015b10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00015b20: 2020 2020 2073 656c 662e 6661 7468 6572       self.father
+00015b30: 5f67 6976 656e 5f6e 616d 6520 3d20 6661  _given_name = fa
+00015b40: 7468 6572 5f6e 616d 652e 6769 7665 6e0a  ther_name.given.
+00015b50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015b60: 2e66 6174 6865 725f 6661 6d69 6c79 5f6e  .father_family_n
+00015b70: 616d 6520 3d20 6661 7468 6572 5f6e 616d  ame = father_nam
+00015b80: 652e 6661 6d69 6c79 0a20 2020 2020 2020  e.family.       
+00015b90: 2073 656c 662e 7068 6f6e 655f 6e75 6d62   self.phone_numb
+00015ba0: 6572 203d 2073 656c 662e 6765 745f 7068  er = self.get_ph
+00015bb0: 6f6e 655f 6e75 6d62 6572 2870 6174 6965  one_number(patie
+00015bc0: 6e74 3d70 6174 6965 6e74 290a 2020 2020  nt=patient).    
+00015bd0: 2020 2020 0a20 2020 2064 6566 2074 6f5f      .    def to_
+00015be0: 6668 6972 5f70 6174 6965 6e74 2873 656c  fhir_patient(sel
+00015bf0: 662c 2070 6174 6965 6e74 3d4e 6f6e 652c  f, patient=None,
+00015c00: 2063 6f64 696e 675f 7379 7374 656d 3d4e   coding_system=N
+00015c10: 6f6e 652c 2063 6f64 696e 675f 7665 7273  one, coding_vers
+00015c20: 696f 6e3d 4e6f 6e65 293a 0a20 2020 2020  ion=None):.     
+00015c30: 2020 2069 6620 7061 7469 656e 7420 6973     if patient is
+00015c40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00015c50: 2020 2070 6174 6965 6e74 203d 2073 656c     patient = sel
+00015c60: 662e 6668 6972 5f72 6573 6f75 7263 650a  f.fhir_resource.
+00015c70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00015c80: 2e69 6420 6973 206e 6f74 204e 6f6e 653a  .id is not None:
+00015c90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00015ca0: 662e 7365 745f 6964 2869 643d 7365 6c66  f.set_id(id=self
+00015cb0: 2e69 642c 2070 6174 6965 6e74 3d70 6174  .id, patient=pat
+00015cc0: 6965 6e74 290a 2020 2020 2020 2020 6966  ient).        if
+00015cd0: 2073 656c 662e 6e69 7520 6973 204e 6f6e   self.niu is Non
+00015ce0: 6520 616e 6420 7365 6c66 2e6e 616d 2069  e and self.nam i
+00015cf0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00015d00: 2020 2020 7365 6c66 2e73 6574 5f61 7563      self.set_auc
+00015d10: 756e 5f69 6465 6e74 6966 6961 6e74 2870  un_identifiant(p
+00015d20: 6174 6965 6e74 3d70 6174 6965 6e74 290a  atient=patient).
+00015d30: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00015d40: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00015d50: 662e 6e61 6d20 6973 206e 6f74 204e 6f6e  f.nam is not Non
+00015d60: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00015d70: 2020 2073 656c 662e 7365 745f 6e61 6d28     self.set_nam(
+00015d80: 6e61 6d3d 7365 6c66 2e6e 616d 2c20 7061  nam=self.nam, pa
+00015d90: 7469 656e 743d 7061 7469 656e 7429 0a20  tient=patient). 
+00015da0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00015db0: 6c66 2e6e 6975 2069 7320 6e6f 7420 4e6f  lf.niu is not No
+00015dc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00015dd0: 2020 2020 7365 6c66 2e73 6574 5f6e 6975      self.set_niu
+00015de0: 286e 6975 3d73 656c 662e 6e69 752c 2070  (niu=self.niu, p
+00015df0: 6174 6965 6e74 3d70 6174 6965 6e74 290a  atient=patient).
+00015e00: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00015e10: 5f61 6374 6976 6528 6163 7469 7665 3d73  _active(active=s
+00015e20: 656c 662e 6163 7469 7665 2c20 7061 7469  elf.active, pati
+00015e30: 656e 743d 7061 7469 656e 7429 0a20 2020  ent=patient).   
+00015e40: 2020 2020 2073 656c 662e 7365 745f 6d61       self.set_ma
+00015e50: 7463 6872 616d 7128 6d61 7463 6872 616d  tchramq(matchram
+00015e60: 713d 7365 6c66 2e6d 6174 6368 7261 6d71  q=self.matchramq
+00015e70: 2c20 7061 7469 656e 743d 7061 7469 656e  , patient=patien
+00015e80: 7429 0a20 2020 2020 2020 2069 6620 7365  t).        if se
+00015e90: 6c66 2e61 6464 7265 7373 5f63 6974 7920  lf.address_city 
+00015ea0: 6973 206e 6f74 204e 6f6e 6520 6f72 2073  is not None or s
+00015eb0: 656c 662e 6164 6472 6573 735f 636f 756e  elf.address_coun
+00015ec0: 7472 7920 6973 206e 6f74 204e 6f6e 6520  try is not None 
+00015ed0: 6f72 2073 656c 662e 6164 6472 6573 735f  or self.address_
+00015ee0: 6c69 6e65 2069 7320 6e6f 7420 4e6f 6e65  line is not None
+00015ef0: 206f 7220 7365 6c66 2e61 6464 7265 7373   or self.address
+00015f00: 5f70 6f73 7461 6c5f 636f 6465 2069 7320  _postal_code is 
+00015f10: 6e6f 7420 4e6f 6e65 206f 7220 7365 6c66  not None or self
+00015f20: 2e61 6464 7265 7373 5f73 7461 7465 2069  .address_state i
+00015f30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00015f40: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00015f50: 5f61 6464 7265 7373 280a 2020 2020 2020  _address(.      
+00015f60: 2020 2020 2020 2020 2020 6164 6472 6573            addres
+00015f70: 735f 6369 7479 3d73 656c 662e 6164 6472  s_city=self.addr
+00015f80: 6573 735f 6369 7479 2c0a 2020 2020 2020  ess_city,.      
+00015f90: 2020 2020 2020 2020 2020 6164 6472 6573            addres
+00015fa0: 735f 636f 756e 7472 793d 7365 6c66 2e61  s_country=self.a
+00015fb0: 6464 7265 7373 5f63 6f75 6e74 7279 2c0a  ddress_country,.
+00015fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fd0: 6164 6472 6573 735f 6c69 6e65 3d73 656c  address_line=sel
+00015fe0: 662e 6164 6472 6573 735f 6c69 6e65 2c0a  f.address_line,.
+00015ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016000: 6164 6472 6573 735f 7374 6174 653d 7365  address_state=se
+00016010: 6c66 2e61 6464 7265 7373 5f73 7461 7465  lf.address_state
+00016020: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016030: 2020 6164 6472 6573 735f 706f 7374 616c    address_postal
+00016040: 5f63 6f64 653d 7365 6c66 2e61 6464 7265  _code=self.addre
+00016050: 7373 5f70 6f73 7461 6c5f 636f 6465 2c0a  ss_postal_code,.
+00016060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016070: 7061 7469 656e 743d 7061 7469 656e 7429  patient=patient)
+00016080: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00016090: 2020 2020 2069 6620 7365 6c66 2e62 6972       if self.bir
+000160a0: 7468 5f64 6174 6520 6973 206e 6f74 204e  th_date is not N
+000160b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000160c0: 2073 656c 662e 7365 745f 6269 7274 685f   self.set_birth_
+000160d0: 6461 7465 2873 7472 5f64 6174 653d 7365  date(str_date=se
+000160e0: 6c66 2e62 6972 7468 5f64 6174 652c 2070  lf.birth_date, p
+000160f0: 6174 6965 6e74 3d70 6174 6965 6e74 290a  atient=patient).
+00016100: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00016110: 6661 6d69 6c79 5f6e 616d 6520 6973 206e  family_name is n
+00016120: 6f74 204e 6f6e 6520 6f72 2073 656c 662e  ot None or self.
+00016130: 6769 7665 6e5f 6e61 6d65 2069 7320 6e6f  given_name is no
+00016140: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00016150: 2020 2020 7365 6c66 2e73 6574 5f6e 616d      self.set_nam
+00016160: 6528 6769 7665 6e5f 6e61 6d65 3d73 656c  e(given_name=sel
+00016170: 662e 6769 7665 6e5f 6e61 6d65 2c20 6661  f.given_name, fa
+00016180: 6d69 6c79 5f6e 616d 653d 7365 6c66 2e66  mily_name=self.f
+00016190: 616d 696c 795f 6e61 6d65 290a 2020 2020  amily_name).    
+000161a0: 2020 2020 6966 2073 656c 662e 6661 7468      if self.fath
+000161b0: 6572 5f66 616d 696c 795f 6e61 6d65 2069  er_family_name i
+000161c0: 7320 6e6f 7420 4e6f 6e65 206f 7220 7365  s not None or se
+000161d0: 6c66 2e66 6174 6865 725f 6769 7665 6e5f  lf.father_given_
+000161e0: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
+000161f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00016200: 6c66 2e73 6574 5f66 6174 6865 725f 6e61  lf.set_father_na
+00016210: 6d65 2866 6174 6865 725f 6769 7665 6e5f  me(father_given_
+00016220: 6e61 6d65 3d73 656c 662e 6661 7468 6572  name=self.father
+00016230: 5f67 6976 656e 5f6e 616d 652c 2066 6174  _given_name, fat
+00016240: 6865 725f 6661 6d69 6c79 5f6e 616d 653d  her_family_name=
+00016250: 7365 6c66 2e66 6174 6865 725f 6661 6d69  self.father_fami
+00016260: 6c79 5f6e 616d 652c 2063 6f64 696e 675f  ly_name, coding_
+00016270: 7379 7374 656d 3d63 6f64 696e 675f 7379  system=coding_sy
+00016280: 7374 656d 2c20 636f 6469 6e67 5f76 6572  stem, coding_ver
+00016290: 7369 6f6e 3d63 6f64 696e 675f 7665 7273  sion=coding_vers
+000162a0: 696f 6e29 0a20 2020 2020 2020 2069 6620  ion).        if 
+000162b0: 7365 6c66 2e6d 6f74 6865 725f 6661 6d69  self.mother_fami
+000162c0: 6c79 5f6e 616d 6520 6973 206e 6f74 204e  ly_name is not N
+000162d0: 6f6e 6520 6f72 2073 656c 662e 6d6f 7468  one or self.moth
+000162e0: 6572 5f67 6976 656e 5f6e 616d 6520 6973  er_given_name is
+000162f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00016300: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+00016310: 6d6f 7468 6572 5f6e 616d 6528 6d6f 7468  mother_name(moth
+00016320: 6572 5f67 6976 656e 5f6e 616d 653d 7365  er_given_name=se
+00016330: 6c66 2e6d 6f74 6865 725f 6769 7665 6e5f  lf.mother_given_
+00016340: 6e61 6d65 2c20 6d6f 7468 6572 5f66 616d  name, mother_fam
+00016350: 696c 795f 6e61 6d65 3d73 656c 662e 6d6f  ily_name=self.mo
+00016360: 7468 6572 5f66 616d 696c 795f 6e61 6d65  ther_family_name
+00016370: 2c20 636f 6469 6e67 5f73 7973 7465 6d3d  , coding_system=
+00016380: 636f 6469 6e67 5f73 7973 7465 6d2c 2063  coding_system, c
+00016390: 6f64 696e 675f 7665 7273 696f 6e3d 636f  oding_version=co
+000163a0: 6469 6e67 5f76 6572 7369 6f6e 290a 2020  ding_version).  
+000163b0: 2020 2020 2020 7365 6c66 2e73 6574 5f67        self.set_g
+000163c0: 656e 6465 7228 6765 6e64 6572 3d73 656c  ender(gender=sel
+000163d0: 662e 6765 6e64 6572 2c20 7061 7469 656e  f.gender, patien
+000163e0: 743d 7061 7469 656e 7429 0a20 2020 2020  t=patient).     
+000163f0: 2020 2069 6620 7365 6c66 2e70 686f 6e65     if self.phone
+00016400: 5f6e 756d 6265 7220 6973 206e 6f74 204e  _number is not N
+00016410: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00016420: 2073 656c 662e 7365 745f 7068 6f6e 655f   self.set_phone_
+00016430: 6e75 6d62 6572 2870 686f 6e65 5f6e 756d  number(phone_num
+00016440: 6265 723d 7365 6c66 2e70 686f 6e65 5f6e  ber=self.phone_n
+00016450: 756d 6265 722c 2070 6174 6965 6e74 3d70  umber, patient=p
+00016460: 6174 6965 6e74 290a 0a63 6c61 7373 204f  atient)..class O
+00016470: 7267 616e 697a 6174 696f 6e46 4849 5228  rganizationFHIR(
+00016480: 4261 7365 4648 4952 293a 0a20 2020 206f  BaseFHIR):.    o
+00016490: 7267 616e 697a 6174 696f 6e5f 656e 6470  rganization_endp
+000164a0: 6f69 6e74 203d 2022 7b62 6173 655f 7572  oint = "{base_ur
+000164b0: 6c7d 2f4f 7267 616e 697a 6174 696f 6e22  l}/Organization"
+000164c0: 0a20 2020 2073 6561 7263 685f 656e 6470  .    search_endp
+000164d0: 6f69 6e74 203d 206f 7267 616e 697a 6174  oint = organizat
+000164e0: 696f 6e5f 656e 6470 6f69 6e74 202b 2022  ion_endpoint + "
+000164f0: 2f5f 7365 6172 6368 220a 2020 2020 6f72  /_search".    or
+00016500: 6761 6e69 7a61 7469 6f6e 5f62 795f 6964  ganization_by_id
+00016510: 5f65 6e64 706f 696e 7420 3d20 6f72 6761  _endpoint = orga
+00016520: 6e69 7a61 7469 6f6e 5f65 6e64 706f 696e  nization_endpoin
+00016530: 7420 2b20 222f 7b69 647d 220a 2020 2020  t + "/{id}".    
+00016540: 7272 7373 5f73 7973 7465 6d20 3d20 2768  rrss_system = 'h
+00016550: 7474 7073 3a2f 2f70 726f 2e63 6f6e 7375  ttps://pro.consu
+00016560: 6c74 6174 696f 6e2e 7272 7373 2e72 7473  ltation.rrss.rts
+00016570: 732e 7163 2e63 6127 0a20 2020 2072 7273  s.qc.ca'.    rrs
+00016580: 735f 6d6f 745f 636c 655f 6578 7465 6e73  s_mot_cle_extens
+00016590: 696f 6e5f 7572 6c20 3d20 2768 7474 703a  ion_url = 'http:
+000165a0: 2f2f 7777 772e 7361 6e74 6570 7562 6c69  //www.santepubli
+000165b0: 7175 652e 7274 7373 2e71 632e 6361 2f73  que.rtss.qc.ca/s
+000165c0: 6970 6d69 2f72 7273 732f 312e 302e 302f  ipmi/rrss/1.0.0/
+000165d0: 6578 7465 6e73 696f 6e73 2f23 6d6f 7473  extensions/#mots
+000165e0: 636c 6573 270a 2020 2020 7065 7269 6f64  cles'.    period
+000165f0: 5f75 726c 203d 2022 6874 7470 3a2f 2f77  _url = "http://w
+00016600: 7777 2e73 616e 7465 7075 626c 6971 7565  ww.santepublique
+00016610: 2e72 7473 732e 7163 2e63 612f 7369 706d  .rtss.qc.ca/sipm
+00016620: 692f 7272 7373 2f31 2e30 2e30 2f65 7874  i/rrss/1.0.0/ext
+00016630: 656e 7369 6f6e 732f 7065 7269 6f64 220a  ensions/period".
+00016640: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00016650: 5f28 7365 6c66 2c20 6261 7365 5f75 726c  _(self, base_url
+00016660: 3d4e 6f6e 652c 2062 6173 655f 7572 693d  =None, base_uri=
+00016670: 4e6f 6e65 2c20 7265 736f 7572 6365 3d4e  None, resource=N
+00016680: 6f6e 652c 2074 6f6b 656e 5f68 6561 6465  one, token_heade
+00016690: 723d 4e6f 6e65 2c20 7661 6c69 6461 7465  r=None, validate
+000166a0: 5f63 6572 7473 3d54 7275 6529 202d 3e20  _certs=True) -> 
+000166b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 7375  None:.        su
+000166c0: 7065 7228 292e 5f5f 696e 6974 5f5f 2862  per().__init__(b
+000166d0: 6173 655f 7572 6c3d 6261 7365 5f75 726c  ase_url=base_url
+000166e0: 2c20 6261 7365 5f75 7269 3d62 6173 655f  , base_uri=base_
+000166f0: 7572 692c 2074 6f6b 656e 5f68 6561 6465  uri, token_heade
+00016700: 723d 746f 6b65 6e5f 6865 6164 6572 290a  r=token_header).
+00016710: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00016720: 6964 6174 655f 6365 7274 7320 3d20 7661  idate_certs = va
+00016730: 6c69 6461 7465 5f63 6572 7473 0a20 2020  lidate_certs.   
+00016740: 2020 2020 2069 6620 7265 736f 7572 6365       if resource
+00016750: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00016760: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00016770: 6869 725f 7265 736f 7572 6365 203d 204f  hir_resource = O
+00016780: 7267 616e 697a 6174 696f 6e28 6a73 6f6e  rganization(json
+00016790: 6469 6374 3d72 6573 6f75 7263 6529 0a20  dict=resource). 
+000167a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000167b0: 2020 2020 2020 2020 2073 656c 662e 6668           self.fh
+000167c0: 6972 5f72 6573 6f75 7263 6520 3d20 4f72  ir_resource = Or
+000167d0: 6761 6e69 7a61 7469 6f6e 2829 0a0a 2020  ganization()..  
+000167e0: 2020 6465 6620 6765 7446 6869 7252 6573    def getFhirRes
+000167f0: 6f75 7263 6528 7365 6c66 293a 0a20 2020  ource(self):.   
+00016800: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00016810: 2e66 6869 725f 7265 736f 7572 6365 2e61  .fhir_resource.a
+00016820: 735f 6a73 6f6e 2829 0a0a 2020 2020 6465  s_json()..    de
+00016830: 6620 6765 745f 6964 2873 656c 662c 206f  f get_id(self, o
+00016840: 7267 616e 697a 6174 696f 6e3d 4e6f 6e65  rganization=None
+00016850: 293a 0a20 2020 2020 2020 2069 6620 6f72  ):.        if or
+00016860: 6761 6e69 7a61 7469 6f6e 2069 7320 4e6f  ganization is No
+00016870: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00016880: 6f72 6761 6e69 7a61 7469 6f6e 203d 2073  organization = s
+00016890: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+000168a0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+000168b0: 206f 7267 616e 697a 6174 696f 6e2e 6964   organization.id
+000168c0: 0a0a 2020 2020 6465 6620 6765 745f 6964  ..    def get_id
+000168d0: 5f72 7273 7328 7365 6c66 2c20 6f72 6761  _rrss(self, orga
+000168e0: 6e69 7a61 7469 6f6e 3d4e 6f6e 6529 3a0a  nization=None):.
+000168f0: 2020 2020 2020 2020 6966 206f 7267 616e          if organ
+00016900: 697a 6174 696f 6e20 6973 204e 6f6e 653a  ization is None:
+00016910: 0a20 2020 2020 2020 2020 2020 206f 7267  .            org
+00016920: 616e 697a 6174 696f 6e20 3d20 7365 6c66  anization = self
+00016930: 2e66 6869 725f 7265 736f 7572 6365 0a20  .fhir_resource. 
+00016940: 2020 2020 2020 2069 6620 6f72 6761 6e69         if organi
+00016950: 7a61 7469 6f6e 2e69 6465 6e74 6966 6965  zation.identifie
+00016960: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+00016970: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00016980: 6465 6e74 6966 6965 7220 696e 206f 7267  dentifier in org
+00016990: 616e 697a 6174 696f 6e2e 6964 656e 7469  anization.identi
+000169a0: 6669 6572 3a0a 2020 2020 2020 2020 2020  fier:.          
+000169b0: 2020 2020 2020 6966 2069 6465 6e74 6966        if identif
+000169c0: 6965 722e 7379 7374 656d 203d 3d20 7365  ier.system == se
+000169d0: 6c66 2e72 7273 735f 7379 7374 656d 3a0a  lf.rrss_system:.
+000169e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169f0: 2020 2020 7265 7475 726e 2069 6465 6e74      return ident
+00016a00: 6966 6965 722e 7661 6c75 650a 2020 2020  ifier.value.    
+00016a10: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00016a20: 0a20 2020 2064 6566 2073 6574 5f6e 616d  .    def set_nam
+00016a30: 6528 7365 6c66 2c20 6f72 6761 6e69 7a61  e(self, organiza
+00016a40: 7469 6f6e 3d4e 6f6e 652c 206e 616d 653d  tion=None, name=
+00016a50: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
+00016a60: 6620 6f72 6761 6e69 7a61 7469 6f6e 2069  f organization i
+00016a70: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00016a80: 2020 2020 6f72 6761 6e69 7a61 7469 6f6e      organization
+00016a90: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
+00016aa0: 6f75 7263 650a 0a20 2020 2020 2020 206f  ource..        o
+00016ab0: 7267 616e 697a 6174 696f 6e2e 6e61 6d65  rganization.name
+00016ac0: 203d 206e 616d 650a 0a20 2020 2064 6566   = name..    def
+00016ad0: 2067 6574 5f6e 616d 6528 7365 6c66 2c20   get_name(self, 
+00016ae0: 6f72 6761 6e69 7a61 7469 6f6e 3d4e 6f6e  organization=Non
+00016af0: 6529 3a0a 2020 2020 2020 2020 6966 206f  e):.        if o
+00016b00: 7267 616e 697a 6174 696f 6e20 6973 204e  rganization is N
+00016b10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00016b20: 206f 7267 616e 697a 6174 696f 6e20 3d20   organization = 
+00016b30: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
+00016b40: 6365 0a20 2020 2020 2020 2072 6574 7572  ce.        retur
+00016b50: 6e20 6f72 6761 6e69 7a61 7469 6f6e 2e6e  n organization.n
+00016b60: 616d 650a 0a20 2020 2064 6566 2068 6176  ame..    def hav
+00016b70: 655f 6d6f 745f 636c 6528 7365 6c66 2c20  e_mot_cle(self, 
+00016b80: 6f72 6761 6e69 7a61 7469 6f6e 3d4e 6f6e  organization=Non
+00016b90: 652c 206d 6f74 5f63 6c65 3d4e 6f6e 6529  e, mot_cle=None)
+00016ba0: 3a0a 2020 2020 2020 2020 6966 206f 7267  :.        if org
+00016bb0: 616e 697a 6174 696f 6e20 6973 204e 6f6e  anization is Non
+00016bc0: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+00016bd0: 7267 616e 697a 6174 696f 6e20 3d20 7365  rganization = se
+00016be0: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+00016bf0: 0a20 2020 2020 2020 2069 6620 6d6f 745f  .        if mot_
+00016c00: 636c 6520 6973 206e 6f74 204e 6f6e 6520  cle is not None 
+00016c10: 616e 6420 6f72 6761 6e69 7a61 7469 6f6e  and organization
+00016c20: 2e65 7874 656e 7369 6f6e 2069 7320 6e6f  .extension is no
+00016c30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00016c40: 2020 2020 666f 7220 6578 7465 6e73 696f      for extensio
+00016c50: 6e20 696e 206f 7267 616e 697a 6174 696f  n in organizatio
+00016c60: 6e2e 6578 7465 6e73 696f 6e3a 0a20 2020  n.extension:.   
+00016c70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016c80: 6578 7465 6e73 696f 6e2e 7572 6c20 3d3d  extension.url ==
+00016c90: 2073 656c 662e 7272 7373 5f6d 6f74 5f63   self.rrss_mot_c
+00016ca0: 6c65 5f65 7874 656e 7369 6f6e 5f75 726c  le_extension_url
+00016cb0: 2061 6e64 2065 7874 656e 7369 6f6e 2e76   and extension.v
+00016cc0: 616c 7565 5374 7269 6e67 203d 3d20 6d6f  alueString == mo
+00016cd0: 745f 636c 653a 0a20 2020 2020 2020 2020  t_cle:.         
+00016ce0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00016cf0: 6e20 5472 7565 0a20 2020 2020 2020 2072  n True.        r
+00016d00: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00016d10: 2064 6566 2067 6574 5f65 6666 6563 7469   def get_effecti
+00016d20: 7665 5f66 726f 6d28 7365 6c66 2c20 6f72  ve_from(self, or
+00016d30: 6761 6e69 7a61 7469 6f6e 3d4e 6f6e 6529  ganization=None)
+00016d40: 3a0a 2020 2020 2020 2020 6966 206f 7267  :.        if org
+00016d50: 616e 697a 6174 696f 6e20 6973 204e 6f6e  anization is Non
+00016d60: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+00016d70: 7267 616e 697a 6174 696f 6e20 3d20 7365  rganization = se
+00016d80: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+00016d90: 0a20 2020 2020 2020 2070 6572 696f 645f  .        period_
+00016da0: 6578 7420 3d20 7365 6c66 2e67 6574 5f70  ext = self.get_p
+00016db0: 6572 696f 645f 6578 7428 6f72 6761 6e69  eriod_ext(organi
+00016dc0: 7a61 7469 6f6e 3d6f 7267 616e 697a 6174  zation=organizat
+00016dd0: 696f 6e29 0a20 2020 2020 2020 2069 6620  ion).        if 
+00016de0: 7065 7269 6f64 5f65 7874 2069 7320 6e6f  period_ext is no
+00016df0: 7420 4e6f 6e65 2061 6e64 2070 6572 696f  t None and perio
+00016e00: 645f 6578 742e 7661 6c75 6550 6572 696f  d_ext.valuePerio
+00016e10: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00016e20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00016e30: 6574 7572 6e20 7065 7269 6f64 5f65 7874  eturn period_ext
+00016e40: 2e76 616c 7565 5065 7269 6f64 2e73 7461  .valuePeriod.sta
+00016e50: 7274 0a20 2020 2020 2020 2072 6574 7572  rt.        retur
+00016e60: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
+00016e70: 6765 745f 6566 6665 6374 6976 655f 746f  get_effective_to
+00016e80: 2873 656c 662c 206f 7267 616e 697a 6174  (self, organizat
+00016e90: 696f 6e3d 4e6f 6e65 293a 0a20 2020 2020  ion=None):.     
+00016ea0: 2020 2069 6620 6f72 6761 6e69 7a61 7469     if organizati
+00016eb0: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00016ec0: 2020 2020 2020 2020 6f72 6761 6e69 7a61          organiza
+00016ed0: 7469 6f6e 203d 2073 656c 662e 6668 6972  tion = self.fhir
+00016ee0: 5f72 6573 6f75 7263 650a 2020 2020 2020  _resource.      
+00016ef0: 2020 7065 7269 6f64 5f65 7874 203d 2073    period_ext = s
+00016f00: 656c 662e 6765 745f 7065 7269 6f64 5f65  elf.get_period_e
+00016f10: 7874 286f 7267 616e 697a 6174 696f 6e3d  xt(organization=
+00016f20: 6f72 6761 6e69 7a61 7469 6f6e 290a 2020  organization).  
+00016f30: 2020 2020 2020 6966 2070 6572 696f 645f        if period_
+00016f40: 6578 7420 6973 206e 6f74 204e 6f6e 6520  ext is not None 
+00016f50: 616e 6420 7065 7269 6f64 5f65 7874 2e76  and period_ext.v
+00016f60: 616c 7565 5065 7269 6f64 2069 7320 6e6f  aluePeriod is no
+00016f70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00016f80: 2020 2020 2020 2020 7265 7475 726e 2070          return p
+00016f90: 6572 696f 645f 6578 742e 7661 6c75 6550  eriod_ext.valueP
+00016fa0: 6572 696f 642e 656e 640a 2020 2020 2020  eriod.end.      
+00016fb0: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
+00016fc0: 2020 2064 6566 2073 6574 5f65 6666 6563     def set_effec
+00016fd0: 7469 7665 5f66 726f 6d28 7365 6c66 2c20  tive_from(self, 
+00016fe0: 6f72 6761 6e69 7a61 7469 6f6e 3d4e 6f6e  organization=Non
+00016ff0: 652c 2065 6666 6563 7469 7665 5f66 726f  e, effective_fro
+00017000: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+00017010: 2069 6620 6f72 6761 6e69 7a61 7469 6f6e   if organization
+00017020: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00017030: 2020 2020 2020 6f72 6761 6e69 7a61 7469        organizati
+00017040: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
+00017050: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
+00017060: 6668 6972 5f65 6666 6563 7469 7665 5f66  fhir_effective_f
+00017070: 726f 6d20 3d20 4e6f 6e65 0a20 2020 2020  rom = None.     
+00017080: 2020 2069 6620 7479 7065 2865 6666 6563     if type(effec
+00017090: 7469 7665 5f66 726f 6d29 2069 7320 7374  tive_from) is st
+000170a0: 723a 0a20 2020 2020 2020 2020 2020 2066  r:.            f
+000170b0: 6869 725f 6566 6665 6374 6976 655f 6672  hir_effective_fr
+000170c0: 6f6d 203d 2046 4849 5244 6174 6528 6a73  om = FHIRDate(js
+000170d0: 6f6e 7661 6c3d 6566 6665 6374 6976 655f  onval=effective_
+000170e0: 6672 6f6d 290a 2020 2020 2020 2020 656c  from).        el
+000170f0: 6966 2074 7970 6528 6566 6665 6374 6976  if type(effectiv
+00017100: 655f 6672 6f6d 2920 6973 2046 4849 5244  e_from) is FHIRD
+00017110: 6174 653a 0a20 2020 2020 2020 2020 2020  ate:.           
+00017120: 2066 6869 725f 6566 6665 6374 6976 655f   fhir_effective_
+00017130: 6672 6f6d 203d 2065 6666 6563 7469 7665  from = effective
+00017140: 5f66 726f 6d0a 2020 2020 2020 2020 7065  _from.        pe
+00017150: 7269 6f64 5f65 7874 203d 2073 656c 662e  riod_ext = self.
+00017160: 6765 745f 7065 7269 6f64 5f65 7874 2829  get_period_ext()
+00017170: 0a20 2020 2020 2020 2069 6620 7065 7269  .        if peri
+00017180: 6f64 5f65 7874 2069 7320 4e6f 6e65 206f  od_ext is None o
+00017190: 7220 7065 7269 6f64 5f65 7874 2e76 616c  r period_ext.val
+000171a0: 7565 5065 7269 6f64 2069 7320 4e6f 6e65  uePeriod is None
+000171b0: 3a0a 2020 2020 2020 2020 2020 2020 7065  :.            pe
+000171c0: 7269 6f64 203d 2050 6572 696f 6428 290a  riod = Period().
+000171d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000171e0: 2020 2020 2020 2020 2020 7065 7269 6f64            period
+000171f0: 203d 2070 6572 696f 645f 6578 742e 7661   = period_ext.va
+00017200: 6c75 6550 6572 696f 640a 2020 2020 2020  luePeriod.      
+00017210: 2020 7065 7269 6f64 2e73 7461 7274 203d    period.start =
+00017220: 2066 6869 725f 6566 6665 6374 6976 655f   fhir_effective_
+00017230: 6672 6f6d 0a20 2020 2020 2020 2073 656c  from.        sel
+00017240: 662e 7365 745f 7065 7269 6f64 5f65 7874  f.set_period_ext
+00017250: 286f 7267 616e 697a 6174 696f 6e3d 6f72  (organization=or
+00017260: 6761 6e69 7a61 7469 6f6e 2c20 7065 7269  ganization, peri
+00017270: 6f64 3d70 6572 696f 6429 0a0a 2020 2020  od=period)..    
+00017280: 6465 6620 7365 745f 6566 6665 6374 6976  def set_effectiv
+00017290: 655f 746f 2873 656c 662c 206f 7267 616e  e_to(self, organ
+000172a0: 697a 6174 696f 6e3d 4e6f 6e65 2c20 6566  ization=None, ef
+000172b0: 6665 6374 6976 655f 746f 3d4e 6f6e 6529  fective_to=None)
+000172c0: 3a0a 2020 2020 2020 2020 6966 206f 7267  :.        if org
+000172d0: 616e 697a 6174 696f 6e20 6973 204e 6f6e  anization is Non
+000172e0: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+000172f0: 7267 616e 697a 6174 696f 6e20 3d20 7365  rganization = se
+00017300: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+00017310: 0a20 2020 2020 2020 2066 6869 725f 6566  .        fhir_ef
+00017320: 6665 6374 6976 655f 746f 203d 204e 6f6e  fective_to = Non
+00017330: 650a 2020 2020 2020 2020 6966 2074 7970  e.        if typ
+00017340: 6528 6566 6665 6374 6976 655f 746f 2920  e(effective_to) 
+00017350: 6973 2073 7472 3a0a 2020 2020 2020 2020  is str:.        
+00017360: 2020 2020 6668 6972 5f65 6666 6563 7469      fhir_effecti
+00017370: 7665 5f74 6f20 3d20 4648 4952 4461 7465  ve_to = FHIRDate
+00017380: 286a 736f 6e76 616c 3d65 6666 6563 7469  (jsonval=effecti
+00017390: 7665 5f74 6f29 0a20 2020 2020 2020 2065  ve_to).        e
+000173a0: 6c69 6620 7479 7065 2865 6666 6563 7469  lif type(effecti
+000173b0: 7665 5f74 6f29 2069 7320 4648 4952 4461  ve_to) is FHIRDa
+000173c0: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
+000173d0: 6668 6972 5f65 6666 6563 7469 7665 5f74  fhir_effective_t
+000173e0: 6f20 3d20 6566 6665 6374 6976 655f 746f  o = effective_to
+000173f0: 0a20 2020 2020 2020 2070 6572 696f 645f  .        period_
+00017400: 6578 7420 3d20 7365 6c66 2e67 6574 5f70  ext = self.get_p
+00017410: 6572 696f 645f 6578 7428 290a 2020 2020  eriod_ext().    
+00017420: 2020 2020 6966 2070 6572 696f 645f 6578      if period_ex
+00017430: 7420 6973 204e 6f6e 6520 6f72 2070 6572  t is None or per
+00017440: 696f 645f 6578 742e 7661 6c75 6550 6572  iod_ext.valuePer
+00017450: 696f 6420 6973 204e 6f6e 653a 0a20 2020  iod is None:.   
+00017460: 2020 2020 2020 2020 2070 6572 696f 6420           period 
+00017470: 3d20 5065 7269 6f64 2829 0a20 2020 2020  = Period().     
+00017480: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00017490: 2020 2020 2070 6572 696f 6420 3d20 7065       period = pe
+000174a0: 7269 6f64 5f65 7874 2e76 616c 7565 5065  riod_ext.valuePe
+000174b0: 7269 6f64 0a20 2020 2020 2020 2070 6572  riod.        per
+000174c0: 696f 642e 656e 6420 3d20 6668 6972 5f65  iod.end = fhir_e
+000174d0: 6666 6563 7469 7665 5f74 6f0a 2020 2020  ffective_to.    
+000174e0: 2020 2020 7365 6c66 2e73 6574 5f70 6572      self.set_per
+000174f0: 696f 645f 6578 7428 6f72 6761 6e69 7a61  iod_ext(organiza
+00017500: 7469 6f6e 3d6f 7267 616e 697a 6174 696f  tion=organizatio
+00017510: 6e2c 2070 6572 696f 643d 7065 7269 6f64  n, period=period
+00017520: 290a 0a20 2020 2064 6566 2067 6574 5f70  )..    def get_p
+00017530: 6572 696f 645f 6578 7428 7365 6c66 2c20  eriod_ext(self, 
+00017540: 6f72 6761 6e69 7a61 7469 6f6e 3d4e 6f6e  organization=Non
+00017550: 6529 3a0a 2020 2020 2020 2020 6966 206f  e):.        if o
+00017560: 7267 616e 697a 6174 696f 6e20 6973 204e  rganization is N
+00017570: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00017580: 206f 7267 616e 697a 6174 696f 6e20 3d20   organization = 
+00017590: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
+000175a0: 6365 0a20 2020 2020 2020 2069 6620 6f72  ce.        if or
+000175b0: 6761 6e69 7a61 7469 6f6e 2e65 7874 656e  ganization.exten
+000175c0: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
+000175d0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+000175e0: 7220 6578 7420 696e 206f 7267 616e 697a  r ext in organiz
+000175f0: 6174 696f 6e2e 6578 7465 6e73 696f 6e3a  ation.extension:
+00017600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017610: 2069 6620 6578 742e 7572 6c20 3d3d 2073   if ext.url == s
+00017620: 656c 662e 7065 7269 6f64 5f75 726c 3a0a  elf.period_url:.
+00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017640: 2020 2020 7265 7475 726e 2065 7874 0a20      return ext. 
+00017650: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00017660: 6e65 0a0a 2020 2020 6465 6620 7365 745f  ne..    def set_
+00017670: 7065 7269 6f64 5f65 7874 2873 656c 662c  period_ext(self,
+00017680: 206f 7267 616e 697a 6174 696f 6e3d 4e6f   organization=No
+00017690: 6e65 2c20 7065 7269 6f64 3d4e 6f6e 6529  ne, period=None)
+000176a0: 3a0a 2020 2020 2020 2020 6966 206f 7267  :.        if org
+000176b0: 616e 697a 6174 696f 6e20 6973 204e 6f6e  anization is Non
+000176c0: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+000176d0: 7267 616e 697a 6174 696f 6e20 3d20 7365  rganization = se
+000176e0: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+000176f0: 0a20 2020 2020 2020 2069 6620 6f72 6761  .        if orga
+00017700: 6e69 7a61 7469 6f6e 2e65 7874 656e 7369  nization.extensi
+00017710: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00017720: 2020 2020 2020 2020 6f72 6761 6e69 7a61          organiza
+00017730: 7469 6f6e 2e65 7874 656e 7369 6f6e 203d  tion.extension =
+00017740: 205b 5d0a 2020 2020 2020 2020 7065 7269   [].        peri
+00017750: 6f64 5f65 7874 203d 2073 656c 662e 6765  od_ext = self.ge
+00017760: 745f 7065 7269 6f64 5f65 7874 286f 7267  t_period_ext(org
+00017770: 616e 697a 6174 696f 6e3d 6f72 6761 6e69  anization=organi
+00017780: 7a61 7469 6f6e 290a 2020 2020 2020 2020  zation).        
+00017790: 6966 2070 6572 696f 645f 6578 7420 6973  if period_ext is
+000177a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000177b0: 2020 2070 6572 696f 645f 6578 7420 3d20     period_ext = 
+000177c0: 4578 7465 6e73 696f 6e28 290a 2020 2020  Extension().    
+000177d0: 2020 2020 2020 2020 7065 7269 6f64 5f65          period_e
+000177e0: 7874 2e75 726c 203d 2073 656c 662e 7065  xt.url = self.pe
+000177f0: 7269 6f64 5f75 726c 0a20 2020 2020 2020  riod_url.       
+00017800: 2020 2020 206f 7267 616e 697a 6174 696f       organizatio
+00017810: 6e2e 6578 7465 6e73 696f 6e2e 6170 7065  n.extension.appe
+00017820: 6e64 2870 6572 696f 645f 6578 7429 0a20  nd(period_ext). 
 00017830: 2020 2020 2020 2070 6572 696f 645f 6578         period_ex
-00017840: 7420 3d20 4578 7465 6e73 696f 6e28 290a  t = Extension().
-00017850: 2020 2020 2020 2020 2020 2020 7065 7269              peri
-00017860: 6f64 5f65 7874 2e75 726c 203d 2073 656c  od_ext.url = sel
-00017870: 662e 7065 7269 6f64 5f75 726c 0a20 2020  f.period_url.   
-00017880: 2020 2020 2020 2020 206f 7267 616e 697a           organiz
-00017890: 6174 696f 6e2e 6578 7465 6e73 696f 6e2e  ation.extension.
-000178a0: 6170 7065 6e64 2870 6572 696f 645f 6578  append(period_ex
-000178b0: 7429 0a20 2020 2020 2020 2070 6572 696f  t).        perio
-000178c0: 645f 6578 742e 7661 6c75 6550 6572 696f  d_ext.valuePerio
-000178d0: 6420 3d20 7065 7269 6f64 0a0a 2020 2020  d = period..    
-000178e0: 6465 6620 6765 745f 7068 6f6e 6573 2873  def get_phones(s
-000178f0: 656c 662c 206f 7267 616e 697a 6174 696f  elf, organizatio
-00017900: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
-00017910: 2069 6620 6f72 6761 6e69 7a61 7469 6f6e   if organization
-00017920: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00017930: 2020 2020 2020 6f72 6761 6e69 7a61 7469        organizati
-00017940: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
-00017950: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
-00017960: 7068 6f6e 6573 203d 205b 5d0a 2020 2020  phones = [].    
-00017970: 2020 2020 6966 206f 7267 616e 697a 6174      if organizat
-00017980: 696f 6e2e 7465 6c65 636f 6d20 6973 204e  ion.telecom is N
-00017990: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000179a0: 2072 6574 7572 6e20 7068 6f6e 6573 0a20   return phones. 
-000179b0: 2020 2020 2020 2066 6f72 2074 656c 6563         for telec
-000179c0: 6f6d 2069 6e20 6f72 6761 6e69 7a61 7469  om in organizati
-000179d0: 6f6e 2e74 656c 6563 6f6d 3a0a 2020 2020  on.telecom:.    
-000179e0: 2020 2020 2020 2020 6966 2074 656c 6563          if telec
-000179f0: 6f6d 2e73 7973 7465 6d20 3d3d 2022 7068  om.system == "ph
-00017a00: 6f6e 6522 3a0a 2020 2020 2020 2020 2020  one":.          
-00017a10: 2020 2020 2020 7068 6f6e 6520 3d20 7b7d        phone = {}
-00017a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017a30: 2070 686f 6e65 5b22 7661 6c75 6522 5d20   phone["value"] 
-00017a40: 3d20 7465 6c65 636f 6d2e 7661 6c75 650a  = telecom.value.
-00017a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a60: 7068 6f6e 655b 2275 7365 225d 203d 2074  phone["use"] = t
-00017a70: 656c 6563 6f6d 2e75 7365 0a20 2020 2020  elecom.use.     
-00017a80: 2020 2020 2020 2020 2020 2070 686f 6e65             phone
-00017a90: 732e 6170 7065 6e64 2870 686f 6e65 290a  s.append(phone).
-00017aa0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00017ab0: 686f 6e65 730a 0a20 2020 2064 6566 2067  hones..    def g
-00017ac0: 6574 5f63 6f6e 7461 6374 735f 7068 6f6e  et_contacts_phon
-00017ad0: 6573 2873 656c 662c 206f 7267 616e 697a  es(self, organiz
-00017ae0: 6174 696f 6e3d 4e6f 6e65 293a 0a20 2020  ation=None):.   
-00017af0: 2020 2020 2069 6620 6f72 6761 6e69 7a61       if organiza
-00017b00: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-00017b10: 2020 2020 2020 2020 2020 6f72 6761 6e69            organi
-00017b20: 7a61 7469 6f6e 203d 2073 656c 662e 6668  zation = self.fh
-00017b30: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
-00017b40: 2020 2020 7068 6f6e 6573 203d 205b 5d0a      phones = [].
-00017b50: 2020 2020 2020 2020 6966 206f 7267 616e          if organ
-00017b60: 697a 6174 696f 6e2e 636f 6e74 6163 7420  ization.contact 
-00017b70: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00017b80: 2020 2020 2072 6574 7572 6e20 7068 6f6e       return phon
-00017b90: 6573 0a20 2020 2020 2020 2066 6f72 2063  es.        for c
-00017ba0: 6f6e 7461 6374 2069 6e20 6f72 6761 6e69  ontact in organi
-00017bb0: 7a61 7469 6f6e 2e63 6f6e 7461 6374 3a0a  zation.contact:.
-00017bc0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00017bd0: 6f6e 7461 6374 2e74 656c 6563 6f6d 2069  ontact.telecom i
-00017be0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00017bf0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00017c00: 7465 6c65 636f 6d20 696e 2063 6f6e 7461  telecom in conta
-00017c10: 6374 2e74 656c 6563 6f6d 3a0a 2020 2020  ct.telecom:.    
-00017c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c30: 6966 2074 656c 6563 6f6d 2e73 7973 7465  if telecom.syste
-00017c40: 6d20 3d3d 2022 7068 6f6e 6522 3a0a 2020  m == "phone":.  
-00017c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c60: 2020 2020 2020 7068 6f6e 6520 3d20 7b7d        phone = {}
-00017c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017c80: 2020 2020 2020 2020 2070 686f 6e65 5b22           phone["
-00017c90: 7661 6c75 6522 5d20 3d20 7465 6c65 636f  value"] = teleco
-00017ca0: 6d2e 7661 6c75 650a 2020 2020 2020 2020  m.value.        
-00017cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cc0: 7068 6f6e 655b 2275 7365 225d 203d 2074  phone["use"] = t
-00017cd0: 656c 6563 6f6d 2e75 7365 0a20 2020 2020  elecom.use.     
-00017ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cf0: 2020 2070 686f 6e65 732e 6170 7065 6e64     phones.append
-00017d00: 2870 686f 6e65 290a 2020 2020 2020 2020  (phone).        
-00017d10: 7265 7475 726e 2070 686f 6e65 730a 0a20  return phones.. 
-00017d20: 2020 2064 6566 2069 735f 6163 7469 7665     def is_active
-00017d30: 2873 656c 662c 206f 7267 616e 697a 6174  (self, organizat
-00017d40: 696f 6e3d 4e6f 6e65 293a 0a20 2020 2020  ion=None):.     
-00017d50: 2020 2069 6620 6f72 6761 6e69 7a61 7469     if organizati
-00017d60: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
-00017d70: 2020 2020 2020 2020 6f72 6761 6e69 7a61          organiza
-00017d80: 7469 6f6e 203d 2073 656c 662e 6668 6972  tion = self.fhir
-00017d90: 5f72 6573 6f75 7263 650a 2020 2020 2020  _resource.      
-00017da0: 2020 7265 7475 726e 206f 7267 616e 697a    return organiz
-00017db0: 6174 696f 6e2e 6163 7469 7665 0a0a 2020  ation.active..  
-00017dc0: 2020 6465 6620 7365 6172 6368 2873 656c    def search(sel
-00017dd0: 662c 206e 616d 653d 4e6f 6e65 2c20 6964  f, name=None, id
-00017de0: 656e 7469 6669 6572 3d4e 6f6e 6529 3a0a  entifier=None):.
-00017df0: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-00017e00: 207b 7d0a 2020 2020 2020 2020 6966 206e   {}.        if n
-00017e10: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-00017e20: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-00017e30: 616d 735b 276e 616d 6527 5d20 3d20 6e61  ams['name'] = na
-00017e40: 6d65 0a20 2020 2020 2020 2069 6620 6964  me.        if id
-00017e50: 656e 7469 6669 6572 2069 7320 6e6f 7420  entifier is not 
-00017e60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00017e70: 2020 7061 7261 6d73 5b27 6964 656e 7469    params['identi
-00017e80: 6669 6572 275d 203d 2069 6465 6e74 6966  fier'] = identif
-00017e90: 6965 720a 2020 2020 2020 2020 7265 7370  ier.        resp
-00017ea0: 6f6e 7365 203d 2072 6571 7565 7374 732e  onse = requests.
-00017eb0: 6765 7428 7572 6c3d 7365 6c66 2e6f 7267  get(url=self.org
-00017ec0: 616e 697a 6174 696f 6e5f 656e 6470 6f69  anization_endpoi
-00017ed0: 6e74 2e66 6f72 6d61 7428 6261 7365 5f75  nt.format(base_u
-00017ee0: 726c 3d73 656c 662e 6765 745f 6668 6972  rl=self.get_fhir
-00017ef0: 5f75 726c 2829 292c 2070 6172 616d 733d  _url()), params=
-00017f00: 7061 7261 6d73 2c20 6865 6164 6572 733d  params, headers=
-00017f10: 7365 6c66 2e68 6561 6465 7273 2c20 7665  self.headers, ve
-00017f20: 7269 6679 3d73 656c 662e 7661 6c69 6461  rify=self.valida
-00017f30: 7465 5f63 6572 7473 290a 2020 2020 2020  te_certs).      
-00017f40: 2020 636f 6e74 656e 7420 3d20 6a73 6f6e    content = json
-00017f50: 2e6c 6f61 6473 2872 6573 706f 6e73 652e  .loads(response.
-00017f60: 636f 6e74 656e 742e 6465 636f 6465 2829  content.decode()
-00017f70: 290a 2020 2020 2020 200a 2020 2020 2020  ).       .      
-00017f80: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
-00017f90: 745f 7669 7369 746f 725f 6672 6f6d 5f6a  t_visitor_from_j
-00017fa0: 736f 6e28 6a73 6f6e 6469 6374 3d63 6f6e  son(jsondict=con
-00017fb0: 7465 6e74 290a 0a20 2020 2064 6566 2067  tent)..    def g
-00017fc0: 6574 5f62 795f 6964 2873 656c 662c 206f  et_by_id(self, o
-00017fd0: 7267 5f69 643d 4e6f 6e65 293a 0a20 2020  rg_id=None):.   
-00017fe0: 2020 2020 2069 6620 6f72 675f 6964 2069       if org_id i
-00017ff0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00018000: 2020 2020 6f72 675f 6964 203d 2073 656c      org_id = sel
-00018010: 662e 6765 745f 6964 2829 0a20 2020 2020  f.get_id().     
-00018020: 2020 2069 6620 6f72 675f 6964 2069 7320     if org_id is 
-00018030: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00018040: 2020 2020 2020 7572 6c20 3d20 7365 6c66        url = self
-00018050: 2e6f 7267 616e 697a 6174 696f 6e5f 6279  .organization_by
-00018060: 5f69 645f 656e 6470 6f69 6e74 2e66 6f72  _id_endpoint.for
-00018070: 6d61 7428 6261 7365 5f75 726c 3d73 656c  mat(base_url=sel
-00018080: 662e 6765 745f 6668 6972 5f75 726c 2829  f.get_fhir_url()
-00018090: 2c20 6964 3d6f 7267 5f69 6429 0a20 2020  , id=org_id).   
-000180a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000180b0: 7365 6c66 2e67 6574 5f62 795f 7572 6c28  self.get_by_url(
-000180c0: 7572 6c3d 7572 6c29 0a20 2020 2020 2020  url=url).       
-000180d0: 200a 2020 2020 6465 6620 6765 745f 6279   .    def get_by
-000180e0: 5f72 6566 6572 656e 6365 2873 656c 662c  _reference(self,
-000180f0: 2072 6566 6572 656e 6365 3d4e 6f6e 6529   reference=None)
-00018100: 3a0a 2020 2020 2020 2020 6966 2072 6566  :.        if ref
-00018110: 6572 656e 6365 2069 7320 6e6f 7420 4e6f  erence is not No
-00018120: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00018130: 7572 6c20 3d20 227b 307d 2f7b 317d 222e  url = "{0}/{1}".
-00018140: 666f 726d 6174 2873 656c 662e 6765 745f  format(self.get_
-00018150: 6668 6972 5f75 726c 2829 2c20 7265 6665  fhir_url(), refe
-00018160: 7265 6e63 652e 7265 6665 7265 6e63 6529  rence.reference)
-00018170: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00018180: 7572 6e20 7365 6c66 2e67 6574 5f62 795f  urn self.get_by_
-00018190: 7572 6c28 7572 6c3d 7572 6c29 0a0a 2020  url(url=url)..  
-000181a0: 2020 6465 6620 6765 745f 6279 5f75 726c    def get_by_url
-000181b0: 2873 656c 662c 2075 726c 293a 2020 2020  (self, url):    
-000181c0: 2020 2020 0a20 2020 2020 2020 2072 6573      .        res
-000181d0: 706f 6e73 6520 3d20 7265 7175 6573 7473  ponse = requests
-000181e0: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
-000181f0: 2020 7572 6c3d 7572 6c2c 0a20 2020 2020    url=url,.     
-00018200: 2020 2020 2020 2068 6561 6465 7273 3d73         headers=s
-00018210: 656c 662e 6865 6164 6572 732c 0a20 2020  elf.headers,.   
-00018220: 2020 2020 2020 2020 2076 6572 6966 793d           verify=
-00018230: 7365 6c66 2e76 616c 6964 6174 655f 6365  self.validate_ce
-00018240: 7274 730a 2020 2020 2020 2020 290a 2020  rts.        ).  
-00018250: 2020 2020 2020 6966 2072 6573 706f 6e73        if respons
-00018260: 652e 7374 6174 7573 5f63 6f64 6520 3d3d  e.status_code ==
-00018270: 2032 3030 3a0a 2020 2020 2020 2020 2020   200:.          
-00018280: 2020 6a73 6f6e 6469 6374 203d 206a 736f    jsondict = jso
-00018290: 6e2e 6c6f 6164 7328 7265 7370 6f6e 7365  n.loads(response
-000182a0: 2e63 6f6e 7465 6e74 290a 2020 2020 2020  .content).      
-000182b0: 2020 2020 2020 7265 736f 7572 6365 203d        resource =
-000182c0: 2073 656c 662e 6765 745f 6d6f 6465 6c5f   self.get_model_
-000182d0: 6672 6f6d 5f6a 736f 6e28 6a73 6f6e 6469  from_json(jsondi
-000182e0: 6374 3d6a 736f 6e64 6963 7429 0a20 2020  ct=jsondict).   
-000182f0: 2020 2020 2020 2020 2069 6620 7479 7065           if type
-00018300: 2872 6573 6f75 7263 6529 2069 7320 4f72  (resource) is Or
-00018310: 6761 6e69 7a61 7469 6f6e 3a0a 2020 2020  ganization:.    
-00018320: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018330: 2e66 6869 725f 7265 736f 7572 6365 203d  .fhir_resource =
-00018340: 2072 6573 6f75 7263 650a 2020 2020 2020   resource.      
-00018350: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-00018360: 650a 0a20 2020 2064 6566 2063 7265 6174  e..    def creat
-00018370: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00018380: 2072 6573 203d 2073 656c 662e 6765 7446   res = self.getF
-00018390: 6869 7252 6573 6f75 7263 6528 290a 2020  hirResource().  
-000183a0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-000183b0: 2072 6571 7565 7374 732e 706f 7374 280a   requests.post(.
-000183c0: 2020 2020 2020 2020 2020 2020 7572 6c3d              url=
-000183d0: 7365 6c66 2e6f 7267 616e 697a 6174 696f  self.organizatio
-000183e0: 6e5f 656e 6470 6f69 6e74 2e66 6f72 6d61  n_endpoint.forma
-000183f0: 7428 6261 7365 5f75 726c 3d73 656c 662e  t(base_url=self.
-00018400: 6765 745f 6668 6972 5f75 726c 2829 292c  get_fhir_url()),
-00018410: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00018420: 613d 6a73 6f6e 2e64 756d 7073 2872 6573  a=json.dumps(res
-00018430: 292c 0a20 2020 2020 2020 2020 2020 2068  ),.            h
-00018440: 6561 6465 7273 3d73 656c 662e 6865 6164  eaders=self.head
-00018450: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
-00018460: 2076 6572 6966 793d 7365 6c66 2e76 616c   verify=self.val
-00018470: 6964 6174 655f 6365 7274 7329 0a20 2020  idate_certs).   
-00018480: 2020 2020 2069 6620 7265 7370 6f6e 7365       if response
-00018490: 2e73 7461 7475 735f 636f 6465 203d 3d20  .status_code == 
-000184a0: 3230 313a 0a20 2020 2020 2020 2020 2020  201:.           
-000184b0: 206a 736f 6e64 6963 7420 3d20 6a73 6f6e   jsondict = json
-000184c0: 2e6c 6f61 6473 2872 6573 706f 6e73 652e  .loads(response.
-000184d0: 636f 6e74 656e 7429 0a20 2020 2020 2020  content).       
-000184e0: 2020 2020 2072 6573 6f75 7263 6520 3d20       resource = 
-000184f0: 7365 6c66 2e67 6574 5f6d 6f64 656c 5f66  self.get_model_f
-00018500: 726f 6d5f 6a73 6f6e 286a 736f 6e64 6963  rom_json(jsondic
-00018510: 743d 6a73 6f6e 6469 6374 290a 2020 2020  t=jsondict).    
-00018520: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-00018530: 7265 736f 7572 6365 2920 6973 204f 7267  resource) is Org
-00018540: 616e 697a 6174 696f 6e3a 0a20 2020 2020  anization:.     
-00018550: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018560: 6668 6972 5f72 6573 6f75 7263 6520 3d20  fhir_resource = 
-00018570: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
-00018580: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-00018590: 0a0a 2020 2020 6465 6620 7570 6461 7465  ..    def update
-000185a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000185b0: 7265 7320 3d20 7365 6c66 2e67 6574 4668  res = self.getFh
-000185c0: 6972 5265 736f 7572 6365 2829 0a20 2020  irResource().   
-000185d0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-000185e0: 7265 7175 6573 7473 2e70 7574 280a 2020  requests.put(.  
-000185f0: 2020 2020 2020 2020 2020 7572 6c3d 7365            url=se
-00018600: 6c66 2e6f 7267 616e 697a 6174 696f 6e5f  lf.organization_
-00018610: 6279 5f69 645f 656e 6470 6f69 6e74 2e66  by_id_endpoint.f
-00018620: 6f72 6d61 7428 6261 7365 5f75 726c 3d73  ormat(base_url=s
-00018630: 656c 662e 6765 745f 6668 6972 5f75 726c  elf.get_fhir_url
-00018640: 2829 2c20 6964 3d73 656c 662e 6765 745f  (), id=self.get_
-00018650: 6964 2829 292c 0a20 2020 2020 2020 2020  id()),.         
-00018660: 2020 2064 6174 613d 6a73 6f6e 2e64 756d     data=json.dum
-00018670: 7073 2872 6573 292c 0a20 2020 2020 2020  ps(res),.       
-00018680: 2020 2020 2068 6561 6465 7273 3d73 656c       headers=sel
-00018690: 662e 6865 6164 6572 732c 0a20 2020 2020  f.headers,.     
-000186a0: 2020 2020 2020 2076 6572 6966 793d 7365         verify=se
-000186b0: 6c66 2e76 616c 6964 6174 655f 6365 7274  lf.validate_cert
-000186c0: 7329 0a20 2020 2020 2020 2069 6620 7265  s).        if re
-000186d0: 7370 6f6e 7365 2e73 7461 7475 735f 636f  sponse.status_co
-000186e0: 6465 203d 3d20 3230 303a 0a20 2020 2020  de == 200:.     
-000186f0: 2020 2020 2020 206a 736f 6e64 6963 7420         jsondict 
-00018700: 3d20 6a73 6f6e 2e6c 6f61 6473 2872 6573  = json.loads(res
-00018710: 706f 6e73 652e 636f 6e74 656e 7429 0a20  ponse.content). 
-00018720: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
-00018730: 7263 6520 3d20 7365 6c66 2e67 6574 5f6d  rce = self.get_m
-00018740: 6f64 656c 5f66 726f 6d5f 6a73 6f6e 286a  odel_from_json(j
-00018750: 736f 6e64 6963 743d 6a73 6f6e 6469 6374  sondict=jsondict
-00018760: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00018770: 2074 7970 6528 7265 736f 7572 6365 2920   type(resource) 
-00018780: 6973 204f 7267 616e 697a 6174 696f 6e3a  is Organization:
-00018790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000187a0: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
-000187b0: 7263 6520 3d20 7265 736f 7572 6365 0a20  rce = resource. 
-000187c0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000187d0: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
-000187e0: 6465 6c65 7465 2873 656c 6629 3a0a 2020  delete(self):.  
-000187f0: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
-00018800: 2e67 6574 4668 6972 5265 736f 7572 6365  .getFhirResource
-00018810: 2829 0a20 2020 2020 2020 2072 6573 706f  ().        respo
-00018820: 6e73 6520 3d20 7265 7175 6573 7473 2e64  nse = requests.d
-00018830: 656c 6574 6528 0a20 2020 2020 2020 2020  elete(.         
-00018840: 2020 2075 726c 3d73 656c 662e 6f72 6761     url=self.orga
-00018850: 6e69 7a61 7469 6f6e 5f62 795f 6964 5f65  nization_by_id_e
-00018860: 6e64 706f 696e 742e 666f 726d 6174 2862  ndpoint.format(b
-00018870: 6173 655f 7572 6c3d 7365 6c66 2e67 6574  ase_url=self.get
-00018880: 5f66 6869 725f 7572 6c28 292c 2069 643d  _fhir_url(), id=
-00018890: 7365 6c66 2e67 6574 5f69 6428 2929 2c0a  self.get_id()),.
-000188a0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000188b0: 3d6a 736f 6e2e 6475 6d70 7328 7265 7329  =json.dumps(res)
-000188c0: 2c0a 2020 2020 2020 2020 2020 2020 6865  ,.            he
-000188d0: 6164 6572 733d 7365 6c66 2e68 6561 6465  aders=self.heade
-000188e0: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
-000188f0: 7665 7269 6679 3d73 656c 662e 7661 6c69  verify=self.vali
-00018900: 6461 7465 5f63 6572 7473 290a 2020 2020  date_certs).    
-00018910: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-00018920: 6e73 650a 0a63 6c61 7373 204c 6f63 6174  nse..class Locat
-00018930: 696f 6e46 4849 5228 4261 7365 4648 4952  ionFHIR(BaseFHIR
-00018940: 293a 0a20 2020 206c 6f63 6174 696f 6e5f  ):.    location_
-00018950: 656e 6470 6f69 6e74 203d 2022 7b62 6173  endpoint = "{bas
-00018960: 655f 7572 6c7d 2f4c 6f63 6174 696f 6e22  e_url}/Location"
-00018970: 0a20 2020 206c 6f63 6174 696f 6e5f 6279  .    location_by
-00018980: 5f69 645f 656e 6470 6f69 6e74 203d 206c  _id_endpoint = l
-00018990: 6f63 6174 696f 6e5f 656e 6470 6f69 6e74  ocation_endpoint
-000189a0: 202b 2022 2f7b 6964 7d22 0a20 2020 2072   + "/{id}".    r
-000189b0: 7273 735f 7379 7374 656d 203d 2027 6874  rss_system = 'ht
-000189c0: 7470 733a 2f2f 7072 6f2e 636f 6e73 756c  tps://pro.consul
-000189d0: 7461 7469 6f6e 2e72 7273 732e 7274 7373  tation.rrss.rtss
-000189e0: 2e71 632e 6361 270a 2020 2020 7272 7373  .qc.ca'.    rrss
-000189f0: 5f6d 6f74 5f63 6c65 5f65 7874 656e 7369  _mot_cle_extensi
-00018a00: 6f6e 5f75 726c 203d 2027 6874 7470 3a2f  on_url = 'http:/
-00018a10: 2f77 7777 2e73 616e 7465 7075 626c 6971  /www.santepubliq
-00018a20: 7565 2e72 7473 732e 7163 2e63 612f 7369  ue.rtss.qc.ca/si
-00018a30: 706d 692f 7272 7373 2f31 2e30 2e30 2f65  pmi/rrss/1.0.0/e
-00018a40: 7874 656e 7369 6f6e 732f 236d 6f74 7363  xtensions/#motsc
-00018a50: 6c65 7327 0a20 2020 2070 6572 696f 645f  les'.    period_
-00018a60: 7572 6c20 3d20 2268 7474 703a 2f2f 7777  url = "http://ww
-00018a70: 772e 7361 6e74 6570 7562 6c69 7175 652e  w.santepublique.
-00018a80: 7274 7373 2e71 632e 6361 2f73 6970 6d69  rtss.qc.ca/sipmi
-00018a90: 2f72 7273 732f 312e 302e 302f 6578 7465  /rrss/1.0.0/exte
-00018aa0: 6e73 696f 6e73 2f70 6572 696f 6422 0a0a  nsions/period"..
-00018ab0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00018ac0: 2873 656c 662c 2062 6173 655f 7572 6c3d  (self, base_url=
-00018ad0: 4e6f 6e65 2c20 6261 7365 5f75 7269 3d4e  None, base_uri=N
-00018ae0: 6f6e 652c 2072 6573 6f75 7263 653d 4e6f  one, resource=No
-00018af0: 6e65 2c20 746f 6b65 6e5f 6865 6164 6572  ne, token_header
-00018b00: 3d4e 6f6e 652c 2076 616c 6964 6174 655f  =None, validate_
-00018b10: 6365 7274 733d 5472 7565 2920 2d3e 204e  certs=True) -> N
-00018b20: 6f6e 653a 0a20 2020 2020 2020 2073 7570  one:.        sup
-00018b30: 6572 2829 2e5f 5f69 6e69 745f 5f28 6261  er().__init__(ba
-00018b40: 7365 5f75 726c 3d62 6173 655f 7572 6c2c  se_url=base_url,
-00018b50: 2062 6173 655f 7572 693d 6261 7365 5f75   base_uri=base_u
-00018b60: 7269 2c20 746f 6b65 6e5f 6865 6164 6572  ri, token_header
-00018b70: 3d74 6f6b 656e 5f68 6561 6465 7229 0a20  =token_header). 
-00018b80: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-00018b90: 6461 7465 5f63 6572 7473 203d 2076 616c  date_certs = val
-00018ba0: 6964 6174 655f 6365 7274 730a 2020 2020  idate_certs.    
-00018bb0: 2020 2020 6966 2072 6573 6f75 7263 6520      if resource 
-00018bc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00018bd0: 2020 2020 2020 2020 2073 656c 662e 6668           self.fh
-00018be0: 6972 5f72 6573 6f75 7263 6520 3d20 4c6f  ir_resource = Lo
-00018bf0: 6361 7469 6f6e 286a 736f 6e64 6963 743d  cation(jsondict=
-00018c00: 7265 736f 7572 6365 290a 2020 2020 2020  resource).      
-00018c10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00018c20: 2020 2020 7365 6c66 2e66 6869 725f 7265      self.fhir_re
-00018c30: 736f 7572 6365 203d 204c 6f63 6174 696f  source = Locatio
-00018c40: 6e28 290a 0a20 2020 2064 6566 2067 6574  n()..    def get
-00018c50: 4668 6972 5265 736f 7572 6365 2873 656c  FhirResource(sel
-00018c60: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00018c70: 726e 2073 656c 662e 6668 6972 5f72 6573  rn self.fhir_res
-00018c80: 6f75 7263 652e 6173 5f6a 736f 6e28 290a  ource.as_json().
-00018c90: 0a20 2020 2064 6566 2068 6176 655f 6d6f  .    def have_mo
-00018ca0: 745f 636c 6528 7365 6c66 2c20 6c6f 6361  t_cle(self, loca
-00018cb0: 7469 6f6e 3d4e 6f6e 652c 206d 6f74 5f63  tion=None, mot_c
-00018cc0: 6c65 3d4e 6f6e 6529 3a0a 2020 2020 2020  le=None):.      
-00018cd0: 2020 6966 206c 6f63 6174 696f 6e20 6973    if location is
-00018ce0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00018cf0: 2020 206c 6f63 6174 696f 6e20 3d20 7365     location = se
-00018d00: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
-00018d10: 0a20 2020 2020 2020 2069 6620 6d6f 745f  .        if mot_
-00018d20: 636c 6520 6973 206e 6f74 204e 6f6e 6520  cle is not None 
-00018d30: 616e 6420 6c6f 6361 7469 6f6e 2e65 7874  and location.ext
-00018d40: 656e 7369 6f6e 2069 7320 6e6f 7420 4e6f  ension is not No
-00018d50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00018d60: 666f 7220 6578 7465 6e73 696f 6e20 696e  for extension in
-00018d70: 206c 6f63 6174 696f 6e2e 6578 7465 6e73   location.extens
-00018d80: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-00018d90: 2020 2020 2069 6620 6578 7465 6e73 696f       if extensio
-00018da0: 6e2e 7572 6c20 3d3d 2073 656c 662e 7272  n.url == self.rr
-00018db0: 7373 5f6d 6f74 5f63 6c65 5f65 7874 656e  ss_mot_cle_exten
-00018dc0: 7369 6f6e 5f75 726c 2061 6e64 2065 7874  sion_url and ext
-00018dd0: 656e 7369 6f6e 2e76 616c 7565 5374 7269  ension.valueStri
-00018de0: 6e67 203d 3d20 6d6f 745f 636c 653a 0a20  ng == mot_cle:. 
-00018df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e00: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00018e10: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00018e20: 6c73 650a 0a20 2020 2064 6566 2073 6574  lse..    def set
-00018e30: 5f6e 616d 6528 7365 6c66 2c20 6c6f 6361  _name(self, loca
-00018e40: 7469 6f6e 3d4e 6f6e 652c 206e 616d 653d  tion=None, name=
-00018e50: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
-00018e60: 6620 6c6f 6361 7469 6f6e 2069 7320 4e6f  f location is No
-00018e70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00018e80: 6c6f 6361 7469 6f6e 203d 2073 656c 662e  location = self.
-00018e90: 6668 6972 5f72 6573 6f75 7263 650a 0a20  fhir_resource.. 
-00018ea0: 2020 2020 2020 206c 6f63 6174 696f 6e2e         location.
-00018eb0: 6e61 6d65 203d 206e 616d 650a 0a20 2020  name = name..   
-00018ec0: 2064 6566 2067 6574 5f6e 616d 6528 7365   def get_name(se
-00018ed0: 6c66 2c20 6c6f 6361 7469 6f6e 3d4e 6f6e  lf, location=Non
-00018ee0: 6529 3a0a 2020 2020 2020 2020 6966 206c  e):.        if l
-00018ef0: 6f63 6174 696f 6e20 6973 204e 6f6e 653a  ocation is None:
-00018f00: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-00018f10: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
-00018f20: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
-00018f30: 2020 2072 6574 7572 6e20 6c6f 6361 7469     return locati
-00018f40: 6f6e 2e6e 616d 650a 0a20 2020 2064 6566  on.name..    def
-00018f50: 2067 6574 5f69 6428 7365 6c66 2c20 6c6f   get_id(self, lo
-00018f60: 6361 7469 6f6e 3d4e 6f6e 6529 3a0a 2020  cation=None):.  
-00018f70: 2020 2020 2020 6966 206c 6f63 6174 696f        if locatio
-00018f80: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
-00018f90: 2020 2020 2020 206c 6f63 6174 696f 6e20         location 
-00018fa0: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
-00018fb0: 7572 6365 0a20 2020 2020 2020 2072 6574  urce.        ret
-00018fc0: 7572 6e20 6c6f 6361 7469 6f6e 2e69 640a  urn location.id.
-00018fd0: 0a20 2020 2064 6566 2067 6574 5f69 645f  .    def get_id_
-00018fe0: 7272 7373 2873 656c 662c 206c 6f63 6174  rrss(self, locat
-00018ff0: 696f 6e3d 4e6f 6e65 293a 0a20 2020 2020  ion=None):.     
-00019000: 2020 2069 6620 6c6f 6361 7469 6f6e 2069     if location i
-00019010: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00019020: 2020 2020 6c6f 6361 7469 6f6e 203d 2073      location = s
-00019030: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
-00019040: 650a 2020 2020 2020 2020 6966 206c 6f63  e.        if loc
-00019050: 6174 696f 6e2e 6964 656e 7469 6669 6572  ation.identifier
-00019060: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00019070: 2020 2020 2020 2020 2020 666f 7220 6964            for id
-00019080: 656e 7469 6669 6572 2069 6e20 6c6f 6361  entifier in loca
-00019090: 7469 6f6e 2e69 6465 6e74 6966 6965 723a  tion.identifier:
-000190a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000190b0: 2069 6620 6964 656e 7469 6669 6572 2e73   if identifier.s
-000190c0: 7973 7465 6d20 3d3d 2073 656c 662e 7272  ystem == self.rr
-000190d0: 7373 5f73 7973 7465 6d3a 0a20 2020 2020  ss_system:.     
-000190e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000190f0: 6574 7572 6e20 6964 656e 7469 6669 6572  eturn identifier
-00019100: 2e76 616c 7565 0a20 2020 2020 2020 2072  .value.        r
-00019110: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-00019120: 6465 6620 6765 745f 7068 6f6e 6573 2873  def get_phones(s
-00019130: 656c 662c 206c 6f63 6174 696f 6e3d 4e6f  elf, location=No
-00019140: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
-00019150: 6c6f 6361 7469 6f6e 2069 7320 4e6f 6e65  location is None
-00019160: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00019170: 6361 7469 6f6e 203d 2073 656c 662e 6668  cation = self.fh
-00019180: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
-00019190: 2020 2020 7068 6f6e 6573 203d 205b 5d0a      phones = [].
-000191a0: 2020 2020 2020 2020 6966 206c 6f63 6174          if locat
-000191b0: 696f 6e2e 7465 6c65 636f 6d20 6973 204e  ion.telecom is N
-000191c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000191d0: 2072 6574 7572 6e20 7068 6f6e 6573 0a20   return phones. 
-000191e0: 2020 2020 2020 2066 6f72 2074 656c 6563         for telec
-000191f0: 6f6d 2069 6e20 6c6f 6361 7469 6f6e 2e74  om in location.t
-00019200: 656c 6563 6f6d 3a0a 2020 2020 2020 2020  elecom:.        
-00019210: 2020 2020 6966 2074 656c 6563 6f6d 2e73      if telecom.s
-00019220: 7973 7465 6d20 3d3d 2022 7068 6f6e 6522  ystem == "phone"
-00019230: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019240: 2020 7068 6f6e 6520 3d20 7b7d 0a20 2020    phone = {}.   
-00019250: 2020 2020 2020 2020 2020 2020 2070 686f               pho
-00019260: 6e65 5b22 7661 6c75 6522 5d20 3d20 7465  ne["value"] = te
-00019270: 6c65 636f 6d2e 7661 6c75 650a 2020 2020  lecom.value.    
-00019280: 2020 2020 2020 2020 2020 2020 7068 6f6e              phon
-00019290: 655b 2275 7365 225d 203d 2074 656c 6563  e["use"] = telec
-000192a0: 6f6d 2e75 7365 0a20 2020 2020 2020 2020  om.use.         
-000192b0: 2020 2020 2020 2070 686f 6e65 732e 6170         phones.ap
-000192c0: 7065 6e64 2870 686f 6e65 290a 2020 2020  pend(phone).    
-000192d0: 2020 2020 7265 7475 726e 2070 686f 6e65      return phone
-000192e0: 730a 0a20 2020 2064 6566 2067 6574 5f65  s..    def get_e
-000192f0: 6666 6563 7469 7665 5f66 726f 6d28 7365  ffective_from(se
-00019300: 6c66 2c20 6c6f 6361 7469 6f6e 3d4e 6f6e  lf, location=Non
-00019310: 6529 3a0a 2020 2020 2020 2020 6966 206c  e):.        if l
-00019320: 6f63 6174 696f 6e20 6973 204e 6f6e 653a  ocation is None:
-00019330: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-00019340: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
-00019350: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
-00019360: 2020 2070 6572 696f 645f 6578 7420 3d20     period_ext = 
-00019370: 7365 6c66 2e67 6574 5f70 6572 696f 645f  self.get_period_
-00019380: 6578 7428 6c6f 6361 7469 6f6e 3d6c 6f63  ext(location=loc
-00019390: 6174 696f 6e29 0a20 2020 2020 2020 2069  ation).        i
-000193a0: 6620 7065 7269 6f64 5f65 7874 2069 7320  f period_ext is 
-000193b0: 6e6f 7420 4e6f 6e65 2061 6e64 2070 6572  not None and per
-000193c0: 696f 645f 6578 742e 7661 6c75 6550 6572  iod_ext.valuePer
-000193d0: 696f 6420 6973 206e 6f74 204e 6f6e 653a  iod is not None:
-000193e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000193f0: 2072 6574 7572 6e20 7065 7269 6f64 5f65   return period_e
-00019400: 7874 2e76 616c 7565 5065 7269 6f64 2e73  xt.valuePeriod.s
-00019410: 7461 7274 0a20 2020 2020 2020 2072 6574  tart.        ret
-00019420: 7572 6e20 4e6f 6e65 0a0a 2020 2020 6465  urn None..    de
-00019430: 6620 6765 745f 6566 6665 6374 6976 655f  f get_effective_
-00019440: 746f 2873 656c 662c 206c 6f63 6174 696f  to(self, locatio
-00019450: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
-00019460: 2069 6620 6c6f 6361 7469 6f6e 2069 7320   if location is 
-00019470: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00019480: 2020 6c6f 6361 7469 6f6e 203d 2073 656c    location = sel
-00019490: 662e 6668 6972 5f72 6573 6f75 7263 650a  f.fhir_resource.
-000194a0: 2020 2020 2020 2020 7065 7269 6f64 5f65          period_e
-000194b0: 7874 203d 2073 656c 662e 6765 745f 7065  xt = self.get_pe
-000194c0: 7269 6f64 5f65 7874 286c 6f63 6174 696f  riod_ext(locatio
-000194d0: 6e3d 6c6f 6361 7469 6f6e 290a 2020 2020  n=location).    
-000194e0: 2020 2020 6966 2070 6572 696f 645f 6578      if period_ex
-000194f0: 7420 6973 206e 6f74 204e 6f6e 6520 616e  t is not None an
-00019500: 6420 7065 7269 6f64 5f65 7874 2e76 616c  d period_ext.val
-00019510: 7565 5065 7269 6f64 2069 7320 6e6f 7420  uePeriod is not 
-00019520: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00019530: 2020 2020 2020 7265 7475 726e 2070 6572        return per
-00019540: 696f 645f 6578 742e 7661 6c75 6550 6572  iod_ext.valuePer
-00019550: 696f 642e 656e 640a 2020 2020 2020 2020  iod.end.        
-00019560: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-00019570: 2064 6566 2073 6574 5f65 6666 6563 7469   def set_effecti
-00019580: 7665 5f66 726f 6d28 7365 6c66 2c20 6c6f  ve_from(self, lo
-00019590: 6361 7469 6f6e 3d4e 6f6e 652c 2065 6666  cation=None, eff
-000195a0: 6563 7469 7665 5f66 726f 6d3d 4e6f 6e65  ective_from=None
-000195b0: 293a 0a20 2020 2020 2020 2069 6620 6c6f  ):.        if lo
-000195c0: 6361 7469 6f6e 2069 7320 4e6f 6e65 3a0a  cation is None:.
-000195d0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-000195e0: 7469 6f6e 203d 2073 656c 662e 6668 6972  tion = self.fhir
-000195f0: 5f72 6573 6f75 7263 650a 2020 2020 2020  _resource.      
-00019600: 2020 6668 6972 5f65 6666 6563 7469 7665    fhir_effective
-00019610: 5f66 726f 6d20 3d20 4e6f 6e65 0a20 2020  _from = None.   
-00019620: 2020 2020 2069 6620 7479 7065 2865 6666       if type(eff
-00019630: 6563 7469 7665 5f66 726f 6d29 2069 7320  ective_from) is 
-00019640: 7374 723a 0a20 2020 2020 2020 2020 2020  str:.           
-00019650: 2066 6869 725f 6566 6665 6374 6976 655f   fhir_effective_
-00019660: 6672 6f6d 203d 2046 4849 5244 6174 6528  from = FHIRDate(
-00019670: 6a73 6f6e 7661 6c3d 6566 6665 6374 6976  jsonval=effectiv
-00019680: 655f 6672 6f6d 290a 2020 2020 2020 2020  e_from).        
-00019690: 656c 6966 2074 7970 6528 6566 6665 6374  elif type(effect
-000196a0: 6976 655f 6672 6f6d 2920 6973 2046 4849  ive_from) is FHI
-000196b0: 5244 6174 653a 0a20 2020 2020 2020 2020  RDate:.         
-000196c0: 2020 2066 6869 725f 6566 6665 6374 6976     fhir_effectiv
-000196d0: 655f 6672 6f6d 203d 2065 6666 6563 7469  e_from = effecti
-000196e0: 7665 5f66 726f 6d0a 2020 2020 2020 2020  ve_from.        
-000196f0: 7065 7269 6f64 5f65 7874 203d 2073 656c  period_ext = sel
-00019700: 662e 6765 745f 7065 7269 6f64 5f65 7874  f.get_period_ext
-00019710: 2829 0a20 2020 2020 2020 2069 6620 7065  ().        if pe
-00019720: 7269 6f64 5f65 7874 2069 7320 4e6f 6e65  riod_ext is None
-00019730: 206f 7220 7065 7269 6f64 5f65 7874 2e76   or period_ext.v
-00019740: 616c 7565 5065 7269 6f64 2069 7320 4e6f  aluePeriod is No
-00019750: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00019760: 7065 7269 6f64 203d 2050 6572 696f 6428  period = Period(
-00019770: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00019780: 2020 2020 2020 2020 2020 2020 7065 7269              peri
-00019790: 6f64 203d 2070 6572 696f 645f 6578 742e  od = period_ext.
-000197a0: 7661 6c75 6550 6572 696f 640a 2020 2020  valuePeriod.    
-000197b0: 2020 2020 7065 7269 6f64 2e73 7461 7274      period.start
-000197c0: 203d 2066 6869 725f 6566 6665 6374 6976   = fhir_effectiv
-000197d0: 655f 6672 6f6d 0a20 2020 2020 2020 2073  e_from.        s
-000197e0: 656c 662e 7365 745f 7065 7269 6f64 5f65  elf.set_period_e
-000197f0: 7874 286c 6f63 6174 696f 6e3d 6c6f 6361  xt(location=loca
-00019800: 7469 6f6e 2c20 7065 7269 6f64 3d70 6572  tion, period=per
-00019810: 696f 6429 0a0a 2020 2020 6465 6620 7365  iod)..    def se
-00019820: 745f 6566 6665 6374 6976 655f 746f 2873  t_effective_to(s
-00019830: 656c 662c 206c 6f63 6174 696f 6e3d 4e6f  elf, location=No
-00019840: 6e65 2c20 6566 6665 6374 6976 655f 746f  ne, effective_to
-00019850: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00019860: 6966 206c 6f63 6174 696f 6e20 6973 204e  if location is N
-00019870: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00019880: 206c 6f63 6174 696f 6e20 3d20 7365 6c66   location = self
-00019890: 2e66 6869 725f 7265 736f 7572 6365 0a20  .fhir_resource. 
-000198a0: 2020 2020 2020 2066 6869 725f 6566 6665         fhir_effe
-000198b0: 6374 6976 655f 746f 203d 204e 6f6e 650a  ctive_to = None.
-000198c0: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-000198d0: 6566 6665 6374 6976 655f 746f 2920 6973  effective_to) is
-000198e0: 2073 7472 3a0a 2020 2020 2020 2020 2020   str:.          
-000198f0: 2020 6668 6972 5f65 6666 6563 7469 7665    fhir_effective
-00019900: 5f74 6f20 3d20 4648 4952 4461 7465 286a  _to = FHIRDate(j
-00019910: 736f 6e76 616c 3d65 6666 6563 7469 7665  sonval=effective
-00019920: 5f74 6f29 0a20 2020 2020 2020 2065 6c69  _to).        eli
-00019930: 6620 7479 7065 2865 6666 6563 7469 7665  f type(effective
-00019940: 5f74 6f29 2069 7320 4648 4952 4461 7465  _to) is FHIRDate
-00019950: 3a0a 2020 2020 2020 2020 2020 2020 6668  :.            fh
-00019960: 6972 5f65 6666 6563 7469 7665 5f74 6f20  ir_effective_to 
-00019970: 3d20 6566 6665 6374 6976 655f 746f 0a20  = effective_to. 
-00019980: 2020 2020 2020 2070 6572 696f 645f 6578         period_ex
-00019990: 7420 3d20 7365 6c66 2e67 6574 5f70 6572  t = self.get_per
-000199a0: 696f 645f 6578 7428 290a 2020 2020 2020  iod_ext().      
-000199b0: 2020 6966 2070 6572 696f 645f 6578 7420    if period_ext 
-000199c0: 6973 204e 6f6e 6520 6f72 2070 6572 696f  is None or perio
-000199d0: 645f 6578 742e 7661 6c75 6550 6572 696f  d_ext.valuePerio
-000199e0: 6420 6973 204e 6f6e 653a 0a20 2020 2020  d is None:.     
-000199f0: 2020 2020 2020 2070 6572 696f 6420 3d20         period = 
-00019a00: 5065 7269 6f64 2829 0a20 2020 2020 2020  Period().       
-00019a10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00019a20: 2020 2070 6572 696f 6420 3d20 7065 7269     period = peri
-00019a30: 6f64 5f65 7874 2e76 616c 7565 5065 7269  od_ext.valuePeri
-00019a40: 6f64 0a20 2020 2020 2020 2070 6572 696f  od.        perio
-00019a50: 642e 656e 6420 3d20 6668 6972 5f65 6666  d.end = fhir_eff
-00019a60: 6563 7469 7665 5f74 6f0a 2020 2020 2020  ective_to.      
-00019a70: 2020 7365 6c66 2e73 6574 5f70 6572 696f    self.set_perio
-00019a80: 645f 6578 7428 6c6f 6361 7469 6f6e 3d6c  d_ext(location=l
-00019a90: 6f63 6174 696f 6e2c 2070 6572 696f 643d  ocation, period=
-00019aa0: 7065 7269 6f64 290a 0a20 2020 2064 6566  period)..    def
-00019ab0: 2067 6574 5f70 6572 696f 645f 6578 7428   get_period_ext(
-00019ac0: 7365 6c66 2c20 6c6f 6361 7469 6f6e 3d4e  self, location=N
-00019ad0: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-00019ae0: 206c 6f63 6174 696f 6e20 6973 204e 6f6e   location is Non
-00019af0: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
-00019b00: 6f63 6174 696f 6e20 3d20 7365 6c66 2e66  ocation = self.f
-00019b10: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
-00019b20: 2020 2020 2069 6620 6c6f 6361 7469 6f6e       if location
-00019b30: 2e65 7874 656e 7369 6f6e 2069 7320 6e6f  .extension is no
-00019b40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00019b50: 2020 2020 666f 7220 6578 7420 696e 206c      for ext in l
-00019b60: 6f63 6174 696f 6e2e 6578 7465 6e73 696f  ocation.extensio
-00019b70: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
-00019b80: 2020 2069 6620 6578 742e 7572 6c20 3d3d     if ext.url ==
-00019b90: 2073 656c 662e 7065 7269 6f64 5f75 726c   self.period_url
-00019ba0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019bb0: 2020 2020 2020 7265 7475 726e 2065 7874        return ext
-00019bc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00019bd0: 4e6f 6e65 0a0a 2020 2020 6465 6620 7365  None..    def se
-00019be0: 745f 7065 7269 6f64 5f65 7874 2873 656c  t_period_ext(sel
-00019bf0: 662c 206c 6f63 6174 696f 6e3d 4e6f 6e65  f, location=None
-00019c00: 2c20 7065 7269 6f64 3d4e 6f6e 6529 3a0a  , period=None):.
-00019c10: 2020 2020 2020 2020 6966 206c 6f63 6174          if locat
-00019c20: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
-00019c30: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
-00019c40: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
-00019c50: 736f 7572 6365 0a20 2020 2020 2020 2069  source.        i
-00019c60: 6620 6c6f 6361 7469 6f6e 2e65 7874 656e  f location.exten
-00019c70: 7369 6f6e 2069 7320 4e6f 6e65 3a0a 2020  sion is None:.  
-00019c80: 2020 2020 2020 2020 2020 6c6f 6361 7469            locati
-00019c90: 6f6e 2e65 7874 656e 7369 6f6e 203d 205b  on.extension = [
-00019ca0: 5d0a 2020 2020 2020 2020 7065 7269 6f64  ].        period
-00019cb0: 5f65 7874 203d 2073 656c 662e 6765 745f  _ext = self.get_
-00019cc0: 7065 7269 6f64 5f65 7874 286c 6f63 6174  period_ext(locat
-00019cd0: 696f 6e3d 6c6f 6361 7469 6f6e 290a 2020  ion=location).  
-00019ce0: 2020 2020 2020 6966 2070 6572 696f 645f        if period_
-00019cf0: 6578 7420 6973 204e 6f6e 653a 0a20 2020  ext is None:.   
-00019d00: 2020 2020 2020 2020 2070 6572 696f 645f           period_
-00019d10: 6578 7420 3d20 4578 7465 6e73 696f 6e28  ext = Extension(
-00019d20: 290a 2020 2020 2020 2020 2020 2020 7065  ).            pe
-00019d30: 7269 6f64 5f65 7874 2e75 726c 203d 2073  riod_ext.url = s
-00019d40: 656c 662e 7065 7269 6f64 5f75 726c 0a20  elf.period_url. 
-00019d50: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
-00019d60: 696f 6e2e 6578 7465 6e73 696f 6e2e 6170  ion.extension.ap
-00019d70: 7065 6e64 2870 6572 696f 645f 6578 7429  pend(period_ext)
-00019d80: 0a20 2020 2020 2020 2070 6572 696f 645f  .        period_
-00019d90: 6578 742e 7661 6c75 6550 6572 696f 6420  ext.valuePeriod 
-00019da0: 3d20 7065 7269 6f64 0a0a 2020 2020 6465  = period..    de
-00019db0: 6620 6973 5f61 6374 6976 6528 7365 6c66  f is_active(self
-00019dc0: 2c20 6c6f 6361 7469 6f6e 3d4e 6f6e 6529  , location=None)
-00019dd0: 3a0a 2020 2020 2020 2020 6966 206c 6f63  :.        if loc
-00019de0: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
-00019df0: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
-00019e00: 696f 6e20 3d20 7365 6c66 2e66 6869 725f  ion = self.fhir_
-00019e10: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
-00019e20: 2069 6620 6c6f 6361 7469 6f6e 2e73 7461   if location.sta
-00019e30: 7475 7320 3d3d 2022 6163 7469 7665 223a  tus == "active":
-00019e40: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00019e50: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-00019e60: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-00019e70: 2020 2020 2020 0a20 2020 2064 6566 2073        .    def s
-00019e80: 6561 7263 6828 7365 6c66 2c20 6e61 6d65  earch(self, name
-00019e90: 3d4e 6f6e 652c 2061 6464 7265 7373 5f63  =None, address_c
-00019ea0: 6974 793d 4e6f 6e65 2c20 6964 656e 7469  ity=None, identi
-00019eb0: 6669 6572 3d4e 6f6e 6529 3a0a 2020 2020  fier=None):.    
-00019ec0: 2020 2020 7061 7261 6d73 203d 207b 7d0a      params = {}.
-00019ed0: 2020 2020 2020 2020 6966 206e 616d 6520          if name 
-00019ee0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00019ef0: 2020 2020 2020 2020 2070 6172 616d 735b           params[
-00019f00: 276e 616d 6527 5d20 3d20 6e61 6d65 0a20  'name'] = name. 
-00019f10: 2020 2020 2020 2069 6620 6964 656e 7469         if identi
-00019f20: 6669 6572 2069 7320 6e6f 7420 4e6f 6e65  fier is not None
-00019f30: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00019f40: 7261 6d73 5b27 6964 656e 7469 6669 6572  rams['identifier
-00019f50: 275d 203d 2069 6465 6e74 6966 6965 720a  '] = identifier.
-00019f60: 2020 2020 2020 2020 6966 2061 6464 7265          if addre
-00019f70: 7373 5f63 6974 7920 6973 206e 6f74 204e  ss_city is not N
-00019f80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00019f90: 2070 6172 616d 735b 2761 6464 7265 7373   params['address
-00019fa0: 2d63 6974 7927 5d20 3d20 6164 6472 6573  -city'] = addres
-00019fb0: 735f 6369 7479 0a20 2020 2020 2020 2072  s_city.        r
-00019fc0: 6573 706f 6e73 6520 3d20 7265 7175 6573  esponse = reques
-00019fd0: 7473 2e67 6574 280a 2020 2020 2020 2020  ts.get(.        
-00019fe0: 2020 2020 7572 6c3d 7365 6c66 2e6c 6f63      url=self.loc
-00019ff0: 6174 696f 6e5f 656e 6470 6f69 6e74 2e66  ation_endpoint.f
-0001a000: 6f72 6d61 7428 6261 7365 5f75 726c 3d73  ormat(base_url=s
-0001a010: 656c 662e 6765 745f 6668 6972 5f75 726c  elf.get_fhir_url
-0001a020: 2829 292c 0a20 2020 2020 2020 2020 2020  ()),.           
-0001a030: 2070 6172 616d 733d 7061 7261 6d73 2c0a   params=params,.
-0001a040: 2020 2020 2020 2020 2020 2020 6865 6164              head
-0001a050: 6572 733d 7365 6c66 2e68 6561 6465 7273  ers=self.headers
-0001a060: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
-0001a070: 7269 6679 3d73 656c 662e 7661 6c69 6461  rify=self.valida
-0001a080: 7465 5f63 6572 7473 290a 2020 2020 2020  te_certs).      
-0001a090: 2020 636f 6e74 656e 7420 3d20 6a73 6f6e    content = json
-0001a0a0: 2e6c 6f61 6473 2872 6573 706f 6e73 652e  .loads(response.
-0001a0b0: 636f 6e74 656e 742e 6465 636f 6465 2829  content.decode()
-0001a0c0: 290a 2020 2020 0a20 2020 2020 2020 2072  ).    .        r
-0001a0d0: 6574 7572 6e20 7365 6c66 2e67 6574 5f76  eturn self.get_v
-0001a0e0: 6973 6974 6f72 5f66 726f 6d5f 6a73 6f6e  isitor_from_json
-0001a0f0: 286a 736f 6e64 6963 743d 636f 6e74 656e  (jsondict=conten
-0001a100: 7429 0a0a 2020 2020 6465 6620 6765 745f  t)..    def get_
-0001a110: 6279 5f69 6428 7365 6c66 2c20 6c6f 6361  by_id(self, loca
-0001a120: 7469 6f6e 5f69 643d 4e6f 6e65 293a 0a20  tion_id=None):. 
-0001a130: 2020 2020 2020 2069 6620 6c6f 6361 7469         if locati
-0001a140: 6f6e 5f69 6420 6973 204e 6f6e 653a 0a20  on_id is None:. 
-0001a150: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
-0001a160: 696f 6e5f 6964 203d 2073 656c 662e 6765  ion_id = self.ge
-0001a170: 745f 6964 2829 0a20 2020 2020 2020 2069  t_id().        i
-0001a180: 6620 6c6f 6361 7469 6f6e 5f69 6420 6973  f location_id is
-0001a190: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0001a1a0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-0001a1b0: 3d20 7265 7175 6573 7473 2e67 6574 280a  = requests.get(.
-0001a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1d0: 7572 6c3d 7365 6c66 2e6c 6f63 6174 696f  url=self.locatio
-0001a1e0: 6e5f 6279 5f69 645f 656e 6470 6f69 6e74  n_by_id_endpoint
-0001a1f0: 2e66 6f72 6d61 7428 6261 7365 5f75 726c  .format(base_url
-0001a200: 3d73 656c 662e 6765 745f 6668 6972 5f75  =self.get_fhir_u
-0001a210: 726c 2829 2c20 6964 3d6c 6f63 6174 696f  rl(), id=locatio
-0001a220: 6e5f 6964 292c 0a20 2020 2020 2020 2020  n_id),.         
-0001a230: 2020 2020 2020 2068 6561 6465 7273 3d73         headers=s
-0001a240: 656c 662e 6865 6164 6572 732c 0a20 2020  elf.headers,.   
-0001a250: 2020 2020 2020 2020 2020 2020 2076 6572               ver
-0001a260: 6966 793d 7365 6c66 2e76 616c 6964 6174  ify=self.validat
-0001a270: 655f 6365 7274 730a 2020 2020 2020 2020  e_certs.        
-0001a280: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0001a290: 2020 6966 2072 6573 706f 6e73 652e 7374    if response.st
-0001a2a0: 6174 7573 5f63 6f64 6520 3d3d 2032 3030  atus_code == 200
-0001a2b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001a2c0: 2020 6a73 6f6e 6469 6374 203d 206a 736f    jsondict = jso
-0001a2d0: 6e2e 6c6f 6164 7328 7265 7370 6f6e 7365  n.loads(response
-0001a2e0: 2e63 6f6e 7465 6e74 290a 2020 2020 2020  .content).      
-0001a2f0: 2020 2020 2020 2020 2020 7265 736f 7572            resour
-0001a300: 6365 203d 2073 656c 662e 6765 745f 6d6f  ce = self.get_mo
-0001a310: 6465 6c5f 6672 6f6d 5f6a 736f 6e28 6a73  del_from_json(js
-0001a320: 6f6e 6469 6374 3d6a 736f 6e64 6963 7429  ondict=jsondict)
-0001a330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a340: 2069 6620 7479 7065 2872 6573 6f75 7263   if type(resourc
-0001a350: 6529 2069 7320 4c6f 6361 7469 6f6e 3a0a  e) is Location:.
-0001a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a370: 2020 2020 7365 6c66 2e66 6869 725f 7265      self.fhir_re
-0001a380: 736f 7572 6365 203d 2072 6573 6f75 7263  source = resourc
-0001a390: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
-0001a3a0: 7475 726e 2072 6573 706f 6e73 650a 2020  turn response.  
-0001a3b0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-0001a3c0: 650a 0a20 2020 2064 6566 2063 7265 6174  e..    def creat
-0001a3d0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0001a3e0: 2072 6573 203d 2073 656c 662e 6765 7446   res = self.getF
-0001a3f0: 6869 7252 6573 6f75 7263 6528 290a 2020  hirResource().  
-0001a400: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-0001a410: 2072 6571 7565 7374 732e 706f 7374 280a   requests.post(.
-0001a420: 2020 2020 2020 2020 2020 2020 7572 6c3d              url=
-0001a430: 7365 6c66 2e6c 6f63 6174 696f 6e5f 656e  self.location_en
-0001a440: 6470 6f69 6e74 2e66 6f72 6d61 7428 6261  dpoint.format(ba
-0001a450: 7365 5f75 726c 3d73 656c 662e 6765 745f  se_url=self.get_
-0001a460: 6668 6972 5f75 726c 2829 292c 0a20 2020  fhir_url()),.   
-0001a470: 2020 2020 2020 2020 2064 6174 613d 6a73           data=js
-0001a480: 6f6e 2e64 756d 7073 2872 6573 292c 0a20  on.dumps(res),. 
-0001a490: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-0001a4a0: 7273 3d73 656c 662e 6865 6164 6572 732c  rs=self.headers,
-0001a4b0: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
-0001a4c0: 6966 793d 7365 6c66 2e76 616c 6964 6174  ify=self.validat
-0001a4d0: 655f 6365 7274 7329 0a20 2020 2020 2020  e_certs).       
-0001a4e0: 2069 6620 7265 7370 6f6e 7365 2e73 7461   if response.sta
-0001a4f0: 7475 735f 636f 6465 203d 3d20 3230 313a  tus_code == 201:
-0001a500: 0a20 2020 2020 2020 2020 2020 206a 736f  .            jso
-0001a510: 6e64 6963 7420 3d20 6a73 6f6e 2e6c 6f61  ndict = json.loa
-0001a520: 6473 2872 6573 706f 6e73 652e 636f 6e74  ds(response.cont
-0001a530: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
-0001a540: 2072 6573 6f75 7263 6520 3d20 7365 6c66   resource = self
-0001a550: 2e67 6574 5f6d 6f64 656c 5f66 726f 6d5f  .get_model_from_
-0001a560: 6a73 6f6e 286a 736f 6e64 6963 743d 6a73  json(jsondict=js
-0001a570: 6f6e 6469 6374 290a 2020 2020 2020 2020  ondict).        
-0001a580: 2020 2020 6966 2074 7970 6528 7265 736f      if type(reso
-0001a590: 7572 6365 2920 6973 204c 6f63 6174 696f  urce) is Locatio
-0001a5a0: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
-0001a5b0: 2020 2073 656c 662e 6668 6972 5f72 6573     self.fhir_res
-0001a5c0: 6f75 7263 6520 3d20 7265 736f 7572 6365  ource = resource
-0001a5d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001a5e0: 7265 7370 6f6e 7365 0a0a 2020 2020 6465  response..    de
-0001a5f0: 6620 7570 6461 7465 2873 656c 6629 3a0a  f update(self):.
-0001a600: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-0001a610: 6c66 2e67 6574 4668 6972 5265 736f 7572  lf.getFhirResour
-0001a620: 6365 2829 0a20 2020 2020 2020 2072 6573  ce().        res
-0001a630: 706f 6e73 6520 3d20 7265 7175 6573 7473  ponse = requests
-0001a640: 2e70 7574 280a 2020 2020 2020 2020 2020  .put(.          
-0001a650: 2020 7572 6c3d 7365 6c66 2e6c 6f63 6174    url=self.locat
-0001a660: 696f 6e5f 6279 5f69 645f 656e 6470 6f69  ion_by_id_endpoi
-0001a670: 6e74 2e66 6f72 6d61 7428 6261 7365 5f75  nt.format(base_u
-0001a680: 726c 3d73 656c 662e 6765 745f 6668 6972  rl=self.get_fhir
-0001a690: 5f75 726c 2829 2c20 6964 3d73 656c 662e  _url(), id=self.
-0001a6a0: 6765 745f 6964 2829 292c 0a20 2020 2020  get_id()),.     
-0001a6b0: 2020 2020 2020 2064 6174 613d 6a73 6f6e         data=json
-0001a6c0: 2e64 756d 7073 2872 6573 292c 0a20 2020  .dumps(res),.   
-0001a6d0: 2020 2020 2020 2020 2068 6561 6465 7273           headers
-0001a6e0: 3d73 656c 662e 6865 6164 6572 732c 0a20  =self.headers,. 
-0001a6f0: 2020 2020 2020 2020 2020 2076 6572 6966             verif
-0001a700: 793d 7365 6c66 2e76 616c 6964 6174 655f  y=self.validate_
-0001a710: 6365 7274 7329 0a20 2020 2020 2020 2069  certs).        i
-0001a720: 6620 7265 7370 6f6e 7365 2e73 7461 7475  f response.statu
-0001a730: 735f 636f 6465 203d 3d20 3230 303a 0a20  s_code == 200:. 
-0001a740: 2020 2020 2020 2020 2020 206a 736f 6e64             jsond
-0001a750: 6963 7420 3d20 6a73 6f6e 2e6c 6f61 6473  ict = json.loads
-0001a760: 2872 6573 706f 6e73 652e 636f 6e74 656e  (response.conten
-0001a770: 7429 0a20 2020 2020 2020 2020 2020 2072  t).            r
-0001a780: 6573 6f75 7263 6520 3d20 7365 6c66 2e67  esource = self.g
-0001a790: 6574 5f6d 6f64 656c 5f66 726f 6d5f 6a73  et_model_from_js
-0001a7a0: 6f6e 286a 736f 6e64 6963 743d 6a73 6f6e  on(jsondict=json
-0001a7b0: 6469 6374 290a 2020 2020 2020 2020 2020  dict).          
-0001a7c0: 2020 6966 2074 7970 6528 7265 736f 7572    if type(resour
-0001a7d0: 6365 2920 6973 204c 6f63 6174 696f 6e3a  ce) is Location:
-0001a7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a7f0: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
-0001a800: 7263 6520 3d20 7265 736f 7572 6365 0a20  rce = resource. 
-0001a810: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0001a820: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
-0001a830: 6465 6c65 7465 2873 656c 6629 3a0a 2020  delete(self):.  
-0001a840: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
-0001a850: 2e67 6574 4668 6972 5265 736f 7572 6365  .getFhirResource
-0001a860: 2829 0a20 2020 2020 2020 2072 6573 706f  ().        respo
-0001a870: 6e73 6520 3d20 7265 7175 6573 7473 2e64  nse = requests.d
-0001a880: 656c 6574 6528 0a20 2020 2020 2020 2020  elete(.         
-0001a890: 2020 2075 726c 3d73 656c 662e 6c6f 6361     url=self.loca
-0001a8a0: 7469 6f6e 5f62 795f 6964 5f65 6e64 706f  tion_by_id_endpo
-0001a8b0: 696e 742e 666f 726d 6174 2862 6173 655f  int.format(base_
-0001a8c0: 7572 6c3d 7365 6c66 2e67 6574 5f66 6869  url=self.get_fhi
-0001a8d0: 725f 7572 6c28 292c 2069 643d 7365 6c66  r_url(), id=self
-0001a8e0: 2e67 6574 5f69 6428 2929 2c0a 2020 2020  .get_id()),.    
-0001a8f0: 2020 2020 2020 2020 6461 7461 3d6a 736f          data=jso
-0001a900: 6e2e 6475 6d70 7328 7265 7329 2c0a 2020  n.dumps(res),.  
-0001a910: 2020 2020 2020 2020 2020 6865 6164 6572            header
-0001a920: 733d 7365 6c66 2e68 6561 6465 7273 2c0a  s=self.headers,.
-0001a930: 2020 2020 2020 2020 2020 2020 7665 7269              veri
-0001a940: 6679 3d73 656c 662e 7661 6c69 6461 7465  fy=self.validate
-0001a950: 5f63 6572 7473 290a 2020 2020 2020 2020  _certs).        
-0001a960: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-0001a970: 0a63 6c61 7373 204d 6564 6963 6174 696f  .class Medicatio
-0001a980: 6e46 4849 5228 4261 7365 4648 4952 293a  nFHIR(BaseFHIR):
-0001a990: 0a20 2020 206d 6564 6963 6174 696f 6e5f  .    medication_
-0001a9a0: 656e 6470 6f69 6e74 203d 2022 7b62 6173  endpoint = "{bas
-0001a9b0: 655f 7572 6c7d 2f4d 6564 6963 6174 696f  e_url}/Medicatio
-0001a9c0: 6e22 0a20 2020 2067 6574 5f62 795f 7472  n".    get_by_tr
-0001a9d0: 6164 655f 6e61 6d65 5f65 6e64 706f 696e  ade_name_endpoin
-0001a9e0: 7420 3d20 6d65 6469 6361 7469 6f6e 5f65  t = medication_e
-0001a9f0: 6e64 706f 696e 7420 2b20 222f 7b74 7261  ndpoint + "/{tra
-0001aa00: 6465 5f6e 616d 657d 220a 2020 2020 6465  de_name}".    de
-0001aa10: 6661 756c 745f 7175 616e 7469 7479 5f75  fault_quantity_u
-0001aa20: 726c 203d 2027 6874 7470 3a2f 2f77 7777  rl = 'http://www
-0001aa30: 2e73 616e 7465 7075 626c 6971 7565 2e72  .santepublique.r
-0001aa40: 7473 732e 7163 2e63 612f 7369 706d 692f  tss.qc.ca/sipmi/
-0001aa50: 6661 2f31 2e30 2e30 2f65 7874 656e 7369  fa/1.0.0/extensi
-0001aa60: 6f6e 732f 236d 6564 6963 6174 696f 6e2f  ons/#medication/
-0001aa70: 6465 6661 756c 7471 7561 6e74 6974 7927  defaultquantity'
-0001aa80: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-0001aa90: 5f5f 2873 656c 662c 2062 6173 655f 7572  __(self, base_ur
-0001aaa0: 6c3d 4e6f 6e65 2c20 6261 7365 5f75 7269  l=None, base_uri
-0001aab0: 3d4e 6f6e 652c 2072 6573 6f75 7263 653d  =None, resource=
-0001aac0: 4e6f 6e65 2c20 746f 6b65 6e5f 6865 6164  None, token_head
-0001aad0: 6572 3d4e 6f6e 652c 2076 616c 6964 6174  er=None, validat
-0001aae0: 655f 6365 7274 733d 5472 7565 2920 2d3e  e_certs=True) ->
-0001aaf0: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-0001ab00: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-0001ab10: 6261 7365 5f75 726c 3d62 6173 655f 7572  base_url=base_ur
-0001ab20: 6c2c 2062 6173 655f 7572 693d 6261 7365  l, base_uri=base
-0001ab30: 5f75 7269 2c20 746f 6b65 6e5f 6865 6164  _uri, token_head
-0001ab40: 6572 3d74 6f6b 656e 5f68 6561 6465 7229  er=token_header)
-0001ab50: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
-0001ab60: 6c69 6461 7465 5f63 6572 7473 203d 2076  lidate_certs = v
-0001ab70: 616c 6964 6174 655f 6365 7274 730a 2020  alidate_certs.  
-0001ab80: 2020 2020 2020 6966 2072 6573 6f75 7263        if resourc
-0001ab90: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-0001aba0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001abb0: 6668 6972 5f72 6573 6f75 7263 6520 3d20  fhir_resource = 
-0001abc0: 4d65 6469 6361 7469 6f6e 286a 736f 6e64  Medication(jsond
-0001abd0: 6963 743d 7265 736f 7572 6365 290a 2020  ict=resource).  
-0001abe0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001abf0: 2020 2020 2020 2020 7365 6c66 2e66 6869          self.fhi
-0001ac00: 725f 7265 736f 7572 6365 203d 204d 6564  r_resource = Med
-0001ac10: 6963 6174 696f 6e28 290a 0a20 2020 2064  ication()..    d
-0001ac20: 6566 2067 6574 4668 6972 5265 736f 7572  ef getFhirResour
-0001ac30: 6365 2873 656c 6629 3a0a 2020 2020 2020  ce(self):.      
-0001ac40: 2020 7265 7475 726e 2073 656c 662e 6668    return self.fh
-0001ac50: 6972 5f72 6573 6f75 7263 652e 6173 5f6a  ir_resource.as_j
-0001ac60: 736f 6e28 290a 0a20 2020 2064 6566 2067  son()..    def g
-0001ac70: 6574 5f62 6174 6368 6573 2873 656c 6629  et_batches(self)
-0001ac80: 3a0a 2020 2020 2020 2020 6966 2074 7970  :.        if typ
-0001ac90: 6528 7365 6c66 2e66 6869 725f 7265 736f  e(self.fhir_reso
-0001aca0: 7572 6365 2e70 726f 6475 6374 2920 6973  urce.product) is
-0001acb0: 204d 6564 6963 6174 696f 6e50 726f 6475   MedicationProdu
-0001acc0: 6374 2061 6e64 2074 7970 6528 7365 6c66  ct and type(self
-0001acd0: 2e66 6869 725f 7265 736f 7572 6365 2e70  .fhir_resource.p
-0001ace0: 726f 6475 6374 2e62 6174 6368 2920 6973  roduct.batch) is
-0001acf0: 206c 6973 743a 0a20 2020 2020 2020 2020   list:.         
-0001ad00: 2020 2072 6574 7572 6e20 7365 6c66 2e66     return self.f
-0001ad10: 6869 725f 7265 736f 7572 6365 2e70 726f  hir_resource.pro
-0001ad20: 6475 6374 2e62 6174 6368 0a20 2020 2020  duct.batch.     
-0001ad30: 2020 2072 6574 7572 6e20 5b5d 0a0a 2020     return []..  
-0001ad40: 2020 6465 6620 6765 745f 6279 5f74 7261    def get_by_tra
-0001ad50: 6465 5f6e 616d 6528 7365 6c66 2c20 7472  de_name(self, tr
-0001ad60: 6164 655f 6e61 6d65 293a 0a20 2020 2020  ade_name):.     
-0001ad70: 2020 206d 6564 6963 6174 696f 6e5f 7265     medication_re
-0001ad80: 7370 6f6e 7365 203d 2072 6571 7565 7374  sponse = request
-0001ad90: 732e 6765 7428 0a20 2020 2020 2020 2020  s.get(.         
-0001ada0: 2020 2075 726c 3d73 656c 662e 6765 745f     url=self.get_
-0001adb0: 6279 5f74 7261 6465 5f6e 616d 655f 656e  by_trade_name_en
-0001adc0: 6470 6f69 6e74 2e66 6f72 6d61 7428 6261  dpoint.format(ba
-0001add0: 7365 5f75 726c 3d73 656c 662e 6765 745f  se_url=self.get_
-0001ade0: 6668 6972 5f75 726c 2829 2c20 7472 6164  fhir_url(), trad
-0001adf0: 655f 6e61 6d65 3d74 7261 6465 5f6e 616d  e_name=trade_nam
-0001ae00: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-0001ae10: 6865 6164 6572 733d 7365 6c66 2e68 6561  headers=self.hea
-0001ae20: 6465 7273 2c0a 2020 2020 2020 2020 2020  ders,.          
-0001ae30: 2020 7665 7269 6679 3d73 656c 662e 7661    verify=self.va
-0001ae40: 6c69 6461 7465 5f63 6572 7473 0a20 2020  lidate_certs.   
-0001ae50: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-0001ae60: 6620 6d65 6469 6361 7469 6f6e 5f72 6573  f medication_res
-0001ae70: 706f 6e73 652e 7374 6174 7573 5f63 6f64  ponse.status_cod
-0001ae80: 6520 3d3d 2032 3030 3a0a 2020 2020 2020  e == 200:.      
-0001ae90: 2020 2020 2020 6d65 6469 6361 7469 6f6e        medication
-0001aea0: 5f64 6963 7420 3d20 6a73 6f6e 2e6c 6f61  _dict = json.loa
-0001aeb0: 6473 286d 6564 6963 6174 696f 6e5f 7265  ds(medication_re
-0001aec0: 7370 6f6e 7365 2e63 6f6e 7465 6e74 290a  sponse.content).
-0001aed0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001aee0: 2e66 6869 725f 7265 736f 7572 6365 203d  .fhir_resource =
-0001aef0: 204d 6564 6963 6174 696f 6e28 6a73 6f6e   Medication(json
-0001af00: 6469 6374 3d6d 6564 6963 6174 696f 6e5f  dict=medication_
-0001af10: 6469 6374 290a 0a20 2020 2064 6566 2067  dict)..    def g
-0001af20: 6574 5f64 6566 6175 6c74 5f71 7561 6e74  et_default_quant
-0001af30: 6974 795f 666f 725f 6261 7463 6828 7365  ity_for_batch(se
-0001af40: 6c66 2c20 6261 7463 6829 3a0a 2020 2020  lf, batch):.    
-0001af50: 2020 2020 666f 7220 6578 7420 696e 2062      for ext in b
-0001af60: 6174 6368 2e65 7874 656e 7369 6f6e 3a0a  atch.extension:.
-0001af70: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-0001af80: 7874 2e75 726c 203d 3d20 7365 6c66 2e64  xt.url == self.d
-0001af90: 6566 6175 6c74 5f71 7561 6e74 6974 795f  efault_quantity_
-0001afa0: 7572 6c3a 0a20 2020 2020 2020 2020 2020  url:.           
-0001afb0: 2020 2020 2072 6574 7572 6e20 6578 742e       return ext.
-0001afc0: 7661 6c75 6551 7561 6e74 6974 790a 0a63  valueQuantity..c
-0001afd0: 6c61 7373 2050 7261 6374 6974 696f 6e65  lass Practitione
-0001afe0: 7246 4849 5228 4261 7365 4648 4952 293a  rFHIR(BaseFHIR):
-0001aff0: 0a20 2020 2070 7261 6374 6974 696f 6e65  .    practitione
-0001b000: 725f 656e 6470 6f69 6e74 203d 2022 7b62  r_endpoint = "{b
-0001b010: 6173 655f 7572 6c7d 2f50 7261 6374 6974  ase_url}/Practit
-0001b020: 696f 6e65 7222 0a20 2020 2070 7261 6374  ioner".    pract
-0001b030: 6974 696f 6e65 725f 6279 5f69 645f 656e  itioner_by_id_en
-0001b040: 6470 6f69 6e74 203d 2070 7261 6374 6974  dpoint = practit
-0001b050: 696f 6e65 725f 656e 6470 6f69 6e74 202b  ioner_endpoint +
-0001b060: 2022 2f7b 6964 7d22 0a0a 2020 2020 6465   "/{id}"..    de
-0001b070: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0001b080: 2062 6173 655f 7572 6c3d 4e6f 6e65 2c20   base_url=None, 
-0001b090: 6261 7365 5f75 7269 3d4e 6f6e 652c 2072  base_uri=None, r
-0001b0a0: 6573 6f75 7263 653d 4e6f 6e65 2c20 746f  esource=None, to
-0001b0b0: 6b65 6e5f 6865 6164 6572 3d4e 6f6e 652c  ken_header=None,
-0001b0c0: 2076 616c 6964 6174 655f 6365 7274 733d   validate_certs=
-0001b0d0: 5472 7565 2920 2d3e 204e 6f6e 653a 0a20  True) -> None:. 
-0001b0e0: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-0001b0f0: 5f69 6e69 745f 5f28 6261 7365 5f75 726c  _init__(base_url
-0001b100: 3d62 6173 655f 7572 6c2c 2062 6173 655f  =base_url, base_
-0001b110: 7572 693d 6261 7365 5f75 7269 2c20 746f  uri=base_uri, to
-0001b120: 6b65 6e5f 6865 6164 6572 3d74 6f6b 656e  ken_header=token
-0001b130: 5f68 6561 6465 7229 0a20 2020 2020 2020  _header).       
-0001b140: 2073 656c 662e 7661 6c69 6461 7465 5f63   self.validate_c
-0001b150: 6572 7473 203d 2076 616c 6964 6174 655f  erts = validate_
-0001b160: 6365 7274 730a 2020 2020 2020 2020 6966  certs.        if
-0001b170: 2072 6573 6f75 7263 6520 6973 206e 6f74   resource is not
-0001b180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001b190: 2020 2073 656c 662e 6668 6972 5f72 6573     self.fhir_res
-0001b1a0: 6f75 7263 6520 3d20 5072 6163 7469 7469  ource = Practiti
-0001b1b0: 6f6e 6572 286a 736f 6e64 6963 743d 7265  oner(jsondict=re
-0001b1c0: 736f 7572 6365 290a 2020 2020 2020 2020  source).        
-0001b1d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001b1e0: 2020 7365 6c66 2e66 6869 725f 7265 736f    self.fhir_reso
-0001b1f0: 7572 6365 203d 2050 7261 6374 6974 696f  urce = Practitio
-0001b200: 6e65 7228 290a 0a20 2020 2064 6566 2067  ner()..    def g
-0001b210: 6574 4668 6972 5265 736f 7572 6365 2873  etFhirResource(s
-0001b220: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
-0001b230: 7475 726e 2073 656c 662e 6668 6972 5f72  turn self.fhir_r
-0001b240: 6573 6f75 7263 652e 6173 5f6a 736f 6e28  esource.as_json(
-0001b250: 290a 0a20 2020 2064 6566 2073 6561 7263  )..    def searc
-0001b260: 6828 7365 6c66 2c20 6964 656e 7469 6669  h(self, identifi
-0001b270: 6572 3d4e 6f6e 652c 2072 6f6c 653d 4e6f  er=None, role=No
-0001b280: 6e65 2c20 6661 6d69 6c79 3d4e 6f6e 652c  ne, family=None,
-0001b290: 2067 6976 656e 3d4e 6f6e 6529 3a0a 2020   given=None):.  
-0001b2a0: 2020 2020 2020 7061 7261 6d73 203d 207b        params = {
-0001b2b0: 7d0a 2020 2020 2020 2020 6966 2069 6465  }.        if ide
-0001b2c0: 6e74 6966 6965 7220 6973 206e 6f74 204e  ntifier is not N
-0001b2d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001b2e0: 2070 6172 616d 735b 2269 6465 6e74 6966   params["identif
-0001b2f0: 6965 7222 5d20 3d20 6964 656e 7469 6669  ier"] = identifi
-0001b300: 6572 0a20 2020 2020 2020 2069 6620 726f  er.        if ro
-0001b310: 6c65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  le is not None:.
-0001b320: 2020 2020 2020 2020 2020 2020 7061 7261              para
-0001b330: 6d73 5b22 726f 6c65 225d 203d 2072 6f6c  ms["role"] = rol
-0001b340: 650a 2020 2020 2020 2020 6966 2066 616d  e.        if fam
-0001b350: 696c 7920 6973 206e 6f74 204e 6f6e 653a  ily is not None:
-0001b360: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-0001b370: 616d 735b 2266 616d 696c 7922 5d20 3d20  ams["family"] = 
-0001b380: 6661 6d69 6c79 0a20 2020 2020 2020 2069  family.        i
-0001b390: 6620 6769 7665 6e20 6973 206e 6f74 204e  f given is not N
-0001b3a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001b3b0: 2070 6172 616d 735b 2267 6976 656e 225d   params["given"]
-0001b3c0: 203d 2067 6976 656e 0a0a 2020 2020 2020   = given..      
-0001b3d0: 2020 7072 6163 7469 7469 6f6e 6572 5f72    practitioner_r
-0001b3e0: 6573 706f 6e73 6520 3d20 7265 7175 6573  esponse = reques
-0001b3f0: 7473 2e67 6574 280a 2020 2020 2020 2020  ts.get(.        
-0001b400: 2020 2020 7572 6c3d 7365 6c66 2e70 7261      url=self.pra
-0001b410: 6374 6974 696f 6e65 725f 656e 6470 6f69  ctitioner_endpoi
-0001b420: 6e74 2e66 6f72 6d61 7428 6261 7365 5f75  nt.format(base_u
-0001b430: 726c 3d73 656c 662e 6765 745f 6668 6972  rl=self.get_fhir
-0001b440: 5f75 726c 2829 292c 0a20 2020 2020 2020  _url()),.       
-0001b450: 2020 2020 2068 6561 6465 7273 3d73 656c       headers=sel
-0001b460: 662e 6865 6164 6572 732c 0a20 2020 2020  f.headers,.     
-0001b470: 2020 2020 2020 2070 6172 616d 733d 7061         params=pa
-0001b480: 7261 6d73 2c0a 2020 2020 2020 2020 2020  rams,.          
-0001b490: 2020 7665 7269 6679 3d73 656c 662e 7661    verify=self.va
-0001b4a0: 6c69 6461 7465 5f63 6572 7473 0a20 2020  lidate_certs.   
-0001b4b0: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
-0001b4c0: 6620 7072 6163 7469 7469 6f6e 6572 5f72  f practitioner_r
-0001b4d0: 6573 706f 6e73 652e 7374 6174 7573 5f63  esponse.status_c
-0001b4e0: 6f64 6520 3d3d 2032 3030 3a0a 2020 2020  ode == 200:.    
-0001b4f0: 2020 2020 2020 2020 636f 6e74 656e 745f          content_
-0001b500: 6469 6374 203d 206a 736f 6e2e 6c6f 6164  dict = json.load
-0001b510: 7328 7072 6163 7469 7469 6f6e 6572 5f72  s(practitioner_r
-0001b520: 6573 706f 6e73 652e 636f 6e74 656e 7429  esponse.content)
-0001b530: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001b540: 7572 6e20 4275 6e64 6c65 4648 4952 2872  urn BundleFHIR(r
-0001b550: 6573 6f75 7263 653d 636f 6e74 656e 745f  esource=content_
-0001b560: 6469 6374 290a 2020 2020 2020 2020 7265  dict).        re
-0001b570: 7475 726e 204e 6f6e 650a 0a20 2020 2064  turn None..    d
-0001b580: 6566 2067 6574 5f66 616d 696c 7928 7365  ef get_family(se
-0001b590: 6c66 2c20 7072 6163 7469 7469 6f6e 6572  lf, practitioner
-0001b5a0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0001b5b0: 6966 2070 7261 6374 6974 696f 6e65 7220  if practitioner 
-0001b5c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0001b5d0: 2020 2020 2070 7261 6374 6974 696f 6e65       practitione
-0001b5e0: 7220 3d20 7365 6c66 2e66 6869 725f 7265  r = self.fhir_re
-0001b5f0: 736f 7572 6365 0a0a 2020 2020 2020 2020  source..        
-0001b600: 6966 2074 7970 6528 7072 6163 7469 7469  if type(practiti
-0001b610: 6f6e 6572 2e6e 616d 6529 2069 7320 4875  oner.name) is Hu
-0001b620: 6d61 6e4e 616d 653a 0a20 2020 2020 2020  manName:.       
-0001b630: 2020 2020 2072 6574 7572 6e20 7072 6163       return prac
-0001b640: 7469 7469 6f6e 6572 2e6e 616d 652e 6661  titioner.name.fa
-0001b650: 6d69 6c79 0a20 2020 2020 2020 2072 6574  mily.        ret
-0001b660: 7572 6e20 4e6f 6e65 0a0a 0a20 2020 2064  urn None...    d
-0001b670: 6566 2067 6574 5f67 6976 656e 2873 656c  ef get_given(sel
-0001b680: 662c 2070 7261 6374 6974 696f 6e65 723d  f, practitioner=
-0001b690: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
-0001b6a0: 6620 7072 6163 7469 7469 6f6e 6572 2069  f practitioner i
-0001b6b0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0001b6c0: 2020 2020 7072 6163 7469 7469 6f6e 6572      practitioner
-0001b6d0: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
-0001b6e0: 6f75 7263 650a 0a20 2020 2020 2020 2069  ource..        i
-0001b6f0: 6620 7479 7065 2870 7261 6374 6974 696f  f type(practitio
-0001b700: 6e65 722e 6e61 6d65 2920 6973 2048 756d  ner.name) is Hum
-0001b710: 616e 4e61 6d65 3a0a 2020 2020 2020 2020  anName:.        
-0001b720: 2020 2020 7265 7475 726e 2070 7261 6374      return pract
-0001b730: 6974 696f 6e65 722e 6e61 6d65 2e67 6976  itioner.name.giv
-0001b740: 656e 0a20 2020 2020 2020 2072 6574 7572  en.        retur
-0001b750: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
-0001b760: 6765 745f 6964 2873 656c 662c 2070 7261  get_id(self, pra
-0001b770: 6374 6974 696f 6e65 723d 4e6f 6e65 293a  ctitioner=None):
-0001b780: 0a20 2020 2020 2020 2069 6620 7072 6163  .        if prac
-0001b790: 7469 7469 6f6e 6572 2069 7320 4e6f 6e65  titioner is None
-0001b7a0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-0001b7b0: 6163 7469 7469 6f6e 6572 203d 2073 656c  actitioner = sel
-0001b7c0: 662e 6668 6972 5f72 6573 6f75 7263 650a  f.fhir_resource.
-0001b7d0: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-0001b7e0: 7261 6374 6974 696f 6e65 722e 6964 0a0a  ractitioner.id..
-0001b7f0: 2020 2020 6465 6620 6765 745f 6279 5f69      def get_by_i
-0001b800: 6428 7365 6c66 2c20 7072 6163 7469 7469  d(self, practiti
-0001b810: 6f6e 6572 5f69 643d 4e6f 6e65 293a 0a20  oner_id=None):. 
-0001b820: 2020 2020 2020 2069 6620 7072 6163 7469         if practi
-0001b830: 7469 6f6e 6572 5f69 6420 6973 204e 6f6e  tioner_id is Non
-0001b840: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-0001b850: 7261 6374 6974 696f 6e65 725f 6964 203d  ractitioner_id =
-0001b860: 2073 656c 662e 6765 745f 6964 2829 0a20   self.get_id(). 
-0001b870: 2020 2020 2020 2069 6620 7072 6163 7469         if practi
-0001b880: 7469 6f6e 6572 5f69 6420 6973 206e 6f74  tioner_id is not
-0001b890: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001b8a0: 2020 2072 6573 706f 6e73 6520 3d20 7265     response = re
-0001b8b0: 7175 6573 7473 2e67 6574 280a 2020 2020  quests.get(.    
-0001b8c0: 2020 2020 2020 2020 2020 2020 7572 6c3d              url=
-0001b8d0: 7365 6c66 2e70 7261 6374 6974 696f 6e65  self.practitione
-0001b8e0: 725f 6279 5f69 645f 656e 6470 6f69 6e74  r_by_id_endpoint
-0001b8f0: 2e66 6f72 6d61 7428 6261 7365 5f75 726c  .format(base_url
-0001b900: 3d73 656c 662e 6765 745f 6668 6972 5f75  =self.get_fhir_u
-0001b910: 726c 2829 2c20 6964 3d70 7261 6374 6974  rl(), id=practit
-0001b920: 696f 6e65 725f 6964 292c 0a20 2020 2020  ioner_id),.     
-0001b930: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-0001b940: 7273 3d73 656c 662e 6865 6164 6572 732c  rs=self.headers,
-0001b950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b960: 2076 6572 6966 793d 7365 6c66 2e76 616c   verify=self.val
-0001b970: 6964 6174 655f 6365 7274 730a 2020 2020  idate_certs.    
-0001b980: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0001b990: 2020 2020 2020 6966 2072 6573 706f 6e73        if respons
-0001b9a0: 652e 7374 6174 7573 5f63 6f64 6520 3d3d  e.status_code ==
-0001b9b0: 2032 3030 3a0a 2020 2020 2020 2020 2020   200:.          
-0001b9c0: 2020 2020 2020 6a73 6f6e 6469 6374 203d        jsondict =
-0001b9d0: 206a 736f 6e2e 6c6f 6164 7328 7265 7370   json.loads(resp
-0001b9e0: 6f6e 7365 2e63 6f6e 7465 6e74 290a 2020  onse.content).  
-0001b9f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001ba00: 736f 7572 6365 203d 2073 656c 662e 6765  source = self.ge
-0001ba10: 745f 6d6f 6465 6c5f 6672 6f6d 5f6a 736f  t_model_from_jso
-0001ba20: 6e28 6a73 6f6e 6469 6374 3d6a 736f 6e64  n(jsondict=jsond
-0001ba30: 6963 7429 0a20 2020 2020 2020 2020 2020  ict).           
-0001ba40: 2020 2020 2069 6620 7479 7065 2872 6573       if type(res
-0001ba50: 6f75 7263 6529 2069 7320 4c6f 6361 7469  ource) is Locati
-0001ba60: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-0001ba70: 2020 2020 2020 2020 7365 6c66 2e66 6869          self.fhi
-0001ba80: 725f 7265 736f 7572 6365 203d 2072 6573  r_resource = res
-0001ba90: 6f75 7263 650a 2020 2020 2020 2020 2020  ource.          
-0001baa0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-0001bab0: 650a 0a20 2020 2020 2020 2072 6574 7572  e..        retur
-0001bac0: 6e20 4e6f 6e65 0a0a 636c 6173 7320 5661  n None..class Va
-0001bad0: 6c75 6553 6574 4648 4952 2842 6173 6546  lueSetFHIR(BaseF
-0001bae0: 4849 5229 3a0a 2020 2020 7661 6c75 6573  HIR):.    values
-0001baf0: 6574 5f65 6e64 706f 696e 7420 3d20 227b  et_endpoint = "{
-0001bb00: 6261 7365 5f75 726c 7d2f 5661 6c75 6553  base_url}/ValueS
-0001bb10: 6574 220a 2020 2020 7661 6c75 6573 6574  et".    valueset
-0001bb20: 5f76 6f63 6162 756c 6172 795f 646f 6d61  _vocabulary_doma
-0001bb30: 696e 5f65 6e64 706f 696e 7420 3d20 7661  in_endpoint = va
-0001bb40: 6c75 6573 6574 5f65 6e64 706f 696e 7420  lueset_endpoint 
-0001bb50: 2b20 222f 7b64 6f6d 6169 6e7d 220a 0a20  + "/{domain}".. 
-0001bb60: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0001bb70: 7365 6c66 2c20 6261 7365 5f75 726c 3d4e  self, base_url=N
-0001bb80: 6f6e 652c 2062 6173 655f 7572 693d 4e6f  one, base_uri=No
-0001bb90: 6e65 2c20 7265 736f 7572 6365 3d4e 6f6e  ne, resource=Non
-0001bba0: 652c 2074 6f6b 656e 5f68 6561 6465 723d  e, token_header=
-0001bbb0: 4e6f 6e65 2c20 7661 6c69 6461 7465 5f63  None, validate_c
-0001bbc0: 6572 7473 3d54 7275 6529 202d 3e20 4e6f  erts=True) -> No
-0001bbd0: 6e65 3a0a 2020 2020 2020 2020 7375 7065  ne:.        supe
-0001bbe0: 7228 292e 5f5f 696e 6974 5f5f 2862 6173  r().__init__(bas
-0001bbf0: 655f 7572 6c3d 6261 7365 5f75 726c 2c20  e_url=base_url, 
-0001bc00: 6261 7365 5f75 7269 3d62 6173 655f 7572  base_uri=base_ur
-0001bc10: 692c 2074 6f6b 656e 5f68 6561 6465 723d  i, token_header=
-0001bc20: 746f 6b65 6e5f 6865 6164 6572 290a 2020  token_header).  
-0001bc30: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0001bc40: 6174 655f 6365 7274 7320 3d20 7661 6c69  ate_certs = vali
-0001bc50: 6461 7465 5f63 6572 7473 0a20 2020 2020  date_certs.     
-0001bc60: 2020 2069 6620 7265 736f 7572 6365 2069     if resource i
-0001bc70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0001bc80: 2020 2020 2020 2020 7365 6c66 2e66 6869          self.fhi
-0001bc90: 725f 7265 736f 7572 6365 203d 2056 616c  r_resource = Val
-0001bca0: 7565 5365 7428 6a73 6f6e 6469 6374 3d72  ueSet(jsondict=r
-0001bcb0: 6573 6f75 7263 6529 0a20 2020 2020 2020  esource).       
-0001bcc0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001bcd0: 2020 2073 656c 662e 6668 6972 5f72 6573     self.fhir_res
-0001bce0: 6f75 7263 6520 3d20 5661 6c75 6553 6574  ource = ValueSet
-0001bcf0: 2829 0a0a 2020 2020 6465 6620 6765 7446  ()..    def getF
-0001bd00: 6869 7252 6573 6f75 7263 6528 7365 6c66  hirResource(self
-0001bd10: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0001bd20: 6e20 7365 6c66 2e66 6869 725f 7265 736f  n self.fhir_reso
-0001bd30: 7572 6365 2e61 735f 6a73 6f6e 2829 0a0a  urce.as_json()..
-0001bd40: 2020 2020 6465 6620 6765 745f 6765 6e64      def get_gend
-0001bd50: 6572 2873 656c 6629 3a0a 2020 2020 2020  er(self):.      
-0001bd60: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
-0001bd70: 745f 7661 6c75 6573 6574 5f62 795f 646f  t_valueset_by_do
-0001bd80: 6d61 696e 2864 6f6d 6169 6e3d 2267 656e  main(domain="gen
-0001bd90: 6465 7222 290a 0a20 2020 2064 6566 2067  der")..    def g
-0001bda0: 6574 5f61 646d 696e 6973 7472 6174 696f  et_administratio
-0001bdb0: 6e73 6974 6528 7365 6c66 293a 0a20 2020  nsite(self):.   
-0001bdc0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001bdd0: 2e67 6574 5f76 616c 7565 7365 745f 6279  .get_valueset_by
-0001bde0: 5f64 6f6d 6169 6e28 646f 6d61 696e 3d22  _domain(domain="
-0001bdf0: 6164 6d69 6e69 7374 7261 7469 6f6e 7369  administrationsi
-0001be00: 7465 2229 0a0a 2020 2020 6465 6620 6765  te")..    def ge
-0001be10: 745f 7661 6c75 6573 6574 5f62 795f 646f  t_valueset_by_do
-0001be20: 6d61 696e 2873 656c 662c 2064 6f6d 6169  main(self, domai
-0001be30: 6e29 3a0a 2020 2020 2020 2020 7661 6c75  n):.        valu
-0001be40: 6573 6574 5f72 6573 706f 6e73 6520 3d20  eset_response = 
-0001be50: 7265 7175 6573 7473 2e67 6574 280a 2020  requests.get(.  
-0001be60: 2020 2020 2020 2020 2020 7572 6c3d 7365            url=se
-0001be70: 6c66 2e76 616c 7565 7365 745f 766f 6361  lf.valueset_voca
-0001be80: 6275 6c61 7279 5f64 6f6d 6169 6e5f 656e  bulary_domain_en
-0001be90: 6470 6f69 6e74 2e66 6f72 6d61 7428 6261  dpoint.format(ba
-0001bea0: 7365 5f75 726c 3d73 656c 662e 6765 745f  se_url=self.get_
-0001beb0: 6668 6972 5f75 726c 2829 2c20 646f 6d61  fhir_url(), doma
-0001bec0: 696e 3d64 6f6d 6169 6e29 2c0a 2020 2020  in=domain),.    
-0001bed0: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
-0001bee0: 7365 6c66 2e68 6561 6465 7273 2c0a 2020  self.headers,.  
-0001bef0: 2020 2020 2020 2020 2020 7665 7269 6679            verify
-0001bf00: 3d73 656c 662e 7661 6c69 6461 7465 5f63  =self.validate_c
-0001bf10: 6572 7473 0a20 2020 2020 2020 2029 0a20  erts.        ). 
-0001bf20: 2020 2020 2020 2069 6620 7661 6c75 6573         if values
-0001bf30: 6574 5f72 6573 706f 6e73 652e 7374 6174  et_response.stat
-0001bf40: 7573 5f63 6f64 6520 3d3d 2032 3030 3a0a  us_code == 200:.
-0001bf50: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0001bf60: 656e 745f 6469 6374 203d 206a 736f 6e2e  ent_dict = json.
-0001bf70: 6c6f 6164 7328 7661 6c75 6573 6574 5f72  loads(valueset_r
-0001bf80: 6573 706f 6e73 652e 636f 6e74 656e 7429  esponse.content)
-0001bf90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001bfa0: 662e 6668 6972 5f72 6573 6f75 7263 6520  f.fhir_resource 
-0001bfb0: 3d20 5661 6c75 6553 6574 286a 736f 6e64  = ValueSet(jsond
-0001bfc0: 6963 743d 636f 6e74 656e 745f 6469 6374  ict=content_dict
-0001bfd0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0001bfe0: 6e20 7661 6c75 6573 6574 5f72 6573 706f  n valueset_respo
-0001bff0: 6e73 650a 0a20 2020 2064 6566 2073 6561  nse..    def sea
-0001c000: 7263 685f 636f 6465 5f73 7973 7465 6d5f  rch_code_system_
-0001c010: 636f 6e63 6570 7428 7365 6c66 2c20 636f  concept(self, co
-0001c020: 6465 3d4e 6f6e 652c 2064 6973 706c 6179  de=None, display
-0001c030: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0001c040: 636f 6465 5f73 7973 7465 6d5f 636f 6e63  code_system_conc
-0001c050: 6570 7420 3d20 4e6f 6e65 0a20 2020 2020  ept = None.     
-0001c060: 2020 2069 6620 2873 656c 662e 6668 6972     if (self.fhir
-0001c070: 5f72 6573 6f75 7263 6520 6973 206e 6f74  _resource is not
+00017840: 742e 7661 6c75 6550 6572 696f 6420 3d20  t.valuePeriod = 
+00017850: 7065 7269 6f64 0a0a 2020 2020 6465 6620  period..    def 
+00017860: 6765 745f 7068 6f6e 6573 2873 656c 662c  get_phones(self,
+00017870: 206f 7267 616e 697a 6174 696f 6e3d 4e6f   organization=No
+00017880: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
+00017890: 6f72 6761 6e69 7a61 7469 6f6e 2069 7320  organization is 
+000178a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000178b0: 2020 6f72 6761 6e69 7a61 7469 6f6e 203d    organization =
+000178c0: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
+000178d0: 7263 650a 2020 2020 2020 2020 7068 6f6e  rce.        phon
+000178e0: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
+000178f0: 6966 206f 7267 616e 697a 6174 696f 6e2e  if organization.
+00017900: 7465 6c65 636f 6d20 6973 204e 6f6e 653a  telecom is None:
+00017910: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00017920: 7572 6e20 7068 6f6e 6573 0a20 2020 2020  urn phones.     
+00017930: 2020 2066 6f72 2074 656c 6563 6f6d 2069     for telecom i
+00017940: 6e20 6f72 6761 6e69 7a61 7469 6f6e 2e74  n organization.t
+00017950: 656c 6563 6f6d 3a0a 2020 2020 2020 2020  elecom:.        
+00017960: 2020 2020 6966 2074 656c 6563 6f6d 2e73      if telecom.s
+00017970: 7973 7465 6d20 3d3d 2022 7068 6f6e 6522  ystem == "phone"
+00017980: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017990: 2020 7068 6f6e 6520 3d20 7b7d 0a20 2020    phone = {}.   
+000179a0: 2020 2020 2020 2020 2020 2020 2070 686f               pho
+000179b0: 6e65 5b22 7661 6c75 6522 5d20 3d20 7465  ne["value"] = te
+000179c0: 6c65 636f 6d2e 7661 6c75 650a 2020 2020  lecom.value.    
+000179d0: 2020 2020 2020 2020 2020 2020 7068 6f6e              phon
+000179e0: 655b 2275 7365 225d 203d 2074 656c 6563  e["use"] = telec
+000179f0: 6f6d 2e75 7365 0a20 2020 2020 2020 2020  om.use.         
+00017a00: 2020 2020 2020 2070 686f 6e65 732e 6170         phones.ap
+00017a10: 7065 6e64 2870 686f 6e65 290a 2020 2020  pend(phone).    
+00017a20: 2020 2020 7265 7475 726e 2070 686f 6e65      return phone
+00017a30: 730a 0a20 2020 2064 6566 2067 6574 5f63  s..    def get_c
+00017a40: 6f6e 7461 6374 735f 7068 6f6e 6573 2873  ontacts_phones(s
+00017a50: 656c 662c 206f 7267 616e 697a 6174 696f  elf, organizatio
+00017a60: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
+00017a70: 2069 6620 6f72 6761 6e69 7a61 7469 6f6e   if organization
+00017a80: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00017a90: 2020 2020 2020 6f72 6761 6e69 7a61 7469        organizati
+00017aa0: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
+00017ab0: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
+00017ac0: 7068 6f6e 6573 203d 205b 5d0a 2020 2020  phones = [].    
+00017ad0: 2020 2020 6966 206f 7267 616e 697a 6174      if organizat
+00017ae0: 696f 6e2e 636f 6e74 6163 7420 6973 204e  ion.contact is N
+00017af0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00017b00: 2072 6574 7572 6e20 7068 6f6e 6573 0a20   return phones. 
+00017b10: 2020 2020 2020 2066 6f72 2063 6f6e 7461         for conta
+00017b20: 6374 2069 6e20 6f72 6761 6e69 7a61 7469  ct in organizati
+00017b30: 6f6e 2e63 6f6e 7461 6374 3a0a 2020 2020  on.contact:.    
+00017b40: 2020 2020 2020 2020 6966 2063 6f6e 7461          if conta
+00017b50: 6374 2e74 656c 6563 6f6d 2069 7320 6e6f  ct.telecom is no
+00017b60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00017b70: 2020 2020 2020 2020 666f 7220 7465 6c65          for tele
+00017b80: 636f 6d20 696e 2063 6f6e 7461 6374 2e74  com in contact.t
+00017b90: 656c 6563 6f6d 3a0a 2020 2020 2020 2020  elecom:.        
+00017ba0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00017bb0: 656c 6563 6f6d 2e73 7973 7465 6d20 3d3d  elecom.system ==
+00017bc0: 2022 7068 6f6e 6522 3a0a 2020 2020 2020   "phone":.      
+00017bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017be0: 2020 7068 6f6e 6520 3d20 7b7d 0a20 2020    phone = {}.   
+00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c00: 2020 2020 2070 686f 6e65 5b22 7661 6c75       phone["valu
+00017c10: 6522 5d20 3d20 7465 6c65 636f 6d2e 7661  e"] = telecom.va
+00017c20: 6c75 650a 2020 2020 2020 2020 2020 2020  lue.            
+00017c30: 2020 2020 2020 2020 2020 2020 7068 6f6e              phon
+00017c40: 655b 2275 7365 225d 203d 2074 656c 6563  e["use"] = telec
+00017c50: 6f6d 2e75 7365 0a20 2020 2020 2020 2020  om.use.         
+00017c60: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00017c70: 686f 6e65 732e 6170 7065 6e64 2870 686f  hones.append(pho
+00017c80: 6e65 290a 2020 2020 2020 2020 7265 7475  ne).        retu
+00017c90: 726e 2070 686f 6e65 730a 0a20 2020 2064  rn phones..    d
+00017ca0: 6566 2069 735f 6163 7469 7665 2873 656c  ef is_active(sel
+00017cb0: 662c 206f 7267 616e 697a 6174 696f 6e3d  f, organization=
+00017cc0: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
+00017cd0: 6620 6f72 6761 6e69 7a61 7469 6f6e 2069  f organization i
+00017ce0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00017cf0: 2020 2020 6f72 6761 6e69 7a61 7469 6f6e      organization
+00017d00: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
+00017d10: 6f75 7263 650a 2020 2020 2020 2020 7265  ource.        re
+00017d20: 7475 726e 206f 7267 616e 697a 6174 696f  turn organizatio
+00017d30: 6e2e 6163 7469 7665 0a0a 2020 2020 6465  n.active..    de
+00017d40: 6620 7365 6172 6368 2873 656c 662c 206e  f search(self, n
+00017d50: 616d 653d 4e6f 6e65 2c20 6964 656e 7469  ame=None, identi
+00017d60: 6669 6572 3d4e 6f6e 6529 3a0a 2020 2020  fier=None):.    
+00017d70: 2020 2020 7061 7261 6d73 203d 207b 7d0a      params = {}.
+00017d80: 2020 2020 2020 2020 6966 206e 616d 6520          if name 
+00017d90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00017da0: 2020 2020 2020 2020 2070 6172 616d 735b           params[
+00017db0: 276e 616d 6527 5d20 3d20 6e61 6d65 0a20  'name'] = name. 
+00017dc0: 2020 2020 2020 2069 6620 6964 656e 7469         if identi
+00017dd0: 6669 6572 2069 7320 6e6f 7420 4e6f 6e65  fier is not None
+00017de0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+00017df0: 7261 6d73 5b27 6964 656e 7469 6669 6572  rams['identifier
+00017e00: 275d 203d 2069 6465 6e74 6966 6965 720a  '] = identifier.
+00017e10: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00017e20: 203d 2072 6571 7565 7374 732e 6765 7428   = requests.get(
+00017e30: 7572 6c3d 7365 6c66 2e6f 7267 616e 697a  url=self.organiz
+00017e40: 6174 696f 6e5f 656e 6470 6f69 6e74 2e66  ation_endpoint.f
+00017e50: 6f72 6d61 7428 6261 7365 5f75 726c 3d73  ormat(base_url=s
+00017e60: 656c 662e 6765 745f 6668 6972 5f75 726c  elf.get_fhir_url
+00017e70: 2829 292c 2070 6172 616d 733d 7061 7261  ()), params=para
+00017e80: 6d73 2c20 6865 6164 6572 733d 7365 6c66  ms, headers=self
+00017e90: 2e68 6561 6465 7273 2c20 7665 7269 6679  .headers, verify
+00017ea0: 3d73 656c 662e 7661 6c69 6461 7465 5f63  =self.validate_c
+00017eb0: 6572 7473 290a 2020 2020 2020 2020 636f  erts).        co
+00017ec0: 6e74 656e 7420 3d20 6a73 6f6e 2e6c 6f61  ntent = json.loa
+00017ed0: 6473 2872 6573 706f 6e73 652e 636f 6e74  ds(response.cont
+00017ee0: 656e 742e 6465 636f 6465 2829 290a 2020  ent.decode()).  
+00017ef0: 2020 2020 200a 2020 2020 2020 2020 7265       .        re
+00017f00: 7475 726e 2073 656c 662e 6765 745f 7669  turn self.get_vi
+00017f10: 7369 746f 725f 6672 6f6d 5f6a 736f 6e28  sitor_from_json(
+00017f20: 6a73 6f6e 6469 6374 3d63 6f6e 7465 6e74  jsondict=content
+00017f30: 290a 0a20 2020 2064 6566 2067 6574 5f62  )..    def get_b
+00017f40: 795f 6964 2873 656c 662c 206f 7267 5f69  y_id(self, org_i
+00017f50: 643d 4e6f 6e65 293a 0a20 2020 2020 2020  d=None):.       
+00017f60: 2069 6620 6f72 675f 6964 2069 7320 4e6f   if org_id is No
+00017f70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00017f80: 6f72 675f 6964 203d 2073 656c 662e 6765  org_id = self.ge
+00017f90: 745f 6964 2829 0a20 2020 2020 2020 2069  t_id().        i
+00017fa0: 6620 6f72 675f 6964 2069 7320 6e6f 7420  f org_id is not 
+00017fb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00017fc0: 2020 7572 6c20 3d20 7365 6c66 2e6f 7267    url = self.org
+00017fd0: 616e 697a 6174 696f 6e5f 6279 5f69 645f  anization_by_id_
+00017fe0: 656e 6470 6f69 6e74 2e66 6f72 6d61 7428  endpoint.format(
+00017ff0: 6261 7365 5f75 726c 3d73 656c 662e 6765  base_url=self.ge
+00018000: 745f 6668 6972 5f75 726c 2829 2c20 6964  t_fhir_url(), id
+00018010: 3d6f 7267 5f69 6429 0a20 2020 2020 2020  =org_id).       
+00018020: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00018030: 2e67 6574 5f62 795f 7572 6c28 7572 6c3d  .get_by_url(url=
+00018040: 7572 6c29 0a20 2020 2020 2020 200a 2020  url).        .  
+00018050: 2020 6465 6620 6765 745f 6279 5f72 6566    def get_by_ref
+00018060: 6572 656e 6365 2873 656c 662c 2072 6566  erence(self, ref
+00018070: 6572 656e 6365 3d4e 6f6e 6529 3a0a 2020  erence=None):.  
+00018080: 2020 2020 2020 6966 2072 6566 6572 656e        if referen
+00018090: 6365 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ce is not None:.
+000180a0: 2020 2020 2020 2020 2020 2020 7572 6c20              url 
+000180b0: 3d20 227b 307d 2f7b 317d 222e 666f 726d  = "{0}/{1}".form
+000180c0: 6174 2873 656c 662e 6765 745f 6668 6972  at(self.get_fhir
+000180d0: 5f75 726c 2829 2c20 7265 6665 7265 6e63  _url(), referenc
+000180e0: 652e 7265 6665 7265 6e63 6529 0a20 2020  e.reference).   
+000180f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00018100: 7365 6c66 2e67 6574 5f62 795f 7572 6c28  self.get_by_url(
+00018110: 7572 6c3d 7572 6c29 0a0a 2020 2020 6465  url=url)..    de
+00018120: 6620 6765 745f 6279 5f75 726c 2873 656c  f get_by_url(sel
+00018130: 662c 2075 726c 293a 2020 2020 2020 2020  f, url):        
+00018140: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00018150: 6520 3d20 7265 7175 6573 7473 2e67 6574  e = requests.get
+00018160: 280a 2020 2020 2020 2020 2020 2020 7572  (.            ur
+00018170: 6c3d 7572 6c2c 0a20 2020 2020 2020 2020  l=url,.         
+00018180: 2020 2068 6561 6465 7273 3d73 656c 662e     headers=self.
+00018190: 6865 6164 6572 732c 0a20 2020 2020 2020  headers,.       
+000181a0: 2020 2020 2076 6572 6966 793d 7365 6c66       verify=self
+000181b0: 2e76 616c 6964 6174 655f 6365 7274 730a  .validate_certs.
+000181c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000181d0: 2020 6966 2072 6573 706f 6e73 652e 7374    if response.st
+000181e0: 6174 7573 5f63 6f64 6520 3d3d 2032 3030  atus_code == 200
+000181f0: 3a0a 2020 2020 2020 2020 2020 2020 6a73  :.            js
+00018200: 6f6e 6469 6374 203d 206a 736f 6e2e 6c6f  ondict = json.lo
+00018210: 6164 7328 7265 7370 6f6e 7365 2e63 6f6e  ads(response.con
+00018220: 7465 6e74 290a 2020 2020 2020 2020 2020  tent).          
+00018230: 2020 7265 736f 7572 6365 203d 2073 656c    resource = sel
+00018240: 662e 6765 745f 6d6f 6465 6c5f 6672 6f6d  f.get_model_from
+00018250: 5f6a 736f 6e28 6a73 6f6e 6469 6374 3d6a  _json(jsondict=j
+00018260: 736f 6e64 6963 7429 0a20 2020 2020 2020  sondict).       
+00018270: 2020 2020 2069 6620 7479 7065 2872 6573       if type(res
+00018280: 6f75 7263 6529 2069 7320 4f72 6761 6e69  ource) is Organi
+00018290: 7a61 7469 6f6e 3a0a 2020 2020 2020 2020  zation:.        
+000182a0: 2020 2020 2020 2020 7365 6c66 2e66 6869          self.fhi
+000182b0: 725f 7265 736f 7572 6365 203d 2072 6573  r_resource = res
+000182c0: 6f75 7263 650a 2020 2020 2020 2020 7265  ource.        re
+000182d0: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+000182e0: 2020 2064 6566 2063 7265 6174 6528 7365     def create(se
+000182f0: 6c66 293a 0a20 2020 2020 2020 2072 6573  lf):.        res
+00018300: 203d 2073 656c 662e 6765 7446 6869 7252   = self.getFhirR
+00018310: 6573 6f75 7263 6528 290a 2020 2020 2020  esource().      
+00018320: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
+00018330: 7565 7374 732e 706f 7374 280a 2020 2020  uests.post(.    
+00018340: 2020 2020 2020 2020 7572 6c3d 7365 6c66          url=self
+00018350: 2e6f 7267 616e 697a 6174 696f 6e5f 656e  .organization_en
+00018360: 6470 6f69 6e74 2e66 6f72 6d61 7428 6261  dpoint.format(ba
+00018370: 7365 5f75 726c 3d73 656c 662e 6765 745f  se_url=self.get_
+00018380: 6668 6972 5f75 726c 2829 292c 0a20 2020  fhir_url()),.   
+00018390: 2020 2020 2020 2020 2064 6174 613d 6a73           data=js
+000183a0: 6f6e 2e64 756d 7073 2872 6573 292c 0a20  on.dumps(res),. 
+000183b0: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+000183c0: 7273 3d73 656c 662e 6865 6164 6572 732c  rs=self.headers,
+000183d0: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
+000183e0: 6966 793d 7365 6c66 2e76 616c 6964 6174  ify=self.validat
+000183f0: 655f 6365 7274 7329 0a20 2020 2020 2020  e_certs).       
+00018400: 2069 6620 7265 7370 6f6e 7365 2e73 7461   if response.sta
+00018410: 7475 735f 636f 6465 203d 3d20 3230 313a  tus_code == 201:
+00018420: 0a20 2020 2020 2020 2020 2020 206a 736f  .            jso
+00018430: 6e64 6963 7420 3d20 6a73 6f6e 2e6c 6f61  ndict = json.loa
+00018440: 6473 2872 6573 706f 6e73 652e 636f 6e74  ds(response.cont
+00018450: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
+00018460: 2072 6573 6f75 7263 6520 3d20 7365 6c66   resource = self
+00018470: 2e67 6574 5f6d 6f64 656c 5f66 726f 6d5f  .get_model_from_
+00018480: 6a73 6f6e 286a 736f 6e64 6963 743d 6a73  json(jsondict=js
+00018490: 6f6e 6469 6374 290a 2020 2020 2020 2020  ondict).        
+000184a0: 2020 2020 6966 2074 7970 6528 7265 736f      if type(reso
+000184b0: 7572 6365 2920 6973 204f 7267 616e 697a  urce) is Organiz
+000184c0: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
+000184d0: 2020 2020 2020 2073 656c 662e 6668 6972         self.fhir
+000184e0: 5f72 6573 6f75 7263 6520 3d20 7265 736f  _resource = reso
+000184f0: 7572 6365 0a20 2020 2020 2020 2072 6574  urce.        ret
+00018500: 7572 6e20 7265 7370 6f6e 7365 0a0a 2020  urn response..  
+00018510: 2020 6465 6620 7570 6461 7465 2873 656c    def update(sel
+00018520: 6629 3a0a 2020 2020 2020 2020 7265 7320  f):.        res 
+00018530: 3d20 7365 6c66 2e67 6574 4668 6972 5265  = self.getFhirRe
+00018540: 736f 7572 6365 2829 0a20 2020 2020 2020  source().       
+00018550: 2072 6573 706f 6e73 6520 3d20 7265 7175   response = requ
+00018560: 6573 7473 2e70 7574 280a 2020 2020 2020  ests.put(.      
+00018570: 2020 2020 2020 7572 6c3d 7365 6c66 2e6f        url=self.o
+00018580: 7267 616e 697a 6174 696f 6e5f 6279 5f69  rganization_by_i
+00018590: 645f 656e 6470 6f69 6e74 2e66 6f72 6d61  d_endpoint.forma
+000185a0: 7428 6261 7365 5f75 726c 3d73 656c 662e  t(base_url=self.
+000185b0: 6765 745f 6668 6972 5f75 726c 2829 2c20  get_fhir_url(), 
+000185c0: 6964 3d73 656c 662e 6765 745f 6964 2829  id=self.get_id()
+000185d0: 292c 0a20 2020 2020 2020 2020 2020 2064  ),.            d
+000185e0: 6174 613d 6a73 6f6e 2e64 756d 7073 2872  ata=json.dumps(r
+000185f0: 6573 292c 0a20 2020 2020 2020 2020 2020  es),.           
+00018600: 2068 6561 6465 7273 3d73 656c 662e 6865   headers=self.he
+00018610: 6164 6572 732c 0a20 2020 2020 2020 2020  aders,.         
+00018620: 2020 2076 6572 6966 793d 7365 6c66 2e76     verify=self.v
+00018630: 616c 6964 6174 655f 6365 7274 7329 0a20  alidate_certs). 
+00018640: 2020 2020 2020 2069 6620 7265 7370 6f6e         if respon
+00018650: 7365 2e73 7461 7475 735f 636f 6465 203d  se.status_code =
+00018660: 3d20 3230 303a 0a20 2020 2020 2020 2020  = 200:.         
+00018670: 2020 206a 736f 6e64 6963 7420 3d20 6a73     jsondict = js
+00018680: 6f6e 2e6c 6f61 6473 2872 6573 706f 6e73  on.loads(respons
+00018690: 652e 636f 6e74 656e 7429 0a20 2020 2020  e.content).     
+000186a0: 2020 2020 2020 2072 6573 6f75 7263 6520         resource 
+000186b0: 3d20 7365 6c66 2e67 6574 5f6d 6f64 656c  = self.get_model
+000186c0: 5f66 726f 6d5f 6a73 6f6e 286a 736f 6e64  _from_json(jsond
+000186d0: 6963 743d 6a73 6f6e 6469 6374 290a 2020  ict=jsondict).  
+000186e0: 2020 2020 2020 2020 2020 6966 2074 7970            if typ
+000186f0: 6528 7265 736f 7572 6365 2920 6973 204f  e(resource) is O
+00018700: 7267 616e 697a 6174 696f 6e3a 0a20 2020  rganization:.   
+00018710: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018720: 662e 6668 6972 5f72 6573 6f75 7263 6520  f.fhir_resource 
+00018730: 3d20 7265 736f 7572 6365 0a20 2020 2020  = resource.     
+00018740: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
+00018750: 7365 0a0a 2020 2020 6465 6620 6465 6c65  se..    def dele
+00018760: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00018770: 2020 7265 7320 3d20 7365 6c66 2e67 6574    res = self.get
+00018780: 4668 6972 5265 736f 7572 6365 2829 0a20  FhirResource(). 
+00018790: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+000187a0: 3d20 7265 7175 6573 7473 2e64 656c 6574  = requests.delet
+000187b0: 6528 0a20 2020 2020 2020 2020 2020 2075  e(.            u
+000187c0: 726c 3d73 656c 662e 6f72 6761 6e69 7a61  rl=self.organiza
+000187d0: 7469 6f6e 5f62 795f 6964 5f65 6e64 706f  tion_by_id_endpo
+000187e0: 696e 742e 666f 726d 6174 2862 6173 655f  int.format(base_
+000187f0: 7572 6c3d 7365 6c66 2e67 6574 5f66 6869  url=self.get_fhi
+00018800: 725f 7572 6c28 292c 2069 643d 7365 6c66  r_url(), id=self
+00018810: 2e67 6574 5f69 6428 2929 2c0a 2020 2020  .get_id()),.    
+00018820: 2020 2020 2020 2020 6461 7461 3d6a 736f          data=jso
+00018830: 6e2e 6475 6d70 7328 7265 7329 2c0a 2020  n.dumps(res),.  
+00018840: 2020 2020 2020 2020 2020 6865 6164 6572            header
+00018850: 733d 7365 6c66 2e68 6561 6465 7273 2c0a  s=self.headers,.
+00018860: 2020 2020 2020 2020 2020 2020 7665 7269              veri
+00018870: 6679 3d73 656c 662e 7661 6c69 6461 7465  fy=self.validate
+00018880: 5f63 6572 7473 290a 2020 2020 2020 2020  _certs).        
+00018890: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
+000188a0: 0a63 6c61 7373 204c 6f63 6174 696f 6e46  .class LocationF
+000188b0: 4849 5228 4261 7365 4648 4952 293a 0a20  HIR(BaseFHIR):. 
+000188c0: 2020 206c 6f63 6174 696f 6e5f 656e 6470     location_endp
+000188d0: 6f69 6e74 203d 2022 7b62 6173 655f 7572  oint = "{base_ur
+000188e0: 6c7d 2f4c 6f63 6174 696f 6e22 0a20 2020  l}/Location".   
+000188f0: 206c 6f63 6174 696f 6e5f 6279 5f69 645f   location_by_id_
+00018900: 656e 6470 6f69 6e74 203d 206c 6f63 6174  endpoint = locat
+00018910: 696f 6e5f 656e 6470 6f69 6e74 202b 2022  ion_endpoint + "
+00018920: 2f7b 6964 7d22 0a20 2020 2072 7273 735f  /{id}".    rrss_
+00018930: 7379 7374 656d 203d 2027 6874 7470 733a  system = 'https:
+00018940: 2f2f 7072 6f2e 636f 6e73 756c 7461 7469  //pro.consultati
+00018950: 6f6e 2e72 7273 732e 7274 7373 2e71 632e  on.rrss.rtss.qc.
+00018960: 6361 270a 2020 2020 7272 7373 5f6d 6f74  ca'.    rrss_mot
+00018970: 5f63 6c65 5f65 7874 656e 7369 6f6e 5f75  _cle_extension_u
+00018980: 726c 203d 2027 6874 7470 3a2f 2f77 7777  rl = 'http://www
+00018990: 2e73 616e 7465 7075 626c 6971 7565 2e72  .santepublique.r
+000189a0: 7473 732e 7163 2e63 612f 7369 706d 692f  tss.qc.ca/sipmi/
+000189b0: 7272 7373 2f31 2e30 2e30 2f65 7874 656e  rrss/1.0.0/exten
+000189c0: 7369 6f6e 732f 236d 6f74 7363 6c65 7327  sions/#motscles'
+000189d0: 0a20 2020 2070 6572 696f 645f 7572 6c20  .    period_url 
+000189e0: 3d20 2268 7474 703a 2f2f 7777 772e 7361  = "http://www.sa
+000189f0: 6e74 6570 7562 6c69 7175 652e 7274 7373  ntepublique.rtss
+00018a00: 2e71 632e 6361 2f73 6970 6d69 2f72 7273  .qc.ca/sipmi/rrs
+00018a10: 732f 312e 302e 302f 6578 7465 6e73 696f  s/1.0.0/extensio
+00018a20: 6e73 2f70 6572 696f 6422 0a0a 2020 2020  ns/period"..    
+00018a30: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00018a40: 662c 2062 6173 655f 7572 6c3d 4e6f 6e65  f, base_url=None
+00018a50: 2c20 6261 7365 5f75 7269 3d4e 6f6e 652c  , base_uri=None,
+00018a60: 2072 6573 6f75 7263 653d 4e6f 6e65 2c20   resource=None, 
+00018a70: 746f 6b65 6e5f 6865 6164 6572 3d4e 6f6e  token_header=Non
+00018a80: 652c 2076 616c 6964 6174 655f 6365 7274  e, validate_cert
+00018a90: 733d 5472 7565 2920 2d3e 204e 6f6e 653a  s=True) -> None:
+00018aa0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00018ab0: 2e5f 5f69 6e69 745f 5f28 6261 7365 5f75  .__init__(base_u
+00018ac0: 726c 3d62 6173 655f 7572 6c2c 2062 6173  rl=base_url, bas
+00018ad0: 655f 7572 693d 6261 7365 5f75 7269 2c20  e_uri=base_uri, 
+00018ae0: 746f 6b65 6e5f 6865 6164 6572 3d74 6f6b  token_header=tok
+00018af0: 656e 5f68 6561 6465 7229 0a20 2020 2020  en_header).     
+00018b00: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+00018b10: 5f63 6572 7473 203d 2076 616c 6964 6174  _certs = validat
+00018b20: 655f 6365 7274 730a 2020 2020 2020 2020  e_certs.        
+00018b30: 6966 2072 6573 6f75 7263 6520 6973 206e  if resource is n
+00018b40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00018b50: 2020 2020 2073 656c 662e 6668 6972 5f72       self.fhir_r
+00018b60: 6573 6f75 7263 6520 3d20 4c6f 6361 7469  esource = Locati
+00018b70: 6f6e 286a 736f 6e64 6963 743d 7265 736f  on(jsondict=reso
+00018b80: 7572 6365 290a 2020 2020 2020 2020 656c  urce).        el
+00018b90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00018ba0: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
+00018bb0: 6365 203d 204c 6f63 6174 696f 6e28 290a  ce = Location().
+00018bc0: 0a20 2020 2064 6566 2067 6574 4668 6972  .    def getFhir
+00018bd0: 5265 736f 7572 6365 2873 656c 6629 3a0a  Resource(self):.
+00018be0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00018bf0: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+00018c00: 652e 6173 5f6a 736f 6e28 290a 0a20 2020  e.as_json()..   
+00018c10: 2064 6566 2068 6176 655f 6d6f 745f 636c   def have_mot_cl
+00018c20: 6528 7365 6c66 2c20 6c6f 6361 7469 6f6e  e(self, location
+00018c30: 3d4e 6f6e 652c 206d 6f74 5f63 6c65 3d4e  =None, mot_cle=N
+00018c40: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
+00018c50: 206c 6f63 6174 696f 6e20 6973 204e 6f6e   location is Non
+00018c60: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
+00018c70: 6f63 6174 696f 6e20 3d20 7365 6c66 2e66  ocation = self.f
+00018c80: 6869 725f 7265 736f 7572 6365 0a20 2020  hir_resource.   
+00018c90: 2020 2020 2069 6620 6d6f 745f 636c 6520       if mot_cle 
+00018ca0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00018cb0: 6c6f 6361 7469 6f6e 2e65 7874 656e 7369  location.extensi
+00018cc0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
+00018cd0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00018ce0: 6578 7465 6e73 696f 6e20 696e 206c 6f63  extension in loc
+00018cf0: 6174 696f 6e2e 6578 7465 6e73 696f 6e3a  ation.extension:
+00018d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018d10: 2069 6620 6578 7465 6e73 696f 6e2e 7572   if extension.ur
+00018d20: 6c20 3d3d 2073 656c 662e 7272 7373 5f6d  l == self.rrss_m
+00018d30: 6f74 5f63 6c65 5f65 7874 656e 7369 6f6e  ot_cle_extension
+00018d40: 5f75 726c 2061 6e64 2065 7874 656e 7369  _url and extensi
+00018d50: 6f6e 2e76 616c 7565 5374 7269 6e67 203d  on.valueString =
+00018d60: 3d20 6d6f 745f 636c 653a 0a20 2020 2020  = mot_cle:.     
+00018d70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00018d80: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00018d90: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00018da0: 0a20 2020 2064 6566 2073 6574 5f6e 616d  .    def set_nam
+00018db0: 6528 7365 6c66 2c20 6c6f 6361 7469 6f6e  e(self, location
+00018dc0: 3d4e 6f6e 652c 206e 616d 653d 4e6f 6e65  =None, name=None
+00018dd0: 293a 0a20 2020 2020 2020 2069 6620 6c6f  ):.        if lo
+00018de0: 6361 7469 6f6e 2069 7320 4e6f 6e65 3a0a  cation is None:.
+00018df0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+00018e00: 7469 6f6e 203d 2073 656c 662e 6668 6972  tion = self.fhir
+00018e10: 5f72 6573 6f75 7263 650a 0a20 2020 2020  _resource..     
+00018e20: 2020 206c 6f63 6174 696f 6e2e 6e61 6d65     location.name
+00018e30: 203d 206e 616d 650a 0a20 2020 2064 6566   = name..    def
+00018e40: 2067 6574 5f6e 616d 6528 7365 6c66 2c20   get_name(self, 
+00018e50: 6c6f 6361 7469 6f6e 3d4e 6f6e 6529 3a0a  location=None):.
+00018e60: 2020 2020 2020 2020 6966 206c 6f63 6174          if locat
+00018e70: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
+00018e80: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
+00018e90: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
+00018ea0: 736f 7572 6365 0a20 2020 2020 2020 2072  source.        r
+00018eb0: 6574 7572 6e20 6c6f 6361 7469 6f6e 2e6e  eturn location.n
+00018ec0: 616d 650a 0a20 2020 2064 6566 2067 6574  ame..    def get
+00018ed0: 5f69 6428 7365 6c66 2c20 6c6f 6361 7469  _id(self, locati
+00018ee0: 6f6e 3d4e 6f6e 6529 3a0a 2020 2020 2020  on=None):.      
+00018ef0: 2020 6966 206c 6f63 6174 696f 6e20 6973    if location is
+00018f00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00018f10: 2020 206c 6f63 6174 696f 6e20 3d20 7365     location = se
+00018f20: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+00018f30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00018f40: 6c6f 6361 7469 6f6e 2e69 640a 0a20 2020  location.id..   
+00018f50: 2064 6566 2067 6574 5f69 645f 7272 7373   def get_id_rrss
+00018f60: 2873 656c 662c 206c 6f63 6174 696f 6e3d  (self, location=
+00018f70: 4e6f 6e65 293a 0a20 2020 2020 2020 2069  None):.        i
+00018f80: 6620 6c6f 6361 7469 6f6e 2069 7320 4e6f  f location is No
+00018f90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00018fa0: 6c6f 6361 7469 6f6e 203d 2073 656c 662e  location = self.
+00018fb0: 6668 6972 5f72 6573 6f75 7263 650a 2020  fhir_resource.  
+00018fc0: 2020 2020 2020 6966 206c 6f63 6174 696f        if locatio
+00018fd0: 6e2e 6964 656e 7469 6669 6572 2069 7320  n.identifier is 
+00018fe0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00018ff0: 2020 2020 2020 666f 7220 6964 656e 7469        for identi
+00019000: 6669 6572 2069 6e20 6c6f 6361 7469 6f6e  fier in location
+00019010: 2e69 6465 6e74 6966 6965 723a 0a20 2020  .identifier:.   
+00019020: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00019030: 6964 656e 7469 6669 6572 2e73 7973 7465  identifier.syste
+00019040: 6d20 3d3d 2073 656c 662e 7272 7373 5f73  m == self.rrss_s
+00019050: 7973 7465 6d3a 0a20 2020 2020 2020 2020  ystem:.         
+00019060: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00019070: 6e20 6964 656e 7469 6669 6572 2e76 616c  n identifier.val
+00019080: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00019090: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
+000190a0: 6765 745f 7068 6f6e 6573 2873 656c 662c  get_phones(self,
+000190b0: 206c 6f63 6174 696f 6e3d 4e6f 6e65 293a   location=None):
+000190c0: 0a20 2020 2020 2020 2069 6620 6c6f 6361  .        if loca
+000190d0: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
+000190e0: 2020 2020 2020 2020 2020 6c6f 6361 7469            locati
+000190f0: 6f6e 203d 2073 656c 662e 6668 6972 5f72  on = self.fhir_r
+00019100: 6573 6f75 7263 650a 2020 2020 2020 2020  esource.        
+00019110: 7068 6f6e 6573 203d 205b 5d0a 2020 2020  phones = [].    
+00019120: 2020 2020 6966 206c 6f63 6174 696f 6e2e      if location.
+00019130: 7465 6c65 636f 6d20 6973 204e 6f6e 653a  telecom is None:
+00019140: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00019150: 7572 6e20 7068 6f6e 6573 0a20 2020 2020  urn phones.     
+00019160: 2020 2066 6f72 2074 656c 6563 6f6d 2069     for telecom i
+00019170: 6e20 6c6f 6361 7469 6f6e 2e74 656c 6563  n location.telec
+00019180: 6f6d 3a0a 2020 2020 2020 2020 2020 2020  om:.            
+00019190: 6966 2074 656c 6563 6f6d 2e73 7973 7465  if telecom.syste
+000191a0: 6d20 3d3d 2022 7068 6f6e 6522 3a0a 2020  m == "phone":.  
+000191b0: 2020 2020 2020 2020 2020 2020 2020 7068                ph
+000191c0: 6f6e 6520 3d20 7b7d 0a20 2020 2020 2020  one = {}.       
+000191d0: 2020 2020 2020 2020 2070 686f 6e65 5b22           phone["
+000191e0: 7661 6c75 6522 5d20 3d20 7465 6c65 636f  value"] = teleco
+000191f0: 6d2e 7661 6c75 650a 2020 2020 2020 2020  m.value.        
+00019200: 2020 2020 2020 2020 7068 6f6e 655b 2275          phone["u
+00019210: 7365 225d 203d 2074 656c 6563 6f6d 2e75  se"] = telecom.u
+00019220: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+00019230: 2020 2070 686f 6e65 732e 6170 7065 6e64     phones.append
+00019240: 2870 686f 6e65 290a 2020 2020 2020 2020  (phone).        
+00019250: 7265 7475 726e 2070 686f 6e65 730a 0a20  return phones.. 
+00019260: 2020 2064 6566 2067 6574 5f65 6666 6563     def get_effec
+00019270: 7469 7665 5f66 726f 6d28 7365 6c66 2c20  tive_from(self, 
+00019280: 6c6f 6361 7469 6f6e 3d4e 6f6e 6529 3a0a  location=None):.
+00019290: 2020 2020 2020 2020 6966 206c 6f63 6174          if locat
+000192a0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
+000192b0: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
+000192c0: 6e20 3d20 7365 6c66 2e66 6869 725f 7265  n = self.fhir_re
+000192d0: 736f 7572 6365 0a20 2020 2020 2020 2070  source.        p
+000192e0: 6572 696f 645f 6578 7420 3d20 7365 6c66  eriod_ext = self
+000192f0: 2e67 6574 5f70 6572 696f 645f 6578 7428  .get_period_ext(
+00019300: 6c6f 6361 7469 6f6e 3d6c 6f63 6174 696f  location=locatio
+00019310: 6e29 0a20 2020 2020 2020 2069 6620 7065  n).        if pe
+00019320: 7269 6f64 5f65 7874 2069 7320 6e6f 7420  riod_ext is not 
+00019330: 4e6f 6e65 2061 6e64 2070 6572 696f 645f  None and period_
+00019340: 6578 742e 7661 6c75 6550 6572 696f 6420  ext.valuePeriod 
+00019350: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00019360: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00019370: 7572 6e20 7065 7269 6f64 5f65 7874 2e76  urn period_ext.v
+00019380: 616c 7565 5065 7269 6f64 2e73 7461 7274  aluePeriod.start
+00019390: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000193a0: 4e6f 6e65 0a0a 2020 2020 6465 6620 6765  None..    def ge
+000193b0: 745f 6566 6665 6374 6976 655f 746f 2873  t_effective_to(s
+000193c0: 656c 662c 206c 6f63 6174 696f 6e3d 4e6f  elf, location=No
+000193d0: 6e65 293a 0a20 2020 2020 2020 2069 6620  ne):.        if 
+000193e0: 6c6f 6361 7469 6f6e 2069 7320 4e6f 6e65  location is None
+000193f0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00019400: 6361 7469 6f6e 203d 2073 656c 662e 6668  cation = self.fh
+00019410: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
+00019420: 2020 2020 7065 7269 6f64 5f65 7874 203d      period_ext =
+00019430: 2073 656c 662e 6765 745f 7065 7269 6f64   self.get_period
+00019440: 5f65 7874 286c 6f63 6174 696f 6e3d 6c6f  _ext(location=lo
+00019450: 6361 7469 6f6e 290a 2020 2020 2020 2020  cation).        
+00019460: 6966 2070 6572 696f 645f 6578 7420 6973  if period_ext is
+00019470: 206e 6f74 204e 6f6e 6520 616e 6420 7065   not None and pe
+00019480: 7269 6f64 5f65 7874 2e76 616c 7565 5065  riod_ext.valuePe
+00019490: 7269 6f64 2069 7320 6e6f 7420 4e6f 6e65  riod is not None
+000194a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000194b0: 2020 7265 7475 726e 2070 6572 696f 645f    return period_
+000194c0: 6578 742e 7661 6c75 6550 6572 696f 642e  ext.valuePeriod.
+000194d0: 656e 640a 2020 2020 2020 2020 7265 7475  end.        retu
+000194e0: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
+000194f0: 2073 6574 5f65 6666 6563 7469 7665 5f66   set_effective_f
+00019500: 726f 6d28 7365 6c66 2c20 6c6f 6361 7469  rom(self, locati
+00019510: 6f6e 3d4e 6f6e 652c 2065 6666 6563 7469  on=None, effecti
+00019520: 7665 5f66 726f 6d3d 4e6f 6e65 293a 0a20  ve_from=None):. 
+00019530: 2020 2020 2020 2069 6620 6c6f 6361 7469         if locati
+00019540: 6f6e 2069 7320 4e6f 6e65 3a0a 2020 2020  on is None:.    
+00019550: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
+00019560: 203d 2073 656c 662e 6668 6972 5f72 6573   = self.fhir_res
+00019570: 6f75 7263 650a 2020 2020 2020 2020 6668  ource.        fh
+00019580: 6972 5f65 6666 6563 7469 7665 5f66 726f  ir_effective_fro
+00019590: 6d20 3d20 4e6f 6e65 0a20 2020 2020 2020  m = None.       
+000195a0: 2069 6620 7479 7065 2865 6666 6563 7469   if type(effecti
+000195b0: 7665 5f66 726f 6d29 2069 7320 7374 723a  ve_from) is str:
+000195c0: 0a20 2020 2020 2020 2020 2020 2066 6869  .            fhi
+000195d0: 725f 6566 6665 6374 6976 655f 6672 6f6d  r_effective_from
+000195e0: 203d 2046 4849 5244 6174 6528 6a73 6f6e   = FHIRDate(json
+000195f0: 7661 6c3d 6566 6665 6374 6976 655f 6672  val=effective_fr
+00019600: 6f6d 290a 2020 2020 2020 2020 656c 6966  om).        elif
+00019610: 2074 7970 6528 6566 6665 6374 6976 655f   type(effective_
+00019620: 6672 6f6d 2920 6973 2046 4849 5244 6174  from) is FHIRDat
+00019630: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+00019640: 6869 725f 6566 6665 6374 6976 655f 6672  hir_effective_fr
+00019650: 6f6d 203d 2065 6666 6563 7469 7665 5f66  om = effective_f
+00019660: 726f 6d0a 2020 2020 2020 2020 7065 7269  rom.        peri
+00019670: 6f64 5f65 7874 203d 2073 656c 662e 6765  od_ext = self.ge
+00019680: 745f 7065 7269 6f64 5f65 7874 2829 0a20  t_period_ext(). 
+00019690: 2020 2020 2020 2069 6620 7065 7269 6f64         if period
+000196a0: 5f65 7874 2069 7320 4e6f 6e65 206f 7220  _ext is None or 
+000196b0: 7065 7269 6f64 5f65 7874 2e76 616c 7565  period_ext.value
+000196c0: 5065 7269 6f64 2069 7320 4e6f 6e65 3a0a  Period is None:.
+000196d0: 2020 2020 2020 2020 2020 2020 7065 7269              peri
+000196e0: 6f64 203d 2050 6572 696f 6428 290a 2020  od = Period().  
+000196f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00019700: 2020 2020 2020 2020 7065 7269 6f64 203d          period =
+00019710: 2070 6572 696f 645f 6578 742e 7661 6c75   period_ext.valu
+00019720: 6550 6572 696f 640a 2020 2020 2020 2020  ePeriod.        
+00019730: 7065 7269 6f64 2e73 7461 7274 203d 2066  period.start = f
+00019740: 6869 725f 6566 6665 6374 6976 655f 6672  hir_effective_fr
+00019750: 6f6d 0a20 2020 2020 2020 2073 656c 662e  om.        self.
+00019760: 7365 745f 7065 7269 6f64 5f65 7874 286c  set_period_ext(l
+00019770: 6f63 6174 696f 6e3d 6c6f 6361 7469 6f6e  ocation=location
+00019780: 2c20 7065 7269 6f64 3d70 6572 696f 6429  , period=period)
+00019790: 0a0a 2020 2020 6465 6620 7365 745f 6566  ..    def set_ef
+000197a0: 6665 6374 6976 655f 746f 2873 656c 662c  fective_to(self,
+000197b0: 206c 6f63 6174 696f 6e3d 4e6f 6e65 2c20   location=None, 
+000197c0: 6566 6665 6374 6976 655f 746f 3d4e 6f6e  effective_to=Non
+000197d0: 6529 3a0a 2020 2020 2020 2020 6966 206c  e):.        if l
+000197e0: 6f63 6174 696f 6e20 6973 204e 6f6e 653a  ocation is None:
+000197f0: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
+00019800: 6174 696f 6e20 3d20 7365 6c66 2e66 6869  ation = self.fhi
+00019810: 725f 7265 736f 7572 6365 0a20 2020 2020  r_resource.     
+00019820: 2020 2066 6869 725f 6566 6665 6374 6976     fhir_effectiv
+00019830: 655f 746f 203d 204e 6f6e 650a 2020 2020  e_to = None.    
+00019840: 2020 2020 6966 2074 7970 6528 6566 6665      if type(effe
+00019850: 6374 6976 655f 746f 2920 6973 2073 7472  ctive_to) is str
+00019860: 3a0a 2020 2020 2020 2020 2020 2020 6668  :.            fh
+00019870: 6972 5f65 6666 6563 7469 7665 5f74 6f20  ir_effective_to 
+00019880: 3d20 4648 4952 4461 7465 286a 736f 6e76  = FHIRDate(jsonv
+00019890: 616c 3d65 6666 6563 7469 7665 5f74 6f29  al=effective_to)
+000198a0: 0a20 2020 2020 2020 2065 6c69 6620 7479  .        elif ty
+000198b0: 7065 2865 6666 6563 7469 7665 5f74 6f29  pe(effective_to)
+000198c0: 2069 7320 4648 4952 4461 7465 3a0a 2020   is FHIRDate:.  
+000198d0: 2020 2020 2020 2020 2020 6668 6972 5f65            fhir_e
+000198e0: 6666 6563 7469 7665 5f74 6f20 3d20 6566  ffective_to = ef
+000198f0: 6665 6374 6976 655f 746f 0a20 2020 2020  fective_to.     
+00019900: 2020 2070 6572 696f 645f 6578 7420 3d20     period_ext = 
+00019910: 7365 6c66 2e67 6574 5f70 6572 696f 645f  self.get_period_
+00019920: 6578 7428 290a 2020 2020 2020 2020 6966  ext().        if
+00019930: 2070 6572 696f 645f 6578 7420 6973 204e   period_ext is N
+00019940: 6f6e 6520 6f72 2070 6572 696f 645f 6578  one or period_ex
+00019950: 742e 7661 6c75 6550 6572 696f 6420 6973  t.valuePeriod is
+00019960: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00019970: 2020 2070 6572 696f 6420 3d20 5065 7269     period = Peri
+00019980: 6f64 2829 0a20 2020 2020 2020 2065 6c73  od().        els
+00019990: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+000199a0: 6572 696f 6420 3d20 7065 7269 6f64 5f65  eriod = period_e
+000199b0: 7874 2e76 616c 7565 5065 7269 6f64 0a20  xt.valuePeriod. 
+000199c0: 2020 2020 2020 2070 6572 696f 642e 656e         period.en
+000199d0: 6420 3d20 6668 6972 5f65 6666 6563 7469  d = fhir_effecti
+000199e0: 7665 5f74 6f0a 2020 2020 2020 2020 7365  ve_to.        se
+000199f0: 6c66 2e73 6574 5f70 6572 696f 645f 6578  lf.set_period_ex
+00019a00: 7428 6c6f 6361 7469 6f6e 3d6c 6f63 6174  t(location=locat
+00019a10: 696f 6e2c 2070 6572 696f 643d 7065 7269  ion, period=peri
+00019a20: 6f64 290a 0a20 2020 2064 6566 2067 6574  od)..    def get
+00019a30: 5f70 6572 696f 645f 6578 7428 7365 6c66  _period_ext(self
+00019a40: 2c20 6c6f 6361 7469 6f6e 3d4e 6f6e 6529  , location=None)
+00019a50: 3a0a 2020 2020 2020 2020 6966 206c 6f63  :.        if loc
+00019a60: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
+00019a70: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+00019a80: 696f 6e20 3d20 7365 6c66 2e66 6869 725f  ion = self.fhir_
+00019a90: 7265 736f 7572 6365 0a20 2020 2020 2020  resource.       
+00019aa0: 2069 6620 6c6f 6361 7469 6f6e 2e65 7874   if location.ext
+00019ab0: 656e 7369 6f6e 2069 7320 6e6f 7420 4e6f  ension is not No
+00019ac0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00019ad0: 666f 7220 6578 7420 696e 206c 6f63 6174  for ext in locat
+00019ae0: 696f 6e2e 6578 7465 6e73 696f 6e3a 0a20  ion.extension:. 
+00019af0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00019b00: 6620 6578 742e 7572 6c20 3d3d 2073 656c  f ext.url == sel
+00019b10: 662e 7065 7269 6f64 5f75 726c 3a0a 2020  f.period_url:.  
+00019b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b30: 2020 7265 7475 726e 2065 7874 0a20 2020    return ext.   
+00019b40: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00019b50: 0a0a 2020 2020 6465 6620 7365 745f 7065  ..    def set_pe
+00019b60: 7269 6f64 5f65 7874 2873 656c 662c 206c  riod_ext(self, l
+00019b70: 6f63 6174 696f 6e3d 4e6f 6e65 2c20 7065  ocation=None, pe
+00019b80: 7269 6f64 3d4e 6f6e 6529 3a0a 2020 2020  riod=None):.    
+00019b90: 2020 2020 6966 206c 6f63 6174 696f 6e20      if location 
+00019ba0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00019bb0: 2020 2020 206c 6f63 6174 696f 6e20 3d20       location = 
+00019bc0: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
+00019bd0: 6365 0a20 2020 2020 2020 2069 6620 6c6f  ce.        if lo
+00019be0: 6361 7469 6f6e 2e65 7874 656e 7369 6f6e  cation.extension
+00019bf0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00019c00: 2020 2020 2020 6c6f 6361 7469 6f6e 2e65        location.e
+00019c10: 7874 656e 7369 6f6e 203d 205b 5d0a 2020  xtension = [].  
+00019c20: 2020 2020 2020 7065 7269 6f64 5f65 7874        period_ext
+00019c30: 203d 2073 656c 662e 6765 745f 7065 7269   = self.get_peri
+00019c40: 6f64 5f65 7874 286c 6f63 6174 696f 6e3d  od_ext(location=
+00019c50: 6c6f 6361 7469 6f6e 290a 2020 2020 2020  location).      
+00019c60: 2020 6966 2070 6572 696f 645f 6578 7420    if period_ext 
+00019c70: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00019c80: 2020 2020 2070 6572 696f 645f 6578 7420       period_ext 
+00019c90: 3d20 4578 7465 6e73 696f 6e28 290a 2020  = Extension().  
+00019ca0: 2020 2020 2020 2020 2020 7065 7269 6f64            period
+00019cb0: 5f65 7874 2e75 726c 203d 2073 656c 662e  _ext.url = self.
+00019cc0: 7065 7269 6f64 5f75 726c 0a20 2020 2020  period_url.     
+00019cd0: 2020 2020 2020 206c 6f63 6174 696f 6e2e         location.
+00019ce0: 6578 7465 6e73 696f 6e2e 6170 7065 6e64  extension.append
+00019cf0: 2870 6572 696f 645f 6578 7429 0a20 2020  (period_ext).   
+00019d00: 2020 2020 2070 6572 696f 645f 6578 742e       period_ext.
+00019d10: 7661 6c75 6550 6572 696f 6420 3d20 7065  valuePeriod = pe
+00019d20: 7269 6f64 0a0a 2020 2020 6465 6620 6973  riod..    def is
+00019d30: 5f61 6374 6976 6528 7365 6c66 2c20 6c6f  _active(self, lo
+00019d40: 6361 7469 6f6e 3d4e 6f6e 6529 3a0a 2020  cation=None):.  
+00019d50: 2020 2020 2020 6966 206c 6f63 6174 696f        if locatio
+00019d60: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+00019d70: 2020 2020 2020 206c 6f63 6174 696f 6e20         location 
+00019d80: 3d20 7365 6c66 2e66 6869 725f 7265 736f  = self.fhir_reso
+00019d90: 7572 6365 0a20 2020 2020 2020 2069 6620  urce.        if 
+00019da0: 6c6f 6361 7469 6f6e 2e73 7461 7475 7320  location.status 
+00019db0: 3d3d 2022 6163 7469 7665 223a 0a20 2020  == "active":.   
+00019dc0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00019dd0: 5472 7565 0a20 2020 2020 2020 2072 6574  True.        ret
+00019de0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00019df0: 2020 0a20 2020 2064 6566 2073 6561 7263    .    def searc
+00019e00: 6828 7365 6c66 2c20 6e61 6d65 3d4e 6f6e  h(self, name=Non
+00019e10: 652c 2061 6464 7265 7373 5f63 6974 793d  e, address_city=
+00019e20: 4e6f 6e65 2c20 6964 656e 7469 6669 6572  None, identifier
+00019e30: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00019e40: 7061 7261 6d73 203d 207b 7d0a 2020 2020  params = {}.    
+00019e50: 2020 2020 6966 206e 616d 6520 6973 206e      if name is n
+00019e60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00019e70: 2020 2020 2070 6172 616d 735b 276e 616d       params['nam
+00019e80: 6527 5d20 3d20 6e61 6d65 0a20 2020 2020  e'] = name.     
+00019e90: 2020 2069 6620 6964 656e 7469 6669 6572     if identifier
+00019ea0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00019eb0: 2020 2020 2020 2020 2020 7061 7261 6d73            params
+00019ec0: 5b27 6964 656e 7469 6669 6572 275d 203d  ['identifier'] =
+00019ed0: 2069 6465 6e74 6966 6965 720a 2020 2020   identifier.    
+00019ee0: 2020 2020 6966 2061 6464 7265 7373 5f63      if address_c
+00019ef0: 6974 7920 6973 206e 6f74 204e 6f6e 653a  ity is not None:
+00019f00: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+00019f10: 616d 735b 2761 6464 7265 7373 2d63 6974  ams['address-cit
+00019f20: 7927 5d20 3d20 6164 6472 6573 735f 6369  y'] = address_ci
+00019f30: 7479 0a20 2020 2020 2020 2072 6573 706f  ty.        respo
+00019f40: 6e73 6520 3d20 7265 7175 6573 7473 2e67  nse = requests.g
+00019f50: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+00019f60: 7572 6c3d 7365 6c66 2e6c 6f63 6174 696f  url=self.locatio
+00019f70: 6e5f 656e 6470 6f69 6e74 2e66 6f72 6d61  n_endpoint.forma
+00019f80: 7428 6261 7365 5f75 726c 3d73 656c 662e  t(base_url=self.
+00019f90: 6765 745f 6668 6972 5f75 726c 2829 292c  get_fhir_url()),
+00019fa0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+00019fb0: 616d 733d 7061 7261 6d73 2c0a 2020 2020  ams=params,.    
+00019fc0: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
+00019fd0: 7365 6c66 2e68 6561 6465 7273 2c0a 2020  self.headers,.  
+00019fe0: 2020 2020 2020 2020 2020 7665 7269 6679            verify
+00019ff0: 3d73 656c 662e 7661 6c69 6461 7465 5f63  =self.validate_c
+0001a000: 6572 7473 290a 2020 2020 2020 2020 636f  erts).        co
+0001a010: 6e74 656e 7420 3d20 6a73 6f6e 2e6c 6f61  ntent = json.loa
+0001a020: 6473 2872 6573 706f 6e73 652e 636f 6e74  ds(response.cont
+0001a030: 656e 742e 6465 636f 6465 2829 290a 2020  ent.decode()).  
+0001a040: 2020 0a20 2020 2020 2020 2072 6574 7572    .        retur
+0001a050: 6e20 7365 6c66 2e67 6574 5f76 6973 6974  n self.get_visit
+0001a060: 6f72 5f66 726f 6d5f 6a73 6f6e 286a 736f  or_from_json(jso
+0001a070: 6e64 6963 743d 636f 6e74 656e 7429 0a0a  ndict=content)..
+0001a080: 2020 2020 6465 6620 6765 745f 6279 5f69      def get_by_i
+0001a090: 6428 7365 6c66 2c20 6c6f 6361 7469 6f6e  d(self, location
+0001a0a0: 5f69 643d 4e6f 6e65 293a 0a20 2020 2020  _id=None):.     
+0001a0b0: 2020 2069 6620 6c6f 6361 7469 6f6e 5f69     if location_i
+0001a0c0: 6420 6973 204e 6f6e 653a 0a20 2020 2020  d is None:.     
+0001a0d0: 2020 2020 2020 206c 6f63 6174 696f 6e5f         location_
+0001a0e0: 6964 203d 2073 656c 662e 6765 745f 6964  id = self.get_id
+0001a0f0: 2829 0a20 2020 2020 2020 2069 6620 6c6f  ().        if lo
+0001a100: 6361 7469 6f6e 5f69 6420 6973 206e 6f74  cation_id is not
+0001a110: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001a120: 2020 2072 6573 706f 6e73 6520 3d20 7265     response = re
+0001a130: 7175 6573 7473 2e67 6574 280a 2020 2020  quests.get(.    
+0001a140: 2020 2020 2020 2020 2020 2020 7572 6c3d              url=
+0001a150: 7365 6c66 2e6c 6f63 6174 696f 6e5f 6279  self.location_by
+0001a160: 5f69 645f 656e 6470 6f69 6e74 2e66 6f72  _id_endpoint.for
+0001a170: 6d61 7428 6261 7365 5f75 726c 3d73 656c  mat(base_url=sel
+0001a180: 662e 6765 745f 6668 6972 5f75 726c 2829  f.get_fhir_url()
+0001a190: 2c20 6964 3d6c 6f63 6174 696f 6e5f 6964  , id=location_id
+0001a1a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001a1b0: 2020 2068 6561 6465 7273 3d73 656c 662e     headers=self.
+0001a1c0: 6865 6164 6572 732c 0a20 2020 2020 2020  headers,.       
+0001a1d0: 2020 2020 2020 2020 2076 6572 6966 793d           verify=
+0001a1e0: 7365 6c66 2e76 616c 6964 6174 655f 6365  self.validate_ce
+0001a1f0: 7274 730a 2020 2020 2020 2020 2020 2020  rts.            
+0001a200: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0001a210: 2072 6573 706f 6e73 652e 7374 6174 7573   response.status
+0001a220: 5f63 6f64 6520 3d3d 2032 3030 3a0a 2020  _code == 200:.  
+0001a230: 2020 2020 2020 2020 2020 2020 2020 6a73                js
+0001a240: 6f6e 6469 6374 203d 206a 736f 6e2e 6c6f  ondict = json.lo
+0001a250: 6164 7328 7265 7370 6f6e 7365 2e63 6f6e  ads(response.con
+0001a260: 7465 6e74 290a 2020 2020 2020 2020 2020  tent).          
+0001a270: 2020 2020 2020 7265 736f 7572 6365 203d        resource =
+0001a280: 2073 656c 662e 6765 745f 6d6f 6465 6c5f   self.get_model_
+0001a290: 6672 6f6d 5f6a 736f 6e28 6a73 6f6e 6469  from_json(jsondi
+0001a2a0: 6374 3d6a 736f 6e64 6963 7429 0a20 2020  ct=jsondict).   
+0001a2b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001a2c0: 7479 7065 2872 6573 6f75 7263 6529 2069  type(resource) i
+0001a2d0: 7320 4c6f 6361 7469 6f6e 3a0a 2020 2020  s Location:.    
+0001a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2f0: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
+0001a300: 6365 203d 2072 6573 6f75 7263 650a 2020  ce = resource.  
+0001a310: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001a320: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
+0001a330: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
+0001a340: 2020 2064 6566 2063 7265 6174 6528 7365     def create(se
+0001a350: 6c66 293a 0a20 2020 2020 2020 2072 6573  lf):.        res
+0001a360: 203d 2073 656c 662e 6765 7446 6869 7252   = self.getFhirR
+0001a370: 6573 6f75 7263 6528 290a 2020 2020 2020  esource().      
+0001a380: 2020 7265 7370 6f6e 7365 203d 2072 6571    response = req
+0001a390: 7565 7374 732e 706f 7374 280a 2020 2020  uests.post(.    
+0001a3a0: 2020 2020 2020 2020 7572 6c3d 7365 6c66          url=self
+0001a3b0: 2e6c 6f63 6174 696f 6e5f 656e 6470 6f69  .location_endpoi
+0001a3c0: 6e74 2e66 6f72 6d61 7428 6261 7365 5f75  nt.format(base_u
+0001a3d0: 726c 3d73 656c 662e 6765 745f 6668 6972  rl=self.get_fhir
+0001a3e0: 5f75 726c 2829 292c 0a20 2020 2020 2020  _url()),.       
+0001a3f0: 2020 2020 2064 6174 613d 6a73 6f6e 2e64       data=json.d
+0001a400: 756d 7073 2872 6573 292c 0a20 2020 2020  umps(res),.     
+0001a410: 2020 2020 2020 2068 6561 6465 7273 3d73         headers=s
+0001a420: 656c 662e 6865 6164 6572 732c 0a20 2020  elf.headers,.   
+0001a430: 2020 2020 2020 2020 2076 6572 6966 793d           verify=
+0001a440: 7365 6c66 2e76 616c 6964 6174 655f 6365  self.validate_ce
+0001a450: 7274 7329 0a20 2020 2020 2020 2069 6620  rts).        if 
+0001a460: 7265 7370 6f6e 7365 2e73 7461 7475 735f  response.status_
+0001a470: 636f 6465 203d 3d20 3230 313a 0a20 2020  code == 201:.   
+0001a480: 2020 2020 2020 2020 206a 736f 6e64 6963           jsondic
+0001a490: 7420 3d20 6a73 6f6e 2e6c 6f61 6473 2872  t = json.loads(r
+0001a4a0: 6573 706f 6e73 652e 636f 6e74 656e 7429  esponse.content)
+0001a4b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0001a4c0: 6f75 7263 6520 3d20 7365 6c66 2e67 6574  ource = self.get
+0001a4d0: 5f6d 6f64 656c 5f66 726f 6d5f 6a73 6f6e  _model_from_json
+0001a4e0: 286a 736f 6e64 6963 743d 6a73 6f6e 6469  (jsondict=jsondi
+0001a4f0: 6374 290a 2020 2020 2020 2020 2020 2020  ct).            
+0001a500: 6966 2074 7970 6528 7265 736f 7572 6365  if type(resource
+0001a510: 2920 6973 204c 6f63 6174 696f 6e3a 0a20  ) is Location:. 
+0001a520: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a530: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+0001a540: 6520 3d20 7265 736f 7572 6365 0a20 2020  e = resource.   
+0001a550: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+0001a560: 6f6e 7365 0a0a 2020 2020 6465 6620 7570  onse..    def up
+0001a570: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+0001a580: 2020 2020 7265 7320 3d20 7365 6c66 2e67      res = self.g
+0001a590: 6574 4668 6972 5265 736f 7572 6365 2829  etFhirResource()
+0001a5a0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+0001a5b0: 6520 3d20 7265 7175 6573 7473 2e70 7574  e = requests.put
+0001a5c0: 280a 2020 2020 2020 2020 2020 2020 7572  (.            ur
+0001a5d0: 6c3d 7365 6c66 2e6c 6f63 6174 696f 6e5f  l=self.location_
+0001a5e0: 6279 5f69 645f 656e 6470 6f69 6e74 2e66  by_id_endpoint.f
+0001a5f0: 6f72 6d61 7428 6261 7365 5f75 726c 3d73  ormat(base_url=s
+0001a600: 656c 662e 6765 745f 6668 6972 5f75 726c  elf.get_fhir_url
+0001a610: 2829 2c20 6964 3d73 656c 662e 6765 745f  (), id=self.get_
+0001a620: 6964 2829 292c 0a20 2020 2020 2020 2020  id()),.         
+0001a630: 2020 2064 6174 613d 6a73 6f6e 2e64 756d     data=json.dum
+0001a640: 7073 2872 6573 292c 0a20 2020 2020 2020  ps(res),.       
+0001a650: 2020 2020 2068 6561 6465 7273 3d73 656c       headers=sel
+0001a660: 662e 6865 6164 6572 732c 0a20 2020 2020  f.headers,.     
+0001a670: 2020 2020 2020 2076 6572 6966 793d 7365         verify=se
+0001a680: 6c66 2e76 616c 6964 6174 655f 6365 7274  lf.validate_cert
+0001a690: 7329 0a20 2020 2020 2020 2069 6620 7265  s).        if re
+0001a6a0: 7370 6f6e 7365 2e73 7461 7475 735f 636f  sponse.status_co
+0001a6b0: 6465 203d 3d20 3230 303a 0a20 2020 2020  de == 200:.     
+0001a6c0: 2020 2020 2020 206a 736f 6e64 6963 7420         jsondict 
+0001a6d0: 3d20 6a73 6f6e 2e6c 6f61 6473 2872 6573  = json.loads(res
+0001a6e0: 706f 6e73 652e 636f 6e74 656e 7429 0a20  ponse.content). 
+0001a6f0: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
+0001a700: 7263 6520 3d20 7365 6c66 2e67 6574 5f6d  rce = self.get_m
+0001a710: 6f64 656c 5f66 726f 6d5f 6a73 6f6e 286a  odel_from_json(j
+0001a720: 736f 6e64 6963 743d 6a73 6f6e 6469 6374  sondict=jsondict
+0001a730: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0001a740: 2074 7970 6528 7265 736f 7572 6365 2920   type(resource) 
+0001a750: 6973 204c 6f63 6174 696f 6e3a 0a20 2020  is Location:.   
+0001a760: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001a770: 662e 6668 6972 5f72 6573 6f75 7263 6520  f.fhir_resource 
+0001a780: 3d20 7265 736f 7572 6365 0a20 2020 2020  = resource.     
+0001a790: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
+0001a7a0: 7365 0a0a 2020 2020 6465 6620 6465 6c65  se..    def dele
+0001a7b0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0001a7c0: 2020 7265 7320 3d20 7365 6c66 2e67 6574    res = self.get
+0001a7d0: 4668 6972 5265 736f 7572 6365 2829 0a20  FhirResource(). 
+0001a7e0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+0001a7f0: 3d20 7265 7175 6573 7473 2e64 656c 6574  = requests.delet
+0001a800: 6528 0a20 2020 2020 2020 2020 2020 2075  e(.            u
+0001a810: 726c 3d73 656c 662e 6c6f 6361 7469 6f6e  rl=self.location
+0001a820: 5f62 795f 6964 5f65 6e64 706f 696e 742e  _by_id_endpoint.
+0001a830: 666f 726d 6174 2862 6173 655f 7572 6c3d  format(base_url=
+0001a840: 7365 6c66 2e67 6574 5f66 6869 725f 7572  self.get_fhir_ur
+0001a850: 6c28 292c 2069 643d 7365 6c66 2e67 6574  l(), id=self.get
+0001a860: 5f69 6428 2929 2c0a 2020 2020 2020 2020  _id()),.        
+0001a870: 2020 2020 6461 7461 3d6a 736f 6e2e 6475      data=json.du
+0001a880: 6d70 7328 7265 7329 2c0a 2020 2020 2020  mps(res),.      
+0001a890: 2020 2020 2020 6865 6164 6572 733d 7365        headers=se
+0001a8a0: 6c66 2e68 6561 6465 7273 2c0a 2020 2020  lf.headers,.    
+0001a8b0: 2020 2020 2020 2020 7665 7269 6679 3d73          verify=s
+0001a8c0: 656c 662e 7661 6c69 6461 7465 5f63 6572  elf.validate_cer
+0001a8d0: 7473 290a 2020 2020 2020 2020 7265 7475  ts).        retu
+0001a8e0: 726e 2072 6573 706f 6e73 650a 0a63 6c61  rn response..cla
+0001a8f0: 7373 204d 6564 6963 6174 696f 6e46 4849  ss MedicationFHI
+0001a900: 5228 4261 7365 4648 4952 293a 0a20 2020  R(BaseFHIR):.   
+0001a910: 206d 6564 6963 6174 696f 6e5f 656e 6470   medication_endp
+0001a920: 6f69 6e74 203d 2022 7b62 6173 655f 7572  oint = "{base_ur
+0001a930: 6c7d 2f4d 6564 6963 6174 696f 6e22 0a20  l}/Medication". 
+0001a940: 2020 2067 6574 5f62 795f 7472 6164 655f     get_by_trade_
+0001a950: 6e61 6d65 5f65 6e64 706f 696e 7420 3d20  name_endpoint = 
+0001a960: 6d65 6469 6361 7469 6f6e 5f65 6e64 706f  medication_endpo
+0001a970: 696e 7420 2b20 222f 7b74 7261 6465 5f6e  int + "/{trade_n
+0001a980: 616d 657d 220a 2020 2020 6465 6661 756c  ame}".    defaul
+0001a990: 745f 7175 616e 7469 7479 5f75 726c 203d  t_quantity_url =
+0001a9a0: 2027 6874 7470 3a2f 2f77 7777 2e73 616e   'http://www.san
+0001a9b0: 7465 7075 626c 6971 7565 2e72 7473 732e  tepublique.rtss.
+0001a9c0: 7163 2e63 612f 7369 706d 692f 6661 2f31  qc.ca/sipmi/fa/1
+0001a9d0: 2e30 2e30 2f65 7874 656e 7369 6f6e 732f  .0.0/extensions/
+0001a9e0: 236d 6564 6963 6174 696f 6e2f 6465 6661  #medication/defa
+0001a9f0: 756c 7471 7561 6e74 6974 7927 0a0a 2020  ultquantity'..  
+0001aa00: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0001aa10: 656c 662c 2062 6173 655f 7572 6c3d 4e6f  elf, base_url=No
+0001aa20: 6e65 2c20 6261 7365 5f75 7269 3d4e 6f6e  ne, base_uri=Non
+0001aa30: 652c 2072 6573 6f75 7263 653d 4e6f 6e65  e, resource=None
+0001aa40: 2c20 746f 6b65 6e5f 6865 6164 6572 3d4e  , token_header=N
+0001aa50: 6f6e 652c 2076 616c 6964 6174 655f 6365  one, validate_ce
+0001aa60: 7274 733d 5472 7565 2920 2d3e 204e 6f6e  rts=True) -> Non
+0001aa70: 653a 0a20 2020 2020 2020 2073 7570 6572  e:.        super
+0001aa80: 2829 2e5f 5f69 6e69 745f 5f28 6261 7365  ().__init__(base
+0001aa90: 5f75 726c 3d62 6173 655f 7572 6c2c 2062  _url=base_url, b
+0001aaa0: 6173 655f 7572 693d 6261 7365 5f75 7269  ase_uri=base_uri
+0001aab0: 2c20 746f 6b65 6e5f 6865 6164 6572 3d74  , token_header=t
+0001aac0: 6f6b 656e 5f68 6561 6465 7229 0a20 2020  oken_header).   
+0001aad0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+0001aae0: 7465 5f63 6572 7473 203d 2076 616c 6964  te_certs = valid
+0001aaf0: 6174 655f 6365 7274 730a 2020 2020 2020  ate_certs.      
+0001ab00: 2020 6966 2072 6573 6f75 7263 6520 6973    if resource is
+0001ab10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0001ab20: 2020 2020 2020 2073 656c 662e 6668 6972         self.fhir
+0001ab30: 5f72 6573 6f75 7263 6520 3d20 4d65 6469  _resource = Medi
+0001ab40: 6361 7469 6f6e 286a 736f 6e64 6963 743d  cation(jsondict=
+0001ab50: 7265 736f 7572 6365 290a 2020 2020 2020  resource).      
+0001ab60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001ab70: 2020 2020 7365 6c66 2e66 6869 725f 7265      self.fhir_re
+0001ab80: 736f 7572 6365 203d 204d 6564 6963 6174  source = Medicat
+0001ab90: 696f 6e28 290a 0a20 2020 2064 6566 2067  ion()..    def g
+0001aba0: 6574 4668 6972 5265 736f 7572 6365 2873  etFhirResource(s
+0001abb0: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+0001abc0: 7475 726e 2073 656c 662e 6668 6972 5f72  turn self.fhir_r
+0001abd0: 6573 6f75 7263 652e 6173 5f6a 736f 6e28  esource.as_json(
+0001abe0: 290a 0a20 2020 2064 6566 2067 6574 5f62  )..    def get_b
+0001abf0: 6174 6368 6573 2873 656c 6629 3a0a 2020  atches(self):.  
+0001ac00: 2020 2020 2020 6966 2074 7970 6528 7365        if type(se
+0001ac10: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+0001ac20: 2e70 726f 6475 6374 2920 6973 204d 6564  .product) is Med
+0001ac30: 6963 6174 696f 6e50 726f 6475 6374 2061  icationProduct a
+0001ac40: 6e64 2074 7970 6528 7365 6c66 2e66 6869  nd type(self.fhi
+0001ac50: 725f 7265 736f 7572 6365 2e70 726f 6475  r_resource.produ
+0001ac60: 6374 2e62 6174 6368 2920 6973 206c 6973  ct.batch) is lis
+0001ac70: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+0001ac80: 6574 7572 6e20 7365 6c66 2e66 6869 725f  eturn self.fhir_
+0001ac90: 7265 736f 7572 6365 2e70 726f 6475 6374  resource.product
+0001aca0: 2e62 6174 6368 0a20 2020 2020 2020 2072  .batch.        r
+0001acb0: 6574 7572 6e20 5b5d 0a0a 2020 2020 6465  eturn []..    de
+0001acc0: 6620 6765 745f 6279 5f74 7261 6465 5f6e  f get_by_trade_n
+0001acd0: 616d 6528 7365 6c66 2c20 7472 6164 655f  ame(self, trade_
+0001ace0: 6e61 6d65 293a 0a20 2020 2020 2020 206d  name):.        m
+0001acf0: 6564 6963 6174 696f 6e5f 7265 7370 6f6e  edication_respon
+0001ad00: 7365 203d 2072 6571 7565 7374 732e 6765  se = requests.ge
+0001ad10: 7428 0a20 2020 2020 2020 2020 2020 2075  t(.            u
+0001ad20: 726c 3d73 656c 662e 6765 745f 6279 5f74  rl=self.get_by_t
+0001ad30: 7261 6465 5f6e 616d 655f 656e 6470 6f69  rade_name_endpoi
+0001ad40: 6e74 2e66 6f72 6d61 7428 6261 7365 5f75  nt.format(base_u
+0001ad50: 726c 3d73 656c 662e 6765 745f 6668 6972  rl=self.get_fhir
+0001ad60: 5f75 726c 2829 2c20 7472 6164 655f 6e61  _url(), trade_na
+0001ad70: 6d65 3d74 7261 6465 5f6e 616d 6529 2c0a  me=trade_name),.
+0001ad80: 2020 2020 2020 2020 2020 2020 6865 6164              head
+0001ad90: 6572 733d 7365 6c66 2e68 6561 6465 7273  ers=self.headers
+0001ada0: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+0001adb0: 7269 6679 3d73 656c 662e 7661 6c69 6461  rify=self.valida
+0001adc0: 7465 5f63 6572 7473 0a20 2020 2020 2020  te_certs.       
+0001add0: 2029 0a20 2020 2020 2020 2069 6620 6d65   ).        if me
+0001ade0: 6469 6361 7469 6f6e 5f72 6573 706f 6e73  dication_respons
+0001adf0: 652e 7374 6174 7573 5f63 6f64 6520 3d3d  e.status_code ==
+0001ae00: 2032 3030 3a0a 2020 2020 2020 2020 2020   200:.          
+0001ae10: 2020 6d65 6469 6361 7469 6f6e 5f64 6963    medication_dic
+0001ae20: 7420 3d20 6a73 6f6e 2e6c 6f61 6473 286d  t = json.loads(m
+0001ae30: 6564 6963 6174 696f 6e5f 7265 7370 6f6e  edication_respon
+0001ae40: 7365 2e63 6f6e 7465 6e74 290a 2020 2020  se.content).    
+0001ae50: 2020 2020 2020 2020 7365 6c66 2e66 6869          self.fhi
+0001ae60: 725f 7265 736f 7572 6365 203d 204d 6564  r_resource = Med
+0001ae70: 6963 6174 696f 6e28 6a73 6f6e 6469 6374  ication(jsondict
+0001ae80: 3d6d 6564 6963 6174 696f 6e5f 6469 6374  =medication_dict
+0001ae90: 290a 0a20 2020 2064 6566 2067 6574 5f64  )..    def get_d
+0001aea0: 6566 6175 6c74 5f71 7561 6e74 6974 795f  efault_quantity_
+0001aeb0: 666f 725f 6261 7463 6828 7365 6c66 2c20  for_batch(self, 
+0001aec0: 6261 7463 6829 3a0a 2020 2020 2020 2020  batch):.        
+0001aed0: 666f 7220 6578 7420 696e 2062 6174 6368  for ext in batch
+0001aee0: 2e65 7874 656e 7369 6f6e 3a0a 2020 2020  .extension:.    
+0001aef0: 2020 2020 2020 2020 6966 2065 7874 2e75          if ext.u
+0001af00: 726c 203d 3d20 7365 6c66 2e64 6566 6175  rl == self.defau
+0001af10: 6c74 5f71 7561 6e74 6974 795f 7572 6c3a  lt_quantity_url:
+0001af20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001af30: 2072 6574 7572 6e20 6578 742e 7661 6c75   return ext.valu
+0001af40: 6551 7561 6e74 6974 790a 0a63 6c61 7373  eQuantity..class
+0001af50: 2050 7261 6374 6974 696f 6e65 7246 4849   PractitionerFHI
+0001af60: 5228 4261 7365 4648 4952 293a 0a20 2020  R(BaseFHIR):.   
+0001af70: 2070 7261 6374 6974 696f 6e65 725f 656e   practitioner_en
+0001af80: 6470 6f69 6e74 203d 2022 7b62 6173 655f  dpoint = "{base_
+0001af90: 7572 6c7d 2f50 7261 6374 6974 696f 6e65  url}/Practitione
+0001afa0: 7222 0a20 2020 2070 7261 6374 6974 696f  r".    practitio
+0001afb0: 6e65 725f 6279 5f69 645f 656e 6470 6f69  ner_by_id_endpoi
+0001afc0: 6e74 203d 2070 7261 6374 6974 696f 6e65  nt = practitione
+0001afd0: 725f 656e 6470 6f69 6e74 202b 2022 2f7b  r_endpoint + "/{
+0001afe0: 6964 7d22 0a0a 2020 2020 6465 6620 5f5f  id}"..    def __
+0001aff0: 696e 6974 5f5f 2873 656c 662c 2062 6173  init__(self, bas
+0001b000: 655f 7572 6c3d 4e6f 6e65 2c20 6261 7365  e_url=None, base
+0001b010: 5f75 7269 3d4e 6f6e 652c 2072 6573 6f75  _uri=None, resou
+0001b020: 7263 653d 4e6f 6e65 2c20 746f 6b65 6e5f  rce=None, token_
+0001b030: 6865 6164 6572 3d4e 6f6e 652c 2076 616c  header=None, val
+0001b040: 6964 6174 655f 6365 7274 733d 5472 7565  idate_certs=True
+0001b050: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0001b060: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+0001b070: 745f 5f28 6261 7365 5f75 726c 3d62 6173  t__(base_url=bas
+0001b080: 655f 7572 6c2c 2062 6173 655f 7572 693d  e_url, base_uri=
+0001b090: 6261 7365 5f75 7269 2c20 746f 6b65 6e5f  base_uri, token_
+0001b0a0: 6865 6164 6572 3d74 6f6b 656e 5f68 6561  header=token_hea
+0001b0b0: 6465 7229 0a20 2020 2020 2020 2073 656c  der).        sel
+0001b0c0: 662e 7661 6c69 6461 7465 5f63 6572 7473  f.validate_certs
+0001b0d0: 203d 2076 616c 6964 6174 655f 6365 7274   = validate_cert
+0001b0e0: 730a 2020 2020 2020 2020 6966 2072 6573  s.        if res
+0001b0f0: 6f75 7263 6520 6973 206e 6f74 204e 6f6e  ource is not Non
+0001b100: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0001b110: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+0001b120: 6520 3d20 5072 6163 7469 7469 6f6e 6572  e = Practitioner
+0001b130: 286a 736f 6e64 6963 743d 7265 736f 7572  (jsondict=resour
+0001b140: 6365 290a 2020 2020 2020 2020 656c 7365  ce).        else
+0001b150: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0001b160: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+0001b170: 203d 2050 7261 6374 6974 696f 6e65 7228   = Practitioner(
+0001b180: 290a 0a20 2020 2064 6566 2067 6574 4668  )..    def getFh
+0001b190: 6972 5265 736f 7572 6365 2873 656c 6629  irResource(self)
+0001b1a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001b1b0: 2073 656c 662e 6668 6972 5f72 6573 6f75   self.fhir_resou
+0001b1c0: 7263 652e 6173 5f6a 736f 6e28 290a 0a20  rce.as_json().. 
+0001b1d0: 2020 2064 6566 2073 6561 7263 6828 7365     def search(se
+0001b1e0: 6c66 2c20 6964 656e 7469 6669 6572 3d4e  lf, identifier=N
+0001b1f0: 6f6e 652c 2072 6f6c 653d 4e6f 6e65 2c20  one, role=None, 
+0001b200: 6661 6d69 6c79 3d4e 6f6e 652c 2067 6976  family=None, giv
+0001b210: 656e 3d4e 6f6e 6529 3a0a 2020 2020 2020  en=None):.      
+0001b220: 2020 7061 7261 6d73 203d 207b 7d0a 2020    params = {}.  
+0001b230: 2020 2020 2020 6966 2069 6465 6e74 6966        if identif
+0001b240: 6965 7220 6973 206e 6f74 204e 6f6e 653a  ier is not None:
+0001b250: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+0001b260: 616d 735b 2269 6465 6e74 6966 6965 7222  ams["identifier"
+0001b270: 5d20 3d20 6964 656e 7469 6669 6572 0a20  ] = identifier. 
+0001b280: 2020 2020 2020 2069 6620 726f 6c65 2069         if role i
+0001b290: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0001b2a0: 2020 2020 2020 2020 7061 7261 6d73 5b22          params["
+0001b2b0: 726f 6c65 225d 203d 2072 6f6c 650a 2020  role"] = role.  
+0001b2c0: 2020 2020 2020 6966 2066 616d 696c 7920        if family 
+0001b2d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0001b2e0: 2020 2020 2020 2020 2070 6172 616d 735b           params[
+0001b2f0: 2266 616d 696c 7922 5d20 3d20 6661 6d69  "family"] = fami
+0001b300: 6c79 0a20 2020 2020 2020 2069 6620 6769  ly.        if gi
+0001b310: 7665 6e20 6973 206e 6f74 204e 6f6e 653a  ven is not None:
+0001b320: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+0001b330: 616d 735b 2267 6976 656e 225d 203d 2067  ams["given"] = g
+0001b340: 6976 656e 0a0a 2020 2020 2020 2020 7072  iven..        pr
+0001b350: 6163 7469 7469 6f6e 6572 5f72 6573 706f  actitioner_respo
+0001b360: 6e73 6520 3d20 7265 7175 6573 7473 2e67  nse = requests.g
+0001b370: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+0001b380: 7572 6c3d 7365 6c66 2e70 7261 6374 6974  url=self.practit
+0001b390: 696f 6e65 725f 656e 6470 6f69 6e74 2e66  ioner_endpoint.f
+0001b3a0: 6f72 6d61 7428 6261 7365 5f75 726c 3d73  ormat(base_url=s
+0001b3b0: 656c 662e 6765 745f 6668 6972 5f75 726c  elf.get_fhir_url
+0001b3c0: 2829 292c 0a20 2020 2020 2020 2020 2020  ()),.           
+0001b3d0: 2068 6561 6465 7273 3d73 656c 662e 6865   headers=self.he
+0001b3e0: 6164 6572 732c 0a20 2020 2020 2020 2020  aders,.         
+0001b3f0: 2020 2070 6172 616d 733d 7061 7261 6d73     params=params
+0001b400: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+0001b410: 7269 6679 3d73 656c 662e 7661 6c69 6461  rify=self.valida
+0001b420: 7465 5f63 6572 7473 0a20 2020 2020 2020  te_certs.       
+0001b430: 2029 0a20 2020 2020 2020 2069 6620 7072   ).        if pr
+0001b440: 6163 7469 7469 6f6e 6572 5f72 6573 706f  actitioner_respo
+0001b450: 6e73 652e 7374 6174 7573 5f63 6f64 6520  nse.status_code 
+0001b460: 3d3d 2032 3030 3a0a 2020 2020 2020 2020  == 200:.        
+0001b470: 2020 2020 636f 6e74 656e 745f 6469 6374      content_dict
+0001b480: 203d 206a 736f 6e2e 6c6f 6164 7328 7072   = json.loads(pr
+0001b490: 6163 7469 7469 6f6e 6572 5f72 6573 706f  actitioner_respo
+0001b4a0: 6e73 652e 636f 6e74 656e 7429 0a20 2020  nse.content).   
+0001b4b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001b4c0: 4275 6e64 6c65 4648 4952 2872 6573 6f75  BundleFHIR(resou
+0001b4d0: 7263 653d 636f 6e74 656e 745f 6469 6374  rce=content_dict
+0001b4e0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001b4f0: 204e 6f6e 650a 0a20 2020 2064 6566 2067   None..    def g
+0001b500: 6574 5f66 616d 696c 7928 7365 6c66 2c20  et_family(self, 
+0001b510: 7072 6163 7469 7469 6f6e 6572 3d4e 6f6e  practitioner=Non
+0001b520: 6529 3a0a 2020 2020 2020 2020 6966 2070  e):.        if p
+0001b530: 7261 6374 6974 696f 6e65 7220 6973 204e  ractitioner is N
+0001b540: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0001b550: 2070 7261 6374 6974 696f 6e65 7220 3d20   practitioner = 
+0001b560: 7365 6c66 2e66 6869 725f 7265 736f 7572  self.fhir_resour
+0001b570: 6365 0a0a 2020 2020 2020 2020 6966 2074  ce..        if t
+0001b580: 7970 6528 7072 6163 7469 7469 6f6e 6572  ype(practitioner
+0001b590: 2e6e 616d 6529 2069 7320 4875 6d61 6e4e  .name) is HumanN
+0001b5a0: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+0001b5b0: 2072 6574 7572 6e20 7072 6163 7469 7469   return practiti
+0001b5c0: 6f6e 6572 2e6e 616d 652e 6661 6d69 6c79  oner.name.family
+0001b5d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001b5e0: 4e6f 6e65 0a0a 0a20 2020 2064 6566 2067  None...    def g
+0001b5f0: 6574 5f67 6976 656e 2873 656c 662c 2070  et_given(self, p
+0001b600: 7261 6374 6974 696f 6e65 723d 4e6f 6e65  ractitioner=None
+0001b610: 293a 0a20 2020 2020 2020 2069 6620 7072  ):.        if pr
+0001b620: 6163 7469 7469 6f6e 6572 2069 7320 4e6f  actitioner is No
+0001b630: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001b640: 7072 6163 7469 7469 6f6e 6572 203d 2073  practitioner = s
+0001b650: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+0001b660: 650a 0a20 2020 2020 2020 2069 6620 7479  e..        if ty
+0001b670: 7065 2870 7261 6374 6974 696f 6e65 722e  pe(practitioner.
+0001b680: 6e61 6d65 2920 6973 2048 756d 616e 4e61  name) is HumanNa
+0001b690: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+0001b6a0: 7265 7475 726e 2070 7261 6374 6974 696f  return practitio
+0001b6b0: 6e65 722e 6e61 6d65 2e67 6976 656e 0a20  ner.name.given. 
+0001b6c0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0001b6d0: 6e65 0a0a 2020 2020 6465 6620 6765 745f  ne..    def get_
+0001b6e0: 6964 2873 656c 662c 2070 7261 6374 6974  id(self, practit
+0001b6f0: 696f 6e65 723d 4e6f 6e65 293a 0a20 2020  ioner=None):.   
+0001b700: 2020 2020 2069 6620 7072 6163 7469 7469       if practiti
+0001b710: 6f6e 6572 2069 7320 4e6f 6e65 3a0a 2020  oner is None:.  
+0001b720: 2020 2020 2020 2020 2020 7072 6163 7469            practi
+0001b730: 7469 6f6e 6572 203d 2073 656c 662e 6668  tioner = self.fh
+0001b740: 6972 5f72 6573 6f75 7263 650a 2020 2020  ir_resource.    
+0001b750: 2020 2020 7265 7475 726e 2070 7261 6374      return pract
+0001b760: 6974 696f 6e65 722e 6964 0a0a 2020 2020  itioner.id..    
+0001b770: 6465 6620 6765 745f 6279 5f69 6428 7365  def get_by_id(se
+0001b780: 6c66 2c20 7072 6163 7469 7469 6f6e 6572  lf, practitioner
+0001b790: 5f69 643d 4e6f 6e65 293a 0a20 2020 2020  _id=None):.     
+0001b7a0: 2020 2069 6620 7072 6163 7469 7469 6f6e     if practition
+0001b7b0: 6572 5f69 6420 6973 204e 6f6e 653a 0a20  er_id is None:. 
+0001b7c0: 2020 2020 2020 2020 2020 2070 7261 6374             pract
+0001b7d0: 6974 696f 6e65 725f 6964 203d 2073 656c  itioner_id = sel
+0001b7e0: 662e 6765 745f 6964 2829 0a20 2020 2020  f.get_id().     
+0001b7f0: 2020 2069 6620 7072 6163 7469 7469 6f6e     if practition
+0001b800: 6572 5f69 6420 6973 206e 6f74 204e 6f6e  er_id is not Non
+0001b810: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0001b820: 6573 706f 6e73 6520 3d20 7265 7175 6573  esponse = reques
+0001b830: 7473 2e67 6574 280a 2020 2020 2020 2020  ts.get(.        
+0001b840: 2020 2020 2020 2020 7572 6c3d 7365 6c66          url=self
+0001b850: 2e70 7261 6374 6974 696f 6e65 725f 6279  .practitioner_by
+0001b860: 5f69 645f 656e 6470 6f69 6e74 2e66 6f72  _id_endpoint.for
+0001b870: 6d61 7428 6261 7365 5f75 726c 3d73 656c  mat(base_url=sel
+0001b880: 662e 6765 745f 6668 6972 5f75 726c 2829  f.get_fhir_url()
+0001b890: 2c20 6964 3d70 7261 6374 6974 696f 6e65  , id=practitione
+0001b8a0: 725f 6964 292c 0a20 2020 2020 2020 2020  r_id),.         
+0001b8b0: 2020 2020 2020 2068 6561 6465 7273 3d73         headers=s
+0001b8c0: 656c 662e 6865 6164 6572 732c 0a20 2020  elf.headers,.   
+0001b8d0: 2020 2020 2020 2020 2020 2020 2076 6572               ver
+0001b8e0: 6966 793d 7365 6c66 2e76 616c 6964 6174  ify=self.validat
+0001b8f0: 655f 6365 7274 730a 2020 2020 2020 2020  e_certs.        
+0001b900: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001b910: 2020 6966 2072 6573 706f 6e73 652e 7374    if response.st
+0001b920: 6174 7573 5f63 6f64 6520 3d3d 2032 3030  atus_code == 200
+0001b930: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b940: 2020 6a73 6f6e 6469 6374 203d 206a 736f    jsondict = jso
+0001b950: 6e2e 6c6f 6164 7328 7265 7370 6f6e 7365  n.loads(response
+0001b960: 2e63 6f6e 7465 6e74 290a 2020 2020 2020  .content).      
+0001b970: 2020 2020 2020 2020 2020 7265 736f 7572            resour
+0001b980: 6365 203d 2073 656c 662e 6765 745f 6d6f  ce = self.get_mo
+0001b990: 6465 6c5f 6672 6f6d 5f6a 736f 6e28 6a73  del_from_json(js
+0001b9a0: 6f6e 6469 6374 3d6a 736f 6e64 6963 7429  ondict=jsondict)
+0001b9b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b9c0: 2069 6620 7479 7065 2872 6573 6f75 7263   if type(resourc
+0001b9d0: 6529 2069 7320 4c6f 6361 7469 6f6e 3a0a  e) is Location:.
+0001b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9f0: 2020 2020 7365 6c66 2e66 6869 725f 7265      self.fhir_re
+0001ba00: 736f 7572 6365 203d 2072 6573 6f75 7263  source = resourc
+0001ba10: 650a 2020 2020 2020 2020 2020 2020 7265  e.            re
+0001ba20: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+0001ba30: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0001ba40: 6e65 0a0a 636c 6173 7320 5661 6c75 6553  ne..class ValueS
+0001ba50: 6574 4648 4952 2842 6173 6546 4849 5229  etFHIR(BaseFHIR)
+0001ba60: 3a0a 2020 2020 7661 6c75 6573 6574 5f65  :.    valueset_e
+0001ba70: 6e64 706f 696e 7420 3d20 227b 6261 7365  ndpoint = "{base
+0001ba80: 5f75 726c 7d2f 5661 6c75 6553 6574 220a  _url}/ValueSet".
+0001ba90: 2020 2020 7661 6c75 6573 6574 5f76 6f63      valueset_voc
+0001baa0: 6162 756c 6172 795f 646f 6d61 696e 5f65  abulary_domain_e
+0001bab0: 6e64 706f 696e 7420 3d20 7661 6c75 6573  ndpoint = values
+0001bac0: 6574 5f65 6e64 706f 696e 7420 2b20 222f  et_endpoint + "/
+0001bad0: 7b64 6f6d 6169 6e7d 220a 0a20 2020 2064  {domain}"..    d
+0001bae0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0001baf0: 2c20 6261 7365 5f75 726c 3d4e 6f6e 652c  , base_url=None,
+0001bb00: 2062 6173 655f 7572 693d 4e6f 6e65 2c20   base_uri=None, 
+0001bb10: 7265 736f 7572 6365 3d4e 6f6e 652c 2074  resource=None, t
+0001bb20: 6f6b 656e 5f68 6561 6465 723d 4e6f 6e65  oken_header=None
+0001bb30: 2c20 7661 6c69 6461 7465 5f63 6572 7473  , validate_certs
+0001bb40: 3d54 7275 6529 202d 3e20 4e6f 6e65 3a0a  =True) -> None:.
+0001bb50: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+0001bb60: 5f5f 696e 6974 5f5f 2862 6173 655f 7572  __init__(base_ur
+0001bb70: 6c3d 6261 7365 5f75 726c 2c20 6261 7365  l=base_url, base
+0001bb80: 5f75 7269 3d62 6173 655f 7572 692c 2074  _uri=base_uri, t
+0001bb90: 6f6b 656e 5f68 6561 6465 723d 746f 6b65  oken_header=toke
+0001bba0: 6e5f 6865 6164 6572 290a 2020 2020 2020  n_header).      
+0001bbb0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+0001bbc0: 6365 7274 7320 3d20 7661 6c69 6461 7465  certs = validate
+0001bbd0: 5f63 6572 7473 0a20 2020 2020 2020 2069  _certs.        i
+0001bbe0: 6620 7265 736f 7572 6365 2069 7320 6e6f  f resource is no
+0001bbf0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0001bc00: 2020 2020 7365 6c66 2e66 6869 725f 7265      self.fhir_re
+0001bc10: 736f 7572 6365 203d 2056 616c 7565 5365  source = ValueSe
+0001bc20: 7428 6a73 6f6e 6469 6374 3d72 6573 6f75  t(jsondict=resou
+0001bc30: 7263 6529 0a20 2020 2020 2020 2065 6c73  rce).        els
+0001bc40: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0001bc50: 656c 662e 6668 6972 5f72 6573 6f75 7263  elf.fhir_resourc
+0001bc60: 6520 3d20 5661 6c75 6553 6574 2829 0a0a  e = ValueSet()..
+0001bc70: 2020 2020 6465 6620 6765 7446 6869 7252      def getFhirR
+0001bc80: 6573 6f75 7263 6528 7365 6c66 293a 0a20  esource(self):. 
+0001bc90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001bca0: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+0001bcb0: 2e61 735f 6a73 6f6e 2829 0a0a 2020 2020  .as_json()..    
+0001bcc0: 6465 6620 6765 745f 6765 6e64 6572 2873  def get_gender(s
+0001bcd0: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+0001bce0: 7475 726e 2073 656c 662e 6765 745f 7661  turn self.get_va
+0001bcf0: 6c75 6573 6574 5f62 795f 646f 6d61 696e  lueset_by_domain
+0001bd00: 2864 6f6d 6169 6e3d 2267 656e 6465 7222  (domain="gender"
+0001bd10: 290a 0a20 2020 2064 6566 2067 6574 5f61  )..    def get_a
+0001bd20: 646d 696e 6973 7472 6174 696f 6e73 6974  dministrationsit
+0001bd30: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0001bd40: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
+0001bd50: 5f76 616c 7565 7365 745f 6279 5f64 6f6d  _valueset_by_dom
+0001bd60: 6169 6e28 646f 6d61 696e 3d22 6164 6d69  ain(domain="admi
+0001bd70: 6e69 7374 7261 7469 6f6e 7369 7465 2229  nistrationsite")
+0001bd80: 0a0a 2020 2020 6465 6620 6765 745f 7661  ..    def get_va
+0001bd90: 6c75 6573 6574 5f62 795f 646f 6d61 696e  lueset_by_domain
+0001bda0: 2873 656c 662c 2064 6f6d 6169 6e29 3a0a  (self, domain):.
+0001bdb0: 2020 2020 2020 2020 7661 6c75 6573 6574          valueset
+0001bdc0: 5f72 6573 706f 6e73 6520 3d20 7265 7175  _response = requ
+0001bdd0: 6573 7473 2e67 6574 280a 2020 2020 2020  ests.get(.      
+0001bde0: 2020 2020 2020 7572 6c3d 7365 6c66 2e76        url=self.v
+0001bdf0: 616c 7565 7365 745f 766f 6361 6275 6c61  alueset_vocabula
+0001be00: 7279 5f64 6f6d 6169 6e5f 656e 6470 6f69  ry_domain_endpoi
+0001be10: 6e74 2e66 6f72 6d61 7428 6261 7365 5f75  nt.format(base_u
+0001be20: 726c 3d73 656c 662e 6765 745f 6668 6972  rl=self.get_fhir
+0001be30: 5f75 726c 2829 2c20 646f 6d61 696e 3d64  _url(), domain=d
+0001be40: 6f6d 6169 6e29 2c0a 2020 2020 2020 2020  omain),.        
+0001be50: 2020 2020 6865 6164 6572 733d 7365 6c66      headers=self
+0001be60: 2e68 6561 6465 7273 2c0a 2020 2020 2020  .headers,.      
+0001be70: 2020 2020 2020 7665 7269 6679 3d73 656c        verify=sel
+0001be80: 662e 7661 6c69 6461 7465 5f63 6572 7473  f.validate_certs
+0001be90: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0001bea0: 2020 2069 6620 7661 6c75 6573 6574 5f72     if valueset_r
+0001beb0: 6573 706f 6e73 652e 7374 6174 7573 5f63  esponse.status_c
+0001bec0: 6f64 6520 3d3d 2032 3030 3a0a 2020 2020  ode == 200:.    
+0001bed0: 2020 2020 2020 2020 636f 6e74 656e 745f          content_
+0001bee0: 6469 6374 203d 206a 736f 6e2e 6c6f 6164  dict = json.load
+0001bef0: 7328 7661 6c75 6573 6574 5f72 6573 706f  s(valueset_respo
+0001bf00: 6e73 652e 636f 6e74 656e 7429 0a20 2020  nse.content).   
+0001bf10: 2020 2020 2020 2020 2073 656c 662e 6668           self.fh
+0001bf20: 6972 5f72 6573 6f75 7263 6520 3d20 5661  ir_resource = Va
+0001bf30: 6c75 6553 6574 286a 736f 6e64 6963 743d  lueSet(jsondict=
+0001bf40: 636f 6e74 656e 745f 6469 6374 290a 0a20  content_dict).. 
+0001bf50: 2020 2020 2020 2072 6574 7572 6e20 7661         return va
+0001bf60: 6c75 6573 6574 5f72 6573 706f 6e73 650a  lueset_response.
+0001bf70: 0a20 2020 2064 6566 2073 6561 7263 685f  .    def search_
+0001bf80: 636f 6465 5f73 7973 7465 6d5f 636f 6e63  code_system_conc
+0001bf90: 6570 7428 7365 6c66 2c20 636f 6465 3d4e  ept(self, code=N
+0001bfa0: 6f6e 652c 2064 6973 706c 6179 3d4e 6f6e  one, display=Non
+0001bfb0: 6529 3a0a 2020 2020 2020 2020 636f 6465  e):.        code
+0001bfc0: 5f73 7973 7465 6d5f 636f 6e63 6570 7420  _system_concept 
+0001bfd0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+0001bfe0: 6620 2873 656c 662e 6668 6972 5f72 6573  f (self.fhir_res
+0001bff0: 6f75 7263 6520 6973 206e 6f74 204e 6f6e  ource is not Non
+0001c000: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0001c010: 2020 616e 6420 7365 6c66 2e66 6869 725f    and self.fhir_
+0001c020: 7265 736f 7572 6365 2e63 6f64 6553 7973  resource.codeSys
+0001c030: 7465 6d20 6973 206e 6f74 204e 6f6e 650a  tem is not None.
+0001c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c050: 616e 6420 7365 6c66 2e66 6869 725f 7265  and self.fhir_re
+0001c060: 736f 7572 6365 2e63 6f64 6553 7973 7465  source.codeSyste
+0001c070: 6d2e 636f 6e63 6570 7420 6973 206e 6f74  m.concept is not
 0001c080: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0001c090: 2020 2020 2020 616e 6420 7365 6c66 2e66        and self.f
-0001c0a0: 6869 725f 7265 736f 7572 6365 2e63 6f64  hir_resource.cod
-0001c0b0: 6553 7973 7465 6d20 6973 206e 6f74 204e  eSystem is not N
-0001c0c0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-0001c0d0: 2020 2020 616e 6420 7365 6c66 2e66 6869      and self.fhi
-0001c0e0: 725f 7265 736f 7572 6365 2e63 6f64 6553  r_resource.codeS
-0001c0f0: 7973 7465 6d2e 636f 6e63 6570 7420 6973  ystem.concept is
-0001c100: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
-0001c110: 2020 2020 2020 2020 2020 616e 6420 6c65            and le
-0001c120: 6e28 7365 6c66 2e66 6869 725f 7265 736f  n(self.fhir_reso
-0001c130: 7572 6365 2e63 6f64 6553 7973 7465 6d2e  urce.codeSystem.
-0001c140: 636f 6e63 6570 7429 203e 2030 293a 0a20  concept) > 0):. 
-0001c150: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-0001c160: 6f6e 6365 7074 2069 6e20 7365 6c66 2e66  oncept in self.f
-0001c170: 6869 725f 7265 736f 7572 6365 2e63 6f64  hir_resource.cod
-0001c180: 6553 7973 7465 6d2e 636f 6e63 6570 743a  eSystem.concept:
-0001c190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c1a0: 2069 6620 2828 636f 6465 2069 7320 6e6f   if ((code is no
-0001c1b0: 7420 4e6f 6e65 2061 6e64 2063 6f6e 6365  t None and conce
-0001c1c0: 7074 2e63 6f64 6520 3d3d 2063 6f64 6529  pt.code == code)
-0001c1d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c1e0: 2020 2020 2020 2020 206f 7220 2864 6973           or (dis
-0001c1f0: 706c 6179 2069 7320 6e6f 7420 4e6f 6e65  play is not None
-0001c200: 2061 6e64 2063 6f6e 6365 7074 2e64 6973   and concept.dis
-0001c210: 706c 6179 203d 3d20 6469 7370 6c61 7929  play == display)
-0001c220: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001c230: 2020 2020 2020 2063 6f64 655f 7379 7374         code_syst
-0001c240: 656d 5f63 6f6e 6365 7074 203d 2063 6f6e  em_concept = con
-0001c250: 6365 7074 0a0a 2020 2020 2020 2020 7265  cept..        re
-0001c260: 7475 726e 2063 6f64 655f 7379 7374 656d  turn code_system
-0001c270: 5f63 6f6e 6365 7074 0a0a                 _concept..
+0001c090: 2020 2020 2020 616e 6420 6c65 6e28 7365        and len(se
+0001c0a0: 6c66 2e66 6869 725f 7265 736f 7572 6365  lf.fhir_resource
+0001c0b0: 2e63 6f64 6553 7973 7465 6d2e 636f 6e63  .codeSystem.conc
+0001c0c0: 6570 7429 203e 2030 293a 0a20 2020 2020  ept) > 0):.     
+0001c0d0: 2020 2020 2020 2066 6f72 2063 6f6e 6365         for conce
+0001c0e0: 7074 2069 6e20 7365 6c66 2e66 6869 725f  pt in self.fhir_
+0001c0f0: 7265 736f 7572 6365 2e63 6f64 6553 7973  resource.codeSys
+0001c100: 7465 6d2e 636f 6e63 6570 743a 0a20 2020  tem.concept:.   
+0001c110: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001c120: 2828 636f 6465 2069 7320 6e6f 7420 4e6f  ((code is not No
+0001c130: 6e65 2061 6e64 2063 6f6e 6365 7074 2e63  ne and concept.c
+0001c140: 6f64 6520 3d3d 2063 6f64 6529 0a20 2020  ode == code).   
+0001c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c160: 2020 2020 206f 7220 2864 6973 706c 6179       or (display
+0001c170: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0001c180: 2063 6f6e 6365 7074 2e64 6973 706c 6179   concept.display
+0001c190: 203d 3d20 6469 7370 6c61 7929 293a 0a20   == display)):. 
+0001c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1b0: 2020 2063 6f64 655f 7379 7374 656d 5f63     code_system_c
+0001c1c0: 6f6e 6365 7074 203d 2063 6f6e 6365 7074  oncept = concept
+0001c1d0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001c1e0: 2063 6f64 655f 7379 7374 656d 5f63 6f6e   code_system_con
+0001c1f0: 6365 7074 0a0a                           cept..
```

### Comparing `inspqcommun-1.6.3/inspqcommun/identity/keycloak.py` & `inspqcommun-1.6.4/inspqcommun/identity/keycloak.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/inspqcommun/identity/keycloak_token.py` & `inspqcommun-1.6.4/inspqcommun/identity/keycloak_token.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/inspqcommun/identity/keycloak_tools.py` & `inspqcommun-1.6.4/inspqcommun/identity/keycloak_tools.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/inspqcommun/kafka/consommateur.py` & `inspqcommun-1.6.4/inspqcommun/kafka/consommateur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/inspqcommun/kafka/producteur.py` & `inspqcommun-1.6.4/inspqcommun/kafka/producteur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/inspqcommun/userprovisioning/scim.py` & `inspqcommun-1.6.4/inspqcommun/userprovisioning/scim.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/inspqcommun.egg-info/PKG-INFO` & `inspqcommun-1.6.4/inspqcommun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspqcommun
-Version: 1.6.3
+Version: 1.6.4
 Summary: Librairies communes de INSPQ
 Home-page: https://gitlab.forge.gouv.qc.ca/inspq/commun/python/inspqcommun.git
 Author: Philippe Gauthier
 Author-email: philippe.gauthier@inspq.qc.ca
 License: LiLiQ
 License-File: LICENSE
```

### Comparing `inspqcommun-1.6.3/inspqcommun.egg-info/SOURCES.txt` & `inspqcommun-1.6.4/inspqcommun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/setup.py` & `inspqcommun-1.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/tests/test_fhir.py` & `inspqcommun-1.6.4/tests/test_fhir.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/tests/test_integration_fhir.py` & `inspqcommun-1.6.4/tests/test_integration_fhir.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/tests/test_integration_keycloak.py` & `inspqcommun-1.6.4/tests/test_integration_keycloak.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/tests/test_kafka.py` & `inspqcommun-1.6.4/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/tests/test_keycloak.py` & `inspqcommun-1.6.4/tests/test_keycloak.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-1.6.3/tests/test_scim.py` & `inspqcommun-1.6.4/tests/test_scim.py`

 * *Files identical despite different names*

