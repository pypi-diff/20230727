# Comparing `tmp/atooms_database-0.1.0-py2.py3-none-any.whl.zip` & `tmp/atooms_database-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,19 @@
-Zip file size: 76348 bytes, number of entries: 55
+Zip file size: 70030 bytes, number of entries: 37
 -rw-rw-r--  2.0 unx      722 b- defN 23-Jun-06 05:58 atooms/__init__.py
--rw-rw-r--  2.0 unx     5595 b- defN 23-Jun-06 13:31 atooms/database/__init__.py
--rw-rw-r--  2.0 unx      859 b- defN 23-Jun-06 05:58 atooms/database/_cutoffs.py
--rw-rw-r--  2.0 unx    11596 b- defN 23-Jun-06 12:29 atooms/database/_db.json
--rw-rw-r--  2.0 unx      362 b- defN 23-Jun-06 05:58 atooms/database/_potentials.py
+-rw-rw-r--  2.0 unx     2579 b- defN 23-Jun-07 18:30 atooms/database/__init__.py
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jun-07 18:30 atooms/database/_cutoffs.py
+-rw-rw-r--  2.0 unx    12417 b- defN 23-Jul-27 20:15 atooms/database/_models.json
+-rw-rw-r--  2.0 unx     1634 b- defN 23-Jun-10 15:29 atooms/database/_potentials.py
+-rw-rw-r--  2.0 unx     1871 b- defN 23-Jun-07 16:16 atooms/database/_samples.json
 -rw-rw-r--  2.0 unx     1824 b- defN 23-Jun-06 05:58 atooms/database/_schemas.py
--rw-rw-r--  2.0 unx     5492 b- defN 23-Jun-06 13:30 atooms/database/database.py
--rw-rw-r--  2.0 unx     4268 b- defN 23-Jun-06 11:27 atooms/database/helpers.py
--rw-rw-r--  2.0 unx     2010 b- defN 23-Jun-06 12:14 atooms/database/hooks.py
--rw-rw-r--  2.0 unx      452 b- defN 23-Jun-06 05:58 atooms/database/_v1/bernu_hiwatari_hansen_pastore.json
--rw-rw-r--  2.0 unx      557 b- defN 23-Jun-06 05:58 atooms/database/_v1/coslovich_pastore.json
--rw-rw-r--  2.0 unx      472 b- defN 23-Jun-06 05:58 atooms/database/_v1/dellavalle_gazzillo_frattini_pastore.json
--rw-rw-r--  2.0 unx      453 b- defN 23-Jun-06 05:58 atooms/database/_v1/gaussian_core.json
--rw-rw-r--  2.0 unx      494 b- defN 23-Jun-06 05:58 atooms/database/_v1/grigera_cavagna_giardina_parisi.json
--rw-rw-r--  2.0 unx      400 b- defN 23-Jun-06 05:58 atooms/database/_v1/harmonic_spheres.json
--rw-rw-r--  2.0 unx      368 b- defN 23-Jun-06 05:58 atooms/database/_v1/kob_andersen.json
--rw-rw-r--  2.0 unx      312 b- defN 23-Jun-06 05:58 atooms/database/_v1/lennard_jones.json
--rw-rw-r--  2.0 unx      466 b- defN 23-Jun-06 05:58 atooms/database/_v1/roux_barrat_hansen.json
--rw-rw-r--  2.0 unx      473 b- defN 23-Jun-06 05:58 atooms/database/_v1/wahnstrom.json
--rw-rw-r--  2.0 unx      612 b- defN 23-Jun-06 05:58 atooms/database/_v2/coslovich_pastore.json
--rw-rw-r--  2.0 unx      519 b- defN 23-Jun-06 05:58 atooms/database/_v2/dellavalle_gazzillo_frattini_pastore.json
--rw-rw-r--  2.0 unx      425 b- defN 23-Jun-06 05:58 atooms/database/_v2/kob_andersen.json
+-rw-rw-r--  2.0 unx     9607 b- defN 23-Jun-24 15:50 atooms/database/database.py
+-rw-rw-r--  2.0 unx     4664 b- defN 23-Jun-12 18:47 atooms/database/helpers.py
+-rw-rw-r--  2.0 unx     3233 b- defN 23-Jun-12 18:47 atooms/database/hooks.py
+-rw-rw-r--  2.0 unx     3214 b- defN 23-Jun-07 15:45 atooms/database/schema.py
 -rw-rw-r--  2.0 unx     3106 b- defN 23-Jun-06 12:29 atooms/database/f90/__init__.py
 -rw-rw-r--  2.0 unx     2875 b- defN 23-Jun-06 05:58 atooms/database/f90/cubic_spline.f90
 -rw-rw-r--  2.0 unx      965 b- defN 23-Jun-06 05:58 atooms/database/f90/cut.f90
 -rw-rw-r--  2.0 unx     2041 b- defN 23-Jun-06 05:58 atooms/database/f90/cut_shift.f90
 -rw-rw-r--  2.0 unx      769 b- defN 23-Jun-06 05:58 atooms/database/f90/gaussian.f90
 -rw-rw-r--  2.0 unx      993 b- defN 23-Jun-06 05:58 atooms/database/f90/harmonic_potential.f90
 -rw-rw-r--  2.0 unx     1516 b- defN 23-Jun-06 05:58 atooms/database/f90/inverse_power.f90
@@ -32,26 +21,19 @@
 -rw-rw-r--  2.0 unx     1023 b- defN 23-Jun-06 05:58 atooms/database/f90/lennard_jones.f90
 -rw-rw-r--  2.0 unx     2018 b- defN 23-Jun-06 05:58 atooms/database/f90/linear_cut_shift.f90
 -rw-rw-r--  2.0 unx     2022 b- defN 23-Jun-06 05:58 atooms/database/f90/quadratic_cut_shift.f90
 -rw-rw-r--  2.0 unx     1364 b- defN 23-Jun-06 05:58 atooms/database/f90/sum_inverse_power.f90
 -rw-rw-r--  2.0 unx     1137 b- defN 23-Jun-06 05:58 atooms/database/f90/yukawa.f90
 -rw-rw-r--  2.0 unx       35 b- defN 23-Jun-06 05:58 atooms/database/rumd/__init__.py
 -rw-rw-r--  2.0 unx     6469 b- defN 23-Jun-06 11:37 atooms/database/rumd/interaction.py
