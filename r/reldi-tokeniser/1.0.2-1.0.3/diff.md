# Comparing `tmp/reldi-tokeniser-1.0.2.tar.gz` & `tmp/reldi-tokeniser-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/luka/Development/rsdo/reldi-tokeniser/dist/tmp_sbgzq_4/reldi-tokeniser-1.0.2.tar", last modified: Tue Jun 28 12:30:03 2022, max compression
+gzip compressed data, was "reldi-tokeniser-1.0.3.tar", last modified: Thu Jul 27 11:07:27 2023, max compression
```

## Comparing `reldi-tokeniser-1.0.2.tar` & `reldi-tokeniser-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 luka      (1000) luka      (1000)        0 2022-06-28 12:30:03.000000 reldi-tokeniser-1.0.2/
--rw-rw-r--   0 luka      (1000) luka      (1000)    11357 2021-09-09 07:39:32.000000 reldi-tokeniser-1.0.2/LICENSE
--rw-rw-r--   0 luka      (1000) luka      (1000)     3900 2022-06-28 12:30:03.000000 reldi-tokeniser-1.0.2/PKG-INFO
--rw-rw-r--   0 luka      (1000) luka      (1000)     3609 2021-12-29 08:03:19.000000 reldi-tokeniser-1.0.2/README.md
-drwxrwxr-x   0 luka      (1000) luka      (1000)        0 2022-06-28 12:30:03.000000 reldi-tokeniser-1.0.2/reldi_tokeniser/
--rw-rw-r--   0 luka      (1000) luka      (1000)       28 2021-12-29 08:03:19.000000 reldi-tokeniser-1.0.2/reldi_tokeniser/__init__.py
--rw-rw-r--   0 luka      (1000) luka      (1000)     2621 2021-12-29 08:03:19.000000 reldi-tokeniser-1.0.2/reldi_tokeniser/bg.abbrev
--rw-rw-r--   0 luka      (1000) luka      (1000)      950 2021-12-29 08:03:19.000000 reldi-tokeniser-1.0.2/reldi_tokeniser/hr.abbrev
--rw-rw-r--   0 luka      (1000) luka      (1000)     1743 2021-12-29 08:03:19.000000 reldi-tokeniser-1.0.2/reldi_tokeniser/mk.abbrev
--rw-rw-r--   0 luka      (1000) luka      (1000)     2470 2021-12-29 08:03:19.000000 reldi-tokeniser-1.0.2/reldi_tokeniser/punct
--rw-rw-r--   0 luka      (1000) luka      (1000)     1573 2021-12-29 08:03:19.000000 reldi-tokeniser-1.0.2/reldi_tokeniser/sl.abbrev
--rw-rw-r--   0 luka      (1000) luka      (1000)     2052 2021-12-29 08:03:19.000000 reldi-tokeniser-1.0.2/reldi_tokeniser/sr.abbrev
--rwxrwxr-x   0 luka      (1000) luka      (1000)    14651 2022-06-28 08:19:08.000000 reldi-tokeniser-1.0.2/reldi_tokeniser/tokeniser.py
-drwxrwxr-x   0 luka      (1000) luka      (1000)        0 2022-06-28 12:30:03.000000 reldi-tokeniser-1.0.2/reldi_tokeniser.egg-info/
--rw-rw-r--   0 luka      (1000) luka      (1000)     3900 2022-06-28 12:30:03.000000 reldi-tokeniser-1.0.2/reldi_tokeniser.egg-info/PKG-INFO
--rw-rw-r--   0 luka      (1000) luka      (1000)      391 2022-06-28 12:30:03.000000 reldi-tokeniser-1.0.2/reldi_tokeniser.egg-info/SOURCES.txt
--rw-rw-r--   0 luka      (1000) luka      (1000)        1 2022-06-28 12:30:03.000000 reldi-tokeniser-1.0.2/reldi_tokeniser.egg-info/dependency_links.txt
--rw-rw-r--   0 luka      (1000) luka      (1000)       16 2022-06-28 12:30:03.000000 reldi-tokeniser-1.0.2/reldi_tokeniser.egg-info/top_level.txt
--rw-rw-r--   0 luka      (1000) luka      (1000)       38 2022-06-28 12:30:03.000000 reldi-tokeniser-1.0.2/setup.cfg
--rw-rw-r--   0 luka      (1000) luka      (1000)      714 2022-06-28 08:23:23.000000 reldi-tokeniser-1.0.2/setup.py
+drwxrwxr-x   0 luka      (1000) luka      (1000)        0 2023-07-27 11:07:27.637884 reldi-tokeniser-1.0.3/
+-rw-rw-r--   0 luka      (1000) luka      (1000)    11357 2023-07-24 12:23:28.000000 reldi-tokeniser-1.0.3/LICENSE
+-rw-rw-r--   0 luka      (1000) luka      (1000)     3900 2023-07-27 11:07:27.637884 reldi-tokeniser-1.0.3/PKG-INFO
+-rw-rw-r--   0 luka      (1000) luka      (1000)     3609 2023-07-24 12:23:28.000000 reldi-tokeniser-1.0.3/README.md
+drwxrwxr-x   0 luka      (1000) luka      (1000)        0 2023-07-27 11:07:27.637884 reldi-tokeniser-1.0.3/reldi_tokeniser/
+-rw-rw-r--   0 luka      (1000) luka      (1000)       28 2023-07-24 12:23:28.000000 reldi-tokeniser-1.0.3/reldi_tokeniser/__init__.py
+-rw-rw-r--   0 luka      (1000) luka      (1000)     2621 2023-07-24 12:23:28.000000 reldi-tokeniser-1.0.3/reldi_tokeniser/bg.abbrev
+-rw-rw-r--   0 luka      (1000) luka      (1000)      950 2023-07-24 12:23:28.000000 reldi-tokeniser-1.0.3/reldi_tokeniser/hr.abbrev
+-rw-rw-r--   0 luka      (1000) luka      (1000)     1743 2023-07-24 12:23:28.000000 reldi-tokeniser-1.0.3/reldi_tokeniser/mk.abbrev
+-rw-rw-r--   0 luka      (1000) luka      (1000)     2470 2023-07-24 12:23:28.000000 reldi-tokeniser-1.0.3/reldi_tokeniser/punct
+-rw-rw-r--   0 luka      (1000) luka      (1000)     1573 2023-07-24 12:23:28.000000 reldi-tokeniser-1.0.3/reldi_tokeniser/sl.abbrev
+-rw-rw-r--   0 luka      (1000) luka      (1000)     2052 2023-07-24 12:23:28.000000 reldi-tokeniser-1.0.3/reldi_tokeniser/sr.abbrev
+-rwxrwxr-x   0 luka      (1000) luka      (1000)    14660 2023-07-27 10:07:30.000000 reldi-tokeniser-1.0.3/reldi_tokeniser/tokeniser.py
+drwxrwxr-x   0 luka      (1000) luka      (1000)        0 2023-07-27 11:07:27.637884 reldi-tokeniser-1.0.3/reldi_tokeniser.egg-info/
+-rw-rw-r--   0 luka      (1000) luka      (1000)     3900 2023-07-27 11:07:27.000000 reldi-tokeniser-1.0.3/reldi_tokeniser.egg-info/PKG-INFO
+-rw-rw-r--   0 luka      (1000) luka      (1000)      391 2023-07-27 11:07:27.000000 reldi-tokeniser-1.0.3/reldi_tokeniser.egg-info/SOURCES.txt
+-rw-rw-r--   0 luka      (1000) luka      (1000)        1 2023-07-27 11:07:27.000000 reldi-tokeniser-1.0.3/reldi_tokeniser.egg-info/dependency_links.txt
+-rw-rw-r--   0 luka      (1000) luka      (1000)       16 2023-07-27 11:07:27.000000 reldi-tokeniser-1.0.3/reldi_tokeniser.egg-info/top_level.txt
+-rw-rw-r--   0 luka      (1000) luka      (1000)       38 2023-07-27 11:07:27.637884 reldi-tokeniser-1.0.3/setup.cfg
+-rw-rw-r--   0 luka      (1000) luka      (1000)      714 2023-07-27 10:48:43.000000 reldi-tokeniser-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `reldi-tokeniser-1.0.2/LICENSE` & `reldi-tokeniser-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reldi-tokeniser-1.0.2/PKG-INFO` & `reldi-tokeniser-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reldi-tokeniser
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sentence splitting and tokenization for South Slavic languages
 Home-page: https://www.github.com/clarinsi/reldi-tokeniser
 Author: CLARIN.SI
 License: apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `reldi-tokeniser-1.0.2/README.md` & `reldi-tokeniser-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `reldi-tokeniser-1.0.2/reldi_tokeniser/bg.abbrev` & `reldi-tokeniser-1.0.3/reldi_tokeniser/bg.abbrev`

 * *Files identical despite different names*

