# Comparing `tmp/simple_icd_10_cm-1.1.2.tar.gz` & `tmp/simple_icd_10_cm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\simple_icd_10_cm-1.1.2.tar", last modified: Tue Sep 21 18:11:58 2021, max compression
+gzip compressed data, was "simple_icd_10_cm-1.2.0.tar", last modified: Thu Jul 27 20:19:04 2023, max compression
```

## Comparing `simple_icd_10_cm-1.1.2.tar` & `simple_icd_10_cm-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-09-21 18:11:58.923921 simple_icd_10_cm-1.1.2/
--rw-rw-rw-   0        0        0     1094 2021-05-30 17:33:14.000000 simple_icd_10_cm-1.1.2/LICENSE
--rw-rw-rw-   0        0        0    32044 2021-09-21 18:11:58.923131 simple_icd_10_cm-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    31457 2021-09-21 18:10:22.000000 simple_icd_10_cm-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2021-09-21 18:11:58.923921 simple_icd_10_cm-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      903 2021-09-21 18:11:06.000000 simple_icd_10_cm-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-21 18:11:58.662451 simple_icd_10_cm-1.1.2/simple_icd_10_cm/
--rw-rw-rw-   0        0        0       31 2021-07-05 17:09:18.000000 simple_icd_10_cm-1.1.2/simple_icd_10_cm/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-21 18:11:58.801643 simple_icd_10_cm-1.1.2/simple_icd_10_cm/data/
--rw-rw-rw-   0        0        0        0 2021-07-05 19:51:40.000000 simple_icd_10_cm-1.1.2/simple_icd_10_cm/data/__init__.py
--rw-rw-rw-   0        0        0 14261470 2021-05-28 19:44:37.000000 simple_icd_10_cm-1.1.2/simple_icd_10_cm/data/icd10cm-order-Jan-2021.txt
--rw-rw-rw-   0        0        0  9253467 2021-06-18 20:10:27.000000 simple_icd_10_cm-1.1.2/simple_icd_10_cm/data/icd10cm_tabular_2021.xml
--rw-rw-rw-   0        0        0    19739 2021-09-21 18:11:19.000000 simple_icd_10_cm-1.1.2/simple_icd_10_cm/simple_icd_10_cm.py
-drwxrwxrwx   0        0        0        0 2021-09-21 18:11:58.669433 simple_icd_10_cm-1.1.2/simple_icd_10_cm.egg-info/
--rw-rw-rw-   0        0        0    32044 2021-09-21 18:11:58.000000 simple_icd_10_cm-1.1.2/simple_icd_10_cm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2021-09-21 18:11:58.000000 simple_icd_10_cm-1.1.2/simple_icd_10_cm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-21 18:11:58.000000 simple_icd_10_cm-1.1.2/simple_icd_10_cm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2021-09-21 18:11:58.000000 simple_icd_10_cm-1.1.2/simple_icd_10_cm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 20:19:04.010991 simple_icd_10_cm-1.2.0/
+-rw-rw-rw-   0        0        0     1094 2021-05-30 17:33:14.000000 simple_icd_10_cm-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    32005 2023-07-27 20:19:04.010991 simple_icd_10_cm-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    31457 2021-09-21 18:10:22.000000 simple_icd_10_cm-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 20:19:04.010991 simple_icd_10_cm-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      905 2023-07-27 20:05:15.000000 simple_icd_10_cm-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:19:03.649953 simple_icd_10_cm-1.2.0/simple_icd_10_cm/
+-rw-rw-rw-   0        0        0       31 2021-07-05 17:09:18.000000 simple_icd_10_cm-1.2.0/simple_icd_10_cm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:19:04.010991 simple_icd_10_cm-1.2.0/simple_icd_10_cm/data/
+-rw-rw-rw-   0        0        0        0 2021-07-05 19:51:40.000000 simple_icd_10_cm-1.2.0/simple_icd_10_cm/data/__init__.py
+-rw-rw-rw-   0        0        0 14261470 2021-05-28 19:44:37.000000 simple_icd_10_cm-1.2.0/simple_icd_10_cm/data/icd10cm-order-Jan-2021.txt
+-rw-rw-rw-   0        0        0  9253467 2021-06-18 20:10:27.000000 simple_icd_10_cm-1.2.0/simple_icd_10_cm/data/icd10cm_tabular_2021.xml
+-rw-rw-rw-   0        0        0    20252 2023-07-27 20:16:29.000000 simple_icd_10_cm-1.2.0/simple_icd_10_cm/simple_icd_10_cm.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:19:03.681169 simple_icd_10_cm-1.2.0/simple_icd_10_cm.egg-info/
+-rw-rw-rw-   0        0        0    32005 2023-07-27 20:19:03.000000 simple_icd_10_cm-1.2.0/simple_icd_10_cm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-07-27 20:19:03.000000 simple_icd_10_cm-1.2.0/simple_icd_10_cm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 20:19:03.000000 simple_icd_10_cm-1.2.0/simple_icd_10_cm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-27 20:19:03.000000 simple_icd_10_cm-1.2.0/simple_icd_10_cm.egg-info/top_level.txt
```

### Comparing `simple_icd_10_cm-1.1.2/LICENSE` & `simple_icd_10_cm-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_icd_10_cm-1.1.2/PKG-INFO` & `simple_icd_10_cm-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: simple_icd_10_cm
-Version: 1.1.2
+Version: 1.2.0
 Summary: A simple python library for ICD-10-CM codes
 Home-page: https://github.com/StefanoTrv/simple_icd_10_CM
 Author: Stefano Travasci
 Author-email: stefanotravasci@gmail.com