--rw-rw-r--  2.0 unx     1823 b- defN 23-Jun-06 05:58 atooms/database/storage/_db.json
--rw-rw-r--  2.0 unx      373 b- defN 23-Jun-06 05:58 atooms/database/storage/bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.json
 -rw-rw-r--  2.0 unx     6774 b- defN 23-Jun-06 05:58 atooms/database/storage/bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.xyz
--rw-rw-r--  2.0 unx      320 b- defN 23-Jun-06 05:58 atooms/database/storage/coslovich_pastore/0_488db481cdac35e599922a26129c3e35.json
 -rw-rw-r--  2.0 unx     9280 b- defN 23-Jun-06 05:58 atooms/database/storage/coslovich_pastore/0_488db481cdac35e599922a26129c3e35.xyz
--rw-rw-r--  2.0 unx      364 b- defN 23-Jun-06 05:58 atooms/database/storage/grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.json
 -rw-rw-r--  2.0 unx    59127 b- defN 23-Jun-06 05:58 atooms/database/storage/grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.xyz
--rw-rw-r--  2.0 unx      307 b- defN 23-Jun-06 05:58 atooms/database/storage/kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.json
 -rw-rw-r--  2.0 unx     4656 b- defN 23-Jun-06 05:58 atooms/database/storage/kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.xyz
--rw-rw-r--  2.0 unx      318 b- defN 23-Jun-06 05:58 atooms/database/storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.json
 -rw-rw-r--  2.0 unx     7888 b- defN 23-Jun-06 05:58 atooms/database/storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.xyz
--rw-rw-r--  2.0 unx      309 b- defN 23-Jun-06 05:58 atooms/database/storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.json
 -rw-rw-r--  2.0 unx     5927 b- defN 23-Jun-06 05:58 atooms/database/storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-06 13:34 atooms_database-0.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3455 b- defN 23-Jun-06 13:34 atooms_database-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-06 13:34 atooms_database-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       64 b- defN 23-Jun-06 13:34 atooms_database-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5624 b- defN 23-Jun-06 13:34 atooms_database-0.1.0.dist-info/RECORD
-55 files, 173563 bytes uncompressed, 66998 bytes compressed:  61.4%
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-27 20:15 atooms_database-0.2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3475 b- defN 23-Jul-27 20:15 atooms_database-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-27 20:15 atooms_database-0.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       64 b- defN 23-Jul-27 20:15 atooms_database-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3561 b- defN 23-Jul-27 20:15 atooms_database-0.2.0.dist-info/RECORD
+37 files, 171599 bytes uncompressed, 64162 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -3,69 +3,36 @@
 
 Filename: atooms/database/__init__.py
 Comment: 
 
 Filename: atooms/database/_cutoffs.py
 Comment: 
 
-Filename: atooms/database/_db.json
+Filename: atooms/database/_models.json
 Comment: 
 
 Filename: atooms/database/_potentials.py
 Comment: 
 
+Filename: atooms/database/_samples.json
+Comment: 
+
 Filename: atooms/database/_schemas.py
 Comment: 
 
 Filename: atooms/database/database.py
 Comment: 
 
 Filename: atooms/database/helpers.py
 Comment: 
 
 Filename: atooms/database/hooks.py
 Comment: 
 
-Filename: atooms/database/_v1/bernu_hiwatari_hansen_pastore.json
-Comment: 
-
-Filename: atooms/database/_v1/coslovich_pastore.json
-Comment: 
-
-Filename: atooms/database/_v1/dellavalle_gazzillo_frattini_pastore.json
-Comment: 
-
-Filename: atooms/database/_v1/gaussian_core.json
-Comment: 
-
-Filename: atooms/database/_v1/grigera_cavagna_giardina_parisi.json
-Comment: 
-
-Filename: atooms/database/_v1/harmonic_spheres.json
-Comment: 
-
-Filename: atooms/database/_v1/kob_andersen.json
-Comment: 
-
-Filename: atooms/database/_v1/lennard_jones.json
-Comment: 
-
-Filename: atooms/database/_v1/roux_barrat_hansen.json
-Comment: 
-
-Filename: atooms/database/_v1/wahnstrom.json
-Comment: 
-
-Filename: atooms/database/_v2/coslovich_pastore.json
-Comment: 
-
-Filename: atooms/database/_v2/dellavalle_gazzillo_frattini_pastore.json
-Comment: 
-
-Filename: atooms/database/_v2/kob_andersen.json
+Filename: atooms/database/schema.py
 Comment: 
 
 Filename: atooms/database/f90/__init__.py
 Comment: 
 
 Filename: atooms/database/f90/cubic_spline.f90
 Comment: 
@@ -105,62 +72,41 @@
 
 Filename: atooms/database/rumd/__init__.py
 Comment: 
 
 Filename: atooms/database/rumd/interaction.py
 Comment: 
 
-Filename: atooms/database/storage/_db.json
-Comment: 
-
-Filename: atooms/database/storage/bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.json
-Comment: 
-
 Filename: atooms/database/storage/bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.xyz
 Comment: 
 
-Filename: atooms/database/storage/coslovich_pastore/0_488db481cdac35e599922a26129c3e35.json
-Comment: 
-
 Filename: atooms/database/storage/coslovich_pastore/0_488db481cdac35e599922a26129c3e35.xyz
 Comment: 
 
-Filename: atooms/database/storage/grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.json
-Comment: 
-
 Filename: atooms/database/storage/grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.xyz
 Comment: 
 
-Filename: atooms/database/storage/kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.json
-Comment: 
-
 Filename: atooms/database/storage/kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.xyz
 Comment: 
 
-Filename: atooms/database/storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.json
-Comment: 
-
 Filename: atooms/database/storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.xyz
 Comment: 
 
-Filename: atooms/database/storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.json
-Comment: 
-
 Filename: atooms/database/storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz
 Comment: 
 
-Filename: atooms_database-0.1.0.dist-info/LICENSE
+Filename: atooms_database-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: atooms_database-0.1.0.dist-info/METADATA
+Filename: atooms_database-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: atooms_database-0.1.0.dist-info/WHEEL
+Filename: atooms_database-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: atooms_database-0.1.0.dist-info/top_level.txt
+Filename: atooms_database-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: atooms_database-0.1.0.dist-info/RECORD
+Filename: atooms_database-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atooms/database/__init__.py

