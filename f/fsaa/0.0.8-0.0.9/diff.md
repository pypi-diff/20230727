# Comparing `tmp/fsaa-0.0.8.tar.gz` & `tmp/fsaa-0.0.9.tar.gz`

## Comparing `fsaa-0.0.8.tar` & `fsaa-0.0.9.tar`

### file list

```diff
@@ -1,62 +1,64 @@
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fsaa-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.8/CITATION.cff
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.8/CODEOWNERS
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.8/environment.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fsaa-0.0.8/requirements.txt
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fsaa-0.0.8/update-version.sh
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.8/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.8/assets/logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/attack.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/core.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/utils.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/examples/tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/initializers/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/initializers/random.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/initializers/random_sign.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/losses/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/losses/cossim_loss.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/losses/lpips_loss.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/losses/mse_loss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/masks/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/masks/custom.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/masks/jnd.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/masks/nomask.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/cae/__init__.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/cae/cae.py
--rw-r--r--   0        0        0    24969 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/cae/modeling_finetune.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/cae/utils.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/hf/hf_models.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/hub/hub_models.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/ibot/ibot.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/ibot/utils.py
--rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/ibot/vits.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/ijepa/ijepa.py
--rw-r--r--   0        0        0    20548 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/models/ijepa/vision_transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/transforms/__init__.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/transforms/compose.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/transforms/normalize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/updaters/__init__.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/updaters/fgsm.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/updaters/langevin.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/updaters/pgd.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.8/fsaa/updaters/random.py
--rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.8/imgs/adv.png
--rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.8/imgs/mask.png
--rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.8/imgs/orig.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_attack.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_initializers.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_masks.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_models.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_transforms.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.8/tests/test_updaters.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.8/.gitignore
--rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.8/LICENSE
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.8/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fsaa-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 fsaa-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fsaa-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.9/CITATION.cff
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.9/CODEOWNERS
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.9/environment.yml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 fsaa-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fsaa-0.0.9/update-version.sh
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.9/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.9/assets/logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/attack.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/core.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/examples/tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/initializers/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/initializers/random.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/initializers/random_sign.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/losses/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/losses/cossim_loss.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/losses/lpips_loss.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/losses/mse_loss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/masks/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/masks/custom.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/masks/jnd.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/masks/nomask.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/cae/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/cae/cae.py
+-rw-r--r--   0        0        0    24969 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/cae/modeling_finetune.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/cae/utils.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/hf/hf_models.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/hub/hub_models.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/ibot/ibot.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/ibot/utils.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/ibot/vits.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/ijepa/ijepa.py
+-rw-r--r--   0        0        0    20548 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/models/ijepa/vision_transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/transforms/__init__.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/transforms/compose.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/transforms/normalize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/updaters/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/updaters/fgsm.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/updaters/langevin.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/updaters/pgd.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/updaters/random.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/updaters/lr_schedulers/function.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fsaa-0.0.9/fsaa/updaters/lr_schedulers/linear.py
+-rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.9/imgs/adv.png
+-rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.9/imgs/mask.png
+-rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.9/imgs/orig.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.9/tests/test_attack.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.9/tests/test_initializers.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.9/tests/test_masks.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 fsaa-0.0.9/tests/test_models.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.9/tests/test_transforms.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 fsaa-0.0.9/tests/test_updaters.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.9/.gitignore
+-rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.9/README.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 fsaa-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 fsaa-0.0.9/PKG-INFO
```

### Comparing `fsaa-0.0.8/.pre-commit-config.yaml` & `fsaa-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/environment.yml` & `fsaa-0.0.9/environment.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/update-version.sh` & `fsaa-0.0.9/update-version.sh`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/.github/workflows/python-publish.yml` & `fsaa-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/.vscode/launch.json` & `fsaa-0.0.9/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/assets/logo.png` & `fsaa-0.0.9/assets/logo.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/attack.py` & `fsaa-0.0.9/fsaa/attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/core.py` & `fsaa-0.0.9/fsaa/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,34 +13,53 @@
         return self.initialize(x, *args, **kwargs)
 
     @abstractmethod
     def initialize(self, x: Tensor, *args, **kwargs) -> Tensor:
         raise NotImplementedError
 
 
+class Scheduler(ABC):
+    def __init__(self, base_lr: float = 2 / 255, *args, **kwargs):
+        super(Scheduler, self).__init__(*args, **kwargs)
+        self.base_lr = base_lr
+
+    def __call__(self, step: int, steps: int, *args, **kwargs) -> float:
+        return self.get_step_lr(step, steps, *args, **kwargs)
+
+    @abstractmethod
+    def get_step_lr(self, step: int, steps: int, *args, **kwargs) -> float:
+        raise NotImplementedError
+
+
 class PerturbationUpdater(ABC):
