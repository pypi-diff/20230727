# Comparing `tmp/TorchSUL-0.2.1.tar.gz` & `tmp/TorchSUL-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSUL-0.2.1.tar", last modified: Sun Jul 16 13:17:58 2023, max compression
+gzip compressed data, was "TorchSUL-0.2.3.tar", last modified: Thu Jul 27 12:27:18 2023, max compression
```

## Comparing `TorchSUL-0.2.1.tar` & `TorchSUL-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-16 13:17:58.491801 TorchSUL-0.2.1/
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4038 2023-07-16 13:17:58.489799 TorchSUL-0.2.1/PKG-INFO
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3865 2023-07-16 13:16:20.000000 TorchSUL-0.2.1/README.md
-drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-16 13:17:58.433885 TorchSUL-0.2.1/TorchSUL/
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3920 2023-07-16 13:10:08.000000 TorchSUL-0.2.1/TorchSUL/Base.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      932 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/Config.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    22926 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/Layers.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    15107 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/Model.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    13358 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/Quant.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      260 2023-07-15 09:40:38.000000 TorchSUL-0.2.1/TorchSUL/__init__.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     1912 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/sul_tool.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     6446 2023-07-16 13:09:25.000000 TorchSUL-0.2.1/TorchSUL/sulplotter.py
-drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-16 13:17:58.477697 TorchSUL-0.2.1/TorchSUL.egg-info/
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4038 2023-07-16 13:17:58.000000 TorchSUL-0.2.1/TorchSUL.egg-info/PKG-INFO
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      333 2023-07-16 13:17:58.000000 TorchSUL-0.2.1/TorchSUL.egg-info/SOURCES.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        1 2023-07-16 13:17:58.000000 TorchSUL-0.2.1/TorchSUL.egg-info/dependency_links.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       45 2023-07-16 13:17:58.000000 TorchSUL-0.2.1/TorchSUL.egg-info/requires.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        9 2023-07-16 13:17:58.000000 TorchSUL-0.2.1/TorchSUL.egg-info/top_level.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       38 2023-07-16 13:17:58.491801 TorchSUL-0.2.1/setup.cfg
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      669 2023-07-16 13:12:17.000000 TorchSUL-0.2.1/setup.py
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-27 12:27:18.545262 TorchSUL-0.2.3/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4199 2023-07-27 12:27:18.542263 TorchSUL-0.2.3/PKG-INFO
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4030 2023-07-27 00:49:09.000000 TorchSUL-0.2.3/README.md
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-27 12:27:18.411130 TorchSUL-0.2.3/TorchSUL/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3925 2023-07-27 12:26:40.000000 TorchSUL-0.2.3/TorchSUL/Base.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      932 2023-07-27 00:43:05.000000 TorchSUL-0.2.3/TorchSUL/Config.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    22926 2023-07-16 13:09:25.000000 TorchSUL-0.2.3/TorchSUL/Layers.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    16258 2023-07-27 12:26:40.000000 TorchSUL-0.2.3/TorchSUL/Model.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    13358 2023-07-16 13:09:25.000000 TorchSUL-0.2.3/TorchSUL/Quant.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      260 2023-07-15 09:40:38.000000 TorchSUL-0.2.3/TorchSUL/__init__.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     1912 2023-07-16 13:09:25.000000 TorchSUL-0.2.3/TorchSUL/sul_tool.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     6446 2023-07-16 13:09:25.000000 TorchSUL-0.2.3/TorchSUL/sulplotter.py
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-27 12:27:18.505263 TorchSUL-0.2.3/TorchSUL.egg-info/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4199 2023-07-27 12:27:18.000000 TorchSUL-0.2.3/TorchSUL.egg-info/PKG-INFO
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      333 2023-07-27 12:27:18.000000 TorchSUL-0.2.3/TorchSUL.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        1 2023-07-27 12:27:18.000000 TorchSUL-0.2.3/TorchSUL.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       45 2023-07-27 12:27:18.000000 TorchSUL-0.2.3/TorchSUL.egg-info/requires.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        9 2023-07-27 12:27:18.000000 TorchSUL-0.2.3/TorchSUL.egg-info/top_level.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       38 2023-07-27 12:27:18.546263 TorchSUL-0.2.3/setup.cfg
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      669 2023-07-27 12:27:03.000000 TorchSUL-0.2.3/setup.py
```

### Comparing `TorchSUL-0.2.1/PKG-INFO` & `TorchSUL-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchSUL
-Version: 0.2.1
+Version: 0.2.3
 Summary: Simple but useful layers for Pytorch
 Home-page: https://github.com/ddddwee1/TorchSUL
 Author: Cheng Yu
 Author-email: chengyu996@gmail.com
 Description-Content-Type: text/markdown
 
 # TorchSUL
