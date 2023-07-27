# Comparing `tmp/peptacular-0.1.0.tar.gz` & `tmp/peptacular-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptacular-0.1.0.tar", last modified: Mon Jul 17 22:50:49 2023, max compression
+gzip compressed data, was "peptacular-0.2.0.tar", last modified: Thu Jul 27 18:33:55 2023, max compression
```

## Comparing `peptacular-0.1.0.tar` & `peptacular-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:50:49.383376 peptacular-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-17 22:50:36.000000 peptacular-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-17 22:50:49.383376 peptacular-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 22:50:36.000000 peptacular-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-17 22:50:36.000000 peptacular-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:50:49.383376 peptacular-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-17 22:50:36.000000 peptacular-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:50:49.379376 peptacular-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:50:49.383376 peptacular-0.1.0/src/peptacular/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    13130 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/spans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:50:49.383376 peptacular-0.1.0/src/peptacular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-17 22:50:49.000000 peptacular-0.1.0/src/peptacular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-17 22:50:49.000000 peptacular-0.1.0/src/peptacular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:50:49.000000 peptacular-0.1.0/src/peptacular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 22:50:49.000000 peptacular-0.1.0/src/peptacular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 22:50:49.000000 peptacular-0.1.0/src/peptacular.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:50:49.383376 peptacular-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-17 22:50:36.000000 peptacular-0.1.0/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-07-17 22:50:36.000000 peptacular-0.1.0/tests/test_peptide.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-17 22:50:36.000000 peptacular-0.1.0/tests/test_protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-17 22:50:36.000000 peptacular-0.1.0/tests/test_spans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:33:55.749860 peptacular-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 18:33:45.000000 peptacular-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-27 18:33:55.745860 peptacular-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-27 18:33:45.000000 peptacular-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 18:33:45.000000 peptacular-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 18:33:55.749860 peptacular-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 18:33:45.000000 peptacular-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:33:55.745860 peptacular-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:33:55.745860 peptacular-0.2.0/src/peptacular/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/fragmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20388 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-07-27 18:33:45.000000 peptacular-0.2.0/src/peptacular/spans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:33:55.745860 peptacular-0.2.0/src/peptacular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-27 18:33:55.000000 peptacular-0.2.0/src/peptacular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-27 18:33:55.000000 peptacular-0.2.0/src/peptacular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:33:55.000000 peptacular-0.2.0/src/peptacular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 18:33:55.000000 peptacular-0.2.0/src/peptacular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 18:33:55.000000 peptacular-0.2.0/src/peptacular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:33:55.745860 peptacular-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-27 18:33:45.000000 peptacular-0.2.0/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-27 18:33:45.000000 peptacular-0.2.0/tests/test_protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-27 18:33:45.000000 peptacular-0.2.0/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-27 18:33:45.000000 peptacular-0.2.0/tests/test_spans.py
```

### Comparing `peptacular-0.1.0/LICENSE` & `peptacular-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peptacular-0.1.0/PKG-INFO` & `peptacular-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.1.0
+Version: 0.2.0
 Summary: Utility package for handling peptide and protein sequences
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `peptacular-0.1.0/README.md` & `peptacular-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `peptacular-0.1.0/pyproject.toml` & `peptacular-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peptacular-0.1.0/src/peptacular/constants.py` & `peptacular-0.2.0/src/peptacular/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,15 +110,14 @@
     'U': 150.0319,
     'R': 156.1875,
     'Y': 163.1760,
     'W': 186.2132,
     'O': 237.2982
 }
 
-
 UWPR_AVERAGE_AA_MASSES = {
     'G': 57.05132,
     'A': 71.0779,
     'S': 87.0773,
     'P': 97.11518,
     'V': 99.13106,
     'T': 101.10388,
@@ -137,50 +136,49 @@
     'U': 150.3079,
     'R': 156.18568,
     'Y': 163.17326,
     'W': 186.2099,
     'O': 237.29816
 }
 