-License: UNKNOWN
 Keywords: ICD-10-CM ICD-10 icd 10 CM codes clinical modification
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # simple_icd_10_cm
 A simple python library for ICD-10-CM codes
 
 ## Index
@@ -443,9 +441,7 @@
 Paypal: [![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/donate?hosted_button_id=9HMMFAZE248VN)
 
 Curecoin: BKxCWuWzsqtLzAvAjtpsHpJ7LqFHPubqft
 
 Bitcoin: bc1qjtnvzzgpsxz397l03vhrw8l30vl2p7fepmn5yy
 
 <sub>*let me know if your favorite donation method is not in this list*</sub>
-
-
```

### Comparing `simple_icd_10_cm-1.1.2/README.md` & `simple_icd_10_cm-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_icd_10_cm-1.1.2/setup.py` & `simple_icd_10_cm-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simple_icd_10_cm",
-    version="1.1.2",
+    version="1.2.0",
     author="Stefano Travasci",
     author_email="stefanotravasci@gmail.com",
     description="A simple python library for ICD-10-CM codes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/StefanoTrv/simple_icd_10_CM",
     packages=setuptools.find_packages(),
     package_dir={'simple_icd_10_cm': 'simple_icd_10_cm'},
     package_data={'simple_icd_10_cm': ['data/*']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3',
+    python_requires='>=3.9',
     keywords='ICD-10-CM ICD-10 icd 10 CM codes clinical modification',
 )
```

### Comparing `simple_icd_10_cm-1.1.2/simple_icd_10_cm/data/icd10cm-order-Jan-2021.txt` & `simple_icd_10_cm-1.2.0/simple_icd_10_cm/data/icd10cm-order-Jan-2021.txt`

 * *Files identical despite different names*

### Comparing `simple_icd_10_cm-1.1.2/simple_icd_10_cm/data/icd10cm_tabular_2021.xml` & `simple_icd_10_cm-1.2.0/simple_icd_10_cm/data/icd10cm_tabular_2021.xml`

 * *Files identical despite different names*

### Comparing `simple_icd_10_cm-1.1.2/simple_icd_10_cm/simple_icd_10_cm.py` & `simple_icd_10_cm-1.2.0/simple_icd_10_cm/simple_icd_10_cm.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
     import importlib.resources as pkg_resources
 except ImportError:
     # Try backported to PY<37 `importlib_resources`.
     import importlib_resources as pkg_resources
 
 from . import data  # relative-import the "package" containing the data
 
-chapter_list = []
+chapter_list: list["_CodeTree"] = []
 
-code_to_node = {}
+code_to_node: dict[str, "_CodeTree"] = {}
 
-all_codes_list = []
+all_codes_list: list[str] = []
 
-all_codes_list_no_dots = []
+all_codes_list_no_dots: list[str] = []
 
-code_to_index_dictionary = {}
+code_to_index_dictionary: dict[str, int] = {}
 
 class _CodeTree:
     def __init__(self, tree, parent = None, seven_chr_def_ancestor = None, seven_chr_note_ancestor = None, use_additional_code_ancestor = None, code_first_ancestor = None):
         #initialize all the values
         self.name = ""
         self.description = ""
         self.type = ""
@@ -149,182 +149,182 @@
     if len(code)<4 or code[3]==".":
         return code
     elif code[:3]+"."+code[3:] in code_to_node:
         return code[:3]+"."+code[3:]
     else:
         return code
 
-def is_valid_item(code):
+def is_valid_item(code: str) -> bool:
     return code in code_to_node or len(code)>=4 and code[:3]+"."+code[3:] in code_to_node
 
-def is_chapter(code):
+def is_chapter(code: str) -> bool:
     code = _add_dot_to_code(code)
     if code in code_to_node:
         return code_to_node[code].type=="chapter"
     else:
         return False
 
-def is_block(code):
+def is_block(code: str) -> bool:
     code = _add_dot_to_code(code)
     if code in code_to_node:
         return code_to_node[code].type=="section" or code_to_node[code].parent!=None and code_to_node[code].parent.name==code #second half of the or is for sections containing a single category
     else:
         return False
 
-def is_category(code):
+def is_category(code: str) -> bool:
     code = _add_dot_to_code(code)
     if code in code_to_node:
         return code_to_node[code].type=="category"
     else:
         return False
 
-def is_subcategory(code, include_extended_subcategories=True):
+def is_subcategory(code: str, include_extended_subcategories=True) -> bool:
     code = _add_dot_to_code(code)
     if code in code_to_node:
         return code_to_node[code].type=="subcategory" or code_to_node[code].type=="extended subcategory" and include_extended_subcategories
     else:
         return False
 
-def is_extended_subcategory(code):
+def is_extended_subcategory(code: str) -> bool:
     code = _add_dot_to_code(code)
     if code in code_to_node:
         return code_to_node[code].type=="extended subcategory"
     else:
         return False
     
-def is_category_or_subcategory(code):
+def is_category_or_subcategory(code: str) -> bool:
     return is_subcategory(code) or is_category(code)
 
-def is_chapter_or_block(code):
+def is_chapter_or_block(code: str) -> bool:
     return is_block(code) or is_chapter(code)
 
-def get_description(code, prioritize_blocks=False):
+def get_description(code: str, prioritize_blocks=False) -> str:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         return node.parent.description
     else:
         return node.description
 
-def get_excludes1(code, prioritize_blocks=False):
+def get_excludes1(code: str, prioritize_blocks=False) -> list[str]:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         return node.parent.excludes1.copy()
     else:
         return node.excludes1.copy()
 
-def get_excludes2(code, prioritize_blocks=False):
+def get_excludes2(code: str, prioritize_blocks=False) -> list[str]:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         return node.parent.excludes2.copy()
     else:
         return node.excludes2.copy()
 
-def get_includes(code, prioritize_blocks=False):
+def get_includes(code: str, prioritize_blocks=False) -> list[str]:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         return node.parent.includes.copy()
     else:
         return node.includes.copy()
 
-def get_inclusion_term(code, prioritize_blocks=False):
+def get_inclusion_term(code: str, prioritize_blocks=False) -> list[str]:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         return node.parent.inclusion_term.copy()
     else:
         return node.inclusion_term.copy()
 
-def get_seven_chr_def(code, search_in_ancestors=False, prioritize_blocks=False):
+def get_seven_chr_def(code: str, search_in_ancestors=False, prioritize_blocks=False) -> dict[str, str]:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     res = node.seven_chr_def.copy()
     if search_in_ancestors and len(res)==0 and node.seven_chr_def_ancestor!=None:
         return node.seven_chr_def_ancestor.seven_chr_def.copy()
     else:
         return res
 
-def get_seven_chr_note(code, search_in_ancestors=False, prioritize_blocks=False):
+def get_seven_chr_note(code: str, search_in_ancestors=False, prioritize_blocks=False) -> str:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     res = node.seven_chr_note
     if search_in_ancestors and res=="" and node.seven_chr_note_ancestor!=None:
         return node.seven_chr_note_ancestor.seven_chr_note
     else:
         return res
 
-def get_use_additional_code(code, search_in_ancestors=False, prioritize_blocks=False):
+def get_use_additional_code(code: str, search_in_ancestors=False, prioritize_blocks=False) -> str:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     res = node.use_additional_code
     if search_in_ancestors and res=="" and node.use_additional_code_ancestor!=None:
         return node.use_additional_code_ancestor.use_additional_code
     else:
         return res
 
-def get_code_first(code, search_in_ancestors=False, prioritize_blocks=False):
+def get_code_first(code: str, search_in_ancestors=False, prioritize_blocks=False) -> str:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     res = node.code_first
     if search_in_ancestors and res=="" and node.code_first_ancestor!=None:
         return node.code_first_ancestor.code_first
     else:
         return res
 
-def get_parent(code, prioritize_blocks=False):
+def get_parent(code: str, prioritize_blocks=False) -> str:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     if node.parent!=None:
         return node.parent.name
     else:
         return ""
 
-def get_children(code, prioritize_blocks=False):
+def get_children(code: str, prioritize_blocks=False) -> list[str]:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     res = []
     for child in node.children:
         res.append(child.name)
     return res
 
-def is_leaf(code, prioritize_blocks=False):
+def is_leaf(code: str, prioritize_blocks=False) -> bool:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     return len(node.children)==0
 
-def get_full_data(code, search_in_ancestors=False, prioritize_blocks=False):
+def get_full_data(code: str, search_in_ancestors=False, prioritize_blocks=False) -> str:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     str = "Name:\n"+node.name+"\nDescription:\n"+node.description
     if node.parent!=None:
@@ -363,65 +363,65 @@
         str = str + "\nChildren:\nNone--"
     else:
         str = str + "\nChildren:\n"
         for child in node.children:
             str = str + child.name + ", "
     return str[:-2]
 
-def get_ancestors(code, prioritize_blocks=False):
+def get_ancestors(code: str,prioritize_blocks=False) -> list[str]:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     result = []
     while node.parent != None:
         result.append(node.parent.name)
         node=node.parent
     return result
 
-def get_descendants(code, prioritize_blocks=False):
+def get_descendants(code: str,prioritize_blocks=False) -> list[str]:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(code)]
     if prioritize_blocks and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     result = []
     _add_children_to_list(node, result)
     return result
 
 def _add_children_to_list(node, list):
     for child in node.children:
         list.append(child.name)
         _add_children_to_list(child,list)
 
