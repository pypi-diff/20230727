# Comparing `tmp/fsaa-0.0.7.tar.gz` & `tmp/fsaa-0.0.8.tar.gz`

## Comparing `fsaa-0.0.7.tar` & `fsaa-0.0.8.tar`

### file list

```diff
@@ -1,58 +1,62 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.7/CITATION.cff
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.7/CODEOWNERS
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.7/environment.yml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fsaa-0.0.7/requirements.txt
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fsaa-0.0.7/update-version.sh
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.7/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.7/.vscode/settings.json
--rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.7/assets/logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/attack.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/core.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/utils.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/examples/tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/initializers/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/initializers/random.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/initializers/random_sign.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/losses/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/losses/cossim_loss.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/losses/lpips_loss.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/losses/mse_loss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/masks/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/masks/custom.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/masks/jnd.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/masks/nomask.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/__init__.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/hf/hf_models.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/hf_models/hf_models.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/hub/hub_models.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/hub_models/hub_models.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/ibot/ibot.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/ibot/utils.py
--rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/models/ibot/vits.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/transforms/__init__.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/transforms/compose.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/transforms/normalize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/updaters/__init__.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/updaters/fgsm.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/updaters/langevin.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/updaters/pgd.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.7/fsaa/updaters/random.py
--rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.7/imgs/adv.png
--rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.7/imgs/mask.png
--rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.7/imgs/orig.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_attack.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_initializers.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_masks.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_models.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_transforms.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.7/tests/test_updaters.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.7/.gitignore
--rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.7/LICENSE
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.7/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fsaa-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 fsaa-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fsaa-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.8/CITATION.cff
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.8/CODEOWNERS
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.8/environment.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fsaa-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fsaa-0.0.8/update-version.sh
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.8/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.8/assets/logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/attack.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/core.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/examples/tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/initializers/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/initializers/random.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/initializers/random_sign.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/losses/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/losses/cossim_loss.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/losses/lpips_loss.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/losses/mse_loss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/masks/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/masks/custom.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/masks/jnd.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/masks/nomask.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/cae/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/cae/cae.py
+-rw-r--r--   0        0        0    24969 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/cae/modeling_finetune.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/cae/utils.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/hf/hf_models.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/hub/hub_models.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/ibot/ibot.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/ibot/utils.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/ibot/vits.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/ijepa/ijepa.py
+-rw-r--r--   0        0        0    20548 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/ijepa/vision_transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/transforms/__init__.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/transforms/compose.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/transforms/normalize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/updaters/__init__.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/updaters/fgsm.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/updaters/langevin.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/updaters/pgd.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/updaters/random.py
+-rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.8/imgs/adv.png
+-rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.8/imgs/mask.png
+-rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.8/imgs/orig.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_attack.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_initializers.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_masks.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_models.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_transforms.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_updaters.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.8/.gitignore
+-rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.8/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fsaa-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 fsaa-0.0.8/PKG-INFO
```

### Comparing `fsaa-0.0.7/.pre-commit-config.yaml` & `fsaa-0.0.8/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     hooks:
     -   id: isort
         name: isort (python)
 -   repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
     -   id: flake8
-        entry: flake8 --ignore=F403,F405,W503,W504
+        entry: flake8 --ignore=E501,F403,F405,W503,W504
 -   repo: local
     hooks:
     -   id: pytest
         name: pytest
         entry: pytest tests
         language: system
         types: [python]