```diff
@@ -12,29 +12,28 @@
 import glob
 import json
 import tempfile
 import shutil
 import hashlib
 from copy import deepcopy
 from .helpers import _wget
-from . import _schemas
-from . import f90, rumd
+from . import f90, rumd, hooks
 from .database import _TinyDB, Database, Query
-from .helpers import pprint
-import hooks
+from .helpers import pprint, copy
+from .schema import schema_version, schemas
+from .hooks import version
 
 _root = os.path.dirname(__file__)
-_storage = os.path.join(_root, 'storage')
-schemas = {1: _schemas.m1, 2: _schemas.m2}
 default_schema_version = 1
 
 # Databases
-samples = Database(os.path.join(_storage, "_db.json"))
-samples.storage_path='{model}/{version}_{md5_hash}'
-models = _TinyDB(os.path.join(_root, "_db.json"))
+samples = Database(os.path.join(_root, "_samples.json"))
+samples.storage_path = 'storage/{model}/{version}_{md5_hash}'
+models = _TinyDB(os.path.join(_root, "_models.json"))
+models.require = ('name', 'version', 'schema_version')  # or state?
 
 # Default query
 query = Query()
 
 # Public API
 
 def model(name, version=0, schema_version=None):
@@ -83,96 +82,8 @@
 
 def potential(name):
     return potentials[name]
     
 def cutoff(name):
     return cutoffs[name]
 
-# Internal API for entries to database
-
-# TODO: This should be done as import via an org mode file
-def add_model(path):
-    """
-    If `path` is a directory, add all json files in there to the
-    global `database`. If `path` ends with `json`, it will be assumed
-    to be match one or multiple json files (ex. `*.json`).
-    """
-    if path.endswith('json'):
-        search_path = glob.glob(path)
-    else:
-        search_path = glob.glob('{}/*.json'.format(path))
-
-    for _path in search_path:
-        # Read json file
-        with open(_path) as fh:
-            try:
-                model = json.load(fh)
-            except (ValueError, json.decoder.JSONDecodeError):
-                print('Error reading file {}'.format(_path))
-                raise
-
-        # By default, the model name is the file basename (stripped of .json)
-        if 'name' not in model:
-            name = os.path.basename(_path)[:-5]
-            model['name'] = '-'.join([entry.capitalize() for entry in name.split('_')])
-        if 'version' not in model:
-            model['version'] = 0
-        model['schema_version'] = _schema_version(model)
-
-        # Store model in database
-        query = Query()
-        models.upsert(model,
-                      (query.name == model["name"]) &
-                      (query.version == model["version"]) &
-                      (query.schema_version == model["schema_version"]))
-
-# def store_from_json(json_file, pretend=False):
-#     import json
-#     with open(json_file) as fh:
-#         data = json.load(fh)
-#         data["path"] = os.path.join(os.path.dirname(json_file),
-#                                     os.path.basename(data["path"]))
-#         store(pretend=pretend, **data)
-
-        
-# Model schema internal helpers
-
-def _validate_model(model, schema_version=None):
-    from jsonschema import validate
-    if schema_version is None:
-        schema_version = default_schema_version
-    validate(instance=model, schema=schemas[schema_version])
-
-def _schema_version(model):
-    """
-    Return the schema version of the model
-    """
-    from jsonschema import ValidationError
-
-    # Validate model against either version
-    valid = []
-    for schema_version in [1, 2]:
-        try:
-            _validate_model(model, schema_version)
-            valid.append(schema_version)
-        except ValidationError:
-            pass
-    # Return the schema id
-    if len(valid) == 1:
-        return valid[0]
-    elif len(valid) == 0:
-        raise ValidationError(f'invalid model {model}')
-    else:
-        raise InternalError(f'model {model} is valid for multiple schemas, this should not happen')
-
-def _convert(model, schema_version):
-    """
-    Convert model to schema `schema_version`. Do nothing is schema version is already the requested one
-    """
-    from .helpers import _upgrade_1_to_2
-    if _schema_version(model) == schema_version:
-        return model
-    elif _schema_version(model) == 1 and schema_version == 2:
-        return _upgrade_1_to_2(model)
-    else:
-        raise ValueError('cannot handle this conversion')
```

## atooms/database/_cutoffs.py

 * *Ordering differences only*

```diff
@@ -16,19 +16,19 @@
         def wrapper(r, isp, jsp, *args, **kwargs):
             return func(r, isp, jsp, *args, **kwargs) - self._params['shift'][isp, jsp]
         return wrapper
 
 class cut:
     pass
 
-class cubic_spline:
-    pass
-
 class linear:
     pass
 
 class quadratic:
     pass
 
+class cubic_spline:
+    pass
+
 cut_shift = shift
 linear_cut_shift = linear
 quadratic_cut_shift = quadratic
```

## atooms/database/_potentials.py

```diff
@@ -1,23 +1,44 @@
-def inverse_power(r, isp, jsp, epsilon, sigma, exponent):
-    return epsilon[isp, jsp] * (sigma[isp, jsp] / r)**exponent
+def inverse_power(r, epsilon, sigma, exponent):
+    return \
+        epsilon*(sigma/r)**exponent, \
+        epsilon*exponent*(sigma/r)**exponent/r**2, \
+        (-epsilon*exponent**2*(sigma/r)**exponent/r**2 - epsilon*exponent*(sigma/r)**exponent/r**2)/r
+
+def sum_inverse_power(r, epsilon, sigma, exponent):
+    return 0.0, 0.0, 0.0
+
+def yukawa(r, epsilon, kappa, sigma):
+    return \
+        epsilon*exp(kappa*(-r + sigma))/(kappa*r), \
+        epsilon*(kappa*r + 1)*exp(-kappa*(r - sigma))/(kappa*r**3), \
+        epsilon*(-kappa**2*r**2 - 2*kappa*r - 2)*exp(-kappa*(r - sigma))/(kappa*r**4)
+
+def lennard_jones(r, epsilon, sigma):
+    return \
+        4*epsilon*(-sigma**6/r**6 + sigma**12/r**12), \
+        -4*epsilon*(6*sigma**6/r**7 - 12*sigma**12/r**13)/r, \
+        -4*epsilon*(-42*sigma**6/r**8 + 156*sigma**12/r**14)/r
+
+def fene(r, kappa, R, sigma):
+    u = -R**2*kappa*log(-r**2/sigma**2 + 1)
+    w = 2*R**2*kappa/(r**2 - sigma**2)
+    h = 2*R**2*kappa*(-r**2 - sigma**2)/(r*(r**2 - sigma**2)**2)
+    if (r**2 < 2**(1./6)):
+        u += 4*epsilon*(-sigma**6/r**6 + sigma**12/r**12) + epsilon
+        w += 24*epsilon*sigma**6*(-r**6 + 2*sigma**6)/r**14
+        h += 24*epsilon*sigma**6*(7*r**6 - 26*sigma**6)/r**15
+    return u, w, h
+
+def gaussian(r, epsilon, sigma):
+    return \
+        epsilon*exp(-r**2/sigma**2),\
+        2*epsilon*exp(-r**2/sigma**2)/sigma**2,\
+        2*epsilon*(-2*r**2 + sigma**2)*exp(-r**2/sigma**2)/(r*sigma**4)
+    return 0.0
+
+def harmonic(r, epsilon, sigma):
+    return \
+        0.5*epsilon*(-r/sigma + 1)**2,\
+        1.0*epsilon*(-r + sigma)/(r*sigma**2),\
+        -1.0*epsilon/(r*sigma**2)
 
-def sum_inverse_power():
-    return 0.0
-
-def yukawa():
-    return 0.0
-
-def lennard_jones():
-    return 0.0
-
-def inverse_power_exp():
-    return 0.0
-
-def fene():
-    return 0.0
-
-def gaussian():
-    return 0.0
-
-def harmonic():
-    return 0.0
```