@@ -29,20 +29,24 @@
 
 ```
 pip install --upgrade torchsul
 ```
 
 ## Patch Notes
 
-#### 2023-07-16:  Bugfixes 
+#### 2023-07-27 (0.2.2)
+1. Add support for loading standard pytorch state dict. Users can set "from_torch" flag to load from standard pytorch state dict.
+
+
+#### 2023-07-16:  Bugfixes (0.2.1)
 1. Now *M.Model.\_laod_from_state_dict2* can normally manipulate state dictionary of its child modules 
 2. Add quantization support for fc layers. 
 
 
-#### 2023-07-15:  Upgrade to 0.2.0. 
+#### 2023-07-15:  Upgrade to 0.2.0
 1. This is acually a pruning of previous version, where many redundant and outdated modules/functions are removed. You may find some layers are not supported anymore because there should be a convenient pytorch equivalance to be used. 
 2. This package is reformed since version 0.2.0. The submodule "DataReader" and "sulio" are removed, and all codes which utilizes these submodules will *no longer be supported*. It is recommended to use pytorch's dataloader for reading data. 
 3. Add config module to handle configs from yaml files. One the one hand, it's easier to control experiments from outside; on the other hand, build-in configs will prettify the codes.
 4. Remove caffe conversion support in package as it's redundant. One can use external method to build caffe converter (e.g, forward hooks) to convert models. As an alternative, the caffe conversion codes (modified Models & layers.py) still remain in examples.
```

### Comparing `TorchSUL-0.2.1/README.md` & `TorchSUL-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,24 @@
 
 ```
 pip install --upgrade torchsul
 ```
 
 ## Patch Notes
 
-#### 2023-07-16:  Bugfixes 
+#### 2023-07-27 (0.2.2)
+1. Add support for loading standard pytorch state dict. Users can set "from_torch" flag to load from standard pytorch state dict.
+
+
+#### 2023-07-16:  Bugfixes (0.2.1)
 1. Now *M.Model.\_laod_from_state_dict2* can normally manipulate state dictionary of its child modules 
 2. Add quantization support for fc layers. 
 
 
-#### 2023-07-15:  Upgrade to 0.2.0. 
+#### 2023-07-15:  Upgrade to 0.2.0
 1. This is acually a pruning of previous version, where many redundant and outdated modules/functions are removed. You may find some layers are not supported anymore because there should be a convenient pytorch equivalance to be used. 
 2. This package is reformed since version 0.2.0. The submodule "DataReader" and "sulio" are removed, and all codes which utilizes these submodules will *no longer be supported*. It is recommended to use pytorch's dataloader for reading data. 
 3. Add config module to handle configs from yaml files. One the one hand, it's easier to control experiments from outside; on the other hand, build-in configs will prettify the codes.
 4. Remove caffe conversion support in package as it's redundant. One can use external method to build caffe converter (e.g, forward hooks) to convert models. As an alternative, the caffe conversion codes (modified Models & layers.py) still remain in examples.