```

### Comparing `fsaa-0.0.7/environment.yml` & `fsaa-0.0.8/environment.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/update-version.sh` & `fsaa-0.0.8/update-version.sh`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/.github/workflows/python-publish.yml` & `fsaa-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/.vscode/launch.json` & `fsaa-0.0.8/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/assets/logo.png` & `fsaa-0.0.8/assets/logo.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/fsaa/attack.py` & `fsaa-0.0.8/fsaa/attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/fsaa/core.py` & `fsaa-0.0.8/fsaa/core.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/fsaa/utils.py` & `fsaa-0.0.8/fsaa/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 from fsaa.initializers.random_sign import RandomSignInitializer
 from fsaa.losses.cossim_loss import CosSimLoss
 from fsaa.losses.lpips_loss import LPIPSAlexLoss, LPIPSVGGLoss
 from fsaa.losses.mse_loss import MeanSquaredErrorLoss
 from fsaa.masks.custom import CustomMask
 from fsaa.masks.jnd import JNDMask
 from fsaa.masks.nomask import NoMask
+from fsaa.models.cae.cae import SUPPORTED_CAE_MODELS, CAEModel
 from fsaa.models.hf.hf_models import SUPPORTED_HF_MODELS, HFModel
 from fsaa.models.hub.hub_models import SUPPORTED_HUB_MODELS, HubModel
 from fsaa.models.ibot.ibot import SUPPORTED_IBOT_MODELS, iBOTModel
+from fsaa.models.ijepa.ijepa import IJEPA, SUPPORTED_IJEPA_MODELS
 from fsaa.updaters.fgsm import FGSMUpdater
 from fsaa.updaters.langevin import LangevinUpdater
 from fsaa.updaters.pgd import PGDUpdater
 from fsaa.updaters.random import RandomUpdater
 
 INITIALIZERS = {
     "Random": RandomInitializer,
@@ -40,17 +42,19 @@
 MASKS = {
     "JND": JNDMask,
     "Custom": CustomMask,
     "NoMask": NoMask
 }
 
 SUPPORTED_MODELS = (
+    SUPPORTED_CAE_MODELS +
     SUPPORTED_HUB_MODELS +
     SUPPORTED_HF_MODELS +
-    SUPPORTED_IBOT_MODELS
+    SUPPORTED_IBOT_MODELS +
+    SUPPORTED_IJEPA_MODELS
 )
 
 
 def get_initializer(name: str, lr: float, **kwargs) -> PerturbationInitializer:
     """Returns the initializer used for the attack."""
     return INITIALIZERS[name](lr, **kwargs)
 
@@ -74,15 +78,21 @@
     """Returns the model used for the attack."""
     if model_name not in SUPPORTED_MODELS:
         raise ValueError(
             f"Model '{model_name}' is not supported. \
                 Pick one of {SUPPORTED_MODELS}"
         )
 
+    if model_name in SUPPORTED_CAE_MODELS:
+        return CAEModel(model_name)
+
     if model_name in SUPPORTED_HUB_MODELS:
         return HubModel(model_name)
 
     if model_name in SUPPORTED_HF_MODELS:
         return HFModel(model_name)
 
     if model_name in SUPPORTED_IBOT_MODELS:
         return iBOTModel(model_name)
+
+    if model_name in SUPPORTED_IJEPA_MODELS:
+        return IJEPA(model_name)
```

### Comparing `fsaa-0.0.7/fsaa/examples/tutorial.py` & `fsaa-0.0.8/fsaa/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/fsaa/losses/lpips_loss.py` & `fsaa-0.0.8/fsaa/losses/lpips_loss.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/fsaa/masks/jnd.py` & `fsaa-0.0.8/fsaa/masks/jnd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/fsaa/models/hf/hf_models.py` & `fsaa-0.0.8/fsaa/models/hf/hf_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from torch.nn import Module
 from transformers import AutoModel, logging
 
 from fsaa.attack import TransformAndModelWrapper