-
 PROTEASES = {'arg-c': 'R',
- 'asp-n': '\\w(?=D)',
- 'bnps-skatole': 'W',
- 'caspase 1': '(?<=[FWYL]\\w[HAT])D(?=[^PEDQKR])',
- 'caspase 2': '(?<=DVA)D(?=[^PEDQKR])',
- 'caspase 3': '(?<=DMQ)D(?=[^PEDQKR])',
- 'caspase 4': '(?<=LEV)D(?=[^PEDQKR])',
- 'caspase 5': '(?<=[LW]EH)D',
- 'caspase 6': '(?<=VE[HI])D(?=[^PEDQKR])',
- 'caspase 7': '(?<=DEV)D(?=[^PEDQKR])',
- 'caspase 8': '(?<=[IL]ET)D(?=[^PEDQKR])',
- 'caspase 9': '(?<=LEH)D',
- 'caspase 10': '(?<=IEA)D',
- 'chymotrypsin high specificity': '([FY](?=[^P]))|(W(?=[^MP]))',
- 'chymotrypsin low specificity': '([FLY](?=[^P]))|(W(?=[^MP]))|(M(?=[^PY]))|(H(?=[^DMPW]))',
- 'chymotrypsin': '([FLY](?=[^P]))|(W(?=[^MP]))|(M(?=[^PY]))|(H(?=[^DMPW]))',
- 'clostripain': 'R',
- 'cnbr': 'M',
- 'enterokinase': '(?<=[DE]{3})K',
- 'factor xa': '(?<=[AFGILTVM][DE]G)R',
- 'formic acid': 'D',
- 'glutamyl endopeptidase': 'E',
- 'glu-c': 'E',
- 'granzyme b': '(?<=IEP)D',
- 'hydroxylamine': 'N(?=G)',
- 'iodosobenzoic acid': 'W',
- 'lys-c': 'K',
- 'lys-n': '\\w(?=K)',
- 'ntcb': '\\w(?=C)',
- 'pepsin ph1.3': '((?<=[^HKR][^P])[^R](?=[FL][^P]))|((?<=[^HKR][^P])[FL](?=\\w[^P]))',
- 'pepsin ph2.0': '((?<=[^HKR][^P])[^R](?=[FLWY][^P]))|((?<=[^HKR][^P])[FLWY](?=\\w[^P]))',
- 'proline endopeptidase': '(?<=[HKR])P(?=[^P])',
- 'proteinase k': '[AEFILTVWY]',
- 'staphylococcal peptidase i': '(?<=[^E])E',
- 'thermolysin': '[^DE](?=[AFILMV])',
- 'thrombin': '((?<=G)R(?=G))|((?<=[AFGILTVM][AFGILTVWA]P)R(?=[^DE][^DE]))',
- 'trypsin_full': '([KR](?=[^P]))|((?<=W)K(?=P))|((?<=M)R(?=P))',
- 'trypsin_exception': '((?<=[CD])K(?=D))|((?<=C)K(?=[HY]))|((?<=C)R(?=K))|((?<=R)R(?=[HR]))',
- 'trypsin': '([KR](?=[^P]))',
- 'trypsin/P': '([KR])',
- 'non-specific': '()',
- 'no-cleave': '_'}
+             'asp-n': '\\w(?=D)',
+             'bnps-skatole': 'W',
+             'caspase 1': '(?<=[FWYL]\\w[HAT])D(?=[^PEDQKR])',
+             'caspase 2': '(?<=DVA)D(?=[^PEDQKR])',
+             'caspase 3': '(?<=DMQ)D(?=[^PEDQKR])',
+             'caspase 4': '(?<=LEV)D(?=[^PEDQKR])',
+             'caspase 5': '(?<=[LW]EH)D',
+             'caspase 6': '(?<=VE[HI])D(?=[^PEDQKR])',
+             'caspase 7': '(?<=DEV)D(?=[^PEDQKR])',
+             'caspase 8': '(?<=[IL]ET)D(?=[^PEDQKR])',
+             'caspase 9': '(?<=LEH)D',
+             'caspase 10': '(?<=IEA)D',
+             'chymotrypsin high specificity': '([FY](?=[^P]))|(W(?=[^MP]))',
+             'chymotrypsin low specificity': '([FLY](?=[^P]))|(W(?=[^MP]))|(M(?=[^PY]))|(H(?=[^DMPW]))',
+             'chymotrypsin': '([FLY](?=[^P]))|(W(?=[^MP]))|(M(?=[^PY]))|(H(?=[^DMPW]))',
+             'clostripain': 'R',
+             'cnbr': 'M',
+             'enterokinase': '(?<=[DE]{3})K',
+             'factor xa': '(?<=[AFGILTVM][DE]G)R',
+             'formic acid': 'D',
+             'glutamyl endopeptidase': 'E',
+             'glu-c': 'E',
+             'granzyme b': '(?<=IEP)D',
+             'hydroxylamine': 'N(?=G)',
+             'iodosobenzoic acid': 'W',
+             'lys-c': 'K',
+             'lys-n': '\\w(?=K)',
+             'ntcb': '\\w(?=C)',
+             'pepsin ph1.3': '((?<=[^HKR][^P])[^R](?=[FL][^P]))|((?<=[^HKR][^P])[FL](?=\\w[^P]))',
+             'pepsin ph2.0': '((?<=[^HKR][^P])[^R](?=[FLWY][^P]))|((?<=[^HKR][^P])[FLWY](?=\\w[^P]))',
+             'proline endopeptidase': '(?<=[HKR])P(?=[^P])',
+             'proteinase k': '[AEFILTVWY]',
+             'staphylococcal peptidase i': '(?<=[^E])E',
+             'thermolysin': '[^DE](?=[AFILMV])',
+             'thrombin': '((?<=G)R(?=G))|((?<=[AFGILTVM][AFGILTVWA]P)R(?=[^DE][^DE]))',
+             'trypsin_full': '([KR](?=[^P]))|((?<=W)K(?=P))|((?<=M)R(?=P))',
+             'trypsin_exception': '((?<=[CD])K(?=D))|((?<=C)K(?=[HY]))|((?<=C)R(?=K))|((?<=R)R(?=[HR]))',
+             'trypsin': '([KR](?=[^P]))',
+             'trypsin/P': '([KR])',
+             'non-specific': '()',
+             'no-cleave': '_'}
```

### Comparing `peptacular-0.1.0/src/peptacular/mass.py` & `peptacular-0.2.0/src/peptacular/mass.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,62 @@
+from typing import List
+
 import numpy as np
 
 from .constants import *
 from peptacular.sequence import parse_modified_sequence, strip_modifications, sequence_generator, \
     identify_cleavage_sites
 
 