-def is_ancestor(a,b,prioritize_blocks_a=False,prioritize_blocks_b=False):
+def is_ancestor(a:str,b:str,prioritize_blocks_a=False,prioritize_blocks_b=False) -> bool:
     if not is_valid_item(a):
         raise ValueError("The code \""+a+"\" does not exist.")
     node = code_to_node[_add_dot_to_code(a)]
     if prioritize_blocks_a and node.parent!=None and node.parent.name==node.name:
         node = node.parent
     return a in get_ancestors(b, prioritize_blocks=prioritize_blocks_b) and (a!=b or prioritize_blocks_a)
 
-def is_descendant(a,b,prioritize_blocks_a=False,prioritize_blocks_b=False):
+def is_descendant(a:str,b:str,prioritize_blocks_a=False,prioritize_blocks_b=False) -> bool:
     return is_ancestor(b,a,prioritize_blocks_a=prioritize_blocks_b,prioritize_blocks_b=prioritize_blocks_a)
 
-def get_nearest_common_ancestor(a,b,prioritize_blocks_a=False,prioritize_blocks_b=False):
+def get_nearest_common_ancestor(a:str,b:str,prioritize_blocks_a=False,prioritize_blocks_b=False) -> str:
     anc_a = [_add_dot_to_code(a)] + get_ancestors(a, prioritize_blocks=prioritize_blocks_a)
     anc_b = [_add_dot_to_code(b)] + get_ancestors(b, prioritize_blocks=prioritize_blocks_b)
     if len(anc_b) > len(anc_a):
         temp = anc_a
         anc_a = anc_b
         anc_b = temp
     for anc in anc_a:
         if anc in anc_b:
             return anc
     return ""
 
