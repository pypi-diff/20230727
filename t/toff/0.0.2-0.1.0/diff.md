# Comparing `tmp/toff-0.0.2.tar.gz` & `tmp/toff-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toff-0.0.2.tar", last modified: Mon Mar 27 20:05:41 2023, max compression
+gzip compressed data, was "toff-0.1.0.tar", last modified: Thu Jul 27 13:30:20 2023, max compression
```

## Comparing `toff-0.0.2.tar` & `toff-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:05:41.977796 toff-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-27 20:05:26.000000 toff-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-03-27 20:05:41.977796 toff-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-03-27 20:05:26.000000 toff-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-27 20:05:41.977796 toff-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-27 20:05:26.000000 toff-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:05:41.973796 toff-0.0.2/toff/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-27 20:05:26.000000 toff-0.0.2/toff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-27 20:05:26.000000 toff-0.0.2/toff/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-27 20:05:26.000000 toff-0.0.2/toff/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14424 2023-03-27 20:05:26.000000 toff-0.0.2/toff/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:05:41.977796 toff-0.0.2/toff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:30:20.515086 toff-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 13:29:53.000000 toff-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-07-27 13:30:20.515086 toff-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-27 13:29:53.000000 toff-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-27 13:30:20.515086 toff-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 13:29:53.000000 toff-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:30:20.515086 toff-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-27 13:29:53.000000 toff-0.1.0/tests/test_small.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:30:20.515086 toff-0.1.0/toff/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-27 13:29:53.000000 toff-0.1.0/toff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-27 13:29:53.000000 toff-0.1.0/toff/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-27 13:29:53.000000 toff-0.1.0/toff/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18047 2023-07-27 13:29:53.000000 toff-0.1.0/toff/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:30:20.515086 toff-0.1.0/toff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-07-27 13:30:20.000000 toff-0.1.0/toff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-27 13:30:20.000000 toff-0.1.0/toff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:30:20.000000 toff-0.1.0/toff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 13:30:20.000000 toff-0.1.0/toff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 13:30:20.000000 toff-0.1.0/toff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 13:30:20.000000 toff-0.1.0/toff.egg-info/top_level.txt
```

### Comparing `toff-0.0.2/LICENSE` & `toff-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toff-0.0.2/PKG-INFO` & `toff-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toff
-Version: 0.0.2
+Version: 0.1.0
 Summary: toff is a python package to get topologies from the OpenFF initiative
 Home-page: https://github.com/ale94mleon/toff
 Author: Alejandro Martínez León
 Author-email: ale94mleon@gmail.com
 License: Apache License 2.0
 Project-URL: Discussions, https://github.com/ale94mleon/toff/discussions
 Project-URL: Documentation, https://toff.readthedocs.io/en/latest/
@@ -52,15 +52,19 @@
       - |license|
     * - **Downloads**
       - |downloads|
 
 Description
 -----------
 
-**TOFF** (Topologies from OpenFF) is a python package to get topologies from the OpenFF initiative. It was strongly inspired in this `Aniket's script <https://github.com/aniketsh/OpenFF/blob/82a2b5803e36b72f3525e3b8631cf256fbd8e35a/openff_topology.py>`__.
+**TOFF** (Topologies from OpenFF) is a python package initially developed to get topologies from the OpenFF initiative.
+It was strongly inspired in this `Aniket's script <https://github.com/aniketsh/OpenFF/blob/82a2b5803e36b72f3525e3b8631cf256fbd8e35a/openff_topology.py>`__.
+Since version **0.1.0** it is alos possible to get `GAFF <https://ambermd.org/antechamber/gaff.html>`__ and
+`Espaloma <https://docs.espaloma.org/en/latest/>`__ parameters by using **EspalomaTemplateGenerator** and **GAFFTemplateGenerator**
+from `openmmforcefields.generators <https://github.com/openmm/openmmforcefields/tree/main/openmmforcefields/generators>`__.
 
 
 You can try it out prior to any installation on `Binder <https://mybinder.org/v2/gh/ale94mleon/TOFF/HEAD?labpath=%2Fdocs%2Fnotebooks%2F>`__.
 
 Documentation
 -------------