## atooms/database/database.py

```diff
@@ -1,155 +1,276 @@
 import os
 import tempfile
 import hashlib
 from tinydb import TinyDB, Query
+from tinydb.table import Table
 from atooms.core.utils import mkdir
-from .helpers import _wget
-
+from .hooks import absolute_path
+from .helpers import _wget, copy, pprint
+try:
+    from tqdm import tqdm as progress
+except:
+    progress = lambda x: x
 
 class _TinyDB(TinyDB):
 
+    """
+    A custom TinyDB database with read hooks, required variables and
+    columns accessor
+    """
+
+    def __init__(self, *args, **kwargs):
+        if len(args) == 0 and len(kwargs) == 0:
+            from tinydb.storages import MemoryStorage
+            super().__init__(storage=MemoryStorage)
+        else:
+            super().__init__(*args, **kwargs)
+        self.require = ()
+        self._hooks = []
+
+    def add_hook(self, hook, *args, **kwargs):
+        """Register a new hook to be applied when accessing the entries"""
+        if hook not in [hook[0] for hook in self._hooks]:
+            self._hooks.append((hook, args, kwargs))
+
+    def remove_hooks(self):
+        """Remove hooks"""
+        self._hooks = []
+
+    def _apply_hooks(self, entry):
+        """Apply hooks and store the values in the new entry"""
+        for hook in self._hooks:
+            result = hook[0](entry, *hook[1], **hook[2])
+            entry.update(result)
+        return entry
+
     def columns(self, merge=set.intersection):
         """Return columns of database"""
-        cols = set(self.all()[0])
-        for entry in self.all():
-            cols = merge(cols, set(entry.keys()))
+        cols = None
+        for entry in self:
+            if cols is None:
+                cols = set(entry.keys())
+            else:
+                cols = merge(cols, set(entry.keys()))
         return sorted(list(cols))
 
-    
+    def rows(self, cond=None, columns=(), sort_by=()):
+        """
+        Return rows matching a condition as dicts with columns as keys,
+        sorted according to column keys.
+        """
+        if cond is None:
+            entries = self.all()
+        else:
+            entries = self.search(cond)
+
+        if sort_by is not None:
+            if not (isinstance(sort_by, list) or isinstance(sort_by, tuple)):
+                sort_by = [sort_by]
+            entries = sorted(entries, key=lambda x: [x[_] for _ in sort_by])
+
+        if len(columns) == 0:
+            columns = self.columns()
+
+        output = {}
+        for column in columns:
+            output[column] = [entry[column] for entry in entries]
+        return output
+
+    def pprint(self, cond=None, **kwargs):
+        """Pretty print"""
+        if cond is None:
+            entries = self.all()
+        else:
+            entries = self.search(cond)
+        pprint(entries, **kwargs)
+
+    def insert(self, entry):
+        """
+        We upsert against the `self.require` variable. If all required
+        variables of the new entry match an existing one and overwrite
+        is True, then we only update the entry. If overwrite is False,
+        an error is raised.
+        """
+        if len(self.require) == 0:
+            # TODO: could not get this with super()
+            from tinydb.table import Table
+            Table.insert(self, entry)
+        else:
+            # Make sure that all required variables match
+            query = Query()
+            queries = []
+            for var in self.require:
+                queries.append(query[var] == entry[var])
+            cond = queries[0]
+            for q in queries[1: ]:
+                cond = cond.__and__(q)
+            self.upsert(entry, cond)
+
+    def update(self):
+        """Update database entries, to store metadata from hooks"""
+        # This will store metadata from hooks
+        for entry in progress(self.all()):
+            self.insert(**entry)
+
+    # The following two methods are redefined to allow for readonly
+    # hooks that are applied only when accessing the
+    # database. Otherwise, we can first store the hooks results in the
+    # database (via some update) and get rid of them.
+
+    # TODO: should we keep hooks or just provide decorators to client code?
+
+    # Note: storing absolute paths in a portable way can be achieved by
+    # restoring read only hooks, overloading all() and search(). This may
+    # also be useful when the db is read only and we do not want to modify
+    # it. If we store them upon insertion, the database will not be
+    # portable when moving it to a new folder and this is a feature to
+    # preserve. We could of course just process the output list in client
+    # code, but things like searching for custom columns would not be
+    # possible. One possible nomenclature is pre and post hook, like git.
+
+    def __iter__(self):
+        """
+        Return an iterator for the default table's documents.
+        """
+        for entry in self.table(self.default_table_name):
+            entry = self._apply_hooks(entry)
+            yield entry
+
+    def search(self, cond):
+        """
+        Search for all documents matching a 'where' cond.
+
+        :param cond: the condition to check against
+        :returns: list of matching documents
+        """
+        # TODO: how should we overload this?
+        entries = self.table(self.default_table_name).search(cond)
+        for entry in entries:
+            self._apply_hooks(entry)
+        return entries
+
+    def all(self):
+        """
+        Get all documents stored in the table.
+
+        :returns: a list with all documents.
+        """
+        return list(iter(self))
+
 class Database(_TinyDB):
 
+    """
+    A simple database of files
+    """
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # Look for the root of the db file, if present
         # This is where we will store the files, if requested
         try:
             path = self._storage._handle.name
+            # TODO: perhaps rename root? or privatize?
             self.storage_root = os.path.dirname(path)
+            self.add_hook(absolute_path, self.storage_root)
         except AttributeError:
             self.storage_root = None
         self.storage_path = '{md5_hash}'
-        self._hooks = []
+        self.require = ('md5_hash', )
 
-    def add_hook(self, hook, *args, **kwargs):
-        """Register a new hook"""
-        self._hooks.append((hook, args, kwargs))
+    def remove_hooks(self):
+        """Remove hooks"""
+        # Make sure absolute paths are always added
+        super().remove_hooks()
+        self.add_hook(absolute_path, self.storage_root)
+
+    # TODO: avoid reinsertions if path (exists & hash is the same)
+    def insert(self, input_path=None, copy=False, **kwargs):
+        """
+        Insert a new `input_path` in the database. If `copy` is True, the
+        file is copied in the database storage.
+        """
+        if input_path is None:
+            # Useful for update. We assume absolute_path has been added already...
+            input_path = kwargs["absolute_path"]
 
-    def _apply_hooks(self, entry):
-        """Apply hooks and store the values in the new entry"""
-        for hook in self._hooks:
-            result = hook[0](os.path.join(self.storage_root, entry['path']), *hook[1], **hook[2])
-            entry.update(result)
-        return entry
-        
-    def insert(self, path, copy=False, **kwargs):
-        # TODO: move path to kwargs?
         # Set paths: storage_path is what goes in the db
-        if path.startswith('http'):
+        if input_path.startswith('http'):
             tmpdir = tempfile.mkdtemp()
-            basename = os.path.basename(path)
-            _wget(path, tmpdir)
+            basename = os.path.basename(input_path)
+            _wget(input_path, tmpdir)
             local_path = os.path.join(tmpdir, basename)
         else:
-            local_path = path
-        # TODO: add to entry
-        extension = os.path.splitext(local_path)[-1]
+            local_path = input_path
 
-        # We now have a local copy in local_path, get the md5 hash
+        # Read data
         with open(local_path, "rb") as fh:
             data = fh.read()
-        md5_hash = hashlib.md5(data).hexdigest()
 
         # Create the new entry
+        # TODO: handle http paths
         entry = {}
-        # User provided data
         entry.update(**kwargs)
-        # Default values
-        entry['md5_hash'] = md5_hash
-        # TODO: pass path explicitly to _apply_hooks() so we can use the additional metadata in defining the final path
-        # TODO: handle http paths
-        # If storing a local copy, we use the storage in path
-        if copy:
-            entry['path'] = self.storage_path.format(**entry)
-        else:
-            entry['path'] = path
-        # Apply hooks and store the values in the new entry
-        entry = self._apply_hooks(entry)
-        
-        # Store copy of data
+        entry['md5_hash'] = hashlib.md5(data).hexdigest()
+
         if copy:
-            out_path = os.path.join(self.storage_root, entry["path"]) + extension
+            # If storing a local copy, we interpolate the path
+            extension = os.path.splitext(local_path)[-1]
+            entry['path'] = self.storage_path.format(**entry) + extension
+            out_path = os.path.join(self.storage_root, entry["path"])
             with open(out_path, "wb") as fh:
                 fh.write(data)
+        else:
+            # TODO: should we make it absolute? or relative to what?
+            entry['path'] = input_path
 
         # Add the entry to the database
-        # If the file hash is found we update, else we add a new entry
-        query = Query()
-        self.upsert(entry, query.md5_hash == md5_hash)
+        super().insert(entry)
 
     def insert_glob(self, path, copy=False, **kwargs):
+        """Insert multiple files from a globbale `path`."""
         from glob import glob
-        for _path in glob(path, recursive=True):
+        for _path in progress(glob(path, recursive=True)):
             self.insert(_path, copy, **kwargs)
 
     def insert_multiple(self, path, copy=False, **kwargs):
-        for _path in path:
+        """Insert multiple files from an interable `path`"""
+        for _path in progress(path):
             self.insert(_path, copy, **kwargs)
 
-    def update(self, ignore=()):
-        """Useful to apply new hooks?"""
-        # Move to _TinyDB?
-        ignore = ['path'] + list(ignore)
+    def _missing(self):
+        """Check that the paths of all the entries exist"""
+        # TODO: handle http links (check if accessible)
+        # TODO: this does not work
+        # query = Query()
+        # return self.search(~ (query.absolute_path.test(os.path.exists)))
+        docs = []
+        for entry in self.all():
+           if not os.path.exists(entry['absolute_path']):
+               docs.append(entry)
+        return docs
+
+    def update(self):
+        """
+        Update database entries, clearing missing files and storing
+        updated metadata from hooks
+        """
+        # Files that have been deleted are removed from the db
+        #query = Query()
+        #return self.search(~ (query.absolute_path.test(os.path.exists)))
+        ids = []
         for entry in self.all():
-            path = entry['path']
-            kwargs = {k: entry[k] for k in entry if k not in ignore}
-            self.insert(path, **kwargs)
+           if not os.path.exists(entry['absolute_path']):
+               ids.append(entry.doc_id)
+        self.remove(doc_ids=ids)
+        # if len(ids) > 0:
+        #     print(f"{len(ids)} entries will be removed")
+        # Now update the rest of the entries
+        super().update()
 
     def copy(self, query, path='/tmp/{path}'):
-        """Get a copy of `path` in the samples database and return the path to it"""
-        import shutil
+        """Get copies entries matching `query` in the database and return the paths"""
         paths = []
-        # TODO: getting the full path via storage_root is what prevent this from
-        # detaching as a standalone function
         for entry in self.search(query):
-            if path is None:
-                tmpdir = tempfile.mkdtemp()
-                basename = os.path.basename(entry['path'])
-                path = os.path.join(tmpdir, basename)
-            else:
-                path = path.format(**entry)
-                
-            if entry['path'].startswith('http'):
-                _wget(entry['path'], tmpdir)
-            else:
-                from atooms.core.utils import mkdir
-                mkdir(os.path.dirname(path))
-                shutil.copy(os.path.join(self.storage_root, entry['path']), path)
-            paths.append(path)
+            out_path = copy(entry, root=self.storage_root)
+            paths.append(out_path)
         return paths
-
-    # The following two methods are redefined to allow for readonly
-    # hooks that are applied only when accessing the
-    # database. Otherwise, we can first store the hooks results in the
-    # database (via some update?) and get rid of them.
-    
-    def __iter__(self):
-        """
-        Return an iterator for the default table's documents.
-        """
-        for entry in self.table(self.default_table_name):
-            entry = self._apply_hooks(entry)
-            yield entry
-
-    def search(self, cond):
-        """
-        Search for all documents matching a 'where' cond.
-
-        :param cond: the condition to check against
-        :returns: list of matching documents
-        """
-        # TODO: how should we overload this?
-        entries = self.table(self.default_table_name).search(cond)
-        for entry in entries:
-            self._apply_hooks(entry)
-        return entries
-
```