-def get_all_codes(with_dots=True):
+def get_all_codes(with_dots=True) -> list[str]:
     if all_codes_list==[]:
         for chapter in chapter_list:
             _add_tree_to_list(chapter)
     if with_dots:
         return all_codes_list.copy()
     else:
         return all_codes_list_no_dots.copy()
@@ -431,15 +431,15 @@
     if(len(tree.name)>4 and tree.name[3]=="."):
         all_codes_list_no_dots.append(tree.name[:3]+tree.name[4:])
     else:
         all_codes_list_no_dots.append(tree.name)
     for child in tree.children:
         _add_tree_to_list(child)
 
-def get_index(code):
+def get_index(code: str) -> int:
     if not is_valid_item(code):
         raise ValueError("The code \""+code+"\" does not exist.")
     code = _add_dot_to_code(code)
     if all_codes_list==[]:
         for chapter in chapter_list:
             _add_tree_to_list(chapter)
     if code in code_to_index_dictionary:
@@ -449,18 +449,18 @@
         for c in all_codes_list:
             if c==code:
                 code_to_index_dictionary[code]=i
                 return i
             else:
                 i=i+1
 
-def remove_dot(code):
+def remove_dot(code: str) -> str:
     if all_codes_list==[]:
         for chapter in chapter_list:
             _add_tree_to_list(chapter)
     return all_codes_list_no_dots[get_index(code)]
 