```

### Comparing `toff-0.0.2/README.rst` & `toff-0.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,19 @@
       - |license|
     * - **Downloads**
       - |downloads|
 
 Description
 -----------
 
-**TOFF** (Topologies from OpenFF) is a python package to get topologies from the OpenFF initiative. It was strongly inspired in this `Aniket's script <https://github.com/aniketsh/OpenFF/blob/82a2b5803e36b72f3525e3b8631cf256fbd8e35a/openff_topology.py>`__.
+**TOFF** (Topologies from OpenFF) is a python package initially developed to get topologies from the OpenFF initiative.
+It was strongly inspired in this `Aniket's script <https://github.com/aniketsh/OpenFF/blob/82a2b5803e36b72f3525e3b8631cf256fbd8e35a/openff_topology.py>`__.
+Since version **0.1.0** it is alos possible to get `GAFF <https://ambermd.org/antechamber/gaff.html>`__ and
+`Espaloma <https://docs.espaloma.org/en/latest/>`__ parameters by using **EspalomaTemplateGenerator** and **GAFFTemplateGenerator**
+from `openmmforcefields.generators <https://github.com/openmm/openmmforcefields/tree/main/openmmforcefields/generators>`__.
 
 
 You can try it out prior to any installation on `Binder <https://mybinder.org/v2/gh/ale94mleon/TOFF/HEAD?labpath=%2Fdocs%2Fnotebooks%2F>`__.
 
 Documentation
 -------------
```

### Comparing `toff-0.0.2/setup.cfg` & `toff-0.1.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = toff
-version = attr: toff.__version__
+version = attr: toff._version.__version__
 author = Alejandro Martínez León
 author_email = ale94mleon@gmail.com
 description = toff is a python package to get topologies from the OpenFF initiative
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/ale94mleon/toff
 project_urls = 
@@ -37,14 +37,15 @@
 [options]
 packages = find:
 python_requires = >= 3.8, < 3.11
 include_package_data = True
 install_requires = 
 	pyyaml
 	parmed
+	rdkit
 
 [options.extras_require]
 test = 
 	pytest
 
 [options.entry_points]
 console_scripts =
```

### Comparing `toff-0.0.2/toff/_version.py` & `toff-0.1.0/toff/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 # We will use semantic version (major, minor, patch)
-__main_version_tuple__ = (0, 0, 2)
+__main_version_tuple__ = (0, 1, 0)
 __pre_version_tuple__ = None # or None or an empty tuple, the first char is alpha, beta, rc, etc...
 
 if __pre_version_tuple__:
     __version_tuple__ = tuple(list(__main_version_tuple__) + list(__pre_version_tuple__))
     __version__ = '.'.join([str(i) for i in __main_version_tuple__]) + f'{__pre_version_tuple__[0][0]}' + '.'.join([str(i) for i in __pre_version_tuple__[1:]])
 else:
     __version_tuple__ = __main_version_tuple__
```

### Comparing `toff-0.0.2/toff/cli.py` & `toff-0.1.0/toff/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         action='version',
         version=f"toff: {__version__}")
     args = parser.parse_args()
 
     print(f"You are using toff:{__version__}")
     with open(args.yaml_file, 'r') as c:
         Config = yaml.safe_load(c)
-    InitKwargs = ['force_field_code','ext_types','hmr_factor','overwrite','out_dir']
-    CallKwargs = ['input_mol','mol_resi_name','gen_conformer']
+    InitKwargs = ['force_field_code','ext_types','hmr_factor','overwrite', 'safe_naming_prefix', 'out_dir']
+    CallKwargs = ['input_mol','mol_resi_name']
 
     UserExtraNonValidKwargs = set(Config.keys()) - set(InitKwargs + CallKwargs)
     if 'input_mol' not in Config:
         raise RuntimeError("Not input_mol parameter provided in the configuration yaml file.")
     elif UserExtraNonValidKwargs:
         warnings.warn(f"Parameters: [{' '.join(UserExtraNonValidKwargs)}] is/are not valid and therefore discarded.")