```

### Comparing `TorchSUL-0.2.1/TorchSUL/Base.py` & `TorchSUL-0.2.3/TorchSUL/Base.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 	def setup_cfg(self):
 		def set_cfg(obj):
 			if hasattr(obj, 'cfg'):
 				obj.cfg = self.cfg 
 		self.apply(set_cfg)
 
-	def set_flag(self, k, v):
+	def set_flag(self, k, v=True):
 		def set_model_flag(obj):
 			if hasattr(obj, '_model_flags'):
 				obj._model_flags[k] = v 
 		self.apply(set_model_flag)
 
 	def get_flag(self, k):
 		return self._model_flags.get(k, None)
```

### Comparing `TorchSUL-0.2.1/TorchSUL/Config.py` & `TorchSUL-0.2.3/TorchSUL/Config.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.1/TorchSUL/Layers.py` & `TorchSUL-0.2.3/TorchSUL/Layers.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.1/TorchSUL/Model.py` & `TorchSUL-0.2.3/TorchSUL/Model.py`

 * *Files 7% similar despite different names*

```diff
@@ -183,25 +183,53 @@
 		if self.batch_norm:
 			bn = self.bn.to_torch()
 			setattr(self, 'bn', bn)
 		if self.activation==PARAM_RELU:
 			relu = nn.ReLU()
 			setattr(self, 'act', relu)
 
-	def _load_from_state_dict(self, state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs):
-		super()._load_from_state_dict(state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs)
-		if (self.get_flag('fc2conv')) and ((prefix + 'fc.weight') in state_dict):
-			w = state_dict.pop(prefix+'fc.weight').unsqueeze(-1).unsqueeze(-1)
-			state_dict[prefix+'conv.weight'] = w 
+	def _load_from_state_dict2(self, state_dict, prefix):
+		def _load_weight(k):
+			if not k in state_dict:
+				raise Exception('Attenpt to find', k, 'but only exist', state_dict.keys(), '\nCannot find weight in checkpoint for layer:', prefix)
+			return state_dict.pop(k)
+		def _load_bias(k):
 			if self.conv.usebias:
-				if prefix+'fc.bias' in state_dict:
-					b = state_dict.pop(prefix+'fc.bias')
-					state_dict[prefix+'conv.bias'] = b
+				try:
+					b = state_dict.pop(k)
+				except:
+					raise Exception('Attenpt to find', k, 'but only exist', state_dict.keys(), '\nBias is set for layer', prefix, 'but not found in checkpoint. \nTry to set usebias=False to fix this problem')
 			else:
-				raise Exception('Bias not found for layer', prefix, '\nTry to set usebias=False to fix this problem')
+				b = None
+			return b 
+
+		# get names for params
+		if prefix+'conv.weight' in state_dict:
+			# normal load 
+			w = prefix + 'conv.weight'
+			b = prefix + 'conv.bias'
+		elif self.get_flag('fc2conv') and ((prefix+'fc.weight') in state_dict):
+			w = prefix + 'fc.weight'
+			b = prefix + 'fc.bias'
+		elif self.get_flag('from_torch'):
+			w = prefix + 'weight'
+			b = prefix + 'bias'
+		else:
+			raise Exception('Cannot find weight in checkpoint for layer:', prefix)
+
+		# laod weight and bias 
+		w = _load_weight(w)
+		b = _load_bias(b)
+		if self.get_flag('fc2conv') and len(w.shape)==2:
+			w = w.unsqueeze(-1).unsqueeze(-1)
+
+		# write processed params to state dict 
+		state_dict[prefix+'conv.weight'] = w 
+		if b is not None:
+			state_dict[prefix+'conv.bias'] = b
 
 
 class DeConvLayer(Model):
 	def initialize(self, size, outchn, stride=1, pad='SAME_LEFT', dilation_rate=1, activation=-1, batch_norm=False, affine=True, usebias=True, groups=1):
 		self.conv = L.deconv2D(size, outchn, stride, pad, dilation_rate, usebias, groups)
 		if batch_norm:
 			self.bn = L.BatchNorm(affine=affine)