-    def __init__(self, lr, *args, **kwargs):
+    def __init__(self, lr, scheduler: Scheduler = None, *args, **kwargs):
         super(PerturbationUpdater, self).__init__()
         self.lr = lr
+        self.scheduler = scheduler
 
     def __call__(
         self,
         x: Tensor,
         grad: Tensor,
         step: int,
         steps: int,
         loss: Tensor,
         *args,
         **kwargs,
     ) -> Tensor:
-        return self.update(x, grad, step, steps, loss, *args, **kwargs)
+        lr = self.lr
+
+        if self.scheduler is not None:
+            lr = self.scheduler(step, steps)
+
+        return self.update(x, grad, lr, step, steps, loss, *args, **kwargs)
 
     @abstractmethod
     def update(
-        self, x: Tensor, grad: Tensor, step: int, steps: int, loss: Tensor
+        self, x: Tensor, grad: Tensor, lr: float, step: int, steps: int, loss: Tensor
     ) -> Tensor:
         raise NotImplementedError
 
 
 class PerceptualMask(ABC):
     def __init__(self, *args, **kwargs):
         super(PerceptualMask, self).__init__()
```

### Comparing `fsaa-0.0.8/fsaa/utils.py` & `fsaa-0.0.9/fsaa/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,56 +13,63 @@
 from fsaa.models.cae.cae import SUPPORTED_CAE_MODELS, CAEModel
 from fsaa.models.hf.hf_models import SUPPORTED_HF_MODELS, HFModel
 from fsaa.models.hub.hub_models import SUPPORTED_HUB_MODELS, HubModel
 from fsaa.models.ibot.ibot import SUPPORTED_IBOT_MODELS, iBOTModel
 from fsaa.models.ijepa.ijepa import IJEPA, SUPPORTED_IJEPA_MODELS
 from fsaa.updaters.fgsm import FGSMUpdater
 from fsaa.updaters.langevin import LangevinUpdater
+from fsaa.updaters.lr_schedulers.function import FunctionScheduler
+from fsaa.updaters.lr_schedulers.linear import LinearScheduler
 from fsaa.updaters.pgd import PGDUpdater
 from fsaa.updaters.random import RandomUpdater
 
 INITIALIZERS = {
     "Random": RandomInitializer,
     "RandomSign": RandomSignInitializer,
 }
 
+SCHEDULERS = {
+    "Function": FunctionScheduler,
+    "Linear": LinearScheduler,
+}
+
 UPDATERS = {
     "FGSM": FGSMUpdater,
     "Langevin": LangevinUpdater,
     "PGD": PGDUpdater,
     "Random": RandomUpdater,
 }
 
 LOSSES = {
     "CosSim": CosSimLoss,
     "MSE": MeanSquaredErrorLoss,
     "LPIPSAlex": LPIPSAlexLoss,
     "LPIPSVGG": LPIPSVGGLoss,
 }
 
-MASKS = {
-    "JND": JNDMask,
-    "Custom": CustomMask,
-    "NoMask": NoMask
-}
+MASKS = {"JND": JNDMask, "Custom": CustomMask, "NoMask": NoMask}
 
 SUPPORTED_MODELS = (
-    SUPPORTED_CAE_MODELS +
-    SUPPORTED_HUB_MODELS +
-    SUPPORTED_HF_MODELS +
-    SUPPORTED_IBOT_MODELS +
-    SUPPORTED_IJEPA_MODELS
+    SUPPORTED_CAE_MODELS
+    + SUPPORTED_HUB_MODELS
+    + SUPPORTED_HF_MODELS
+    + SUPPORTED_IBOT_MODELS
+    + SUPPORTED_IJEPA_MODELS
 )
 
 
 def get_initializer(name: str, lr: float, **kwargs) -> PerturbationInitializer:
     """Returns the initializer used for the attack."""
     return INITIALIZERS[name](lr, **kwargs)
 
 
+def get_scheduler(name: str, base_lr: float, **kwargs) -> PerturbationUpdater:
+    return SCHEDULERS[name](base_lr, **kwargs)
+
+
 def get_updater(name: str, lr: float, **kwargs) -> PerturbationUpdater:
     """Returns the updater used for the attack."""
     return UPDATERS[name](lr, **kwargs)
 
 
 def get_loss(name: str, **kwargs) -> Module:
     """Returns the loss used for the attack."""