```

### Comparing `toff-0.0.2/toff/utils.py` & `toff-0.1.0/toff/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 import numpy as np
 import os, warnings, tempfile
 from copy import deepcopy
 from rdkit import Chem
 from rdkit.Chem import AllChem
-from openff.toolkit.typing.engines.smirnoff import ForceField
+from openff.toolkit.typing.engines import smirnoff
 from openff.toolkit.topology import Molecule
-from openmm.app import PDBFile
+from openmm import app
 import parmed
 from typing import List, Iterable
 
 
 #This module was strongly inspired in https://github.com/aniketsh/OpenFF/blob/82a2b5803e36b72f3525e3b8631cf256fbd8e35a/openff_topology.py
 
 def confgen(mol: Chem.rdchem.Mol):
@@ -73,14 +73,15 @@
             mol = Chem.MolFromInchi(f.readline())
     elif extension == 'smi':
         with open(input_path_mol, 'r') as f:
             mol = Chem.MolFromSmiles(f.readline())
     elif extension == 'mol':
         mol = Chem.MolFromMolFile(input_path_mol)
     elif extension == 'sdf':
+        # TODO, check what happens if more than one conformation is provided. Maybe it is beneficial and this information is used by OpenFF
         mol = Chem.SDMolSupplier(input_path_mol)[0]
     elif extension == 'mol2':
         mol = Chem.MolFromMol2File(input_path_mol)
     # elif extension == 'pdb':
     #     mol = Chem.MolFromPDBFile(input_path_mol)
     else:
         raise NotImplementedError(f"Only: *.inchi, *.smi, *.mol, *.sdf *.mol2 are valid extensions. But *.{extension} was provided")
@@ -239,35 +240,112 @@
             atom.atom_type.name = f"{prefix}{atom.atom_type.name}"
         atom.type = atom.atom_type.name
     if inplace:
         return None
     else:
         return ligand_structure
 