+# TODO: Remove numpy dependency and separate index functions into separate project
+
+
+def filter_by_mass(sequences: list[str], min_mass: float = None, max_mass: float = None) -> List[str]:
+    """
+    Filters a list of sequences by mass, returning only those that fall within the specified range.
+
+    Args:
+        sequences (list[str]): A list of sequences to be filtered.
+        min_mass (float): Minimum mass of the returned sequences.
+        max_mass (float): Maximum mass of the returned sequences.
+
+    Returns:
+        list[str]: A list of sequences that fall within the specified mass range.
+    """
+
+    min_mass = min_mass or 0
+    max_mass = max_mass or float('inf')
+
+    return [sequence for sequence in sequences if min_mass <= calculate_mass(sequence) <= max_mass]
+
+
 def calculate_mass(sequence: str, charge=0, ion_type: str = 'y', monoisotopic=True) -> float:
     """
     Calculate the mass of a peptide sequence considering possible modifications, charge and ion type.
 
     Args:
         sequence (str): Peptide sequence, possibly including modifications.
         charge (int, optional): Peptide charge. Default is 0.
         ion_type (str, optional): Ion type ('a', 'b', 'c', 'x', 'y', 'z'). Default is 'y'.
         monoisotopic (bool, optional): If true, uses monoisotopic masses. Defaults to True.
 
     Returns:
         float: The calculated mass of the peptide sequence.
     """
     # Select mass set based on monoisotopic flag
-    atomic_masses, aa_masses = (MONO_ISOTOPIC_ATOMIC_MASSES, MONO_ISOTOPIC_AA_MASSES) if monoisotopic else (AVERAGE_ATOMIC_MASSES, AVERAGE_AA_MASSES)
+    atomic_masses, aa_masses = (MONO_ISOTOPIC_ATOMIC_MASSES, MONO_ISOTOPIC_AA_MASSES) if monoisotopic else \
+        (AVERAGE_ATOMIC_MASSES, AVERAGE_AA_MASSES)
 
     # Parse modifications and strip them from sequence
     mods = parse_modified_sequence(sequence)
     stripped_sequence = strip_modifications(sequence)
 
     # Calculate mass