-from fsaa.transforms.normalize import (HALF_NORMALIZATION_MEAN,
-                                       HALF_NORMALIZATION_STD, IMAGENET_MEAN,
+from fsaa.transforms.normalize import (IMAGENET_INCEPTION_MEAN,
+                                       IMAGENET_INCEPTION_STD, IMAGENET_MEAN,
                                        IMAGENET_STD, Normalize)
 
 SUPPORTED_BEIT_MODELS = [
-    "microsoft/beit-base-patch16-224",
     "microsoft/beit-base-patch16-224-pt22k",
-    "microsoft/beit-base-patch16-224-pt22k-ft22k",
+    "microsoft/beit-large-patch16-224-pt22k"
 ]
 
 SUPPORTED_DINO_MODELS = [
-    "facebook/dino-vits8",
     "facebook/dino-vits16",
-    "facebook/dino-vitb8",
     "facebook/dino-vitb16",
 ]
 
 SUPPORTED_MAE_MODELS = [
     "facebook/vit-mae-base",
     "facebook/vit-mae-large",
     "facebook/vit-mae-huge",
@@ -61,21 +58,16 @@
                 f"Model '{model_name}' is not supported. \
                 Pick one of {SUPPORTED_BEIT_MODELS}"
             )
 
         hf_model = name_to_model(model_name)
 
         if model_name in SUPPORTED_BEIT_MODELS:
-            mean, std = HALF_NORMALIZATION_MEAN, HALF_NORMALIZATION_STD
-
-        if (
-            model_name in SUPPORTED_DINO_MODELS
-            or model_name in SUPPORTED_MAE_MODELS
-            or model_name in SUPPORTED_MSN_MODELS
-        ):
+            mean, std = IMAGENET_INCEPTION_MEAN, IMAGENET_INCEPTION_STD
+        else:
             mean, std = IMAGENET_MEAN, IMAGENET_STD
 
         self.model = TransformAndModelWrapper(
             hf_model, transform=Normalize(mean, std)
         )
 
     def forward(self, x):
```

### Comparing `fsaa-0.0.7/fsaa/models/hf_models/hf_models.py` & `fsaa-0.0.8/fsaa/models/hub/hub_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,80 @@
+import torch
 from torch.nn import Module
-from transformers import AutoModel, logging
 
 from fsaa.attack import TransformAndModelWrapper
-from fsaa.transforms.normalize import (HALF_NORMALIZATION_MEAN,
-                                       HALF_NORMALIZATION_STD, IMAGENET_MEAN,
-                                       IMAGENET_STD, Normalize)
-
-SUPPORTED_BEIT_MODELS = [
-    "microsoft/beit-base-patch16-224",
-    "microsoft/beit-base-patch16-224-pt22k",
-    "microsoft/beit-base-patch16-224-pt22k-ft22k",
+from fsaa.transforms.normalize import IMAGENET_MEAN, IMAGENET_STD, Normalize
+
+SUPPORTED_BARLOWTWINS_MODELS = [
+    "barlowtwins_resnet50",
 ]
 
-SUPPORTED_DINO_MODELS = [
-    "facebook/dino-vits8",
-    "facebook/dino-vits16",
-    "facebook/dino-vitb8",
-    "facebook/dino-vitb16",
+SUPPORTED_DINOV2_MODELS = [
+    "dinov2_vits14",
+    "dinov2_vitb14",
+    "dinov2_vitl14",
+    "dinov2_vitg14",
 ]
 
-SUPPORTED_MAE_MODELS = [
-    "facebook/vit-mae-base",
-    "facebook/vit-mae-large",
-    "facebook/vit-mae-huge",
+SUPPORTED_SWAV_MODELS = [
+    "swav_resnet50",
+    "swav_resnet50w2",
+    "swav_resnet50w4",
+    "swav_resnet50w5",
 ]
 
-SUPPORTED_MSN_MODELS = [
-    "facebook/vit-msn-small",
-    "facebook/vit-msn-base",
-    "facebook/vit-msn-large"
+SUPPORTED_VICREG_MODELS = [
+    "vicreg_resnet50",
+    "vicreg_resnet50x2",
+    "vicreg_resnet200x2"
 ]
 
-SUPPORTED_HF_MODELS = (
-    SUPPORTED_BEIT_MODELS
-    + SUPPORTED_DINO_MODELS
-    + SUPPORTED_MAE_MODELS
-    + SUPPORTED_MSN_MODELS
+SUPPORTED_HUB_MODELS = (
+    SUPPORTED_BARLOWTWINS_MODELS +
+    SUPPORTED_DINOV2_MODELS +
+    SUPPORTED_SWAV_MODELS +
+    SUPPORTED_VICREG_MODELS
 )
 
 
-def name_to_model(model_name: str):
-    """Returns the model from the given name."""
-    logging.set_verbosity_error()
-    model = AutoModel.from_pretrained(model_name)
-
-    if model_name in SUPPORTED_MAE_MODELS:
-        model.embeddings.config.mask_ratio = 0
-
-    logging.set_verbosity_warning()
-    return model
-
-
-class HFModel(Module):
+class HubModel(Module):
     """Base class for all feature extractors."""
 
     def __init__(self, model_name):
-        super(HFModel, self).__init__()
-        if model_name not in SUPPORTED_HF_MODELS:
+        super(HubModel, self).__init__()
+        if model_name not in SUPPORTED_HUB_MODELS:
             raise ValueError(
                 f"Model '{model_name}' is not supported. \
-                Pick one of {SUPPORTED_BEIT_MODELS}"
+                Pick one of {SUPPORTED_HUB_MODELS}"
             )
 
-        hf_model = name_to_model(model_name)
-
-        if model_name in SUPPORTED_BEIT_MODELS:
-            mean, std = HALF_NORMALIZATION_MEAN, HALF_NORMALIZATION_STD
-
-        if (
-            model_name in SUPPORTED_DINO_MODELS
-            or model_name in SUPPORTED_MAE_MODELS
-            or model_name in SUPPORTED_MSN_MODELS
-        ):
-            mean, std = IMAGENET_MEAN, IMAGENET_STD
+        if model_name in SUPPORTED_BARLOWTWINS_MODELS:
+            hub_model = torch.hub.load("facebookresearch/barlowtwins:main",
+                                       model_name.split("_")[1],
+                                       verbose=False)
+
+        if model_name in SUPPORTED_DINOV2_MODELS:
+            hub_model = torch.hub.load("facebookresearch/dinov2",
+                                       model_name,
+                                       verbose=False)
+
+        if model_name in SUPPORTED_SWAV_MODELS:
+            hub_model = torch.hub.load("facebookresearch/swav:main",
+                                       model_name.split("_")[1],
+                                       verbose=False)
+
+        if model_name in SUPPORTED_VICREG_MODELS:
+            hub_model = torch.hub.load('facebookresearch/vicreg:main',
+                                       model_name.split("_")[1],
+                                       verbose=False)
+
+        # Removing classification head if any
+        if hasattr(hub_model, "fc"):
+            hub_model.fc = torch.nn.Identity()
 
         self.model = TransformAndModelWrapper(
-            hf_model, transform=Normalize(mean, std)
+            hub_model,
+            transform=Normalize(IMAGENET_MEAN, IMAGENET_STD)
         )
 
     def forward(self, x):
-        """Runs the given batch through the model to extract features."""
-        return self.model(x)["last_hidden_state"][:, 0, :]
+        return self.model(x)
```

### Comparing `fsaa-0.0.7/fsaa/models/ibot/ibot.py` & `fsaa-0.0.8/fsaa/models/ibot/ibot.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,30 +2,24 @@
 import os
 
 import torch
 import torch.nn as nn
 import wget
 
 from fsaa.attack import TransformAndModelWrapper
-from fsaa.models.ibot.vits import vit_base, vit_large, vit_small
+from fsaa.models.ibot.vits import vit_base, vit_large
 from fsaa.transforms.normalize import IMAGENET_MEAN, IMAGENET_STD, Normalize
 
 SUPPORTED_IBOT_MODELS = [
-    "ibot_vits_16",
-    "ibot_vitb_16",
     "ibot_vitb_16_pt22k",
-    "ibot_vitl_16",
-    "ibot_vitl_16_pt22k",
+    "ibot_vitl_16_pt22k"
 ]
 
 NAMES_TO_MODELS = {
-    "ibot_vits_16": vit_small,
-    "ibot_vitb_16": vit_base,
     "ibot_vitb_16_pt22k": lambda: vit_base(masked_im_modeling=True),
-    "ibot_vitl_16": vit_large,
     "ibot_vitl_16_pt22k": lambda: vit_large(masked_im_modeling=True)
 }
 
 
 def model_name_to_url(model_name: str):
     name = model_name.split("ibot_")[1]
     prefix = "https://lf3-nlp-opensource.bytetos.com"
```

### Comparing `fsaa-0.0.7/fsaa/models/ibot/utils.py` & `fsaa-0.0.8/fsaa/models/ibot/utils.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/fsaa/models/ibot/vits.py` & `fsaa-0.0.8/fsaa/models/ibot/vits.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/fsaa/transforms/normalize.py` & `fsaa-0.0.8/fsaa/transforms/normalize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from warnings import warn
 
 from torch import Tensor
 from torchvision.transforms import Normalize as TorchNormalize
 
 from fsaa.core import DifferentiableTransform
 
-HALF_NORMALIZATION_MEAN = [0.5, 0.5, 0.5]
-HALF_NORMALIZATION_STD = [0.5, 0.5, 0.5]
+IMAGENET_INCEPTION_MEAN = [0.5, 0.5, 0.5]
+IMAGENET_INCEPTION_STD = [0.5, 0.5, 0.5]
 
 IMAGENET_MEAN = [0.485, 0.456, 0.406]
 IMAGENET_STD = [0.229, 0.224, 0.225]
 
 OPENAI_NORMALIZATION_MEAN = [0.48145466, 0.4578275, 0.40821073]
 OPENAI_NORMALIZATION_STD = [0.26862954, 0.26130258, 0.27577711]
```

### Comparing `fsaa-0.0.7/fsaa/updaters/langevin.py` & `fsaa-0.0.8/fsaa/updaters/langevin.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/fsaa/updaters/pgd.py` & `fsaa-0.0.8/fsaa/updaters/pgd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/fsaa/updaters/random.py` & `fsaa-0.0.8/fsaa/updaters/random.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/imgs/adv.png` & `fsaa-0.0.8/imgs/adv.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/imgs/mask.png` & `fsaa-0.0.8/imgs/mask.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/imgs/orig.png` & `fsaa-0.0.8/imgs/orig.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/tests/test_attack.py` & `fsaa-0.0.8/tests/test_attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/tests/test_initializers.py` & `fsaa-0.0.8/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/tests/test_masks.py` & `fsaa-0.0.8/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/tests/test_models.py` & `fsaa-0.0.8/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/tests/test_updaters.py` & `fsaa-0.0.8/tests/test_updaters.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/.gitignore` & `fsaa-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/LICENSE` & `fsaa-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.7/README.md` & `fsaa-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 ```
 @software{Pulfer_FSAA_2023,
 author = {Pulfer, Brian},
 month = jul,
 title = {{FSAA}},
 url = {https://github.com/BrianPulfer/fsaa},
-version = {0.0.7},
+version = {0.0.8},
 year = {2023}
 }
 ```
 ___
 
 ## Acknowledgements
 Part of the code was taken and adapted from the following repositories:
```

### Comparing `fsaa-0.0.7/pyproject.toml` & `fsaa-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # Project metadata
 [project]
 name = "fsaa"
-version = "0.0.7"
+version = "0.0.8"
 authors = [{ name="Brian Pulfer", email="brianpulfer95@gmail.com" }]
 description = "A simple library for adversarial attacks in feature space."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
```

### Comparing `fsaa-0.0.7/PKG-INFO` & `fsaa-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsaa
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple library for adversarial attacks in feature space.
 Project-URL: Homepage, https://github.com/BrianPulfer/fsaa
 Project-URL: Bug Tracker, https://github.com/BrianPulfer/fsaa/issues
 Author-email: Brian Pulfer <brianpulfer95@gmail.com>
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -136,15 +136,15 @@
 
 ```
 @software{Pulfer_FSAA_2023,
 author = {Pulfer, Brian},
 month = jul,
 title = {{FSAA}},
 url = {https://github.com/BrianPulfer/fsaa},
-version = {0.0.7},
+version = {0.0.8},
 year = {2023}
 }
 ```
 ___
 
 ## Acknowledgements
 Part of the code was taken and adapted from the following repositories:
```