```

### Comparing `fsaa-0.0.8/fsaa/examples/tutorial.py` & `fsaa-0.0.9/fsaa/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/losses/lpips_loss.py` & `fsaa-0.0.9/fsaa/losses/lpips_loss.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/masks/jnd.py` & `fsaa-0.0.9/fsaa/masks/jnd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/models/cae/cae.py` & `fsaa-0.0.9/fsaa/models/cae/cae.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/models/cae/modeling_finetune.py` & `fsaa-0.0.9/fsaa/models/cae/modeling_finetune.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/models/cae/utils.py` & `fsaa-0.0.9/fsaa/models/cae/utils.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/models/hf/hf_models.py` & `fsaa-0.0.9/fsaa/models/hf/hf_models.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/models/hub/hub_models.py` & `fsaa-0.0.9/fsaa/models/hub/hub_models.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/models/ibot/ibot.py` & `fsaa-0.0.9/fsaa/models/ibot/ibot.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/models/ibot/utils.py` & `fsaa-0.0.9/fsaa/models/ibot/utils.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/models/ibot/vits.py` & `fsaa-0.0.9/fsaa/models/ibot/vits.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/models/ijepa/ijepa.py` & `fsaa-0.0.9/fsaa/models/ijepa/ijepa.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/models/ijepa/vision_transformer.py` & `fsaa-0.0.9/fsaa/models/ijepa/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/transforms/normalize.py` & `fsaa-0.0.9/fsaa/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/fsaa/updaters/langevin.py` & `fsaa-0.0.9/fsaa/updaters/langevin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import torch
 
-from fsaa.core import PerturbationUpdater
+from fsaa.core import PerturbationUpdater, Scheduler
 
 
 class LangevinUpdater(PerturbationUpdater):
     """Langevin perturbation update."""
 
     def __init__(self,
                  lr: float = 2 / 255,
+                 scheduler: Scheduler = None,
                  eta: float = None,
                  *args,
                  **kwargs):
-        super(LangevinUpdater, self).__init__(lr, *args, **kwargs)
+        super(LangevinUpdater, self).__init__(lr, scheduler, *args, **kwargs)
         self.eta = eta if eta is not None else (2 * self.lr) ** 0.5
 
     def update(
         self,
         x: torch.Tensor,
         grad: torch.Tensor,
+        lr: float,
         step: int,
         steps: int,
         loss: torch.Tensor,
     ) -> torch.Tensor:
         grad_log_loss = grad / loss
-        return x - self.lr * grad_log_loss + self.eta * torch.randn_like(x)
+        return x - lr * grad_log_loss + self.eta * torch.randn_like(x)
```

### Comparing `fsaa-0.0.8/imgs/adv.png` & `fsaa-0.0.9/imgs/adv.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/imgs/mask.png` & `fsaa-0.0.9/imgs/mask.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/imgs/orig.png` & `fsaa-0.0.9/imgs/orig.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/tests/test_attack.py` & `fsaa-0.0.9/tests/test_attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/tests/test_initializers.py` & `fsaa-0.0.9/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/tests/test_masks.py` & `fsaa-0.0.9/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/tests/test_models.py` & `fsaa-0.0.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/.gitignore` & `fsaa-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/LICENSE` & `fsaa-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.8/README.md` & `fsaa-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 ```
 @software{Pulfer_FSAA_2023,
 author = {Pulfer, Brian},
 month = jul,
 title = {{FSAA}},
 url = {https://github.com/BrianPulfer/fsaa},
-version = {0.0.8},
+version = {0.0.9},
 year = {2023}
 }
 ```
 ___
 
 ## Acknowledgements
 Part of the code was taken and adapted from the following repositories:
```

### Comparing `fsaa-0.0.8/pyproject.toml` & `fsaa-0.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # Project metadata
 [project]
 name = "fsaa"
-version = "0.0.8"
+version = "0.0.9"
 authors = [{ name="Brian Pulfer", email="brianpulfer95@gmail.com" }]
 description = "A simple library for adversarial attacks in feature space."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "accelerate",
+    "gdown",
     "lpips",
     "numpy",
+    "pre-commit",
+    "pytest",
+    "timm",
     "torch",
     "torchvision",
     "tqdm",
     "transformers",
     "wget",
     "xformers"
 ]
```

### Comparing `fsaa-0.0.8/PKG-INFO` & `fsaa-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: fsaa
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple library for adversarial attacks in feature space.
 Project-URL: Homepage, https://github.com/BrianPulfer/fsaa
 Project-URL: Bug Tracker, https://github.com/BrianPulfer/fsaa/issues
 Author-email: Brian Pulfer <brianpulfer95@gmail.com>
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: accelerate
+Requires-Dist: gdown
 Requires-Dist: lpips
 Requires-Dist: numpy
+Requires-Dist: pre-commit
+Requires-Dist: pytest
+Requires-Dist: timm
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: tqdm
 Requires-Dist: transformers
 Requires-Dist: wget
 Requires-Dist: xformers
 Description-Content-Type: text/markdown
@@ -136,15 +140,15 @@
 
 ```
 @software{Pulfer_FSAA_2023,
 author = {Pulfer, Brian},
 month = jul,
 title = {{FSAA}},
 url = {https://github.com/BrianPulfer/fsaa},
-version = {0.0.8},
+version = {0.0.9},
 year = {2023}
 }
 ```
 ___
 
 ## Acknowledgements
 Part of the code was taken and adapted from the following repositories:
```