+def generate_structure(rdkit_mol:Chem.rdchem.Mol, force_field_type:str = 'openff', force_field_code:str = None) -> parmed.structure.Structure:
+    """Generate a Structure object with the topology information from the specified force field.
+    OpenFF, GAFF and Espaloma flawors are supported
+
+    Parameters
+    ----------
+    rdkit_mol : Chem.rdchem.Mol
+        An RDKit molecule
+    force_field_type : str, optional
+        This is used to identify the force field. Valid options are openff, gaff, espaloma (case insensitive), by default 'openff'
+    force_field_code : str, optional
+        This is the code that represent the force field.  Any valid OpenFF, GAFF or Espaloma string representation.
+        Visit the `openff-forcefields <https://github.com/openforcefield/openff-forcefields>`__
+        and `openmmforcefields <https://github.com/openmm/openmmforcefields>` for
+        more information. Its default value will dynamically change depending on force_field_type as:
+        * openff -> openff_unconstrained-2.0.0.offxml
+        * gaff -> gaff-2.11
+        * espaloma -> espaloma-0.2.2
+
+    Returns
+    -------
+    parmed.structure.Structure
+        The Structure object with its corresponding force field parameters
+
+    Raises
+    ------
+    Exception
+        Invalid force_field_type.
+    """
+    force_field_code_default = {
+        'openff': 'openff_unconstrained-2.0.0.offxml',
+        'gaff': 'gaff-2.11',
+        'espaloma': 'espaloma-0.2.2'
+    }
+    # Check validity of force_field_type
+    force_field_type = force_field_type.lower()
+    if force_field_type in force_field_code_default:
+        # Update the internal default options if the user provided a force_field_code
+        if force_field_code:
+            force_field_code_default[force_field_type] = force_field_code
+    else:
+        raise Exception(f"{force_field_type = } is not valid. Choose from: {force_field_code_default.keys()}.")
+    # Create temporal pdb file
+    tmp_pdb = tempfile.NamedTemporaryFile(suffix='.pdb')
+    Chem.MolToPDBFile(rdkit_mol, tmp_pdb.name)
+
+    # Generate the topology
+    molecule = Molecule(rdkit_mol)
+    pdb_obj = app.PDBFile(tmp_pdb.name)
+    if force_field_type == 'openff':
+        system = smirnoff.ForceField(force_field_code_default[force_field_type]).create_openmm_system(molecule.to_topology())
+    else:
+        forcefield_obj = app.ForceField()
+        if force_field_type == 'gaff':
+            # Create the GAFF template generator
+            from openmmforcefields.generators import GAFFTemplateGenerator
+            template_generator = GAFFTemplateGenerator(molecules=molecule, forcefield = force_field_code_default[force_field_type])
+        elif force_field_type == 'espaloma':
+            # Create the Espaloma template generator
+            from openmmforcefields.generators import EspalomaTemplateGenerator
+            template_generator = EspalomaTemplateGenerator(molecules=molecule, forcefield = force_field_code_default[force_field_type])
+            
+        forcefield_obj.registerTemplateGenerator(template_generator.generator)
+        system = forcefield_obj.createSystem(pdb_obj.topology)
+    
+    structure = parmed.openmm.load_topology(pdb_obj.topology, system = system, xyz = pdb_obj.positions)
+    tmp_pdb.close()
+    return structure
+
 class Parameterize:
     """This is the main class for the parameterization
     """
 
     def __init__(
             self,
-            force_field_code:str = 'openff_unconstrained-2.0.0.offxml',
+            force_field_type:str = 'openff',
+            force_field_code:str = None,
             ext_types:List[str] = None,
             hmr_factor:float = None,
             overwrite:bool = False,
             safe_naming_prefix:str = None,
             out_dir:str = '.',
             ) -> None:
         """This is the constructor of the class.
+        GAFF and Espaloma capabilities came on version toff:0.1.0
 
         Parameters
         ----------
+        force_field_type : str, optional
+            This is used to identify the force field. Valid options are openff, gaff, espaloma (case insensitive), by default 'openff'
         force_field_code : str, optional
-            Any valid Open Force Field string representation.
-            Visit the `GitHub repo <https://github.com/openforcefield/openff-forcefields>`__ for
-            more information, by default 'openff_unconstrained-2.0.0.offxml'
+            This is the code that represent the force field.  Any valid OpenFF, GAFF or Espaloma string representation.
+            Visit the `openff-forcefields <https://github.com/openforcefield/openff-forcefields>`__
+            and `openmmforcefields <https://github.com/openmm/openmmforcefields>` for
+            more information. Its default value will dynamically change depending on force_field_type as:
+            * openff -> openff_unconstrained-2.0.0.offxml
+            * gaff -> gaff-2.11
+            * espaloma -> espaloma-0.2.2
         ext_types : List[str], optional
             Any extension from:
             'pdb', 'pqr', 'cif','pdbx',
             'parm7', 'prmtop', 'psf', 'top',
             'gro', 'mol2', '.mol3', 'crd',
             'rst7', 'inpcrd', 'restrt', 'ncrst'
             by default None which means that it will output: 'top', 'pdb', 'gro' files
@@ -282,14 +360,15 @@
             of the atom types. This is sometime needed to avoid incompatibilities
             with other force fields, by default None
         out_dir : str, optional
             Where the files will be written, by default '.'
         """
 
         self.force_field_code = force_field_code
+        self.force_field_type = force_field_type.lower()
         self.ext_types = ext_types
         self.hmr_factor = hmr_factor
         self.overwrite = overwrite
         self.safe_naming_prefix = safe_naming_prefix
         self.out_dir = os.path.abspath(out_dir)
 
     def __repr__(self) -> str:
@@ -306,15 +385,15 @@
         """This class is callable. And this is its implementation.
         it will return the specified files (ext_types in __init__) in the directory out_dir.
 
         Parameters
         ----------
         input_mol : str, Chem.rdchem.Mol molecule
             Could be a path to any file compatible with :meth:`toff.utils.get_rdkit_mol`:
-            (.inchi, .smi, .mol, .mol2)
+            (.inchi, .smi, .mol, .sdf, .mol2)
             or any valid RDKit molecule
         mol_resi_name : str, optional
             The residue name that will have the ligand. It is recommended to use
             name no longer than 4 characters, by default "MOL"
 
         Raises
         ------
@@ -332,27 +411,19 @@
 
         if len(mol_resi_name) > 4:
             warnings.warn(f"mol_resi_name = {mol_resi_name} is to large. consider to use a code with no more than 4 characters.")
 
         # Create if needed the output directory
         if not os.path.isdir(self.out_dir): os.makedirs(self.out_dir)
 
-        # Create temporal pdb file
-        tmp_pdb = tempfile.NamedTemporaryFile(suffix='.pdb')
-        Chem.MolToPDBFile(rdkit_mol, tmp_pdb.name)
-
-        # Generate the topology
-        try:
-            openff_mol = Molecule(rdkit_mol)
-            ligand_pdbfile = PDBFile(tmp_pdb.name)
-            ligand_system = ForceField(self.force_field_code).create_openmm_system(openff_mol.to_topology())
-            ligand_structure = parmed.openmm.load_topology(ligand_pdbfile.topology, ligand_system, xyz = ligand_pdbfile.positions)
-        except Exception as e:
-            raise Exception(e)
-        tmp_pdb.close()
+        ligand_structure = generate_structure(
+            rdkit_mol = rdkit_mol,
+            force_field_type = self.force_field_type,
+            force_field_code = self.force_field_code
+        )
         
         # Make Hydrogens Heavy for 4fs timestep
         if self.hmr_factor:
             parmed.tools.HMassRepartition(ligand_structure, self.hmr_factor).execute()
 
         # Change the residue name, dafault MOL
         for atom in ligand_structure.atoms:
```

### Comparing `toff-0.0.2/toff.egg-info/PKG-INFO` & `toff-0.1.0/toff.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toff
-Version: 0.0.2
+Version: 0.1.0
 Summary: toff is a python package to get topologies from the OpenFF initiative
 Home-page: https://github.com/ale94mleon/toff
 Author: Alejandro Martínez León
 Author-email: ale94mleon@gmail.com
 License: Apache License 2.0
 Project-URL: Discussions, https://github.com/ale94mleon/toff/discussions
 Project-URL: Documentation, https://toff.readthedocs.io/en/latest/
@@ -52,15 +52,19 @@
       - |license|
     * - **Downloads**
       - |downloads|
 
 Description
 -----------
 
-**TOFF** (Topologies from OpenFF) is a python package to get topologies from the OpenFF initiative. It was strongly inspired in this `Aniket's script <https://github.com/aniketsh/OpenFF/blob/82a2b5803e36b72f3525e3b8631cf256fbd8e35a/openff_topology.py>`__.
+**TOFF** (Topologies from OpenFF) is a python package initially developed to get topologies from the OpenFF initiative.
+It was strongly inspired in this `Aniket's script <https://github.com/aniketsh/OpenFF/blob/82a2b5803e36b72f3525e3b8631cf256fbd8e35a/openff_topology.py>`__.
+Since version **0.1.0** it is alos possible to get `GAFF <https://ambermd.org/antechamber/gaff.html>`__ and
+`Espaloma <https://docs.espaloma.org/en/latest/>`__ parameters by using **EspalomaTemplateGenerator** and **GAFFTemplateGenerator**
+from `openmmforcefields.generators <https://github.com/openmm/openmmforcefields/tree/main/openmmforcefields/generators>`__.
 
 
 You can try it out prior to any installation on `Binder <https://mybinder.org/v2/gh/ale94mleon/TOFF/HEAD?labpath=%2Fdocs%2Fnotebooks%2F>`__.
 
 Documentation
 -------------
```