-def add_dot(code):
+def add_dot(code: str) -> str:
     if all_codes_list==[]:
         for chapter in chapter_list:
             _add_tree_to_list(chapter)
     return all_codes_list[get_index(code)]
```

### Comparing `simple_icd_10_cm-1.1.2/simple_icd_10_cm.egg-info/PKG-INFO` & `simple_icd_10_cm-1.2.0/simple_icd_10_cm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: simple-icd-10-cm
-Version: 1.1.2
+Version: 1.2.0
 Summary: A simple python library for ICD-10-CM codes
 Home-page: https://github.com/StefanoTrv/simple_icd_10_CM
 Author: Stefano Travasci
 Author-email: stefanotravasci@gmail.com
-License: UNKNOWN
 Keywords: ICD-10-CM ICD-10 icd 10 CM codes clinical modification
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # simple_icd_10_cm
 A simple python library for ICD-10-CM codes
 
 ## Index
@@ -443,9 +441,7 @@
 Paypal: [![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif)](https://www.paypal.com/donate?hosted_button_id=9HMMFAZE248VN)
 
 Curecoin: BKxCWuWzsqtLzAvAjtpsHpJ7LqFHPubqft
 
 Bitcoin: bc1qjtnvzzgpsxz397l03vhrw8l30vl2p7fepmn5yy
 
 <sub>*let me know if your favorite donation method is not in this list*</sub>
-
-
```