@@ -335,14 +363,29 @@
 		if self.batch_norm:
 			bn = self.bn.to_torch()
 			setattr(self, 'bn', bn)
 		if self.activation==PARAM_RELU:
 			relu = nn.ReLU()
 			setattr(self, 'act', relu)
 
+	def _load_from_state_dict2(self, state_dict, prefix):
+		if self.get_flag('from_torch'):
+			w = state_dict.pop(prefix + 'weight')
+			if self.fc.usebias:
+				try:
+					b = state_dict.pop(prefix + 'bias')
+				except:
+					raise Exception('Bias is set for layer', prefix, 'but not found in checkpoint. \nTry to set usebias=False to fix this problem')
+			else:
+				b = None
+
+			state_dict[prefix+'fc.weight'] = w
+			if b is not None: 
+				state_dict[prefix+'fc.bias'] = b
+
 
 class LSTMCell(Model):
 	def initialize(self, outdim):
 		self.F = L.fcLayer(outdim, usebias=False, norm=False)
 		self.O = L.fcLayer(outdim, usebias=False, norm=False)
 		self.I = L.fcLayer(outdim, usebias=False, norm=False)
 		self.C = L.fcLayer(outdim, usebias=False, norm=False)
```

### Comparing `TorchSUL-0.2.1/TorchSUL/Quant.py` & `TorchSUL-0.2.3/TorchSUL/Quant.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.1/TorchSUL/sul_tool.py` & `TorchSUL-0.2.3/TorchSUL/sul_tool.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.1/TorchSUL/sulplotter.py` & `TorchSUL-0.2.3/TorchSUL/sulplotter.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.1/TorchSUL.egg-info/PKG-INFO` & `TorchSUL-0.2.3/TorchSUL.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchSUL
-Version: 0.2.1
+Version: 0.2.3
 Summary: Simple but useful layers for Pytorch
 Home-page: https://github.com/ddddwee1/TorchSUL
 Author: Cheng Yu
 Author-email: chengyu996@gmail.com
 Description-Content-Type: text/markdown
 
 # TorchSUL
@@ -29,20 +29,24 @@
 
 ```
 pip install --upgrade torchsul
 ```
 
 ## Patch Notes
 
-#### 2023-07-16:  Bugfixes 
+#### 2023-07-27 (0.2.2)
+1. Add support for loading standard pytorch state dict. Users can set "from_torch" flag to load from standard pytorch state dict.
+
+
+#### 2023-07-16:  Bugfixes (0.2.1)
 1. Now *M.Model.\_laod_from_state_dict2* can normally manipulate state dictionary of its child modules 
 2. Add quantization support for fc layers. 
 
 
-#### 2023-07-15:  Upgrade to 0.2.0. 
+#### 2023-07-15:  Upgrade to 0.2.0
 1. This is acually a pruning of previous version, where many redundant and outdated modules/functions are removed. You may find some layers are not supported anymore because there should be a convenient pytorch equivalance to be used. 
 2. This package is reformed since version 0.2.0. The submodule "DataReader" and "sulio" are removed, and all codes which utilizes these submodules will *no longer be supported*. It is recommended to use pytorch's dataloader for reading data. 
 3. Add config module to handle configs from yaml files. One the one hand, it's easier to control experiments from outside; on the other hand, build-in configs will prettify the codes.
 4. Remove caffe conversion support in package as it's redundant. One can use external method to build caffe converter (e.g, forward hooks) to convert models. As an alternative, the caffe conversion codes (modified Models & layers.py) still remain in examples.
```

### Comparing `TorchSUL-0.2.1/setup.py` & `TorchSUL-0.2.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup_args = dict(
     name='TorchSUL',
-    version='0.2.1',
+    version='0.2.3',
     description='Simple but useful layers for Pytorch',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Cheng Yu',
     author_email='chengyu996@gmail.com',
     url='https://github.com/ddddwee1/TorchSUL',
```