## atooms/database/helpers.py

```diff
@@ -1,127 +1,142 @@
-def pprint(rows, columns=None, sort_by=None, max_rows=20):
-    """Pretty print rows from a list of dicts"""
+import os
+import shutil
+import hashlib
+from .schema import schema_version
+
+
+def pprint(rows, columns=None, sort_by=None, max_rows=10):
+    """Pretty print `rows` (a list of dicts)"""
     
-    def _tabular(data, sort_by=0, max_len=100):
+    def _tabular(data, max_len=100):
         """General function to format `data` list in tabular table"""
         # Predict formatting
         lens = [0 for _ in range(len(data[0]))]
         for entry in data:
             for i, value in enumerate(entry):
                 lens[i] = max(lens[i], len(str(value)))
         fmts = [f'{{:{lens[i]}s}}' for i in range(len(lens))]
         fmt = ' '.join(fmts)
 
         # Store list of lines
         lines = []
         lines.append(fmt.format(*data[0]))
         lines.append('-'*(sum(lens) + len(lens) - 1))
-        for entry in sorted(data[1:], key=lambda x: x[sort_by]):
+        for entry in data[1:]:
             entry = [str(_) for _ in entry]
             lines.append(fmt.format(*entry))
-            if len(lines) > max_rows:
+            if len(lines) > max_rows and max_rows > 0:
+                lines.append(f'... {len(data) - max_rows} entries not shown')
                 break
 
         # Limit columns
         if sum(lens) > max_len:
             for i, line in enumerate(lines):
                 if i < 2:
                     fill = '     '
                 else:
                     fill = ' ... '
                 lines[i] = line[:max_len//2] + fill + line[sum(lens) - max_len//2:]
         return lines
 
     # Format and sort the data        
     if columns is None:
-        columns = set(rows[0])
+        columns = set([e for e in rows[0] if not e.startswith('__')])
         for entry in rows:
-            columns = set.union(columns, set(entry.keys()))
-    if sort_by is None:
-        sort_by = 0
-    else:
-        sort_by = columns.index(sort_by)
-
+            new_columns = set([e for e in entry if not e.startswith('__')])
+            columns = set.union(columns, new_columns)
+        columns = sorted(columns)
+
+    if sort_by is not None:
+        if not (isinstance(sort_by, list) or isinstance(sort_by, tuple)):
+            sort_by = [sort_by]
+        rows = sorted(rows[1:], key=lambda x: [x[_] for _ in sort_by])
+  
     # Tabularize lines and join them
     rows = [columns] + [[str(entry.get(key)) for key in columns] for entry in rows]
-    lines = _tabular(rows, sort_by=sort_by)
+    lines = _tabular(rows)
     print('\n'.join(lines))
 
 def _wget(url, output_dir):
     """Like wget on the command line"""
-    import sys
-    import os
-    import shutil
     try:
         from urllib.request import urlopen  # Python 3
     except ImportError:
         from urllib2 import urlopen  # Python 2
 
     basename = os.path.basename(url)
     output_file = os.path.join(output_dir, basename)
     response = urlopen(url)
     length = 16*1024
     with open(output_file, 'wb') as fh:
         shutil.copyfileobj(response, fh, length)
 
-def _upgrade_1_to_2(model):
-    """Convert from schema version 1 to 2"""
-    new_model = {}
-    # Optional
-    if "reference" in model:
-        new_model["reference"] = model["reference"]
-    if "doi" in model:
-        new_model["doi"] = model["doi"]
-    new_model["potential"] = []
-    for potential in model["potential"]:
-        new_potential = {}
-        new_potential["type"] = potential["type"]
-        new_potential["parameters"] = {}
-        db = {}
-        for key in potential["parameters"]:
-            db[key] = {}
-            nsp = len(potential["parameters"][key])
-            for i in range(nsp):
-                for j in range(nsp):
-                    if j<i: continue
-                    pair = f'{i+1}-{j+1}'
-                    db[key][pair] = potential["parameters"][key][i][j]
-        last_key = key
-        for pair in db[last_key].keys():
-            new_potential["parameters"][pair] = {key:db[key][pair] for key in db.keys()}
-        new_model["potential"].append(new_potential)
-
-    new_cutoffs = []
-    for cutoff in model["cutoff"]:
-        new_cutoff = {}
-        new_cutoff["type"] = cutoff["type"]
-        new_cutoff["parameters"] = {}
-        db = {}
-        for key in cutoff["parameters"]:
-            db[key] = {}
-            nsp = len(cutoff["parameters"][key])
-            for i in range(nsp):
-                for j in range(nsp):
-                    if j<i: continue
-                    pair = f'{i+1}-{j+1}'
-                    db[key][pair] = cutoff["parameters"][key][i][j]
-        last_key = key
-        for pair in db[last_key].keys():
-            new_cutoff["parameters"][pair] = {key:db[key][pair] for key in db.keys()}
-        new_cutoffs.append(new_cutoff)
-    for i, new_cutoff in enumerate(new_cutoffs):
-        new_model["potential"][i]["cutoff"] = new_cutoff
-    return new_model
 
+def copy(entry, path='/tmp/{path}', root=''):
+    """Get a copy of `path` in the samples database and return the path to it"""
+    from atooms.core.utils import mkdir
+
+    # Handle output path
+    if path is None:
+        # Output path is a temporary directory
+        tmpdir = tempfile.mkdtemp()
+        basename = os.path.basename(entry['path'])
+        path = os.path.join(tmpdir, basename)
+    else:
+        # Interpolate path with entry fields
+        path = path.format(**entry)
+
+    # Now copy
+    if entry['path'].startswith('http'):
+        # Over the network
+        _wget(entry['path'], tmpdir)
+    else:
+        # Local storage
+        mkdir(os.path.dirname(path))
+        if entry['path'].startswith('/'):
+            # Absolute path, so ignore root variable
+            shutil.copy(entry['path'], path)
+        else:
+            # Path is relative to root, most likely database folder
+            shutil.copy(os.path.join(root, entry['path']), path)
+
+    return path
 
 class _objdict(dict):
 
     """Boots a dict with object-like attribute accessor"""
 
     def __getattr__(self, name):
         return self[name]
 
     def __setattr__(self, name, value):
         self[name] = value
 
     def __delattr__(self, name):
         del self[name]
+
+def add_model_json(path):
+    """
+    If `path` is a directory, add all json files in there to the
+    global `database`. If `path` ends with `json`, it will be assumed
+    to be match one or multiple json files (ex. `*.json`).
+    """
+    if path.endswith('json'):
+        search_path = glob.glob(path)
+    else:
+        search_path = glob.glob('{}/*.json'.format(path))
+
+    for _path in search_path:
+        # Read json file
+        with open(_path) as fh:
+            try:
+                model = json.load(fh)
+            except (ValueError, json.decoder.JSONDecodeError):
+                print('Error reading file {}'.format(_path))
+                raise
+
+        # By default, the model name is the file basename (stripped of .json)
+        if 'name' not in model:
+            name = os.path.basename(_path)[:-5]
+            model['name'] = '-'.join([entry.capitalize() for entry in name.split('_')])
+
+        yield model
```