### Comparing `reldi-tokeniser-1.0.2/reldi_tokeniser/hr.abbrev` & `reldi-tokeniser-1.0.3/reldi_tokeniser/hr.abbrev`

 * *Files identical despite different names*

### Comparing `reldi-tokeniser-1.0.2/reldi_tokeniser/mk.abbrev` & `reldi-tokeniser-1.0.3/reldi_tokeniser/mk.abbrev`

 * *Files identical despite different names*

### Comparing `reldi-tokeniser-1.0.2/reldi_tokeniser/punct` & `reldi-tokeniser-1.0.3/reldi_tokeniser/punct`

 * *Files identical despite different names*

### Comparing `reldi-tokeniser-1.0.2/reldi_tokeniser/sl.abbrev` & `reldi-tokeniser-1.0.3/reldi_tokeniser/sl.abbrev`

 * *Files identical despite different names*

### Comparing `reldi-tokeniser-1.0.2/reldi_tokeniser/sr.abbrev` & `reldi-tokeniser-1.0.3/reldi_tokeniser/sr.abbrev`

 * *Files identical despite different names*

### Comparing `reldi-tokeniser-1.0.2/reldi_tokeniser/tokeniser.py` & `reldi-tokeniser-1.0.3/reldi_tokeniser/tokeniser.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
     'arrow':r'<[-]+|[-]+>',
     'dot':r'[.!?/]{2,}',
     'space':r'\s+',
     'other':r'(.)\1*',
     'order':('abbrev','num','url','htmlesc','tag','mail','mention','hashtag','emoticon','word','arrow','dot','space','other')
   },
 