-    mass = sum(aa_masses[aa] for aa in stripped_sequence) + sum(float(value) for value in mods.values()) + (charge * atomic_masses['PROTON'])
+    mass = sum(aa_masses[aa] for aa in stripped_sequence) + sum(float(value) for value in mods.values()) + \
+        (charge * atomic_masses['PROTON'])
 
     # Adjust mass based on ion type
     ion_adjustments = {
         'a': -(atomic_masses['CARBON'] + atomic_masses['OXYGEN']),
         'c': atomic_masses['HYDROGEN'] * 3 + atomic_masses['NITROGEN'],
         'x': atomic_masses['CARBON'] + atomic_masses['OXYGEN'] * 2,
         'y': atomic_masses['HYDROGEN'] * 2 + atomic_masses['OXYGEN'],
```

### Comparing `peptacular-0.1.0/src/peptacular/protein.py` & `peptacular-0.2.0/src/peptacular/protein.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.1.0/src/peptacular/sequence.py` & `peptacular-0.2.0/src/peptacular/sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import re
 from copy import deepcopy
-from typing import Dict, List, Any
+from typing import Dict, List, Any, Union, Generator
 
 import regex as reg
 
 from .constants import PROTEASES
 from .spans import span_to_sequence, build_spans, build_non_enzymatic_spans, build_left_semi_spans, \
     build_right_semi_spans
 
 
+# TODO: Figure out how to specify modifications: either dict[int, str] or dict[int, str]?
+
+
 def _are_parentheses_balanced(text):
     """
     Check if parentheses in the given text are balanced or not.
 
     The function uses a stack data structure to ensure each opening parenthesis '('
     has a corresponding closing parenthesis ')' and vice versa.
 
@@ -83,15 +86,15 @@
                         of the modified amino acid.
 
     Raises:
         ValueError: If the sequence contains unmatched parentheses indicating incorrect
                     modification notation.
 
     Example:
-        >>> parse_modified_sequence('PEP(Phospho)TIDEK')
+        >>> parse_modified_sequence('PEP(Phospho)TIDE')
         {3: 'Phospho'}
     """
 
     # Check parentheses balance
     if not _are_parentheses_balanced(sequence):
         raise ValueError(f'Incorrect modification notation in peptide sequence : {sequence}!')
 
@@ -128,16 +131,16 @@
     Returns:
         str: The peptide sequence with the specified modifications.
 
     Raises:
         ValueError: If an index in modifications is invalid for the sequence.
 
     Example:
-        >>> create_modified_sequence('PEPTIDEK', {3: 5.0})
-        'PEP(5.0)TIDEK'
+        >>> create_modified_sequence('PEPTIDE', {3: 5.0})
+        'PEP(5.0)TIDE'
     """
 
     modified_sequence = []
     prev_index = 0
 
     # Sort the modifications by index in descending order
     for i, mod in sorted(modifications.items()):
@@ -206,16 +209,14 @@
         set: A list of right subsequences of the input sequence.
     """
 
     spans = build_right_semi_spans((0, len(sequence), 0), min_len, max_len)
     return [span_to_sequence(sequence, span) for span in spans]
 
 
-from typing import List
-
 def get_semi_sequences(sequence: str, min_len: int = None, max_len: int = None) -> List[str]:
     """
     Generate a list of all semi-enzymatic amino acid sequences of a given string sequence.
 
     Args:
         sequence (str): A string representing the protein sequence.
         min_len (int, optional): The minimum length of the semi-enzymatic sequence. Default is None.
@@ -255,15 +256,16 @@
         enzyme_regex (str): The enzyme regular expression for identifying cleavage sites.
         missed_cleavages (int): The maximum number of missed cleavages.
         semi (bool): Whether the sequence includes semi enzymatic peptides.
         min_len (int, optional): The minimum length of the enzymatic sequence. Default is None.
         max_len (int, optional): The maximum length of the enzymatic sequence. Default is None.
 
     Returns:
-        List[str]: A list of enzymatic sequences within the defined length bounds and satisfying the enzyme cleavage rules.
+        List[str]: A list of enzymatic sequences within the defined length bounds and satisfying the enzyme cleavage
+                   rules.
     """
 
     cleavage_sites = identify_cleavage_sites(sequence, enzyme_regex)
     spans = build_spans(len(sequence), cleavage_sites, missed_cleavages, min_len, max_len, semi)
     return [span_to_sequence(sequence, span) for span in spans]
 
 
@@ -338,15 +340,15 @@
 
     original_mods = parse_modified_sequence(sequence)
     stripped_sequence = strip_modifications(sequence)
     mods = rec_mod_builder(mod_map, stripped_sequence, 0, original_mods, max_mods + len(original_mods))
     return [create_modified_sequence(stripped_sequence, mod) for mod in mods]
 
 
-def sequence_generator(sequence: str, forward: bool):
+def sequence_generator(sequence: str, forward: bool) -> Generator[str, None, None]:
     """
     Generates amino acid sequences either from the front or the back.
 
     Args:
         sequence (str): The initial amino acid sequence.
         forward (bool): If True, start generating from the front; else, start from the back.
 
@@ -355,15 +357,15 @@
     """
     if forward:
         return _sequence_generator_front(sequence)
     else:
         return _sequence_generator_back(sequence)
 
 
-def _sequence_generator_back(sequence: str):
+def _sequence_generator_back(sequence: str) -> Generator[str, None, None]:
     """
     Generates amino acid sequences starting from the back of the sequence.
 
     Args:
         sequence (str): The initial amino acid sequence.
 
     Yields:
@@ -382,33 +384,35 @@
 
             index = start_of_modification
 
         yield sequence
         sequence = sequence[:index - 1]
 
 
-def _sequence_generator_front(sequence: str):
+def _sequence_generator_front(sequence: str) -> Generator[str, None, None]:
     """
     Generates sub-sequences starting from the front of the sequence.
 
     Args:
         sequence (str): The initial sequence.
 
     Yields:
         str: The sequence with the front amino acid (and modification) removed.
 
     Returns:
         None: If the modification ends at the end of the sequence.
     """
     if sequence[0] == '(':
         yield sequence
-
         end_of_modification = sequence.find(')')
         sequence = sequence[end_of_modification + 2:]
 
+        if sequence == '':
+            return None
+
         if sequence[0] == '(':
             end_of_modification = sequence.find(')')
             sequence = sequence[end_of_modification + 1:]
 
     while sequence:
         index = 0
         if len(sequence) > 1 and sequence[1] == '(':
@@ -419,15 +423,15 @@
 
             index = end_of_modification
 
         yield sequence
         sequence = sequence[index + 1:]
 
 
-def reverse_sequence(sequence: str):
+def reverse_sequence(sequence: str) -> str:
     """
     Reverses the sequence, while preserving the position of any modifications.
 
     Args:
         sequence (str): The amino acid sequence to be reversed.
 
     Returns:
@@ -435,15 +439,15 @@
     """
     mods = parse_modified_sequence(sequence)
     stripped_sequence = strip_modifications(sequence)[::-1]
     mod_reverse = {len(stripped_sequence) - 1 - k if k != -1 else -1: v for k, v in mods.items()}
     return create_modified_sequence(stripped_sequence, mod_reverse)
 
 
-def shift_sequence_left(sequence: str, shift: int):
+def shift_sequence_left(sequence: str, shift: int) -> str:
     """
     Shifts the sequence to the left by a given number of positions, while preserving the position of any modifications.
 
     Args:
         sequence (str): The sequence to be shifted.
         shift (int): The number of positions to shift the sequence to the left.
 
@@ -461,15 +465,15 @@
 
     # Shift mod positions, taking care to avoid negative keys
     shifted_sequence_mods = {(k - effective_shift) % seq_len if k != -1 else -1: v for k, v in mods.items()}
 
     return create_modified_sequence(shifted_stripped_sequence, shifted_sequence_mods)
 
 
-def identify_cleavage_sites(protein_sequence: str, enzyme_regex: str):
+def identify_cleavage_sites(protein_sequence: str, enzyme_regex: str) -> List[int]:
     """
     Identifies cleavage sites in a protein sequence, based on enzyme_regex pattern.
     If enzyme_regex is a key in PROTEASES, the corresponding regex pattern will be used.
     Cleavage sites are identified as the positions after matching residues.
 
     Args:
         protein_sequence (str): The protein sequence to be processed.
@@ -485,16 +489,17 @@
 
     enzyme_sites = []
     for site in reg.finditer(enzyme_regex, protein_sequence, overlapped=True):
         enzyme_sites.append(site.span(0))
     return [site[0] + 1 for site in enzyme_sites]
 
 
-def digest_sequence(sequence: str, enzyme_regex: str, missed_cleavages: int, min_len: int,
-                    max_len: int, semi: bool) -> List[str]:
+def digest_sequence(sequence: str, enzyme_regex: Union[List[str], str], missed_cleavages: int, min_len: int = None,
+                    max_len: int = None, semi: bool = False) -> List[
+    str]:
     """
     Digests a given amino acid sequence using specified enzyme rules and parameters, returning a list of peptides.
 
     The sequence is broken down into peptides based on the enzyme's cleavage rules, with the number of
     missed cleavages taken into account. The returned peptides are filtered based on minimum and maximum length.
 
     Args:
@@ -504,9 +509,49 @@
         min_len (int): Minimum length of the returned peptides.
         max_len (int): Maximum length of the returned peptides.
         semi (bool): Whether to include semi-digested peptides.
 
     Returns:
         List[str]: The list of digested peptides.
     """
-    spans = build_spans(len(sequence), identify_cleavage_sites(sequence, enzyme_regex), missed_cleavages, min_len, max_len, semi)
-    return [span_to_sequence(sequence, span) for span in spans]
+
+    if isinstance(enzyme_regex, str):
+        enzyme_regex = [enzyme_regex]
+
+    cleavage_sites = []
+    for regex in enzyme_regex:
+        cleavage_sites.extend(identify_cleavage_sites(sequence, regex))
+    cleavage_sites.sort()
+
+    spans = build_spans(len(sequence), cleavage_sites, missed_cleavages, min_len, max_len, semi)
+    sequences = [span_to_sequence(sequence, span) for span in spans]
+
+    return sequences
+
+
+def get_fragment_sequences(sequence: str, ion_type: str) -> List[str]:
+    """
+    Generate fragment sequences for a given peptide sequence based on the specified ion type
+
+    Args:
+        sequence (str): The peptide sequence.
+        ion_type (str): The type of ion for which fragments are generated.
+
+    Returns:
+        List[str]: The fragment sequences.
+    """
+
+    return list(sequence_generator(sequence, forward=ion_type in 'xyz'))
+
+
+def get_internal_fragment_sequences(sequence: str, ion_type:str) -> List[str]:
+    """
+    Generate internal fragment sequences for a given peptide sequence based on the specified ion type.
+
+    Args:
+        sequence (str): The peptide sequence.
+        ion_type (str): The type of ion for which internal fragments are generated.
+
+    Returns:
+        List[str]: The internal fragment sequences.
+    """
+    return list(sequence_generator(sequence, forward=ion_type not in 'xyz'))
```

### Comparing `peptacular-0.1.0/src/peptacular/spans.py` & `peptacular-0.2.0/src/peptacular/spans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from functools import wraps
 from typing import Tuple, List, Optional
 from itertools import groupby
 
+# TODO: Remove wrapper function? Its confusing and hurts readability
+
 
 def span_processing(func):
     """
     A decorator to enforce constraints on the span and min_len and max_len arguments of decorated functions.
     The span should be a tuple of length 3 and min_len and max_len should be None or an integer.
     """
 
@@ -175,15 +177,15 @@
 
     :param spans: A list of tuples, where each tuple represents a span with three integers (start, end, value).
     :param min_len: The minimum length of the left semi-spans.
     :param max_len: The maximum length of the left semi-spans.
     :return: A list of tuples representing all left semi-spans that are within the specified length range.
 
     This function groups the spans by the start position, for each group, it checks every span to see if its length
-    is at least the minimum length. If it is, it calculates the new maximum length, which is the smaller of the max_len
+    is at least the minimum length. If it is, it calculates the new maximum length, which is the smallest of the max_len
     and the span's length. Then it adds the left semi-spans to the list of semi-spans.
     """
     semi_spans = []
     spans = sorted(spans, key=lambda x: (x[0], -x[2]))
     for _, group in groupby(spans, key=lambda x: x[0]):
         group = list(group)
         for i, span in enumerate(group):
@@ -211,15 +213,15 @@
 
     :param spans: A list of tuples, where each tuple represents a span with three integers (start, end, value).
     :param min_len: The minimum length of the right semi-spans.
     :param max_len: The maximum length of the right semi-spans.
     :return: A list of tuples representing all right semi-spans that are within the specified length range.
 
     This function groups the spans by the start position, for each group, it checks every span to see if its length
-    is at least the minimum length. If it is, it calculates the new maximum length, which is the smaller of the max_len
+    is at least the minimum length. If it is, it calculates the new maximum length, which is the smallest of the max_len
     and the span's length. Then it adds the right semi-spans to the list of semi-spans.
     """
 
     semi_spans = []
     spans = sorted(spans, key=lambda x: (x[1], -x[2]))
     for _, group in groupby(spans, key=lambda x: x[1]):
         group = list(group)
```

### Comparing `peptacular-0.1.0/src/peptacular.egg-info/PKG-INFO` & `peptacular-0.2.0/src/peptacular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.1.0
+Version: 0.2.0
 Summary: Utility package for handling peptide and protein sequences
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `peptacular-0.1.0/tests/test_mass.py` & `peptacular-0.2.0/tests/test_mass.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,9 +64,10 @@
 
         for ion_type in 'abcxyz':
             frags = sorted(list(fragment_sequence(sequence='PET', types=(ion_type), max_charge=1)))
             pyteomics_frags = sorted(pyteomics[ion_type])
             for f, pf in zip(frags, pyteomics_frags):
                 self.assertAlmostEqual(f, pf, 6)
 
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `peptacular-0.1.0/tests/test_peptide.py` & `peptacular-0.2.0/tests/test_sequence.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from peptacular.sequence import parse_modified_sequence, create_modified_sequence, strip_modifications, \
     get_semi_sequences, get_non_enzymatic_sequences, convert_to_ms2_pip_style, \
     get_left_semi_sequences, get_right_semi_sequences, add_static_mods, add_variable_mods, sequence_generator, \
-    _sequence_generator_back, _sequence_generator_front
+    _sequence_generator_back, _sequence_generator_front, get_fragment_sequences, get_internal_fragment_sequences
 
 import unittest
 
 
 class TestPeptide(unittest.TestCase):
 
     def test_read_modified_peptide(self):
@@ -150,23 +150,24 @@
         self.assertEqual(set(get_non_enzymatic_sequences('PEPT', min_len=2, max_len=4)),
                          {'PE', 'EP', 'PT', 'PEP', 'EPT', 'PEPT'})
 
     def test_add_static_mod(self):
         self.assertEqual(add_static_mods('PEPCTIDE', {'C': 57.021464}), 'PEPC(57.021464)TIDE')
         self.assertEqual(add_static_mods('PEPC(57.021464)TIDE', {'C': 57.021464}), 'PEPC(57.021464)TIDE')
         self.assertEqual(add_static_mods('CPEPTIDEC', {'C': 57.021464}), 'C(57.021464)PEPTIDEC(57.021464)')
+        self.assertEqual(add_static_mods('P(1)EPCTIDE(1)', {'C': 57.021464}), 'P(1)EPC(57.021464)TIDE(1)')
 
     def test_add_variable_mod(self):
         self.assertEqual(set(add_variable_mods('PEPCTIDCE', {'C': 57.021464}, 2)), {'PEPC(57.021464)TIDCE',
                                                                                     'PEPC(57.021464)TIDC(57.021464)E',
                                                                                     'PEPCTIDC(57.021464)E',
                                                                                     'PEPCTIDCE'})
 
-        self.assertEqual(set(add_variable_mods('PEPC(20)TIDCE', {'C': 57.021464}, 2)), {'PEPC(20)TIDCE',
-                                                                                        'PEPC(20)TIDC(57.021464)E'})
+        self.assertEqual(set(add_variable_mods('P(1)EPC(20)TIDCE', {'C': 57.021464}, 2)), {'P(1)EPC(20)TIDCE',
+                                                                                        'P(1)EPC(20)TIDC(57.021464)E'})
 
     def test_peptide_generator(self):
         # Test forward generator
         generator = sequence_generator("A(P)C(P)G", True)
         self.assertEqual(next(generator), "A(P)C(P)G")
         self.assertEqual(next(generator), "C(P)G")
         self.assertEqual(next(generator), "G")
@@ -193,10 +194,54 @@
         generator = _sequence_generator_front("(P)A(P)C(P)G")
         self.assertEqual(next(generator), "(P)A(P)C(P)G")
         self.assertEqual(next(generator), "C(P)G")
         self.assertEqual(next(generator), "G")
         with self.assertRaises(StopIteration):
             next(generator)
 
+    def test_get_fragment_sequences(self):
+        sequence = "PEPTIDE"
+
+        for ion_type in 'abc':
+            fragments = get_fragment_sequences(sequence, ion_type)
+            self.assertEqual(fragments, ['P', 'PE', 'PEP', 'PEPT', 'PEPTI', 'PEPTID', 'PEPTIDE'][::-1])
+
+        for ion_type in 'xyz':
+            fragments = get_fragment_sequences(sequence, ion_type)
+            self.assertEqual(fragments, ['E', 'DE', 'IDE', 'TIDE', 'PTIDE', 'EPTIDE', 'PEPTIDE'][::-1])
+
+    def test_get_internal_fragment_sequences(self):
+        sequence = "PEPTIDE"
+
+        for ion_type in 'xyz':
+            fragments = get_internal_fragment_sequences(sequence, ion_type)
+            self.assertEqual(fragments, ['P', 'PE', 'PEP', 'PEPT', 'PEPTI', 'PEPTID', 'PEPTIDE'][::-1])
+
+        for ion_type in 'abc':
+            fragments = get_internal_fragment_sequences(sequence, ion_type)
+            self.assertEqual(fragments, ['E', 'DE', 'IDE', 'TIDE', 'PTIDE', 'EPTIDE', 'PEPTIDE'][::-1])
+
+    def test_get_fragment_sequences_modified(self):
+        sequence = "(-10)PEP(2)TIDE(100)"
+
+        for ion_type in 'abc':
+            fragments = get_fragment_sequences(sequence, ion_type)
+            self.assertEqual(fragments, ['(-10)P', '(-10)PE', '(-10)PEP(2)', '(-10)PEP(2)T', '(-10)PEP(2)TI', '(-10)PEP(2)TID', '(-10)PEP(2)TIDE(100)'][::-1])
+
+        for ion_type in 'xyz':
+            fragments = get_fragment_sequences(sequence, ion_type)
+            self.assertEqual(fragments, ['E(100)', 'DE(100)', 'IDE(100)', 'TIDE(100)', 'P(2)TIDE(100)', 'EP(2)TIDE(100)', '(-10)PEP(2)TIDE(100)'][::-1])
+
+    def test_get_internal_fragment_sequences_modified(self):
+        sequence = "(-10)PEP(2)TIDE(100)"
+
+        for ion_type in 'xyz':
+            fragments = get_internal_fragment_sequences(sequence, ion_type)
+            self.assertEqual(fragments, ['(-10)P', '(-10)PE', '(-10)PEP(2)', '(-10)PEP(2)T', '(-10)PEP(2)TI', '(-10)PEP(2)TID', '(-10)PEP(2)TIDE(100)'][::-1])
+
+        for ion_type in 'abc':
+            fragments = get_internal_fragment_sequences(sequence, ion_type)
+            self.assertEqual(fragments, ['E(100)', 'DE(100)', 'IDE(100)', 'TIDE(100)', 'P(2)TIDE(100)', 'EP(2)TIDE(100)', '(-10)PEP(2)TIDE(100)'][::-1])
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `peptacular-0.1.0/tests/test_protein.py` & `peptacular-0.2.0/tests/test_protein.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.1.0/tests/test_spans.py` & `peptacular-0.2.0/tests/test_spans.py`

 * *Files identical despite different names*