## atooms/database/hooks.py

```diff
@@ -1,58 +1,89 @@
 import os
 import re
 import numpy
 from atooms.core.utils import tipify
 from atooms.trajectory import Trajectory
 from atooms.system.particle import distinct_species, composition
+from .helpers import schema_version
 
+def version(entry):
+    """Detect schema_version and set default version"""
+    schema = schema_version(entry)
+    if 'version' not in entry:
+        return {'version': 0,
+                'schema_version': schema
+                }
+    else:
+        return {'schema_version': schema}
 
-def model_version(path, model, version=0):
-    return {
-	"model": model,
-        "version": version,
-    }
-
-def format_extension(path, format=None):
+def absolute_path(entry, root):
+    """Add absolute path"""
+    if entry['path'].startswith('/'):
+        return {'absolute_path': entry['path']}
+    else:
+        return {'absolute_path': os.path.join(root, entry['path'])}
+    
+def format_extension(entry, format=None):
+    path = entry['path']
     if format is None:
         ext = os.path.splitext(path)[-1].strip('.')
         if len(ext) > 0:
             format = ext
     return {
         "format": format,
         "extension": ext
     }
 
-def metadata_from_atooms(path):
+def metadata_from_atooms(entry):
+    # TODO: use db['cache'] to gather all caches
+    # Cache to avoid fetching data if not necessary
+    # TODO: what happens with directories?
+    path = entry['absolute_path']
+    if not os.path.exists(path):
+        # Exit gracefully. This is ok if files are removed and are
+        # then cleared with update()
+        return {}
+        
+    last_modified = os.path.getmtime(path)
+    if '__cache_metadata_from_atooms' in entry:
+        if entry['__cache_metadata_from_atooms'] >= last_modified:
+            return {}
+
+    # Store metadata
     th = Trajectory(path)
     system = th[0]
-    radii = system.dump('particle.radius')
     db = {}
-    db['format'] = str(th.__class__)
+    db['__cache_metadata_from_atooms'] = os.path.getmtime(th.filename)
+    s = re.search(r'([a-zA-Z0-9]*)Trajectory([a-zA-Z0-9]*)', str(th.__class__))
+    fmt = (s.group(1) + s.group(2)).lower()
+    db['format'] = fmt
     db['frames'] = len(th)
     db['megabytes'] = int((os.path.getsize(th.filename) / 1e6))
     db['particles'] = len(system.particle)
     db['species'] = ', '.join(distinct_species(system.particle))
     db['composition'] = dict(composition(system.particle))
-    db['size dispersion'] = str((numpy.std(radii) / numpy.mean(radii)))
+    # radii = system.dump('particle.radius')
+    # db['size dispersion'] = str((numpy.std(radii) / numpy.mean(radii)))
     db['density'] = round(system.density, 10)
     if system.cell is not None:
         db['cell side'] = str(list(system.cell.side))[1: -1]
         db['cell volume'] = system.cell.volume
     if len(th) > 1:
         db['steps'] = int(th.steps[-1])
         db['duration'] = int(th.times[-1])
         db['timestep'] = float(th.timestep)
         db['block size'] = int(th.block_size)
         db['grandcanonical'] = th.grandcanonical
     th.close()
     return db
 
-def metadata_from_path(path, aliases=(('T', 'temperature'),
-                                      ('P', 'pressure'))):
+def metadata_from_path(entry, aliases=(('T', 'temperature'),
+                                       ('P', 'pressure'))):
+    path = entry['path']
     db = {}
     for entry in os.path.dirname(path).split('/'):
         for sub in entry.split('_'):
             res = re.match('([a-zA-Z]*)([0-9.]*)', sub)
             if len(res.group(2)) > 0:
                 key = res.group(1)
                 for alias in aliases:
```