-
   'bg':{
     'abbrev':r'|'.join(abbrevs['bg']['B']+abbrevs['bg']['N']+abbrevs['bg']['S']),
     'num':num,
     'url':url,
     'htmlesc':r'&#?[a-z0-9]+;',
     'tag':r'</?[a-z][\w:]*>|<[a-z][\w:]*/?>',
     'mail':r'[\w.-]+@\w+(?:[.-]\w+)+',
@@ -233,15 +232,15 @@
       'tag': tag
     }
     if args['document']:
       args['conllu'] = True
     if args['tag']:
       args['conllu'] = True
     self.args = args
-    lang = args['lang']
+    self.lang = args['lang']
     self.mode = 'standard'
     if args['nonstandard']:
       self.mode = 'nonstandard'
     self.tokenizer = generate_tokenizer(lang)
     if args['tag']:
       self.punct_re = re.compile(r'^[' + re.escape(punct) + ']+$', re.UNICODE)
       self.symb_re = re.compile(r'^[' + re.escape('#%&<>+=°x÷$@µ©™®§') + ']+$')
@@ -394,15 +393,15 @@
         if line.startswith('# newdoc id = '):
           par_id = 0
           if mode == 'object':
             pre_metadata += line
           else:
             self.output.write(line)
           continue
-      out = self.represent_tomaz(process[self.mode](self.tokenizer, line, lang), par_id, mode)
+      out = self.represent_tomaz(process[self.mode](self.tokenizer, line, self.lang), par_id, mode)
       if mode == 'object':
         if pre_metadata and len(out) > 0:
           out[0]['metadata'] = pre_metadata + out[0]['metadata']
         document.append(out)
       else:
         self.output.write(out)
       if self.args['bert']:
```

### Comparing `reldi-tokeniser-1.0.2/reldi_tokeniser.egg-info/PKG-INFO` & `reldi-tokeniser-1.0.3/reldi_tokeniser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reldi-tokeniser
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sentence splitting and tokenization for South Slavic languages
 Home-page: https://www.github.com/clarinsi/reldi-tokeniser
 Author: CLARIN.SI
 License: apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `reldi-tokeniser-1.0.2/setup.py` & `reldi-tokeniser-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(long_description=long_description,
       long_description_content_type="text/markdown",
       name='reldi-tokeniser',
-      version='1.0.2',
+      version='1.0.3',
       licence='apache-2.0',
       description='Sentence splitting and tokenization for South Slavic languages',
       author='CLARIN.SI',
       url='https://www.github.com/clarinsi/reldi-tokeniser',
       packages=['reldi_tokeniser'],
       package_data={'reldi_tokeniser': ['*.abbrev', 'punct']}
      )
```