## Comparing `atooms/database/_db.json` & `atooms/database/_models.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9777777777777779%*

 * *Differences: {"'_default'": "{'14': OrderedDict([('reference', 'Proc. R. Soc. Lond. A, 106, 463 (1924)'), "*

 * *               "('doi', '10.1098/rspa.1924.0082'), ('name', 'lennard_jones'), ('version', 0), "*

 * *               "('potential', [OrderedDict([('type', 'lennard_jones'), ('parameters', "*

 * *               "OrderedDict([('epsilon', [[1.0]]), ('sigma', [[1.0]])]))])]), ('cutoff', "*

 * *               "[OrderedDict([('type', 'cut_shift'), ('parameters', OrderedDict([('rcut', "*

 * *               "[[2.5]])]))])]), ('schema_version' […]*

```diff
@@ -855,14 +855,123 @@
                     "type": "lennard_jones"
                 }
             ],
             "reference": "J. Phys.: Condens. Matter 21, 285107 (2009)",
             "schema_version": 2,
             "version": 0
         },
+        "14": {
+            "cutoff": [
+                {
+                    "parameters": {
+                        "rcut": [
+                            [
+                                2.5
+                            ]
+                        ]
+                    },
+                    "type": "cut_shift"
+                }
+            ],
+            "doi": "10.1098/rspa.1924.0082",
+            "name": "lennard_jones",
+            "potential": [
+                {
+                    "parameters": {
+                        "epsilon": [
+                            [
+                                1.0
+                            ]
+                        ],
+                        "sigma": [
+                            [
+                                1.0
+                            ]
+                        ]
+                    },
+                    "type": "lennard_jones"
+                }
+            ],
+            "reference": "Proc. R. Soc. Lond. A, 106, 463 (1924)",
+            "schema_version": 1,
+            "version": 0
+        },
+        "15": {
+            "cutoff": [
+                {
+                    "parameters": {
+                        "rcut": [
+                            [
+                                2.5,
+                                2.0,
+                                2.25
+                            ],
+                            [
+                                2.0,
+                                2.2,
+                                2.1
+                            ],
+                            [
+                                2.25,
+                                2.1,
+                                2.35
+                            ]
+                        ]
+                    },
+                    "type": "cut_shift"
+                }
+            ],
+            "doi": "10.1103/physrevlett.125.085505",
+            "name": "kob_andersen_2",
+            "notes": "KA2 in the reference",
+            "potential": [
+                {
+                    "parameters": {
+                        "epsilon": [
+                            [
+                                1.0,
+                                1.5,
+                                1.25
+                            ],
+                            [
+                                1.5,
+                                0.5,
+                                1.0
+                            ],
+                            [
+                                1.25,
+                                1.0,
+                                0.75
+                            ]
+                        ],
+                        "sigma": [
+                            [
+                                1.0,
+                                0.8,
+                                0.9
+                            ],
+                            [
+                                0.8,
+                                0.88,
+                                0.84
+                            ],
+                            [
+                                0.9,
+                                0.84,
+                                0.94
+                            ]
+                        ]
+                    },
+                    "type": "lennard_jones"
+                }
+            ],
+            "reference": "Phys. Rev. Lett. 125, 085505 (2020)",
+            "schema_version": 1,
+            "version": 0
+        },
         "2": {
             "cutoff": [
                 {
                     "parameters": {
                         "rcut": [
                             [
                                 2.5,
```

## Comparing `atooms/database/storage/_db.json` & `atooms/database/_samples.json`

 * *Files 9% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9858217592592593%*

 * *Differences: {"'_default'": "{'1': {'path': "*

 * *               "'storage/coslovich_pastore/0_488db481cdac35e599922a26129c3e35.xyz'}, '2': {'path': "*

 * *               "'storage/kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.xyz'}, '3': {'path': "*

 * *               "'storage/grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.xyz'}, "*

 * *               "'4': {'path': 'storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz'}, "*

 * *               "'5': {'path': 'storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57 […]*

```diff
@@ -2,68 +2,68 @@
     "_default": {
         "1": {
             "density": 1.655,
             "format": "xyz",
             "md5_hash": "488db481cdac35e599922a26129c3e35",
             "model": "coslovich_pastore",
             "number_of_particles": 300,
-            "path": "coslovich_pastore/0_488db481cdac35e599922a26129c3e35.xyz",
+            "path": "storage/coslovich_pastore/0_488db481cdac35e599922a26129c3e35.xyz",
             "potential_energy_per_particle": 0.0,
             "temperature": 0.31,
             "version": 0
         },
         "2": {
             "density": 1.2,
             "format": "xyz",
             "md5_hash": "8f4a9fe755e5c1966c10b50c9a53e6bf",
             "model": "kob_andersen",
             "number_of_particles": 150,
-            "path": "kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.xyz",
+            "path": "storage/kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.xyz",
             "potential_energy_per_particle": 0.0,
             "temperature": 0.0,
             "version": 0
         },
         "3": {
             "density": 1.0,
             "format": "xyz",
             "md5_hash": "0ac97fa8c69c320e48bd1fca80855e8a",
             "model": "grigera_cavagna_giardina_parisi",
             "number_of_particles": 1000,
-            "path": "grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.xyz",
+            "path": "storage/grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.xyz",
             "potential_energy_per_particle": 2.1449771790499375,
             "temperature": 0.2461,
             "version": 0
         },
         "4": {
             "density": 1.0,
             "format": "xyz",
             "md5_hash": "5cc3b80bc415fa5c262e83410ca65779",
             "model": "lennard_jones",
             "number_of_particles": 108,
-            "path": "lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz",
+            "path": "storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz",
             "potential_energy_per_particle": 0.0,
             "temperature": 0.0,
             "version": 0
         },
         "5": {
             "density": 1.0,
             "format": null,
             "md5_hash": "13ce47602b259f7802e89e23ffd57f19",
             "model": "lennard_jones",
             "number_of_particles": 256,
-            "path": "lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.xyz",
+            "path": "storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.xyz",
             "potential_energy_per_particle": -3.8079776291909284,
             "version": 0
         },
         "6": {
             "density": 0.5341880341880343,
             "format": "xyz",
             "md5_hash": "f61d7e58b9656cf9640f6e5754441930",
             "model": "bernu_hiwatari_hansen_pastore",
             "number_of_particles": 216,
-            "path": "bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.xyz",
+            "path": "storage/bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.xyz",
             "potential_energy_per_particle": 1.8746927108811235,
             "temperature": 0.208,
             "version": 0
         }
     }
 }
```

## Comparing `atooms_database-0.1.0.dist-info/METADATA` & `atooms_database-0.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atooms-database
-Version: 0.1.0
+Version: 0.2.0
 Summary: Database of interaction database for classical molecular dynamics and Monte Carlo simulations
 Home-page: https://framagit.org/atooms/database
 Author: Daniele Coslovich
 Author-email: dcoslovich@units.it
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: atooms (~=3.17)
 Requires-Dist: f2py-jit (~=0.5)
 Requires-Dist: jsonschema
 Requires-Dist: tinydb
+Requires-Dist: tqdm
 
 Atooms database
 ===============
 
 [![pypi](https://img.shields.io/pypi/v/atooms-database.svg)](https://pypi.python.org/pypi/atooms-database/)
 [![version](https://img.shields.io/pypi/pyversions/atooms-database.svg)](https://pypi.python.org/pypi/atooms-database/)
 [![license](https://img.shields.io/pypi/l/atooms-pp.svg)](https://en.wikipedia.org/wiki/GNU_General_Public_License)
```

